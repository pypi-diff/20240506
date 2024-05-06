# Comparing `tmp/stac_fastapi_types-2.5.5.post1.tar.gz` & `tmp/stac_fastapi_types-3.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_types-2.5.5.post1.tar", last modified: Thu Apr 25 12:06:19 2024, max compression
+gzip compressed data, was "stac_fastapi_types-3.0.0a0.tar", last modified: Mon May  6 16:07:31 2024, max compression
```

## Comparing `stac_fastapi_types-2.5.5.post1.tar` & `stac_fastapi_types-3.0.0a0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:19.653653 stac_fastapi_types-2.5.5.post1/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-25 12:06:19.653653 stac_fastapi_types-2.5.5.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:11.000000 stac_fastapi_types-2.5.5.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-25 12:06:19.653653 stac_fastapi_types-2.5.5.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-25 12:06:11.000000 stac_fastapi_types-2.5.5.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:19.649653 stac_fastapi_types-2.5.5.post1/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:19.649653 stac_fastapi_types-2.5.5.post1/stac_fastapi/types/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 12:06:11.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-25 12:06:11.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi/types/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-25 12:06:11.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi/types/conformance.py
--rw-r--r--   0 runner    (1001) docker     (127)    25247 2024-04-25 12:06:11.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi/types/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-25 12:06:11.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi/types/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-25 12:06:11.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi/types/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-25 12:06:11.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi/types/links.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-25 12:06:11.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi/types/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-25 12:06:11.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi/types/rfc3339.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-25 12:06:11.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi/types/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-25 12:06:11.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi/types/stac.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 12:06:11.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi/types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:19.653653 stac_fastapi_types-2.5.5.post1/stac_fastapi.types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-25 12:06:19.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi.types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-25 12:06:19.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi.types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:06:19.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi.types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:06:19.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi.types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-25 12:06:19.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi.types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 12:06:19.000000 stac_fastapi_types-2.5.5.post1/stac_fastapi.types.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:06:19.653653 stac_fastapi_types-2.5.5.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-25 12:06:11.000000 stac_fastapi_types-2.5.5.post1/tests/test_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-25 12:06:11.000000 stac_fastapi_types-2.5.5.post1/tests/test_rfc3339.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:31.238577 stac_fastapi_types-3.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-06 16:07:31.238577 stac_fastapi_types-3.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-06 16:07:31.238577 stac_fastapi_types-3.0.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:31.234578 stac_fastapi_types-3.0.0a0/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:31.234578 stac_fastapi_types-3.0.0a0/stac_fastapi/types/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/conformance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24819 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/rfc3339.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/stac.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:31.238577 stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-06 16:07:31.000000 stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-06 16:07:31.000000 stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:07:31.000000 stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:07:31.000000 stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-06 16:07:31.000000 stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 16:07:31.000000 stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:31.238577 stac_fastapi_types-3.0.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/tests/test_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/tests/test_rfc3339.py
```

### Comparing `stac_fastapi_types-2.5.5.post1/PKG-INFO` & `stac_fastapi_types-3.0.0a0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.types
-Version: 2.5.5.post1
+Version: 3.0.0a0
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
@@ -14,18 +14,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: fastapi>=0.73.0
-Requires-Dist: attrs
-Requires-Dist: pydantic[dotenv]<2
-Requires-Dist: stac_pydantic==2.0.*
+Requires-Dist: fastapi>=0.100.0
+Requires-Dist: attrs>=23.2.0
+Requires-Dist: pydantic-settings>=2
+Requires-Dist: stac_pydantic>=3
 Requires-Dist: pystac==1.*
 Requires-Dist: iso8601<2.2.0,>=1.0.2
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
```

### Comparing `stac_fastapi_types-2.5.5.post1/setup.py` & `stac_fastapi_types-3.0.0a0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
-    "fastapi>=0.73.0",
-    "attrs",
-    "pydantic[dotenv]<2",
-    "stac_pydantic==2.0.*",
+    "fastapi>=0.100.0",
+    "attrs>=23.2.0",
+    "pydantic-settings>=2",
+    "stac_pydantic>=3",
     "pystac==1.*",
     "iso8601>=1.0.2,<2.2.0",
 ]
 
 extra_reqs = {
     "dev": [
         "pytest",
```

### Comparing `stac_fastapi_types-2.5.5.post1/stac_fastapi/types/config.py` & `stac_fastapi_types-3.0.0a0/stac_fastapi/types/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """stac_fastapi.types.config module."""
+
 from typing import Optional, Set
 
-from pydantic import BaseSettings
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 
 class ApiSettings(BaseSettings):
     """ApiSettings.
 
     Defines api configuration, potentially through environment variables.
     See https://pydantic-docs.helpmanual.io/usage/settings/.
@@ -31,19 +32,15 @@
     app_port: int = 8000
     reload: bool = True
     enable_response_models: bool = False
 
     openapi_url: str = "/api"
     docs_url: str = "/api.html"
 
-    class Config:
-        """Model config (https://pydantic-docs.helpmanual.io/usage/model_config/)."""
-
-        extra = "allow"
-        env_file = ".env"
+    model_config = SettingsConfigDict(env_file=".env", extra="allow")
 
 
 class Settings:
     """Holds the global instance of settings."""
 
     _instance: Optional[ApiSettings] = None
```

### Comparing `stac_fastapi_types-2.5.5.post1/stac_fastapi/types/conformance.py` & `stac_fastapi_types-3.0.0a0/stac_fastapi/types/conformance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Conformance Classes."""
+
 from enum import Enum
 
 
 class STACConformanceClasses(str, Enum):
     """Conformance classes for the STAC API spec."""
 
     CORE = "https://api.stacspec.org/v1.0.0/core"
```

### Comparing `stac_fastapi_types-2.5.5.post1/stac_fastapi/types/core.py` & `stac_fastapi_types-3.0.0a0/stac_fastapi/types/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """Base clients."""
 
+
 import abc
 from typing import Any, Dict, List, Optional, Union
 from urllib.parse import urljoin
 
 import attr
 from fastapi import Request
+from geojson_pydantic.geometries import Geometry
+from stac_pydantic import Collection, Item, ItemCollection
+from stac_pydantic.api.version import STAC_API_VERSION
 from stac_pydantic.links import Relations
 from stac_pydantic.shared import BBox, MimeTypes
-from stac_pydantic.version import STAC_VERSION
 from starlette.responses import Response
 
-from stac_fastapi.types import stac as stac_types
+from stac_fastapi.types import stac
 from stac_fastapi.types.config import ApiSettings
 from stac_fastapi.types.conformance import BASE_CONFORMANCE_CLASSES
 from stac_fastapi.types.extension import ApiExtension
 from stac_fastapi.types.requests import get_base_url
 from stac_fastapi.types.rfc3339 import DateTimeType
 from stac_fastapi.types.search import BaseSearchPostRequest
-from stac_fastapi.types.stac import Conformance
 
 NumType = Union[float, int]
 StacType = Dict[str, Any]
 
 api_settings = ApiSettings()
 
 
@@ -30,17 +32,17 @@
 class BaseTransactionsClient(abc.ABC):
     """Defines a pattern for implementing the STAC API Transaction Extension."""
 
     @abc.abstractmethod
     def create_item(
         self,
         collection_id: str,
-        item: Union[stac_types.Item, stac_types.ItemCollection],
+        item: Union[Item, ItemCollection],
         **kwargs,
-    ) -> Optional[Union[stac_types.Item, Response, None]]:
+    ) -> Optional[Union[stac.Item, Response, None]]:
         """Create a new item.
 
         Called with `POST /collections/{collection_id}/items`.
 
         Args:
             item: the item or item collection
             collection_id: the id of the collection from the resource path
@@ -48,16 +50,16 @@
         Returns:
             The item that was created or None if item collection.
         """
         ...
 
     @abc.abstractmethod
     def update_item(
-        self, collection_id: str, item_id: str, item: stac_types.Item, **kwargs
-    ) -> Optional[Union[stac_types.Item, Response]]:
+        self, collection_id: str, item_id: str, item: Item, **kwargs
+    ) -> Optional[Union[stac.Item, Response]]:
         """Perform a complete update on an existing item.
 
         Called with `PUT /collections/{collection_id}/items`. It is expected
         that this item already exists.  The update should do a diff against the
         saved item and perform any necessary updates.  Partial updates are not
         supported by the transactions extension.
 
@@ -69,15 +71,15 @@
             The updated item.
         """
         ...
 
     @abc.abstractmethod
     def delete_item(
         self, item_id: str, collection_id: str, **kwargs
-    ) -> Optional[Union[stac_types.Item, Response]]:
+    ) -> Optional[Union[stac.Item, Response]]:
         """Delete an item from a collection.
 
         Called with `DELETE /collections/{collection_id}/items/{item_id}`
 
         Args:
             item_id: id of the item.
             collection_id: id of the collection.
@@ -85,32 +87,32 @@
         Returns:
             The deleted item.
         """
         ...
 
     @abc.abstractmethod
     def create_collection(
-        self, collection: stac_types.Collection, **kwargs
-    ) -> Optional[Union[stac_types.Collection, Response]]:
+        self, collection: Collection, **kwargs
+    ) -> Optional[Union[stac.Collection, Response]]:
         """Create a new collection.
 
         Called with `POST /collections`.
 
         Args:
             collection: the collection
 
         Returns:
             The collection that was created.
         """
         ...
 
     @abc.abstractmethod
     def update_collection(
-        self, collection_id: str, collection: stac_types.Collection, **kwargs
-    ) -> Optional[Union[stac_types.Collection, Response]]:
+        self, collection_id: str, collection: Collection, **kwargs
+    ) -> Optional[Union[stac.Collection, Response]]:
         """Perform a complete update on an existing collection.
 
         Called with `PUT /collections/{collection_id}`. It is expected that this
         collection already exists.  The update should do a diff against the saved
         collection and perform any necessary updates.  Partial updates are not
         supported by the transactions extension.
 
@@ -122,15 +124,15 @@
             The updated collection.
         """
         ...
 
     @abc.abstractmethod
     def delete_collection(
         self, collection_id: str, **kwargs
-    ) -> Optional[Union[stac_types.Collection, Response]]:
+    ) -> Optional[Union[stac.Collection, Response]]:
         """Delete a collection.
 
         Called with `DELETE /collections/{collection_id}`
 
         Args:
             collection_id: id of the collection.
 
@@ -144,17 +146,17 @@
 class AsyncBaseTransactionsClient(abc.ABC):
     """Defines a pattern for implementing the STAC transaction extension."""
 
     @abc.abstractmethod
     async def create_item(
         self,
         collection_id: str,
-        item: Union[stac_types.Item, stac_types.ItemCollection],
+        item: Union[Item, ItemCollection],
         **kwargs,
-    ) -> Optional[Union[stac_types.Item, Response, None]]:
+    ) -> Optional[Union[stac.Item, Response, None]]:
         """Create a new item.
 
         Called with `POST /collections/{collection_id}/items`.
 
         Args:
             item: the item or item collection
             collection_id: the id of the collection from the resource path
@@ -162,16 +164,16 @@
         Returns:
             The item that was created or None if item collection.
         """
         ...
 
     @abc.abstractmethod
     async def update_item(
-        self, collection_id: str, item_id: str, item: stac_types.Item, **kwargs
-    ) -> Optional[Union[stac_types.Item, Response]]:
+        self, collection_id: str, item_id: str, item: Item, **kwargs
+    ) -> Optional[Union[stac.Item, Response]]:
         """Perform a complete update on an existing item.
 
         Called with `PUT /collections/{collection_id}/items`. It is expected
         that this item already exists.  The update should do a diff against the
         saved item and perform any necessary updates.  Partial updates are not
         supported by the transactions extension.
 
@@ -182,15 +184,15 @@
             The updated item.
         """
         ...
 
     @abc.abstractmethod
     async def delete_item(
         self, item_id: str, collection_id: str, **kwargs
-    ) -> Optional[Union[stac_types.Item, Response]]:
+    ) -> Optional[Union[stac.Item, Response]]:
         """Delete an item from a collection.
 
         Called with `DELETE /collections/{collection_id}/items/{item_id}`
 
         Args:
             item_id: id of the item.
             collection_id: id of the collection.
@@ -198,32 +200,32 @@
         Returns:
             The deleted item.
         """
         ...
 
     @abc.abstractmethod
     async def create_collection(
-        self, collection: stac_types.Collection, **kwargs
-    ) -> Optional[Union[stac_types.Collection, Response]]:
+        self, collection: Collection, **kwargs
+    ) -> Optional[Union[stac.Collection, Response]]:
         """Create a new collection.
 
         Called with `POST /collections`.
 
         Args:
             collection: the collection
 
         Returns:
             The collection that was created.
         """
         ...
 
     @abc.abstractmethod
     async def update_collection(
-        self, collection_id: str, collection: stac_types.Collection, **kwargs
-    ) -> Optional[Union[stac_types.Collection, Response]]:
+        self, collection_id: str, collection: Collection, **kwargs
+    ) -> Optional[Union[stac.Collection, Response]]:
         """Perform a complete update on an existing collection.
 
         Called with `PUT /collections/{collection_id}`. It is expected that this item
         already exists.  The update should do a diff against the saved collection and
         perform any necessary updates.  Partial updates are not supported by the
         transactions extension.
 
@@ -235,15 +237,15 @@
             The updated collection.
         """
         ...
 
     @abc.abstractmethod
     async def delete_collection(
         self, collection_id: str, **kwargs
-    ) -> Optional[Union[stac_types.Collection, Response]]:
+    ) -> Optional[Union[stac.Collection, Response]]:
         """Delete a collection.
 
         Called with `DELETE /collections/{collection_id}`
 
         Args:
             collection_id: id of the collection.
 
@@ -253,71 +255,72 @@
         ...
 
 
 @attr.s
 class LandingPageMixin(abc.ABC):
     """Create a STAC landing page (GET /)."""
 
-    stac_version: str = attr.ib(default=STAC_VERSION)
+    stac_version: str = attr.ib(default=STAC_API_VERSION)
     landing_page_id: str = attr.ib(default=api_settings.stac_fastapi_landing_id)
     title: str = attr.ib(default=api_settings.stac_fastapi_title)
     description: str = attr.ib(default=api_settings.stac_fastapi_description)
 
     def _landing_page(
         self,
         base_url: str,
         conformance_classes: List[str],
         extension_schemas: List[str],
-    ) -> stac_types.LandingPage:
-        landing_page = stac_types.LandingPage(
+    ) -> stac.LandingPage:
+        landing_page = stac.LandingPage(
             type="Catalog",
             id=self.landing_page_id,
             title=self.title,
             description=self.description,
             stac_version=self.stac_version,
             conformsTo=conformance_classes,
             links=[
                 {
                     "rel": Relations.self.value,
-                    "type": MimeTypes.json,
+                    "type": MimeTypes.json.value,
                     "href": base_url,
                 },
                 {
                     "rel": Relations.root.value,
-                    "type": MimeTypes.json,
+                    "type": MimeTypes.json.value,
                     "href": base_url,
                 },
                 {
-                    "rel": "data",
-                    "type": MimeTypes.json,
+                    "rel": Relations.data.value,
+                    "type": MimeTypes.json.value,
                     "href": urljoin(base_url, "collections"),
                 },
                 {
                     "rel": Relations.conformance.value,
-                    "type": MimeTypes.json,
+                    "type": MimeTypes.json.value,
                     "title": "STAC/OGC conformance classes implemented by this server",
                     "href": urljoin(base_url, "conformance"),
                 },
                 {
                     "rel": Relations.search.value,
-                    "type": MimeTypes.geojson,
+                    "type": MimeTypes.geojson.value,
                     "title": "STAC search",
                     "href": urljoin(base_url, "search"),
                     "method": "GET",
                 },
                 {
                     "rel": Relations.search.value,
-                    "type": MimeTypes.geojson,
+                    "type": MimeTypes.geojson.value,
                     "title": "STAC search",
                     "href": urljoin(base_url, "search"),
                     "method": "POST",
                 },
             ],
             stac_extensions=extension_schemas,
         )
+
         return landing_page
 
 
 @attr.s  # type:ignore
 class BaseCoreClient(LandingPageMixin, abc.ABC):
     """Defines a pattern for implementing STAC api core endpoints.
 
