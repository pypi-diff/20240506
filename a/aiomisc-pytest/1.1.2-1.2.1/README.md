# Comparing `tmp/aiomisc_pytest-1.1.2.tar.gz` & `tmp/aiomisc_pytest-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomisc_pytest-1.1.2.tar", max compression
+gzip compressed data, was "aiomisc_pytest-1.2.1.tar", max compression
```

## Comparing `aiomisc_pytest-1.1.2.tar` & `aiomisc_pytest-1.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1125 2024-03-11 14:23:51.426862 aiomisc_pytest-1.1.2/COPYING
--rw-r--r--   0        0        0     6667 2024-03-11 14:23:51.426862 aiomisc_pytest-1.1.2/README.md
--rw-r--r--   0        0        0    24220 2024-03-11 14:23:51.426862 aiomisc_pytest-1.1.2/aiomisc_pytest.py
--rw-r--r--   0        0        0     1868 2024-03-11 14:24:07.414948 aiomisc_pytest-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     7879 1970-01-01 00:00:00.000000 aiomisc_pytest-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1125 2024-05-06 20:17:37.893022 aiomisc_pytest-1.2.1/COPYING
+-rw-r--r--   0        0        0     6667 2024-05-06 20:17:37.893022 aiomisc_pytest-1.2.1/README.md
+-rw-r--r--   0        0        0    24220 2024-05-06 20:17:37.893022 aiomisc_pytest-1.2.1/aiomisc_pytest.py
+-rw-r--r--   0        0        0     1891 2024-05-06 20:17:59.113062 aiomisc_pytest-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7822 1970-01-01 00:00:00.000000 aiomisc_pytest-1.2.1/PKG-INFO
```

### Comparing `aiomisc_pytest-1.1.2/COPYING` & `aiomisc_pytest-1.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `aiomisc_pytest-1.1.2/README.md` & `aiomisc_pytest-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aiomisc_pytest-1.1.2/aiomisc_pytest.py` & `aiomisc_pytest-1.2.1/aiomisc_pytest.py`

 * *Files identical despite different names*

### Comparing `aiomisc_pytest-1.1.2/pyproject.toml` & `aiomisc_pytest-1.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "aiomisc-pytest"
 license = "MIT"
-version = "1.1.2"
+version = "1.2.1"
 description = "pytest integration for aiomisc"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.md"
 packages = [{include = "aiomisc_pytest.py"}]
 keywords=["pytest", "aiomisc"]
 classifiers = [
     "Environment :: Plugins",
@@ -16,33 +16,34 @@
     "Operating System :: MacOS",
     "Operating System :: Microsoft",
     "Operating System :: POSIX",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-pytest = "^7.2.1"
+python = "^3.8"
+pytest = "8.2.0"
 aiomisc = ">=17"
 
 [tool.poetry.group.uvloop.dependencies]
-uvloop = "^0.17.0"
+uvloop = "^0.19.0"
 
 [tool.poetry.group.dev.dependencies]
 pylama = "^8.4.1"
 mypy = "^1.0.0"
 pytest-cov = "^4.0.0"
+setuptools = "^69.5.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins.pytest11]
 aiomisc = "aiomisc_pytest"
```

### Comparing `aiomisc_pytest-1.1.2/PKG-INFO` & `aiomisc_pytest-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: aiomisc-pytest
-Version: 1.1.2
+Version: 1.2.1
 Summary: pytest integration for aiomisc
 License: MIT
 Keywords: pytest,aiomisc
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Plugins
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: aiomisc (>=17)
-Requires-Dist: pytest (>=7.2.1,<8.0.0)
+Requires-Dist: pytest (==8.2.0)
 Description-Content-Type: text/markdown
 
 aiomisc pytest plugin
 =====================
 
 This package contains a plugin for pytest.
```

