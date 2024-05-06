# Comparing `tmp/communication_services-0.1.1.tar.gz` & `tmp/communication_services-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "communication_services-0.1.1.tar", last modified: Mon May  6 11:14:10 2024, max compression
+gzip compressed data, was "communication_services-0.1.2.tar", last modified: Mon May  6 11:35:30 2024, max compression
```

## Comparing `communication_services-0.1.1.tar` & `communication_services-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 pirgazi   (1000) pirgazi   (1000)        0 2024-05-06 11:14:10.975248 communication_services-0.1.1/
--rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)        0 2024-04-23 11:46:46.000000 communication_services-0.1.1/MANIFEST.in
--rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)     7709 2024-05-06 11:14:10.975248 communication_services-0.1.1/PKG-INFO
--rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)     6210 2024-04-20 13:23:56.000000 communication_services-0.1.1/README.md
-drwxrwxr-x   0 pirgazi   (1000) pirgazi   (1000)        0 2024-05-06 11:14:10.975248 communication_services-0.1.1/communication_services.egg-info/
--rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)     7709 2024-05-06 11:14:10.000000 communication_services-0.1.1/communication_services.egg-info/PKG-INFO
--rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)      259 2024-05-06 11:14:10.000000 communication_services-0.1.1/communication_services.egg-info/SOURCES.txt
--rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)        1 2024-05-06 11:14:10.000000 communication_services-0.1.1/communication_services.egg-info/dependency_links.txt
--rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)       29 2024-05-06 11:14:10.000000 communication_services-0.1.1/communication_services.egg-info/requires.txt
--rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)        1 2024-05-06 11:14:10.000000 communication_services-0.1.1/communication_services.egg-info/top_level.txt
--rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)       38 2024-05-06 11:14:10.975248 communication_services-0.1.1/setup.cfg
--rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)     1538 2024-05-06 11:13:58.000000 communication_services-0.1.1/setup.py
+drwxrwxr-x   0 pirgazi   (1000) pirgazi   (1000)        0 2024-05-06 11:35:30.599958 communication_services-0.1.2/
+-rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)        0 2024-04-23 11:46:46.000000 communication_services-0.1.2/MANIFEST.in
+-rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)     7709 2024-05-06 11:35:30.599958 communication_services-0.1.2/PKG-INFO
+-rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)     6210 2024-04-20 13:23:56.000000 communication_services-0.1.2/README.md
+drwxrwxr-x   0 pirgazi   (1000) pirgazi   (1000)        0 2024-05-06 11:35:30.599958 communication_services-0.1.2/communication_services.egg-info/
+-rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)     7709 2024-05-06 11:35:30.000000 communication_services-0.1.2/communication_services.egg-info/PKG-INFO
+-rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)      259 2024-05-06 11:35:30.000000 communication_services-0.1.2/communication_services.egg-info/SOURCES.txt
+-rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)        1 2024-05-06 11:35:30.000000 communication_services-0.1.2/communication_services.egg-info/dependency_links.txt
+-rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)       29 2024-05-06 11:35:30.000000 communication_services-0.1.2/communication_services.egg-info/requires.txt
+-rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)        1 2024-05-06 11:35:30.000000 communication_services-0.1.2/communication_services.egg-info/top_level.txt
+-rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)       38 2024-05-06 11:35:30.599958 communication_services-0.1.2/setup.cfg
+-rw-rw-r--   0 pirgazi   (1000) pirgazi   (1000)     1513 2024-05-06 11:35:16.000000 communication_services-0.1.2/setup.py
```

### Comparing `communication_services-0.1.1/PKG-INFO` & `communication_services-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communication_services
-Version: 0.1.1
+Version: 0.1.2
 Summary: A short description of your project
 Home-page: https://gitlab.com/geniusai1/partialtruckload-communication-serivecs.git
 Author: genius studio
 Author-email: info@geniusai.com
 License: UNKNOWN
 Description: # Notifiy_Service_Python
```

### Comparing `communication_services-0.1.1/README.md` & `communication_services-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `communication_services-0.1.1/communication_services.egg-info/PKG-INFO` & `communication_services-0.1.2/communication_services.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communication-services
-Version: 0.1.1
+Version: 0.1.2
 Summary: A short description of your project
 Home-page: https://gitlab.com/geniusai1/partialtruckload-communication-serivecs.git
 Author: genius studio
 Author-email: info@geniusai.com
 License: UNKNOWN
 Description: # Notifiy_Service_Python
```

### Comparing `communication_services-0.1.1/setup.py` & `communication_services-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='communication_services',
-    version='0.1.1',
+    version='0.1.2',
     author='genius studio',
     author_email='info@geniusai.com',
     description='A short description of your project',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://gitlab.com/geniusai1/partialtruckload-communication-serivecs.git',  # Link to your project's GitHub repo
-    packages=find_packages(exclude=('tests', 'docs')),
+    packages=find_packages(),
     include_package_data=True,
     install_requires=[
         # Add your project dependencies here
         # 'requests',
         # 'numpy',
         'celery',
         'twilio',
```