@@ -352,24 +355,25 @@
 
         for extension in self.extensions:
             extension_classes = getattr(extension, "conformance_classes", [])
             base_conformance.extend(extension_classes)
 
         return base_conformance
 
-    def landing_page(self, **kwargs) -> stac_types.LandingPage:
+    def landing_page(self, **kwargs) -> stac.LandingPage:
         """Landing page.
 
         Called with `GET /`.
 
         Returns:
             API landing page, serving as an entry point to the API.
         """
         request: Request = kwargs["request"]
         base_url = get_base_url(request)
+
         landing_page = self._landing_page(
             base_url=base_url,
             conformance_classes=self.conformance_classes(),
             extension_schemas=[],
         )
 
         # Add Queryables link
@@ -384,60 +388,61 @@
                     "href": urljoin(base_url, "queryables"),
                     "method": "GET",
                 }
             )
 
         # Add Collections links
         collections = self.all_collections(request=kwargs["request"])
+
         for collection in collections["collections"]:
             landing_page["links"].append(
                 {
                     "rel": Relations.child.value,
                     "type": MimeTypes.json.value,
                     "title": collection.get("title") or collection.get("id"),
                     "href": urljoin(base_url, f"collections/{collection['id']}"),
                 }
             )
 
         # Add OpenAPI URL
         landing_page["links"].append(
             {
-                "rel": "service-desc",
-                "type": "application/vnd.oai.openapi+json;version=3.0",
+                "rel": Relations.service_desc.value,
+                "type": MimeTypes.openapi.value,
                 "title": "OpenAPI service description",
                 "href": str(request.url_for("openapi")),
             }
         )
 
         # Add human readable service-doc
         landing_page["links"].append(
             {
-                "rel": "service-doc",
-                "type": "text/html",
+                "rel": Relations.service_doc.value,
+                "type": MimeTypes.html.value,
                 "title": "OpenAPI service documentation",
                 "href": str(request.url_for("swagger_ui_html")),
             }
         )
 
