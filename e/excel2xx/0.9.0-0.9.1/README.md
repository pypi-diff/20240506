# Comparing `tmp/excel2xx-0.9.0.tar.gz` & `tmp/excel2xx-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel2xx-0.9.0.tar", last modified: Wed Aug 16 06:17:40 2023, max compression
+gzip compressed data, was "excel2xx-0.9.1.tar", last modified: Wed Aug 16 09:04:20 2023, max compression
```

## Comparing `excel2xx-0.9.0.tar` & `excel2xx-0.9.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 cupen     (1000) cupen     (1000)        0 2023-08-16 06:17:40.906252 excel2xx-0.9.0/
--rw-r--r--   0 cupen     (1000) cupen     (1000)      482 2023-08-16 02:41:04.000000 excel2xx-0.9.0/LICENSE
--rw-r--r--   0 cupen     (1000) cupen     (1000)     4878 2023-08-16 06:17:40.906252 excel2xx-0.9.0/PKG-INFO
--rw-r--r--   0 cupen     (1000) cupen     (1000)     3859 2023-08-16 02:41:04.000000 excel2xx-0.9.0/README.md
-drwxr-xr-x   0 cupen     (1000) cupen     (1000)        0 2023-08-16 06:17:40.906252 excel2xx-0.9.0/excel2xx/
--rw-r--r--   0 cupen     (1000) cupen     (1000)     8811 2023-08-16 06:16:34.000000 excel2xx-0.9.0/excel2xx/__init__.py
--rw-r--r--   0 cupen     (1000) cupen     (1000)      330 2023-08-16 02:41:04.000000 excel2xx-0.9.0/excel2xx/__main__.py
--rw-r--r--   0 cupen     (1000) cupen     (1000)     1576 2023-08-16 02:41:04.000000 excel2xx-0.9.0/excel2xx/export.py
--rw-r--r--   0 cupen     (1000) cupen     (1000)      534 2023-08-16 06:15:50.000000 excel2xx-0.9.0/excel2xx/exportor.py
--rw-r--r--   0 cupen     (1000) cupen     (1000)    12604 2023-08-16 04:59:00.000000 excel2xx-0.9.0/excel2xx/fields.py
--rw-r--r--   0 cupen     (1000) cupen     (1000)     1951 2023-08-16 02:41:04.000000 excel2xx-0.9.0/excel2xx/main.py
--rw-r--r--   0 cupen     (1000) cupen     (1000)       98 2023-08-16 02:41:04.000000 excel2xx-0.9.0/excel2xx/utils.py
-drwxr-xr-x   0 cupen     (1000) cupen     (1000)        0 2023-08-16 06:17:40.906252 excel2xx-0.9.0/excel2xx.egg-info/
--rw-r--r--   0 cupen     (1000) cupen     (1000)     4878 2023-08-16 06:17:40.000000 excel2xx-0.9.0/excel2xx.egg-info/PKG-INFO
--rw-r--r--   0 cupen     (1000) cupen     (1000)      405 2023-08-16 06:17:40.000000 excel2xx-0.9.0/excel2xx.egg-info/SOURCES.txt
--rw-r--r--   0 cupen     (1000) cupen     (1000)        1 2023-08-16 06:17:40.000000 excel2xx-0.9.0/excel2xx.egg-info/dependency_links.txt
--rw-r--r--   0 cupen     (1000) cupen     (1000)       55 2023-08-16 06:17:40.000000 excel2xx-0.9.0/excel2xx.egg-info/entry_points.txt
--rw-r--r--   0 cupen     (1000) cupen     (1000)       60 2023-08-16 06:17:40.000000 excel2xx-0.9.0/excel2xx.egg-info/requires.txt
--rw-r--r--   0 cupen     (1000) cupen     (1000)        9 2023-08-16 06:17:40.000000 excel2xx-0.9.0/excel2xx.egg-info/top_level.txt
--rw-r--r--   0 cupen     (1000) cupen     (1000)       67 2023-08-16 06:17:40.906252 excel2xx-0.9.0/setup.cfg
--rw-r--r--   0 cupen     (1000) cupen     (1000)     1540 2023-08-16 06:17:36.000000 excel2xx-0.9.0/setup.py
-drwxr-xr-x   0 cupen     (1000) cupen     (1000)        0 2023-08-16 06:17:40.906252 excel2xx-0.9.0/tests/
--rw-r--r--   0 cupen     (1000) cupen     (1000)       32 2023-08-16 02:41:04.000000 excel2xx-0.9.0/tests/test_abc.py
--rw-r--r--   0 cupen     (1000) cupen     (1000)      355 2023-08-16 05:00:12.000000 excel2xx-0.9.0/tests/test_fields.py
+drwxr-xr-x   0 cupen     (1000) cupen     (1000)        0 2023-08-16 09:04:20.886012 excel2xx-0.9.1/
+-rw-r--r--   0 cupen     (1000) cupen     (1000)      482 2023-08-16 02:41:04.000000 excel2xx-0.9.1/LICENSE
+-rw-r--r--   0 cupen     (1000) cupen     (1000)     4878 2023-08-16 09:04:20.886012 excel2xx-0.9.1/PKG-INFO
+-rw-r--r--   0 cupen     (1000) cupen     (1000)     3859 2023-08-16 02:41:04.000000 excel2xx-0.9.1/README.md
+drwxr-xr-x   0 cupen     (1000) cupen     (1000)        0 2023-08-16 09:04:20.886012 excel2xx-0.9.1/excel2xx/
+-rw-r--r--   0 cupen     (1000) cupen     (1000)     5838 2023-08-16 08:50:40.000000 excel2xx-0.9.1/excel2xx/__init__.py
+-rw-r--r--   0 cupen     (1000) cupen     (1000)      330 2023-08-16 02:41:04.000000 excel2xx-0.9.1/excel2xx/__main__.py
+-rw-r--r--   0 cupen     (1000) cupen     (1000)     1576 2023-08-16 02:41:04.000000 excel2xx-0.9.1/excel2xx/export.py
+-rw-r--r--   0 cupen     (1000) cupen     (1000)      674 2023-08-16 08:49:17.000000 excel2xx-0.9.1/excel2xx/exportor.py
+-rw-r--r--   0 cupen     (1000) cupen     (1000)     3217 2023-08-16 08:51:00.000000 excel2xx-0.9.1/excel2xx/fieldmeta.py
+-rw-r--r--   0 cupen     (1000) cupen     (1000)    12627 2023-08-16 08:49:35.000000 excel2xx-0.9.1/excel2xx/fields.py
+-rw-r--r--   0 cupen     (1000) cupen     (1000)     1951 2023-08-16 02:41:04.000000 excel2xx-0.9.1/excel2xx/main.py
+-rw-r--r--   0 cupen     (1000) cupen     (1000)       98 2023-08-16 02:41:04.000000 excel2xx-0.9.1/excel2xx/utils.py
+drwxr-xr-x   0 cupen     (1000) cupen     (1000)        0 2023-08-16 09:04:20.886012 excel2xx-0.9.1/excel2xx.egg-info/
+-rw-r--r--   0 cupen     (1000) cupen     (1000)     4878 2023-08-16 09:04:20.000000 excel2xx-0.9.1/excel2xx.egg-info/PKG-INFO
+-rw-r--r--   0 cupen     (1000) cupen     (1000)      427 2023-08-16 09:04:20.000000 excel2xx-0.9.1/excel2xx.egg-info/SOURCES.txt
+-rw-r--r--   0 cupen     (1000) cupen     (1000)        1 2023-08-16 09:04:20.000000 excel2xx-0.9.1/excel2xx.egg-info/dependency_links.txt
+-rw-r--r--   0 cupen     (1000) cupen     (1000)       55 2023-08-16 09:04:20.000000 excel2xx-0.9.1/excel2xx.egg-info/entry_points.txt
+-rw-r--r--   0 cupen     (1000) cupen     (1000)       60 2023-08-16 09:04:20.000000 excel2xx-0.9.1/excel2xx.egg-info/requires.txt
+-rw-r--r--   0 cupen     (1000) cupen     (1000)        9 2023-08-16 09:04:20.000000 excel2xx-0.9.1/excel2xx.egg-info/top_level.txt
+-rw-r--r--   0 cupen     (1000) cupen     (1000)       67 2023-08-16 09:04:20.886012 excel2xx-0.9.1/setup.cfg
+-rw-r--r--   0 cupen     (1000) cupen     (1000)     1540 2023-08-16 09:03:41.000000 excel2xx-0.9.1/setup.py
+drwxr-xr-x   0 cupen     (1000) cupen     (1000)        0 2023-08-16 09:04:20.886012 excel2xx-0.9.1/tests/
+-rw-r--r--   0 cupen     (1000) cupen     (1000)       32 2023-08-16 02:41:04.000000 excel2xx-0.9.1/tests/test_abc.py
+-rw-r--r--   0 cupen     (1000) cupen     (1000)      355 2023-08-16 05:00:12.000000 excel2xx-0.9.1/tests/test_fields.py
```

### Comparing `excel2xx-0.9.0/PKG-INFO` & `excel2xx-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel2xx
-Version: 0.9.0
+Version: 0.9.1
 Summary: Extract data from excel file, and export to json, msgpack, or any code(mako template).
 Home-page: https://github.com/cupen/excel2xx
 Author: cupen
 Author-email: xcupen@gmail.com
 License: WTFPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `excel2xx-0.9.0/README.md` & `excel2xx-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `excel2xx-0.9.0/excel2xx/export.py` & `excel2xx-0.9.1/excel2xx/export.py`

 * *Files identical despite different names*

### Comparing `excel2xx-0.9.0/excel2xx/fields.py` & `excel2xx-0.9.1/excel2xx/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# coding:utf-8
+# coding=utf-8
 from __future__ import unicode_literals, print_function
 
 import datetime
 import re
 import json
 import math
 from collections import namedtuple, OrderedDict
