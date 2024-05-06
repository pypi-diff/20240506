# Comparing `tmp/pure_utils-0.7.0.tar.gz` & `tmp/pure_utils-0.8.0.tar.gz`

## Comparing `pure_utils-0.7.0.tar` & `pure_utils-0.8.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 pure_utils-0.7.0/Makefile
--rwxr-xr-x   0        0        0      628 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/Makefile
--rwxr-xr-x   0        0        0     1412 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/conf.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/source/changelog.rst
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/source/commands.rst
--rwxr-xr-x   0        0        0      745 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/source/index.rst
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/source/license.rst
--rwxr-xr-x   0        0        0      145 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/source/refs/index.rst
--rwxr-xr-x   0        0        0     8643 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/templates/page.html
--rwxr-xr-x   0        0        0      762 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.docs/templates/autosummary/module.rst
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.github/workflows/ci.yaml
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/__init__.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/common.py
--rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/containers.py
--rw-r--r--   0        0        0     7296 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/debug.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/profiler.py
--rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/repeaters.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/strings.py
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/times.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/_internal/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/_internal/_profile_stats.py
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pure_utils/_internal/_profile_stats_serializers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/test_common.py
--rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/test_containers.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/test_debug.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/test_profiler.py
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/test_repeaters.py
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/test_strings.py
--rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 pure_utils-0.7.0/tests/test_times.py
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 pure_utils-0.7.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pure_utils-0.7.0/LICENSE
--rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 pure_utils-0.7.0/README.md
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 pure_utils-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 pure_utils-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 pure_utils-0.8.0/Makefile
+-rwxr-xr-x   0        0        0      628 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/Makefile
+-rwxr-xr-x   0        0        0     1412 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/conf.py
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/source/changelog.rst
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/source/commands.rst
+-rwxr-xr-x   0        0        0      742 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/source/index.rst
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/source/license.rst
+-rwxr-xr-x   0        0        0      158 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/source/refs/index.rst
+-rwxr-xr-x   0        0        0     8643 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/templates/page.html
+-rwxr-xr-x   0        0        0      762 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/templates/autosummary/module.rst
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/__init__.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/common.py
+-rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/containers.py
+-rw-r--r--   0        0        0     7296 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/debug.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/profiler.py
+-rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/repeaters.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/strings.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/system.py
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/times.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/_internal/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/_internal/_profile_stats.py
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/_internal/_profile_stats_serializers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/test_common.py
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/test_containers.py
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/test_debug.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/test_profiler.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/test_repeaters.py
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/test_strings.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/test_system.py
+-rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/test_times.py
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pure_utils-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 pure_utils-0.8.0/README.md
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8803 2020-02-02 00:00:00.000000 pure_utils-0.8.0/PKG-INFO
```

### Comparing `pure_utils-0.7.0/Makefile` & `pure_utils-0.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/.docs/Makefile` & `pure_utils-0.8.0/.docs/Makefile`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/.docs/conf.py` & `pure_utils-0.8.0/.docs/conf.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/.docs/source/changelog.rst` & `pure_utils-0.8.0/.docs/source/changelog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+v0.8.0 - [2024-05-06]
+---------------------
+* Add new module - ``system`` (system purpose utilities).
+* Update development dependencies.
+* Use dynamic version into pyproject.toml.
+* Fix project short description.
+
 v0.7.0 - [2024-04-22]
 ---------------------
 * Add new module - ``repeaters`` (utilities for repeat functions).
 * Update development dependencies.
 
 v0.6.0 - [2024-03-01]
 ---------------------
```

### Comparing `pure_utils-0.7.0/.docs/source/commands.rst` & `pure_utils-0.8.0/.docs/source/commands.rst`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/.docs/source/index.rst` & `pure_utils-0.8.0/.docs/source/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pure-utils
 ==========
 
-Yet another python utilities, with the goal of collecting useful bicycles and crutches in one place ;).
+Yet another python utilities, with the goal of collecting useful bicycles and crutches in one place.
 
 **Main principles**:
 
 1. No third party dependencies (standart library only).
 2. Mostly pure functions without side effects.
 3. Interfaces with type annotations.
 4. Comprehensive documentation with examples of use.
