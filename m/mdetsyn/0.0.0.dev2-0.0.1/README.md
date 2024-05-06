# Comparing `tmp/mdetsyn-0.0.0.dev2.tar.gz` & `tmp/mdetsyn-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdetsyn-0.0.0.dev2.tar", last modified: Mon May  6 08:52:26 2024, max compression
+gzip compressed data, was "mdetsyn-0.0.1.tar", last modified: Mon May  6 08:58:50 2024, max compression
```

## Comparing `mdetsyn-0.0.0.dev2.tar` & `mdetsyn-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-06 08:52:26.926816 mdetsyn-0.0.0.dev2/
--rw-r--r--   0 dongtrinh  (1001) dongtrinh  (1001)      517 2024-05-06 08:52:26.926816 mdetsyn-0.0.0.dev2/PKG-INFO
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)      243 2024-05-06 08:15:50.000000 mdetsyn-0.0.0.dev2/README.md
-drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-06 08:52:26.926816 mdetsyn-0.0.0.dev2/mdetsyn/
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       33 2024-05-06 08:46:15.000000 mdetsyn-0.0.0.dev2/mdetsyn/__init__.py
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)     7301 2024-05-06 08:50:24.000000 mdetsyn-0.0.0.dev2/mdetsyn/detsyn.py
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)     7486 2024-05-06 07:48:17.000000 mdetsyn-0.0.0.dev2/mdetsyn/helpers.py
-drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-06 08:52:26.926816 mdetsyn-0.0.0.dev2/mdetsyn.egg-info/
--rw-r--r--   0 dongtrinh  (1001) dongtrinh  (1001)      517 2024-05-06 08:52:26.000000 mdetsyn-0.0.0.dev2/mdetsyn.egg-info/PKG-INFO
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)      246 2024-05-06 08:52:26.000000 mdetsyn-0.0.0.dev2/mdetsyn.egg-info/SOURCES.txt
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)        1 2024-05-06 08:52:26.000000 mdetsyn-0.0.0.dev2/mdetsyn.egg-info/dependency_links.txt
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       21 2024-05-06 08:52:26.000000 mdetsyn-0.0.0.dev2/mdetsyn.egg-info/requires.txt
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)        8 2024-05-06 08:52:26.000000 mdetsyn-0.0.0.dev2/mdetsyn.egg-info/top_level.txt
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       20 2024-05-06 07:47:54.000000 mdetsyn-0.0.0.dev2/requirements.txt
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       38 2024-05-06 08:52:26.926816 mdetsyn-0.0.0.dev2/setup.cfg
--rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)      701 2024-05-06 08:52:17.000000 mdetsyn-0.0.0.dev2/setup.py
+drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-06 08:58:50.243886 mdetsyn-0.0.1/
+-rw-r--r--   0 dongtrinh  (1001) dongtrinh  (1001)      866 2024-05-06 08:58:50.243886 mdetsyn-0.0.1/PKG-INFO
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)      597 2024-05-06 08:57:33.000000 mdetsyn-0.0.1/README.md
+drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-06 08:58:50.243886 mdetsyn-0.0.1/mdetsyn/
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       33 2024-05-06 08:46:15.000000 mdetsyn-0.0.1/mdetsyn/__init__.py
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)     7301 2024-05-06 08:50:24.000000 mdetsyn-0.0.1/mdetsyn/detsyn.py
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)     7486 2024-05-06 07:48:17.000000 mdetsyn-0.0.1/mdetsyn/helpers.py
+drwxrwxr-x   0 dongtrinh  (1001) dongtrinh  (1001)        0 2024-05-06 08:58:50.243886 mdetsyn-0.0.1/mdetsyn.egg-info/
+-rw-r--r--   0 dongtrinh  (1001) dongtrinh  (1001)      866 2024-05-06 08:58:50.000000 mdetsyn-0.0.1/mdetsyn.egg-info/PKG-INFO
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)      246 2024-05-06 08:58:50.000000 mdetsyn-0.0.1/mdetsyn.egg-info/SOURCES.txt
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)        1 2024-05-06 08:58:50.000000 mdetsyn-0.0.1/mdetsyn.egg-info/dependency_links.txt
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       21 2024-05-06 08:58:50.000000 mdetsyn-0.0.1/mdetsyn.egg-info/requires.txt
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)        8 2024-05-06 08:58:50.000000 mdetsyn-0.0.1/mdetsyn.egg-info/top_level.txt
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       20 2024-05-06 07:47:54.000000 mdetsyn-0.0.1/requirements.txt
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)       38 2024-05-06 08:58:50.243886 mdetsyn-0.0.1/setup.cfg
+-rw-rw-r--   0 dongtrinh  (1001) dongtrinh  (1001)      696 2024-05-06 08:58:06.000000 mdetsyn-0.0.1/setup.py
```

### Comparing `mdetsyn-0.0.0.dev2/mdetsyn/detsyn.py` & `mdetsyn-0.0.1/mdetsyn/detsyn.py`

 * *Files identical despite different names*

### Comparing `mdetsyn-0.0.0.dev2/mdetsyn/helpers.py` & `mdetsyn-0.0.1/mdetsyn/helpers.py`

 * *Files identical despite different names*

### Comparing `mdetsyn-0.0.0.dev2/setup.py` & `mdetsyn-0.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def get_requirements_txt(requirements_path):
     with open(requirements_path, 'r') as file:
         requirements = [line.rstrip('\n') for line in file.readlines()]
     return requirements
 
 setup( 
     name='mdetsyn', 
-    version='0.0.0.dev2', 
+    version='0.0.1', 
     description='Data Synthesis pipeline to generate object detection data', 
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown',
     author='PD-Mera', 
     author_email='phuongdong1772000@gmail.com', 
     packages=find_packages(), 
     data_files=["requirements.txt"],
```