-        return landing_page
+        return stac.LandingPage(**landing_page)
 
-    def conformance(self, **kwargs) -> stac_types.Conformance:
+    def conformance(self, **kwargs) -> stac.Conformance:
         """Conformance classes.
 
         Called with `GET /conformance`.
 
         Returns:
             Conformance classes which the server conforms to.
         """
-        return Conformance(conformsTo=self.conformance_classes())
+        return stac.Conformance(conformsTo=self.conformance_classes())
 
     @abc.abstractmethod
     def post_search(
         self, search_request: BaseSearchPostRequest, **kwargs
-    ) -> stac_types.ItemCollection:
+    ) -> stac.ItemCollection:
         """Cross catalog search (POST).
 
         Called with `POST /search`.
 
         Args:
             search_request: search request parameters.
 
@@ -448,60 +453,56 @@
 
     @abc.abstractmethod
     def get_search(
         self,
         collections: Optional[List[str]] = None,
         ids: Optional[List[str]] = None,
         bbox: Optional[BBox] = None,
+        intersects: Optional[Geometry] = None,
         datetime: Optional[DateTimeType] = None,
         limit: Optional[int] = 10,
-        query: Optional[str] = None,
-        token: Optional[str] = None,
-        fields: Optional[List[str]] = None,
-        sortby: Optional[str] = None,
-        intersects: Optional[str] = None,
         **kwargs,
-    ) -> stac_types.ItemCollection:
+    ) -> stac.ItemCollection:
         """Cross catalog search (GET).
 
         Called with `GET /search`.
 
         Returns:
             ItemCollection containing items which match the search criteria.
         """
         ...
 
     @abc.abstractmethod
-    def get_item(self, item_id: str, collection_id: str, **kwargs) -> stac_types.Item:
+    def get_item(self, item_id: str, collection_id: str, **kwargs) -> stac.Item:
         """Get item by id.
 
         Called with `GET /collections/{collection_id}/items/{item_id}`.
 
         Args:
             item_id: Id of the item.
             collection_id: Id of the collection.
 
         Returns:
             Item.
         """
         ...
 
     @abc.abstractmethod
-    def all_collections(self, **kwargs) -> stac_types.Collections:
+    def all_collections(self, **kwargs) -> stac.Collections:
         """Get all available collections.
 
         Called with `GET /collections`.
 
         Returns:
             A list of collections.
         """
         ...
 
     @abc.abstractmethod
-    def get_collection(self, collection_id: str, **kwargs) -> stac_types.Collection:
+    def get_collection(self, collection_id: str, **kwargs) -> stac.Collection:
         """Get collection by id.
 
         Called with `GET /collections/{collection_id}`.
 
         Args:
             collection_id: Id of the collection.
 
