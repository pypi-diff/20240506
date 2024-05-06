# Comparing `tmp/pyathena-3.8.1.tar.gz` & `tmp/pyathena-3.8.2.tar.gz`

## Comparing `pyathena-3.8.1.tar` & `pyathena-3.8.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/__init__.py
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/async_cursor.py
--rw-r--r--   0        0        0    23825 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/common.py
--rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/connection.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/converter.py
--rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/cursor.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/error.py
--rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/formatter.py
--rw-r--r--   0        0        0    22930 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/py.typed
--rw-r--r--   0        0        0    23041 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/result_set.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/arrow/__init__.py
--rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/arrow/async_cursor.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/arrow/converter.py
--rw-r--r--   0        0        0     6854 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/arrow/cursor.py
--rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/arrow/result_set.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/arrow/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/fastparquet/__init__.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/fastparquet/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/filesystem/__init__.py
--rw-r--r--   0        0        0    34952 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/filesystem/s3.py
--rw-r--r--   0        0        0    14350 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/filesystem/s3_object.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/pandas/__init__.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/pandas/async_cursor.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/pandas/converter.py
--rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/pandas/cursor.py
--rw-r--r--   0        0        0    13467 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/pandas/result_set.py
--rw-r--r--   0        0        0    10297 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/pandas/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/spark/__init__.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/spark/async_cursor.py
--rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/spark/common.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/spark/cursor.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/sqlalchemy/arrow.py
--rw-r--r--   0        0        0    42007 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/sqlalchemy/base.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/sqlalchemy/pandas.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/sqlalchemy/requirements.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/sqlalchemy/rest.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/sqlalchemy/types.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/sqlalchemy/util.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pyathena-3.8.1/.gitignore
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pyathena-3.8.1/LICENSE
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 pyathena-3.8.1/README.rst
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyproject.toml
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 pyathena-3.8.1/PKG-INFO
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/__init__.py
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/async_cursor.py
+-rw-r--r--   0        0        0    23825 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/common.py
+-rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/connection.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/converter.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/cursor.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/error.py
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/formatter.py
+-rw-r--r--   0        0        0    22930 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/py.typed
+-rw-r--r--   0        0        0    23041 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/result_set.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/util.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/arrow/__init__.py
+-rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/arrow/async_cursor.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/arrow/converter.py
+-rw-r--r--   0        0        0     6854 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/arrow/cursor.py
+-rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/arrow/result_set.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/arrow/util.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/fastparquet/__init__.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/fastparquet/util.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/filesystem/__init__.py
+-rw-r--r--   0        0        0    43497 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/filesystem/s3.py
+-rw-r--r--   0        0        0    15098 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/filesystem/s3_object.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/pandas/__init__.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/pandas/async_cursor.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/pandas/converter.py
+-rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/pandas/cursor.py
+-rw-r--r--   0        0        0    13467 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/pandas/result_set.py
+-rw-r--r--   0        0        0    10297 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/pandas/util.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/spark/__init__.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/spark/async_cursor.py
+-rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/spark/common.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/spark/cursor.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/sqlalchemy/arrow.py
+-rw-r--r--   0        0        0    42007 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/sqlalchemy/base.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/sqlalchemy/pandas.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/sqlalchemy/rest.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/sqlalchemy/types.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/sqlalchemy/util.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pyathena-3.8.2/.gitignore
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pyathena-3.8.2/LICENSE
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 pyathena-3.8.2/README.rst
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyproject.toml
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 pyathena-3.8.2/PKG-INFO
```

### Comparing `pyathena-3.8.1/pyathena/__init__.py` & `pyathena-3.8.2/pyathena/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pyathena.error import *  # noqa
 
 if TYPE_CHECKING:
     from pyathena.connection import Connection, ConnectionCursor
     from pyathena.cursor import Cursor
 
-__version__ = "3.8.1"
+__version__ = "3.8.2"
 user_agent_extra: str = f"PyAthena/{__version__}"
 
 # Globals https://www.python.org/dev/peps/pep-0249/#globals
 apilevel: str = "2.0"
 threadsafety: int = 2
 paramstyle: str = "pyformat"
