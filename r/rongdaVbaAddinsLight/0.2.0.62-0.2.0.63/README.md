# Comparing `tmp/rongdaVbaAddinsLight-0.2.0.62.tar.gz` & `tmp/rongdaVbaAddinsLight-0.2.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rongdaVbaAddinsLight-0.2.0.62.tar", last modified: Tue Apr  2 03:43:48 2024, max compression
+gzip compressed data, was "rongdaVbaAddinsLight-0.2.0.63.tar", last modified: Mon May  6 08:27:41 2024, max compression
```

## Comparing `rongdaVbaAddinsLight-0.2.0.62.tar` & `rongdaVbaAddinsLight-0.2.0.63.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 03:43:48.057919 rongdaVbaAddinsLight-0.2.0.62/
--rw-rw-rw-   0        0        0        0 2023-10-11 02:09:37.000000 rongdaVbaAddinsLight-0.2.0.62/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdaVbaAddinsLight-0.2.0.62/MANIFEST.in
--rw-rw-rw-   0        0        0      405 2024-04-02 03:43:48.056911 rongdaVbaAddinsLight-0.2.0.62/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-10-11 02:09:37.000000 rongdaVbaAddinsLight-0.2.0.62/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 03:43:48.025907 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/
-drwxrwxrwx   0        0        0        0 2024-04-02 03:43:48.040906 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/Function/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/Function/__init__.py
--rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/Function/minusFunction.pyd
--rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/Function/minusFunctionpy.py
--rw-rw-rw-   0        0        0  1998544 2024-04-02 03:41:08.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/RDaddins.xlam
--rw-rw-rw-   0        0        0     8192 2023-08-21 07:30:54.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/RecentTime.db
-drwxrwxrwx   0        0        0        0 2024-04-02 03:43:48.044908 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/Ui/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/Ui/__init__.py
--rw-rw-rw-   0        0        0    66560 2023-08-17 01:40:15.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/Ui/rongdaVbaAddinsUi.pyd
--rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 03:43:48.046906 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/package/
--rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/package/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 03:43:48.054908 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/package/pyzipper/
--rw-rw-rw-   0        0        0      152 2023-12-29 05:53:14.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/package/pyzipper/__init__.py
--rw-rw-rw-   0        0        0       63 2023-12-29 05:53:05.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/package/pyzipper/__version__.py
--rw-rw-rw-   0        0        0    95557 2023-12-29 05:53:06.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/package/pyzipper/zipfile.py
--rw-rw-rw-   0        0        0    11589 2023-12-29 05:52:58.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/package/pyzipper/zipfile_aes.py
--rw-rw-rw-   0        0        0   388096 2024-01-17 01:38:22.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/registerCode.pyd
--rw-rw-rw-   0        0        0   210944 2024-04-02 03:18:31.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/rongdavbaaddinsLight.pyd
--rw-rw-rw-   0        0        0      152 2023-08-22 06:02:10.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/runregiterCode.py
--rw-rw-rw-   0        0        0    57354 2024-04-02 03:41:08.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/文件处理类模板.xlsx
-drwxrwxrwx   0        0        0        0 2024-04-02 03:43:48.033932 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight.egg-info/
--rw-rw-rw-   0        0        0      405 2024-04-02 03:43:47.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      969 2024-04-02 03:43:47.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 03:43:47.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-04-02 03:43:47.000000 rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2024-04-02 03:43:48.059910 rongdaVbaAddinsLight-0.2.0.62/setup.cfg
--rw-rw-rw-   0        0        0     1032 2024-04-02 03:42:17.000000 rongdaVbaAddinsLight-0.2.0.62/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:27:41.645329 rongdaVbaAddinsLight-0.2.0.63/
+-rw-rw-rw-   0        0        0        0 2023-10-11 02:09:37.000000 rongdaVbaAddinsLight-0.2.0.63/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdaVbaAddinsLight-0.2.0.63/MANIFEST.in
+-rw-rw-rw-   0        0        0      405 2024-05-06 08:27:41.643332 rongdaVbaAddinsLight-0.2.0.63/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2023-10-11 02:09:37.000000 rongdaVbaAddinsLight-0.2.0.63/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 08:27:41.597326 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/
+drwxrwxrwx   0        0        0        0 2024-05-06 08:27:41.618366 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/Function/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/Function/__init__.py
+-rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/Function/minusFunction.pyd
+-rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/Function/minusFunctionpy.py
+-rw-rw-rw-   0        0        0  1998544 2024-04-02 03:41:08.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/RDaddins.xlam
+-rw-rw-rw-   0        0        0     8192 2023-08-21 07:30:54.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/RecentTime.db
+drwxrwxrwx   0        0        0        0 2024-05-06 08:27:41.624334 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/Ui/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/Ui/__init__.py
+-rw-rw-rw-   0        0        0    66560 2023-08-17 01:40:15.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/Ui/rongdaVbaAddinsUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:27:41.628330 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/
+-rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:27:41.641331 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/pyzipper/
+-rw-rw-rw-   0        0        0      152 2023-12-29 05:53:14.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/pyzipper/__init__.py
+-rw-rw-rw-   0        0        0       63 2023-12-29 05:53:05.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/pyzipper/__version__.py
+-rw-rw-rw-   0        0        0    95557 2023-12-29 05:53:06.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/pyzipper/zipfile.py
+-rw-rw-rw-   0        0        0    11589 2023-12-29 05:52:58.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/pyzipper/zipfile_aes.py
+-rw-rw-rw-   0        0        0   379904 2024-05-06 08:16:13.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/registerCode.pyd
+-rw-rw-rw-   0        0        0   210944 2024-05-06 08:27:08.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/rongdavbaaddinsLight.pyd
+-rw-rw-rw-   0        0        0      152 2023-08-22 06:02:10.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/runregiterCode.py
+-rw-rw-rw-   0        0        0    57354 2024-04-02 03:41:08.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/文件处理类模板.xlsx
+drwxrwxrwx   0        0        0        0 2024-05-06 08:27:41.610330 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight.egg-info/
+-rw-rw-rw-   0        0        0      405 2024-05-06 08:27:41.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      969 2024-05-06 08:27:41.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 08:27:41.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-05-06 08:27:41.000000 rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2024-05-06 08:27:41.646329 rongdaVbaAddinsLight-0.2.0.63/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2024-05-06 08:24:19.000000 rongdaVbaAddinsLight-0.2.0.63/setup.py
```

### Comparing `rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/RDaddins.xlam` & `rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/RDaddins.xlam`

 * *Files identical despite different names*

### Comparing `rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/RecentTime.db` & `rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/RecentTime.db`

 * *Files identical despite different names*

### Comparing `rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/package/pyzipper/zipfile.py` & `rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/pyzipper/zipfile.py`

 * *Files identical despite different names*

### Comparing `rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/package/pyzipper/zipfile_aes.py` & `rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/package/pyzipper/zipfile_aes.py`

 * *Files identical despite different names*

### Comparing `rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight/文件处理类模板.xlsx` & `rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight/文件处理类模板.xlsx`

 * *Files identical despite different names*

### Comparing `rongdaVbaAddinsLight-0.2.0.62/rongdaVbaAddinsLight.egg-info/SOURCES.txt` & `rongdaVbaAddinsLight-0.2.0.63/rongdaVbaAddinsLight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rongdaVbaAddinsLight-0.2.0.62/setup.py` & `rongdaVbaAddinsLight-0.2.0.63/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 2
 PATCH = 0
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}.62"
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.63"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "rongdaVbaAddinsLight",
     version=VERSION,
```

