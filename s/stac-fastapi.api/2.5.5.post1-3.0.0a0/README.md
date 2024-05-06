# Comparing `tmp/stac_fastapi_api-2.5.5.post1.tar.gz` & `tmp/stac_fastapi_api-3.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_api-2.5.5.post1.tar", last modified: Thu Apr 25 12:06:26 2024, max compression
+gzip compressed data, was "stac_fastapi_api-3.0.0a0.tar", last modified: Mon May  6 16:07:40 2024, max compression
```

## Comparing `stac_fastapi_api-2.5.5.post1.tar` & `stac_fastapi_api-3.0.0a0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:26.873719 stac_fastapi_api-2.5.5.post1/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-25 12:06:26.873719 stac_fastapi_api-2.5.5.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:11.000000 stac_fastapi_api-2.5.5.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-25 12:06:26.873719 stac_fastapi_api-2.5.5.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-25 12:06:11.000000 stac_fastapi_api-2.5.5.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:26.869719 stac_fastapi_api-2.5.5.post1/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:26.873719 stac_fastapi_api-2.5.5.post1/stac_fastapi/api/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 12:06:11.000000 stac_fastapi_api-2.5.5.post1/stac_fastapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14595 2024-04-25 12:06:11.000000 stac_fastapi_api-2.5.5.post1/stac_fastapi/api/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-25 12:06:11.000000 stac_fastapi_api-2.5.5.post1/stac_fastapi/api/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-25 12:06:11.000000 stac_fastapi_api-2.5.5.post1/stac_fastapi/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-25 12:06:11.000000 stac_fastapi_api-2.5.5.post1/stac_fastapi/api/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-25 12:06:11.000000 stac_fastapi_api-2.5.5.post1/stac_fastapi/api/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-25 12:06:11.000000 stac_fastapi_api-2.5.5.post1/stac_fastapi/api/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-25 12:06:11.000000 stac_fastapi_api-2.5.5.post1/stac_fastapi/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 12:06:11.000000 stac_fastapi_api-2.5.5.post1/stac_fastapi/api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:26.873719 stac_fastapi_api-2.5.5.post1/stac_fastapi.api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-25 12:06:26.000000 stac_fastapi_api-2.5.5.post1/stac_fastapi.api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-25 12:06:26.000000 stac_fastapi_api-2.5.5.post1/stac_fastapi.api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:06:26.000000 stac_fastapi_api-2.5.5.post1/stac_fastapi.api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:06:26.000000 stac_fastapi_api-2.5.5.post1/stac_fastapi.api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 12:06:26.000000 stac_fastapi_api-2.5.5.post1/stac_fastapi.api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 12:06:26.000000 stac_fastapi_api-2.5.5.post1/stac_fastapi.api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:26.873719 stac_fastapi_api-2.5.5.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-25 12:06:11.000000 stac_fastapi_api-2.5.5.post1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-25 12:06:11.000000 stac_fastapi_api-2.5.5.post1/tests/test_app_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-25 12:06:11.000000 stac_fastapi_api-2.5.5.post1/tests/test_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:40.282728 stac_fastapi_api-3.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-06 16:07:40.282728 stac_fastapi_api-3.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-06 16:07:40.282728 stac_fastapi_api-3.0.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:40.274727 stac_fastapi_api-3.0.0a0/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:40.278728 stac_fastapi_api-3.0.0a0/stac_fastapi/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16992 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/stac_fastapi/api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:40.278728 stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-06 16:07:40.000000 stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-06 16:07:40.000000 stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:07:40.000000 stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:07:40.000000 stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-06 16:07:40.000000 stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 16:07:40.000000 stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:40.278728 stac_fastapi_api-3.0.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/tests/test_app_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-06 16:07:22.000000 stac_fastapi_api-3.0.0a0/tests/test_models.py
```

### Comparing `stac_fastapi_api-2.5.5.post1/PKG-INFO` & `stac_fastapi_api-3.0.0a0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
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
 Requires-Dist: brotli_asgi
 Requires-Dist: stac-fastapi.types
 Provides-Extra: dev
 Requires-Dist: httpx; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
