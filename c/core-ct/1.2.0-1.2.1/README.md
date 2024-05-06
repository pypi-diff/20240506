# Comparing `tmp/core_ct-1.2.0.tar.gz` & `tmp/core_ct-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_ct-1.2.0.tar", max compression
+gzip compressed data, was "core_ct-1.2.1.tar", max compression
```

## Comparing `core_ct-1.2.0.tar` & `core_ct-1.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1080 2024-04-22 21:34:15.496923 core_ct-1.2.0/LICENSE
--rw-r--r--   0        0        0     2593 2024-04-22 21:34:15.496923 core_ct-1.2.0/README.md
--rw-r--r--   0        0        0      981 2024-04-22 21:34:16.032928 core_ct-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       72 2024-04-22 21:34:16.032928 core_ct-1.2.0/src/core_ct/__init__.py
--rw-r--r--   0        0        0      747 2024-04-22 21:34:16.032928 core_ct-1.2.0/src/core_ct/analysis.py
--rw-r--r--   0        0        0    22849 2024-04-22 21:34:16.032928 core_ct-1.2.0/src/core_ct/core.py
--rw-r--r--   0        0        0     6274 2024-04-22 21:34:16.032928 core_ct-1.2.0/src/core_ct/importers.py
--rw-r--r--   0        0        0     4647 2024-04-22 21:34:16.036928 core_ct-1.2.0/src/core_ct/slice.py
--rw-r--r--   0        0        0     7286 2024-04-22 21:34:16.036928 core_ct-1.2.0/src/core_ct/visualize.py
--rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 core_ct-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-06 21:29:43.853330 core_ct-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2593 2024-05-06 21:29:43.853330 core_ct-1.2.1/README.md
+-rw-r--r--   0        0        0      981 2024-05-06 21:29:44.389333 core_ct-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-05-06 21:29:44.389333 core_ct-1.2.1/src/core_ct/__init__.py
+-rw-r--r--   0        0        0      747 2024-05-06 21:29:44.389333 core_ct-1.2.1/src/core_ct/analysis.py
+-rw-r--r--   0        0        0    22841 2024-05-06 21:29:44.389333 core_ct-1.2.1/src/core_ct/core.py
+-rw-r--r--   0        0        0     6274 2024-05-06 21:29:44.389333 core_ct-1.2.1/src/core_ct/importers.py
+-rw-r--r--   0        0        0     4647 2024-05-06 21:29:44.389333 core_ct-1.2.1/src/core_ct/slice.py
+-rw-r--r--   0        0        0     7286 2024-05-06 21:29:44.389333 core_ct-1.2.1/src/core_ct/visualize.py
+-rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 core_ct-1.2.1/PKG-INFO
```

### Comparing `core_ct-1.2.0/LICENSE` & `core_ct-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `core_ct-1.2.0/README.md` & `core_ct-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `core_ct-1.2.0/pyproject.toml` & `core_ct-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "core-ct"
-version = "1.2.0"
+version = "1.2.1"
 description = "A Python library to assist geologists with the analysis of rock core CT scans"
 authors = [
     "Kira Hanson <khanson@mines.edu>",
     "Carla Ellefsen <cellefsen@mines.edu>",
     "Connor Sparks <csparks@mines.edu>",
     "Asa Sprow <arsprow@mines.edu>",
 ]
```

### Comparing `core_ct-1.2.0/src/core_ct/analysis.py` & `core_ct-1.2.1/src/core_ct/analysis.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.2.0/src/core_ct/core.py` & `core_ct-1.2.1/src/core_ct/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,19 +298,19 @@
             y_center = int(self.data.shape[1] / 2)
         if z_center is None:
             z_center = int(self.data.shape[2] / 2)
 
         center: tuple[int, int, int] = (x_center, y_center, z_center)
 
         # make sure all indexes are within bounds
-        for axis, idx in enumerate(center):
-            if idx >= self.shape()[axis]:
+        for ax, idx in enumerate(center):
+            if idx >= self.shape()[ax]:
                 warnings.warn(
-                    f"Center index is out of bounds on axis {axis}, value is {idx} but "
-                    f"axis size is {self.shape()[axis]}"
+                    f"Center index is out of bounds on axis {ax}, value is {idx} but "
+                    f"axis size is {self.shape()[ax]}"
                     )
 
         starts: list[int] = [0] * 3
         ends: list[int] = [0] * 3
         for ax in range(0, 3):
             if ax == axis:
                 starts[ax] = 0
```

### Comparing `core_ct-1.2.0/src/core_ct/importers.py` & `core_ct-1.2.1/src/core_ct/importers.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.2.0/src/core_ct/slice.py` & `core_ct-1.2.1/src/core_ct/slice.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.2.0/src/core_ct/visualize.py` & `core_ct-1.2.1/src/core_ct/visualize.py`

 * *Files identical despite different names*

### Comparing `core_ct-1.2.0/PKG-INFO` & `core_ct-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-ct
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python library to assist geologists with the analysis of rock core CT scans
 License: MIT
 Author: Kira Hanson
 Author-email: khanson@mines.edu
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

