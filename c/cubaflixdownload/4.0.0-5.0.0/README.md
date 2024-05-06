# Comparing `tmp/cubaflixdownload-4.0.0.tar.gz` & `tmp/cubaflixdownload-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubaflixdownload-4.0.0.tar", last modified: Sun May  5 23:17:12 2024, max compression
+gzip compressed data, was "cubaflixdownload-5.0.0.tar", last modified: Sun May  5 23:37:48 2024, max compression
```

## Comparing `cubaflixdownload-4.0.0.tar` & `cubaflixdownload-5.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 23:17:12.104569 cubaflixdownload-4.0.0/
--rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 cubaflixdownload-4.0.0/LICENSE
--rw-rw-rw-   0        0        0     1001 2024-05-05 23:17:12.099569 cubaflixdownload-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 cubaflixdownload-4.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 23:17:12.024568 cubaflixdownload-4.0.0/cubaflixdownload/
--rw-rw-rw-   0        0        0      931 2024-03-26 07:28:02.000000 cubaflixdownload-4.0.0/cubaflixdownload/__init__.py
--rw-rw-rw-   0        0        0       75 2024-05-05 23:16:51.000000 cubaflixdownload-4.0.0/cubaflixdownload/version.py
-drwxrwxrwx   0        0        0        0 2024-05-05 23:17:12.092069 cubaflixdownload-4.0.0/cubaflixdownload.egg-info/
--rw-rw-rw-   0        0        0     1001 2024-05-05 23:17:08.000000 cubaflixdownload-4.0.0/cubaflixdownload.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-05-05 23:17:10.000000 cubaflixdownload-4.0.0/cubaflixdownload.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 23:17:08.000000 cubaflixdownload-4.0.0/cubaflixdownload.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-05 23:17:08.000000 cubaflixdownload-4.0.0/cubaflixdownload.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-05 23:17:08.000000 cubaflixdownload-4.0.0/cubaflixdownload.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-05-05 23:17:08.000000 cubaflixdownload-4.0.0/cubaflixdownload.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-05 23:17:12.108070 cubaflixdownload-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1632 2024-03-26 07:30:21.000000 cubaflixdownload-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 23:37:48.588710 cubaflixdownload-5.0.0/
+-rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 cubaflixdownload-5.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1001 2024-05-05 23:37:48.583710 cubaflixdownload-5.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 cubaflixdownload-5.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 23:37:48.479704 cubaflixdownload-5.0.0/cubaflixdownload/
+-rw-rw-rw-   0        0        0      931 2024-03-26 07:28:02.000000 cubaflixdownload-5.0.0/cubaflixdownload/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-05-05 23:37:19.000000 cubaflixdownload-5.0.0/cubaflixdownload/version.py
+drwxrwxrwx   0        0        0        0 2024-05-05 23:37:48.544708 cubaflixdownload-5.0.0/cubaflixdownload.egg-info/
+-rw-rw-rw-   0        0        0     1001 2024-05-05 23:37:47.000000 cubaflixdownload-5.0.0/cubaflixdownload.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-05-05 23:37:47.000000 cubaflixdownload-5.0.0/cubaflixdownload.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 23:37:47.000000 cubaflixdownload-5.0.0/cubaflixdownload.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-05 23:37:47.000000 cubaflixdownload-5.0.0/cubaflixdownload.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-05 23:37:47.000000 cubaflixdownload-5.0.0/cubaflixdownload.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-05-05 23:37:47.000000 cubaflixdownload-5.0.0/cubaflixdownload.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-05 23:37:48.589711 cubaflixdownload-5.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1632 2024-03-26 07:30:21.000000 cubaflixdownload-5.0.0/setup.py
```

### Comparing `cubaflixdownload-4.0.0/LICENSE` & `cubaflixdownload-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cubaflixdownload-4.0.0/PKG-INFO` & `cubaflixdownload-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubaflixdownload
-Version: 4.0.0
+Version: 5.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/shorturl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cubaflixdownload-4.0.0/README.md` & `cubaflixdownload-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cubaflixdownload-4.0.0/cubaflixdownload/__init__.py` & `cubaflixdownload-5.0.0/cubaflixdownload/__init__.py`

 * *Files identical despite different names*

### Comparing `cubaflixdownload-4.0.0/cubaflixdownload.egg-info/PKG-INFO` & `cubaflixdownload-5.0.0/cubaflixdownload.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubaflixdownload
-Version: 4.0.0
+Version: 5.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/shorturl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cubaflixdownload-4.0.0/setup.py` & `cubaflixdownload-5.0.0/setup.py`

 * *Files identical despite different names*

