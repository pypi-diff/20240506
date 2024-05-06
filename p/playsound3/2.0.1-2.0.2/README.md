# Comparing `tmp/playsound3-2.0.1.tar.gz` & `tmp/playsound3-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playsound3-2.0.1.tar", last modified: Mon May  6 17:40:12 2024, max compression
+gzip compressed data, was "playsound3-2.0.2.tar", last modified: Mon May  6 17:42:27 2024, max compression
```

## Comparing `playsound3-2.0.1.tar` & `playsound3-2.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:40:12.144879 playsound3-2.0.1/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1962 2024-05-06 14:15:46.000000 playsound3-2.0.1/LICENSE
--rw-r--r--   0 gaha      (1000) gaha      (1000)     2603 2024-05-06 17:40:12.144879 playsound3-2.0.1/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1602 2024-05-06 17:39:21.000000 playsound3-2.0.1/README.md
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:40:12.144879 playsound3-2.0.1/playsound3/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       44 2024-05-06 14:32:01.000000 playsound3-2.0.1/playsound3/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     3349 2024-05-06 17:36:33.000000 playsound3-2.0.1/playsound3/playsound3.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:40:12.144879 playsound3-2.0.1/playsound3.egg-info/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     2603 2024-05-06 17:40:12.000000 playsound3-2.0.1/playsound3.egg-info/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)      258 2024-05-06 17:40:12.000000 playsound3-2.0.1/playsound3.egg-info/SOURCES.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-05-06 17:40:12.000000 playsound3-2.0.1/playsound3.egg-info/dependency_links.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-05-06 17:40:12.000000 playsound3-2.0.1/playsound3.egg-info/requires.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       11 2024-05-06 17:40:12.000000 playsound3-2.0.1/playsound3.egg-info/top_level.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-05-06 12:41:28.000000 playsound3-2.0.1/pyproject.toml
--rw-r--r--   0 gaha      (1000) gaha      (1000)       38 2024-05-06 17:40:12.144879 playsound3-2.0.1/setup.cfg
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1365 2024-05-06 17:39:46.000000 playsound3-2.0.1/setup.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:42:27.758476 playsound3-2.0.2/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1962 2024-05-06 14:15:46.000000 playsound3-2.0.2/LICENSE
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     2604 2024-05-06 17:42:27.758476 playsound3-2.0.2/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1603 2024-05-06 17:42:11.000000 playsound3-2.0.2/README.md
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:42:27.758476 playsound3-2.0.2/playsound3/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       44 2024-05-06 14:32:01.000000 playsound3-2.0.2/playsound3/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     3349 2024-05-06 17:36:33.000000 playsound3-2.0.2/playsound3/playsound3.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:42:27.758476 playsound3-2.0.2/playsound3.egg-info/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     2604 2024-05-06 17:42:27.000000 playsound3-2.0.2/playsound3.egg-info/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      258 2024-05-06 17:42:27.000000 playsound3-2.0.2/playsound3.egg-info/SOURCES.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-05-06 17:42:27.000000 playsound3-2.0.2/playsound3.egg-info/dependency_links.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-05-06 17:42:27.000000 playsound3-2.0.2/playsound3.egg-info/requires.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       11 2024-05-06 17:42:27.000000 playsound3-2.0.2/playsound3.egg-info/top_level.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-05-06 12:41:28.000000 playsound3-2.0.2/pyproject.toml
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       38 2024-05-06 17:42:27.758476 playsound3-2.0.2/setup.cfg
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1365 2024-05-06 17:42:18.000000 playsound3-2.0.2/setup.py
```

### Comparing `playsound3-2.0.1/LICENSE` & `playsound3-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `playsound3-2.0.1/PKG-INFO` & `playsound3-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playsound3
-Version: 2.0.1
+Version: 2.0.2
 Summary: Cross-platform library to play audio files
 Home-page: https://github.com/sjmikler/playsound3
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Keywords: sound playsound music wave wav mp3 media song play audio
 Classifier: License :: OSI Approved :: MIT License
@@ -65,8 +65,8 @@
 It requires one argument - the path to the file with the sound you'd like to play. This may be a local file, or a URL.
 There's an optional second argument, block, which is set to True by default. Setting it to False makes the function run asynchronously.
 
 ## Supported systems
 
 * Linux, using GStreamer (built-in on Linux distributions)
 * Windows, using windll.winmm (built-in on Windows)
-* OS X using afplay utility (built-in OS X)
+* OS X, using afplay utility (built-in OS X)
```

### Comparing `playsound3-2.0.1/README.md` & `playsound3-2.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,8 @@
 It requires one argument - the path to the file with the sound you'd like to play. This may be a local file, or a URL.
 There's an optional second argument, block, which is set to True by default. Setting it to False makes the function run asynchronously.
 
 ## Supported systems
 
 * Linux, using GStreamer (built-in on Linux distributions)
 * Windows, using windll.winmm (built-in on Windows)
-* OS X using afplay utility (built-in OS X)
+* OS X, using afplay utility (built-in OS X)
```

### Comparing `playsound3-2.0.1/playsound3/playsound3.py` & `playsound3-2.0.2/playsound3/playsound3.py`

 * *Files identical despite different names*

### Comparing `playsound3-2.0.1/playsound3.egg-info/PKG-INFO` & `playsound3-2.0.2/playsound3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playsound3
-Version: 2.0.1
+Version: 2.0.2
 Summary: Cross-platform library to play audio files
 Home-page: https://github.com/sjmikler/playsound3
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Keywords: sound playsound music wave wav mp3 media song play audio
 Classifier: License :: OSI Approved :: MIT License
@@ -65,8 +65,8 @@
 It requires one argument - the path to the file with the sound you'd like to play. This may be a local file, or a URL.
 There's an optional second argument, block, which is set to True by default. Setting it to False makes the function run asynchronously.
 
 ## Supported systems
 
 * Linux, using GStreamer (built-in on Linux distributions)
 * Windows, using windll.winmm (built-in on Windows)
-* OS X using afplay utility (built-in OS X)
+* OS X, using afplay utility (built-in OS X)
```

### Comparing `playsound3-2.0.1/setup.py` & `playsound3-2.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     return Path(__file__).parent / path
 
 
 long_description = package_relative_path("README.md").read_text(encoding="UTF-8")
 
 setup(
     name="playsound3",
-    version="2.0.1",
+    version="2.0.2",
     description="Cross-platform library to play audio files",
     url="https://github.com/sjmikler/playsound3",
     author="Szymon Mikler",
     author_email="sjmikler@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

