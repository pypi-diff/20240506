# Comparing `tmp/playsound3-2.0.0a0.tar.gz` & `tmp/playsound3-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playsound3-2.0.0a0.tar", last modified: Mon May  6 17:23:56 2024, max compression
+gzip compressed data, was "playsound3-2.0.1.tar", last modified: Mon May  6 17:40:12 2024, max compression
```

## Comparing `playsound3-2.0.0a0.tar` & `playsound3-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:23:56.914131 playsound3-2.0.0a0/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1962 2024-05-06 14:15:46.000000 playsound3-2.0.0a0/LICENSE
--rw-r--r--   0 gaha      (1000) gaha      (1000)     2293 2024-05-06 17:23:56.914131 playsound3-2.0.0a0/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1290 2024-05-06 14:15:50.000000 playsound3-2.0.0a0/README.md
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:23:56.914131 playsound3-2.0.0a0/playsound3/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       44 2024-05-06 14:32:01.000000 playsound3-2.0.0a0/playsound3/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     3096 2024-05-06 17:18:09.000000 playsound3-2.0.0a0/playsound3/playsound3.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:23:56.914131 playsound3-2.0.0a0/playsound3.egg-info/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     2293 2024-05-06 17:23:56.000000 playsound3-2.0.0a0/playsound3.egg-info/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)      258 2024-05-06 17:23:56.000000 playsound3-2.0.0a0/playsound3.egg-info/SOURCES.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-05-06 17:23:56.000000 playsound3-2.0.0a0/playsound3.egg-info/dependency_links.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-05-06 17:23:56.000000 playsound3-2.0.0a0/playsound3.egg-info/requires.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       11 2024-05-06 17:23:56.000000 playsound3-2.0.0a0/playsound3.egg-info/top_level.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-05-06 12:41:28.000000 playsound3-2.0.0a0/pyproject.toml
--rw-r--r--   0 gaha      (1000) gaha      (1000)       38 2024-05-06 17:23:56.914131 playsound3-2.0.0a0/setup.cfg
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1371 2024-05-06 17:23:52.000000 playsound3-2.0.0a0/setup.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:40:12.144879 playsound3-2.0.1/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1962 2024-05-06 14:15:46.000000 playsound3-2.0.1/LICENSE
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     2603 2024-05-06 17:40:12.144879 playsound3-2.0.1/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1602 2024-05-06 17:39:21.000000 playsound3-2.0.1/README.md
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:40:12.144879 playsound3-2.0.1/playsound3/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       44 2024-05-06 14:32:01.000000 playsound3-2.0.1/playsound3/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     3349 2024-05-06 17:36:33.000000 playsound3-2.0.1/playsound3/playsound3.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-05-06 17:40:12.144879 playsound3-2.0.1/playsound3.egg-info/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     2603 2024-05-06 17:40:12.000000 playsound3-2.0.1/playsound3.egg-info/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      258 2024-05-06 17:40:12.000000 playsound3-2.0.1/playsound3.egg-info/SOURCES.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-05-06 17:40:12.000000 playsound3-2.0.1/playsound3.egg-info/dependency_links.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-05-06 17:40:12.000000 playsound3-2.0.1/playsound3.egg-info/requires.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       11 2024-05-06 17:40:12.000000 playsound3-2.0.1/playsound3.egg-info/top_level.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-05-06 12:41:28.000000 playsound3-2.0.1/pyproject.toml
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       38 2024-05-06 17:40:12.144879 playsound3-2.0.1/setup.cfg
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1365 2024-05-06 17:39:46.000000 playsound3-2.0.1/setup.py
```

### Comparing `playsound3-2.0.0a0/LICENSE` & `playsound3-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `playsound3-2.0.0a0/PKG-INFO` & `playsound3-2.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playsound3
-Version: 2.0.0a0
+Version: 2.0.1
 Summary: Cross-platform library to play audio files
 Home-page: https://github.com/sjmikler/playsound3
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Keywords: sound playsound music wave wav mp3 media song play audio
 Classifier: License :: OSI Approved :: MIT License
@@ -19,42 +19,54 @@
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players :: MP3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygobject; platform_system == "Linux"
 
-> Note: this repository is an attempt to fix playsound library
+> This repository was initially forked from [TaylorSMarks/playsound](https://github.com/TaylorSMarks/playsound/blob/master/playsound.py)
 
-playsound
-------------
+# Playsound3
 
-Pure Python, cross platform, single function module with no dependencies for playing sounds.
+[![PyPi version](https://img.shields.io/badge/dynamic/json?label=latest&query=info.version&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fplaysound3%2Fjson)](https://pypi.org/project/playsound3)
+[![PyPI license](https://img.shields.io/badge/dynamic/json?label=license&query=info.license&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fplaysound3%2Fjson)](https://pypi.org/project/playsound3)
+
+## Installation
 
-Installation
-------------
 Install via pip:
 
 ```
-pip install playsound
+pip install playsound3
 ```
 
-Quick Start
------------
-Once you've installed, you can really quickly verified that it works with just this:
+## Quick Start
+
+Once installed, you can use the playsound function to play sound files:
 
 ```python
-from playsound2 import playsound
+from playsound3 import playsound
 