```

### Comparing `pyathena-3.8.1/pyathena/async_cursor.py` & `pyathena-3.8.2/pyathena/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/common.py` & `pyathena-3.8.2/pyathena/common.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/connection.py` & `pyathena-3.8.2/pyathena/connection.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/converter.py` & `pyathena-3.8.2/pyathena/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/cursor.py` & `pyathena-3.8.2/pyathena/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/error.py` & `pyathena-3.8.2/pyathena/error.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/formatter.py` & `pyathena-3.8.2/pyathena/formatter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/model.py` & `pyathena-3.8.2/pyathena/model.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/result_set.py` & `pyathena-3.8.2/pyathena/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/util.py` & `pyathena-3.8.2/pyathena/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/arrow/async_cursor.py` & `pyathena-3.8.2/pyathena/arrow/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/arrow/converter.py` & `pyathena-3.8.2/pyathena/arrow/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/arrow/cursor.py` & `pyathena-3.8.2/pyathena/arrow/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/arrow/result_set.py` & `pyathena-3.8.2/pyathena/arrow/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/arrow/util.py` & `pyathena-3.8.2/pyathena/arrow/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/fastparquet/util.py` & `pyathena-3.8.2/pyathena/fastparquet/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/filesystem/s3.py` & `pyathena-3.8.2/pyathena/filesystem/s3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import itertools
 import logging
+import mimetypes
+import os.path
 import re
 from concurrent.futures import Future, as_completed
 from concurrent.futures.thread import ThreadPoolExecutor
 from copy import deepcopy
 from datetime import datetime
 from multiprocessing import cpu_count
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Pattern, Tuple, Union, cast
@@ -14,14 +16,15 @@
 import botocore.exceptions
 from boto3 import Session
 from botocore import UNSIGNED
 from botocore.client import BaseClient, Config
 from fsspec import AbstractFileSystem
 from fsspec.callbacks import _DEFAULT_CALLBACK
 from fsspec.spec import AbstractBufferedFile
