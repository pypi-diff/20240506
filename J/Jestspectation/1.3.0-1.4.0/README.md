# Comparing `tmp/jestspectation-1.3.0.tar.gz` & `tmp/jestspectation-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jestspectation-1.3.0.tar", max compression
+gzip compressed data, was "jestspectation-1.4.0.tar", max compression
```

## Comparing `jestspectation-1.3.0.tar` & `jestspectation-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     1073 2023-12-06 06:33:56.587921 jestspectation-1.3.0/LICENSE
--rw-r--r--   0        0        0     1354 2023-12-06 06:33:56.587921 jestspectation-1.3.0/README.md
--rw-r--r--   0        0        0     1455 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/__any.py
--rw-r--r--   0        0        0      609 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/__config/__config.py
--rw-r--r--   0        0        0      105 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/__config/__init__.py
--rw-r--r--   0        0        0    18537 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/__containers.py
--rw-r--r--   0        0        0     2451 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/__equals.py
--rw-r--r--   0        0        0     3625 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/__float_approx.py
--rw-r--r--   0        0        0     1245 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/__init__.py
--rw-r--r--   0        0        0     3145 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/__jestspectation_base.py
--rw-r--r--   0        0        0     2861 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/__py_diffs.py
--rw-r--r--   0        0        0     1304 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/__strings/__containing.py
--rw-r--r--   0        0        0      292 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/__strings/__init__.py
--rw-r--r--   0        0        0     4741 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/__strings/__lines_like.py
--rw-r--r--   0        0        0     1360 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/__strings/__matching_regex.py
--rw-r--r--   0        0        0     2547 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/__strings/__text_like.py
--rw-r--r--   0        0        0     3699 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/__util.py
--rw-r--r--   0        0        0     1670 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/logicals/__and.py
--rw-r--r--   0        0        0      242 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/logicals/__init__.py
--rw-r--r--   0        0        0     1279 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/logicals/__not.py
--rw-r--r--   0        0        0     1612 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/logicals/__or.py
--rw-r--r--   0        0        0     2162 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/logicals/__xor.py
--rw-r--r--   0        0        0        0 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/py.typed
--rw-r--r--   0        0        0      719 2023-12-06 06:33:56.587921 jestspectation-1.3.0/jestspectation/pytest.py
--rw-r--r--   0        0        0     1556 2023-12-06 06:33:56.587921 jestspectation-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 jestspectation-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-06 11:47:28.382850 jestspectation-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1470 2024-05-06 11:47:28.382850 jestspectation-1.4.0/README.md
+-rw-r--r--   0        0        0     1455 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/__any.py
+-rw-r--r--   0        0        0      550 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/__assert.py
+-rw-r--r--   0        0        0      609 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/__config/__config.py
+-rw-r--r--   0        0        0      105 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/__config/__init__.py
+-rw-r--r--   0        0        0    18537 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/__containers.py
+-rw-r--r--   0        0        0     2705 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/__equals.py
+-rw-r--r--   0        0        0     3625 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/__float_approx.py
+-rw-r--r--   0        0        0     1294 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/__init__.py
+-rw-r--r--   0        0        0     3145 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/__jestspectation_base.py
+-rw-r--r--   0        0        0     2861 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/__py_diffs.py
+-rw-r--r--   0        0        0     1304 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/__strings/__containing.py
+-rw-r--r--   0        0        0      292 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/__strings/__init__.py
+-rw-r--r--   0        0        0     4741 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/__strings/__lines_like.py
+-rw-r--r--   0        0        0     1360 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/__strings/__matching_regex.py
+-rw-r--r--   0        0        0     2547 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/__strings/__text_like.py
+-rw-r--r--   0        0        0     3699 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/__util.py
+-rw-r--r--   0        0        0     1670 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/logicals/__and.py
+-rw-r--r--   0        0        0      242 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/logicals/__init__.py
+-rw-r--r--   0        0        0     1279 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/logicals/__not.py
+-rw-r--r--   0        0        0     1612 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/logicals/__or.py
+-rw-r--r--   0        0        0     2162 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/logicals/__xor.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/py.typed
+-rw-r--r--   0        0        0      719 2024-05-06 11:47:28.386849 jestspectation-1.4.0/jestspectation/pytest.py
+-rw-r--r--   0        0        0     1562 2024-05-06 11:47:28.386849 jestspectation-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 jestspectation-1.4.0/PKG-INFO
```

### Comparing `jestspectation-1.3.0/LICENSE` & `jestspectation-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jestspectation-1.3.0/README.md` & `jestspectation-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 } == {
     "a": 1,
     "b": expect.Any(int),
     "c": expect.FloatApprox(2.5, magnitude=0.5)
 }
 ```
 
+## Documentation
+
+Documentation can be found [on GitHub Pages](https://miguelguthridge.github.io/Jestspectation/).
+
 ## Installation
 
 ```sh
 pip install jestspectation
 ```
 
 ## Usage with Pytest
```

### Comparing `jestspectation-1.3.0/jestspectation/__any.py` & `jestspectation-1.4.0/jestspectation/__any.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.3.0/jestspectation/__config/__config.py` & `jestspectation-1.4.0/jestspectation/__config/__config.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.3.0/jestspectation/__containers.py` & `jestspectation-1.4.0/jestspectation/__containers.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.3.0/jestspectation/__equals.py` & `jestspectation-1.4.0/jestspectation/__equals.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     While this isn't as useful for top-level comparisons, it can be used
     effectively for checking nested data structures.
     """
     def __init__(self, value: object) -> None:
         """
         Matches values that have the same identity as the given value.
 
