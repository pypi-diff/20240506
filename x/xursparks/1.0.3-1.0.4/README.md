# Comparing `tmp/xursparks-1.0.3.tar.gz` & `tmp/xursparks-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xursparks-1.0.3.tar", last modified: Thu May  2 07:16:48 2024, max compression
+gzip compressed data, was "xursparks-1.0.4.tar", last modified: Mon May  6 01:43:00 2024, max compression
```

## Comparing `xursparks-1.0.3.tar` & `xursparks-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-02 07:16:48.417906 xursparks-1.0.3/
--rw-rw-r--   0 doods     (1000) doods     (1000)     5835 2024-05-02 07:16:48.417906 xursparks-1.0.3/PKG-INFO
--rw-rw-r--   0 doods     (1000) doods     (1000)     5345 2024-04-03 04:21:12.000000 xursparks-1.0.3/README.md
--rw-rw-r--   0 doods     (1000) doods     (1000)       89 2024-04-05 01:26:52.000000 xursparks-1.0.3/pyproject.toml
--rw-rw-r--   0 doods     (1000) doods     (1000)       38 2024-05-02 07:16:48.417906 xursparks-1.0.3/setup.cfg
--rw-rw-r--   0 doods     (1000) doods     (1000)      650 2024-05-02 07:16:31.000000 xursparks-1.0.3/setup.py
-drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-02 07:16:48.417906 xursparks-1.0.3/xursparks.egg-info/
--rw-rw-r--   0 doods     (1000) doods     (1000)     5835 2024-05-02 07:16:48.000000 xursparks-1.0.3/xursparks.egg-info/PKG-INFO
--rw-rw-r--   0 doods     (1000) doods     (1000)      165 2024-05-02 07:16:48.000000 xursparks-1.0.3/xursparks.egg-info/SOURCES.txt
--rw-rw-r--   0 doods     (1000) doods     (1000)        1 2024-05-02 07:16:48.000000 xursparks-1.0.3/xursparks.egg-info/dependency_links.txt
--rw-rw-r--   0 doods     (1000) doods     (1000)        1 2024-05-02 07:16:48.000000 xursparks-1.0.3/xursparks.egg-info/top_level.txt
+drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-06 01:43:00.184459 xursparks-1.0.4/
+-rw-rw-r--   0 doods     (1000) doods     (1000)     5835 2024-05-06 01:43:00.184459 xursparks-1.0.4/PKG-INFO
+-rw-rw-r--   0 doods     (1000) doods     (1000)     5345 2024-04-03 04:21:12.000000 xursparks-1.0.4/README.md
+-rw-rw-r--   0 doods     (1000) doods     (1000)       89 2024-04-05 01:26:52.000000 xursparks-1.0.4/pyproject.toml
+-rw-rw-r--   0 doods     (1000) doods     (1000)       38 2024-05-06 01:43:00.184459 xursparks-1.0.4/setup.cfg
+-rw-rw-r--   0 doods     (1000) doods     (1000)      648 2024-05-06 01:39:17.000000 xursparks-1.0.4/setup.py
+drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-06 01:43:00.184459 xursparks-1.0.4/xursparks/
+-rw-rw-r--   0 doods     (1000) doods     (1000)    34868 2024-05-06 01:38:42.000000 xursparks-1.0.4/xursparks/__init__.py
+drwxrwxr-x   0 doods     (1000) doods     (1000)        0 2024-05-06 01:43:00.184459 xursparks-1.0.4/xursparks.egg-info/
+-rw-rw-r--   0 doods     (1000) doods     (1000)     5835 2024-05-06 01:43:00.000000 xursparks-1.0.4/xursparks.egg-info/PKG-INFO
+-rw-rw-r--   0 doods     (1000) doods     (1000)      187 2024-05-06 01:43:00.000000 xursparks-1.0.4/xursparks.egg-info/SOURCES.txt
+-rw-rw-r--   0 doods     (1000) doods     (1000)        1 2024-05-06 01:43:00.000000 xursparks-1.0.4/xursparks.egg-info/dependency_links.txt
+-rw-rw-r--   0 doods     (1000) doods     (1000)       10 2024-05-06 01:43:00.000000 xursparks-1.0.4/xursparks.egg-info/top_level.txt
```

### Comparing `xursparks-1.0.3/PKG-INFO` & `xursparks-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xursparks
-Version: 1.0.3
+Version: 1.0.4
 Summary: Encapsulating Apache Spark for easy usage
 Home-page: https://github.com/dev-doods687/xursparks
 Author: Randell Gabriel Santos
 Author-email: randellsantos@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xursparks-1.0.3/README.md` & `xursparks-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `xursparks-1.0.3/setup.py` & `xursparks-1.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xursparks',
-    version='1.0.3',
-    packages=find_packages(),
+    version='1.0.4',
+    packages=['xursparks'],
     author='Randell Gabriel Santos',
     author_email='randellsantos@gmail.com',
     description='Encapsulating Apache Spark for easy usage',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/dev-doods687/xursparks',
     license='MIT',
```

### Comparing `xursparks-1.0.3/xursparks.egg-info/PKG-INFO` & `xursparks-1.0.4/xursparks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xursparks
-Version: 1.0.3
+Version: 1.0.4
 Summary: Encapsulating Apache Spark for easy usage
 Home-page: https://github.com/dev-doods687/xursparks
 Author: Randell Gabriel Santos
 Author-email: randellsantos@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

