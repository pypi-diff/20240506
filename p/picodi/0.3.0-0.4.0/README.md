# Comparing `tmp/picodi-0.3.0.tar.gz` & `tmp/picodi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picodi-0.3.0.tar", max compression
+gzip compressed data, was "picodi-0.4.0.tar", max compression
```

## Comparing `picodi-0.3.0.tar` & `picodi-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-04-24 17:01:52.125412 picodi-0.3.0/LICENSE
--rw-r--r--   0        0        0     6769 2024-04-24 17:01:52.125412 picodi-0.3.0/README.md
--rw-r--r--   0        0        0      173 2024-04-24 17:01:52.125412 picodi-0.3.0/picodi/__init__.py
--rw-r--r--   0        0        0     7874 2024-04-24 17:01:52.125412 picodi-0.3.0/picodi/picodi.py
--rw-r--r--   0        0        0        0 2024-04-24 17:01:52.125412 picodi-0.3.0/picodi/py.typed
--rw-r--r--   0        0        0     4190 2024-04-24 17:01:52.125412 picodi-0.3.0/picodi/scopes.py
--rw-r--r--   0        0        0     2583 2024-04-24 17:01:52.125412 picodi-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7480 1970-01-01 00:00:00.000000 picodi-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-05 18:24:12.943397 picodi-0.4.0/LICENSE
+-rw-r--r--   0        0        0     6769 2024-05-05 18:24:12.943397 picodi-0.4.0/README.md
+-rw-r--r--   0        0        0      265 2024-05-05 18:24:12.943397 picodi-0.4.0/picodi/__init__.py
+-rw-r--r--   0        0        0     8665 2024-05-05 18:24:12.943397 picodi-0.4.0/picodi/picodi.py
+-rw-r--r--   0        0        0        0 2024-05-05 18:24:12.943397 picodi-0.4.0/picodi/py.typed
+-rw-r--r--   0        0        0     4190 2024-05-05 18:24:12.943397 picodi-0.4.0/picodi/scopes.py
+-rw-r--r--   0        0        0     2583 2024-05-05 18:24:12.943397 picodi-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7531 1970-01-01 00:00:00.000000 picodi-0.4.0/PKG-INFO
```

### Comparing `picodi-0.3.0/LICENSE` & `picodi-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picodi-0.3.0/README.md` & `picodi-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `picodi-0.3.0/picodi/picodi.py` & `picodi-0.4.0/picodi/picodi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 import asyncio
 import functools
 import inspect
 import threading
-from collections.abc import Awaitable, Callable, Coroutine
+from collections.abc import Awaitable, Callable
 from contextlib import asynccontextmanager, contextmanager
 from dataclasses import dataclass, field
+from functools import wraps
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncContextManager,
     ContextManager,
     ParamSpec,
     TypeVar,
@@ -55,20 +56,20 @@
         print("closing db connection")
 
     @inject
     def my_service(db: str = Provide(get_db)):
         assert db == "db connection"
     ```
     """
-    if not getattr(dependency, "_scope_", None):
-        dependency._scope_ = "null"  # type: ignore[attr-defined] # noqa: SF01
+    if not getattr(dependency, "_picodi_scope_", None):
+        dependency._picodi_scope_ = "null"  # type: ignore[attr-defined] # noqa: SF01
     return Depends.from_dependency(dependency)
 
 
-def inject(fn: Callable[P, T]) -> Callable[P, T | Coroutine[Any, Any, T]]:
+def inject(fn: Callable[P, T]) -> Callable[P, T]:
     """
     Decorator to inject dependencies into a function.
     Use it in combination with `Provide` to declare dependencies.
 
     Example:
     ```
     from picodi import inject, Provide
@@ -107,28 +108,29 @@
 
             with ExitStack() as stack:
                 for scope in _scopes.values():
                     stack.enter_context(scope, sync_first=True)
                 result = fn(*bound.args, **bound.kwargs)
             return result
 
-    return wrapper
+    wrapper._picodi_inject_ = True  # type: ignore[attr-defined] # noqa: SF01
+    return wrapper  # type: ignore[return-value]
 
 
 def resource(fn: TC) -> TC:
     """
     Decorator to declare a resource. Resource is a dependency that should be
     called only once, cached and shared across the application.
     On shutdown, all resources will be closed
     (you need to call `shutdown_resources` manually).
     Use it with a dependency generator function to declare a resource.
     """
     if not inspect.isgeneratorfunction(fn) and not inspect.isasyncgenfunction(fn):
         raise TypeError("Resource should be a generator function")
-    fn._scope_ = "singleton"  # type: ignore[attr-defined] # noqa: SF01
+    fn._picodi_scope_ = "singleton"  # type: ignore[attr-defined] # noqa: SF01
     with _lock:
         _resources.append(Depends.from_dependency(fn))
     return fn
 
 
 def init_resources() -> Awaitable | None:
     """
@@ -157,14 +159,32 @@
         return asyncio.gather(*tasks)  # type: ignore[arg-type]
 
     for scope in _scopes.values():
         scope.exit_stack.close(only_sync=True)
     return None
 
 
+def make_dependency(fn: Callable[P, T], *args: Any, **kwargs: Any) -> Callable[..., T]:
+    signature = inspect.signature(fn)
+    bound = signature.bind(*args, **kwargs)
+    bound.apply_defaults()
+
+    has_deps = any(isinstance(value, Depends) for value in bound.arguments.values())
+    if not getattr(fn, "_picodi_inject_", None) and has_deps:
+        fn = inject(fn)
+
+    @wraps(fn)
+    def wrapper(*args_in: P.args, **kwargs_in: P.kwargs) -> T:
+        bound_inner = signature.bind_partial(*args_in, **kwargs_in)
+        bound.arguments.update(bound_inner.arguments)
+        return fn(*bound.args, **bound.kwargs)
+
+    return wrapper
+
+
 CallableManager = Callable[..., AsyncContextManager | ContextManager]
 
 
 @dataclass(frozen=True)
 class Depends:
     dependency: Dependency
     context_manager: CallableManager | None = field(compare=False)
@@ -179,15 +199,17 @@
             is_async = True
         elif inspect.isgeneratorfunction(dependency):
             context_manager = contextmanager(dependency)
 
         return cls(dependency, context_manager, is_async)
 
     def get_scope(self) -> Scope:
-        scope_name = self.dependency._scope_  # type: ignore[attr-defined] # noqa: SF01
+        scope_name = (
+            self.dependency._picodi_scope_  # type: ignore[attr-defined] # noqa: SF01
+        )
         return _scopes[scope_name]
 
     def resolve_value(self) -> Any:
         scope = self.get_scope()
         if self.context_manager:
             return scope.exit_stack.enter_context(self.context_manager())
         return self.dependency()
```

### Comparing `picodi-0.3.0/picodi/scopes.py` & `picodi-0.4.0/picodi/scopes.py`

 * *Files identical despite different names*

### Comparing `picodi-0.3.0/pyproject.toml` & `picodi-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "picodi"
 description = "Simple Dependency Injection for Python"
-version = "0.3.0"
+version = "0.4.0"
 license = "MIT"
 authors = [
   "yakimka"
 ]
 
 readme = "README.md"
```

### Comparing `picodi-0.3.0/PKG-INFO` & `picodi-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: picodi
-Version: 0.3.0
+Version: 0.4.0
 Summary: Simple Dependency Injection for Python
 Home-page: https://github.com/yakimka/picodi
 License: MIT
 Author: yakimka
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Repository, https://github.com/yakimka/picodi
 Description-Content-Type: text/markdown
 
 # Picodi - Python DI (Dependency Injection) Library
 
 [![Build Status](https://github.com/yakimka/picodi/actions/workflows/workflow-ci.yml/badge.svg?branch=main&event=push)](https://github.com/yakimka/picodi/actions/workflows/workflow-ci.yml)
```