@@ -515,15 +516,15 @@
         self,
         collection_id: str,
         bbox: Optional[BBox] = None,
         datetime: Optional[DateTimeType] = None,
         limit: int = 10,
         token: str = None,
         **kwargs,
-    ) -> stac_types.ItemCollection:
+    ) -> stac.ItemCollection:
         """Get all items from a specific collection.
 
         Called with `GET /collections/{collection_id}/items`
 
         Args:
             collection_id: id of the collection.
             limit: number of items to return.
@@ -560,24 +561,25 @@
 
         return list(set(conformance_classes))
 
     def extension_is_enabled(self, extension: str) -> bool:
         """Check if an api extension is enabled."""
         return any([type(ext).__name__ == extension for ext in self.extensions])
 
-    async def landing_page(self, **kwargs) -> stac_types.LandingPage:
+    async def landing_page(self, **kwargs) -> stac.LandingPage:
         """Landing page.
 
         Called with `GET /`.
 
         Returns:
             API landing page, serving as an entry point to the API.
         """
         request: Request = kwargs["request"]
         base_url = get_base_url(request)
+
         landing_page = self._landing_page(
             base_url=base_url,
             conformance_classes=self.conformance_classes(),
             extension_schemas=[],
         )
 
         # Add Queryables link
@@ -592,60 +594,61 @@
                     "href": urljoin(base_url, "queryables"),
                     "method": "GET",
                 }
             )
 
         # Add Collections links
         collections = await self.all_collections(request=kwargs["request"])
+
         for collection in collections["collections"]:
             landing_page["links"].append(
                 {
                     "rel": Relations.child.value,
                     "type": MimeTypes.json.value,
                     "title": collection.get("title") or collection.get("id"),
                     "href": urljoin(base_url, f"collections/{collection['id']}"),
                 }
             )
 
         # Add OpenAPI URL
         landing_page["links"].append(
             {
-                "rel": "service-desc",
-                "type": "application/vnd.oai.openapi+json;version=3.0",
+                "rel": Relations.service_desc.value,
+                "type": MimeTypes.openapi.value,
                 "title": "OpenAPI service description",
                 "href": str(request.url_for("openapi")),
             }
         )
 
         # Add human readable service-doc
         landing_page["links"].append(
             {
-                "rel": "service-doc",
-                "type": "text/html",
+                "rel": Relations.service_doc.value,
+                "type": MimeTypes.html.value,
                 "title": "OpenAPI service documentation",
                 "href": str(request.url_for("swagger_ui_html")),
             }
         )
 
-        return landing_page
+        return stac.LandingPage(**landing_page)
 
-    async def conformance(self, **kwargs) -> stac_types.Conformance:
+    async def conformance(self, **kwargs) -> stac.Conformance:
         """Conformance classes.
 
         Called with `GET /conformance`.
 
         Returns:
             Conformance classes which the server conforms to.
         """
-        return Conformance(conformsTo=self.conformance_classes())
+        return stac.Conformance(conformsTo=self.conformance_classes())
 
     @abc.abstractmethod
     async def post_search(
         self, search_request: BaseSearchPostRequest, **kwargs
-    ) -> stac_types.ItemCollection:
+    ) -> stac.ItemCollection:
         """Cross catalog search (POST).
 
         Called with `POST /search`.
 
         Args:
             search_request: search request parameters.
 
