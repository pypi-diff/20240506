# Comparing `tmp/thatsnakelang-0.1.tar.gz` & `tmp/thatsnakelang-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thatsnakelang-0.1.tar", last modified: Mon May  6 20:52:08 2024, max compression
+gzip compressed data, was "thatsnakelang-0.2.tar", last modified: Mon May  6 21:17:59 2024, max compression
```

## Comparing `thatsnakelang-0.1.tar` & `thatsnakelang-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:52:08.128593 thatsnakelang-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-06 20:52:08.128593 thatsnakelang-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-06 20:52:05.000000 thatsnakelang-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:52:08.124593 thatsnakelang-0.1/hello_world/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-06 20:52:05.000000 thatsnakelang-0.1/hello_world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:52:08.128593 thatsnakelang-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-06 20:52:05.000000 thatsnakelang-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:52:08.128593 thatsnakelang-0.1/thatsnakelang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-06 20:52:08.000000 thatsnakelang-0.1/thatsnakelang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-06 20:52:08.000000 thatsnakelang-0.1/thatsnakelang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:52:08.000000 thatsnakelang-0.1/thatsnakelang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 20:52:08.000000 thatsnakelang-0.1/thatsnakelang.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:17:59.682728 thatsnakelang-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-06 21:17:59.682728 thatsnakelang-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-06 21:17:57.000000 thatsnakelang-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:17:59.678728 thatsnakelang-0.2/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-06 21:17:57.000000 thatsnakelang-0.2/hello_world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:17:59.682728 thatsnakelang-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-06 21:17:57.000000 thatsnakelang-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:17:59.682728 thatsnakelang-0.2/thatsnakelang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-06 21:17:59.000000 thatsnakelang-0.2/thatsnakelang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-06 21:17:59.000000 thatsnakelang-0.2/thatsnakelang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:17:59.000000 thatsnakelang-0.2/thatsnakelang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 21:17:59.000000 thatsnakelang-0.2/thatsnakelang.egg-info/top_level.txt
```

### Comparing `thatsnakelang-0.1/PKG-INFO` & `thatsnakelang-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thatsnakelang
-Version: 0.1
+Version: 0.2
 Summary: A simple Hello World module
 Home-page: https://github.com/reggi/thatsnakelang
 Author: reggi
 Author-email: thomas.reggi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `thatsnakelang-0.1/setup.py` & `thatsnakelang-0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='thatsnakelang',
-    version='0.1',
+    version='0.2',
     packages=['hello_world'],
     description='A simple Hello World module',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='reggi',
     author_email='thomas.reggi@gmail.com',
     url='https://github.com/reggi/thatsnakelang',
```

### Comparing `thatsnakelang-0.1/thatsnakelang.egg-info/PKG-INFO` & `thatsnakelang-0.2/thatsnakelang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thatsnakelang
-Version: 0.1
+Version: 0.2
 Summary: A simple Hello World module
 Home-page: https://github.com/reggi/thatsnakelang
 Author: reggi
 Author-email: thomas.reggi@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

