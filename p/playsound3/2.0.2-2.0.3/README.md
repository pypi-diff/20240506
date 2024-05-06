# Comparing `tmp/playsound3-2.0.2.tar.gz` & `tmp/playsound3-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playsound3-2.0.2.tar", last modified: Mon May  6 17:42:27 2024, max compression
+gzip compressed data, was "playsound3-2.0.3.tar", last modified: Mon May  6 17:49:43 2024, max compression
```

## Comparing `playsound3-2.0.2.tar` & `playsound3-2.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:42:27.758476 playsound3-2.0.2/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1962 2024-05-06 14:15:46.000000 playsound3-2.0.2/LICENSE
--rw-r--r--   0 gaha      (1000) gaha      (1000)     2604 2024-05-06 17:42:27.758476 playsound3-2.0.2/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1603 2024-05-06 17:42:11.000000 playsound3-2.0.2/README.md
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:42:27.758476 playsound3-2.0.2/playsound3/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       44 2024-05-06 14:32:01.000000 playsound3-2.0.2/playsound3/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     3349 2024-05-06 17:36:33.000000 playsound3-2.0.2/playsound3/playsound3.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:42:27.758476 playsound3-2.0.2/playsound3.egg-info/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     2604 2024-05-06 17:42:27.000000 playsound3-2.0.2/playsound3.egg-info/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)      258 2024-05-06 17:42:27.000000 playsound3-2.0.2/playsound3.egg-info/SOURCES.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-05-06 17:42:27.000000 playsound3-2.0.2/playsound3.egg-info/dependency_links.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-05-06 17:42:27.000000 playsound3-2.0.2/playsound3.egg-info/requires.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       11 2024-05-06 17:42:27.000000 playsound3-2.0.2/playsound3.egg-info/top_level.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-05-06 12:41:28.000000 playsound3-2.0.2/pyproject.toml
--rw-r--r--   0 gaha      (1000) gaha      (1000)       38 2024-05-06 17:42:27.758476 playsound3-2.0.2/setup.cfg
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1365 2024-05-06 17:42:18.000000 playsound3-2.0.2/setup.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:49:43.481451 playsound3-2.0.3/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1962 2024-05-06 14:15:46.000000 playsound3-2.0.3/LICENSE
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     2597 2024-05-06 17:49:43.481451 playsound3-2.0.3/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1596 2024-05-06 17:49:06.000000 playsound3-2.0.3/README.md
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:49:43.481451 playsound3-2.0.3/playsound3/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       44 2024-05-06 14:32:01.000000 playsound3-2.0.3/playsound3/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     3346 2024-05-06 17:46:33.000000 playsound3-2.0.3/playsound3/playsound3.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:49:43.481451 playsound3-2.0.3/playsound3.egg-info/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     2597 2024-05-06 17:49:43.000000 playsound3-2.0.3/playsound3.egg-info/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      258 2024-05-06 17:49:43.000000 playsound3-2.0.3/playsound3.egg-info/SOURCES.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-05-06 17:49:43.000000 playsound3-2.0.3/playsound3.egg-info/dependency_links.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-05-06 17:49:43.000000 playsound3-2.0.3/playsound3.egg-info/requires.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       11 2024-05-06 17:49:43.000000 playsound3-2.0.3/playsound3.egg-info/top_level.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-05-06 12:41:28.000000 playsound3-2.0.3/pyproject.toml
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       38 2024-05-06 17:49:43.481451 playsound3-2.0.3/setup.cfg
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1365 2024-05-06 17:49:15.000000 playsound3-2.0.3/setup.py
```

### Comparing `playsound3-2.0.2/LICENSE` & `playsound3-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `playsound3-2.0.2/PKG-INFO` & `playsound3-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playsound3
-Version: 2.0.2
+Version: 2.0.3
 Summary: Cross-platform library to play audio files
 Home-page: https://github.com/sjmikler/playsound3
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Keywords: sound playsound music wave wav mp3 media song play audio
 Classifier: License :: OSI Approved :: MIT License
@@ -58,15 +58,17 @@
 
     Args:
         sound: Path to the sound file.
         block: If True, the function will block execution until the sound finishes playing.
     """
 ```
 