```

### Comparing `pure_utils-0.7.0/.docs/source/license.rst` & `pure_utils-0.8.0/.docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/.docs/templates/page.html` & `pure_utils-0.8.0/.docs/templates/page.html`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/.docs/templates/autosummary/module.rst` & `pure_utils-0.8.0/.docs/templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/.github/workflows/ci.yaml` & `pure_utils-0.8.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/pure_utils/common.py` & `pure_utils-0.8.0/pure_utils/common.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/pure_utils/containers.py` & `pure_utils-0.8.0/pure_utils/containers.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/pure_utils/debug.py` & `pure_utils-0.8.0/pure_utils/debug.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/pure_utils/profiler.py` & `pure_utils-0.8.0/pure_utils/profiler.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/pure_utils/repeaters.py` & `pure_utils-0.8.0/pure_utils/repeaters.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/pure_utils/strings.py` & `pure_utils-0.8.0/pure_utils/strings.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/pure_utils/times.py` & `pure_utils-0.8.0/pure_utils/times.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/pure_utils/_internal/_profile_stats.py` & `pure_utils-0.8.0/pure_utils/_internal/_profile_stats.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/pure_utils/_internal/_profile_stats_serializers.py` & `pure_utils-0.8.0/pure_utils/_internal/_profile_stats_serializers.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/tests/test_containers.py` & `pure_utils-0.8.0/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/tests/test_debug.py` & `pure_utils-0.8.0/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/tests/test_profiler.py` & `pure_utils-0.8.0/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/tests/test_repeaters.py` & `pure_utils-0.8.0/tests/test_repeaters.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/tests/test_strings.py` & `pure_utils-0.8.0/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/tests/test_times.py` & `pure_utils-0.8.0/tests/test_times.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/LICENSE` & `pure_utils-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_utils-0.7.0/README.md` & `pure_utils-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ![Build Status](https://github.com/p3t3rbr0/py3-pure-utils/actions/workflows/ci.yaml/badge.svg?branch=master)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pure-utils)
 ![PyPI Version](https://img.shields.io/pypi/v/pure-utils)
 [![Code Coverage](https://codecov.io/gh/p3t3rbr0/py3-pure-utils/graph/badge.svg?token=283H0MAGUP)](https://codecov.io/gh/p3t3rbr0/py3-pure-utils)
 [![Maintainability](https://api.codeclimate.com/v1/badges/14f70c48db708a419309/maintainability)](https://codeclimate.com/github/p3t3rbr0/py3-pure-utils/maintainability)
 
-Yet another python utilities, with the goal of collecting useful bicycles and crutches in one place ;).
+Yet another python utilities, with the goal of collecting useful bicycles and crutches in one place.
 
 Main principles:
 
 1. No third party dependencies (standart library only).
 2. Mostly pure functions without side effects.
 3. Interfaces with type annotations.
 4. Comprehensive documentation with examples of use.
@@ -44,14 +44,16 @@
   * [ExceptionBasedRepeater](https://p3t3rbr0.github.io/py3-pure-utils/refs/repeaters.html#repeaters.ExceptionBasedRepeater) - Repeater based on catching targeted exceptions.
   * [PredicateBasedRepeater](https://p3t3rbr0.github.io/py3-pure-utils/refs/repeaters.html#repeaters.PredicateBasedRepeater) - Repeater based on predicate function.
   * [repeat](https://p3t3rbr0.github.io/py3-pure-utils/refs/repeaters.html#repeaters.repeat)(repeater: Repeater) - Repeat wrapped function by `repeater` logic.
 * [strings](https://p3t3rbr0.github.io/py3-pure-utils/refs/strings.html) - Utilities for working with strings.
   * [genstr](https://p3t3rbr0.github.io/py3-pure-utils/refs/strings.html#strings.genstr)([length, is_uppercase]) - Generate ASCII-string with random letters.
   * [gunzip](https://p3t3rbr0.github.io/py3-pure-utils/refs/strings.html#strings.gzip)(compressed_string, /) - Compress string (or bytes string) with gzip compression level.
   * [gzip](https://p3t3rbr0.github.io/py3-pure-utils/refs/strings.html#strings.gunzip)(string, /, *[, level]) - Decompress bytes (earlier compressed with gzip) to string.
+* [system](https://p3t3rbr0.github.io/py3-pure-utils/refs/system.html) - The system purpose utilities.
+  * [execute](https://p3t3rbr0.github.io/py3-pure-utils/refs/system.html#system.execute)(args, *[, input, timeout]) - Execute command into external process.
 * [times](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html) - Utilities for working with datetime objects.
   * [apply_tz](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html#times.apply_tz)(dt[, tz]) - Apply timezone context to datetime object.
   * [iso2format](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html#times.iso2format)(isostr, fmt, /) - Convert ISO-8601 datetime string into a string of specified format.
   * [iso2dmy](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html#times.iso2dmy)(isostr, /) - Convert ISO-8601 datetime string into a string of DMY (DD.MM.YYYY) format.
   * [iso2ymd](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html#times.iso2ymd)(isostr, /) - Convert ISO-8601 datetime string into a string of YMD (YYYY-MM-DD) format.
   * [round_by](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html#times.round_by)(dt, /, *, boundary) - Round datetime, discarding excessive precision.
```