+from fsspec.utils import tokenize
 
 import pyathena
 from pyathena.filesystem.s3_object import (
     S3CompleteMultipartUpload,
     S3MultipartUpload,
     S3MultipartUploadPart,
     S3Object,
@@ -36,25 +39,27 @@
 
 _logger = logging.getLogger(__name__)  # type: ignore
 
 
 class S3FileSystem(AbstractFileSystem):
     # https://docs.aws.amazon.com/AmazonS3/latest/userguide/qfacts.html
     # The minimum size of a part in a multipart upload is 5MiB.
-    MULTIPART_UPLOAD_MINIMUM_PART_SIZE: int = 5 * 2**20  # 5MiB
+    MULTIPART_UPLOAD_MIN_PART_SIZE: int = 5 * 2**20  # 5MiB
     # https://docs.aws.amazon.com/AmazonS3/latest/userguide/qfacts.html
     # The maximum size of a part in a multipart upload is 5GiB.
-    MULTIPART_UPLOAD_MAXIMUM_PART_SIZE: int = 5 * 2**30  # 5GiB
-    DEFAULT_BLOCK_SIZE: int = 5 * 2**20  # 5MB
+    MULTIPART_UPLOAD_MAX_PART_SIZE: int = 5 * 2**30  # 5GiB
+    # https://docs.aws.amazon.com/AmazonS3/latest/API/API_DeleteObjects.html
+    DELETE_OBJECTS_MAX_KEYS: int = 1000
+    DEFAULT_BLOCK_SIZE: int = 5 * 2**20  # 5MiB
     PATTERN_PATH: Pattern[str] = re.compile(
         r"(^s3://|^s3a://|^)(?P<bucket>[a-zA-Z0-9.\-_]+)(/(?P<key>[^?]+)|/)?"
         r"($|\?version(Id|ID|id|_id)=(?P<version_id>.+)$)"
     )
 
-    protocol = ["s3", "s3a"]
+    protocol = ("s3", "s3a")
     _extra_tokenize_attributes = ("default_block_size",)
 
     def __init__(
         self,
         connection: Optional["Connection[Any]"] = None,
         default_block_size: Optional[int] = None,
         default_cache_type: Optional[str] = None,
@@ -211,16 +216,16 @@
     def _ls_buckets(self, refresh: bool = False) -> List[S3Object]:
         if "" not in self.dircache or refresh:
             try:
                 response = self._call(
                     self._client.list_buckets,
                 )
             except botocore.exceptions.ClientError as e:
-                if e.response["Error"]["Code"] in ["AccessDenied", "403"]:
-                    return []
+                # if e.response["Error"]["Code"] in ["AccessDenied", "403"]:
+                #     return []
                 raise
             buckets = [
                 S3Object(
                     init={
                         "ContentLength": 0,
                         "ContentType": None,
                         "StorageClass": S3StorageClass.S3_STORAGE_CLASS_BUCKET,
@@ -274,15 +279,15 @@
                             "ContentType": None,
                             "StorageClass": S3StorageClass.S3_STORAGE_CLASS_DIRECTORY,
                             "ETag": None,
                             "LastModified": None,
                         },
                         type=S3ObjectType.S3_OBJECT_TYPE_DIRECTORY,
                         bucket=bucket,
-                        key=c["Prefix"][:-1],
+                        key=c["Prefix"][:-1].rstrip("/"),
                         version_id=version_id,
                     )
                     for c in response.get("CommonPrefixes", [])
                 )
                 files.extend(
                     S3Object(
                         init=c,
@@ -294,15 +299,19 @@
                 )
                 next_token = response.get("NextContinuationToken")
                 if not next_token:
                     break
             if files:
                 self.dircache[path] = files
         else:
-            files = self.dircache[path]
+            cache = self.dircache[path]
+            if not isinstance(cache, list):
+                files = [cache]
+            else:
+                files = cache
         return files
 
     def ls(
         self, path: str, detail: bool = False, refresh: bool = False, **kwargs
     ) -> Union[List[S3Object], List[str]]:
         path = self._strip_protocol(path).rstrip("/")
         if path in ["", "/"]:
@@ -321,22 +330,22 @@
         bucket, key, path_version_id = self.parse_path(path)
         version_id = path_version_id if path_version_id else kwargs.pop("version_id", None)
         if path in ["/", ""]:
             return S3Object(
                 init={
                     "ContentLength": 0,
                     "ContentType": None,
-                    "StorageClass": S3StorageClass.S3_STORAGE_CLASS_DIRECTORY,
+                    "StorageClass": S3StorageClass.S3_STORAGE_CLASS_BUCKET,
                     "ETag": None,
                     "LastModified": None,
                 },
                 type=S3ObjectType.S3_OBJECT_TYPE_DIRECTORY,
                 bucket=bucket,
-                key=path,
-                version_id=version_id,
+                key=None,
+                version_id=None,
             )
         if not refresh:
             caches: Union[List[S3Object], S3Object] = self._ls_from_cache(path)
             if caches is not None:
                 if isinstance(caches, list):
                     cache = next((c for c in caches if c.name == path), None)
                 elif caches.name == path:
@@ -353,21 +362,27 @@
                             "ContentType": None,
                             "StorageClass": S3StorageClass.S3_STORAGE_CLASS_DIRECTORY,
                             "ETag": None,
                             "LastModified": None,
                         },
                         type=S3ObjectType.S3_OBJECT_TYPE_DIRECTORY,
                         bucket=bucket,
-                        key=path,
+                        key=key.rstrip("/") if key else None,
                         version_id=version_id,
                     )
         if key:
-            info = self._head_object(path, refresh=refresh, version_id=version_id)
-            if info:
-                return info
+            object_info = self._head_object(path, refresh=refresh, version_id=version_id)
+            if object_info:
+                return object_info
+        else:
+            bucket_info = self._head_bucket(path, refresh=refresh)
+            if bucket_info:
+                return bucket_info
+            else:
+                raise FileNotFoundError(path)
 
         response = self._call(
             self._client.list_objects_v2,
             Bucket=bucket,
             Prefix=f"{key.rstrip('/')}/" if key else "",
             Delimiter="/",
             MaxKeys=1,
@@ -383,15 +398,15 @@
                     "ContentType": None,
                     "StorageClass": S3StorageClass.S3_STORAGE_CLASS_DIRECTORY,
                     "ETag": None,
                     "LastModified": None,
                 },
                 type=S3ObjectType.S3_OBJECT_TYPE_DIRECTORY,
                 bucket=bucket,
-                key=path,
+                key=key.rstrip("/") if key else None,
                 version_id=version_id,
             )
         else:
             raise FileNotFoundError(path)
 
     def find(
         self,
@@ -446,25 +461,82 @@
                 pass
             file = self._head_bucket(bucket)
             if file:
                 return True
             else:
                 return False
 
-    def rm_file(self, path: str) -> None:
-        # TODO
-        raise NotImplementedError  # pragma: no cover
-
-    def rmdir(self, path: str) -> None:
-        # TODO
-        raise NotImplementedError  # pragma: no cover
-
-    def _rm(self, path: str) -> None:
-        # TODO
-        raise NotImplementedError  # pragma: no cover
+    def rm_file(self, path: str, **kwargs) -> None:
+        bucket, key, version_id = self.parse_path(path)
+        if not key:
+            return
+        self._delete_object(bucket=bucket, key=key, version_id=version_id, **kwargs)
+        self.invalidate_cache(path)
+
+    def rm(self, path, recursive=False, maxdepth=None, **kwargs) -> None:
+        bucket, key, version_id = self.parse_path(path)
+        if not key:
+            raise ValueError("Cannot delete the bucket.")
+
+        expand_path = self.expand_path(path, recursive=recursive, maxdepth=maxdepth)
+        self._delete_objects(bucket, expand_path, **kwargs)
+        for p in expand_path:
+            self.invalidate_cache(p)
+
+    def _delete_object(
+        self, bucket: str, key: str, version_id: Optional[str] = None, **kwargs
+    ) -> None:
+        request = {
+            "Bucket": bucket,
+            "Key": key,
+        }
+        if version_id:
+            request.update({"VersionId": version_id})
+
+        _logger.debug(f"Delete object: s3://{bucket}/{key}?versionId={version_id}")
+        self._call(
+            self._client.delete_object,
+            **request,
+        )
+
+    def _delete_objects(
+        self, bucket: str, paths: List[str], max_workers: Optional[int] = None, **kwargs
+    ) -> None:
+        if not paths:
+            return
+
+        max_workers = max_workers if max_workers else self.max_workers
+        quiet = kwargs.pop("Quiet", True)
+        delete_objects = []
+        for p in paths:
+            bucket, key, version_id = self.parse_path(p)
+            if key:
+                object_ = {"Key": key}
+                if version_id:
+                    object_.update({"VersionId": version_id})
+                delete_objects.append(object_)
+
+        with ThreadPoolExecutor(max_workers=max_workers) as executor:
+            fs = []
+            for delete in [
+                delete_objects[i : i + self.DELETE_OBJECTS_MAX_KEYS]
+                for i in range(0, len(delete_objects), self.DELETE_OBJECTS_MAX_KEYS)
+            ]:
+                request = {
+                    "Bucket": bucket,
+                    "Delete": {
+                        "Objects": delete,
+                        "Quiet": quiet,
+                    },
+                }
+                fs.append(
+                    executor.submit(self._call, self._client.delete_objects, **request, **kwargs)
+                )
+            for f in as_completed(fs):
+                f.result()
 
     def touch(self, path: str, truncate: bool = True, **kwargs) -> Dict[str, Any]:
         bucket, key, version_id = self.parse_path(path)
         if version_id:
             raise ValueError("Cannot touch the file with the version specified.")
         if not truncate and self.exists(path):
             raise ValueError("Cannot touch the existing file without specifying truncate.")
@@ -472,53 +544,227 @@
             raise ValueError("Cannot touch the bucket.")
 
         object_ = self._put_object(bucket=bucket, key=key, body=None, **kwargs)
         self.invalidate_cache(path)
         return object_.to_dict()
 
     def cp_file(self, path1: str, path2: str, **kwargs):
-        # TODO
-        raise NotImplementedError  # pragma: no cover
+        bucket1, key1, version_id1 = self.parse_path(path1)
+        bucket2, key2, version_id2 = self.parse_path(path2)
+        if version_id2:
+            raise ValueError("Cannot copy to a versioned file.")
+
+        info1 = self.info(path1)
+        size1 = info1.get("size", 0)
+        if size1 <= self.MULTIPART_UPLOAD_MAX_PART_SIZE:
+            self._copy_object(
+                bucket1=bucket1,
+                key1=key1,
+                version_id1=version_id1,
+                bucket2=bucket2,
+                key2=key2,
+                **kwargs,
+            )
+        else:
+            self._copy_object_with_multipart_upload(
+                bucket1=bucket1,
+                key1=key1,
+                version_id1=version_id1,
+                size1=size1,
+                bucket2=bucket2,
+                key2=key2,
+                **kwargs,
+            )
+        self.invalidate_cache(path2)
+
+    def _copy_object(
+        self,
+        bucket1: str,
+        key1: str,
+        version_id1: Optional[str],
+        bucket2: str,
+        key2: str,
+        **kwargs,
+    ) -> None:
+        copy_source = {
+            "Bucket": bucket1,
+            "Key": key1,
+        }
+        if version_id1:
+            copy_source.update({"VersionId": version_id1})
+        request = {
+            "CopySource": copy_source,
+            "Bucket": bucket2,
+            "Key": key2,
+        }
+
+        _logger.debug(
+            f"Copy object from s3://{bucket1}/{key1}?versionId={version_id1} "
+            f"to s3://{bucket2}/{key2}."
+        )
+        self._call(self._client.copy_object, **request, **kwargs)
+
+    def _copy_object_with_multipart_upload(
+        self,
+        bucket1: str,
+        key1: str,
+        size1: int,
+        bucket2: str,
+        key2: str,
+        max_workers: Optional[int] = None,
+        block_size: Optional[int] = None,
+        version_id1: Optional[str] = None,
+        **kwargs,
+    ) -> None:
+        max_workers = max_workers if max_workers else self.max_workers
+        block_size = block_size if block_size else self.MULTIPART_UPLOAD_MAX_PART_SIZE
+        if (
+            block_size < self.MULTIPART_UPLOAD_MIN_PART_SIZE
+            or block_size > self.MULTIPART_UPLOAD_MAX_PART_SIZE
+        ):
+            raise ValueError("Block size must be greater than 5MiB and less than 5GiB.")
+
+        copy_source = {
+            "Bucket": bucket1,
+            "Key": key1,
+        }
+        if version_id1:
+            copy_source.update({"VersionId": version_id1})
+
+        ranges = S3File._get_ranges(
+            0,
+            size1,
+            max_workers,
+            block_size,
+        )
+        multipart_upload = self._create_multipart_upload(
+            bucket=bucket2,
+            key=key2,
+            **kwargs,
+        )
+        parts = []
+        with ThreadPoolExecutor(max_workers=max_workers) as executor:
+            fs = [
+                executor.submit(
+                    self._upload_part_copy,
+                    bucket=bucket2,
+                    key=key2,
+                    copy_source=copy_source,
+                    upload_id=cast(str, multipart_upload.upload_id),
+                    part_number=i + 1,
+                    copy_source_ranges=range_,
+                )
+                for i, range_ in enumerate(ranges)
+            ]
+            for f in as_completed(fs):
+                result = f.result()
+                parts.append(
+                    {
+                        "ETag": result.etag,
+                        "PartNumber": result.part_number,
+                    }
+                )
+
+        parts.sort(key=lambda x: x["PartNumber"])
+        self._complete_multipart_upload(
+            bucket=bucket2,
+            key=key2,
+            upload_id=cast(str, multipart_upload.upload_id),
+            parts=parts,
+        )
 
     def cat_file(
         self, path: str, start: Optional[int] = None, end: Optional[int] = None, **kwargs
     ) -> bytes:
         bucket, key, version_id = self.parse_path(path)
-        if start is not None and end is not None:
+        if start is not None or end is not None:
+            size = self.info(path).get("size", 0)
+            if start is None:
+                start = 0
+            elif start < 0:
+                start = size + start
+            if end is None:
+                end = size
+            elif end < 0:
+                end = size + end
             ranges = (start, end)
         else:
             ranges = None
 
         return self._get_object(
             bucket=bucket,
             key=cast(str, key),
             ranges=ranges,
             version_id=version_id,
             **kwargs,
         )[1]
 
-    def pipe_file(self, path: str, value, **kwargs):
-        # TODO
-        raise NotImplementedError  # pragma: no cover
-
     def put_file(self, lpath: str, rpath: str, callback=_DEFAULT_CALLBACK, **kwargs):
-        # TODO
-        raise NotImplementedError  # pragma: no cover
+        if os.path.isdir(lpath):
+            # No support for directory uploads.
+            return
+
+        bucket, key, _ = self.parse_path(rpath)
+        if not key:
+            # No support for bucket copy.
+            return
+
+        size = os.path.getsize(lpath)
+        callback.set_size(size)
+        if "ContentType" not in kwargs:
+            content_type, _ = mimetypes.guess_type(lpath)
+            if content_type is not None:
+                kwargs["ContentType"] = content_type
+
+        with self.open(rpath, "wb", s3_additional_kwargs=kwargs) as remote:
+            with open(lpath, "rb") as local:
+                while data := local.read(remote.blocksize):
+                    remote.write(data)
+                    callback.relative_update(len(data))
+
+        self.invalidate_cache(rpath)
 
     def get_file(self, rpath: str, lpath: str, callback=_DEFAULT_CALLBACK, outfile=None, **kwargs):
-        # TODO
-        raise NotImplementedError  # pragma: no cover
+        if os.path.isdir(lpath):
+            return
+
+        with open(lpath, "wb") as local:
+            with self.open(rpath, "rb", **kwargs) as remote:
+                callback.set_size(remote.size)
+                while data := remote.read(remote.blocksize):
+                    local.write(data)
+                    callback.relative_update(len(data))
 
-    def checksum(self, path: str):
-        # TODO
-        raise NotImplementedError  # pragma: no cover
-
-    def sign(self, path: str, expiration: int = 100, **kwargs):
-        # TODO
-        raise NotImplementedError  # pragma: no cover
+    def checksum(self, path: str, **kwargs):
+        refresh = kwargs.pop("refresh", False)
+        info = self.info(path, refresh=refresh)
+        if info.get("type") != S3ObjectType.S3_OBJECT_TYPE_DIRECTORY:
+            return int(info.get("etag").strip('"').split("-")[0], 16)
+        else:
+            return int(tokenize(info), 16)
+
+    def sign(self, path: str, expiration: int = 3600, **kwargs):
+        bucket, key, version_id = self.parse_path(path)
+        client_method = kwargs.pop("client_method", "get_object")
+        params = {"Bucket": bucket, "Key": key}
+        if version_id:
+            params.update({"VersionId": version_id})
+        if kwargs:
+            params.update(kwargs)
+        request = {
+            "ClientMethod": client_method,
+            "Params": params,
+            "ExpiresIn": expiration,
+        }
+
+        _logger.debug(f"Generate signed url: s3://{bucket}/{key}?versionId={version_id}")
+        return self._call(
+            self._client.generate_presigned_url,
+            **request,
+        )
 
     def created(self, path: str) -> datetime:
         return self.modified(path)
 
     def modified(self, path: str) -> datetime:
         info = self.info(path)
         return cast(datetime, info.get("last_modified"))
@@ -542,26 +788,29 @@
         cache_options: Optional[Dict[Any, Any]] = None,
         **kwargs,
     ) -> S3File:
         if block_size is None:
             block_size = self.default_block_size
         if cache_type is None:
             cache_type = self.default_cache_type
