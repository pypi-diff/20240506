# Comparing `tmp/openweatherapi_sdk-0.1.tar.gz` & `tmp/openweatherapi_sdk-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\openweatherapi_sdk-0.1.tar", last modified: Sun May  5 20:01:19 2024, max compression
+gzip compressed data, was "dist\openweatherapi_sdk-0.2.tar", last modified: Mon May  6 12:50:47 2024, max compression
```

## Comparing `openweatherapi_sdk-0.1.tar` & `openweatherapi_sdk-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 20:01:19.641694 openweatherapi_sdk-0.1/
--rw-rw-rw-   0        0        0     1088 2024-05-05 09:09:40.000000 openweatherapi_sdk-0.1/LICENSE
--rw-rw-rw-   0        0        0     1689 2024-05-05 20:01:19.641694 openweatherapi_sdk-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1273 2024-05-05 19:55:42.000000 openweatherapi_sdk-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 20:01:19.641694 openweatherapi_sdk-0.1/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-05-05 20:00:24.000000 openweatherapi_sdk-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 20:01:19.603093 openweatherapi_sdk-0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-05 20:01:19.641694 openweatherapi_sdk-0.1/src/openweatherapi_sdk.egg-info/
--rw-rw-rw-   0        0        0     1689 2024-05-05 20:01:19.000000 openweatherapi_sdk-0.1/src/openweatherapi_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-05-05 20:01:19.000000 openweatherapi_sdk-0.1/src/openweatherapi_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 20:01:19.000000 openweatherapi_sdk-0.1/src/openweatherapi_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-05 20:01:19.000000 openweatherapi_sdk-0.1/src/openweatherapi_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 20:01:19.000000 openweatherapi_sdk-0.1/src/openweatherapi_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 12:50:47.128352 openweatherapi_sdk-0.2/
+-rw-rw-rw-   0        0        0     1088 2024-05-05 09:09:40.000000 openweatherapi_sdk-0.2/LICENSE
+-rw-rw-rw-   0        0        0     1689 2024-05-06 12:50:47.128352 openweatherapi_sdk-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1273 2024-05-05 19:55:42.000000 openweatherapi_sdk-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 12:50:47.128352 openweatherapi_sdk-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      760 2024-05-06 12:47:30.000000 openweatherapi_sdk-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:50:47.077298 openweatherapi_sdk-0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 12:50:47.124226 openweatherapi_sdk-0.2/src/openweatherapi_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1689 2024-05-06 12:50:46.000000 openweatherapi_sdk-0.2/src/openweatherapi_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-05-06 12:50:46.000000 openweatherapi_sdk-0.2/src/openweatherapi_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 12:50:46.000000 openweatherapi_sdk-0.2/src/openweatherapi_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-06 12:50:46.000000 openweatherapi_sdk-0.2/src/openweatherapi_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 12:50:46.000000 openweatherapi_sdk-0.2/src/openweatherapi_sdk.egg-info/top_level.txt
```

### Comparing `openweatherapi_sdk-0.1/LICENSE` & `openweatherapi_sdk-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openweatherapi_sdk-0.1/PKG-INFO` & `openweatherapi_sdk-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openweatherapi-sdk
-Version: 0.1
+Version: 0.2
 Summary: A simple SDK for interacting with the OpenWeatherMap API
 Author: Snehal Palve
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `openweatherapi_sdk-0.1/README.md` & `openweatherapi_sdk-0.2/README.md`

 * *Files identical despite different names*

### Comparing `openweatherapi_sdk-0.1/setup.py` & `openweatherapi_sdk-0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r") as fh:
     long_description = fh.read()
 
 setup(
     name="openweatherapi-sdk",
-    version="0.1",
+    version="0.2",
     packages=find_packages(),
+    package_data={'': ['sdk/*.py']},  
     install_requires=["requests"],
     author="Snehal Palve",
     description="A simple SDK for interacting with the OpenWeatherMap API",
     long_description=long_description,
     long_description_content_type= "text/markdown",
     classifiers =[
     "Programming Language :: Python :: 3",
```

### Comparing `openweatherapi_sdk-0.1/src/openweatherapi_sdk.egg-info/PKG-INFO` & `openweatherapi_sdk-0.2/src/openweatherapi_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openweatherapi-sdk
-Version: 0.1
+Version: 0.2
 Summary: A simple SDK for interacting with the OpenWeatherMap API
 Author: Snehal Palve
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