```

### Comparing `stac_fastapi_api-2.5.5.post1/setup.py` & `stac_fastapi_api-3.0.0a0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
-    "attrs",
-    "pydantic[dotenv]<2",
-    "stac_pydantic==2.0.*",
     "brotli_asgi",
     "stac-fastapi.types",
 ]
 
 extra_reqs = {
     "dev": [
         "httpx",
```

### Comparing `stac_fastapi_api-2.5.5.post1/stac_fastapi/api/app.py` & `stac_fastapi_api-3.0.0a0/stac_fastapi/api/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Fastapi app creation."""
 
+
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import attr
 from brotli_asgi import BrotliMiddleware
 from fastapi import APIRouter, FastAPI
 from fastapi.openapi.utils import get_openapi
 from fastapi.params import Depends
-from stac_pydantic import Collection, Item, ItemCollection
-from stac_pydantic.api import ConformanceClasses, LandingPage
+from stac_pydantic import api
 from stac_pydantic.api.collections import Collections
-from stac_pydantic.version import STAC_VERSION
+from stac_pydantic.api.version import STAC_API_VERSION
+from stac_pydantic.shared import MimeTypes
+from starlette.middleware import Middleware
 from starlette.responses import JSONResponse, Response
 
 from stac_fastapi.api.errors import DEFAULT_STATUS_CODES, add_exception_handlers
 from stac_fastapi.api.middleware import CORSMiddleware, ProxyHeaderMiddleware
 from stac_fastapi.api.models import (
     CollectionUri,
     EmptyRequest,
@@ -90,31 +92,35 @@
         )
     )
     api_version: str = attr.ib(
         default=attr.Factory(
             lambda self: self.settings.stac_fastapi_version, takes_self=True
         )
     )
-    stac_version: str = attr.ib(default=STAC_VERSION)
+    stac_version: str = attr.ib(default=STAC_API_VERSION)
     description: str = attr.ib(
         default=attr.Factory(
             lambda self: self.settings.stac_fastapi_description, takes_self=True
         )
     )
     search_get_request_model: Type[BaseSearchGetRequest] = attr.ib(
         default=BaseSearchGetRequest
     )
     search_post_request_model: Type[BaseSearchPostRequest] = attr.ib(
         default=BaseSearchPostRequest
     )
     pagination_extension = attr.ib(default=TokenPaginationExtension)
     response_class: Type[Response] = attr.ib(default=JSONResponse)
-    middlewares: List = attr.ib(
+    middlewares: List[Middleware] = attr.ib(
         default=attr.Factory(
-            lambda: [BrotliMiddleware, CORSMiddleware, ProxyHeaderMiddleware]
+            lambda: [
+                Middleware(BrotliMiddleware),
+                Middleware(CORSMiddleware),
+                Middleware(ProxyHeaderMiddleware),
+            ]
         )
     )
     route_dependencies: List[Tuple[List[Scope], List[Depends]]] = attr.ib(default=[])
 
     def get_extension(self, extension: Type[ApiExtension]) -> Optional[ApiExtension]:
         """Get an extension.
 
@@ -134,17 +140,25 @@
 
         Returns:
             None
         """
         self.router.add_api_route(
             name="Landing Page",
             path="/",
-            response_model=LandingPage
-            if self.settings.enable_response_models
-            else None,
+            response_model=(
+                api.LandingPage if self.settings.enable_response_models else None
+            ),
+            responses={
+                200: {
+                    "content": {
+                        MimeTypes.json.value: {},
+                    },
+                    "model": api.LandingPage,
+                },
+            },
             response_class=self.response_class,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=create_async_endpoint(self.client.landing_page, EmptyRequest),
         )
 
@@ -153,17 +167,25 @@
 
         Returns:
             None
         """
         self.router.add_api_route(
             name="Conformance Classes",
             path="/conformance",
-            response_model=ConformanceClasses
-            if self.settings.enable_response_models
-            else None,
+            response_model=(
+                api.ConformanceClasses if self.settings.enable_response_models else None
+            ),
+            responses={
+                200: {
+                    "content": {
+                        MimeTypes.json.value: {},
+                    },
+                    "model": api.ConformanceClasses,
+                },
+            },
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=create_async_endpoint(self.client.conformance, EmptyRequest),
         )
 
@@ -172,15 +194,23 @@
 
         Returns:
             None
         """
         self.router.add_api_route(
             name="Get Item",
             path="/collections/{collection_id}/items/{item_id}",
-            response_model=Item if self.settings.enable_response_models else None,
+            response_model=api.Item if self.settings.enable_response_models else None,
+            responses={
+                200: {
+                    "content": {
+                        MimeTypes.geojson.value: {},
+                    },
+                    "model": api.Item,
+                },
+            },
             response_class=GeoJSONResponse,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=create_async_endpoint(self.client.get_item, ItemUri),
         )
 
@@ -190,17 +220,27 @@
         Returns:
             None
         """
         fields_ext = self.get_extension(FieldsExtension)
         self.router.add_api_route(
             name="Search",
             path="/search",
-            response_model=(ItemCollection if not fields_ext else None)
-            if self.settings.enable_response_models
-            else None,
+            response_model=(
+                (api.ItemCollection if not fields_ext else None)
+                if self.settings.enable_response_models
+                else None
+            ),
+            responses={
+                200: {
+                    "content": {
+                        MimeTypes.geojson.value: {},
+                    },
+                    "model": api.ItemCollection,
+                },
+            },
             response_class=GeoJSONResponse,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["POST"],
             endpoint=create_async_endpoint(
                 self.client.post_search, self.search_post_request_model
             ),
@@ -212,17 +252,27 @@
         Returns:
             None
         """
         fields_ext = self.get_extension(FieldsExtension)
         self.router.add_api_route(
             name="Search",
             path="/search",
-            response_model=(ItemCollection if not fields_ext else None)
-            if self.settings.enable_response_models
-            else None,
+            response_model=(
+                (api.ItemCollection if not fields_ext else None)
+                if self.settings.enable_response_models
+                else None
+            ),
+            responses={
+                200: {
+                    "content": {
+                        MimeTypes.geojson.value: {},
+                    },
+                    "model": api.ItemCollection,
+                },
+            },
             response_class=GeoJSONResponse,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=create_async_endpoint(
                 self.client.get_search, self.search_get_request_model
             ),
@@ -233,17 +283,25 @@
 
         Returns:
             None
         """
         self.router.add_api_route(
             name="Get Collections",
             path="/collections",
-            response_model=Collections
-            if self.settings.enable_response_models
-            else None,
+            response_model=(
+                Collections if self.settings.enable_response_models else None
+            ),
+            responses={
+                200: {
+                    "content": {
+                        MimeTypes.json.value: {},
+                    },
+                    "model": Collections,
+                },
+            },
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=create_async_endpoint(self.client.all_collections, EmptyRequest),
         )
 
@@ -252,15 +310,25 @@
 
         Returns:
             None
         """
         self.router.add_api_route(
             name="Get Collection",
             path="/collections/{collection_id}",
-            response_model=Collection if self.settings.enable_response_models else None,
+            response_model=api.Collection
+            if self.settings.enable_response_models
+            else None,
+            responses={
+                200: {
+                    "content": {
+                        MimeTypes.json.value: {},
+                    },
+                    "model": api.Collection,
+                },
+            },
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=create_async_endpoint(self.client.get_collection, CollectionUri),
         )
 
@@ -279,17 +347,25 @@
             "ItemCollectionURI",
             base_model=ItemCollectionUri,
             mixins=mixins,
         )
         self.router.add_api_route(
             name="Get ItemCollection",
             path="/collections/{collection_id}/items",
-            response_model=ItemCollection
-            if self.settings.enable_response_models
-            else None,
+            response_model=(
+                api.ItemCollection if self.settings.enable_response_models else None
+            ),
+            responses={
+                200: {
+                    "content": {
+                        MimeTypes.geojson.value: {},
+                    },
+                    "model": api.ItemCollection,
+                },
+            },
             response_class=GeoJSONResponse,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["GET"],
             endpoint=create_async_endpoint(self.client.item_collection, request_model),
         )
 
@@ -359,14 +435,19 @@
                 to apply to each scope.
 
         Returns:
             None
         """
         return add_route_dependencies(self.app.router.routes, scopes, dependencies)
 
+    def add_middleware(self, middleware: Middleware):
+        """Add a middleware class to the application."""
+        self.app.user_middleware.insert(0, middleware)
+        self.app.middleware_stack = self.app.build_middleware_stack()
+
     def __attrs_post_init__(self):
         """Post-init hook.
 
         Responsible for setting up the application upon instantiation of the class.
 
         Returns:
             None
@@ -403,12 +484,12 @@
         add_exception_handlers(self.app, status_codes=self.exceptions)
 
         # customize openapi
         self.app.openapi = self.customize_openapi
 
         # add middlewares
         for middleware in self.middlewares:
-            self.app.add_middleware(middleware)
+            self.add_middleware(middleware)
 
         # customize route dependencies
         for scopes, dependencies in self.route_dependencies:
             self.add_route_dependencies(scopes=scopes, dependencies=dependencies)
```

### Comparing `stac_fastapi_api-2.5.5.post1/stac_fastapi/api/config.py` & `stac_fastapi_api-3.0.0a0/stac_fastapi/api/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Application settings."""
+
 import enum
 
 
 # TODO: Move to stac-pydantic
 # Does that make sense now? The shift to json schema rather than a well-known
 # enumeration makes that less obvious.
 class ApiExtensions(enum.Enum):
```

### Comparing `stac_fastapi_api-2.5.5.post1/stac_fastapi/api/errors.py` & `stac_fastapi_api-3.0.0a0/stac_fastapi/api/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Error handling."""
 
 import logging
 from typing import Callable, Dict, Type, TypedDict
 
 from fastapi import FastAPI
-from fastapi.exceptions import RequestValidationError
+from fastapi.exceptions import RequestValidationError, ResponseValidationError
 from starlette import status
 from starlette.requests import Request
 from starlette.responses import JSONResponse
 
 from stac_fastapi.types.errors import (
     ConflictError,
     DatabaseError,
@@ -23,14 +23,15 @@
 DEFAULT_STATUS_CODES = {
     NotFoundError: status.HTTP_404_NOT_FOUND,
     ConflictError: status.HTTP_409_CONFLICT,
     ForeignKeyError: status.HTTP_424_FAILED_DEPENDENCY,
     DatabaseError: status.HTTP_424_FAILED_DEPENDENCY,
     Exception: status.HTTP_500_INTERNAL_SERVER_ERROR,
     InvalidQueryParameter: status.HTTP_400_BAD_REQUEST,
+    ResponseValidationError: status.HTTP_500_INTERNAL_SERVER_ERROR,
 }
 
 
 class ErrorResponse(TypedDict):
     """A JSON error response returned by the API.
 
     The STAC API spec expects that `code` and `description` are both present in
```

### Comparing `stac_fastapi_api-2.5.5.post1/stac_fastapi/api/middleware.py` & `stac_fastapi_api-3.0.0a0/stac_fastapi/api/middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Api middleware."""
+
 import re
 import typing
 from http.client import HTTP_PORT, HTTPS_PORT
 from typing import List, Tuple
 
 from starlette.middleware.cors import CORSMiddleware as _CORSMiddleware
 from starlette.types import ASGIApp, Receive, Scope, Send
```

### Comparing `stac_fastapi_api-2.5.5.post1/stac_fastapi/api/models.py` & `stac_fastapi_api-3.0.0a0/stac_fastapi/api/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Api request/response models."""
 
 import importlib.util
-from typing import Optional, Type, Union
+from typing import List, Optional, Type, Union
 
 import attr
-from fastapi import Body, Path
+from fastapi import Path
 from pydantic import BaseModel, create_model
-from pydantic.fields import UndefinedType
 from stac_pydantic.shared import BBox
 
 from stac_fastapi.types.extension import ApiExtension
 from stac_fastapi.types.rfc3339 import DateTimeType
 from stac_fastapi.types.search import (
     APIRequest,
     BaseSearchGetRequest,
@@ -19,16 +18,16 @@
     str_to_interval,
 )
 
 
 def create_request_model(
     model_name="SearchGetRequest",
     base_model: Union[Type[BaseModel], APIRequest] = BaseSearchGetRequest,
-    extensions: Optional[ApiExtension] = None,
-    mixins: Optional[Union[BaseModel, APIRequest]] = None,
+    extensions: Optional[List[ApiExtension]] = None,
+    mixins: Optional[Union[List[BaseModel], List[APIRequest]]] = None,
     request_type: Optional[str] = "GET",
 ) -> Union[Type[BaseModel], APIRequest]:
     """Create a pydantic model for validating request bodies."""
     fields = {}
     extension_models = []
 
     # Check extensions for additional parameters to search
@@ -43,59 +42,39 @@
     # Handle GET requests
     if all([issubclass(m, APIRequest) for m in models]):
         return attr.make_class(model_name, attrs={}, bases=tuple(models))
 
     # Handle POST requests
     elif all([issubclass(m, BaseModel) for m in models]):
         for model in models:
-            for k, v in model.__fields__.items():
-                field_info = v.field_info
-                body = Body(
-                    None
-                    if isinstance(field_info.default, UndefinedType)
-                    else field_info.default,
-                    default_factory=field_info.default_factory,
-                    alias=field_info.alias,
-                    alias_priority=field_info.alias_priority,
-                    title=field_info.title,
-                    description=field_info.description,
-                    const=field_info.const,
-                    gt=field_info.gt,
-                    ge=field_info.ge,
-                    lt=field_info.lt,
-                    le=field_info.le,
-                    multiple_of=field_info.multiple_of,
-                    min_items=field_info.min_items,
-                    max_items=field_info.max_items,
-                    min_length=field_info.min_length,
-                    max_length=field_info.max_length,
-                    regex=field_info.regex,
-                    extra=field_info.extra,
-                )
-                fields[k] = (v.outer_type_, body)
+            for k, field_info in model.model_fields.items():
+                fields[k] = (field_info.annotation, field_info)
         return create_model(model_name, **fields, __base__=base_model)
 
     raise TypeError("Mixed Request Model types. Check extension request types.")
 
 
 def create_get_request_model(
-    extensions, base_model: BaseSearchGetRequest = BaseSearchGetRequest
-):
+    extensions: Optional[List[ApiExtension]],
+    base_model: BaseSearchGetRequest = BaseSearchGetRequest,
+) -> APIRequest:
     """Wrap create_request_model to create the GET request model."""
+
     return create_request_model(
         "SearchGetRequest",
         base_model=base_model,
         extensions=extensions,
         request_type="GET",
     )
 
 
 def create_post_request_model(
-    extensions, base_model: BaseSearchPostRequest = BaseSearchPostRequest
-):
+    extensions: Optional[List[ApiExtension]],
+    base_model: BaseSearchPostRequest = BaseSearchPostRequest,
+) -> Type[BaseModel]:
     """Wrap create_request_model to create the POST request model."""
     return create_request_model(
         "SearchPostRequest",
         base_model=base_model,
         extensions=extensions,
         request_type="POST",
     )
```

### Comparing `stac_fastapi_api-2.5.5.post1/stac_fastapi/api/openapi.py` & `stac_fastapi_api-3.0.0a0/stac_fastapi/api/openapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """openapi."""
+
 import warnings
 
 from fastapi import FastAPI
 from fastapi.openapi.utils import get_openapi
 from starlette.requests import Request
 from starlette.responses import JSONResponse, Response
 from starlette.routing import Route, request_response
@@ -39,17 +40,15 @@
     old_endpoint = openapi_route.endpoint
 
     # Create a patched endpoint function that modifies the content type of the response
     async def patched_openapi_endpoint(req: Request) -> Response:
         # Get the response from the old endpoint function
         response: JSONResponse = await old_endpoint(req)
         # Update the content type header in place
-        response.headers[
-            "content-type"
-        ] = "application/vnd.oai.openapi+json;version=3.0"
+        response.headers["content-type"] = "application/vnd.oai.openapi+json;version=3.0"
         # Return the updated response
         return response
 
     # When a Route is accessed the `handle` function calls `self.app`. Which is
     # the endpoint function wrapped with `request_response`. So we need to wrap
     # our patched function and replace the existing app with it.
     openapi_route.app = request_response(patched_openapi_endpoint)
```

### Comparing `stac_fastapi_api-2.5.5.post1/stac_fastapi/api/routes.py` & `stac_fastapi_api-3.0.0a0/stac_fastapi/api/routes.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-2.5.5.post1/stac_fastapi.api.egg-info/PKG-INFO` & `stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
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
 Requires-Dist: brotli_asgi
 Requires-Dist: stac-fastapi.types
 Provides-Extra: dev
 Requires-Dist: httpx; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
```

### Comparing `stac_fastapi_api-2.5.5.post1/stac_fastapi.api.egg-info/SOURCES.txt` & `stac_fastapi_api-3.0.0a0/stac_fastapi.api.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,9 +13,11 @@
 stac_fastapi/api/errors.py
 stac_fastapi/api/middleware.py
 stac_fastapi/api/models.py
 stac_fastapi/api/openapi.py
 stac_fastapi/api/routes.py
 stac_fastapi/api/version.py
 tests/test_api.py
+tests/test_app.py
 tests/test_app_prefix.py
-tests/test_middleware.py
+tests/test_middleware.py
+tests/test_models.py
```

### Comparing `stac_fastapi_api-2.5.5.post1/tests/test_api.py` & `stac_fastapi_api-3.0.0a0/tests/test_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,52 +37,84 @@
                 path = route["path"].format(
                     collectionId="test_collection", itemId="test_item"
                 )
                 response = client.request(
                     method=route["method"].lower(),
                     url=path,
                     auth=("bob", "dobbs"),
-                    content='{"dummy": "payload"}',
+                    content=route["payload"],
                     headers={"content-type": "application/json"},
                 )
                 assert (
-                    response.status_code == 200
+                    200 <= response.status_code < 300
                 ), "Authenticated requests should be accepted"
                 assert response.json() == "dummy response"
 
     def test_openapi_content_type(self):
         api = self._build_api()
         with TestClient(api.app) as client:
             response = client.get(api.settings.openapi_url)
             assert (
                 response.headers["content-type"]
                 == "application/vnd.oai.openapi+json;version=3.0"
             )
 
-    def test_build_api_with_route_dependencies(self):
+    def test_build_api_with_route_dependencies(self, collection, item):
         routes = [
-            {"path": "/collections", "method": "POST"},
-            {"path": "/collections/{collectionId}", "method": "PUT"},
-            {"path": "/collections/{collectionId}", "method": "DELETE"},
-            {"path": "/collections/{collectionId}/items", "method": "POST"},
-            {"path": "/collections/{collectionId}/items/{itemId}", "method": "PUT"},
-            {"path": "/collections/{collectionId}/items/{itemId}", "method": "DELETE"},
+            {"path": "/collections", "method": "POST", "payload": collection},
+            {
+                "path": "/collections/{collectionId}",
+                "method": "PUT",
+                "payload": collection,
+            },
+            {"path": "/collections/{collectionId}", "method": "DELETE", "payload": ""},
+            {
+                "path": "/collections/{collectionId}/items",
+                "method": "POST",
+                "payload": item,
+            },
+            {
+                "path": "/collections/{collectionId}/items/{itemId}",
+                "method": "PUT",
+                "payload": item,
+            },
+            {
+                "path": "/collections/{collectionId}/items/{itemId}",
+                "method": "DELETE",
+                "payload": "",
+            },
         ]
         dependencies = [Depends(must_be_bob)]
         api = self._build_api(route_dependencies=[(routes, dependencies)])
         self._assert_dependency_applied(api, routes)
 
-    def test_add_route_dependencies_after_building_api(self):
+    def test_add_route_dependencies_after_building_api(self, collection, item):
         routes = [
-            {"path": "/collections", "method": "POST"},
-            {"path": "/collections/{collectionId}", "method": "PUT"},
-            {"path": "/collections/{collectionId}", "method": "DELETE"},
-            {"path": "/collections/{collectionId}/items", "method": "POST"},
-            {"path": "/collections/{collectionId}/items/{itemId}", "method": "PUT"},
-            {"path": "/collections/{collectionId}/items/{itemId}", "method": "DELETE"},
+            {"path": "/collections", "method": "POST", "payload": collection},
+            {
+                "path": "/collections/{collectionId}",
+                "method": "PUT",
+                "payload": collection,
+            },
+            {"path": "/collections/{collectionId}", "method": "DELETE", "payload": ""},
+            {
+                "path": "/collections/{collectionId}/items",
+                "method": "POST",
+                "payload": item,
+            },
+            {
+                "path": "/collections/{collectionId}/items/{itemId}",
+                "method": "PUT",
+                "payload": item,
+            },
+            {
+                "path": "/collections/{collectionId}/items/{itemId}",
+                "method": "DELETE",
+                "payload": "",
+            },
         ]
         api = self._build_api()
         api.add_route_dependencies(scopes=routes, dependencies=[Depends(must_be_bob)])
         self._assert_dependency_applied(api, routes)
 
 
 class DummyCoreClient(core.BaseCoreClient):
```

### Comparing `stac_fastapi_api-2.5.5.post1/tests/test_app_prefix.py` & `stac_fastapi_api-3.0.0a0/tests/test_app_prefix.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         assert conformance.status_code == 200, conformance.json()
 
         # NOTE: The collections/collection/items/item links do not have the prefix
         # because they are created in the fixtures
         collections = client.get(f"{prefix}/collections")
         assert collections.status_code == 200, collections.json()
         collection_id = collections.json()["collections"][0]["id"]
-        print(collections.json()["links"])
+
         collection = client.get(f"{prefix}/collections/{collection_id}")
         assert collection.status_code == 200, collection.json()
 
         items = client.get(f"{prefix}/collections/{collection_id}/items")
         assert items.status_code == 200, items.json()
 
         item_id = items.json()["features"][0]["id"]
```

### Comparing `stac_fastapi_api-2.5.5.post1/tests/test_middleware.py` & `stac_fastapi_api-3.0.0a0/tests/test_middleware.py`

 * *Files identical despite different names*

