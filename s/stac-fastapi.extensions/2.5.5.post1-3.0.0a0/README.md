# Comparing `tmp/stac_fastapi_extensions-2.5.5.post1.tar.gz` & `tmp/stac_fastapi_extensions-3.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_extensions-2.5.5.post1.tar", last modified: Thu Apr 25 12:06:23 2024, max compression
+gzip compressed data, was "stac_fastapi_extensions-3.0.0a0.tar", last modified: Mon May  6 16:07:34 2024, max compression
```

## Comparing `stac_fastapi_extensions-2.5.5.post1.tar` & `stac_fastapi_extensions-3.0.0a0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:23.093685 stac_fastapi_extensions-2.5.5.post1/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-25 12:06:23.093685 stac_fastapi_extensions-2.5.5.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-25 12:06:23.093685 stac_fastapi_extensions-2.5.5.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:23.085685 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:23.089685 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:23.089685 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:23.089685 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/fields/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/fields/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/fields/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:23.089685 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/filter/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/filter/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/filter/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:23.089685 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/pagination/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/pagination/token_pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:23.089685 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/query/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/query/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/query/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:23.089685 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/sort/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/sort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/sort/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/sort/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:23.089685 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/third_party/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/third_party/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/third_party/bulk_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:23.093685 stac_fastapi_extensions-2.5.5.post1/stac_fastapi.extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-25 12:06:23.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi.extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-25 12:06:23.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi.extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:06:23.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi.extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:06:23.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi.extensions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-25 12:06:23.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi.extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 12:06:23.000000 stac_fastapi_extensions-2.5.5.post1/stac_fastapi.extensions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:23.093685 stac_fastapi_extensions-2.5.5.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-25 12:06:11.000000 stac_fastapi_extensions-2.5.5.post1/tests/test_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.714635 stac_fastapi_extensions-3.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-06 16:07:34.714635 stac_fastapi_extensions-3.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-06 16:07:34.714635 stac_fastapi_extensions-3.0.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.702635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.706635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.706635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.710635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/fields/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/fields/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.710635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/filter/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/filter/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.710635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/pagination/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/pagination/token_pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.710635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/query/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.710635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/sort/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/sort/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/sort/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.710635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/third_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/third_party/bulk_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.710635 stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-06 16:07:34.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-06 16:07:34.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:07:34.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:07:34.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-06 16:07:34.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 16:07:34.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.710635 stac_fastapi_extensions-3.0.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/tests/test_transaction.py
```

### Comparing `stac_fastapi_extensions-2.5.5.post1/PKG-INFO` & `stac_fastapi_extensions-3.0.0a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.extensions
-Version: 2.5.5.post1
+Version: 3.0.0a0
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
@@ -14,17 +14,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: attrs
-Requires-Dist: pydantic[dotenv]<2
-Requires-Dist: stac_pydantic==2.0.*
 Requires-Dist: stac-fastapi.types
 Requires-Dist: stac-fastapi.api
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
```

### Comparing `stac_fastapi_extensions-2.5.5.post1/setup.py` & `stac_fastapi_extensions-3.0.0a0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """stac_fastapi: extensions module."""
 
