# Comparing `tmp/pyjhtdbv2-20230505.0.tar.gz` & `tmp/pyjhtdbv2-20230506.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjhtdbv2-20230505.0.tar", max compression
+gzip compressed data, was "pyjhtdbv2-20230506.0.tar", max compression
```

## Comparing `pyjhtdbv2-20230505.0.tar` & `pyjhtdbv2-20230506.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    21485 2024-05-05 18:30:57.418121 pyjhtdbv2-20230505.0/C/local_tools.c
--rw-r--r--   0        0        0    11323 2024-05-05 18:30:57.418257 pyjhtdbv2-20230505.0/LICENSE
--rw-r--r--   0        0        0     3013 2024-05-05 18:30:57.418344 pyjhtdbv2-20230505.0/README.md
--rw-r--r--   0        0        0     2214 2024-05-05 18:30:57.446934 pyjhtdbv2-20230505.0/pyJHTDB/MortonIndex.py
--rw-r--r--   0        0        0     3468 2024-05-05 18:33:04.019377 pyjhtdbv2-20230505.0/pyJHTDB/__init__.py
--rw-r--r--   0        0        0    30030 2024-05-05 18:30:57.447211 pyjhtdbv2-20230505.0/pyJHTDB/data/big_channel_Y_COOR.txt
--rw-r--r--   0        0        0    28495 2024-05-05 18:30:57.447367 pyjhtdbv2-20230505.0/pyJHTDB/data/channel5200_Y_COOR.txt
--rw-r--r--   0        0        0     6272 2024-05-05 18:30:57.447452 pyjhtdbv2-20230505.0/pyJHTDB/data/channel5200_ygrid.npy
--rw-r--r--   0        0        0    34912 2024-05-05 18:30:57.447656 pyjhtdbv2-20230505.0/pyJHTDB/data/channel_grid.h5
--rw-r--r--   0        0        0     8272 2024-05-05 18:30:57.447769 pyjhtdbv2-20230505.0/pyJHTDB/data/channel_xgrid.npy
--rw-r--r--   0        0        0     2128 2024-05-05 18:30:57.447837 pyjhtdbv2-20230505.0/pyJHTDB/data/channel_ygrid.npy
--rw-r--r--   0        0        0     6224 2024-05-05 18:30:57.447924 pyjhtdbv2-20230505.0/pyJHTDB/data/channel_zgrid.npy
--rw-r--r--   0        0        0      418 2024-05-05 18:30:57.447985 pyjhtdbv2-20230505.0/pyJHTDB/data/convert.py
--rw-r--r--   0        0        0     5264 2024-05-05 18:30:57.448055 pyjhtdbv2-20230505.0/pyJHTDB/data/convert2.py
--rw-r--r--   0        0        0     3885 2024-05-05 18:30:57.448117 pyjhtdbv2-20230505.0/pyJHTDB/data/transition_bl_Y_COORD.txt
--rw-r--r--   0        0        0     1024 2024-05-05 18:30:57.448170 pyjhtdbv2-20230505.0/pyJHTDB/data/transition_bl_ygrid.npy
--rw-r--r--   0        0        0     9278 2024-05-05 18:30:57.448292 pyjhtdbv2-20230505.0/pyJHTDB/dbinfo.py
--rw-r--r--   0        0        0    17025 2024-05-05 18:30:57.448438 pyjhtdbv2-20230505.0/pyJHTDB/generic_splines.py
--rw-r--r--   0        0        0    28111 2024-05-05 18:30:57.448596 pyjhtdbv2-20230505.0/pyJHTDB/interpolator.py
--rw-r--r--   0        0        0    43272 2024-05-05 18:30:57.448807 pyjhtdbv2-20230505.0/pyJHTDB/libJHTDB.py
--rw-r--r--   0        0        0     1864 2024-05-05 18:30:57.448884 pyjhtdbv2-20230505.0/pyJHTDB/misc.py
--rw-r--r--   0        0        0    37105 2024-05-05 18:30:57.449220 pyjhtdbv2-20230505.0/pyJHTDB/test.py
--rw-r--r--   0        0        0    23795 2024-05-05 18:30:57.449354 pyjhtdbv2-20230505.0/pyJHTDB/test_data.py
--rw-r--r--   0        0        0     1167 2024-05-06 13:09:00.068187 pyjhtdbv2-20230505.0/pyproject.toml
--rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 pyjhtdbv2-20230505.0/PKG-INFO
+-rw-r--r--   0        0        0    21485 2024-05-05 18:30:57.418121 pyjhtdbv2-20230506.0/C/local_tools.c
+-rw-r--r--   0        0        0    11323 2024-05-05 18:30:57.418257 pyjhtdbv2-20230506.0/LICENSE
+-rw-r--r--   0        0        0     3013 2024-05-05 18:30:57.418344 pyjhtdbv2-20230506.0/README.md
+-rw-r--r--   0        0        0     2214 2024-05-05 18:30:57.446934 pyjhtdbv2-20230506.0/pyJHTDB/MortonIndex.py
+-rw-r--r--   0        0        0     3468 2024-05-05 18:33:04.019377 pyjhtdbv2-20230506.0/pyJHTDB/__init__.py
+-rw-r--r--   0        0        0    30030 2024-05-05 18:30:57.447211 pyjhtdbv2-20230506.0/pyJHTDB/data/big_channel_Y_COOR.txt
+-rw-r--r--   0        0        0    28495 2024-05-05 18:30:57.447367 pyjhtdbv2-20230506.0/pyJHTDB/data/channel5200_Y_COOR.txt
+-rw-r--r--   0        0        0     6272 2024-05-05 18:30:57.447452 pyjhtdbv2-20230506.0/pyJHTDB/data/channel5200_ygrid.npy
+-rw-r--r--   0        0        0    34912 2024-05-05 18:30:57.447656 pyjhtdbv2-20230506.0/pyJHTDB/data/channel_grid.h5
+-rw-r--r--   0        0        0     8272 2024-05-05 18:30:57.447769 pyjhtdbv2-20230506.0/pyJHTDB/data/channel_xgrid.npy
+-rw-r--r--   0        0        0     2128 2024-05-05 18:30:57.447837 pyjhtdbv2-20230506.0/pyJHTDB/data/channel_ygrid.npy
+-rw-r--r--   0        0        0     6224 2024-05-05 18:30:57.447924 pyjhtdbv2-20230506.0/pyJHTDB/data/channel_zgrid.npy
+-rw-r--r--   0        0        0      418 2024-05-05 18:30:57.447985 pyjhtdbv2-20230506.0/pyJHTDB/data/convert.py
+-rw-r--r--   0        0        0     5264 2024-05-05 18:30:57.448055 pyjhtdbv2-20230506.0/pyJHTDB/data/convert2.py
+-rw-r--r--   0        0        0     3885 2024-05-05 18:30:57.448117 pyjhtdbv2-20230506.0/pyJHTDB/data/transition_bl_Y_COORD.txt
+-rw-r--r--   0        0        0     1024 2024-05-05 18:30:57.448170 pyjhtdbv2-20230506.0/pyJHTDB/data/transition_bl_ygrid.npy
+-rw-r--r--   0        0        0     9278 2024-05-05 18:30:57.448292 pyjhtdbv2-20230506.0/pyJHTDB/dbinfo.py
+-rw-r--r--   0        0        0    17025 2024-05-05 18:30:57.448438 pyjhtdbv2-20230506.0/pyJHTDB/generic_splines.py
+-rw-r--r--   0        0        0    28111 2024-05-05 18:30:57.448596 pyjhtdbv2-20230506.0/pyJHTDB/interpolator.py
+-rw-r--r--   0        0        0    43272 2024-05-05 18:30:57.448807 pyjhtdbv2-20230506.0/pyJHTDB/libJHTDB.py
+-rw-r--r--   0        0        0     1864 2024-05-05 18:30:57.448884 pyjhtdbv2-20230506.0/pyJHTDB/misc.py
+-rw-r--r--   0        0        0    37105 2024-05-05 18:30:57.449220 pyjhtdbv2-20230506.0/pyJHTDB/test.py
+-rw-r--r--   0        0        0    23795 2024-05-05 18:30:57.449354 pyjhtdbv2-20230506.0/pyJHTDB/test_data.py
+-rw-r--r--   0        0        0     1214 2024-05-06 13:23:08.365525 pyjhtdbv2-20230506.0/pyproject.toml
+-rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 pyjhtdbv2-20230506.0/PKG-INFO
```

### Comparing `pyjhtdbv2-20230505.0/C/local_tools.c` & `pyjhtdbv2-20230506.0/C/local_tools.c`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/LICENSE` & `pyjhtdbv2-20230506.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/README.md` & `pyjhtdbv2-20230506.0/README.md`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/MortonIndex.py` & `pyjhtdbv2-20230506.0/pyJHTDB/MortonIndex.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/__init__.py` & `pyjhtdbv2-20230506.0/pyJHTDB/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/data/big_channel_Y_COOR.txt` & `pyjhtdbv2-20230506.0/pyJHTDB/data/big_channel_Y_COOR.txt`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/data/channel5200_Y_COOR.txt` & `pyjhtdbv2-20230506.0/pyJHTDB/data/channel5200_Y_COOR.txt`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/data/channel5200_ygrid.npy` & `pyjhtdbv2-20230506.0/pyJHTDB/data/channel5200_ygrid.npy`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/data/channel_grid.h5` & `pyjhtdbv2-20230506.0/pyJHTDB/data/channel_grid.h5`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/data/channel_xgrid.npy` & `pyjhtdbv2-20230506.0/pyJHTDB/data/channel_xgrid.npy`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/data/channel_ygrid.npy` & `pyjhtdbv2-20230506.0/pyJHTDB/data/channel_ygrid.npy`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/data/channel_zgrid.npy` & `pyjhtdbv2-20230506.0/pyJHTDB/data/channel_zgrid.npy`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/data/convert2.py` & `pyjhtdbv2-20230506.0/pyJHTDB/data/convert2.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/data/transition_bl_Y_COORD.txt` & `pyjhtdbv2-20230506.0/pyJHTDB/data/transition_bl_Y_COORD.txt`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/data/transition_bl_ygrid.npy` & `pyjhtdbv2-20230506.0/pyJHTDB/data/transition_bl_ygrid.npy`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/dbinfo.py` & `pyjhtdbv2-20230506.0/pyJHTDB/dbinfo.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/generic_splines.py` & `pyjhtdbv2-20230506.0/pyJHTDB/generic_splines.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/interpolator.py` & `pyjhtdbv2-20230506.0/pyJHTDB/interpolator.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/libJHTDB.py` & `pyjhtdbv2-20230506.0/pyJHTDB/libJHTDB.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/misc.py` & `pyjhtdbv2-20230506.0/pyJHTDB/misc.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/test.py` & `pyjhtdbv2-20230506.0/pyJHTDB/test.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyJHTDB/test_data.py` & `pyjhtdbv2-20230506.0/pyJHTDB/test_data.py`

 * *Files identical despite different names*

