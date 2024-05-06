# Comparing `tmp/stac_fastapi_core-2.4.0.tar.gz` & `tmp/stac_fastapi_core-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_core-2.4.0.tar", last modified: Sat May  4 10:25:38 2024, max compression
+gzip compressed data, was "stac_fastapi_core-2.4.1.tar", last modified: Mon May  6 16:10:14 2024, max compression
```

## Comparing `stac_fastapi_core-2.4.0.tar` & `stac_fastapi_core-2.4.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 10:25:38.751006 stac_fastapi_core-2.4.0/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1217 2024-05-04 10:25:38.743872 stac_fastapi_core-2.4.0/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)       69 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.0/README.md
--rw-r--r--   0 primeradiant   (501) staff       (20)      104 2024-05-04 10:25:38.752420 stac_fastapi_core-2.4.0/setup.cfg
--rw-r--r--   0 primeradiant   (501) staff       (20)     1385 2024-05-04 09:54:48.000000 stac_fastapi_core-2.4.0/setup.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 10:25:38.576113 stac_fastapi_core-2.4.0/stac_fastapi/
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 10:25:38.716142 stac_fastapi_core-2.4.0/stac_fastapi/core/
--rw-r--r--   0 primeradiant   (501) staff       (20)       20 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.0/stac_fastapi/core/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     1608 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.0/stac_fastapi/core/base_database_logic.py
--rw-r--r--   0 primeradiant   (501) staff       (20)      239 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.0/stac_fastapi/core/base_settings.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     3826 2024-05-02 09:57:35.000000 stac_fastapi_core-2.4.0/stac_fastapi/core/basic_auth.py
--rw-r--r--   0 primeradiant   (501) staff       (20)    35978 2024-05-02 09:57:35.000000 stac_fastapi_core-2.4.0/stac_fastapi/core/core.py
--rw-r--r--   0 primeradiant   (501) staff       (20)      384 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.0/stac_fastapi/core/datetime_utils.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 10:25:38.722440 stac_fastapi_core-2.4.0/stac_fastapi/core/extensions/
--rw-r--r--   0 primeradiant   (501) staff       (20)      167 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.0/stac_fastapi/core/extensions/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     7464 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.0/stac_fastapi/core/extensions/filter.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     1892 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.0/stac_fastapi/core/extensions/query.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 10:25:38.733390 stac_fastapi_core-2.4.0/stac_fastapi/core/models/
--rw-r--r--   0 primeradiant   (501) staff       (20)       48 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.0/stac_fastapi/core/models/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     4470 2024-03-19 04:19:17.000000 stac_fastapi_core-2.4.0/stac_fastapi/core/models/links.py
--rw-r--r--   0 primeradiant   (501) staff       (20)       27 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.0/stac_fastapi/core/models/search.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     5892 2024-03-19 04:19:17.000000 stac_fastapi_core-2.4.0/stac_fastapi/core/serializers.py
--rw-r--r--   0 primeradiant   (501) staff       (20)      473 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.0/stac_fastapi/core/session.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 10:25:38.737304 stac_fastapi_core-2.4.0/stac_fastapi/core/types/
--rw-r--r--   0 primeradiant   (501) staff       (20)     9155 2024-04-24 05:29:38.000000 stac_fastapi_core-2.4.0/stac_fastapi/core/types/core.py
--rw-r--r--   0 primeradiant   (501) staff       (20)      933 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.0/stac_fastapi/core/utilities.py
--rw-r--r--   0 primeradiant   (501) staff       (20)       45 2024-05-04 10:23:33.000000 stac_fastapi_core-2.4.0/stac_fastapi/core/version.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-04 10:25:38.742946 stac_fastapi_core-2.4.0/stac_fastapi.core.egg-info/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1217 2024-05-04 10:25:38.000000 stac_fastapi_core-2.4.0/stac_fastapi.core.egg-info/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)      850 2024-05-04 10:25:38.000000 stac_fastapi_core-2.4.0/stac_fastapi.core.egg-info/SOURCES.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-05-04 10:25:38.000000 stac_fastapi_core-2.4.0/stac_fastapi.core.egg-info/dependency_links.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-01-31 08:38:37.000000 stac_fastapi_core-2.4.0/stac_fastapi.core.egg-info/not-zip-safe
--rw-r--r--   0 primeradiant   (501) staff       (20)      250 2024-05-04 10:25:38.000000 stac_fastapi_core-2.4.0/stac_fastapi.core.egg-info/requires.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-05-04 10:25:38.000000 stac_fastapi_core-2.4.0/stac_fastapi.core.egg-info/top_level.txt
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:10:14.103391 stac_fastapi_core-2.4.1/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1217 2024-05-06 16:10:14.103011 stac_fastapi_core-2.4.1/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)       69 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/README.md
+-rw-r--r--   0 primeradiant   (501) staff       (20)      104 2024-05-06 16:10:14.106200 stac_fastapi_core-2.4.1/setup.cfg
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1385 2024-05-04 09:54:48.000000 stac_fastapi_core-2.4.1/setup.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:10:13.985082 stac_fastapi_core-2.4.1/stac_fastapi/
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:10:14.053169 stac_fastapi_core-2.4.1/stac_fastapi/core/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       20 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1608 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/base_database_logic.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)      239 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/base_settings.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     3826 2024-05-02 09:57:35.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/basic_auth.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)    35886 2024-05-06 15:51:07.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/core.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)      384 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/datetime_utils.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:10:14.064436 stac_fastapi_core-2.4.1/stac_fastapi/core/extensions/
+-rw-r--r--   0 primeradiant   (501) staff       (20)      167 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/extensions/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     7464 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/extensions/filter.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1892 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/extensions/query.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:10:14.083999 stac_fastapi_core-2.4.1/stac_fastapi/core/models/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       48 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/models/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     4470 2024-03-19 04:19:17.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/models/links.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)       27 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/models/search.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     5892 2024-03-19 04:19:17.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/serializers.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)      473 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/session.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:10:14.092935 stac_fastapi_core-2.4.1/stac_fastapi/core/types/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     9155 2024-04-24 05:29:38.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/types/core.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)      933 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/utilities.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)       45 2024-05-06 15:56:07.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/version.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:10:14.101586 stac_fastapi_core-2.4.1/stac_fastapi.core.egg-info/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1217 2024-05-06 16:10:13.000000 stac_fastapi_core-2.4.1/stac_fastapi.core.egg-info/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)      850 2024-05-06 16:10:13.000000 stac_fastapi_core-2.4.1/stac_fastapi.core.egg-info/SOURCES.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-05-06 16:10:13.000000 stac_fastapi_core-2.4.1/stac_fastapi.core.egg-info/dependency_links.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-01-31 08:38:37.000000 stac_fastapi_core-2.4.1/stac_fastapi.core.egg-info/not-zip-safe
+-rw-r--r--   0 primeradiant   (501) staff       (20)      250 2024-05-06 16:10:13.000000 stac_fastapi_core-2.4.1/stac_fastapi.core.egg-info/requires.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-05-06 16:10:13.000000 stac_fastapi_core-2.4.1/stac_fastapi.core.egg-info/top_level.txt
```

### Comparing `stac_fastapi_core-2.4.0/PKG-INFO` & `stac_fastapi_core-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.core
-Version: 2.4.0
+Version: 2.4.1
 Summary: Core library for the Elasticsearch and Opensearch stac-fastapi backends.
 Home-page: https://github.com/stac-utils/stac-fastapi-elasticsearch-opensearch
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `stac_fastapi_core-2.4.0/setup.py` & `stac_fastapi_core-2.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.4.0/stac_fastapi/core/base_database_logic.py` & `stac_fastapi_core-2.4.1/stac_fastapi/core/base_database_logic.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.4.0/stac_fastapi/core/basic_auth.py` & `stac_fastapi_core-2.4.1/stac_fastapi/core/basic_auth.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.4.0/stac_fastapi/core/core.py` & `stac_fastapi_core-2.4.1/stac_fastapi/core/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,17 +314,15 @@
             context_obj = {
                 "returned": len(items),
                 "limit": limit,
             }
             if maybe_count is not None:
                 context_obj["matched"] = maybe_count
 
-        links = []
-        if next_token:
-            links = await PagingLinks(request=request, next=next_token).get_links()
+        links = await PagingLinks(request=request, next=next_token).get_links()
 
         return ItemCollection(
             type="FeatureCollection",
             features=items,
             links=links,
             context=context_obj,
         )
@@ -615,17 +613,15 @@
             context_obj = {
                 "returned": len(items),
                 "limit": limit,
             }
             if maybe_count is not None:
                 context_obj["matched"] = maybe_count
 
-        links = []
-        if next_token:
-            links = await PagingLinks(request=request, next=next_token).get_links()
+        links = await PagingLinks(request=request, next=next_token).get_links()
 
         return ItemCollection(
             type="FeatureCollection",
             features=items,
             links=links,
             context=context_obj,
         )
```

