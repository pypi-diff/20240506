# Comparing `tmp/wapi-python-0.7.9.tar.gz` & `tmp/wapi-python-0.7.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wapi-python-0.7.9.tar", last modified: Wed Nov 23 09:41:15 2022, max compression
+gzip compressed data, was "wapi-python-0.7.9rc1.tar", last modified: Fri Nov 18 07:48:01 2022, max compression
```

## Comparing `wapi-python-0.7.9.tar` & `wapi-python-0.7.9rc1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0     1000 root         (0)        0 2022-11-23 09:41:15.666706 wapi-python-0.7.9/
--rw-r--r--   0     1000 root         (0)     1069 2022-11-23 09:41:05.000000 wapi-python-0.7.9/LICENSE
--rw-r--r--   0     1000 root         (0)       34 2022-11-23 09:41:05.000000 wapi-python-0.7.9/MANIFEST.in
--rw-r--r--   0     1000 root         (0)      528 2022-11-23 09:41:15.666706 wapi-python-0.7.9/PKG-INFO
--rw-r--r--   0     1000 root         (0)     1933 2022-11-23 09:41:05.000000 wapi-python-0.7.9/README.md
--rw-r--r--   0     1000 root         (0)        6 2022-11-23 09:41:05.000000 wapi-python-0.7.9/VERSION
--rw-r--r--   0     1000 root         (0)      128 2022-11-23 09:41:15.666706 wapi-python-0.7.9/setup.cfg
--rw-r--r--   0     1000 root         (0)     1123 2022-11-23 09:41:05.000000 wapi-python-0.7.9/setup.py
-drwxr-xr-x   0     1000 root         (0)        0 2022-11-23 09:41:15.665706 wapi-python-0.7.9/wapi/
--rw-r--r--   0     1000 root         (0)      148 2022-11-23 09:41:05.000000 wapi-python-0.7.9/wapi/__init__.py
--rw-r--r--   0     1000 root         (0)     2117 2022-11-23 09:41:05.000000 wapi-python-0.7.9/wapi/auth.py
--rw-r--r--   0     1000 root         (0)    64230 2022-11-23 09:41:05.000000 wapi-python-0.7.9/wapi/curves.py
--rw-r--r--   0     1000 root         (0)     4194 2022-11-23 09:41:05.000000 wapi-python-0.7.9/wapi/events.py
--rw-r--r--   0     1000 root         (0)    19615 2022-11-23 09:41:05.000000 wapi-python-0.7.9/wapi/session.py
--rw-r--r--   0     1000 root         (0)     9064 2022-11-23 09:41:05.000000 wapi-python-0.7.9/wapi/util.py
-drwxr-xr-x   0     1000 root         (0)        0 2022-11-23 09:41:15.665706 wapi-python-0.7.9/wapi_python.egg-info/
--rw-r--r--   0     1000 root         (0)      528 2022-11-23 09:41:15.000000 wapi-python-0.7.9/wapi_python.egg-info/PKG-INFO
--rw-r--r--   0     1000 root         (0)      319 2022-11-23 09:41:15.000000 wapi-python-0.7.9/wapi_python.egg-info/SOURCES.txt
--rw-r--r--   0     1000 root         (0)        1 2022-11-23 09:41:15.000000 wapi-python-0.7.9/wapi_python.egg-info/dependency_links.txt
--rw-r--r--   0     1000 root         (0)       64 2022-11-23 09:41:15.000000 wapi-python-0.7.9/wapi_python.egg-info/requires.txt
--rw-r--r--   0     1000 root         (0)        5 2022-11-23 09:41:15.000000 wapi-python-0.7.9/wapi_python.egg-info/top_level.txt
+drwxr-xr-x   0     1000 root         (0)        0 2022-11-18 07:48:01.246145 wapi-python-0.7.9rc1/
+-rw-r--r--   0     1000 root         (0)     1069 2022-11-18 07:47:36.000000 wapi-python-0.7.9rc1/LICENSE
+-rw-r--r--   0     1000 root         (0)       34 2022-11-18 07:47:36.000000 wapi-python-0.7.9rc1/MANIFEST.in
+-rw-r--r--   0     1000 root         (0)      531 2022-11-18 07:48:01.246145 wapi-python-0.7.9rc1/PKG-INFO
+-rw-r--r--   0     1000 root         (0)     1933 2022-11-18 07:47:36.000000 wapi-python-0.7.9rc1/README.md
+-rw-r--r--   0     1000 root         (0)        9 2022-11-18 07:47:36.000000 wapi-python-0.7.9rc1/VERSION
+-rw-r--r--   0     1000 root         (0)      128 2022-11-18 07:48:01.247145 wapi-python-0.7.9rc1/setup.cfg
+-rw-r--r--   0     1000 root         (0)     1123 2022-11-18 07:47:36.000000 wapi-python-0.7.9rc1/setup.py
+drwxr-xr-x   0     1000 root         (0)        0 2022-11-18 07:48:01.244145 wapi-python-0.7.9rc1/wapi/
+-rw-r--r--   0     1000 root         (0)      151 2022-11-18 07:47:36.000000 wapi-python-0.7.9rc1/wapi/__init__.py
+-rw-r--r--   0     1000 root         (0)     2117 2022-11-18 07:47:36.000000 wapi-python-0.7.9rc1/wapi/auth.py
+-rw-r--r--   0     1000 root         (0)    64230 2022-11-18 07:47:36.000000 wapi-python-0.7.9rc1/wapi/curves.py
+-rw-r--r--   0     1000 root         (0)     4194 2022-11-18 07:47:36.000000 wapi-python-0.7.9rc1/wapi/events.py
+-rw-r--r--   0     1000 root         (0)    19615 2022-11-18 07:47:36.000000 wapi-python-0.7.9rc1/wapi/session.py
+-rw-r--r--   0     1000 root         (0)     9064 2022-11-18 07:47:36.000000 wapi-python-0.7.9rc1/wapi/util.py
+drwxr-xr-x   0     1000 root         (0)        0 2022-11-18 07:48:01.246145 wapi-python-0.7.9rc1/wapi_python.egg-info/
+-rw-r--r--   0     1000 root         (0)      531 2022-11-18 07:48:01.000000 wapi-python-0.7.9rc1/wapi_python.egg-info/PKG-INFO
+-rw-r--r--   0     1000 root         (0)      319 2022-11-18 07:48:01.000000 wapi-python-0.7.9rc1/wapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0     1000 root         (0)        1 2022-11-18 07:48:01.000000 wapi-python-0.7.9rc1/wapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0     1000 root         (0)       64 2022-11-18 07:48:01.000000 wapi-python-0.7.9rc1/wapi_python.egg-info/requires.txt
+-rw-r--r--   0     1000 root         (0)        5 2022-11-18 07:48:01.000000 wapi-python-0.7.9rc1/wapi_python.egg-info/top_level.txt
```

### Comparing `wapi-python-0.7.9/LICENSE` & `wapi-python-0.7.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `wapi-python-0.7.9/PKG-INFO` & `wapi-python-0.7.9rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wapi-python
-Version: 0.7.9
+Version: 0.7.9rc1
 Summary: Volue Insight API python library
 Home-page: https://www.volueinsight.com
 Author: Volue Insight
 Author-email: support.insight@volue.com
 License: UNKNOWN
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `wapi-python-0.7.9/README.md` & `wapi-python-0.7.9rc1/README.md`

 * *Files identical despite different names*

### Comparing `wapi-python-0.7.9/setup.py` & `wapi-python-0.7.9rc1/setup.py`

 * *Files identical despite different names*

### Comparing `wapi-python-0.7.9/wapi/auth.py` & `wapi-python-0.7.9rc1/wapi/auth.py`

 * *Files identical despite different names*

### Comparing `wapi-python-0.7.9/wapi/curves.py` & `wapi-python-0.7.9rc1/wapi/curves.py`

 * *Files identical despite different names*

### Comparing `wapi-python-0.7.9/wapi/events.py` & `wapi-python-0.7.9rc1/wapi/events.py`

 * *Files identical despite different names*

### Comparing `wapi-python-0.7.9/wapi/session.py` & `wapi-python-0.7.9rc1/wapi/session.py`

 * *Files identical despite different names*

### Comparing `wapi-python-0.7.9/wapi/util.py` & `wapi-python-0.7.9rc1/wapi/util.py`

 * *Files identical despite different names*

### Comparing `wapi-python-0.7.9/wapi_python.egg-info/PKG-INFO` & `wapi-python-0.7.9rc1/wapi_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wapi-python
-Version: 0.7.9
+Version: 0.7.9rc1
 Summary: Volue Insight API python library
 Home-page: https://www.volueinsight.com
 Author: Volue Insight
 Author-email: support.insight@volue.com
 License: UNKNOWN
 Platform: UNKNOWN
 License-File: LICENSE
```

