# Comparing `tmp/astro_SPLASH-0.0.8.tar.gz` & `tmp/astro_SPLASH-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_SPLASH-0.0.8.tar", last modified: Mon May  6 04:53:05 2024, max compression
+gzip compressed data, was "astro_SPLASH-0.0.9.tar", last modified: Mon May  6 04:58:49 2024, max compression
```

## Comparing `astro_SPLASH-0.0.8.tar` & `astro_SPLASH-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:53:05.832371 astro_SPLASH-0.0.8/
--rw-r--r--   0 adamboesky   (501) staff       (20)      372 2024-05-06 04:53:05.831882 astro_SPLASH-0.0.8/PKG-INFO
-drwxr-xr-x   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:53:05.827757 astro_SPLASH-0.0.8/SPLASH/
--rw-r--r--   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:19:09.000000 astro_SPLASH-0.0.8/SPLASH/__init__.py
--rw-r--r--   0 adamboesky   (501) staff       (20)     1068 2024-05-06 04:50:42.000000 astro_SPLASH-0.0.8/SPLASH/network_utils.py
--rw-r--r--   0 adamboesky   (501) staff       (20)    12047 2024-05-06 04:52:16.000000 astro_SPLASH-0.0.8/SPLASH/pipeline.py
-drwxr-xr-x   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:53:05.828637 astro_SPLASH-0.0.8/SPLASH/trained_models/
--rw-r--r--   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:19:22.000000 astro_SPLASH-0.0.8/SPLASH/trained_models/__init__.py
-drwxr-xr-x   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:53:05.831052 astro_SPLASH-0.0.8/astro_SPLASH.egg-info/
--rw-r--r--   0 adamboesky   (501) staff       (20)      372 2024-05-06 04:53:05.000000 astro_SPLASH-0.0.8/astro_SPLASH.egg-info/PKG-INFO
--rw-r--r--   0 adamboesky   (501) staff       (20)      462 2024-05-06 04:53:05.000000 astro_SPLASH-0.0.8/astro_SPLASH.egg-info/SOURCES.txt
--rw-r--r--   0 adamboesky   (501) staff       (20)        1 2024-05-06 04:53:05.000000 astro_SPLASH-0.0.8/astro_SPLASH.egg-info/dependency_links.txt
--rw-r--r--   0 adamboesky   (501) staff       (20)       25 2024-05-06 04:53:05.000000 astro_SPLASH-0.0.8/astro_SPLASH.egg-info/requires.txt
--rw-r--r--   0 adamboesky   (501) staff       (20)        7 2024-05-06 04:53:05.000000 astro_SPLASH-0.0.8/astro_SPLASH.egg-info/top_level.txt
--rw-r--r--   0 adamboesky   (501) staff       (20)       38 2024-05-06 04:53:05.832532 astro_SPLASH-0.0.8/setup.cfg
--rw-r--r--   0 adamboesky   (501) staff       (20)      690 2024-05-06 04:52:33.000000 astro_SPLASH-0.0.8/setup.py
+drwxr-xr-x   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:58:49.676327 astro_SPLASH-0.0.9/
+-rw-r--r--   0 adamboesky   (501) staff       (20)      372 2024-05-06 04:58:49.675824 astro_SPLASH-0.0.9/PKG-INFO
+drwxr-xr-x   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:58:49.672546 astro_SPLASH-0.0.9/SPLASH/
+-rw-r--r--   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:19:09.000000 astro_SPLASH-0.0.9/SPLASH/__init__.py
+-rw-r--r--   0 adamboesky   (501) staff       (20)     1068 2024-05-06 04:50:42.000000 astro_SPLASH-0.0.9/SPLASH/network_utils.py
+-rw-r--r--   0 adamboesky   (501) staff       (20)    12048 2024-05-06 04:58:30.000000 astro_SPLASH-0.0.9/SPLASH/pipeline.py
+drwxr-xr-x   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:58:49.672988 astro_SPLASH-0.0.9/SPLASH/trained_models/
+-rw-r--r--   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:19:22.000000 astro_SPLASH-0.0.9/SPLASH/trained_models/__init__.py
+drwxr-xr-x   0 adamboesky   (501) staff       (20)        0 2024-05-06 04:58:49.674842 astro_SPLASH-0.0.9/astro_SPLASH.egg-info/
+-rw-r--r--   0 adamboesky   (501) staff       (20)      372 2024-05-06 04:58:49.000000 astro_SPLASH-0.0.9/astro_SPLASH.egg-info/PKG-INFO
+-rw-r--r--   0 adamboesky   (501) staff       (20)      462 2024-05-06 04:58:49.000000 astro_SPLASH-0.0.9/astro_SPLASH.egg-info/SOURCES.txt
+-rw-r--r--   0 adamboesky   (501) staff       (20)        1 2024-05-06 04:58:49.000000 astro_SPLASH-0.0.9/astro_SPLASH.egg-info/dependency_links.txt
+-rw-r--r--   0 adamboesky   (501) staff       (20)       25 2024-05-06 04:58:49.000000 astro_SPLASH-0.0.9/astro_SPLASH.egg-info/requires.txt
+-rw-r--r--   0 adamboesky   (501) staff       (20)        7 2024-05-06 04:58:49.000000 astro_SPLASH-0.0.9/astro_SPLASH.egg-info/top_level.txt
+-rw-r--r--   0 adamboesky   (501) staff       (20)       38 2024-05-06 04:58:49.676523 astro_SPLASH-0.0.9/setup.cfg
+-rw-r--r--   0 adamboesky   (501) staff       (20)      690 2024-05-06 04:58:48.000000 astro_SPLASH-0.0.9/setup.py
```

### Comparing `astro_SPLASH-0.0.8/SPLASH/network_utils.py` & `astro_SPLASH-0.0.9/SPLASH/network_utils.py`

 * *Files identical despite different names*

### Comparing `astro_SPLASH-0.0.8/SPLASH/pipeline.py` & `astro_SPLASH-0.0.9/SPLASH/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import torch
 import pickle
 import numpy as np
 
 from typing import Tuple
-from network_utils import resume, get_model
+from .network_utils import resume, get_model
 
 torch.set_default_dtype(torch.float64)  # set the pytorch default to a float64
 MODELS_DIR_PATH = os.path.dirname(os.path.realpath(__file__))
 
 
 class SnPipeline:
     def __init__(self, pipeline_version: str = 'weighted_full_band', pre_transformed: bool = False, within_4sigma: bool = True):
```

### Comparing `astro_SPLASH-0.0.8/setup.py` & `astro_SPLASH-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='astro_SPLASH',
-    version='0.0.8',
+    version='0.0.9',
     author='Adam Boesky',
     author_email='apboesky@gmail.com',
     description='SPLASH (Supernova classification Pipeline Leveraging Attributes of Supernova Hosts)',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

