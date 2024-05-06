# Comparing `tmp/dj_svg-0.3.0.tar.gz` & `tmp/dj_svg-0.3.1.tar.gz`

## Comparing `dj_svg-0.3.0.tar` & `dj_svg-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 dj_svg-0.3.0/dj_svg/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dj_svg-0.3.0/dj_svg/exceptions.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 dj_svg-0.3.0/dj_svg/tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dj_svg-0.3.0/dj_svg/templatetags/__init__.py
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 dj_svg-0.3.0/dj_svg/templatetags/svg.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 dj_svg-0.3.0/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 dj_svg-0.3.0/LICENSE
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 dj_svg-0.3.0/README.md
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 dj_svg-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 dj_svg-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 dj_svg-0.3.1/dj_svg/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 dj_svg-0.3.1/dj_svg/exceptions.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 dj_svg-0.3.1/dj_svg/tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dj_svg-0.3.1/dj_svg/templatetags/__init__.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 dj_svg-0.3.1/dj_svg/templatetags/svg.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 dj_svg-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 dj_svg-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 dj_svg-0.3.1/README.md
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 dj_svg-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 dj_svg-0.3.1/PKG-INFO
```

### Comparing `dj_svg-0.3.0/dj_svg/tests.py` & `dj_svg-0.3.1/dj_svg/tests.py`

 * *Files identical despite different names*

### Comparing `dj_svg-0.3.0/dj_svg/templatetags/svg.py` & `dj_svg-0.3.1/dj_svg/templatetags/svg.py`

 * *Files identical despite different names*

### Comparing `dj_svg-0.3.0/.gitignore` & `dj_svg-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dj_svg-0.3.0/LICENSE` & `dj_svg-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_svg-0.3.0/README.md` & `dj_svg-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dj_svg-0.3.0/pyproject.toml` & `dj_svg-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
-dependencies = ["Django>=4.0", "docutils"]
+dependencies = ["Django>=4.0"]
 
 [tool.hatch.envs.default]
 installer = "uv"
 dependencies = ["pytest", "pytest-cov", "pytest-django", "ruff"]
 
 [[tool.hatch.envs.test.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11"]
```

### Comparing `dj_svg-0.3.0/PKG-INFO` & `dj_svg-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dj-svg
-Version: 0.3.0
+Version: 0.3.1
 Summary: SVG template tag for Django
 Project-URL: Homepage, https://github.com/xshapira/dj-svg
 Project-URL: Documentation, https://github.com/xshapira/dj-svg
 Author-email: Max Shapira <max@winoutt.com>
 Maintainer-email: Max Shapira <max@winoutt.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -25,15 +25,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Requires-Dist: django>=4.0
-Requires-Dist: docutils
 Description-Content-Type: text/markdown
 
 # dj-svg
 
 [![PyPI version](https://badge.fury.io/py/dj-svg.svg)](https://badge.fury.io/py/dj-svg)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/dj-svg.svg)](https://pypi.python.org/pypi/dj-svg/)
 [![PyPI Supported Django Versions](https://img.shields.io/pypi/djversions/dj-svg.svg)](https://docs.djangoproject.com/en/dev/releases/)
```