+        max_workers = kwargs.pop("max_worker", self.max_workers)
+        s3_additional_kwargs = kwargs.pop("s3_additional_kwargs", {})
+        s3_additional_kwargs.update(self.s3_additional_kwargs)
 
         return S3File(
             self,
             path,
             mode,
             version_id=None,
-            max_workers=self.max_workers,
+            max_workers=max_workers,
             block_size=block_size,
             cache_type=cache_type,
             autocommit=autocommit,
             cache_options=cache_options,
-            s3_additional_kwargs=self.s3_additional_kwargs,
+            s3_additional_kwargs=s3_additional_kwargs,
             **kwargs,
         )
 
     def _get_object(
         self,
         bucket: str,
         key: str,
@@ -614,15 +863,15 @@
         )
         return S3MultipartUpload(response)
 
     def _upload_part_copy(
         self,
         bucket: str,
         key: str,
-        copy_source: str,
+        copy_source: Union[str, Dict[str, Any]],
         upload_id: str,
         part_number: int,
         copy_source_ranges: Optional[Tuple[int, int]] = None,
         **kwargs,
     ) -> S3MultipartUploadPart:
         request = {
             "Bucket": bucket,
@@ -708,14 +957,15 @@
         max_workers: int = (cpu_count() or 1) * 5,
         block_size: int = S3FileSystem.DEFAULT_BLOCK_SIZE,
         cache_type: str = "bytes",
         autocommit: bool = True,
         cache_options: Optional[Dict[Any, Any]] = None,
         size: Optional[int] = None,
         s3_additional_kwargs: Optional[Dict[str, Any]] = None,
+        **kwargs,
     ) -> None:
         self.max_workers = max_workers
         self._executor = ThreadPoolExecutor(max_workers=max_workers)
         self.s3_additional_kwargs = s3_additional_kwargs if s3_additional_kwargs else {}
 
         super().__init__(
             fs=fs,
@@ -739,32 +989,30 @@
                     f"the version_id: {path_version_id} specified in the path do not match."
                 )
             self.version_id: Optional[str] = version_id
         elif path_version_id:
             self.version_id = path_version_id
         else:
             self.version_id = version_id
