# Comparing `tmp/cubaflixdownload-2.0.0.tar.gz` & `tmp/cubaflixdownload-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubaflixdownload-2.0.0.tar", last modified: Sat Apr  6 03:28:03 2024, max compression
+gzip compressed data, was "cubaflixdownload-3.0.0.tar", last modified: Sun May  5 22:27:14 2024, max compression
```

## Comparing `cubaflixdownload-2.0.0.tar` & `cubaflixdownload-3.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 03:28:03.866416 cubaflixdownload-2.0.0/
--rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 cubaflixdownload-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     1001 2024-04-06 03:28:03.863416 cubaflixdownload-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 cubaflixdownload-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 03:28:03.809413 cubaflixdownload-2.0.0/cubaflixdownload/
--rw-rw-rw-   0        0        0      931 2024-03-26 07:28:02.000000 cubaflixdownload-2.0.0/cubaflixdownload/__init__.py
--rw-rw-rw-   0        0        0       75 2024-04-06 03:27:44.000000 cubaflixdownload-2.0.0/cubaflixdownload/version.py
-drwxrwxrwx   0        0        0        0 2024-04-06 03:28:03.857416 cubaflixdownload-2.0.0/cubaflixdownload.egg-info/
--rw-rw-rw-   0        0        0     1001 2024-04-06 03:28:02.000000 cubaflixdownload-2.0.0/cubaflixdownload.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-04-06 03:28:02.000000 cubaflixdownload-2.0.0/cubaflixdownload.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 03:28:02.000000 cubaflixdownload-2.0.0/cubaflixdownload.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-06 03:28:02.000000 cubaflixdownload-2.0.0/cubaflixdownload.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-06 03:28:02.000000 cubaflixdownload-2.0.0/cubaflixdownload.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-06 03:28:02.000000 cubaflixdownload-2.0.0/cubaflixdownload.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-04-06 03:28:03.868416 cubaflixdownload-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1632 2024-03-26 07:30:21.000000 cubaflixdownload-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:27:14.884387 cubaflixdownload-3.0.0/
+-rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 cubaflixdownload-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1001 2024-05-05 22:27:14.861386 cubaflixdownload-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 cubaflixdownload-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 22:27:14.729378 cubaflixdownload-3.0.0/cubaflixdownload/
+-rw-rw-rw-   0        0        0      931 2024-03-26 07:28:02.000000 cubaflixdownload-3.0.0/cubaflixdownload/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-05-05 22:26:58.000000 cubaflixdownload-3.0.0/cubaflixdownload/version.py
+drwxrwxrwx   0        0        0        0 2024-05-05 22:27:14.816383 cubaflixdownload-3.0.0/cubaflixdownload.egg-info/
+-rw-rw-rw-   0        0        0     1001 2024-05-05 22:27:13.000000 cubaflixdownload-3.0.0/cubaflixdownload.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-05-05 22:27:14.000000 cubaflixdownload-3.0.0/cubaflixdownload.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 22:27:13.000000 cubaflixdownload-3.0.0/cubaflixdownload.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-05 22:27:13.000000 cubaflixdownload-3.0.0/cubaflixdownload.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-05 22:27:13.000000 cubaflixdownload-3.0.0/cubaflixdownload.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-05-05 22:27:13.000000 cubaflixdownload-3.0.0/cubaflixdownload.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-05 22:27:14.885387 cubaflixdownload-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1632 2024-03-26 07:30:21.000000 cubaflixdownload-3.0.0/setup.py
```

### Comparing `cubaflixdownload-2.0.0/LICENSE` & `cubaflixdownload-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cubaflixdownload-2.0.0/PKG-INFO` & `cubaflixdownload-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubaflixdownload
-Version: 2.0.0
+Version: 3.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/shorturl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cubaflixdownload-2.0.0/README.md` & `cubaflixdownload-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cubaflixdownload-2.0.0/cubaflixdownload/__init__.py` & `cubaflixdownload-3.0.0/cubaflixdownload/__init__.py`

 * *Files identical despite different names*

### Comparing `cubaflixdownload-2.0.0/cubaflixdownload.egg-info/PKG-INFO` & `cubaflixdownload-3.0.0/cubaflixdownload.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubaflixdownload
-Version: 2.0.0
+Version: 3.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/shorturl
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cubaflixdownload-2.0.0/setup.py` & `cubaflixdownload-3.0.0/setup.py`

 * *Files identical despite different names*

