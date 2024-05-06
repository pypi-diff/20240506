# Comparing `tmp/owntools-1.0.tar.gz` & `tmp/owntools-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owntools-1.0.tar", last modified: Mon May  6 01:51:25 2024, max compression
+gzip compressed data, was "owntools-1.2.tar", last modified: Mon May  6 03:13:43 2024, max compression
```

## Comparing `owntools-1.0.tar` & `owntools-1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 01:51:25.637114 owntools-1.0/
--rw-rw-rw-   0        0        0      362 2024-05-06 01:51:25.637114 owntools-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       34 2021-12-27 10:09:09.000000 owntools-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 01:51:25.621478 owntools-1.0/code/
--rw-rw-rw-   0        0        0     4368 2022-06-06 01:42:41.000000 owntools-1.0/code/Common.py
--rw-rw-rw-   0        0        0     3047 2023-04-12 07:57:53.000000 owntools-1.0/code/CrackCode.py
--rw-rw-rw-   0        0        0     6370 2023-04-12 07:57:53.000000 owntools-1.0/code/Download.py
--rw-rw-rw-   0        0        0     1459 2021-12-27 06:01:19.000000 owntools-1.0/code/ExtractFile.py
--rw-rw-rw-   0        0        0      948 2021-12-27 06:01:41.000000 owntools-1.0/code/Image.py
--rw-rw-rw-   0        0        0     1169 2024-05-06 01:00:34.000000 owntools-1.0/code/Loger.py
--rw-rw-rw-   0        0        0     2496 2022-12-13 02:02:22.000000 owntools-1.0/code/Mysql.py
--rw-rw-rw-   0        0        0     2965 2021-12-29 01:50:41.000000 owntools-1.0/code/Subtitles.py
--rw-rw-rw-   0        0        0     2081 2023-02-15 06:12:42.000000 owntools-1.0/code/Time.py
--rw-rw-rw-   0        0        0     4565 2022-01-12 06:36:41.000000 owntools-1.0/code/Translation.py
--rw-rw-rw-   0        0        0      396 2021-12-27 06:01:33.000000 owntools-1.0/code/UncompressRAR.py
--rw-rw-rw-   0        0        0     2343 2023-02-09 00:55:34.000000 owntools-1.0/code/_SSH.py
--rw-rw-rw-   0        0        0      398 2023-02-09 00:55:34.000000 owntools-1.0/code/__init__.py
--rw-rw-rw-   0        0        0     2839 2022-08-25 00:51:34.000000 owntools-1.0/code/ownEmail.py
-drwxrwxrwx   0        0        0        0 2024-05-06 01:51:25.637114 owntools-1.0/owntools.egg-info/
--rw-rw-rw-   0        0        0      362 2024-05-06 01:51:25.000000 owntools-1.0/owntools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2024-05-06 01:51:25.000000 owntools-1.0/owntools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 01:51:25.000000 owntools-1.0/owntools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-06 01:51:25.000000 owntools-1.0/owntools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 01:51:25.637114 owntools-1.0/setup.cfg
--rw-rw-rw-   0        0        0      534 2024-05-06 01:50:44.000000 owntools-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:13:43.370798 owntools-1.2/
+-rw-rw-rw-   0        0        0      362 2024-05-06 03:13:43.370798 owntools-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       34 2021-12-27 10:09:09.000000 owntools-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 03:13:43.358280 owntools-1.2/owntools.egg-info/
+-rw-rw-rw-   0        0        0      362 2024-05-06 03:13:43.000000 owntools-1.2/owntools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2024-05-06 03:13:43.000000 owntools-1.2/owntools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 03:13:43.000000 owntools-1.2/owntools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-05-06 03:13:43.000000 owntools-1.2/owntools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 03:13:43.370798 owntools-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      534 2024-05-06 03:13:27.000000 owntools-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:13:43.366804 owntools-1.2/src/
+-rw-rw-rw-   0        0        0     4368 2022-06-06 01:42:41.000000 owntools-1.2/src/Common.py
+-rw-rw-rw-   0        0        0     3047 2023-04-12 07:57:53.000000 owntools-1.2/src/CrackCode.py
+-rw-rw-rw-   0        0        0     6370 2023-04-12 07:57:53.000000 owntools-1.2/src/Download.py
+-rw-rw-rw-   0        0        0     1459 2021-12-27 06:01:19.000000 owntools-1.2/src/ExtractFile.py
+-rw-rw-rw-   0        0        0      948 2021-12-27 06:01:41.000000 owntools-1.2/src/Image.py
+-rw-rw-rw-   0        0        0     1169 2024-05-06 01:00:34.000000 owntools-1.2/src/Loger.py
+-rw-rw-rw-   0        0        0     2496 2022-12-13 02:02:22.000000 owntools-1.2/src/Mysql.py
+-rw-rw-rw-   0        0        0     2965 2021-12-29 01:50:41.000000 owntools-1.2/src/Subtitles.py
+-rw-rw-rw-   0        0        0     2081 2023-02-15 06:12:42.000000 owntools-1.2/src/Time.py
+-rw-rw-rw-   0        0        0     4565 2022-01-12 06:36:41.000000 owntools-1.2/src/Translation.py
+-rw-rw-rw-   0        0        0      396 2021-12-27 06:01:33.000000 owntools-1.2/src/UncompressRAR.py
+-rw-rw-rw-   0        0        0     2343 2023-02-09 00:55:34.000000 owntools-1.2/src/_SSH.py
+-rw-rw-rw-   0        0        0      400 2024-05-06 03:05:40.000000 owntools-1.2/src/__init__.py
+-rw-rw-rw-   0        0        0     2839 2022-08-25 00:51:34.000000 owntools-1.2/src/ownEmail.py
```

### Comparing `owntools-1.0/code/Common.py` & `owntools-1.2/src/Common.py`

 * *Files identical despite different names*

### Comparing `owntools-1.0/code/CrackCode.py` & `owntools-1.2/src/CrackCode.py`

 * *Files identical despite different names*

### Comparing `owntools-1.0/code/Download.py` & `owntools-1.2/src/Download.py`

 * *Files identical despite different names*

### Comparing `owntools-1.0/code/ExtractFile.py` & `owntools-1.2/src/ExtractFile.py`

 * *Files identical despite different names*

### Comparing `owntools-1.0/code/Image.py` & `owntools-1.2/src/Image.py`

 * *Files identical despite different names*

### Comparing `owntools-1.0/code/Loger.py` & `owntools-1.2/src/Loger.py`

 * *Files identical despite different names*

### Comparing `owntools-1.0/code/Mysql.py` & `owntools-1.2/src/Mysql.py`

 * *Files identical despite different names*

### Comparing `owntools-1.0/code/Subtitles.py` & `owntools-1.2/src/Subtitles.py`

 * *Files identical despite different names*

### Comparing `owntools-1.0/code/Time.py` & `owntools-1.2/src/Time.py`

 * *Files identical despite different names*

### Comparing `owntools-1.0/code/Translation.py` & `owntools-1.2/src/Translation.py`

 * *Files identical despite different names*

### Comparing `owntools-1.0/code/_SSH.py` & `owntools-1.2/src/_SSH.py`

 * *Files identical despite different names*

### Comparing `owntools-1.0/code/ownEmail.py` & `owntools-1.2/src/ownEmail.py`

 * *Files identical despite different names*

### Comparing `owntools-1.0/setup.py` & `owntools-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 print(find_packages())
 
 setup(
     name='owntools',
-    version='1.0',
+    version='1.2',
     packages=find_packages(),
     description='Tools for myself',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Neely',
     author_email='liangxiuyu@outlook.com',
     url='https://github.com/liangxiuyu/owntools',
```

