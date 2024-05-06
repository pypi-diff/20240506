# Comparing `tmp/multiconnection-2.34.14.tar.gz` & `tmp/multiconnection-2.34.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiconnection-2.34.14.tar", last modified: Mon May  6 02:12:53 2024, max compression
+gzip compressed data, was "multiconnection-2.34.16.tar", last modified: Mon May  6 03:25:05 2024, max compression
```

## Comparing `multiconnection-2.34.14.tar` & `multiconnection-2.34.16.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 02:12:53.116432 multiconnection-2.34.14/
--rw-rw-rw-   0        0        0     3112 2024-05-06 02:12:53.115423 multiconnection-2.34.14/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2024-05-04 04:53:14.000000 multiconnection-2.34.14/README.md
--rw-rw-rw-   0        0        0       42 2024-05-06 02:12:53.116432 multiconnection-2.34.14/setup.cfg
--rw-rw-rw-   0        0        0      985 2024-05-06 02:12:40.000000 multiconnection-2.34.14/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 02:12:53.084002 multiconnection-2.34.14/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 02:12:53.111436 multiconnection-2.34.14/src/multiconnection.egg-info/
--rw-rw-rw-   0        0        0     3112 2024-05-06 02:12:51.000000 multiconnection-2.34.14/src/multiconnection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-06 02:12:52.000000 multiconnection-2.34.14/src/multiconnection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 02:12:51.000000 multiconnection-2.34.14/src/multiconnection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-06 02:12:51.000000 multiconnection-2.34.14/src/multiconnection.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 02:12:53.110414 multiconnection-2.34.14/src/roblox_api_wrapper/
--rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiconnection-2.34.14/src/roblox_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiconnection-2.34.14/src/roblox_api_wrapper/getuserinfo.py
--rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiconnection-2.34.14/src/roblox_api_wrapper/login.py
--rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiconnection-2.34.14/src/roblox_api_wrapper/message.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:25:05.727091 multiconnection-2.34.16/
+-rw-rw-rw-   0        0        0     3112 2024-05-06 03:25:05.727091 multiconnection-2.34.16/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-05-04 04:53:14.000000 multiconnection-2.34.16/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 03:25:05.727091 multiconnection-2.34.16/setup.cfg
+-rw-rw-rw-   0        0        0     5279 2024-05-06 03:24:55.000000 multiconnection-2.34.16/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:25:05.711166 multiconnection-2.34.16/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 03:25:05.727091 multiconnection-2.34.16/src/multiconnection.egg-info/
+-rw-rw-rw-   0        0        0     3112 2024-05-06 03:25:05.000000 multiconnection-2.34.16/src/multiconnection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-06 03:25:05.000000 multiconnection-2.34.16/src/multiconnection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 03:25:05.000000 multiconnection-2.34.16/src/multiconnection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-06 03:25:05.000000 multiconnection-2.34.16/src/multiconnection.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 03:25:05.727091 multiconnection-2.34.16/src/roblox_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2024-04-24 22:03:09.000000 multiconnection-2.34.16/src/roblox_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0      119 2024-04-24 22:03:09.000000 multiconnection-2.34.16/src/roblox_api_wrapper/getuserinfo.py
+-rw-rw-rw-   0        0        0      145 2024-04-24 22:03:09.000000 multiconnection-2.34.16/src/roblox_api_wrapper/login.py
+-rw-rw-rw-   0        0        0      107 2024-04-24 22:03:09.000000 multiconnection-2.34.16/src/roblox_api_wrapper/message.py
```

### Comparing `multiconnection-2.34.14/PKG-INFO` & `multiconnection-2.34.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiconnection
-Version: 2.34.14
+Version: 2.34.16
 Summary: Python MultiHTTP for Humans.
 Author: multiconnection
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `multiconnection-2.34.14/README.md` & `multiconnection-2.34.16/README.md`

 * *Files identical despite different names*

### Comparing `multiconnection-2.34.14/src/multiconnection.egg-info/PKG-INFO` & `multiconnection-2.34.16/src/multiconnection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiconnection
-Version: 2.34.14
+Version: 2.34.16
 Summary: Python MultiHTTP for Humans.
 Author: multiconnection
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