-It requires one argument - the path to the file with the sound you'd like to play. This may be a local file, or a URL.
-There's an optional second argument, block, which is set to True by default. Setting it to False makes the function run asynchronously.
+It requires one argument - the path to the file with the sound you'd like to play.
+This should be a local file.
+There's an optional second argument, block, which is set to True by default.
+Setting it to False makes the function run asynchronously.
 
 ## Supported systems
 
 * Linux, using GStreamer (built-in on Linux distributions)
 * Windows, using windll.winmm (built-in on Windows)
 * OS X, using afplay utility (built-in OS X)
```

### Comparing `playsound3-2.0.2/README.md` & `playsound3-2.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 
     Args:
         sound: Path to the sound file.
         block: If True, the function will block execution until the sound finishes playing.
     """
 ```
 
-It requires one argument - the path to the file with the sound you'd like to play. This may be a local file, or a URL.
-There's an optional second argument, block, which is set to True by default. Setting it to False makes the function run asynchronously.
+It requires one argument - the path to the file with the sound you'd like to play.
+This should be a local file.
+There's an optional second argument, block, which is set to True by default.
+Setting it to False makes the function run asynchronously.
 
 ## Supported systems
 
 * Linux, using GStreamer (built-in on Linux distributions)
 * Windows, using windll.winmm (built-in on Windows)
 * OS X, using afplay utility (built-in OS X)
```

### Comparing `playsound3-2.0.2/playsound3/playsound3.py` & `playsound3-2.0.3/playsound3/playsound3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import ctypes
 import logging
 import os
+import platform
 import subprocess
 import uuid
 from pathlib import Path
-from platform import system
 from threading import Thread
 from urllib.request import pathname2url
 
 logger = logging.getLogger(__name__)
 
-SYSTEM = system()
+SYSTEM = platform.system()
 
 
 class PlaysoundException(Exception):
     pass
 
 
 def playsound(sound: os.PathLike, block: bool = True) -> None:
```

### Comparing `playsound3-2.0.2/playsound3.egg-info/PKG-INFO` & `playsound3-2.0.3/playsound3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playsound3
-Version: 2.0.2
+Version: 2.0.3
 Summary: Cross-platform library to play audio files
 Home-page: https://github.com/sjmikler/playsound3
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Keywords: sound playsound music wave wav mp3 media song play audio
 Classifier: License :: OSI Approved :: MIT License
@@ -58,15 +58,17 @@
 
     Args:
         sound: Path to the sound file.
         block: If True, the function will block execution until the sound finishes playing.
     """
 ```
 
-It requires one argument - the path to the file with the sound you'd like to play. This may be a local file, or a URL.
-There's an optional second argument, block, which is set to True by default. Setting it to False makes the function run asynchronously.
+It requires one argument - the path to the file with the sound you'd like to play.
+This should be a local file.
+There's an optional second argument, block, which is set to True by default.
+Setting it to False makes the function run asynchronously.
 
 ## Supported systems
 
 * Linux, using GStreamer (built-in on Linux distributions)
 * Windows, using windll.winmm (built-in on Windows)
 * OS X, using afplay utility (built-in OS X)
```

### Comparing `playsound3-2.0.2/setup.py` & `playsound3-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     return Path(__file__).parent / path
 
 
 long_description = package_relative_path("README.md").read_text(encoding="UTF-8")
 
 setup(
     name="playsound3",
-    version="2.0.2",
+    version="2.0.3",
     description="Cross-platform library to play audio files",
     url="https://github.com/sjmikler/playsound3",
     author="Szymon Mikler",
     author_email="sjmikler@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

