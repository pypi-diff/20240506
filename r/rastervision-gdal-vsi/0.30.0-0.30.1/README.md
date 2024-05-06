# Comparing `tmp/rastervision_gdal_vsi-0.30.0.tar.gz` & `tmp/rastervision_gdal_vsi-0.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastervision_gdal_vsi-0.30.0.tar", last modified: Wed Apr 10 22:11:09 2024, max compression
+gzip compressed data, was "rastervision_gdal_vsi-0.30.1.tar", last modified: Mon May  6 21:02:14 2024, max compression
```

## Comparing `rastervision_gdal_vsi-0.30.0.tar` & `rastervision_gdal_vsi-0.30.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.691690 rastervision_gdal_vsi-0.30.0/
--rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_gdal_vsi-0.30.0/MANIFEST.in
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      553 2024-04-10 22:11:09.691690 rastervision_gdal_vsi-0.30.0/PKG-INFO
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.687690 rastervision_gdal_vsi-0.30.0/rastervision/
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.691690 rastervision_gdal_vsi-0.30.0/rastervision/gdal_vsi/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      358 2023-08-24 18:41:21.000000 rastervision_gdal_vsi-0.30.0/rastervision/gdal_vsi/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7698 2024-04-07 00:38:15.000000 rastervision_gdal_vsi-0.30.0/rastervision/gdal_vsi/vsi_file_system.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.691690 rastervision_gdal_vsi-0.30.0/rastervision_gdal_vsi.egg-info/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      553 2024-04-10 22:11:09.000000 rastervision_gdal_vsi-0.30.0/rastervision_gdal_vsi.egg-info/PKG-INFO
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      380 2024-04-10 22:11:09.000000 rastervision_gdal_vsi-0.30.0/rastervision_gdal_vsi.egg-info/SOURCES.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 22:11:09.000000 rastervision_gdal_vsi-0.30.0/rastervision_gdal_vsi.egg-info/dependency_links.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 21:24:49.000000 rastervision_gdal_vsi-0.30.0/rastervision_gdal_vsi.egg-info/not-zip-safe
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       27 2024-04-10 22:11:09.000000 rastervision_gdal_vsi-0.30.0/rastervision_gdal_vsi.egg-info/requires.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       24 2024-04-10 22:11:09.000000 rastervision_gdal_vsi-0.30.0/rastervision_gdal_vsi.egg-info/top_level.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       50 2024-04-10 21:55:10.000000 rastervision_gdal_vsi-0.30.0/requirements.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-04-10 22:11:09.691690 rastervision_gdal_vsi-0.30.0/setup.cfg
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1720 2024-04-10 21:55:10.000000 rastervision_gdal_vsi-0.30.0/setup.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.575128 rastervision_gdal_vsi-0.30.1/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_gdal_vsi-0.30.1/MANIFEST.in
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      553 2024-05-06 21:02:14.575128 rastervision_gdal_vsi-0.30.1/PKG-INFO
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.571128 rastervision_gdal_vsi-0.30.1/rastervision/
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.571128 rastervision_gdal_vsi-0.30.1/rastervision/gdal_vsi/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      358 2023-08-24 18:41:21.000000 rastervision_gdal_vsi-0.30.1/rastervision/gdal_vsi/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7698 2024-04-07 00:38:15.000000 rastervision_gdal_vsi-0.30.1/rastervision/gdal_vsi/vsi_file_system.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.571128 rastervision_gdal_vsi-0.30.1/rastervision_gdal_vsi.egg-info/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      553 2024-05-06 21:02:14.000000 rastervision_gdal_vsi-0.30.1/rastervision_gdal_vsi.egg-info/PKG-INFO
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      380 2024-05-06 21:02:14.000000 rastervision_gdal_vsi-0.30.1/rastervision_gdal_vsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-05-06 21:02:14.000000 rastervision_gdal_vsi-0.30.1/rastervision_gdal_vsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-05-06 21:02:14.000000 rastervision_gdal_vsi-0.30.1/rastervision_gdal_vsi.egg-info/not-zip-safe
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       27 2024-05-06 21:02:14.000000 rastervision_gdal_vsi-0.30.1/rastervision_gdal_vsi.egg-info/requires.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       13 2024-05-06 21:02:14.000000 rastervision_gdal_vsi-0.30.1/rastervision_gdal_vsi.egg-info/top_level.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       50 2024-05-06 20:16:58.000000 rastervision_gdal_vsi-0.30.1/requirements.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-05-06 21:02:14.575128 rastervision_gdal_vsi-0.30.1/setup.cfg
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1720 2024-05-06 20:16:58.000000 rastervision_gdal_vsi-0.30.1/setup.py
```

### Comparing `rastervision_gdal_vsi-0.30.0/PKG-INFO` & `rastervision_gdal_vsi-0.30.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision_gdal_vsi
-Version: 0.30.0
+Version: 0.30.1
 Summary: A rastervision plugin that adds a GDAL VSI file system
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_gdal_vsi-0.30.0/rastervision/gdal_vsi/vsi_file_system.py` & `rastervision_gdal_vsi-0.30.1/rastervision/gdal_vsi/vsi_file_system.py`

 * *Files identical despite different names*

### Comparing `rastervision_gdal_vsi-0.30.0/setup.py` & `rastervision_gdal_vsi-0.30.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 from os.path import abspath, dirname, join
 from setuptools import setup, find_namespace_packages
 import re
 
 name = 'rastervision_gdal_vsi'
-version = '0.30.0'
+version = '0.30.1'
 description = 'A rastervision plugin that adds a GDAL VSI file system'
 requirement_constraints = {}
 
 here = abspath(dirname(__file__))
 
 
 def parse_requirements(requirements_path: str) -> list[str]:
```