+
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
-    "attrs",
-    "pydantic[dotenv]<2",
-    "stac_pydantic==2.0.*",
     "stac-fastapi.types",
     "stac-fastapi.api",
 ]
 
 extra_reqs = {
     "dev": [
         "pytest",
```

### Comparing `stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/__init__.py` & `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """stac_api.extensions.core module."""
+
 from .context import ContextExtension
 from .fields import FieldsExtension
 from .filter import FilterExtension
 from .pagination import PaginationExtension, TokenPaginationExtension
 from .query import QueryExtension
 from .sort import SortExtension
 from .transaction import TransactionExtension
```

### Comparing `stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/context.py` & `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/context.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/fields/fields.py` & `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/fields/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Fields extension."""
+
 from typing import List, Optional, Set
 
 import attr
 from fastapi import FastAPI
 
 from stac_fastapi.types.extension import ApiExtension
```

### Comparing `stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/fields/request.py` & `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/fields/request.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/filter/filter.py` & `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/filter/filter.py`

 * *Files 11% similar despite different names*

```diff
@@ -93,20 +93,34 @@
             None
         """
         self.router.prefix = app.state.router_prefix
         self.router.add_api_route(
             name="Queryables",
             path="/queryables",
             methods=["GET"],
-            endpoint=create_async_endpoint(
-                self.client.get_queryables, EmptyRequest, self.response_class
-            ),
+            responses={
+                200: {
+                    "content": {
+                        "application/schema+json": {},
+                    },
+                    # TODO: add output model in stac-pydantic
+                },
+            },
+            response_class=self.response_class,
+            endpoint=create_async_endpoint(self.client.get_queryables, EmptyRequest),
         )
         self.router.add_api_route(
             name="Collection Queryables",
             path="/collections/{collection_id}/queryables",
             methods=["GET"],
-            endpoint=create_async_endpoint(
-                self.client.get_queryables, CollectionUri, self.response_class
-            ),
+            responses={
+                200: {
+                    "content": {
+                        "application/schema+json": {},
+                    },
+                    # TODO: add output model in stac-pydantic
+                },
+            },
+            response_class=self.response_class,
+            endpoint=create_async_endpoint(self.client.get_queryables, CollectionUri),
         )
         app.include_router(self.router, tags=["Filter Extension"])
```

### Comparing `stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/filter/request.py` & `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/filter/request.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/pagination/pagination.py` & `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/pagination/token_pagination.py` & `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/pagination/token_pagination.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/query/query.py` & `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/query/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Query extension."""
+
 from typing import List, Optional
 
 import attr
 from fastapi import FastAPI
 
 from stac_fastapi.types.extension import ApiExtension
```

### Comparing `stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/sort/request.py` & `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/sort/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 
     sortby: Optional[str] = attr.ib(default=None, converter=str2list)
 
 
 class SortExtensionPostRequest(BaseModel):
     """Sortby parameter for POST requests."""
 
-    sortby: Optional[List[PostSortModel]]
+    sortby: Optional[List[PostSortModel]] = None
```

### Comparing `stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/sort/sort.py` & `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/sort/sort.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Sort extension."""
+
 from typing import List, Optional
 
 import attr
 from fastapi import FastAPI
 
 from stac_fastapi.types.extension import ApiExtension
```

### Comparing `stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/core/transaction.py` & `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/transaction.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 """Transaction extension."""
 
 from typing import List, Optional, Type, Union
 
 import attr
 from fastapi import APIRouter, Body, FastAPI
-from stac_pydantic import Collection, Item
+from stac_pydantic import Collection, Item, ItemCollection
+from stac_pydantic.shared import MimeTypes
 from starlette.responses import JSONResponse, Response
 
 from stac_fastapi.api.models import CollectionUri, ItemUri
 from stac_fastapi.api.routes import create_async_endpoint
-from stac_fastapi.types import stac as stac_types
 from stac_fastapi.types.config import ApiSettings
 from stac_fastapi.types.core import AsyncBaseTransactionsClient, BaseTransactionsClient
 from stac_fastapi.types.extension import ApiExtension
 
 
 @attr.s
 class PostItem(CollectionUri):
     """Create Item."""
 
-    item: Union[stac_types.Item, stac_types.ItemCollection] = attr.ib(
-        default=Body(None)
-    )
+    item: Union[Item, ItemCollection] = attr.ib(default=Body(None))
 
 
 @attr.s
 class PutItem(ItemUri):
     """Update Item."""
 
-    item: stac_types.Item = attr.ib(default=Body(None))
+    item: Item = attr.ib(default=Body(None))
 
 
 @attr.s
 class PutCollection(CollectionUri):
     """Update Collection."""
 
-    collection: stac_types.Collection = attr.ib(default=Body(None))
+    collection: Collection = attr.ib(default=Body(None))
 
 
 @attr.s
 class TransactionExtension(ApiExtension):
     """Transaction Extension.
 
     The transaction extension adds several endpoints which allow the creation,
@@ -69,93 +67,137 @@
     response_class: Type[Response] = attr.ib(default=JSONResponse)
 
     def register_create_item(self):
         """Register create item endpoint (POST /collections/{collection_id}/items)."""
         self.router.add_api_route(
             name="Create Item",
             path="/collections/{collection_id}/items",
+            status_code=201,
             response_model=Item if self.settings.enable_response_models else None,
+            responses={
+                201: {
+                    "content": {
+                        MimeTypes.geojson.value: {},
+                    },
+                    "model": Item,
+                }
+            },
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["POST"],
             endpoint=create_async_endpoint(self.client.create_item, PostItem),
         )
 
     def register_update_item(self):
         """Register update item endpoint (PUT
         /collections/{collection_id}/items/{item_id})."""
         self.router.add_api_route(
             name="Update Item",
             path="/collections/{collection_id}/items/{item_id}",
             response_model=Item if self.settings.enable_response_models else None,
+            responses={
+                200: {
+                    "content": {
+                        MimeTypes.geojson.value: {},
+                    },
+                    "model": Item,
+                }
+            },
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["PUT"],
             endpoint=create_async_endpoint(self.client.update_item, PutItem),
         )
 
     def register_delete_item(self):
         """Register delete item endpoint (DELETE
         /collections/{collection_id}/items/{item_id})."""
         self.router.add_api_route(
             name="Delete Item",
             path="/collections/{collection_id}/items/{item_id}",
             response_model=Item if self.settings.enable_response_models else None,
+            responses={
+                200: {
+                    "content": {
+                        MimeTypes.geojson.value: {},
+                    },
+                    "model": Item,
+                }
+            },
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["DELETE"],
             endpoint=create_async_endpoint(self.client.delete_item, ItemUri),
         )
 
     def register_create_collection(self):
         """Register create collection endpoint (POST /collections)."""
         self.router.add_api_route(
             name="Create Collection",
             path="/collections",
+            status_code=201,
             response_model=Collection if self.settings.enable_response_models else None,
+            responses={
+                201: {
+                    "content": {
+                        MimeTypes.json.value: {},
+                    },
+                    "model": Collection,
+                }
+            },
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["POST"],
-            endpoint=create_async_endpoint(
-                self.client.create_collection, stac_types.Collection
-            ),
+            endpoint=create_async_endpoint(self.client.create_collection, Collection),
         )
 
     def register_update_collection(self):
         """Register update collection endpoint (PUT /collections/{collection_id})."""
         self.router.add_api_route(
             name="Update Collection",
             path="/collections/{collection_id}",
             response_model=Collection if self.settings.enable_response_models else None,
+            responses={
+                200: {
+                    "content": {
+                        MimeTypes.json.value: {},
+                    },
+                    "model": Collection,
+                }
+            },
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["PUT"],
-            endpoint=create_async_endpoint(
-                self.client.update_collection, PutCollection
-            ),
+            endpoint=create_async_endpoint(self.client.update_collection, PutCollection),
         )
 
     def register_delete_collection(self):
         """Register delete collection endpoint (DELETE /collections/{collection_id})."""
         self.router.add_api_route(
             name="Delete Collection",
             path="/collections/{collection_id}",
             response_model=Collection if self.settings.enable_response_models else None,
+            responses={
+                200: {
+                    "content": {
+                        MimeTypes.json.value: {},
+                    },
+                    "model": Collection,
+                }
+            },
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["DELETE"],
-            endpoint=create_async_endpoint(
-                self.client.delete_collection, CollectionUri
-            ),
+            endpoint=create_async_endpoint(self.client.delete_collection, CollectionUri),
         )
 
     def register(self, app: FastAPI) -> None:
         """Register the extension with a FastAPI application.
 
         Args:
             app: target FastAPI application.
```

### Comparing `stac_fastapi_extensions-2.5.5.post1/stac_fastapi/extensions/third_party/bulk_transactions.py` & `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/third_party/bulk_transactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Bulk transactions extension."""
+
 import abc
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 import attr
 from fastapi import APIRouter, FastAPI
 from pydantic import BaseModel
@@ -105,17 +106,15 @@
                 "id2": { "type": "Feature", ... },
                 "id3": { "type": "Feature", ... }
             },
             "method": "insert"
         }
     """
 
-    client: Union[
-        AsyncBaseBulkTransactionsClient, BaseBulkTransactionsClient
-    ] = attr.ib()
+    client: Union[AsyncBaseBulkTransactionsClient, BaseBulkTransactionsClient] = attr.ib()
     conformance_classes: List[str] = attr.ib(default=list())
     schema_href: Optional[str] = attr.ib(default=None)
 
     def register(self, app: FastAPI) -> None:
         """Register the extension with a FastAPI application.
 
         Args:
```

### Comparing `stac_fastapi_extensions-2.5.5.post1/stac_fastapi.extensions.egg-info/PKG-INFO` & `stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.extensions
-Version: 2.5.5.post1
+Version: 3.0.0a0
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
@@ -14,17 +14,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: attrs
-Requires-Dist: pydantic[dotenv]<2
-Requires-Dist: stac_pydantic==2.0.*
 Requires-Dist: stac-fastapi.types
 Requires-Dist: stac-fastapi.api
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
```

### Comparing `stac_fastapi_extensions-2.5.5.post1/stac_fastapi.extensions.egg-info/SOURCES.txt` & `stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-2.5.5.post1/tests/test_transaction.py` & `stac_fastapi_extensions-3.0.0a0/tests/test_transaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import json
 from typing import Iterator, Union
 
 import pytest
+from stac_pydantic import Collection
+from stac_pydantic.item import Item
+from stac_pydantic.item_collection import ItemCollection
 from starlette.testclient import TestClient
 
 from stac_fastapi.api.app import StacApi
 from stac_fastapi.extensions.core import TransactionExtension
 from stac_fastapi.types.config import ApiSettings
 from stac_fastapi.types.core import BaseCoreClient, BaseTransactionsClient
-from stac_fastapi.types.stac import Collection, Item, ItemCollection
 
 
 class DummyCoreClient(BaseCoreClient):
     def all_collections(self, *args, **kwargs):
         raise NotImplementedError
 
     def get_collection(self, *args, **kwargs):
@@ -30,35 +32,35 @@
     def item_collection(self, *args, **kwargs):
         raise NotImplementedError
 
 
 class DummyTransactionsClient(BaseTransactionsClient):
     """Dummy client returning parts of the request, rather than proper STAC items."""
 
-    def create_item(self, item: Union[Item, ItemCollection], **kwargs):
-        return {"type": item["type"]}
+    def create_item(self, item: Union[Item, ItemCollection], *args, **kwargs):
+        return {"created": True, "type": item.type}
 
     def update_item(self, collection_id: str, item_id: str, item: Item, **kwargs):
         return {
             "path_collection_id": collection_id,
             "path_item_id": item_id,
-            "type": item["type"],
+            "type": item.type,
         }
 
     def delete_item(self, item_id: str, collection_id: str, **kwargs):
         return {
             "path_collection_id": collection_id,
             "path_item_id": item_id,
         }
 
     def create_collection(self, collection: Collection, **kwargs):
-        return {"type": collection["type"]}
+        return {"type": collection.type}
 
     def update_collection(self, collection_id: str, collection: Collection, **kwargs):
-        return {"path_collection_id": collection_id, "type": collection["type"]}
+        return {"path_collection_id": collection_id, "type": collection.type}
 
     def delete_collection(self, collection_id: str, **kwargs):
         return {"path_collection_id": collection_id}
 
 
 def test_create_item(client: TestClient, item: Item) -> None:
     response = client.post("/collections/a-collection/items", content=json.dumps(item))
@@ -153,28 +155,30 @@
     return {
         "type": "Feature",
         "stac_version": "1.0.0",
         "stac_extensions": [],
         "id": "test_item",
         "geometry": {"type": "Point", "coordinates": [-105, 40]},
         "bbox": [-105, 40, -105, 40],
-        "properties": {},
+        "properties": {"datetime": "2020-06-13T13:00:00Z"},
         "links": [],
         "assets": {},
         "collection": "test_collection",
     }
 
 
 @pytest.fixture
 def collection() -> Collection:
     return {
         "type": "Collection",
         "stac_version": "1.0.0",
         "stac_extensions": [],
         "id": "test_collection",
+        "description": "A test collection",
         "extent": {
             "spatial": {"bbox": [[-180, -90, 180, 90]]},
-            "temporal": {
-                "interval": [["2000-01-01T00:00:00Z", "2024-01-01T00:00:00Z"]]
-            },
+            "temporal": {"interval": [["2000-01-01T00:00:00Z", "2024-01-01T00:00:00Z"]]},
         },
+        "links": [],
+        "assets": {},
+        "license": "proprietary",
     }
```

