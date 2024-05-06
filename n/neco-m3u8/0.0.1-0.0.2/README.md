# Comparing `tmp/neco_m3u8-0.0.1.tar.gz` & `tmp/neco_m3u8-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neco_m3u8-0.0.1.tar", last modified: Mon May  6 12:18:39 2024, max compression
+gzip compressed data, was "neco_m3u8-0.0.2.tar", last modified: Mon May  6 12:24:39 2024, max compression
```

## Comparing `neco_m3u8-0.0.1.tar` & `neco_m3u8-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 12:18:39.615502 neco_m3u8-0.0.1/
--rw-rw-rw-   0        0        0      593 2024-05-06 12:18:39.615502 neco_m3u8-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       62 2024-05-06 12:04:48.000000 neco_m3u8-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 12:18:39.614505 neco_m3u8-0.0.1/neco_m3u8.egg-info/
--rw-rw-rw-   0        0        0      593 2024-05-06 12:18:39.000000 neco_m3u8-0.0.1/neco_m3u8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-05-06 12:18:39.000000 neco_m3u8-0.0.1/neco_m3u8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 12:18:39.000000 neco_m3u8-0.0.1/neco_m3u8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-06 12:18:39.000000 neco_m3u8-0.0.1/neco_m3u8.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-06 12:18:39.000000 neco_m3u8-0.0.1/neco_m3u8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 12:18:39.616500 neco_m3u8-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      939 2024-05-06 12:18:39.000000 neco_m3u8-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 12:18:39.613508 neco_m3u8-0.0.1/src/
--rw-rw-rw-   0        0        0     1332 2024-05-06 10:12:25.000000 neco_m3u8-0.0.1/src/decrypto.py
--rw-rw-rw-   0        0        0     1456 2024-05-06 11:49:58.000000 neco_m3u8-0.0.1/src/ffmpeg.py
--rw-rw-rw-   0        0        0     7855 2024-05-06 12:16:28.000000 neco_m3u8-0.0.1/src/neco_m3u8.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:24:39.724205 neco_m3u8-0.0.2/
+-rw-rw-rw-   0        0        0      593 2024-05-06 12:24:39.723209 neco_m3u8-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       62 2024-05-06 12:04:48.000000 neco_m3u8-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 12:24:39.723209 neco_m3u8-0.0.2/neco_m3u8.egg-info/
+-rw-rw-rw-   0        0        0      593 2024-05-06 12:24:39.000000 neco_m3u8-0.0.2/neco_m3u8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-05-06 12:24:39.000000 neco_m3u8-0.0.2/neco_m3u8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 12:24:39.000000 neco_m3u8-0.0.2/neco_m3u8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-06 12:24:39.000000 neco_m3u8-0.0.2/neco_m3u8.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-06 12:24:39.000000 neco_m3u8-0.0.2/neco_m3u8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 12:24:39.724205 neco_m3u8-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      939 2024-05-06 12:24:39.000000 neco_m3u8-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:24:39.722211 neco_m3u8-0.0.2/src/
+-rw-rw-rw-   0        0        0     1332 2024-05-06 10:12:25.000000 neco_m3u8-0.0.2/src/decrypto.py
+-rw-rw-rw-   0        0        0     1456 2024-05-06 11:49:58.000000 neco_m3u8-0.0.2/src/ffmpeg.py
+-rw-rw-rw-   0        0        0     7870 2024-05-06 12:24:29.000000 neco_m3u8-0.0.2/src/neco_m3u8.py
```

### Comparing `neco_m3u8-0.0.1/PKG-INFO` & `neco_m3u8-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neco_m3u8
-Version: 0.0.1
+Version: 0.0.2
 Summary: m3u8解析与下载库,自动获取key解密,需要ffmpeg用于合并ts流
 Home-page: 
 Author: neco_arc
 Author-email: 3306601284@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neco_m3u8-0.0.1/neco_m3u8.egg-info/PKG-INFO` & `neco_m3u8-0.0.2/neco_m3u8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neco_m3u8
-Version: 0.0.1
+Version: 0.0.2
 Summary: m3u8解析与下载库,自动获取key解密,需要ffmpeg用于合并ts流
 Home-page: 
 Author: neco_arc
 Author-email: 3306601284@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neco_m3u8-0.0.1/setup.py` & `neco_m3u8-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 name = 'neco_m3u8'
 author = 'neco_arc'
 description = 'm3u8解析与下载库,自动获取key解密,需要ffmpeg用于合并ts流'
 email = '3306601284@qq.com'
 
 with open('README.md', mode='r', encoding='utf-8') as f:
     long_description = f.read()
```

### Comparing `neco_m3u8-0.0.1/src/decrypto.py` & `neco_m3u8-0.0.2/src/decrypto.py`

 * *Files identical despite different names*

### Comparing `neco_m3u8-0.0.1/src/ffmpeg.py` & `neco_m3u8-0.0.2/src/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `neco_m3u8-0.0.1/src/neco_m3u8.py` & `neco_m3u8-0.0.2/src/neco_m3u8.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import requests
 import m3u8
 import threading
 from DownloadKit import DownloadKit
 from m3u8 import M3U8, Segment
 from urllib.parse import urljoin
-import decrypto, ffmpeg
+from neco_m3u8 import decrypto, ffmpeg
 
 
 class Neco_m3u8:
     def __init__(self):
         self.all_ts_links = []
         self.kit = DownloadKit()
         self.thread_list = []
```