-playsound('/path/to/a/sound/file/you/want/to/play.mp3') 
+playsound("/path/to/sound/file.mp3")
 ```
 
-Documentation
--------------
-The playsound module contains only one thing - the function (also named) playsound.
+## Documentation
+
+The playsound module contains only one thing - the function (also named) playsound:
+
+```python
+def playsound(sound: os.PathLike, block: bool = True) -> None:
+    """Play a sound file using an audio player availabile on your system.
+
+    Args:
+        sound: Path to the sound file.
+        block: If True, the function will block execution until the sound finishes playing.
+    """
+```
 
 It requires one argument - the path to the file with the sound you'd like to play. This may be a local file, or a URL.
 There's an optional second argument, block, which is set to True by default. Setting it to False makes the function run asynchronously.
 
-On Windows, uses windll.winmm. WAVE and MP3 have been tested and are known to work. Other file formats may work as well.
-On OS X, uses AppKit.NSSound. WAVE and MP3 have been tested and are known to work. In general, anything QuickTime can play, playsound should be able to play, for OS X.
-On Linux, uses GStreamer. Known to work on Ubuntu 14.04 and ElementaryOS Loki. I expect any Linux distro with a standard gnome desktop experience should work.
+## Supported systems
+
+* Linux, using GStreamer (built-in on Linux distributions)
+* Windows, using windll.winmm (built-in on Windows)
+* OS X using afplay utility (built-in OS X)
```

### Comparing `playsound3-2.0.0a0/playsound3/playsound3.py` & `playsound3-2.0.1/playsound3/playsound3.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,21 @@
 SYSTEM = system()
 
 
 class PlaysoundException(Exception):
     pass
 
 
-def playsound(sound, block=True):
+def playsound(sound: os.PathLike, block: bool = True) -> None:
+    """Play a sound file using an audio player availabile on your system.
+
+    Args:
+        sound: Path to the sound file.
+        block: If True, the function will block execution until the sound finishes playing.
+    """
     sound = _prepare_path(sound)
 
     if SYSTEM == "Linux":
         func = _playsound_gstreamer
     elif SYSTEM == "Windows":
         func = _playsound_winmm
     elif SYSTEM == "Darwin":
```

### Comparing `playsound3-2.0.0a0/playsound3.egg-info/PKG-INFO` & `playsound3-2.0.1/playsound3.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playsound3
-Version: 2.0.0a0
+Version: 2.0.1
 Summary: Cross-platform library to play audio files
 Home-page: https://github.com/sjmikler/playsound3
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Keywords: sound playsound music wave wav mp3 media song play audio
 Classifier: License :: OSI Approved :: MIT License
@@ -19,42 +19,54 @@
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players :: MP3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygobject; platform_system == "Linux"
 
-> Note: this repository is an attempt to fix playsound library
+> This repository was initially forked from [TaylorSMarks/playsound](https://github.com/TaylorSMarks/playsound/blob/master/playsound.py)
 
-playsound
-------------
+# Playsound3
 
-Pure Python, cross platform, single function module with no dependencies for playing sounds.
+[![PyPi version](https://img.shields.io/badge/dynamic/json?label=latest&query=info.version&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fplaysound3%2Fjson)](https://pypi.org/project/playsound3)
+[![PyPI license](https://img.shields.io/badge/dynamic/json?label=license&query=info.license&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fplaysound3%2Fjson)](https://pypi.org/project/playsound3)
+
+## Installation
 
-Installation
-------------
 Install via pip:
 
 ```
-pip install playsound
+pip install playsound3
 ```
 
-Quick Start
------------
-Once you've installed, you can really quickly verified that it works with just this:
+## Quick Start
+
+Once installed, you can use the playsound function to play sound files:
 
 ```python
-from playsound2 import playsound
+from playsound3 import playsound
 
-playsound('/path/to/a/sound/file/you/want/to/play.mp3') 
+playsound("/path/to/sound/file.mp3")
 ```
 
-Documentation
--------------
-The playsound module contains only one thing - the function (also named) playsound.
+## Documentation
+
+The playsound module contains only one thing - the function (also named) playsound:
+
+```python
+def playsound(sound: os.PathLike, block: bool = True) -> None:
+    """Play a sound file using an audio player availabile on your system.
+
+    Args:
+        sound: Path to the sound file.
+        block: If True, the function will block execution until the sound finishes playing.
+    """
+```
 
 It requires one argument - the path to the file with the sound you'd like to play. This may be a local file, or a URL.
 There's an optional second argument, block, which is set to True by default. Setting it to False makes the function run asynchronously.
 
-On Windows, uses windll.winmm. WAVE and MP3 have been tested and are known to work. Other file formats may work as well.
-On OS X, uses AppKit.NSSound. WAVE and MP3 have been tested and are known to work. In general, anything QuickTime can play, playsound should be able to play, for OS X.
-On Linux, uses GStreamer. Known to work on Ubuntu 14.04 and ElementaryOS Loki. I expect any Linux distro with a standard gnome desktop experience should work.
+## Supported systems
+
+* Linux, using GStreamer (built-in on Linux distributions)
+* Windows, using windll.winmm (built-in on Windows)
+* OS X using afplay utility (built-in OS X)
```

### Comparing `playsound3-2.0.0a0/setup.py` & `playsound3-2.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     return Path(__file__).parent / path
 
 
 long_description = package_relative_path("README.md").read_text(encoding="UTF-8")
 
 setup(
     name="playsound3",
-    version="2.0.0-alpha",
+    version="2.0.1",
     description="Cross-platform library to play audio files",
     url="https://github.com/sjmikler/playsound3",
     author="Szymon Mikler",
     author_email="sjmikler@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

