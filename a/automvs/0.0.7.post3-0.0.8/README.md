# Comparing `tmp/automvs-0.0.7.post3.tar.gz` & `tmp/automvs-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automvs-0.0.7.post3.tar", last modified: Thu May  2 17:45:51 2024, max compression
+gzip compressed data, was "automvs-0.0.8.tar", last modified: Mon May  6 05:44:27 2024, max compression
```

## Comparing `automvs-0.0.7.post3.tar` & `automvs-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-02 17:45:51.388141 automvs-0.0.7.post3/
--rw-rw-r--   0 phil      (1000) phil      (1000)     1069 2024-04-30 16:02:39.000000 automvs-0.0.7.post3/LICENSE
--rw-r--r--   0 phil      (1000) phil      (1000)     1436 2024-05-02 17:45:51.388141 automvs-0.0.7.post3/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      956 2024-04-30 16:02:39.000000 automvs-0.0.7.post3/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-02 17:45:51.384142 automvs-0.0.7.post3/automvs/
--rw-rw-r--   0 phil      (1000) phil      (1000)    20037 2024-05-02 17:45:06.000000 automvs-0.0.7.post3/automvs/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-02 17:45:51.388141 automvs-0.0.7.post3/automvs.egg-info/
--rw-r--r--   0 phil      (1000) phil      (1000)     1436 2024-05-02 17:45:51.000000 automvs-0.0.7.post3/automvs.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-05-02 17:45:51.000000 automvs-0.0.7.post3/automvs.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-02 17:45:51.000000 automvs-0.0.7.post3/automvs.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        8 2024-05-02 17:45:51.000000 automvs-0.0.7.post3/automvs.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-02 17:45:51.388141 automvs-0.0.7.post3/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)      783 2024-05-02 17:45:08.000000 automvs-0.0.7.post3/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-06 05:44:27.421794 automvs-0.0.8/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1069 2024-04-30 16:02:39.000000 automvs-0.0.8/LICENSE
+-rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-05-06 05:44:27.421794 automvs-0.0.8/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      956 2024-04-30 16:02:39.000000 automvs-0.0.8/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-06 05:44:27.421794 automvs-0.0.8/automvs/
+-rw-rw-r--   0 phil      (1000) phil      (1000)    35123 2024-05-06 05:43:46.000000 automvs-0.0.8/automvs/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-06 05:44:27.421794 automvs-0.0.8/automvs.egg-info/
+-rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-05-06 05:44:27.000000 automvs-0.0.8/automvs.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-05-06 05:44:27.000000 automvs-0.0.8/automvs.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-06 05:44:27.000000 automvs-0.0.8/automvs.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        8 2024-05-06 05:44:27.000000 automvs-0.0.8/automvs.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-06 05:44:27.421794 automvs-0.0.8/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)      781 2024-05-06 05:43:56.000000 automvs-0.0.8/setup.py
```

### Comparing `automvs-0.0.7.post3/LICENSE` & `automvs-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `automvs-0.0.7.post3/PKG-INFO` & `automvs-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automvs
-Version: 0.0.7.post3
+Version: 0.0.8
 Summary: Python library for MVS/CE automation
 Home-page: https://github.com/MVS-sysgen/automvs
 Author: Philip Young
 Author-email: mainframed767@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `automvs-0.0.7.post3/README.md` & `automvs-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `automvs-0.0.7.post3/automvs.egg-info/PKG-INFO` & `automvs-0.0.8/automvs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automvs
-Version: 0.0.7.post3
+Version: 0.0.8
 Summary: Python library for MVS/CE automation
 Home-page: https://github.com/MVS-sysgen/automvs
 Author: Philip Young
 Author-email: mainframed767@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `automvs-0.0.7.post3/setup.py` & `automvs-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as file:
         return file.read()
 
 setup(
     name='automvs',
-    version='0.0.7-3',    
+    version='0.0.8',    
     description='Python library for MVS/CE automation',
     url='https://github.com/MVS-sysgen/automvs',
     author='Philip Young',
     author_email='mainframed767@gmail.com',
     license='MIT',
     packages=['automvs'],
     install_requires=[],
```

