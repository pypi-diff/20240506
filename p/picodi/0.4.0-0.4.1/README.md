# Comparing `tmp/picodi-0.4.0.tar.gz` & `tmp/picodi-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picodi-0.4.0.tar", max compression
+gzip compressed data, was "picodi-0.4.1.tar", max compression
```

## Comparing `picodi-0.4.0.tar` & `picodi-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-05-05 18:24:12.943397 picodi-0.4.0/LICENSE
--rw-r--r--   0        0        0     6769 2024-05-05 18:24:12.943397 picodi-0.4.0/README.md
--rw-r--r--   0        0        0      265 2024-05-05 18:24:12.943397 picodi-0.4.0/picodi/__init__.py
--rw-r--r--   0        0        0     8665 2024-05-05 18:24:12.943397 picodi-0.4.0/picodi/picodi.py
--rw-r--r--   0        0        0        0 2024-05-05 18:24:12.943397 picodi-0.4.0/picodi/py.typed
--rw-r--r--   0        0        0     4190 2024-05-05 18:24:12.943397 picodi-0.4.0/picodi/scopes.py
--rw-r--r--   0        0        0     2583 2024-05-05 18:24:12.943397 picodi-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7531 1970-01-01 00:00:00.000000 picodi-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-05 22:05:55.904464 picodi-0.4.1/LICENSE
+-rw-r--r--   0        0        0     6787 2024-05-05 22:05:55.904464 picodi-0.4.1/README.md
+-rw-r--r--   0        0        0      265 2024-05-05 22:05:55.904464 picodi-0.4.1/picodi/__init__.py
+-rw-r--r--   0        0        0     8895 2024-05-05 22:05:55.904464 picodi-0.4.1/picodi/picodi.py
+-rw-r--r--   0        0        0        0 2024-05-05 22:05:55.904464 picodi-0.4.1/picodi/py.typed
+-rw-r--r--   0        0        0     4190 2024-05-05 22:05:55.908464 picodi-0.4.1/picodi/scopes.py
+-rw-r--r--   0        0        0     2583 2024-05-05 22:05:55.908464 picodi-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7549 1970-01-01 00:00:00.000000 picodi-0.4.1/PKG-INFO
```

### Comparing `picodi-0.4.0/LICENSE` & `picodi-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `picodi-0.4.0/README.md` & `picodi-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 ## Using picodi with web frameworks
 
 Picodi can be used with web frameworks like FastAPI or Django.
 
 ```python
 import random
 
-from fastapi import FastAPI
+from fastapi import FastAPI, Depends
 from picodi import Provide, inject
 
 app = FastAPI()
 
 
 def get_random_int():
     yield random.randint(1, 100)
@@ -220,15 +220,15 @@
 @inject
 async def get_redis_connection(port: int = Provide(get_random_int)) -> str:
     return "http://redis:{}".format(port)
 
 
 @app.get("/")
 @inject
-async def read_root(redis: str = Provide(get_redis_connection)):
+async def read_root(redis: str = Depends(Provide(get_redis_connection))):
     return {"redis": redis}
 
 
 # uvicorn fastapi_di:app --reload
 ```
 
 ## API Reference
```

### Comparing `picodi-0.4.0/picodi/picodi.py` & `picodi-0.4.1/picodi/picodi.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,20 @@
 )
 
 from picodi.scopes import ExitStack, NullScope, Scope, SingletonScope
 
 if TYPE_CHECKING:
     from inspect import BoundArguments, Signature
 
+try:
+    import fastapi.params
+except ImportError:
+    fastapi = None
+
+
 Dependency = Callable[..., Any]
 T = TypeVar("T")
 P = ParamSpec("P")
 TC = TypeVar("TC", bound=Callable)
 
 
 _unset = object()
@@ -33,14 +39,18 @@
 _lock = threading.RLock()
 _scopes: dict[str, Scope] = {
     "null": NullScope(),
     "singleton": SingletonScope(),
 }
 
 
