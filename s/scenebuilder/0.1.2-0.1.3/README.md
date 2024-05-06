# Comparing `tmp/scenebuilder-0.1.2.tar.gz` & `tmp/scenebuilder-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenebuilder-0.1.2.tar", max compression
+gzip compressed data, was "scenebuilder-0.1.3.tar", max compression
```

## Comparing `scenebuilder-0.1.2.tar` & `scenebuilder-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-10-19 10:53:34.751175 scenebuilder-0.1.2/LICENSE
--rw-r--r--   0        0        0     3443 2024-05-05 23:21:43.167541 scenebuilder-0.1.2/README.md
--rw-r--r--   0        0        0      369 2024-05-05 23:20:37.771987 scenebuilder-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       38 2024-05-05 17:53:13.810692 scenebuilder-0.1.2/scenebuilder/__init__.py
--rw-r--r--   0        0        0      851 2024-05-05 23:20:30.173794 scenebuilder-0.1.2/scenebuilder/actions_stack.py
--rw-r--r--   0        0        0     4262 2024-05-05 23:20:28.835485 scenebuilder-0.1.2/scenebuilder/construction.py
--rw-r--r--   0        0        0     4909 2024-05-05 23:20:22.042742 scenebuilder-0.1.2/scenebuilder/entities.py
--rw-r--r--   0        0        0      454 2024-05-05 23:20:17.691922 scenebuilder-0.1.2/scenebuilder/mixins.py
--rw-r--r--   0        0        0     2204 2024-05-05 23:20:15.139535 scenebuilder-0.1.2/scenebuilder/observer_utils.py
--rw-r--r--   0        0        0     4341 2024-05-05 23:20:14.044613 scenebuilder-0.1.2/scenebuilder/patches.py
--rw-r--r--   0        0        0    20431 2024-05-05 23:24:43.233779 scenebuilder-0.1.2/scenebuilder/scenebuilder.py
--rw-r--r--   0        0        0     1711 2024-05-05 23:20:11.172433 scenebuilder-0.1.2/scenebuilder/ui_components.py
--rw-r--r--   0        0        0     3449 2024-05-05 18:55:06.173234 scenebuilder-0.1.2/scenebuilder/utils.py
--rw-r--r--   0        0        0     3868 1970-01-01 00:00:00.000000 scenebuilder-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-19 10:53:34.751175 scenebuilder-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3443 2024-05-05 23:21:43.167541 scenebuilder-0.1.3/README.md
+-rw-r--r--   0        0        0      473 2024-05-05 23:52:00.762314 scenebuilder-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       38 2024-05-05 17:53:13.810692 scenebuilder-0.1.3/scenebuilder/__init__.py
+-rw-r--r--   0        0        0      851 2024-05-05 23:20:30.173794 scenebuilder-0.1.3/scenebuilder/actions_stack.py
+-rw-r--r--   0        0        0     4262 2024-05-05 23:20:28.835485 scenebuilder-0.1.3/scenebuilder/construction.py
+-rw-r--r--   0        0        0     4909 2024-05-05 23:20:22.042742 scenebuilder-0.1.3/scenebuilder/entities.py
+-rw-r--r--   0        0        0      454 2024-05-05 23:20:17.691922 scenebuilder-0.1.3/scenebuilder/mixins.py
+-rw-r--r--   0        0        0     2204 2024-05-05 23:20:15.139535 scenebuilder-0.1.3/scenebuilder/observer_utils.py
+-rw-r--r--   0        0        0     4341 2024-05-05 23:20:14.044613 scenebuilder-0.1.3/scenebuilder/patches.py
+-rw-r--r--   0        0        0    20431 2024-05-05 23:24:43.233779 scenebuilder-0.1.3/scenebuilder/scenebuilder.py
+-rw-r--r--   0        0        0     1711 2024-05-05 23:20:11.172433 scenebuilder-0.1.3/scenebuilder/ui_components.py
+-rw-r--r--   0        0        0     3449 2024-05-05 18:55:06.173234 scenebuilder-0.1.3/scenebuilder/utils.py
+-rw-r--r--   0        0        0     3972 1970-01-01 00:00:00.000000 scenebuilder-0.1.3/PKG-INFO
```

### Comparing `scenebuilder-0.1.2/LICENSE` & `scenebuilder-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.1.2/README.md` & `scenebuilder-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.1.2/scenebuilder/actions_stack.py` & `scenebuilder-0.1.3/scenebuilder/actions_stack.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.1.2/scenebuilder/construction.py` & `scenebuilder-0.1.3/scenebuilder/construction.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.1.2/scenebuilder/entities.py` & `scenebuilder-0.1.3/scenebuilder/entities.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.1.2/scenebuilder/observer_utils.py` & `scenebuilder-0.1.3/scenebuilder/observer_utils.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.1.2/scenebuilder/patches.py` & `scenebuilder-0.1.3/scenebuilder/patches.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.1.2/scenebuilder/scenebuilder.py` & `scenebuilder-0.1.3/scenebuilder/scenebuilder.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.1.2/scenebuilder/ui_components.py` & `scenebuilder-0.1.3/scenebuilder/ui_components.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.1.2/scenebuilder/utils.py` & `scenebuilder-0.1.3/scenebuilder/utils.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.1.2/PKG-INFO` & `scenebuilder-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: scenebuilder
-Version: 0.1.2
-Summary: 
+Version: 0.1.3
+Summary: A simple GUI to create 2D scenes with obstacles and drone paths for multi-agent path planning algorithms
 Author: Adrian del Ser
 Author-email: adrian.delser@gmail.com
 Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: matplotlib (>=3.8.0,<4.0.0)
```

