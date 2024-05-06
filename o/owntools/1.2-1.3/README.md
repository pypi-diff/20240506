# Comparing `tmp/owntools-1.2.tar.gz` & `tmp/owntools-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owntools-1.2.tar", last modified: Mon May  6 03:13:43 2024, max compression
+gzip compressed data, was "owntools-1.3.tar", last modified: Mon May  6 06:05:02 2024, max compression
```

## Comparing `owntools-1.2.tar` & `owntools-1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 03:13:43.370798 owntools-1.2/
--rw-rw-rw-   0        0        0      362 2024-05-06 03:13:43.370798 owntools-1.2/PKG-INFO
--rw-rw-rw-   0        0        0       34 2021-12-27 10:09:09.000000 owntools-1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 03:13:43.358280 owntools-1.2/owntools.egg-info/
--rw-rw-rw-   0        0        0      362 2024-05-06 03:13:43.000000 owntools-1.2/owntools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2024-05-06 03:13:43.000000 owntools-1.2/owntools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 03:13:43.000000 owntools-1.2/owntools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-05-06 03:13:43.000000 owntools-1.2/owntools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 03:13:43.370798 owntools-1.2/setup.cfg
--rw-rw-rw-   0        0        0      534 2024-05-06 03:13:27.000000 owntools-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:13:43.366804 owntools-1.2/src/
--rw-rw-rw-   0        0        0     4368 2022-06-06 01:42:41.000000 owntools-1.2/src/Common.py
--rw-rw-rw-   0        0        0     3047 2023-04-12 07:57:53.000000 owntools-1.2/src/CrackCode.py
--rw-rw-rw-   0        0        0     6370 2023-04-12 07:57:53.000000 owntools-1.2/src/Download.py
--rw-rw-rw-   0        0        0     1459 2021-12-27 06:01:19.000000 owntools-1.2/src/ExtractFile.py
--rw-rw-rw-   0        0        0      948 2021-12-27 06:01:41.000000 owntools-1.2/src/Image.py
--rw-rw-rw-   0        0        0     1169 2024-05-06 01:00:34.000000 owntools-1.2/src/Loger.py
--rw-rw-rw-   0        0        0     2496 2022-12-13 02:02:22.000000 owntools-1.2/src/Mysql.py
--rw-rw-rw-   0        0        0     2965 2021-12-29 01:50:41.000000 owntools-1.2/src/Subtitles.py
--rw-rw-rw-   0        0        0     2081 2023-02-15 06:12:42.000000 owntools-1.2/src/Time.py
--rw-rw-rw-   0        0        0     4565 2022-01-12 06:36:41.000000 owntools-1.2/src/Translation.py
--rw-rw-rw-   0        0        0      396 2021-12-27 06:01:33.000000 owntools-1.2/src/UncompressRAR.py
--rw-rw-rw-   0        0        0     2343 2023-02-09 00:55:34.000000 owntools-1.2/src/_SSH.py
--rw-rw-rw-   0        0        0      400 2024-05-06 03:05:40.000000 owntools-1.2/src/__init__.py
--rw-rw-rw-   0        0        0     2839 2022-08-25 00:51:34.000000 owntools-1.2/src/ownEmail.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:05:02.365914 owntools-1.3/
+-rw-rw-rw-   0        0        0      362 2024-05-06 06:05:02.365914 owntools-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       34 2021-12-27 10:09:09.000000 owntools-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 06:05:02.357924 owntools-1.3/owntools/
+-rw-rw-rw-   0        0        0     4368 2022-06-06 01:42:41.000000 owntools-1.3/owntools/Common.py
+-rw-rw-rw-   0        0        0     3047 2023-04-12 07:57:53.000000 owntools-1.3/owntools/CrackCode.py
+-rw-rw-rw-   0        0        0     6370 2023-04-12 07:57:53.000000 owntools-1.3/owntools/Download.py
+-rw-rw-rw-   0        0        0     1459 2021-12-27 06:01:19.000000 owntools-1.3/owntools/ExtractFile.py
+-rw-rw-rw-   0        0        0      948 2021-12-27 06:01:41.000000 owntools-1.3/owntools/Image.py
+-rw-rw-rw-   0        0        0     1169 2024-05-06 01:00:34.000000 owntools-1.3/owntools/Loger.py
+-rw-rw-rw-   0        0        0     2496 2022-12-13 02:02:22.000000 owntools-1.3/owntools/Mysql.py
+-rw-rw-rw-   0        0        0     2965 2021-12-29 01:50:41.000000 owntools-1.3/owntools/Subtitles.py
+-rw-rw-rw-   0        0        0     2081 2023-02-15 06:12:42.000000 owntools-1.3/owntools/Time.py
+-rw-rw-rw-   0        0        0     4565 2022-01-12 06:36:41.000000 owntools-1.3/owntools/Translation.py
+-rw-rw-rw-   0        0        0      396 2021-12-27 06:01:33.000000 owntools-1.3/owntools/UncompressRAR.py
+-rw-rw-rw-   0        0        0     2343 2023-02-09 00:55:34.000000 owntools-1.3/owntools/_SSH.py
+-rw-rw-rw-   0        0        0      400 2024-05-06 03:05:40.000000 owntools-1.3/owntools/__init__.py
+-rw-rw-rw-   0        0        0     2839 2022-08-25 00:51:34.000000 owntools-1.3/owntools/ownEmail.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:05:02.361919 owntools-1.3/owntools.egg-info/
+-rw-rw-rw-   0        0        0      362 2024-05-06 06:05:02.000000 owntools-1.3/owntools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2024-05-06 06:05:02.000000 owntools-1.3/owntools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 06:05:02.000000 owntools-1.3/owntools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-06 06:05:02.000000 owntools-1.3/owntools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 06:05:02.365914 owntools-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      534 2024-05-06 06:04:56.000000 owntools-1.3/setup.py
```

### Comparing `owntools-1.2/setup.py` & `owntools-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 print(find_packages())
 
 setup(
     name='owntools',
-    version='1.2',
+    version='1.3',
     packages=find_packages(),
     description='Tools for myself',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Neely',
     author_email='liangxiuyu@outlook.com',
     url='https://github.com/liangxiuyu/owntools',
```

### Comparing `owntools-1.2/src/Common.py` & `owntools-1.3/owntools/Common.py`

 * *Files identical despite different names*

### Comparing `owntools-1.2/src/CrackCode.py` & `owntools-1.3/owntools/CrackCode.py`

 * *Files identical despite different names*

### Comparing `owntools-1.2/src/Download.py` & `owntools-1.3/owntools/Download.py`

 * *Files identical despite different names*

### Comparing `owntools-1.2/src/ExtractFile.py` & `owntools-1.3/owntools/ExtractFile.py`

 * *Files identical despite different names*

### Comparing `owntools-1.2/src/Image.py` & `owntools-1.3/owntools/Image.py`

 * *Files identical despite different names*

### Comparing `owntools-1.2/src/Loger.py` & `owntools-1.3/owntools/Loger.py`

 * *Files identical despite different names*

### Comparing `owntools-1.2/src/Mysql.py` & `owntools-1.3/owntools/Mysql.py`

 * *Files identical despite different names*

### Comparing `owntools-1.2/src/Subtitles.py` & `owntools-1.3/owntools/Subtitles.py`

 * *Files identical despite different names*

### Comparing `owntools-1.2/src/Time.py` & `owntools-1.3/owntools/Time.py`

 * *Files identical despite different names*

### Comparing `owntools-1.2/src/Translation.py` & `owntools-1.3/owntools/Translation.py`

 * *Files identical despite different names*

### Comparing `owntools-1.2/src/_SSH.py` & `owntools-1.3/owntools/_SSH.py`

 * *Files identical despite different names*

### Comparing `owntools-1.2/src/ownEmail.py` & `owntools-1.3/owntools/ownEmail.py`

 * *Files identical despite different names*