+        While this isn't as useful for top-level comparisons, it can be used
+        effectively for checking nested data structures.
+
         Args:
             value (object): object to check
         """
         self.__value = value
 
     def __repr__(self) -> str:
         return f"Is({self.__value})"
@@ -53,15 +56,18 @@
     Matches objects that have the same value.
 
     This is equivalent to the `==` operator, but with additional information
     on the difference, which can help with debugging.
     """
     def __init__(self, value: object) -> None:
         """
-        Matches values that have the same identity as the given value.
+        Matches objects that have the same value.
+
+        This is equivalent to the `==` operator, but with additional
+        information on the difference, which can help with debugging.
 
         Args:
             value (object): object to check
         """
         self.__value = value
 
     def __repr__(self) -> str:
```

### Comparing `jestspectation-1.3.0/jestspectation/__float_approx.py` & `jestspectation-1.4.0/jestspectation/__float_approx.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.3.0/jestspectation/__init__.py` & `jestspectation-1.4.0/jestspectation/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,21 +24,23 @@
 from .logicals import And, Not, Or, Xor
 from .__strings import (
     StringMatchingRegex,
     StringContaining,
     TextLike,
     LinesLike,
 )
+from .__assert import assert_eq
 from .__config import configure
 
 
 __all__ = [
     'And',
     'Any',
     'Anything',
+    'assert_eq',
     'JestspectationBase',
     'configure',
     'DictContainingKeys',
     'DictContainingValues',
     'DictContainingItems',
     'Equals',
     'FloatApprox',
```

### Comparing `jestspectation-1.3.0/jestspectation/__jestspectation_base.py` & `jestspectation-1.4.0/jestspectation/__jestspectation_base.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.3.0/jestspectation/__py_diffs.py` & `jestspectation-1.4.0/jestspectation/__py_diffs.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.3.0/jestspectation/__strings/__containing.py` & `jestspectation-1.4.0/jestspectation/__strings/__containing.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.3.0/jestspectation/__strings/__lines_like.py` & `jestspectation-1.4.0/jestspectation/__strings/__lines_like.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.3.0/jestspectation/__strings/__matching_regex.py` & `jestspectation-1.4.0/jestspectation/__strings/__matching_regex.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.3.0/jestspectation/__strings/__text_like.py` & `jestspectation-1.4.0/jestspectation/__strings/__text_like.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.3.0/jestspectation/__util.py` & `jestspectation-1.4.0/jestspectation/__util.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.3.0/jestspectation/logicals/__and.py` & `jestspectation-1.4.0/jestspectation/logicals/__and.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.3.0/jestspectation/logicals/__not.py` & `jestspectation-1.4.0/jestspectation/logicals/__not.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.3.0/jestspectation/logicals/__or.py` & `jestspectation-1.4.0/jestspectation/logicals/__or.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.3.0/jestspectation/logicals/__xor.py` & `jestspectation-1.4.0/jestspectation/logicals/__xor.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.3.0/jestspectation/pytest.py` & `jestspectation-1.4.0/jestspectation/pytest.py`

 * *Files identical despite different names*

### Comparing `jestspectation-1.3.0/pyproject.toml` & `jestspectation-1.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "Jestspectation"
-version = "1.3.0"
+version = "1.4.0"
 description = "Pattern matching tools to test complex data structures"
 readme = "README.md"
 
-authors = ["Miguel Guthridge <hdsq@outlook.com.au>"]
+authors = ["Miguel Guthridge <hello@miguelguthridge.com>"]
 license = "MIT"
 
 repository = "https://github.com/MiguelGuthridge/Jestspectation"
 documentation = "https://miguelguthridge.github.io/Jestspectation"
 
 keywords = [
     "jest",
@@ -42,20 +42,20 @@
 "Bug Tracker" = "https://github.com/MiguelGuthridge/Jestspectation/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typing-extensions = "^4.5.0"
 
 [tool.poetry.dev-dependencies]
-mypy = "^1.7.1"
-flake8 = "^6.1.0"
-pytest = "^7.4.3"
-autopep8 = "^2.0.4"
-coverage = "^7.3.2"
+mypy = "^1.9.0"
+flake8 = "^7.0.0"
+pytest = "^8.2.0"
+autopep8 = "^2.1.0"
+coverage = "^7.5.1"
 mkdocs = "^1.5.3"
 mkdocs-gen-files = "^0.5.0"
-mkdocs-material = "^9.4.14"
-mkdocstrings = {version = "^0.24.0", extras = ["python"]}
+mkdocs-material = "^9.5.18"
+mkdocstrings = {version = "^0.25.1", extras = ["python"]}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `jestspectation-1.3.0/PKG-INFO` & `jestspectation-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Jestspectation
-Version: 1.3.0
+Version: 1.4.0
 Summary: Pattern matching tools to test complex data structures
 Home-page: https://github.com/MiguelGuthridge/Jestspectation
 License: MIT
 Keywords: jest,pattern,matching,pytest,equality
 Author: Miguel Guthridge
-Author-email: hdsq@outlook.com.au
+Author-email: hello@miguelguthridge.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -45,14 +45,18 @@
 } == {
     "a": 1,
     "b": expect.Any(int),
     "c": expect.FloatApprox(2.5, magnitude=0.5)
 }
 ```
 
+## Documentation
+
+Documentation can be found [on GitHub Pages](https://miguelguthridge.github.io/Jestspectation/).
+
 ## Installation
 
 ```sh
 pip install jestspectation
 ```
 
 ## Usage with Pytest
```

