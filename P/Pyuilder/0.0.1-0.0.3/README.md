# Comparing `tmp/pyuilder-0.0.1.tar.gz` & `tmp/pyuilder-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuilder-0.0.1.tar", last modified: Mon May  6 00:04:17 2024, max compression
+gzip compressed data, was "pyuilder-0.0.3.tar", last modified: Mon May  6 03:37:32 2024, max compression
```

## Comparing `pyuilder-0.0.1.tar` & `pyuilder-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 00:04:17.261508 pyuilder-0.0.1/
--rw-rw-rw-   0        0        0     1094 2024-05-05 15:39:31.000000 pyuilder-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     6130 2024-05-06 00:04:17.258509 pyuilder-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4853 2024-05-05 23:46:08.000000 pyuilder-0.0.1/README.md
--rw-rw-rw-   0        0        0     1928 2024-05-06 00:04:08.000000 pyuilder-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 00:04:17.261508 pyuilder-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 00:04:17.198970 pyuilder-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 00:04:17.255506 pyuilder-0.0.1/src/Pyuilder.egg-info/
--rw-rw-rw-   0        0        0     6130 2024-05-06 00:04:17.000000 pyuilder-0.0.1/src/Pyuilder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-05-06 00:04:17.000000 pyuilder-0.0.1/src/Pyuilder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 00:04:17.000000 pyuilder-0.0.1/src/Pyuilder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-06 00:04:17.000000 pyuilder-0.0.1/src/Pyuilder.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-06 00:04:17.000000 pyuilder-0.0.1/src/Pyuilder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 00:04:17.243971 pyuilder-0.0.1/src/pyuilder/
--rw-rw-rw-   0        0        0      137 2024-05-05 22:27:02.000000 pyuilder-0.0.1/src/pyuilder/__init__.py
--rw-rw-rw-   0        0        0     4157 2024-05-06 00:01:41.000000 pyuilder-0.0.1/src/pyuilder/pyuilder.py
-drwxrwxrwx   0        0        0        0 2024-05-06 00:04:17.251991 pyuilder-0.0.1/test/
--rw-rw-rw-   0        0        0     2557 2024-05-05 22:42:29.000000 pyuilder-0.0.1/test/test_pyuilder.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:37:32.854846 pyuilder-0.0.3/
+-rw-rw-rw-   0        0        0     1094 2024-05-05 15:39:31.000000 pyuilder-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     7058 2024-05-06 03:37:32.853345 pyuilder-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5464 2024-05-06 02:56:55.000000 pyuilder-0.0.3/README.md
+-rw-rw-rw-   0        0        0     2081 2024-05-06 03:27:07.000000 pyuilder-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 03:37:32.854846 pyuilder-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 03:37:32.795344 pyuilder-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 03:37:32.850344 pyuilder-0.0.3/src/Pyuilder.egg-info/
+-rw-rw-rw-   0        0        0     7058 2024-05-06 03:37:32.000000 pyuilder-0.0.3/src/Pyuilder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2024-05-06 03:37:32.000000 pyuilder-0.0.3/src/Pyuilder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 03:37:32.000000 pyuilder-0.0.3/src/Pyuilder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2024-05-06 03:37:32.000000 pyuilder-0.0.3/src/Pyuilder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-06 03:37:32.000000 pyuilder-0.0.3/src/Pyuilder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 03:37:32.832347 pyuilder-0.0.3/src/pyuilder/
+-rw-rw-rw-   0        0        0      137 2024-05-05 22:27:02.000000 pyuilder-0.0.3/src/pyuilder/__init__.py
+-rw-rw-rw-   0        0        0     4257 2024-05-06 02:00:30.000000 pyuilder-0.0.3/src/pyuilder/pyuilder.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:37:32.847842 pyuilder-0.0.3/test/
+-rw-rw-rw-   0        0        0     2573 2024-05-06 01:46:59.000000 pyuilder-0.0.3/test/test_pyuilder.py
```

### Comparing `pyuilder-0.0.1/LICENSE` & `pyuilder-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuilder-0.0.1/PKG-INFO` & `pyuilder-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,19 @@
-Metadata-Version: 2.1
-Name: Pyuilder
-Version: 0.0.1
-Summary: Provides functionality for implementing the builder pattern in Python.
-Author-email: Kevin Jerome <kjerome64@gmail.com>
-Maintainer-email: Kevin Jerome <kjerome64@gmail.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
-Project-URL: Funding, https://donate.pypi.org
-Project-URL: Say Thanks!, http://saythanks.io/to/example
-Project-URL: Source, https://github.com/pypa/sampleproject/
-Keywords: builder,builder_pattern,design_patterns
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Provides-Extra: dev
-Provides-Extra: test
-Requires-Dist: pytest==8.2.0; extra == "test"
-
 <h1 align="center">Pyuilder ("pill-der")</h1>
 
 <h2 align="center">
 Bringing the Builder Design Pattern to Python
 </h2>
 
 <!-- Shields Here -->
 <p align="center">
