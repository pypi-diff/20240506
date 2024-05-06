# Comparing `tmp/one4all_iop_models-0.1.8.tar.gz` & `tmp/one4all_iop_models-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one4all_iop_models-0.1.8.tar", max compression
+gzip compressed data, was "one4all_iop_models-0.1.9.tar", max compression
```

## Comparing `one4all_iop_models-0.1.8.tar` & `one4all_iop_models-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      364 2024-04-26 09:45:07.666647 one4all_iop_models-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-04-26 09:45:07.666647 one4all_iop_models-0.1.8/one4all_iop_models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 09:45:07.666647 one4all_iop_models-0.1.8/one4all_iop_models/ros_models/__init__.py
--rw-r--r--   0        0        0     1862 2024-04-26 09:45:07.670647 one4all_iop_models-0.1.8/one4all_iop_models/ros_models/robot.py
--rw-r--r--   0        0        0      547 2024-04-26 09:45:07.670647 one4all_iop_models-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 one4all_iop_models-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      364 2024-05-01 19:30:42.182986 one4all_iop_models-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-05-01 19:30:42.182986 one4all_iop_models-0.1.9/one4all_iop_models/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 19:30:42.182986 one4all_iop_models-0.1.9/one4all_iop_models/ros_models/__init__.py
+-rw-r--r--   0        0        0     1862 2024-05-01 19:30:42.182986 one4all_iop_models-0.1.9/one4all_iop_models/ros_models/robot.py
+-rw-r--r--   0        0        0      547 2024-05-01 19:30:42.182986 one4all_iop_models-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 one4all_iop_models-0.1.9/PKG-INFO
```

### Comparing `one4all_iop_models-0.1.8/one4all_iop_models/ros_models/robot.py` & `one4all_iop_models-0.1.9/one4all_iop_models/ros_models/robot.py`

 * *Files identical despite different names*

### Comparing `one4all_iop_models-0.1.8/pyproject.toml` & `one4all_iop_models-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "one4all-iop-models"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Ignacio Jimenez <ignacio.jimenez@idener.ai>"]
 readme = "README.md"
 packages = [{include = "one4all_iop_models"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `one4all_iop_models-0.1.8/PKG-INFO` & `one4all_iop_models-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one4all-iop-models
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Ignacio Jimenez
 Author-email: ignacio.jimenez@idener.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