-        if "r" not in mode and block_size < self.fs.MULTIPART_UPLOAD_MINIMUM_PART_SIZE:
+        if "r" not in mode and block_size < self.fs.MULTIPART_UPLOAD_MIN_PART_SIZE:
             # When writing occurs, the block size should not be smaller
             # than the minimum size of a part in a multipart upload.
-            raise ValueError(
-                f"Block size must be >= {self.fs.MULTIPART_UPLOAD_MINIMUM_PART_SIZE}MB."
-            )
+            raise ValueError(f"Block size must be >= {self.fs.MULTIPART_UPLOAD_MIN_PART_SIZE}MB.")
 
         self.append_block = False
         if "r" in mode:
             info = self.fs.info(self.path, version_id=self.version_id)
             if etag := info.get("etag"):
                 self.s3_additional_kwargs.update({"IfMatch": etag})
             self._details = info
         elif "a" in mode and self.fs.exists(path):
             self.append_block = True
             info = self.fs.info(self.path, version_id=self.version_id)
             loc = info.get("size", 0)
-            if loc < self.fs.MULTIPART_UPLOAD_MINIMUM_PART_SIZE:
+            if loc < self.fs.MULTIPART_UPLOAD_MIN_PART_SIZE:
                 self.write(self.fs.cat(self.path))
             self.loc = loc
             self.s3_additional_kwargs.update(info.to_api_repr())
             self._details = info
         else:
             self._details = {}
 
