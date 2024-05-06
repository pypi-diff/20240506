# Comparing `tmp/phomo-0.4.5.tar.gz` & `tmp/phomo-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phomo-0.4.5.tar", max compression
+gzip compressed data, was "phomo-0.4.6.tar", max compression
```

## Comparing `phomo-0.4.5.tar` & `phomo-0.4.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-09-22 19:31:23.326734 phomo-0.4.5/LICENSE
--rw-r--r--   0        0        0     3948 2023-09-22 23:13:23.476798 phomo-0.4.5/README.md
--rw-r--r--   0        0        0      252 2023-09-22 23:13:23.476798 phomo-0.4.5/phomo/__init__.py
--rw-r--r--   0        0        0     4836 2022-01-14 16:40:00.300031 phomo-0.4.5/phomo/__main__.py
--rw-r--r--   0        0        0     6357 2023-09-22 22:30:39.853453 phomo-0.4.5/phomo/grid.py
--rw-r--r--   0        0        0     2631 2023-09-22 23:13:23.473465 phomo-0.4.5/phomo/master.py
--rw-r--r--   0        0        0     3465 2023-09-22 23:13:23.473465 phomo-0.4.5/phomo/metrics.py
--rw-r--r--   0        0        0    10980 2023-09-22 23:13:23.476798 phomo-0.4.5/phomo/mosaic.py
--rw-r--r--   0        0        0     2006 2023-09-22 23:13:23.476798 phomo-0.4.5/phomo/palette.py
--rw-r--r--   0        0        0     4233 2023-09-22 23:13:23.476798 phomo-0.4.5/phomo/pool.py
--rw-r--r--   0        0        0     4059 2023-09-22 23:13:23.476798 phomo-0.4.5/phomo/utils.py
--rw-r--r--   0        0        0     1043 2024-04-03 16:19:38.802877 phomo-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     5231 1970-01-01 00:00:00.000000 phomo-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-03 16:51:34.142816 phomo-0.4.6/LICENSE
+-rw-r--r--   0        0        0     3948 2023-09-22 23:13:23.476798 phomo-0.4.6/README.md
+-rw-r--r--   0        0        0      252 2023-09-22 23:13:23.476798 phomo-0.4.6/phomo/__init__.py
+-rw-r--r--   0        0        0     4836 2022-01-14 16:40:00.300031 phomo-0.4.6/phomo/__main__.py
+-rw-r--r--   0        0        0     6357 2023-09-22 22:30:39.853453 phomo-0.4.6/phomo/grid.py
+-rw-r--r--   0        0        0     2631 2023-09-22 23:13:23.473465 phomo-0.4.6/phomo/master.py
+-rw-r--r--   0        0        0     3465 2023-09-22 23:13:23.473465 phomo-0.4.6/phomo/metrics.py
+-rw-r--r--   0        0        0    10980 2023-09-22 23:13:23.476798 phomo-0.4.6/phomo/mosaic.py
+-rw-r--r--   0        0        0     2006 2023-09-22 23:13:23.476798 phomo-0.4.6/phomo/palette.py
+-rw-r--r--   0        0        0     4233 2023-09-22 23:13:23.476798 phomo-0.4.6/phomo/pool.py
+-rw-r--r--   0        0        0     4059 2023-09-22 23:13:23.476798 phomo-0.4.6/phomo/utils.py
+-rw-r--r--   0        0        0     1043 2024-05-06 20:58:59.753747 phomo-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     5231 1970-01-01 00:00:00.000000 phomo-0.4.6/PKG-INFO
```

### Comparing `phomo-0.4.5/LICENSE` & `phomo-0.4.6/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023, Loic Coyle
+Copyright (c) 2024, Loic Coyle
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `phomo-0.4.5/README.md` & `phomo-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `phomo-0.4.5/phomo/__main__.py` & `phomo-0.4.6/phomo/__main__.py`

 * *Files identical despite different names*

### Comparing `phomo-0.4.5/phomo/grid.py` & `phomo-0.4.6/phomo/grid.py`

 * *Files identical despite different names*

### Comparing `phomo-0.4.5/phomo/master.py` & `phomo-0.4.6/phomo/master.py`

 * *Files identical despite different names*

### Comparing `phomo-0.4.5/phomo/metrics.py` & `phomo-0.4.6/phomo/metrics.py`

 * *Files identical despite different names*

### Comparing `phomo-0.4.5/phomo/mosaic.py` & `phomo-0.4.6/phomo/mosaic.py`

 * *Files identical despite different names*

### Comparing `phomo-0.4.5/phomo/palette.py` & `phomo-0.4.6/phomo/palette.py`

 * *Files identical despite different names*

### Comparing `phomo-0.4.5/phomo/pool.py` & `phomo-0.4.6/phomo/pool.py`

 * *Files identical despite different names*

### Comparing `phomo-0.4.5/phomo/utils.py` & `phomo-0.4.6/phomo/utils.py`

 * *Files identical despite different names*

### Comparing `phomo-0.4.5/pyproject.toml` & `phomo-0.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phomo"
-version = "0.4.5"
+version = "0.4.6"
 description = "Python package and CLI utility to create photo mosaics."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/phomo"
 keywords = ["photomosaic", "photographic", "mosaic", "art", "image"]
 classifiers = [
```

### Comparing `phomo-0.4.5/PKG-INFO` & `phomo-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phomo
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python package and CLI utility to create photo mosaics.
 Home-page: https://github.com/loiccoyle/phomo
 License: MIT
 Keywords: photomosaic,photographic,mosaic,art,image
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9,<3.13
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phomo Version: 0.4.5 Summary: Python package and
+Metadata-Version: 2.1 Name: phomo Version: 0.4.6 Summary: Python package and
 CLI utility to create photo mosaics. Home-page: https://github.com/loiccoyle/
 phomo License: MIT Keywords: photomosaic,photographic,mosaic,art,image Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: MacOS Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

