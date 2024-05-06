# Comparing `tmp/fortiedr-3.6.4.tar.gz` & `tmp/fortiedr-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortiedr-3.6.4.tar", last modified: Fri May  3 20:29:49 2024, max compression
+gzip compressed data, was "fortiedr-3.6.5.tar", last modified: Mon May  6 12:27:46 2024, max compression
```

## Comparing `fortiedr-3.6.4.tar` & `fortiedr-3.6.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-05-03 20:29:49.652119 fortiedr-3.6.4/
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     1070 2024-05-03 20:00:35.000000 fortiedr-3.6.4/LICENSE
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       62 2024-05-03 20:14:00.000000 fortiedr-3.6.4/MANIFEST.in
--rw-r--r--   0 rafael    (1000) rafael    (1000)     2730 2024-05-03 20:29:49.652119 fortiedr-3.6.4/PKG-INFO
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     2117 2024-05-03 20:00:35.000000 fortiedr-3.6.4/README.md
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-05-03 20:29:49.648119 fortiedr-3.6.4/fortiedr/
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      930 2024-05-03 20:00:35.000000 fortiedr-3.6.4/fortiedr/__init__.py
--rw-rw-r--   0 rafael    (1000) rafael    (1000)    21615 2024-05-03 20:00:35.000000 fortiedr-3.6.4/fortiedr/api_parameters.json
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     1633 2024-05-03 20:00:35.000000 fortiedr-3.6.4/fortiedr/auth.py
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     4311 2024-05-03 20:00:35.000000 fortiedr-3.6.4/fortiedr/connector.py
--rw-rw-r--   0 rafael    (1000) rafael    (1000)   241314 2024-05-03 20:29:23.000000 fortiedr-3.6.4/fortiedr/fortiedr.py
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-05-03 20:29:49.652119 fortiedr-3.6.4/fortiedr.egg-info/
--rw-r--r--   0 rafael    (1000) rafael    (1000)     2730 2024-05-03 20:29:49.000000 fortiedr-3.6.4/fortiedr.egg-info/PKG-INFO
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      308 2024-05-03 20:29:49.000000 fortiedr-3.6.4/fortiedr.egg-info/SOURCES.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)        1 2024-05-03 20:29:49.000000 fortiedr-3.6.4/fortiedr.egg-info/dependency_links.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)        9 2024-05-03 20:29:49.000000 fortiedr-3.6.4/fortiedr.egg-info/top_level.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      571 2024-05-03 20:29:23.000000 fortiedr-3.6.4/pyproject.toml
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       36 2024-05-03 20:00:35.000000 fortiedr-3.6.4/requirements.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       38 2024-05-03 20:29:49.652119 fortiedr-3.6.4/setup.cfg
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      880 2024-05-03 20:29:23.000000 fortiedr-3.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:27:46.748735 fortiedr-3.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-06 12:27:35.000000 fortiedr-3.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-06 12:27:35.000000 fortiedr-3.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-06 12:27:46.748735 fortiedr-3.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-06 12:27:35.000000 fortiedr-3.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:27:46.744735 fortiedr-3.6.5/fortiedr/
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-06 12:27:35.000000 fortiedr-3.6.5/fortiedr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21615 2024-05-06 12:27:35.000000 fortiedr-3.6.5/fortiedr/api_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-06 12:27:35.000000 fortiedr-3.6.5/fortiedr/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-06 12:27:35.000000 fortiedr-3.6.5/fortiedr/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)   241314 2024-05-06 12:27:35.000000 fortiedr-3.6.5/fortiedr/fortiedr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:27:46.748735 fortiedr-3.6.5/fortiedr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-06 12:27:46.000000 fortiedr-3.6.5/fortiedr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-06 12:27:46.000000 fortiedr-3.6.5/fortiedr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 12:27:46.000000 fortiedr-3.6.5/fortiedr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 12:27:46.000000 fortiedr-3.6.5/fortiedr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-06 12:27:35.000000 fortiedr-3.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-06 12:27:35.000000 fortiedr-3.6.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 12:27:46.748735 fortiedr-3.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-06 12:27:35.000000 fortiedr-3.6.5/setup.py
```

### Comparing `fortiedr-3.6.4/LICENSE` & `fortiedr-3.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.4/PKG-INFO` & `fortiedr-3.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortiedr
-Version: 3.6.4
+Version: 3.6.5
 Summary: This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.
 Author: Rafael Foster
 Author-email: Rafael Foster <rafaelgfoster@gmail.com>
 Project-URL: Homepage, https://github.com/rafaelfoster/fortiedr
 Project-URL: Issues, https://github.com/rafaelfoster/fortiedr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fortiedr-3.6.4/README.md` & `fortiedr-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.4/fortiedr/__init__.py` & `fortiedr-3.6.5/fortiedr/__init__.py`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.4/fortiedr/api_parameters.json` & `fortiedr-3.6.5/fortiedr/api_parameters.json`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.4/fortiedr/auth.py` & `fortiedr-3.6.5/fortiedr/auth.py`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.4/fortiedr/connector.py` & `fortiedr-3.6.5/fortiedr/connector.py`

 * *Files identical despite different names*

### Comparing `fortiedr-3.6.4/fortiedr/fortiedr.py` & `fortiedr-3.6.5/fortiedr/fortiedr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import os
 import json
 from typing import BinaryIO
 from fortiedr.auth import Auth as fedrAuth
 from fortiedr.connector import FortiEDR_API_GW
 
-version = "3.6.4"
+version = "3.6.5"
 
 fortiedr_connection = None
 
 class ApplicationControl:
 	'''Application Control Rest Api Controller'''
 
 	def get_applications(self, currentPage: int, organization: str, fileName: str = None, path: str = None, signer: str = None, enabled: bool = None, hash: str = None, operatingSystem: str = None, policyIds: list = None, tag: str = None) -> tuple[bool, None]:
```

### Comparing `fortiedr-3.6.4/fortiedr.egg-info/PKG-INFO` & `fortiedr-3.6.5/fortiedr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortiedr
-Version: 3.6.4
+Version: 3.6.5
 Summary: This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.
 Author: Rafael Foster
 Author-email: Rafael Foster <rafaelgfoster@gmail.com>
 Project-URL: Homepage, https://github.com/rafaelfoster/fortiedr
 Project-URL: Issues, https://github.com/rafaelfoster/fortiedr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fortiedr-3.6.4/pyproject.toml` & `fortiedr-3.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fortiedr"
-version = "3.6.4"
+version = "3.6.5"
 authors = [
   { name="Rafael Foster", email="rafaelgfoster@gmail.com" }
 ]
 description = "This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `fortiedr-3.6.4/setup.py` & `fortiedr-3.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 cur_dir = os.path.dirname(__file__)
 
 with open(f"{cur_dir}/requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="fortiedr",
-    version="3.6.4",
+    version="3.6.5",
     description="This Fortiedr module is an open-source Python library that simplifies interaction with the FortiEDR Cloud API.",
     author="Rafael Foster",
     author_email="rafaelgfoster@gmail.com",
     project_urls={
         "GitHub": "https://github.com/rafaelfoster/fortiedr",
     },
     python_requires=">=3.8",
```