@@ -656,64 +659,56 @@
 
     @abc.abstractmethod
     async def get_search(
         self,
         collections: Optional[List[str]] = None,
         ids: Optional[List[str]] = None,
         bbox: Optional[BBox] = None,
+        intersects: Optional[Geometry] = None,
         datetime: Optional[DateTimeType] = None,
         limit: Optional[int] = 10,
-        query: Optional[str] = None,
-        token: Optional[str] = None,
-        fields: Optional[List[str]] = None,
-        sortby: Optional[str] = None,
-        intersects: Optional[str] = None,
         **kwargs,
-    ) -> stac_types.ItemCollection:
+    ) -> stac.ItemCollection:
         """Cross catalog search (GET).
 
         Called with `GET /search`.
 
         Returns:
             ItemCollection containing items which match the search criteria.
         """
         ...
 
     @abc.abstractmethod
-    async def get_item(
-        self, item_id: str, collection_id: str, **kwargs
-    ) -> stac_types.Item:
+    async def get_item(self, item_id: str, collection_id: str, **kwargs) -> stac.Item:
         """Get item by id.
 
         Called with `GET /collections/{collection_id}/items/{item_id}`.
 
         Args:
             item_id: Id of the item.
             collection_id: Id of the collection.
 
         Returns:
             Item.
         """
         ...
 
     @abc.abstractmethod
