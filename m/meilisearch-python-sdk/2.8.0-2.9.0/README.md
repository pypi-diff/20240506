# Comparing `tmp/meilisearch_python_sdk-2.8.0.tar.gz` & `tmp/meilisearch_python_sdk-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_python_sdk-2.8.0.tar", max compression
+gzip compressed data, was "meilisearch_python_sdk-2.9.0.tar", max compression
```

## Comparing `meilisearch_python_sdk-2.8.0.tar` & `meilisearch_python_sdk-2.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2024-03-11 11:32:21.956439 meilisearch_python_sdk-2.8.0/LICENSE
--rw-r--r--   0        0        0     7151 2024-03-11 11:32:21.956439 meilisearch_python_sdk-2.8.0/README.md
--rw-r--r--   0        0        0      258 2024-03-11 11:32:21.960439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/__init__.py
--rw-r--r--   0        0        0    65791 2024-03-11 11:32:21.960439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/_client.py
--rw-r--r--   0        0        0     6021 2024-03-11 11:32:21.960439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/_http_requests.py
--rw-r--r--   0        0        0    11874 2024-03-11 11:32:21.960439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/_task.py
--rw-r--r--   0        0        0     1610 2024-03-11 11:32:21.960439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/_utils.py
--rw-r--r--   0        0        0       18 2024-03-11 11:32:21.960439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/_version.py
--rw-r--r--   0        0        0     8345 2024-03-11 11:32:21.960439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/decorators.py
--rw-r--r--   0        0        0     2085 2024-03-11 11:32:21.960439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/errors.py
--rw-r--r--   0        0        0   297440 2024-03-11 11:32:21.960439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/index.py
--rw-r--r--   0        0        0        0 2024-03-11 11:32:21.960439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/models/__init__.py
--rw-r--r--   0        0        0     5570 2024-03-11 11:32:21.960439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/models/client.py
--rw-r--r--   0        0        0      236 2024-03-11 11:32:21.964439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/models/documents.py
--rw-r--r--   0        0        0       95 2024-03-11 11:32:21.964439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/models/health.py
--rw-r--r--   0        0        0     2044 2024-03-11 11:32:21.964439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/models/index.py
--rw-r--r--   0        0        0     1854 2024-03-11 11:32:21.964439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/models/search.py
--rw-r--r--   0        0        0     3717 2024-03-11 11:32:21.964439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/models/settings.py
--rw-r--r--   0        0        0     3697 2024-03-11 11:32:21.964439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/models/task.py
--rw-r--r--   0        0        0      215 2024-03-11 11:32:21.964439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/models/version.py
--rw-r--r--   0        0        0     3515 2024-03-11 11:32:21.964439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/plugins.py
--rw-r--r--   0        0        0        0 2024-03-11 11:32:21.964439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/py.typed
--rw-r--r--   0        0        0      173 2024-03-11 11:32:21.964439 meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/types.py
--rw-r--r--   0        0        0     2405 2024-03-11 11:32:21.964439 meilisearch_python_sdk-2.8.0/pyproject.toml
--rw-r--r--   0        0        0     8396 1970-01-01 00:00:00.000000 meilisearch_python_sdk-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-06 09:09:41.791484 meilisearch_python_sdk-2.9.0/LICENSE
+-rw-r--r--   0        0        0     7019 2024-05-06 09:09:41.791484 meilisearch_python_sdk-2.9.0/README.md
+-rw-r--r--   0        0        0      258 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/__init__.py
+-rw-r--r--   0        0        0    66791 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/_client.py
+-rw-r--r--   0        0        0     6039 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/_http_requests.py
+-rw-r--r--   0        0        0    11874 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/_task.py
+-rw-r--r--   0        0        0     1610 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/_utils.py
+-rw-r--r--   0        0        0       18 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/_version.py
+-rw-r--r--   0        0        0     8346 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/decorators.py
+-rw-r--r--   0        0        0     2085 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/errors.py
+-rw-r--r--   0        0        0   305399 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/index.py
+-rw-r--r--   0        0        0        0 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/models/__init__.py
+-rw-r--r--   0        0        0     5700 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/models/client.py
+-rw-r--r--   0        0        0      236 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/models/documents.py
+-rw-r--r--   0        0        0       95 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/models/health.py
+-rw-r--r--   0        0        0     2070 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/models/index.py
+-rw-r--r--   0        0        0     1858 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/models/search.py
+-rw-r--r--   0        0        0     4879 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/models/settings.py
+-rw-r--r--   0        0        0     3749 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/models/task.py
+-rw-r--r--   0        0        0      215 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/models/version.py
+-rw-r--r--   0        0        0     3580 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/plugins.py
+-rw-r--r--   0        0        0        0 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/py.typed
+-rw-r--r--   0        0        0      173 2024-05-06 09:09:41.795484 meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/types.py
+-rw-r--r--   0        0        0     2410 2024-05-06 09:09:41.799484 meilisearch_python_sdk-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8264 1970-01-01 00:00:00.000000 meilisearch_python_sdk-2.9.0/PKG-INFO
```

### Comparing `meilisearch_python_sdk-2.8.0/LICENSE` & `meilisearch_python_sdk-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_python_sdk-2.8.0/README.md` & `meilisearch_python_sdk-2.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 
 [![Tests Status](https://github.com/sanders41/meilisearch-python-sdk/workflows/Testing/badge.svg?branch=main&event=push)](https://github.com/sanders41/meilisearch-python-sdk/actions?query=workflow%3ATesting+branch%3Amain+event%3Apush)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sanders41/meilisearch-python-sdk/main.svg)](https://results.pre-commit.ci/latest/github/sanders41/meilisearch-python-sdk/main)
 [![Coverage](https://codecov.io/github/sanders41/meilisearch-python-sdk/coverage.svg?branch=main)](https://codecov.io/gh/sanders41/meilisearch-python-sdk)
 [![PyPI version](https://badge.fury.io/py/meilisearch-python-sdk.svg)](https://badge.fury.io/py/meilisearch-python-sdk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/meilisearch-python-sdk?color=5cc141)](https://github.com/sanders41/meilisearch-python-sdk)
 
-NOTE: This project was previously named `meilisearch-python-async`. Development on
-that project continues here under the new name.
-
 Meilisearch Python SDK provides both an async and sync client for the
 [Meilisearch](https://github.com/meilisearch/meilisearch) API.
 
 Which client to use depends on your use case. If the code base you are working with uses asyncio,
 for example if you are using [FastAPI](https://fastapi.tiangolo.com/), choose the `AsyncClient`,
 otherwise choose the sync `Client`. The functionality of the two clients is the same, the difference
 being that the `AsyncClient` provides async methods and uses the `AsyncIndex` with its own
```

### Comparing `meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/_client.py` & `meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,15 @@
     async def create_index(
         self,
         uid: str,
         primary_key: str | None = None,
         *,
         settings: MeilisearchSettings | None = None,
         wait: bool = True,
+        timeout_in_ms: int | None = None,
         plugins: AsyncIndexPlugins | None = None,
     ) -> AsyncIndex:
         """Creates a new index.
 
         Args:
 
             uid: The index's unique identifier.
@@ -206,14 +207,17 @@
                 creating the index. The advantage to updating them here is updating the settings after
                 adding documents will cause the documents to be re-indexed. Because of this it will be
                 faster to update them before adding documents. Defaults to None (i.e. default
                 Meilisearch index settings).
             wait: If set to True and settings are being updated, the index will be returned after
                 the settings update has completed. If False it will not wait for settings to complete.
                 Default: True
+            timeout_in_ms: Amount of time in milliseconds to wait before raising a
+                MeilisearchTimeoutError. `None` can also be passed to wait indefinitely. Be aware that
+                if the `None` option is used the wait time could be very long. Defaults to None.
             plugins: Optional plugins can be provided to extend functionality.
 
         Returns:
 
             An instance of AsyncIndex containing the information of the newly created index.
 
         Raises:
@@ -224,15 +228,21 @@
         Examples:
 
             >>> from meilisearch_python_sdk import AsyncClient
             >>> async with AsyncClient("http://localhost.com", "masterKey") as client:
             >>>     index = await client.create_index("movies")
         """
         return await AsyncIndex.create(
-            self.http_client, uid, primary_key, settings=settings, wait=wait, plugins=plugins
+            self.http_client,
+            uid,
+            primary_key,
+            settings=settings,
+            wait=wait,
+            timeout_in_ms=timeout_in_ms,
+            plugins=plugins,
         )
 
     async def create_snapshot(self) -> TaskInfo:
         """Trigger the creation of a Meilisearch snapshot.
 
         Returns:
 
@@ -466,14 +476,15 @@
             response = await self._http_requests.post(
                 "keys", json.loads(key.model_dump_json(by_alias=True))
             )  # type: ignore[attr-defined]
         else:  # pragma: no cover
             warn(
                 "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
                 DeprecationWarning,
+                stacklevel=2,
             )
             response = await self._http_requests.post("keys", json.loads(key.json(by_alias=True)))  # type: ignore[attr-defined]
 
         return Key(**response.json())
 
     async def delete_key(self, key: str) -> int:
         """Deletes an API key.
@@ -621,14 +632,15 @@
                 url,
                 body={"queries": [x.model_dump(by_alias=True) for x in queries]},  # type: ignore[attr-defined]
             )
         else:  # pragma: no cover
             warn(
                 "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
                 DeprecationWarning,
+                stacklevel=2,
             )
             response = await self._http_requests.post(
                 url,
                 body={"queries": [x.dict(by_alias=True) for x in queries]},  # type: ignore[attr-defined]
             )
 
         return [SearchResultsWithUID(**x) for x in response.json()["results"]]
@@ -866,22 +878,22 @@
     ) -> TaskInfo:
         """Delete a list of tasks.
 
         Defaults to deleting all tasks.
 
         Args:
 
-            uids: A list of task UIDs to cancel.
-            index_uids: A list of index UIDs for which to cancel tasks.
-            statuses: A list of statuses to cancel.
-            types: A list of types to cancel.
-            before_enqueued_at: Cancel tasks that were enqueued before the specified date time.
-            after_enqueued_at: Cancel tasks that were enqueued after the specified date time.
-            before_started_at: Cancel tasks that were started before the specified date time.
-            after_finished_at: Cancel tasks that were finished after the specified date time.
+            uids: A list of task UIDs to delete.
+            index_uids: A list of index UIDs for which to delete tasks.
+            statuses: A list of statuses to delete.
+            types: A list of types to delete.
+            before_enqueued_at: Delete tasks that were enqueued before the specified date time.
+            after_enqueued_at: Delete tasks that were enqueued after the specified date time.
+            before_started_at: Delete tasks that were started before the specified date time.
+            after_finished_at: Delete tasks that were finished after the specified date time.
 
         Returns:
 
             The details of the task
 
         Raises:
 
@@ -1049,14 +1061,15 @@
     def create_index(
         self,
         uid: str,
         primary_key: str | None = None,
         *,
         settings: MeilisearchSettings | None = None,
         wait: bool = True,
+        timeout_in_ms: int | None = None,
         plugins: IndexPlugins | None = None,
     ) -> Index:
         """Creates a new index.
 
         Args:
 
             uid: The index's unique identifier.
@@ -1065,14 +1078,17 @@
                 creating the index. The advantage to updating them here is updating the settings after
                 adding documents will cause the documents to be re-indexed. Because of this it will be
                 faster to update them before adding documents. Defaults to None (i.e. default
                 Meilisearch index settings).
             wait: If set to True and settings are being updated, the index will be returned after
                 the settings update has completed. If False it will not wait for settings to complete.
                 Default: True
+            timeout_in_ms: Amount of time in milliseconds to wait before raising a
+                MeilisearchTimeoutError. `None` can also be passed to wait indefinitely. Be aware that
+                if the `None` option is used the wait time could be very long. Defaults to None.
             plugins: Optional plugins can be provided to extend functionality.
 
         Returns:
 
             An instance of Index containing the information of the newly created index.
 
         Raises:
@@ -1083,15 +1099,21 @@
         Examples:
 
             >>> from meilisearch_python_sdk import Client
             >>> client = Client("http://localhost.com", "masterKey")
             >>> index = client.create_index("movies")
         """
         return Index.create(
-            self.http_client, uid, primary_key, settings=settings, wait=wait, plugins=plugins
+            self.http_client,
+            uid,
+            primary_key,
+            settings=settings,
+            wait=wait,
+            timeout_in_ms=timeout_in_ms,
+            plugins=plugins,
         )
 
     def create_snapshot(self) -> TaskInfo:
         """Trigger the creation of a Meilisearch snapshot.
 
         Returns:
 
@@ -1323,14 +1345,15 @@
             response = self._http_requests.post(
                 "keys", json.loads(key.model_dump_json(by_alias=True))
             )  # type: ignore[attr-defined]
         else:  # pragma: no cover
             warn(
                 "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
                 DeprecationWarning,
+                stacklevel=2,
             )
             response = self._http_requests.post("keys", json.loads(key.json(by_alias=True)))  # type: ignore[attr-defined]
 
         return Key(**response.json())
 
     def delete_key(self, key: str) -> int:
         """Deletes an API key.
@@ -1478,14 +1501,15 @@
                 url,
                 body={"queries": [x.model_dump(by_alias=True) for x in queries]},  # type: ignore[attr-defined]
             )
         else:  # pragma: no cover
             warn(
                 "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
                 DeprecationWarning,
+                stacklevel=2,
             )
             response = self._http_requests.post(
                 url,
                 body={"queries": [x.dict(by_alias=True) for x in queries]},  # type: ignore[attr-defined]
             )
 
         return [SearchResultsWithUID(**x) for x in response.json()["results"]]
@@ -1697,22 +1721,22 @@
     ) -> TaskInfo:
         """Delete a list of tasks.
 
         Defaults to deleting all tasks.
 
         Args:
 
-            uids: A list of task UIDs to cancel.
-            index_uids: A list of index UIDs for which to cancel tasks.
-            statuses: A list of statuses to cancel.
-            types: A list of types to cancel.
-            before_enqueued_at: Cancel tasks that were enqueued before the specified date time.
-            after_enqueued_at: Cancel tasks that were enqueued after the specified date time.
-            before_started_at: Cancel tasks that were started before the specified date time.
-            after_finished_at: Cancel tasks that were finished after the specified date time.
+            uids: A list of task UIDs to delete.
+            index_uids: A list of index UIDs for which to delete tasks.
+            statuses: A list of statuses to delete.
+            types: A list of types to delete.
+            before_enqueued_at: Delete tasks that were enqueued before the specified date time.
+            after_enqueued_at: Delete tasks that were enqueued after the specified date time.
+            before_started_at: Delete tasks that were started before the specified date time.
+            after_finished_at: Delete tasks that were finished after the specified date time.
 
         Returns:
 
             The details of the task
 
         Raises:
 
@@ -1871,13 +1895,14 @@
             for k, v in json.loads(key.model_dump_json(by_alias=True)).items()
             if v is not None and k != "key"
         }
     else:  # pragma: no cover
         warn(
             "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
             DeprecationWarning,
+            stacklevel=2,
         )
         return {  # type: ignore[attr-defined]
             k: v
             for k, v in json.loads(key.json(by_alias=True)).items()
             if v is not None and k != "key"
         }
```

### Comparing `meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/_http_requests.py` & `meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/_http_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         except (ConnectError, ConnectTimeout, RemoteProtocolError) as err:
             raise MeilisearchCommunicationError(str(err)) from err
         except HTTPError as err:
             if "response" in locals():
                 raise MeilisearchApiError(str(err), response) from err
             else:
                 # Fail safe just in case error happens before response is created
-                raise MeilisearchError(str(err))  # pragma: no cover
+                raise MeilisearchError(str(err)) from err  # pragma: no cover
 
     async def get(self, path: str) -> Response:
         return await self._send_request(self.http_client.get, path)
 
     async def patch(
         self,
         path: str,
@@ -128,15 +128,15 @@
         except (ConnectError, ConnectTimeout, RemoteProtocolError) as err:
             raise MeilisearchCommunicationError(str(err)) from err
         except HTTPError as err:
             if "response" in locals():
                 raise MeilisearchApiError(str(err), response) from err
             else:
                 # Fail safe just in case error happens before response is created
-                raise MeilisearchError(str(err))  # pragma: no cover
+                raise MeilisearchError(str(err)) from err  # pragma: no cover
 
     def get(self, path: str) -> Response:
         return self._send_request(self.http_client.get, path)
 
     def patch(
         self,
         path: str,
```

### Comparing `meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/_task.py` & `meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/_task.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/_utils.py` & `meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/_utils.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/decorators.py` & `meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         >>> @async_add_documents(index_name="movies", connection_info=client)
         >>> async def my_function() -> list[dict[str, Any]]:
         >>>     return [{"id": 1, "title": "Test 1"}, {"id": 2, "title": "Test 2"}]
         >>>
         >>> # with `ConnectionInfo`
         >>> @async_add_documents(
                 index_name="movies",
-                connection_info=ConnectionInfo(url="http://localhost:7700", api_key="masterKey",
+                connection_info=ConnectionInfo(url="http://localhost:7700", api_key="masterKey"),
             )
         >>> async def my_function() -> list[dict[str, Any]]:
         >>>     return [{"id": 1, "title": "Test 1"}, {"id": 2, "title": "Test 2"}]
     """
 
     def decorator(func: Callable) -> Callable:
         @wraps(func)
```

### Comparing `meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/errors.py` & `meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/index.py` & `meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/index.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import asyncio
 import json
 from csv import DictReader
 from datetime import datetime
 from functools import cached_property, partial
 from pathlib import Path
-from typing import Any, Generator, MutableMapping, Sequence
+from typing import TYPE_CHECKING, Any, Generator, MutableMapping, Sequence
 from urllib.parse import urlencode
 from warnings import warn
 
 import aiofiles
 from camel_converter import to_snake
 from httpx import AsyncClient, Client
 
@@ -22,17 +22,19 @@
 from meilisearch_python_sdk.models.index import IndexStats
 from meilisearch_python_sdk.models.search import FacetSearchResults, Hybrid, SearchResults
 from meilisearch_python_sdk.models.settings import (
     Embedders,
     Faceting,
     HuggingFaceEmbedder,
     MeilisearchSettings,
+    OllamaEmbedder,
     OpenAiEmbedder,
     Pagination,
     ProximityPrecision,
+    RestEmbedder,
     TypoTolerance,
     UserProvidedEmbedder,
 )
 from meilisearch_python_sdk.models.task import TaskInfo
 from meilisearch_python_sdk.plugins import (
     AsyncDocumentPlugin,
     AsyncEvent,
@@ -41,15 +43,17 @@
     AsyncPostSearchPlugin,
     DocumentPlugin,
     Event,
     IndexPlugins,
     Plugin,
     PostSearchPlugin,
 )
-from meilisearch_python_sdk.types import Filter, JsonDict, JsonMapping
+
+if TYPE_CHECKING:  # pragma: no cover
+    from meilisearch_python_sdk.types import Filter, JsonDict, JsonMapping
 
 
 class _BaseIndex:
     def __init__(
         self,
         uid: str,
         primary_key: str | None = None,
@@ -609,14 +613,15 @@
         cls,
         http_client: AsyncClient,
         uid: str,
         primary_key: str | None = None,
         *,
         settings: MeilisearchSettings | None = None,
         wait: bool = True,
+        timeout_in_ms: int | None = None,
         plugins: AsyncIndexPlugins | None = None,
     ) -> AsyncIndex:
         """Creates a new index.
 
         In general this method should not be used directly and instead the index should be created
         through the `Client`.
 
@@ -630,14 +635,17 @@
                 creating the index. The advantage to updating them here is updating the settings after
                 adding documents will cause the documents to be re-indexed. Because of this it will be
                 faster to update them before adding documents. Defaults to None (i.e. default
                 Meilisearch index settings).
             wait: If set to True and settings are being updated, the index will be returned after
                 the settings update has completed. If False it will not wait for settings to complete.
                 Default: True
+            timeout_in_ms: Amount of time in milliseconds to wait before raising a
+                MeilisearchTimeoutError. `None` can also be passed to wait indefinitely. Be aware that
+                if the `None` option is used the wait time could be very long. Defaults to None.
             plugins: Optional plugins can be provided to extend functionality.
 
         Returns:
 
             An instance of AsyncIndex containing the information of the newly created index.
 
         Raises:
@@ -655,15 +663,17 @@
             payload = {"uid": uid}
         else:
             payload = {"primaryKey": primary_key, "uid": uid}
 
         url = "indexes"
         http_request = AsyncHttpRequests(http_client)
         response = await http_request.post(url, payload)
-        await async_wait_for_task(http_client, response.json()["taskUid"], timeout_in_ms=None)
+        await async_wait_for_task(
+            http_client, response.json()["taskUid"], timeout_in_ms=timeout_in_ms
+        )
 
         index_response = await http_request.get(f"{url}/{uid}")
         index_dict = index_response.json()
         index = cls(
             http_client=http_client,
             uid=index_dict["uid"],
             primary_key=index_dict["primaryKey"],
@@ -671,15 +681,17 @@
             updated_at=index_dict["updatedAt"],
             plugins=plugins,
         )
 
         if settings:
             settings_task = await index.update_settings(settings)
             if wait:
-                await async_wait_for_task(http_client, settings_task.task_uid, timeout_in_ms=None)
+                await async_wait_for_task(
+                    http_client, settings_task.task_uid, timeout_in_ms=timeout_in_ms
+                )
 
         return index
 
     async def get_stats(self) -> IndexStats:
         """Get stats of the index.
 
         Returns:
@@ -706,15 +718,15 @@
         self,
         query: str | None = None,
         *,
         offset: int = 0,
         limit: int = 20,
         filter: Filter | None = None,
         facets: list[str] | None = None,
-        attributes_to_retrieve: list[str] = ["*"],
+        attributes_to_retrieve: list[str] | None = None,
         attributes_to_crop: list[str] | None = None,
         crop_length: int = 200,
         attributes_to_highlight: list[str] | None = None,
         sort: list[str] | None = None,
         show_matches_position: bool = False,
         highlight_pre_tag: str = "<em>",
         highlight_post_tag: str = "</em>",
@@ -792,15 +804,14 @@
         Examples:
 
             >>> from meilisearch_python_sdk import AsyncClient
             >>> async with AsyncClient("http://localhost.com", "masterKey") as client:
             >>>     index = client.index("movies")
             >>>     search_results = await index.search("Tron")
         """
-
         body = _process_search_parameters(
             q=query,
             offset=offset,
             limit=limit,
             filter=filter,
             facets=facets,
             attributes_to_retrieve=attributes_to_retrieve,
@@ -957,15 +968,15 @@
         *,
         facet_name: str,
         facet_query: str,
         offset: int = 0,
         limit: int = 20,
         filter: Filter | None = None,
         facets: list[str] | None = None,
-        attributes_to_retrieve: list[str] = ["*"],
+        attributes_to_retrieve: list[str] | None = None,
         attributes_to_crop: list[str] | None = None,
         crop_length: int = 200,
         attributes_to_highlight: list[str] | None = None,
         sort: list[str] | None = None,
         show_matches_position: bool = False,
         highlight_pre_tag: str = "<em>",
         highlight_post_tag: str = "</em>",
@@ -2805,15 +2816,18 @@
             >>>     settings = await index.get_settings()
         """
         response = await self._http_requests.get(self._settings_url)
         response_json = response.json()
         settings = MeilisearchSettings(**response_json)
 
         if response_json.get("embedders"):
-            settings.embedders = _embedder_json_to_settings_model(response_json["embedders"])
+            # TODO: Add back after embedder setting issue fixed https://github.com/meilisearch/meilisearch/issues/4585
+            settings.embedders = _embedder_json_to_settings_model(  # pragma: no cover
+                response_json["embedders"]
+            )
 
         return settings
 
     async def update_settings(
         self, body: MeilisearchSettings, *, compress: bool = False
     ) -> TaskInfo:
         """Update settings of the index.
@@ -2861,14 +2875,15 @@
         """
         if is_pydantic_2():
             body_dict = {k: v for k, v in body.model_dump(by_alias=True).items() if v is not None}  # type: ignore[attr-defined]
         else:  # pragma: no cover
             warn(
                 "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
                 DeprecationWarning,
+                stacklevel=2,
             )
             body_dict = {k: v for k, v in body.dict(by_alias=True).items() if v is not None}  # type: ignore[attr-defined]
 
         response = await self._http_requests.patch(self._settings_url, body_dict, compress=compress)
 
         return TaskInfo(**response.json())
 
@@ -3002,15 +3017,15 @@
             >>> async with AsyncClient("http://localhost.com", "masterKey") as client:
             >>>     index = client.index("movies")
             >>>     distinct_attribute = await index.get_distinct_attribute()
         """
         response = await self._http_requests.get(f"{self._settings_url}/distinct-attribute")
 
         if not response.json():
-            None
+            return None
 
         return response.json()
 
     async def update_distinct_attribute(self, body: str, *, compress: bool = False) -> TaskInfo:
         """Update distinct attribute of the index.
 
         Args:
@@ -3598,14 +3613,15 @@
                 typo_tolerance.model_dump(by_alias=True),
                 compress=compress,
             )  # type: ignore[attr-defined]
         else:  # pragma: no cover
             warn(
                 "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
                 DeprecationWarning,
+                stacklevel=2,
             )
             response = await self._http_requests.patch(
                 f"{self._settings_url}/typo-tolerance",
                 typo_tolerance.dict(by_alias=True),
                 compress=compress,
             )  # type: ignore[attr-defined]
 
@@ -3687,14 +3703,15 @@
                 faceting.model_dump(by_alias=True),
                 compress=compress,
             )  # type: ignore[attr-defined]
         else:  # pragma: no cover
             warn(
                 "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
                 DeprecationWarning,
+                stacklevel=2,
             )
             response = await self._http_requests.patch(
                 f"{self._settings_url}/faceting", faceting.dict(by_alias=True), compress=compress
             )  # type: ignore[attr-defined]
 
         return TaskInfo(**response.json())
 
@@ -3775,14 +3792,15 @@
                 settings.model_dump(by_alias=True),
                 compress=compress,
             )  # type: ignore[attr-defined]
         else:  # pragma: no cover
             warn(
                 "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
                 DeprecationWarning,
+                stacklevel=2,
             )
             response = await self._http_requests.patch(
                 f"{self._settings_url}/pagination", settings.dict(by_alias=True), compress=compress
             )  # type: ignore[attr-defined]
 
         return TaskInfo(**response.json())
 
@@ -3961,14 +3979,92 @@
             >>>     index = client.index("movies")
             >>>     await index.reset_non_separator_tokens()
         """
         response = await self._http_requests.delete(f"{self._settings_url}/non-separator-tokens")
 
         return TaskInfo(**response.json())
 
+    async def get_search_cutoff_ms(self) -> int | None:
+        """Get search cutoff time in ms.
+
+        Returns:
+
+            Integer representing the search cutoff time in ms, or None.
+
+        Raises:
+
+            MeilisearchCommunicationError: If there was an error communicating with the server.
+            MeilisearchApiError: If the Meilisearch API returned an error.
+
+        Examples:
+
+            >>> from meilisearch_async_client import AsyncClient
+            >>> async with AsyncClient("http://localhost.com", "masterKey") as client:
+            >>>     index = client.index("movies")
+            >>>     search_cutoff_ms_settings = await index.get_search_cutoff_ms()
+        """
+        response = await self._http_requests.get(f"{self._settings_url}/search-cutoff-ms")
+
+        return response.json()
+
+    async def update_search_cutoff_ms(
+        self, search_cutoff_ms: int, *, compress: bool = False
+    ) -> TaskInfo:
+        """Update the search cutoff for an index.
+
+        Args:
+
+            search_cutoff_ms: Integer value of the search cutoff time in ms.
+            compress: If set to True the data will be sent in gzip format. Defaults to False.
+
+        Returns:
+
+            The details of the task status.
+
+        Raises:
+
+            MeilisearchCommunicationError: If there was an error communicating with the server.
+            MeilisearchApiError: If the Meilisearch API returned an error.
+
+        Examples:
+
+            >>> from meilisearch_python_sdk import AsyncClient
+            >>> async with AsyncClient("http://localhost.com", "masterKey") as client:
+            >>>     index = client.index("movies")
+            >>>     await index.update_search_cutoff_ms(100)
+        """
+        response = await self._http_requests.put(
+            f"{self._settings_url}/search-cutoff-ms", search_cutoff_ms, compress=compress
+        )
+
+        return TaskInfo(**response.json())
+
+    async def reset_search_cutoff_ms(self) -> TaskInfo:
+        """Reset the search cutoff time to the default value.
+
+        Returns:
+
+            The details of the task status.
+
+        Raises:
+
+            MeilisearchCommunicationError: If there was an error communicating with the server.
+            MeilisearchApiError: If the Meilisearch API returned an error.
+
+        Examples:
+
+            >>> from meilisearch_async_client import AsyncClient
+            >>> async with AsyncClient("http://localhost.com", "masterKey") as client:
+            >>>     index = client.index("movies")
+            >>>     await index.reset_search_cutoff_ms()
+        """
+        response = await self._http_requests.delete(f"{self._settings_url}/search-cutoff-ms")
+
+        return TaskInfo(**response.json())
+
     async def get_word_dictionary(self) -> list[str]:
         """Get word dictionary settings for the index.
 
         Returns:
 
             Word dictionary for the index.
 
@@ -4182,26 +4278,28 @@
                 payload[key] = {
                     k: v for k, v in embedder.model_dump(by_alias=True).items() if v is not None
                 }  # type: ignore[attr-defined]
             else:  # pragma: no cover
                 warn(
                     "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
                     DeprecationWarning,
+                    stacklevel=2,
                 )
                 payload[key] = {
                     k: v for k, v in embedder.dict(by_alias=True).items() if v is not None
                 }  # type: ignore[attr-defined]
 
         response = await self._http_requests.patch(
             f"{self._settings_url}/embedders", payload, compress=compress
         )
 
         return TaskInfo(**response.json())
 
-    async def reset_embedders(self) -> TaskInfo:
+    # TODO: Add back after embedder setting issue fixed https://github.com/meilisearch/meilisearch/issues/4585
+    async def reset_embedders(self) -> TaskInfo:  # pragma: no cover
         """Reset an index's embedders settings to the default value.
 
         Returns:
 
             The details of the task status.
 
         Raises:
@@ -4692,14 +4790,15 @@
         cls,
         http_client: Client,
         uid: str,
         primary_key: str | None = None,
         *,
         settings: MeilisearchSettings | None = None,
         wait: bool = True,
+        timeout_in_ms: int | None = None,
         plugins: IndexPlugins | None = None,
     ) -> Index:
         """Creates a new index.
 
         In general this method should not be used directly and instead the index should be created
         through the `Client`.
 
@@ -4713,14 +4812,17 @@
                 creating the index. The advantage to updating them here is updating the settings after
                 adding documents will cause the documents to be re-indexed. Because of this it will be
                 faster to update them before adding documents. Defaults to None (i.e. default
                 Meilisearch index settings).
             wait: If set to True and settings are being updated, the index will be returned after
                 the settings update has completed. If False it will not wait for settings to complete.
                 Default: True
+            timeout_in_ms: Amount of time in milliseconds to wait before raising a
+                MeilisearchTimeoutError. `None` can also be passed to wait indefinitely. Be aware that
+                if the `None` option is used the wait time could be very long. Defaults to None.
             plugins: Optional plugins can be provided to extend functionality.
 
         Returns:
 
             An instance of Index containing the information of the newly created index.
 
         Raises:
@@ -4738,30 +4840,30 @@
             payload = {"uid": uid}
         else:
             payload = {"primaryKey": primary_key, "uid": uid}
 
         url = "indexes"
         http_request = HttpRequests(http_client)
         response = http_request.post(url, payload)
-        wait_for_task(http_client, response.json()["taskUid"], timeout_in_ms=None)
+        wait_for_task(http_client, response.json()["taskUid"], timeout_in_ms=timeout_in_ms)
         index_response = http_request.get(f"{url}/{uid}")
         index_dict = index_response.json()
         index = cls(
             http_client=http_client,
             uid=index_dict["uid"],
             primary_key=index_dict["primaryKey"],
             created_at=index_dict["createdAt"],
             updated_at=index_dict["updatedAt"],
             plugins=plugins,
         )
 
         if settings:
             settings_task = index.update_settings(settings)
             if wait:
-                wait_for_task(http_client, settings_task.task_uid, timeout_in_ms=None)
+                wait_for_task(http_client, settings_task.task_uid, timeout_in_ms=timeout_in_ms)
 
         return index
 
     def get_stats(self) -> IndexStats:
         """Get stats of the index.
 
         Returns:
@@ -4788,15 +4890,15 @@
         self,
         query: str | None = None,
         *,
         offset: int = 0,
         limit: int = 20,
         filter: Filter | None = None,
         facets: list[str] | None = None,
-        attributes_to_retrieve: list[str] = ["*"],
+        attributes_to_retrieve: list[str] | None = None,
         attributes_to_crop: list[str] | None = None,
         crop_length: int = 200,
         attributes_to_highlight: list[str] | None = None,
         sort: list[str] | None = None,
         show_matches_position: bool = False,
         highlight_pre_tag: str = "<em>",
         highlight_post_tag: str = "</em>",
@@ -4946,15 +5048,15 @@
         *,
         facet_name: str,
         facet_query: str,
         offset: int = 0,
         limit: int = 20,
         filter: Filter | None = None,
         facets: list[str] | None = None,
-        attributes_to_retrieve: list[str] = ["*"],
+        attributes_to_retrieve: list[str] | None = None,
         attributes_to_crop: list[str] | None = None,
         crop_length: int = 200,
         attributes_to_highlight: list[str] | None = None,
         sort: list[str] | None = None,
         show_matches_position: bool = False,
         highlight_pre_tag: str = "<em>",
         highlight_post_tag: str = "</em>",
@@ -6235,15 +6337,18 @@
             >>> settings = index.get_settings()
         """
         response = self._http_requests.get(self._settings_url)
         response_json = response.json()
         settings = MeilisearchSettings(**response_json)
 
         if response_json.get("embedders"):
-            settings.embedders = _embedder_json_to_settings_model(response_json["embedders"])
+            # TODO: Add back after embedder setting issue fixed https://github.com/meilisearch/meilisearch/issues/4585
+            settings.embedders = _embedder_json_to_settings_model(  # pragma: no cover
+                response_json["embedders"]
+            )
 
         return settings
 
     def update_settings(self, body: MeilisearchSettings, *, compress: bool = False) -> TaskInfo:
         """Update settings of the index.
 
         Args:
@@ -6289,14 +6394,15 @@
         """
         if is_pydantic_2():
             body_dict = {k: v for k, v in body.model_dump(by_alias=True).items() if v is not None}  # type: ignore[attr-defined]
         else:  # pragma: no cover
             warn(
                 "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
                 DeprecationWarning,
+                stacklevel=2,
             )
             body_dict = {k: v for k, v in body.dict(by_alias=True).items() if v is not None}  # type: ignore[attr-defined]
 
         response = self._http_requests.patch(self._settings_url, body_dict, compress=compress)
 
         return TaskInfo(**response.json())
 
@@ -6428,15 +6534,15 @@
             >>> client = Client("http://localhost.com", "masterKey")
             >>> index = client.index("movies")
             >>> distinct_attribute = index.get_distinct_attribute()
         """
         response = self._http_requests.get(f"{self._settings_url}/distinct-attribute")
 
         if not response.json():
-            None
+            return None
 
         return response.json()
 
     def update_distinct_attribute(self, body: str, *, compress: bool = False) -> TaskInfo:
         """Update distinct attribute of the index.
 
         Args:
@@ -7015,14 +7121,15 @@
                 typo_tolerance.model_dump(by_alias=True),
                 compress=compress,
             )  # type: ignore[attr-defined]
         else:  # pragma: no cover
             warn(
                 "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
                 DeprecationWarning,
+                stacklevel=2,
             )
             response = self._http_requests.patch(
                 f"{self._settings_url}/typo-tolerance",
                 typo_tolerance.dict(by_alias=True),
                 compress=compress,
             )  # type: ignore[attr-defined]
 
@@ -7104,14 +7211,15 @@
                 faceting.model_dump(by_alias=True),
                 compress=compress,
             )  # type: ignore[attr-defined]
         else:  # pragma: no cover
             warn(
                 "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
                 DeprecationWarning,
+                stacklevel=2,
             )
             response = self._http_requests.patch(
                 f"{self._settings_url}/faceting", faceting.dict(by_alias=True), compress=compress
             )  # type: ignore[attr-defined]
 
         return TaskInfo(**response.json())
 
@@ -7192,14 +7300,15 @@
                 settings.model_dump(by_alias=True),
                 compress=compress,
             )  # type: ignore[attr-defined]
         else:  # pragma: no cover
             warn(
                 "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
                 DeprecationWarning,
+                stacklevel=2,
             )
             response = self._http_requests.patch(
                 f"{self._settings_url}/pagination", settings.dict(by_alias=True), compress=compress
             )  # type: ignore[attr-defined]
 
         return TaskInfo(**response.json())
 
@@ -7378,14 +7487,90 @@
             >>> index = client.index("movies")
             >>> index.reset_non_separator_tokens()
         """
         response = self._http_requests.delete(f"{self._settings_url}/non-separator-tokens")
 
         return TaskInfo(**response.json())
 
+    def get_search_cutoff_ms(self) -> int | None:
+        """Get search cutoff time in ms.
+
+        Returns:
+
+            Integer representing the search cutoff time in ms, or None.
+
+        Raises:
+
+            MeilisearchCommunicationError: If there was an error communicating with the server.
+            MeilisearchApiError: If the Meilisearch API returned an error.
+
+        Examples:
+
+            >>> from meilisearch_async_client import Client
+            >>> client = Client("http://localhost.com", "masterKey")
+            >>> index = client.index("movies")
+            >>> search_cutoff_ms_settings = index.get_search_cutoff_ms()
+        """
+        response = self._http_requests.get(f"{self._settings_url}/search-cutoff-ms")
+
+        return response.json()
+
+    def update_search_cutoff_ms(self, search_cutoff_ms: int, *, compress: bool = False) -> TaskInfo:
+        """Update the search cutoff for an index.
+
+        Args:
+
+            search_cutoff_ms: Integer value of the search cutoff time in ms.
+            compress: If set to True the data will be sent in gzip format. Defaults to False.
+
+        Returns:
+
+            Task to track the action.
+
+        Raises:
+
+            MeilisearchCommunicationError: If there was an error communicating with the server.
+            MeilisearchApiError: If the Meilisearch API returned an error.
+
+        Examples:
+
+            >>> from meilisearch_python_sdk import Client
+            >>> client = Client("http://localhost.com", "masterKey")
+            >>> index = client.index("movies")
+            >>> index.update_search_cutoff_ms(100)
+        """
+        response = self._http_requests.put(
+            f"{self._settings_url}/search-cutoff-ms", search_cutoff_ms, compress=compress
+        )
+
+        return TaskInfo(**response.json())
+
+    def reset_search_cutoff_ms(self) -> TaskInfo:
+        """Reset the search cutoff time to the default value.
+
+        Returns:
+
+            The details of the task status.
+
+        Raises:
+
+            MeilisearchCommunicationError: If there was an error communicating with the server.
+            MeilisearchApiError: If the Meilisearch API returned an error.
+
+        Examples:
+
+            >>> from meilisearch_async_client import Client
+            >>> client = Client("http://localhost.com", "masterKey")
+            >>> index = client.index("movies")
+            >>> index.reset_search_cutoff_ms()
+        """
+        response = self._http_requests.delete(f"{self._settings_url}/search-cutoff-ms")
+
+        return TaskInfo(**response.json())
+
     def get_word_dictionary(self) -> list[str]:
         """Get word dictionary settings for the index.
 
         Returns:
 
             Word dictionary for the index.
 
@@ -7595,26 +7780,28 @@
                 payload[key] = {
                     k: v for k, v in embedder.model_dump(by_alias=True).items() if v is not None
                 }  # type: ignore[attr-defined]
             else:  # pragma: no cover
                 warn(
                     "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
                     DeprecationWarning,
+                    stacklevel=2,
                 )
                 payload[key] = {
                     k: v for k, v in embedder.dict(by_alias=True).items() if v is not None
                 }  # type: ignore[attr-defined]
 
         response = self._http_requests.patch(
             f"{self._settings_url}/embedders", payload, compress=compress
         )
 
         return TaskInfo(**response.json())
 
-    def reset_embedders(self) -> TaskInfo:
+    # TODO: Add back after embedder setting issue fixed https://github.com/meilisearch/meilisearch/issues/4585
+    def reset_embedders(self) -> TaskInfo:  # pragma: no cover
         """Reset an index's embedders settings to the default value.
 
         Returns:
 
             The details of the task status.
 
         Raises:
@@ -7793,15 +7980,15 @@
     q: str | None = None,
     facet_name: str | None = None,
     facet_query: str | None = None,
     offset: int = 0,
     limit: int = 20,
     filter: Filter | None = None,
     facets: list[str] | None = None,
-    attributes_to_retrieve: list[str] = ["*"],
+    attributes_to_retrieve: list[str] | None = None,
     attributes_to_crop: list[str] | None = None,
     crop_length: int = 200,
     attributes_to_highlight: list[str] | None = None,
     sort: list[str] | None = None,
     show_matches_position: bool = False,
     highlight_pre_tag: str = "<em>",
     highlight_post_tag: str = "</em>",
@@ -7811,14 +7998,17 @@
     page: int | None = None,
     attributes_to_search_on: list[str] | None = None,
     show_ranking_score: bool = False,
     show_ranking_score_details: bool = False,
     vector: list[float] | None = None,
     hybrid: Hybrid | None = None,
 ) -> JsonDict:
+    if attributes_to_retrieve is None:
+        attributes_to_retrieve = ["*"]
+
     body: JsonDict = {
         "q": q,
         "offset": offset,
         "limit": limit,
         "filter": filter,
         "facets": facets,
         "attributesToRetrieve": attributes_to_retrieve,
@@ -7852,52 +8042,77 @@
     if hybrid:
         if is_pydantic_2():
             body["hybrid"] = hybrid.model_dump(by_alias=True)  # type: ignore[attr-defined]
         else:  # pragma: no cover
             warn(
                 "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
                 DeprecationWarning,
+                stacklevel=2,
             )
             body["hybrid"] = hybrid.dict(by_alias=True)  # type: ignore[attr-defined]
 
     return body
 
 
 def _build_encoded_url(base_url: str, params: JsonMapping) -> str:
     return f"{base_url}?{urlencode(params)}"
 
 
-def _embedder_json_to_embedders_model(embedder_json: JsonDict | None) -> Embedders | None:
+# TODO: Add back after embedder setting issue fixed https://github.com/meilisearch/meilisearch/issues/4585
+def _embedder_json_to_embedders_model(  # pragma: no cover
+    embedder_json: JsonDict | None,
+) -> Embedders | None:
     if not embedder_json:  # pragma: no cover
         return None
 
-    embedders: dict[str, OpenAiEmbedder | HuggingFaceEmbedder | UserProvidedEmbedder] = {}
+    embedders: dict[
+        str,
+        OpenAiEmbedder | HuggingFaceEmbedder | OllamaEmbedder | RestEmbedder | UserProvidedEmbedder,
+    ] = {}
     for k, v in embedder_json.items():
         if v.get("source") == "openAi":
             embedders[k] = OpenAiEmbedder(**v)
         elif v.get("source") == "huggingFace":
             embedders[k] = HuggingFaceEmbedder(**v)
+        elif v.get("source") == "ollama":
+            embedders[k] = OllamaEmbedder(**v)
+        elif v.get("source") == "rest":
+            embedders[k] = RestEmbedder(**v)
         else:
             embedders[k] = UserProvidedEmbedder(**v)
 
     return Embedders(embedders=embedders)
 
 
-def _embedder_json_to_settings_model(
+# TODO: Add back after embedder setting issue fixed https://github.com/meilisearch/meilisearch/issues/4585
+def _embedder_json_to_settings_model(  # pragma: no cover
     embedder_json: JsonDict | None,
-) -> dict[str, OpenAiEmbedder | HuggingFaceEmbedder | UserProvidedEmbedder] | None:
+) -> (
+    dict[
+        str,
+        OpenAiEmbedder | HuggingFaceEmbedder | OllamaEmbedder | RestEmbedder | UserProvidedEmbedder,
+    ]
+    | None
+):
     if not embedder_json:  # pragma: no cover
         return None
 
-    embedders: dict[str, OpenAiEmbedder | HuggingFaceEmbedder | UserProvidedEmbedder] = {}
+    embedders: dict[
+        str,
+        OpenAiEmbedder | HuggingFaceEmbedder | OllamaEmbedder | RestEmbedder | UserProvidedEmbedder,
+    ] = {}
     for k, v in embedder_json.items():
         if v.get("source") == "openAi":
             embedders[k] = OpenAiEmbedder(**v)
         elif v.get("source") == "huggingFace":
             embedders[k] = HuggingFaceEmbedder(**v)
+        elif v.get("source") == "ollama":
+            embedders[k] = OllamaEmbedder(**v)
+        elif v.get("source") == "rest":
+            embedders[k] = RestEmbedder(**v)
         else:
             embedders[k] = UserProvidedEmbedder(**v)
 
     return embedders
 
 
 def _validate_file_type(file_path: Path) -> None:
```

### Comparing `meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/models/client.py` & `meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/models/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         def validate_last_update(cls, v: str) -> Union[datetime, None]:
             return iso_to_date_time(v)
 
     else:  # pragma: no cover
         warn(
             "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
             DeprecationWarning,
+            stacklevel=2,
         )
 
         @pydantic.validator("last_update", pre=True)
         @classmethod
         def validate_last_update(cls, v: str) -> Union[datetime, None]:
             return iso_to_date_time(v)
 
@@ -49,14 +50,15 @@
         def validate_expires_at(cls, v: str) -> Union[datetime, None]:
             return iso_to_date_time(v)
 
     else:  # pragma: no cover
         warn(
             "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
             DeprecationWarning,
+            stacklevel=2,
         )
 
         @pydantic.validator("expires_at", pre=True)
         @classmethod
         def validate_expires_at(cls, v: str) -> Union[datetime, None]:
             return iso_to_date_time(v)
 
@@ -94,14 +96,15 @@
         def validate_updated_at(cls, v: str) -> Union[datetime, None]:
             return iso_to_date_time(v)
 
     else:  # pragma: no cover
         warn(
             "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
             DeprecationWarning,
+            stacklevel=2,
         )
 
         @pydantic.validator("created_at", pre=True)
         @classmethod
         def validate_created_at(cls, v: str) -> datetime:
             converted = iso_to_date_time(v)
 
@@ -126,14 +129,15 @@
     if is_pydantic_2():
         model_config = pydantic.ConfigDict(ser_json_timedelta="iso8601")  # type: ignore[typeddict-unknown-key]
 
     else:  # pragma: no cover
         warn(
             "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
             DeprecationWarning,
+            stacklevel=2,
         )
 
         class Config:
             json_encoders = {
                 datetime: lambda v: None
                 if not v
                 else (
@@ -155,14 +159,15 @@
     if is_pydantic_2():
         model_config = pydantic.ConfigDict(ser_json_timedelta="iso8601")  # type: ignore[typeddict-unknown-key]
 
     else:  # pragma: no cover
         warn(
             "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
             DeprecationWarning,
+            stacklevel=2,
         )
 
         class Config:
             json_encoders = {
                 datetime: lambda v: None
                 if not v
                 else (
```

### Comparing `meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/models/index.py` & `meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/models/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
             return converted
 
     else:  # pragma: no cover
         warn(
             "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
             DeprecationWarning,
+            stacklevel=2,
         )
 
         @pydantic.validator("created_at", pre=True)
         @classmethod
         def validate_created_at(cls, v: str) -> datetime:
             converted = iso_to_date_time(v)
```

### Comparing `meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/models/search.py` & `meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/models/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,12 +56,12 @@
     processing_time_ms: int
     query: str
     facet_distribution: Optional[JsonDict] = None
     total_pages: Optional[int] = None
     total_hits: Optional[int] = None
     page: Optional[int] = None
     hits_per_page: Optional[int] = None
-    vector: Optional[List[float]] = None
+    semantic_hit_count: Optional[int] = None
 
 
 class SearchResultsWithUID(SearchResults):
     index_uid: str
```

### Comparing `meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/models/task.py` & `meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/models/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         def validate_finished_at(cls, v: str) -> Union[datetime, None]:
             return iso_to_date_time(v)
 
     else:  # pragma: no cover
         warn(
             "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
             DeprecationWarning,
+            stacklevel=2,
         )
 
         @pydantic.validator("enqueued_at", pre=True)
         @classmethod
         def validate_enqueued_at(cls, v: str) -> datetime:
             converted = iso_to_date_time(v)
 
@@ -102,14 +103,15 @@
 
             return converted
 
     else:  # pragma: no cover
         warn(
             "The use of Pydantic less than version 2 is depreciated and will be removed in a future release",
             DeprecationWarning,
+            stacklevel=2,
         )
 
         @pydantic.validator("enqueued_at", pre=True)
         @classmethod
         def validate_enqueued_at(cls, v: str) -> datetime:
             converted = iso_to_date_time(v)
```

### Comparing `meilisearch_python_sdk-2.8.0/meilisearch_python_sdk/plugins.py` & `meilisearch_python_sdk-2.9.0/meilisearch_python_sdk/plugins.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from enum import Enum
-from typing import Any, NamedTuple, Protocol, Sequence
+from typing import TYPE_CHECKING, Any, NamedTuple, Protocol, Sequence
 
-from meilisearch_python_sdk.models.search import FacetSearchResults, SearchResults
-from meilisearch_python_sdk.models.task import TaskInfo
-from meilisearch_python_sdk.types import JsonDict, JsonMapping
+if TYPE_CHECKING:  # pragma: no cover
+    from meilisearch_python_sdk.models.search import FacetSearchResults, SearchResults
+    from meilisearch_python_sdk.models.task import TaskInfo
+    from meilisearch_python_sdk.types import JsonDict, JsonMapping
 
 
 class AsyncEvent(Enum):
     PRE = "pre"
     CONCURRENT = "concurrent"
     POST = "post"
```

### Comparing `meilisearch_python_sdk-2.8.0/pyproject.toml` & `meilisearch_python_sdk-2.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-python-sdk"
-version = "2.8.0"
+version = "2.9.0"
 description = "A Python client providing both async and sync support for the Meilisearch API"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-python-sdk"
 homepage = "https://github.com/sanders41/meilisearch-python-sdk"
 documentation = "https://meilisearch-python-sdk.paulsanders.dev"
@@ -72,15 +72,15 @@
 
 [tool.ruff]
 line-length = 100
 target-version = "py38"
 fix = true
 
 [tool.ruff.lint]
-select=["E", "F", "UP", "I001", "T201", "T203"]
+select=["E", "B", "F", "UP", "I001", "T201", "T203"]
 ignore=[
   # Recommened ignores by ruff when using formatter
   "E501",
   "W191",
   "E111",
   "E114",
   "E117",
```

### Comparing `meilisearch_python_sdk-2.8.0/PKG-INFO` & `meilisearch_python_sdk-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearch-python-sdk
-Version: 2.8.0
+Version: 2.9.0
 Summary: A Python client providing both async and sync support for the Meilisearch API
 Home-page: https://github.com/sanders41/meilisearch-python-sdk
 License: MIT
 Keywords: meilisearch,async,python,client,sdk
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -32,17 +32,14 @@
 
 [![Tests Status](https://github.com/sanders41/meilisearch-python-sdk/workflows/Testing/badge.svg?branch=main&event=push)](https://github.com/sanders41/meilisearch-python-sdk/actions?query=workflow%3ATesting+branch%3Amain+event%3Apush)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sanders41/meilisearch-python-sdk/main.svg)](https://results.pre-commit.ci/latest/github/sanders41/meilisearch-python-sdk/main)
 [![Coverage](https://codecov.io/github/sanders41/meilisearch-python-sdk/coverage.svg?branch=main)](https://codecov.io/gh/sanders41/meilisearch-python-sdk)
 [![PyPI version](https://badge.fury.io/py/meilisearch-python-sdk.svg)](https://badge.fury.io/py/meilisearch-python-sdk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/meilisearch-python-sdk?color=5cc141)](https://github.com/sanders41/meilisearch-python-sdk)
 
-NOTE: This project was previously named `meilisearch-python-async`. Development on
-that project continues here under the new name.
-
 Meilisearch Python SDK provides both an async and sync client for the
 [Meilisearch](https://github.com/meilisearch/meilisearch) API.
 
 Which client to use depends on your use case. If the code base you are working with uses asyncio,
 for example if you are using [FastAPI](https://fastapi.tiangolo.com/), choose the `AsyncClient`,
 otherwise choose the sync `Client`. The functionality of the two clients is the same, the difference
 being that the `AsyncClient` provides async methods and uses the `AsyncIndex` with its own
```