### Comparing `stac_fastapi_core-2.4.0/stac_fastapi/core/extensions/filter.py` & `stac_fastapi_core-2.4.1/stac_fastapi/core/extensions/filter.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.4.0/stac_fastapi/core/extensions/query.py` & `stac_fastapi_core-2.4.1/stac_fastapi/core/extensions/query.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.4.0/stac_fastapi/core/models/links.py` & `stac_fastapi_core-2.4.1/stac_fastapi/core/models/links.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.4.0/stac_fastapi/core/serializers.py` & `stac_fastapi_core-2.4.1/stac_fastapi/core/serializers.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.4.0/stac_fastapi/core/types/core.py` & `stac_fastapi_core-2.4.1/stac_fastapi/core/types/core.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.4.0/stac_fastapi/core/utilities.py` & `stac_fastapi_core-2.4.1/stac_fastapi/core/utilities.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.4.0/stac_fastapi.core.egg-info/PKG-INFO` & `stac_fastapi_core-2.4.1/stac_fastapi.core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.core
-Version: 2.4.0
+Version: 2.4.1
 Summary: Core library for the Elasticsearch and Opensearch stac-fastapi backends.
 Home-page: https://github.com/stac-utils/stac-fastapi-elasticsearch-opensearch
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `stac_fastapi_core-2.4.0/stac_fastapi.core.egg-info/SOURCES.txt` & `stac_fastapi_core-2.4.1/stac_fastapi.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

