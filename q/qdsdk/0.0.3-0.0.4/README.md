# Comparing `tmp/qdsdk-0.0.3.tar.gz` & `tmp/qdsdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdsdk-0.0.3.tar", last modified: Fri Apr 26 02:53:07 2024, max compression
+gzip compressed data, was "qdsdk-0.0.4.tar", last modified: Mon May  6 05:35:47 2024, max compression
```

## Comparing `qdsdk-0.0.3.tar` & `qdsdk-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 02:53:07.664959 qdsdk-0.0.3/
--rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qdsdk-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       38 2024-04-26 02:46:25.000000 qdsdk-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6161 2024-04-26 02:53:07.662958 qdsdk-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4356 2024-03-18 09:51:27.000000 qdsdk-0.0.3/README.md
--rw-rw-rw-   0        0        0      753 2024-04-26 02:52:54.000000 qdsdk-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-26 02:53:07.664959 qdsdk-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-26 02:53:07.625236 qdsdk-0.0.3/src/
--rw-rw-rw-   0        0        0        0 2024-04-26 02:45:44.000000 qdsdk-0.0.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-26 02:53:07.642966 qdsdk-0.0.3/src/qdsdk/
--rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qdsdk-0.0.3/src/qdsdk/__init__.py
--rw-rw-rw-   0        0        0     4498 2024-04-26 02:52:22.000000 qdsdk-0.0.3/src/qdsdk/aio_api.py
--rw-rw-rw-   0        0        0    31189 2024-04-26 02:28:08.000000 qdsdk-0.0.3/src/qdsdk/api.py
--rw-rw-rw-   0        0        0     8348 2024-04-26 02:26:49.000000 qdsdk-0.0.3/src/qdsdk/client.py
--rw-rw-rw-   0        0        0      170 2024-04-25 06:56:16.000000 qdsdk-0.0.3/src/qdsdk/config.py
--rw-rw-rw-   0        0        0      599 2022-10-09 06:46:09.000000 qdsdk-0.0.3/src/qdsdk/qedata.thrift
--rw-rw-rw-   0        0        0      675 2024-04-26 02:40:38.000000 qdsdk-0.0.3/src/qdsdk/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-26 02:53:07.660957 qdsdk-0.0.3/src/qdsdk.egg-info/
--rw-rw-rw-   0        0        0     6161 2024-04-26 02:53:07.000000 qdsdk-0.0.3/src/qdsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2024-04-26 02:53:07.000000 qdsdk-0.0.3/src/qdsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 02:53:07.000000 qdsdk-0.0.3/src/qdsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-04-26 02:53:07.000000 qdsdk-0.0.3/src/qdsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-26 02:53:07.000000 qdsdk-0.0.3/src/qdsdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 05:35:47.392915 qdsdk-0.0.4/
+-rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qdsdk-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       38 2024-04-26 02:46:25.000000 qdsdk-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6161 2024-05-06 05:35:47.392915 qdsdk-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4356 2024-03-18 09:51:27.000000 qdsdk-0.0.4/README.md
+-rw-rw-rw-   0        0        0      753 2024-05-06 05:32:05.000000 qdsdk-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 05:35:47.392915 qdsdk-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 05:35:47.346014 qdsdk-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 05:35:47.377303 qdsdk-0.0.4/src/qdsdk/
+-rw-rw-rw-   0        0        0      511 2024-04-26 03:23:54.000000 qdsdk-0.0.4/src/qdsdk/__init__.py
+-rw-rw-rw-   0        0        0     4498 2024-04-26 03:24:50.000000 qdsdk-0.0.4/src/qdsdk/aio_api.py
+-rw-rw-rw-   0        0        0    31311 2024-04-30 06:15:29.000000 qdsdk-0.0.4/src/qdsdk/api.py
+-rw-rw-rw-   0        0        0     8348 2024-04-26 02:26:49.000000 qdsdk-0.0.4/src/qdsdk/client.py
+-rw-rw-rw-   0        0        0      170 2024-04-25 06:56:16.000000 qdsdk-0.0.4/src/qdsdk/config.py
+-rw-rw-rw-   0        0        0      599 2022-10-09 06:46:09.000000 qdsdk-0.0.4/src/qdsdk/qedata.thrift
+-rw-rw-rw-   0        0        0      675 2024-04-26 02:40:38.000000 qdsdk-0.0.4/src/qdsdk/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 05:35:47.392915 qdsdk-0.0.4/src/qdsdk.egg-info/
+-rw-rw-rw-   0        0        0     6161 2024-05-06 05:35:47.000000 qdsdk-0.0.4/src/qdsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2024-05-06 05:35:47.000000 qdsdk-0.0.4/src/qdsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 05:35:47.000000 qdsdk-0.0.4/src/qdsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-05-06 05:35:47.000000 qdsdk-0.0.4/src/qdsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-06 05:35:47.000000 qdsdk-0.0.4/src/qdsdk.egg-info/top_level.txt
```

### Comparing `qdsdk-0.0.3/LICENSE` & `qdsdk-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qdsdk-0.0.3/PKG-INFO` & `qdsdk-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdsdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: QuantDo SDK for quants
 Author-email: Fisher Yu <yuzs@quantdo.com.cn>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `qdsdk-0.0.3/README.md` & `qdsdk-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `qdsdk-0.0.3/pyproject.toml` & `qdsdk-0.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qdsdk"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Fisher Yu", email="yuzs@quantdo.com.cn" },
 ]
 description = "QuantDo SDK for quants"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `qdsdk-0.0.3/src/qdsdk/aio_api.py` & `qdsdk-0.0.4/src/qdsdk/aio_api.py`

 * *Files identical despite different names*

### Comparing `qdsdk-0.0.3/src/qdsdk/api.py` & `qdsdk-0.0.4/src/qdsdk/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,14 +166,19 @@
     validTypes = ['all', 'options', 'futures', 'spot']
     if not stype in validTypes:
         print("stype不合法, 合法值如下： [\'all\', \'options\', \'futures\']")
 
         return None
     validExchanges = ['DCE', 'SSE', "SFE", "ZCE", "INE", "CCF", "GFE", "ALL"]
     exID = exchange.upper()
+
+    if len(exID) == 0:
+        print("exchange不可为空, 合法值如下:", validExchanges)
+        return None
+
     if not exID in validExchanges:
         print("exchange不合法, 合法值如下:", validExchanges)
         return None
         #print('dataWindow', dateWindow)
     try:
         if dateWindow:
             if len(dateWindow) == 2:
```

### Comparing `qdsdk-0.0.3/src/qdsdk/client.py` & `qdsdk-0.0.4/src/qdsdk/client.py`

 * *Files identical despite different names*

### Comparing `qdsdk-0.0.3/src/qdsdk/qedata.thrift` & `qdsdk-0.0.4/src/qdsdk/qedata.thrift`

 * *Files identical despite different names*

### Comparing `qdsdk-0.0.3/src/qdsdk/utils.py` & `qdsdk-0.0.4/src/qdsdk/utils.py`

 * *Files identical despite different names*

### Comparing `qdsdk-0.0.3/src/qdsdk.egg-info/PKG-INFO` & `qdsdk-0.0.4/src/qdsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdsdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: QuantDo SDK for quants
 Author-email: Fisher Yu <yuzs@quantdo.com.cn>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