+<img alt="Version" src="https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fkevdog824%2Fpyuilder%2Fmain%2Fpyproject.toml"/>
+<img alt="License" src="https://img.shields.io/github/license/Kevdog824/pyuilder"/>
+<img alt="Monthly Downloads" href="https://img.shields.io/pypi/dm/pyuilder">
+<a href="https://github.com/kevdog824/pyuilder/actions/workflows/python.yml"><img alt="Actions Status" src="https://github.com/kevdog824/pyuilder/actions/workflows/python.yml/badge.svg"></a>
 </p>
 
 ---
 
 ## Summary
 
 - [Getting started](#getting-started)
@@ -78,14 +53,16 @@
 ```
 
 #### Customize the Builder & Add Type Annotations
 
 The last example was great and easy to set up but you'll quickly notice you get no intellisense or typing annotations in your IDE. If that's alright with you: great! However, if you want a little more out of pyuilder it's pretty trivial to provide as much information as you want to pyuilder's `Buildable` to get auto-complete, type-hinting, and other useful information in your IDE:
 
 ```py
+from __future__ import annotations
+
 from pyuilder import Buildable, Builder, Setter
 
 
 class MyBuildable(Buildable):
     class builder(Builder["MyBuildable"]):
         field1: Setter[MyBuildable.builder, int]
         field2: Setter[MyBuildable.builder, str]
@@ -112,14 +89,16 @@
   - The second `TypeVar` indicates the value type the field setter accepts: `.field1(value: int).field2(value: str)`.
 
 #### Customize the Way Fields Are Set
 
 The other thing you might want to do is have better control how fields are set when you do something like `.builder().field(...)`. If `field` was a `list` for example you might want to be able to call `field(...)` on the builder multiple times to continuously append values to it (similar to Lombok's `@Singular` in Java). This is certainly possible with pyuilder:
 
 ```py
+from __future__ import annotations
+
 from pyuilder import Buildable, Builder, Setter
 
 
 class MyBuildable(Buildable):
     class builder(Builder["MyBuildable"]):
         field: Setter[MyBuildable.builder, str | list[str]]
```

### Comparing `pyuilder-0.0.1/pyproject.toml` & `pyuilder-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
-name = "Pyuilder"
-version = "0.0.1"
+name = "pyuilder"
+version = "0.0.3"
 description = "Provides functionality for implementing the builder pattern in Python."
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE.txt" }
 keywords = ["builder", "builder_pattern", "design_patterns"]
 authors = [{ name = "Kevin Jerome", email = "kjerome64@gmail.com" }]
 maintainers = [{ name = "Kevin Jerome", email = "kjerome64@gmail.com" }]
@@ -23,43 +23,56 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = []
 
+
 [project.optional-dependencies]
-dev = []
-test = ["pytest==8.2.0"]
+dev = ["mypy==1.10.0", "ruff==0.4.3"]
+test = ["pytest==8.2.0", "pytest-cov==5.0.0"]
+publish = ["build==1.2.1", "twine==5.0.0"]
+ci = ["pyuilder[dev]", "pyuilder[test]", "pyuilder[publish]"]
 
 
 [project.urls]
-"Homepage" = "https://github.com/pypa/sampleproject"
-"Bug Reports" = "https://github.com/pypa/sampleproject/issues"
-"Funding" = "https://donate.pypi.org"
-"Say Thanks!" = "http://saythanks.io/to/example"
-"Source" = "https://github.com/pypa/sampleproject/"
+"Homepage" = "https://github.com/kevdog824/pyuilder"
+"Bug Reports" = "https://github.com/kevdog824/pyuilder/issues"
+"Source" = "https://github.com/kevdog824/pyuilder"
 
 
 [tool.setuptools]
 package-data = { "sample" = ["*.dat"] }
 
 
+[tool.coverage.paths]
+source = ["src"]
+
+
+[tool.coverage.report]
+fail_under = 70
+show_missing = true
+
+
+[tool.pytest.ini_options]
+testpaths = ["test"]
+
+
 [tool.ruff]
 exclude = [
     ".git",
     ".mypy_cache",
     ".pytest_cache",
     ".ruff_cache",
     ".venv",
     ".vscode",
 ]
 line-length = 88
 indent-width = 4
-target-version = "py312"
 
 
 [tool.ruff.format]
 quote-style = "double"
 indent-style = "space"
 
 
@@ -69,11 +82,7 @@
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["E402", "F401"]
 
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
-
-
-[tool.pytest.ini_options]
-testpaths = ["tests"]
```

### Comparing `pyuilder-0.0.1/src/Pyuilder.egg-info/PKG-INFO` & `pyuilder-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
-Name: Pyuilder
-Version: 0.0.1
+Name: pyuilder
+Version: 0.0.3
 Summary: Provides functionality for implementing the builder pattern in Python.
 Author-email: Kevin Jerome <kjerome64@gmail.com>
 Maintainer-email: Kevin Jerome <kjerome64@gmail.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
-Project-URL: Funding, https://donate.pypi.org
-Project-URL: Say Thanks!, http://saythanks.io/to/example
-Project-URL: Source, https://github.com/pypa/sampleproject/
+Project-URL: Homepage, https://github.com/kevdog824/pyuilder
+Project-URL: Bug Reports, https://github.com/kevdog824/pyuilder/issues
+Project-URL: Source, https://github.com/kevdog824/pyuilder
 Keywords: builder,builder_pattern,design_patterns
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,25 +18,39 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
+Requires-Dist: mypy==1.10.0; extra == "dev"
+Requires-Dist: ruff==0.4.3; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest==8.2.0; extra == "test"
+Requires-Dist: pytest-cov==5.0.0; extra == "test"
+Provides-Extra: publish
+Requires-Dist: build==1.2.1; extra == "publish"
+Requires-Dist: twine==5.0.0; extra == "publish"
+Provides-Extra: ci
+Requires-Dist: pyuilder[dev]; extra == "ci"
+Requires-Dist: pyuilder[test]; extra == "ci"
+Requires-Dist: pyuilder[publish]; extra == "ci"
 
 <h1 align="center">Pyuilder ("pill-der")</h1>
 
 <h2 align="center">
 Bringing the Builder Design Pattern to Python
 </h2>
 
 <!-- Shields Here -->
 <p align="center">
+<img alt="Version" src="https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fkevdog824%2Fpyuilder%2Fmain%2Fpyproject.toml"/>
+<img alt="License" src="https://img.shields.io/github/license/Kevdog824/pyuilder"/>
+<img alt="Monthly Downloads" href="https://img.shields.io/pypi/dm/pyuilder">
+<a href="https://github.com/kevdog824/pyuilder/actions/workflows/python.yml"><img alt="Actions Status" src="https://github.com/kevdog824/pyuilder/actions/workflows/python.yml/badge.svg"></a>
 </p>
 
 ---
 
 ## Summary
 
 - [Getting started](#getting-started)
@@ -78,14 +90,16 @@
 ```
 
 #### Customize the Builder & Add Type Annotations
 
 The last example was great and easy to set up but you'll quickly notice you get no intellisense or typing annotations in your IDE. If that's alright with you: great! However, if you want a little more out of pyuilder it's pretty trivial to provide as much information as you want to pyuilder's `Buildable` to get auto-complete, type-hinting, and other useful information in your IDE:
 
 ```py
+from __future__ import annotations
+
 from pyuilder import Buildable, Builder, Setter
 
 
 class MyBuildable(Buildable):
     class builder(Builder["MyBuildable"]):
         field1: Setter[MyBuildable.builder, int]
         field2: Setter[MyBuildable.builder, str]
@@ -112,14 +126,16 @@
   - The second `TypeVar` indicates the value type the field setter accepts: `.field1(value: int).field2(value: str)`.
 
 #### Customize the Way Fields Are Set
 
 The other thing you might want to do is have better control how fields are set when you do something like `.builder().field(...)`. If `field` was a `list` for example you might want to be able to call `field(...)` on the builder multiple times to continuously append values to it (similar to Lombok's `@Singular` in Java). This is certainly possible with pyuilder:
 
 ```py
+from __future__ import annotations
+
 from pyuilder import Buildable, Builder, Setter
 
 
 class MyBuildable(Buildable):
     class builder(Builder["MyBuildable"]):
         field: Setter[MyBuildable.builder, str | list[str]]
```

### Comparing `pyuilder-0.0.1/src/pyuilder/pyuilder.py` & `pyuilder-0.0.3/src/pyuilder/pyuilder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Library that provides functionality for the builder design pattern in Python."""
 
 from __future__ import annotations
 import inspect
 import typing as _t
+import typing_extensions as _te
 
 
 ### Typing
 
 _B = _t.TypeVar("_B", bound="Builder")
 _T = _t.TypeVar("_T")
 
@@ -73,15 +74,15 @@
         """
         self._data: _t.Dict[str, _t.Any] = {**kwargs}
         self._init_param_kinds = [
             inspect._ParameterKind.POSITIONAL_OR_KEYWORD,
             inspect._ParameterKind.KEYWORD_ONLY,
         ]
 
-    def __getattr__(self, __name: str) -> Setter[_t.Self, _t.Any]:
+    def __getattr__(self, __name: str) -> Setter[_te.Self, _t.Any]:
         return Setter(self, __name)
 
     def _break_args(
         self, typ: _t.Type[_T]
     ) -> _t.Tuple[_t.Dict[str, _t.Any], _t.Dict[str, _t.Any]]:
         kwargs: _t.Dict[str, _t.Any] = {}
         sig = inspect.signature(typ)
@@ -106,24 +107,24 @@
 
 ### Builder Generation
 
 
 class Buildable:
     if _t.TYPE_CHECKING:
 
-        class builder(Builder[_t.Self]): ...  # type: ignore
+        class builder(Builder[_te.Self]): ...  # type: ignore # pragma: no cover
 
-    @classmethod
-    def builder(cls, **kwargs: _t.Any) -> Builder[_t.Self]:
+    @classmethod  # type: ignore[no-redef]
+    def builder(cls, **kwargs: _t.Any) -> Builder[_te.Self]:
         """Create a new builder instance for building the class
 
         Args:
             **kwargs (Any): Can set any number of fields here at construction
         """
-        b = Builder(**kwargs)
+        b: Builder[_te.Self] = Builder(**kwargs)
         b.typ = cls
         return b
 
     def __init_subclass__(cls, **_: _t.Any) -> None:
         for value in cls.__dict__.values():
             if isinstance(value, type) and issubclass(value, Builder):
                 value.typ = cls  # type: ignore
```

### Comparing `pyuilder-0.0.1/test/test_pyuilder.py` & `pyuilder-0.0.3/test/test_pyuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pyuilder import Buildable, Builder, Setter
 
 
 ### Setup
 
 
 class NoExplicitBuilderBuildable(Buildable):
-    def __init__(self, field1: int, field2: str) -> None:
+    def __init__(self, field1: int = 0, field2: str = "DEFAULT") -> None:
         self.field1 = field1
         self.field2 = field2
 
 
 @dataclasses.dataclass
 class HasExplicitBuilderBuildable(Buildable):
     field1: int
```