+def _is_fastapi_dependency(value: Any) -> bool:
+    return bool(fastapi and isinstance(value, fastapi.params.Depends))
+
+
 def Provide(dependency: Dependency, /) -> Any:  # noqa: N802
     """
     Declare a provider.
     It takes a single "dependency" callable (like a function).
     Don't call it directly, picodi will call it for you.
     Dependency can be a regular function or a generator with one yield.
     If the dependency is a generator, it will be used as a context manager.
@@ -164,16 +174,15 @@
 
 
 def make_dependency(fn: Callable[P, T], *args: Any, **kwargs: Any) -> Callable[..., T]:
     signature = inspect.signature(fn)
     bound = signature.bind(*args, **kwargs)
     bound.apply_defaults()
 
-    has_deps = any(isinstance(value, Depends) for value in bound.arguments.values())
-    if not getattr(fn, "_picodi_inject_", None) and has_deps:
+    if not getattr(fn, "_picodi_inject_", None):
         fn = inject(fn)
 
     @wraps(fn)
     def wrapper(*args_in: P.args, **kwargs_in: P.kwargs) -> T:
         bound_inner = signature.bind_partial(*args_in, **kwargs_in)
         bound.arguments.update(bound_inner.arguments)
         return fn(*bound.args, **bound.kwargs)
@@ -210,22 +219,27 @@
 
     def resolve_value(self) -> Any:
         scope = self.get_scope()
         if self.context_manager:
             return scope.exit_stack.enter_context(self.context_manager())
         return self.dependency()
 
+    def __call__(self) -> Depends:
+        return self
+
 
 def _arguments_to_getters(
     args: P.args, kwargs: P.kwargs, signature: Signature, is_async: bool
 ) -> tuple[BoundArguments, dict[str, Callable[[], Any]]]:
     bound = signature.bind(*args, **kwargs)
     bound.apply_defaults()
     dependencies: dict[Depends, list[str]] = {}
     for name, value in bound.arguments.items():
+        if _is_fastapi_dependency(value):
+            value = value.dependency
         if isinstance(value, Depends):
             dependencies.setdefault(value, []).append(name)
 
     get_val = _resolve_value_async if is_async else _resolve_value
 
     dep_arguments = {}
     for depends, names in dependencies.items():
```

### Comparing `picodi-0.4.0/picodi/scopes.py` & `picodi-0.4.1/picodi/scopes.py`

 * *Files identical despite different names*

### Comparing `picodi-0.4.0/pyproject.toml` & `picodi-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "picodi"
 description = "Simple Dependency Injection for Python"
-version = "0.4.0"
+version = "0.4.1"
 license = "MIT"
 authors = [
   "yakimka"
 ]
 
 readme = "README.md"
```

### Comparing `picodi-0.4.0/PKG-INFO` & `picodi-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picodi
-Version: 0.4.0
+Version: 0.4.1
 Summary: Simple Dependency Injection for Python
 Home-page: https://github.com/yakimka/picodi
 License: MIT
 Author: yakimka
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -223,15 +223,15 @@
 ## Using picodi with web frameworks
 
 Picodi can be used with web frameworks like FastAPI or Django.
 
 ```python
 import random
 
-from fastapi import FastAPI
+from fastapi import FastAPI, Depends
 from picodi import Provide, inject
 
 app = FastAPI()
 
 
 def get_random_int():
     yield random.randint(1, 100)
@@ -240,15 +240,15 @@
 @inject
 async def get_redis_connection(port: int = Provide(get_random_int)) -> str:
     return "http://redis:{}".format(port)
 
 
 @app.get("/")
 @inject
-async def read_root(redis: str = Provide(get_redis_connection)):
+async def read_root(redis: str = Depends(Provide(get_redis_connection))):
     return {"redis": redis}
 
 
 # uvicorn fastapi_di:app --reload
 ```
 
 ## API Reference
```