@@ -29,14 +29,17 @@
         if typeName == "string":
             return str
         if typeName == "float":
             return float
         if typeName == "ItemExpr":
             return ItemExpr("as_type", typeName).format
         raise Exception("Invalid type %s" % typeName)
+        pass
+
+    pass
 
 
 class Int(Field):
     def format(self, v):
         return int(v)
```

### Comparing `excel2xx-0.9.0/excel2xx/main.py` & `excel2xx-0.9.1/excel2xx/main.py`

 * *Files identical despite different names*

### Comparing `excel2xx-0.9.0/excel2xx.egg-info/PKG-INFO` & `excel2xx-0.9.1/excel2xx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel2xx
-Version: 0.9.0
+Version: 0.9.1
 Summary: Extract data from excel file, and export to json, msgpack, or any code(mako template).
 Home-page: https://github.com/cupen/excel2xx
 Author: cupen
 Author-email: xcupen@gmail.com
 License: WTFPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `excel2xx-0.9.0/setup.py` & `excel2xx-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 fpath = os.path.join(os.path.dirname(__file__), "README.md")
 readme = open(fpath, "r", encoding="utf-8").read()
 
 
 setup(
     name="excel2xx",
-    version="0.9.0",
+    version="0.9.1",
     packages=["excel2xx"],
     url="https://github.com/cupen/excel2xx",
     license="WTFPL",
     author="cupen",
     author_email="xcupen@gmail.com",
     description="Extract data from excel file, and export to json, msgpack, or any code(mako template).",
     long_description=readme,
```