### Comparing `pure_utils-0.7.0/pyproject.toml` & `pure_utils-0.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 [build-system]
 requires = ["hatchling==1.21.1"]
 build-backend = "hatchling.build"
 
-[tool.setuptools]
-include-package-data = false
-
-[tool.setuptools.packages.find]
-include = ["pure_utils*"]
-exclude = ["tests*"]
+[tool.hatch.version]
+path = "pure_utils/__init__.py"
 
 [project]
 name = "pure-utils"
-version = "0.7.0"
+dynamic = ["version"]
 authors = [
-  {name="Peter Bro", email="p3t3rbr0@gmail.com"},
+  {name = "Peter Bro", email = "p3t3rbr0@gmail.com"},
 ]
-description = "Yet another python utilities, with the goal of collecting useful bicycles and crutches in one place ;)."
+description = "Yet another python utilities, with the goal of collecting useful bicycles and crutches in one place."
 keywords = ["utilities", "bicycle", "crutches"]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
@@ -38,22 +34,22 @@
 Documentation = "https://p3t3rbr0.github.io/py3-pure-utils/"
 Repository = "https://github.com/p3t3rbr0/py3-pure-utils.git"
 Issues = "https://github.com/p3t3rbr0/py3-pure-utils/issues"
 Changelog = "https://github.com/p3t3rbr0/py3-pure-utils/blob/master/.docs/source/changelog.rst"
 
 [project.optional-dependencies]
 build = ["build==1.2.1", "twine==5.0.0"]
-docs = ["Sphinx==7.2.6", "furo==2024.1.29"]
+docs = ["Sphinx==7.3.7", "furo==2024.4.27"]
 dev = [
-    "mypy==1.9.0",
+    "mypy==1.10.0",
     "isort==5.13.2",
     "flake8==7.0.0",
-    "black==24.4.0",
+    "black==24.4.2",
     "pydocstyle==6.3.0",
-    "pytest==8.1.1",
+    "pytest==8.2.0",
     "pytest-cov==5.0.0",
     "pytest-mock==3.14.0",
 ]
 
 [tool.mypy]
 exclude = ["tests"]
 ignore_missing_imports = true
```

### Comparing `pure_utils-0.7.0/PKG-INFO` & `pure_utils-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pure-utils
-Version: 0.7.0
-Summary: Yet another python utilities, with the goal of collecting useful bicycles and crutches in one place ;).
+Version: 0.8.0
+Summary: Yet another python utilities, with the goal of collecting useful bicycles and crutches in one place.
 Project-URL: Homepage, https://github.com/p3t3rbr0/py3-pure-utils
 Project-URL: Documentation, https://p3t3rbr0.github.io/py3-pure-utils/
 Project-URL: Repository, https://github.com/p3t3rbr0/py3-pure-utils.git
 Project-URL: Issues, https://github.com/p3t3rbr0/py3-pure-utils/issues
 Project-URL: Changelog, https://github.com/p3t3rbr0/py3-pure-utils/blob/master/.docs/source/changelog.rst
 Author-email: Peter Bro <p3t3rbr0@gmail.com>
 License-File: LICENSE
@@ -22,36 +22,36 @@
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Provides-Extra: build
 Requires-Dist: build==1.2.1; extra == 'build'
 Requires-Dist: twine==5.0.0; extra == 'build'
 Provides-Extra: dev
-Requires-Dist: black==24.4.0; extra == 'dev'
+Requires-Dist: black==24.4.2; extra == 'dev'
 Requires-Dist: flake8==7.0.0; extra == 'dev'
 Requires-Dist: isort==5.13.2; extra == 'dev'
