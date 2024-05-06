# Comparing `tmp/mlsdk-0.0.1.tar.gz` & `tmp/mlsdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlsdk-0.0.1.tar", last modified: Mon May  6 09:58:00 2024, max compression
+gzip compressed data, was "mlsdk-0.0.2.tar", last modified: Mon May  6 10:00:49 2024, max compression
```

## Comparing `mlsdk-0.0.1.tar` & `mlsdk-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-06 09:58:00.670261 mlsdk-0.0.1/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-02 09:49:32.000000 mlsdk-0.0.1/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-02 09:49:32.000000 mlsdk-0.0.1/MANIFEST.in
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      385 2024-05-06 09:58:00.670261 mlsdk-0.0.1/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-02 09:49:32.000000 mlsdk-0.0.1/README.md
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-06 09:58:00.670261 mlsdk-0.0.1/mlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-03 11:00:51.000000 mlsdk-0.0.1/mlsdk/__init__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4121 2024-05-06 09:48:46.000000 mlsdk-0.0.1/mlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9099 2024-05-06 07:54:25.000000 mlsdk-0.0.1/mlsdk/base_class.py
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-06 09:58:00.670261 mlsdk-0.0.1/mlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      385 2024-05-06 09:58:00.000000 mlsdk-0.0.1/mlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      274 2024-05-06 09:58:00.000000 mlsdk-0.0.1/mlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-06 09:58:00.000000 mlsdk-0.0.1/mlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       47 2024-05-06 09:58:00.000000 mlsdk-0.0.1/mlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-06 09:58:00.000000 mlsdk-0.0.1/mlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        6 2024-05-06 09:58:00.000000 mlsdk-0.0.1/mlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-06 09:58:00.680261 mlsdk-0.0.1/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      695 2024-05-06 09:50:14.000000 mlsdk-0.0.1/setup.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-06 10:00:49.950260 mlsdk-0.0.2/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-02 09:49:32.000000 mlsdk-0.0.2/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-02 09:49:32.000000 mlsdk-0.0.2/MANIFEST.in
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      385 2024-05-06 10:00:49.940261 mlsdk-0.0.2/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-02 09:49:32.000000 mlsdk-0.0.2/README.md
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-06 10:00:49.940261 mlsdk-0.0.2/mlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-03 11:00:51.000000 mlsdk-0.0.2/mlsdk/__init__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4121 2024-05-06 09:48:46.000000 mlsdk-0.0.2/mlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9099 2024-05-06 07:54:25.000000 mlsdk-0.0.2/mlsdk/base_class.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-06 10:00:49.940261 mlsdk-0.0.2/mlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      385 2024-05-06 10:00:49.000000 mlsdk-0.0.2/mlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      274 2024-05-06 10:00:49.000000 mlsdk-0.0.2/mlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-06 10:00:49.000000 mlsdk-0.0.2/mlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       47 2024-05-06 10:00:49.000000 mlsdk-0.0.2/mlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       20 2024-05-06 10:00:49.000000 mlsdk-0.0.2/mlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        6 2024-05-06 10:00:49.000000 mlsdk-0.0.2/mlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-06 10:00:49.950260 mlsdk-0.0.2/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      697 2024-05-06 10:00:39.000000 mlsdk-0.0.2/setup.py
```

### Comparing `mlsdk-0.0.1/mlsdk/__main__.py` & `mlsdk-0.0.2/mlsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `mlsdk-0.0.1/mlsdk/base_class.py` & `mlsdk-0.0.2/mlsdk/base_class.py`

 * *Files identical despite different names*

### Comparing `mlsdk-0.0.1/setup.py` & `mlsdk-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mlsdk',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     description='Model Zoo SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'python-dotenv',
-        'silabs-mltk[full]'
+        # 'silabs-mltk[full]'
     ],
     author='EUR',
     author_email='eur@gmail.com',
     license='MIT',
     entry_points={
         "console_scripts": [
             "mlsdk = mlsdk.__main__:main"
```

