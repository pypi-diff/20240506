# Comparing `tmp/python_immutable-1.1.0.tar.gz` & `tmp/python_immutable-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_immutable-1.1.0.tar", max compression
+gzip compressed data, was "python_immutable-1.1.1.tar", max compression
```

## Comparing `python_immutable-1.1.0.tar` & `python_immutable-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-05-05 14:38:52.200583 python_immutable-1.1.0/LICENSE
--rw-r--r--   0        0        0     1215 2024-05-05 14:38:52.200583 python_immutable-1.1.0/README.md
--rw-r--r--   0        0        0      186 2024-05-05 14:38:52.200583 python_immutable-1.1.0/immutable/__init__.py
--rw-r--r--   0        0        0     1897 2024-05-05 14:38:52.200583 python_immutable-1.1.0/immutable/main.py
--rw-r--r--   0        0        0     1525 2024-05-05 14:38:52.200583 python_immutable-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 python_immutable-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-06 20:51:17.566305 python_immutable-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1215 2024-05-06 20:51:17.566305 python_immutable-1.1.1/README.md
+-rw-r--r--   0        0        0      186 2024-05-06 20:51:17.566305 python_immutable-1.1.1/immutable/__init__.py
+-rw-r--r--   0        0        0     1963 2024-05-06 20:51:17.566305 python_immutable-1.1.1/immutable/main.py
+-rw-r--r--   0        0        0       69 2024-05-06 20:51:17.566305 python_immutable-1.1.1/immutable/py.typed
+-rw-r--r--   0        0        0     1525 2024-05-06 20:51:17.566305 python_immutable-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 python_immutable-1.1.1/PKG-INFO
```

### Comparing `python_immutable-1.1.0/LICENSE` & `python_immutable-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_immutable-1.1.0/README.md` & `python_immutable-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `python_immutable-1.1.0/immutable/main.py` & `python_immutable-1.1.1/immutable/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 def immutable(cls: type[_T]) -> type[_T]:
     if sys.version_info < (3, 10):
         return dataclass(frozen=True)(cls)  # pragma: no cover
     return dataclass(frozen=True, kw_only=True, eq=False, unsafe_hash=True)(cls)
 
 
 @dataclass_transform(kw_only_default=True, frozen_default=True)
+@dataclass(kw_only=True, frozen=True, eq=False, unsafe_hash=True)
 class Immutable:
     def __init_subclass__(
         cls: type[Immutable],
         *,
         _immutable_applied: bool = False,
         **kwargs: object,
     ) -> None:
```

### Comparing `python_immutable-1.1.0/pyproject.toml` & `python_immutable-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-immutable"
-version = "1.1.0"
+version = "1.1.1"
 description = "Immutable implementation for Python using dataclasses"
 authors = ["Sassan Haradji <sassanh@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "immutable" }]
 
 [tool.poetry.dependencies]
```

### Comparing `python_immutable-1.1.0/PKG-INFO` & `python_immutable-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-immutable
-Version: 1.1.0
+Version: 1.1.1
 Summary: Immutable implementation for Python using dataclasses
 License: Apache-2.0
 Author: Sassan Haradji
 Author-email: sassanh@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

