# Comparing `tmp/rastervision_aws_batch-0.30.0.tar.gz` & `tmp/rastervision_aws_batch-0.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastervision_aws_batch-0.30.0.tar", last modified: Wed Apr 10 22:11:08 2024, max compression
+gzip compressed data, was "rastervision_aws_batch-0.30.1.tar", last modified: Mon May  6 21:02:13 2024, max compression
```

## Comparing `rastervision_aws_batch-0.30.0.tar` & `rastervision_aws_batch-0.30.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.563693 rastervision_aws_batch-0.30.0/
--rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_aws_batch-0.30.0/MANIFEST.in
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      560 2024-04-10 22:11:08.563693 rastervision_aws_batch-0.30.0/PKG-INFO
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.559693 rastervision_aws_batch-0.30.0/rastervision/
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.563693 rastervision_aws_batch-0.30.0/rastervision/aws_batch/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      592 2024-04-06 20:13:30.000000 rastervision_aws_batch-0.30.0/rastervision/aws_batch/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6121 2024-04-10 21:55:10.000000 rastervision_aws_batch-0.30.0/rastervision/aws_batch/aws_batch_runner.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.563693 rastervision_aws_batch-0.30.0/rastervision_aws_batch.egg-info/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      560 2024-04-10 22:11:08.000000 rastervision_aws_batch-0.30.0/rastervision_aws_batch.egg-info/PKG-INFO
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      389 2024-04-10 22:11:08.000000 rastervision_aws_batch-0.30.0/rastervision_aws_batch.egg-info/SOURCES.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 22:11:08.000000 rastervision_aws_batch-0.30.0/rastervision_aws_batch.egg-info/dependency_links.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 21:24:48.000000 rastervision_aws_batch-0.30.0/rastervision_aws_batch.egg-info/not-zip-safe
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       35 2024-04-10 22:11:08.000000 rastervision_aws_batch-0.30.0/rastervision_aws_batch.egg-info/requires.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       24 2024-04-10 22:11:08.000000 rastervision_aws_batch-0.30.0/rastervision_aws_batch.egg-info/top_level.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       61 2024-04-10 21:55:10.000000 rastervision_aws_batch-0.30.0/requirements.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-04-10 22:11:08.563693 rastervision_aws_batch-0.30.0/setup.cfg
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1727 2024-04-10 21:55:10.000000 rastervision_aws_batch-0.30.0/setup.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.455120 rastervision_aws_batch-0.30.1/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_aws_batch-0.30.1/MANIFEST.in
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      560 2024-05-06 21:02:13.455120 rastervision_aws_batch-0.30.1/PKG-INFO
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.451120 rastervision_aws_batch-0.30.1/rastervision/
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.455120 rastervision_aws_batch-0.30.1/rastervision/aws_batch/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      592 2024-04-06 20:13:30.000000 rastervision_aws_batch-0.30.1/rastervision/aws_batch/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6121 2024-04-10 21:55:10.000000 rastervision_aws_batch-0.30.1/rastervision/aws_batch/aws_batch_runner.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.455120 rastervision_aws_batch-0.30.1/rastervision_aws_batch.egg-info/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      560 2024-05-06 21:02:13.000000 rastervision_aws_batch-0.30.1/rastervision_aws_batch.egg-info/PKG-INFO
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      389 2024-05-06 21:02:13.000000 rastervision_aws_batch-0.30.1/rastervision_aws_batch.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-05-06 21:02:13.000000 rastervision_aws_batch-0.30.1/rastervision_aws_batch.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-05-06 21:02:13.000000 rastervision_aws_batch-0.30.1/rastervision_aws_batch.egg-info/not-zip-safe
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       35 2024-05-06 21:02:13.000000 rastervision_aws_batch-0.30.1/rastervision_aws_batch.egg-info/requires.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       13 2024-05-06 21:02:13.000000 rastervision_aws_batch-0.30.1/rastervision_aws_batch.egg-info/top_level.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       61 2024-05-06 20:16:58.000000 rastervision_aws_batch-0.30.1/requirements.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-05-06 21:02:13.455120 rastervision_aws_batch-0.30.1/setup.cfg
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1727 2024-05-06 20:16:58.000000 rastervision_aws_batch-0.30.1/setup.py
```

### Comparing `rastervision_aws_batch-0.30.0/PKG-INFO` & `rastervision_aws_batch-0.30.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision_aws_batch
-Version: 0.30.0
+Version: 0.30.1
 Summary: A rastervision plugin that adds an AWS Batch pipeline runner
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_aws_batch-0.30.0/rastervision/aws_batch/__init__.py` & `rastervision_aws_batch-0.30.1/rastervision/aws_batch/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_aws_batch-0.30.0/rastervision/aws_batch/aws_batch_runner.py` & `rastervision_aws_batch-0.30.1/rastervision/aws_batch/aws_batch_runner.py`

 * *Files identical despite different names*

### Comparing `rastervision_aws_batch-0.30.0/rastervision_aws_batch.egg-info/PKG-INFO` & `rastervision_aws_batch-0.30.1/rastervision_aws_batch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision-aws-batch
-Version: 0.30.0
+Version: 0.30.1
 Summary: A rastervision plugin that adds an AWS Batch pipeline runner
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_aws_batch-0.30.0/setup.py` & `rastervision_aws_batch-0.30.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 from os.path import abspath, dirname, join
 from setuptools import setup, find_namespace_packages
 import re
 
 name = 'rastervision_aws_batch'
-version = '0.30.0'
+version = '0.30.1'
 description = 'A rastervision plugin that adds an AWS Batch pipeline runner'
 requirement_constraints = {}
 
 here = abspath(dirname(__file__))
 
 
 def parse_requirements(requirements_path: str) -> list[str]:
```

