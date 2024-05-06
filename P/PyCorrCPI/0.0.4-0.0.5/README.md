# Comparing `tmp/PyCorrCPI-0.0.4.tar.gz` & `tmp/PyCorrCPI-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCorrCPI-0.0.4.tar", last modified: Mon May  6 12:30:01 2024, max compression
+gzip compressed data, was "PyCorrCPI-0.0.5.tar", last modified: Mon May  6 12:56:09 2024, max compression
```

## Comparing `PyCorrCPI-0.0.4.tar` & `PyCorrCPI-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 fallum   (778712529) 1704612529        0 2024-05-06 12:30:01.789937 PyCorrCPI-0.0.4/
--rw-r--r--   0 fallum   (778712529) 1704612529    35149 2024-04-23 17:19:14.000000 PyCorrCPI-0.0.4/LICENSE
--rw-r--r--   0 fallum   (778712529) 1704612529      452 2024-05-06 12:30:01.789430 PyCorrCPI-0.0.4/PKG-INFO
-drwxr-xr-x   0 fallum   (778712529) 1704612529        0 2024-05-06 12:30:01.784822 PyCorrCPI-0.0.4/PyCorrCPI/
--rw-r--r--   0 fallum   (778712529) 1704612529      130 2024-04-23 17:22:50.000000 PyCorrCPI-0.0.4/PyCorrCPI/__init__.py
--rwx------   0 fallum   (778712529) 1704612529    44790 2024-05-06 12:27:52.000000 PyCorrCPI-0.0.4/PyCorrCPI/covariance.py
--rw-r--r--   0 fallum   (778712529) 1704612529    14480 2024-05-06 12:26:59.000000 PyCorrCPI-0.0.4/PyCorrCPI/data.py
--rw-r--r--   0 fallum   (778712529) 1704612529     2950 2024-05-06 01:58:47.000000 PyCorrCPI-0.0.4/PyCorrCPI/helpers_numba.py
--rw-r--r--   0 fallum   (778712529) 1704612529      815 2024-05-02 22:28:05.000000 PyCorrCPI-0.0.4/PyCorrCPI/imports.py
--rw-r--r--   0 fallum   (778712529) 1704612529    10331 2024-05-06 02:03:05.000000 PyCorrCPI-0.0.4/PyCorrCPI/output_functions.py
-drwxr-xr-x   0 fallum   (778712529) 1704612529        0 2024-05-06 12:30:01.788678 PyCorrCPI-0.0.4/PyCorrCPI.egg-info/
--rw-r--r--   0 fallum   (778712529) 1704612529      452 2024-05-06 12:30:01.000000 PyCorrCPI-0.0.4/PyCorrCPI.egg-info/PKG-INFO
--rw-r--r--   0 fallum   (778712529) 1704612529      332 2024-05-06 12:30:01.000000 PyCorrCPI-0.0.4/PyCorrCPI.egg-info/SOURCES.txt
--rw-r--r--   0 fallum   (778712529) 1704612529        1 2024-05-06 12:30:01.000000 PyCorrCPI-0.0.4/PyCorrCPI.egg-info/dependency_links.txt
--rw-r--r--   0 fallum   (778712529) 1704612529       71 2024-05-06 12:30:01.000000 PyCorrCPI-0.0.4/PyCorrCPI.egg-info/requires.txt
--rw-r--r--   0 fallum   (778712529) 1704612529       10 2024-05-06 12:30:01.000000 PyCorrCPI-0.0.4/PyCorrCPI.egg-info/top_level.txt
--rw-r--r--   0 fallum   (778712529) 1704612529      108 2024-04-23 20:25:11.000000 PyCorrCPI-0.0.4/README.md
--rw-r--r--   0 fallum   (778712529) 1704612529       38 2024-05-06 12:30:01.790158 PyCorrCPI-0.0.4/setup.cfg
--rw-r--r--   0 fallum   (778712529) 1704612529      712 2024-05-06 12:09:46.000000 PyCorrCPI-0.0.4/setup.py
+drwxr-xr-x   0 fallum   (778712529) 1704612529        0 2024-05-06 12:56:09.981960 PyCorrCPI-0.0.5/
+-rw-r--r--   0 fallum   (778712529) 1704612529    35149 2024-04-23 17:19:14.000000 PyCorrCPI-0.0.5/LICENSE
+-rw-r--r--   0 fallum   (778712529) 1704612529      452 2024-05-06 12:56:09.981348 PyCorrCPI-0.0.5/PKG-INFO
+drwxr-xr-x   0 fallum   (778712529) 1704612529        0 2024-05-06 12:56:09.976448 PyCorrCPI-0.0.5/PyCorrCPI/
+-rw-r--r--   0 fallum   (778712529) 1704612529      130 2024-04-23 17:22:50.000000 PyCorrCPI-0.0.5/PyCorrCPI/__init__.py
+-rwx------   0 fallum   (778712529) 1704612529    44790 2024-05-06 12:27:52.000000 PyCorrCPI-0.0.5/PyCorrCPI/covariance.py
+-rw-r--r--   0 fallum   (778712529) 1704612529    14480 2024-05-06 12:26:59.000000 PyCorrCPI-0.0.5/PyCorrCPI/data.py
+-rw-r--r--   0 fallum   (778712529) 1704612529     2950 2024-05-06 01:58:47.000000 PyCorrCPI-0.0.5/PyCorrCPI/helpers_numba.py
+-rw-r--r--   0 fallum   (778712529) 1704612529      815 2024-05-02 22:28:05.000000 PyCorrCPI-0.0.5/PyCorrCPI/imports.py
+-rw-r--r--   0 fallum   (778712529) 1704612529    10331 2024-05-06 02:03:05.000000 PyCorrCPI-0.0.5/PyCorrCPI/output_functions.py
+drwxr-xr-x   0 fallum   (778712529) 1704612529        0 2024-05-06 12:56:09.980633 PyCorrCPI-0.0.5/PyCorrCPI.egg-info/
+-rw-r--r--   0 fallum   (778712529) 1704612529      452 2024-05-06 12:56:09.000000 PyCorrCPI-0.0.5/PyCorrCPI.egg-info/PKG-INFO
+-rw-r--r--   0 fallum   (778712529) 1704612529      332 2024-05-06 12:56:09.000000 PyCorrCPI-0.0.5/PyCorrCPI.egg-info/SOURCES.txt
+-rw-r--r--   0 fallum   (778712529) 1704612529        1 2024-05-06 12:56:09.000000 PyCorrCPI-0.0.5/PyCorrCPI.egg-info/dependency_links.txt
+-rw-r--r--   0 fallum   (778712529) 1704612529       51 2024-05-06 12:56:09.000000 PyCorrCPI-0.0.5/PyCorrCPI.egg-info/requires.txt
+-rw-r--r--   0 fallum   (778712529) 1704612529       10 2024-05-06 12:56:09.000000 PyCorrCPI-0.0.5/PyCorrCPI.egg-info/top_level.txt
+-rw-r--r--   0 fallum   (778712529) 1704612529      242 2024-05-06 12:42:16.000000 PyCorrCPI-0.0.5/README.md
+-rw-r--r--   0 fallum   (778712529) 1704612529       38 2024-05-06 12:56:09.982173 PyCorrCPI-0.0.5/setup.cfg
+-rw-r--r--   0 fallum   (778712529) 1704612529      683 2024-05-06 12:55:18.000000 PyCorrCPI-0.0.5/setup.py
```

### Comparing `PyCorrCPI-0.0.4/LICENSE` & `PyCorrCPI-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCorrCPI-0.0.4/PyCorrCPI/covariance.py` & `PyCorrCPI-0.0.5/PyCorrCPI/covariance.py`

 * *Files identical despite different names*

### Comparing `PyCorrCPI-0.0.4/PyCorrCPI/data.py` & `PyCorrCPI-0.0.5/PyCorrCPI/data.py`

 * *Files identical despite different names*

### Comparing `PyCorrCPI-0.0.4/PyCorrCPI/helpers_numba.py` & `PyCorrCPI-0.0.5/PyCorrCPI/helpers_numba.py`

 * *Files identical despite different names*

### Comparing `PyCorrCPI-0.0.4/PyCorrCPI/imports.py` & `PyCorrCPI-0.0.5/PyCorrCPI/imports.py`

 * *Files identical despite different names*

### Comparing `PyCorrCPI-0.0.4/PyCorrCPI/output_functions.py` & `PyCorrCPI-0.0.5/PyCorrCPI/output_functions.py`

 * *Files identical despite different names*

### Comparing `PyCorrCPI-0.0.4/setup.py` & `PyCorrCPI-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'PyCorrCPI - corelation analysis for charged-particle imaging experiments'
 
 setup(
         name="PyCorrCPI", 
         version=VERSION,
         author="Felix Allum",
         author_email="fallum@stanford.edu",
         description=DESCRIPTION,
         packages=find_packages(),
-        install_requires=['numpy', 'matplotlib', 'scipy', 'pandas', 'numba', 'math', 'time', 'functools','IPython', 'typing'],
+        install_requires=['numpy', 'matplotlib', 'scipy', 'pandas', 'numba','IPython', 'typing'],
         url='https://github.com/f-allum/PyCCorrCPI/',
-        download_url='https://github.com/f-allum/PyCorrCPI/archive/refs/tags/v0.0.4.tar.gz',
+        download_url='https://github.com/f-allum/PyCorrCPI/archive/refs/tags/v0.0.5.tar.gz',
         keywords=['Coincidence', 'Covariance', 'Cumulant', 'Velocity-map Imaging']
 )
```