-    async def all_collections(self, **kwargs) -> stac_types.Collections:
+    async def all_collections(self, **kwargs) -> stac.Collections:
         """Get all available collections.
 
         Called with `GET /collections`.
 
         Returns:
             A list of collections.
         """
         ...
 
     @abc.abstractmethod
-    async def get_collection(
-        self, collection_id: str, **kwargs
-    ) -> stac_types.Collection:
+    async def get_collection(self, collection_id: str, **kwargs) -> stac.Collection:
         """Get collection by id.
 
         Called with `GET /collections/{collection_id}`.
 
         Args:
             collection_id: Id of the collection.
 
@@ -727,15 +722,15 @@
         self,
         collection_id: str,
         bbox: Optional[BBox] = None,
         datetime: Optional[DateTimeType] = None,
         limit: int = 10,
         token: str = None,
         **kwargs,
-    ) -> stac_types.ItemCollection:
+    ) -> stac.ItemCollection:
         """Get all items from a specific collection.
 
         Called with `GET /collections/{collection_id}/items`
 
         Args:
             collection_id: id of the collection.
             limit: number of items to return.
```

### Comparing `stac_fastapi_types-2.5.5.post1/stac_fastapi/types/errors.py` & `stac_fastapi_types-3.0.0a0/stac_fastapi/types/errors.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.5.post1/stac_fastapi/types/extension.py` & `stac_fastapi_types-3.0.0a0/stac_fastapi/types/extension.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base api extension."""
+
 import abc
 from typing import List, Optional
 
 import attr
 from fastapi import FastAPI
 from pydantic import BaseModel
```

### Comparing `stac_fastapi_types-2.5.5.post1/stac_fastapi/types/links.py` & `stac_fastapi_types-3.0.0a0/stac_fastapi/types/links.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.5.post1/stac_fastapi/types/rfc3339.py` & `stac_fastapi_types-3.0.0a0/stac_fastapi/types/rfc3339.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """rfc3339."""
+
 import re
 from datetime import datetime, timezone
 from typing import Optional, Tuple, Union
 
 import iso8601
 from fastapi import HTTPException
 from pystac.utils import datetime_to_str
```

### Comparing `stac_fastapi_types-2.5.5.post1/stac_fastapi/types/stac.py` & `stac_fastapi_types-3.0.0a0/stac_fastapi/types/stac.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,48 @@
 """STAC types."""
+
 import sys
 from typing import Any, Dict, List, Literal, Optional, Union
 
 from stac_pydantic.shared import BBox
 
 # Avoids a Pydantic error:
 # TypeError: You should use `typing_extensions.TypedDict` instead of
-# `typing.TypedDict` with Python < 3.9.2.  Without it, there is no way to
+# `typing.TypedDict` with Python < 3.12.0.  Without it, there is no way to
 # differentiate required and optional fields when subclassed.
-if sys.version_info < (3, 9, 2):
+if sys.version_info < (3, 12, 0):
     from typing_extensions import TypedDict
 else:
     from typing import TypedDict
 
 NumType = Union[float, int]
 
 
-class LandingPage(TypedDict, total=False):
-    """STAC Landing Page."""
+class Catalog(TypedDict, total=False):
+    """STAC Catalog."""
 
     type: str
     stac_version: str
     stac_extensions: Optional[List[str]]
     id: str
-    title: str
+    title: Optional[str]
     description: str
-    conformsTo: List[str]
     links: List[Dict[str, Any]]
 
 
-class Conformance(TypedDict):
-    """STAC Conformance Classes."""
+class LandingPage(Catalog, total=False):
+    """STAC Landing Page."""
 
     conformsTo: List[str]
 
 
-class Catalog(TypedDict, total=False):
-    """STAC Catalog."""
+class Conformance(TypedDict):
+    """STAC Conformance Classes."""
 
-    type: str
-    stac_version: str
-    stac_extensions: Optional[List[str]]
-    id: str
-    title: Optional[str]
-    description: str
-    links: List[Dict[str, Any]]
+    conformsTo: List[str]
 
 
 class Collection(Catalog, total=False):
     """STAC Collection."""
 
     keywords: List[str]
     license: str
@@ -80,13 +74,12 @@
     features: List[Item]
     links: List[Dict[str, Any]]
     context: Optional[Dict[str, int]]
 
 
 class Collections(TypedDict, total=False):
     """All collections endpoint.