### Comparing `pyjhtdbv2-20230505.0/pyproject.toml` & `pyjhtdbv2-20230506.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyjhtdbv2"
-version = "20230505.0"
+version = "20230506.0"
 description = "Python wrapper for the Johns Hopkins turbulence database library"
 authors = ["Johns Hopkins Turbulence Database Group <turbulence@pha.jhu.edu>"]
 license = "Apache License 2.0"
 packages = [
     { include = "pyJHTDB", from = "." },
 ]
 readme = "README.md"
@@ -17,14 +17,16 @@
     {path = "C/local_tools.c"},
     {path = "turbolib/turblib.c"},
     {path = "turbolib/soapC.c"},
     {path = "turbolib/soapClient.c"},
     {path = "turbolib/stdsoap2.c"},
     {path = "turbolib/*.h"},
     {path = "turbolib/*.nsmap"},
+    {path = "pyJHTDB/*.so", format = "wheel"}
+
 ]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 numpy = ">=1.15.0"
 scipy = ">=1.1.0"
 sympy = ">=1.2"
```

### Comparing `pyjhtdbv2-20230505.0/PKG-INFO` & `pyjhtdbv2-20230506.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjhtdbv2
-Version: 20230505.0
+Version: 20230506.0
 Summary: Python wrapper for the Johns Hopkins turbulence database library
 License: Apache-2.0
 Author: Johns Hopkins Turbulence Database Group
 Author-email: turbulence@pha.jhu.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

