# Comparing `tmp/tlv-1.5.2.tar.gz` & `tmp/tlv-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tlv-1.5.2.tar", last modified: Thu Mar 28 14:18:42 2024, max compression
+gzip compressed data, was "tlv-1.5.3.tar", last modified: Mon May  6 11:28:25 2024, max compression
```

## Comparing `tlv-1.5.2.tar` & `tlv-1.5.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:18:42.676113 tlv-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-28 14:18:28.000000 tlv-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-28 14:18:28.000000 tlv-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-03-28 14:18:42.676113 tlv-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-03-28 14:18:28.000000 tlv-1.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-28 14:18:28.000000 tlv-1.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-28 14:18:42.676113 tlv-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-28 14:18:40.000000 tlv-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:18:42.672113 tlv-1.5.2/tlv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:18:28.000000 tlv-1.5.2/tlv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-28 14:18:28.000000 tlv-1.5.2/tlv/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-03-28 14:18:28.000000 tlv-1.5.2/tlv/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-03-28 14:18:28.000000 tlv-1.5.2/tlv/cls_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-28 14:18:28.000000 tlv-1.5.2/tlv/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-03-28 14:18:28.000000 tlv-1.5.2/tlv/lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-03-28 14:18:28.000000 tlv-1.5.2/tlv/src_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-03-28 14:18:28.000000 tlv-1.5.2/tlv/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:18:42.676113 tlv-1.5.2/tlv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-03-28 14:18:42.000000 tlv-1.5.2/tlv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-28 14:18:42.000000 tlv-1.5.2/tlv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:18:42.000000 tlv-1.5.2/tlv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-28 14:18:42.000000 tlv-1.5.2/tlv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-28 14:18:42.000000 tlv-1.5.2/tlv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-28 14:18:42.000000 tlv-1.5.2/tlv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:25.370055 tlv-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-06 11:28:13.000000 tlv-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-06 11:28:13.000000 tlv-1.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-05-06 11:28:25.370055 tlv-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-05-06 11:28:13.000000 tlv-1.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-06 11:28:13.000000 tlv-1.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-06 11:28:25.370055 tlv-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-06 11:28:23.000000 tlv-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:25.370055 tlv-1.5.3/tlv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:13.000000 tlv-1.5.3/tlv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-06 11:28:13.000000 tlv-1.5.3/tlv/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-06 11:28:13.000000 tlv-1.5.3/tlv/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-05-06 11:28:13.000000 tlv-1.5.3/tlv/cls_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-06 11:28:13.000000 tlv-1.5.3/tlv/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8513 2024-05-06 11:28:13.000000 tlv-1.5.3/tlv/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-06 11:28:13.000000 tlv-1.5.3/tlv/src_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-06 11:28:13.000000 tlv-1.5.3/tlv/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:28:25.370055 tlv-1.5.3/tlv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-05-06 11:28:25.000000 tlv-1.5.3/tlv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-06 11:28:25.000000 tlv-1.5.3/tlv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:28:25.000000 tlv-1.5.3/tlv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-06 11:28:25.000000 tlv-1.5.3/tlv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-06 11:28:25.000000 tlv-1.5.3/tlv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-06 11:28:25.000000 tlv-1.5.3/tlv.egg-info/top_level.txt
```

### Comparing `tlv-1.5.2/LICENSE` & `tlv-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tlv-1.5.2/PKG-INFO` & `tlv-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlv
-Version: 1.5.2
+Version: 1.5.3
 Summary: -- Too less variation -- Find duplicates in source code for various languages
 Home-page: https://github.com/priv-kweihmann/tlv
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Pygments~=2.17
+Requires-Dist: Pygments~=2.18
 Requires-Dist: chardet~=5.2
 
 # tlv
 
 ![Build status](https://github.com/priv-kweihmann/tlv/workflows/Build/badge.svg)
 [![PyPI version](https://badge.fury.io/py/tlv.svg)](https://badge.fury.io/py/tlv)
 [![Python version](https://img.shields.io/pypi/pyversions/tlv)](https://img.shields.io/pypi/pyversions/tlv)
```

### Comparing `tlv-1.5.2/README.md` & `tlv-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `tlv-1.5.2/setup.py` & `tlv-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="tlv",
-    version="1.5.2",
+    version="1.5.3",
     author="Konrad Weihmann",
     author_email="kweihmann@outlook.com",
     description="-- Too less variation -- Find duplicates in source code for various languages",
     long_description=_long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/priv-kweihmann/tlv",
     packages=setuptools.find_packages(),
```

### Comparing `tlv-1.5.2/tlv/arg_parser.py` & `tlv-1.5.3/tlv/arg_parser.py`

 * *Files identical despite different names*

### Comparing `tlv-1.5.2/tlv/cls_ast.py` & `tlv-1.5.3/tlv/cls_ast.py`

 * *Files identical despite different names*

### Comparing `tlv-1.5.2/tlv/lexer.py` & `tlv-1.5.3/tlv/lexer.py`

 * *Files identical despite different names*

### Comparing `tlv-1.5.2/tlv/src_parser.py` & `tlv-1.5.3/tlv/src_parser.py`

 * *Files identical despite different names*

### Comparing `tlv-1.5.2/tlv/tokens.py` & `tlv-1.5.3/tlv/tokens.py`

 * *Files identical despite different names*

### Comparing `tlv-1.5.2/tlv.egg-info/PKG-INFO` & `tlv-1.5.3/tlv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlv
-Version: 1.5.2
+Version: 1.5.3
 Summary: -- Too less variation -- Find duplicates in source code for various languages
 Home-page: https://github.com/priv-kweihmann/tlv
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Pygments~=2.17
+Requires-Dist: Pygments~=2.18
 Requires-Dist: chardet~=5.2
 
 # tlv
 
 ![Build status](https://github.com/priv-kweihmann/tlv/workflows/Build/badge.svg)
 [![PyPI version](https://badge.fury.io/py/tlv.svg)](https://badge.fury.io/py/tlv)
 [![Python version](https://img.shields.io/pypi/pyversions/tlv)](https://img.shields.io/pypi/pyversions/tlv)
```