@@ -782,35 +1030,35 @@
 
         self.multipart_upload = self.fs._create_multipart_upload(
             bucket=self.bucket,
             key=self.key,
             **self.s3_additional_kwargs,
         )
         if self.append_block:
-            if self.tell() > S3FileSystem.MULTIPART_UPLOAD_MAXIMUM_PART_SIZE:
+            if self.tell() > S3FileSystem.MULTIPART_UPLOAD_MAX_PART_SIZE:
                 info = self.fs.info(self.path, version_id=self.version_id)
                 ranges = self._get_ranges(
                     0,
                     # Set copy source file byte size
                     info.get("size", 0),
                     self.max_workers,
-                    S3FileSystem.MULTIPART_UPLOAD_MAXIMUM_PART_SIZE,
+                    S3FileSystem.MULTIPART_UPLOAD_MAX_PART_SIZE,
                 )
-                for i, range in enumerate(ranges):
+                for i, range_ in enumerate(ranges):
                     self.multipart_upload_parts.append(
                         self._executor.submit(
                             self.fs._upload_part_copy,
                             bucket=self.bucket,
                             key=self.key,
                             copy_source=self.path,
                             upload_id=cast(
                                 str, cast(S3MultipartUpload, self.multipart_upload).upload_id
                             ),
                             part_number=i + 1,
-                            copy_source_ranges=range,
+                            copy_source_ranges=range_,
                         )
                     )
             else:
                 self.multipart_upload_parts.append(
                     self._executor.submit(
                         self.fs._upload_part_copy,
                         bucket=self.bucket,
@@ -871,21 +1119,20 @@
         else:
             if not self.multipart_upload:
                 raise RuntimeError("Multipart upload is not initialized.")
 
             parts: List[Dict[str, Any]] = []
             for f in as_completed(self.multipart_upload_parts):
                 result = f.result()
-                part = {
-                    "ETag": result.etag,
-                    "PartNumber": result.part_number,
-                }
-                if result.checksum_sha256:
-                    part.update({"ChecksumSHA256": result.checksum_sha256})
-                parts.append(part)
+                parts.append(
+                    {
+                        "ETag": result.etag,
+                        "PartNumber": result.part_number,
+                    }
+                )
             parts.sort(key=lambda x: x["PartNumber"])
             self.fs._complete_multipart_upload(
                 bucket=self.bucket,
                 key=self.key,
                 upload_id=cast(str, self.multipart_upload.upload_id),
                 parts=parts,
             )
```

### Comparing `pyathena-3.8.1/pyathena/filesystem/s3_object.py` & `pyathena-3.8.2/pyathena/filesystem/s3_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,20 +54,35 @@
 class S3Object(MutableMapping[str, Any]):
     def __init__(
         self,
         init: Dict[str, Any],
         **kwargs,
     ) -> None:
         if init:
-            super().update({_API_FIELD_TO_S3_OBJECT_PROPERTY.get(k, k): v for k, v in init.items()})
+            filtered = {}
+            for k, v in init.items():
+                if k not in _API_FIELD_TO_S3_OBJECT_PROPERTY:
+                    continue
+                filtered[_API_FIELD_TO_S3_OBJECT_PROPERTY[k]] = v
+            if "StorageClass" not in init:
+                # https://docs.aws.amazon.com/AmazonS3/latest/API/API_HeadObject.html#API_HeadObject_ResponseSyntax
+                # Amazon S3 returns this header for all objects except for
+                # S3 Standard storage class objects.
+                filtered[
+                    _API_FIELD_TO_S3_OBJECT_PROPERTY["StorageClass"]
+                ] = S3StorageClass.S3_STORAGE_CLASS_STANDARD
+            super().update(filtered)
             if "Size" in init:
                 self.content_length = init["Size"]
                 self.size = init["Size"]
-            if "ContentLength" in init:
+            elif "ContentLength" in init:
                 self.size = init["ContentLength"]
+            else:
+                self.content_length = 0
+                self.size = 0
         super().update({_API_FIELD_TO_S3_OBJECT_PROPERTY.get(k, k): v for k, v in kwargs.items()})
         if self.get("key") is None:
             self.name = self.get("bucket")
         else:
             self.name = f"{self.get('bucket')}/{self.get('key')}"
 
     def get(self, key: str, default: Any = None) -> Any:
@@ -90,14 +105,17 @@
 
     def __iter__(self) -> Iterator[str]:
         return iter(self.__dict__.keys())
 
     def __len__(self) -> int:
         return len(self.__dict__)
 
+    def __str__(self):
+        return str(self.__dict__)
+
     def to_dict(self) -> Dict[str, Any]:
         return copy.deepcopy(self.__dict__)
 
     def to_api_repr(self) -> Dict[str, Any]:
         fields = {}
         for k, v in _API_FIELD_TO_S3_OBJECT_PROPERTY.items():
             if k in ["ETag", "ContentLength", "LastModified"]:
```

### Comparing `pyathena-3.8.1/pyathena/pandas/async_cursor.py` & `pyathena-3.8.2/pyathena/pandas/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/pandas/converter.py` & `pyathena-3.8.2/pyathena/pandas/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/pandas/cursor.py` & `pyathena-3.8.2/pyathena/pandas/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/pandas/result_set.py` & `pyathena-3.8.2/pyathena/pandas/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/pandas/util.py` & `pyathena-3.8.2/pyathena/pandas/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/spark/async_cursor.py` & `pyathena-3.8.2/pyathena/spark/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/spark/common.py` & `pyathena-3.8.2/pyathena/spark/common.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/spark/cursor.py` & `pyathena-3.8.2/pyathena/spark/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/sqlalchemy/arrow.py` & `pyathena-3.8.2/pyathena/sqlalchemy/arrow.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/sqlalchemy/base.py` & `pyathena-3.8.2/pyathena/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/sqlalchemy/pandas.py` & `pyathena-3.8.2/pyathena/sqlalchemy/pandas.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/sqlalchemy/requirements.py` & `pyathena-3.8.2/pyathena/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyathena/sqlalchemy/types.py` & `pyathena-3.8.2/pyathena/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/LICENSE` & `pyathena-3.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/README.rst` & `pyathena-3.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/pyproject.toml` & `pyathena-3.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.1/PKG-INFO` & `pyathena-3.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: PyAthena
-Version: 3.8.1
+Version: 3.8.2
 Summary: Python DB API 2.0 (PEP 249) client for Amazon Athena
 Project-URL: homepage, https://github.com/laughingman7743/PyAthena/
 Project-URL: repository, https://github.com/laughingman7743/PyAthena/
 Author-email: laughingman7743 <laughingman7743@gmail.com>
 License: Copyright 2017 laughingman7743
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