-Requires-Dist: mypy==1.9.0; extra == 'dev'
+Requires-Dist: mypy==1.10.0; extra == 'dev'
 Requires-Dist: pydocstyle==6.3.0; extra == 'dev'
 Requires-Dist: pytest-cov==5.0.0; extra == 'dev'
 Requires-Dist: pytest-mock==3.14.0; extra == 'dev'
-Requires-Dist: pytest==8.1.1; extra == 'dev'
+Requires-Dist: pytest==8.2.0; extra == 'dev'
 Provides-Extra: docs
-Requires-Dist: furo==2024.1.29; extra == 'docs'
-Requires-Dist: sphinx==7.2.6; extra == 'docs'
+Requires-Dist: furo==2024.4.27; extra == 'docs'
+Requires-Dist: sphinx==7.3.7; extra == 'docs'
 Description-Content-Type: text/markdown
 
 # pure-utils
 
 ![Build Status](https://github.com/p3t3rbr0/py3-pure-utils/actions/workflows/ci.yaml/badge.svg?branch=master)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pure-utils)
 ![PyPI Version](https://img.shields.io/pypi/v/pure-utils)
 [![Code Coverage](https://codecov.io/gh/p3t3rbr0/py3-pure-utils/graph/badge.svg?token=283H0MAGUP)](https://codecov.io/gh/p3t3rbr0/py3-pure-utils)
 [![Maintainability](https://api.codeclimate.com/v1/badges/14f70c48db708a419309/maintainability)](https://codeclimate.com/github/p3t3rbr0/py3-pure-utils/maintainability)
 
-Yet another python utilities, with the goal of collecting useful bicycles and crutches in one place ;).
+Yet another python utilities, with the goal of collecting useful bicycles and crutches in one place.
 
 Main principles:
 
 1. No third party dependencies (standart library only).
 2. Mostly pure functions without side effects.
 3. Interfaces with type annotations.
 4. Comprehensive documentation with examples of use.
@@ -85,14 +85,16 @@
   * [ExceptionBasedRepeater](https://p3t3rbr0.github.io/py3-pure-utils/refs/repeaters.html#repeaters.ExceptionBasedRepeater) - Repeater based on catching targeted exceptions.
   * [PredicateBasedRepeater](https://p3t3rbr0.github.io/py3-pure-utils/refs/repeaters.html#repeaters.PredicateBasedRepeater) - Repeater based on predicate function.
   * [repeat](https://p3t3rbr0.github.io/py3-pure-utils/refs/repeaters.html#repeaters.repeat)(repeater: Repeater) - Repeat wrapped function by `repeater` logic.
 * [strings](https://p3t3rbr0.github.io/py3-pure-utils/refs/strings.html) - Utilities for working with strings.
   * [genstr](https://p3t3rbr0.github.io/py3-pure-utils/refs/strings.html#strings.genstr)([length, is_uppercase]) - Generate ASCII-string with random letters.
   * [gunzip](https://p3t3rbr0.github.io/py3-pure-utils/refs/strings.html#strings.gzip)(compressed_string, /) - Compress string (or bytes string) with gzip compression level.
   * [gzip](https://p3t3rbr0.github.io/py3-pure-utils/refs/strings.html#strings.gunzip)(string, /, *[, level]) - Decompress bytes (earlier compressed with gzip) to string.
+* [system](https://p3t3rbr0.github.io/py3-pure-utils/refs/system.html) - The system purpose utilities.
+  * [execute](https://p3t3rbr0.github.io/py3-pure-utils/refs/system.html#system.execute)(args, *[, input, timeout]) - Execute command into external process.
 * [times](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html) - Utilities for working with datetime objects.
   * [apply_tz](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html#times.apply_tz)(dt[, tz]) - Apply timezone context to datetime object.
   * [iso2format](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html#times.iso2format)(isostr, fmt, /) - Convert ISO-8601 datetime string into a string of specified format.
   * [iso2dmy](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html#times.iso2dmy)(isostr, /) - Convert ISO-8601 datetime string into a string of DMY (DD.MM.YYYY) format.
   * [iso2ymd](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html#times.iso2ymd)(isostr, /) - Convert ISO-8601 datetime string into a string of YMD (YYYY-MM-DD) format.
   * [round_by](https://p3t3rbr0.github.io/py3-pure-utils/refs/times.html#times.round_by)(dt, /, *, boundary) - Round datetime, discarding excessive precision.
```