-
     https://github.com/radiantearth/stac-api-spec/tree/master/collections
     """
 
     collections: List[Collection]
     links: List[Dict[str, Any]]
```

### Comparing `stac_fastapi_types-2.5.5.post1/stac_fastapi.types.egg-info/PKG-INFO` & `stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.types
-Version: 2.5.5.post1
+Version: 3.0.0a0
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
@@ -14,18 +14,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: fastapi>=0.73.0
-Requires-Dist: attrs
-Requires-Dist: pydantic[dotenv]<2
-Requires-Dist: stac_pydantic==2.0.*
+Requires-Dist: fastapi>=0.100.0
+Requires-Dist: attrs>=23.2.0
+Requires-Dist: pydantic-settings>=2
+Requires-Dist: stac_pydantic>=3
 Requires-Dist: pystac==1.*
 Requires-Dist: iso8601<2.2.0,>=1.0.2
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
```

### Comparing `stac_fastapi_types-2.5.5.post1/stac_fastapi.types.egg-info/SOURCES.txt` & `stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.5.post1/tests/test_limit.py` & `stac_fastapi_types-3.0.0a0/tests/test_limit.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-2.5.5.post1/tests/test_rfc3339.py` & `stac_fastapi_types-3.0.0a0/tests/test_rfc3339.py`

 * *Files identical despite different names*

