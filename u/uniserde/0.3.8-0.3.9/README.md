# Comparing `tmp/uniserde-0.3.8.tar.gz` & `tmp/uniserde-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniserde-0.3.8.tar", max compression
+gzip compressed data, was "uniserde-0.3.9.tar", max compression
```

## Comparing `uniserde-0.3.8.tar` & `uniserde-0.3.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1059 2023-07-21 17:40:19.302257 uniserde-0.3.8/LICENSE
--rw-r--r--   0        0        0     9641 2023-08-24 08:36:56.373750 uniserde-0.3.8/README.md
--rw-r--r--   0        0        0      695 2023-08-24 08:29:39.366353 uniserde-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      319 2023-08-24 08:40:28.903714 uniserde-0.3.8/uniserde/__init__.py
--rw-r--r--   0        0        0     2439 2023-07-31 08:58:33.668781 uniserde-0.3.8/uniserde/bson_deserialize.py
--rw-r--r--   0        0        0     2160 2023-08-24 08:35:13.550239 uniserde-0.3.8/uniserde/bson_serialize.py
--rw-r--r--   0        0        0    10650 2023-08-24 08:22:53.765776 uniserde-0.3.8/uniserde/caching_serdeserializer.py
--rw-r--r--   0        0        0     1210 2023-07-04 19:24:43.375352 uniserde-0.3.8/uniserde/case_convert.py
--rw-r--r--   0        0        0     4051 2023-07-28 13:42:15.590760 uniserde-0.3.8/uniserde/common.py
--rw-r--r--   0        0        0     6884 2023-08-24 08:34:42.650186 uniserde-0.3.8/uniserde/json_deserialize.py
--rw-r--r--   0        0        0     5702 2023-08-24 08:34:18.953479 uniserde-0.3.8/uniserde/json_serialize.py
--rw-r--r--   0        0        0     4115 2023-08-01 20:38:30.124059 uniserde-0.3.8/uniserde/lazy_wrapper.py
--rw-r--r--   0        0        0     2143 2023-08-24 08:22:53.765776 uniserde-0.3.8/uniserde/objectid_proxy.py
--rw-r--r--   0        0        0     9198 2023-08-24 08:40:42.130368 uniserde-0.3.8/uniserde/schema_mongodb.py
--rw-r--r--   0        0        0     2992 2023-08-24 08:40:42.233702 uniserde-0.3.8/uniserde/serde_class.py
--rw-r--r--   0        0        0      640 2023-08-24 08:29:01.486294 uniserde-0.3.8/uniserde/typedefs.py
--rw-r--r--   0        0        0    10407 1970-01-01 00:00:00.000000 uniserde-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-11-08 19:57:44.845419 uniserde-0.3.9/LICENSE
+-rw-r--r--   0        0        0     9641 2023-11-08 19:57:45.532086 uniserde-0.3.9/README.md
+-rw-r--r--   0        0        0      695 2024-01-15 21:20:56.225382 uniserde-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      319 2023-11-08 19:57:45.615420 uniserde-0.3.9/uniserde/__init__.py
+-rw-r--r--   0        0        0     2439 2023-11-08 19:57:45.615420 uniserde-0.3.9/uniserde/bson_deserialize.py
+-rw-r--r--   0        0        0     2160 2023-11-08 19:57:45.615420 uniserde-0.3.9/uniserde/bson_serialize.py
+-rw-r--r--   0        0        0    10767 2024-01-15 21:21:02.302055 uniserde-0.3.9/uniserde/caching_serdeserializer.py
+-rw-r--r--   0        0        0     1210 2023-11-08 19:57:45.615420 uniserde-0.3.9/uniserde/case_convert.py
+-rw-r--r--   0        0        0     4228 2024-01-15 21:19:08.455276 uniserde-0.3.9/uniserde/common.py
+-rw-r--r--   0        0        0     6884 2023-11-08 19:57:45.615420 uniserde-0.3.9/uniserde/json_deserialize.py
+-rw-r--r--   0        0        0     5702 2023-11-08 19:57:45.615420 uniserde-0.3.9/uniserde/json_serialize.py
+-rw-r--r--   0        0        0     4115 2023-11-08 19:57:45.615420 uniserde-0.3.9/uniserde/lazy_wrapper.py
+-rw-r--r--   0        0        0     2143 2023-11-08 19:57:45.615420 uniserde-0.3.9/uniserde/objectid_proxy.py
+-rw-r--r--   0        0        0     9305 2024-01-15 21:21:02.305388 uniserde-0.3.9/uniserde/schema_mongodb.py
+-rw-r--r--   0        0        0     2992 2023-11-08 19:57:45.615420 uniserde-0.3.9/uniserde/serde_class.py
+-rw-r--r--   0        0        0      640 2023-11-08 19:57:45.615420 uniserde-0.3.9/uniserde/typedefs.py
+-rw-r--r--   0        0        0    10458 1970-01-01 00:00:00.000000 uniserde-0.3.9/PKG-INFO
```

### Comparing `uniserde-0.3.8/LICENSE` & `uniserde-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.8/README.md` & `uniserde-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.8/pyproject.toml` & `uniserde-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uniserde"
-version = "0.3.8"
+version = "0.3.9"
 description = "Convention based, effortless serialization and deserialization"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/uniserde"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `uniserde-0.3.8/uniserde/bson_deserialize.py` & `uniserde-0.3.9/uniserde/bson_deserialize.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.8/uniserde/bson_serialize.py` & `uniserde-0.3.9/uniserde/bson_serialize.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.8/uniserde/caching_serdeserializer.py` & `uniserde-0.3.9/uniserde/caching_serdeserializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import enum
 import inspect
+import types
 from abc import ABC, abstractmethod
 from typing import *  # type: ignore
 
-from . import case_convert, common, lazy_wrapper, serde_class
-from .common import SerdeError
 from typing_extensions import TypeAlias
 
+from . import case_convert, common, lazy_wrapper, serde_class
+from .common import SerdeError
 
 IN = TypeVar("IN")
 OUT = TypeVar("OUT")
 
 Handler: TypeAlias = Callable[["CachingSerDeserializer[IN, OUT]", IN, Type[OUT]], OUT]
 
 
@@ -95,14 +96,18 @@
         value_type: Type,
     ) -> Handler:
         # Prepare the key for the cache lookup
         type_key = get_origin(value_type)
         if type_key is None:
             type_key = value_type
 
+        # Handle new-style unions
+        if type_key is types.UnionType:
+            type_key = Union
+
         # Custom handlers take precedence
         try:
             custom_handler = self._custom_deserializers[type_key]
         except KeyError:
             pass
         else:
             return lambda self, value, as_type: custom_handler(value, as_type)
```

### Comparing `uniserde-0.3.8/uniserde/case_convert.py` & `uniserde-0.3.9/uniserde/case_convert.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.8/uniserde/common.py` & `uniserde-0.3.9/uniserde/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 import re
+import types
 from datetime import datetime
 from typing import *  # type: ignore
 
 from .objectid_proxy import ObjectId
 
 Recur = Callable[[Any, Type], Any]
 Serializer = Callable[[Any, Type, Recur], Any]
@@ -67,14 +68,18 @@
         return serializer(value)
 
     # Find a matching serializer
     key = get_origin(value_type)
     if key is None:
         key = value_type
 
+    # Handle new-style unions
+    if key is types.UnionType:
+        key = Union
+
     try:
         serializer = serializers[key]
     except KeyError:
         if inspect.isclass(value_type):
             serializer = class_serializer
         else:
             raise ValueError(f"Unsupported field of type {value_type}") from None
@@ -109,14 +114,18 @@
         return deserializer(value)
 
     # Find a matching deserializer
     key = get_origin(value_type)
     if key is None:
         key = value_type
 
+    # Handle new-style unions
+    if key is types.UnionType:
+        key = Union
+
     try:
         deserializer = deserializers[key]
     except KeyError:
         if inspect.isclass(value_type):
             deserializer = class_deserializer
         else:
             raise ValueError(f"Unsupported field of type {value_type}") from None
```

### Comparing `uniserde-0.3.8/uniserde/json_deserialize.py` & `uniserde-0.3.9/uniserde/json_deserialize.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.8/uniserde/json_serialize.py` & `uniserde-0.3.9/uniserde/json_serialize.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.8/uniserde/lazy_wrapper.py` & `uniserde-0.3.9/uniserde/lazy_wrapper.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.8/uniserde/objectid_proxy.py` & `uniserde-0.3.9/uniserde/objectid_proxy.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.8/uniserde/schema_mongodb.py` & `uniserde-0.3.9/uniserde/schema_mongodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import enum
 import inspect
+import types
 from datetime import datetime, timedelta
 from typing import *  # type: ignore
 
 from . import case_convert, serde_class
 from .common import *
 from .objectid_proxy import ObjectId
 from .typedefs import Jsonable
@@ -15,14 +16,18 @@
 
     def process(self, value_type: Type) -> Jsonable:
         # Prepare the key for the handler lookup
         key = get_origin(value_type)
         if key is None:
             key = value_type
 
+        # Handle new-style unions
+        if key is types.UnionType:
+            key = Union
+
         # Custom handlers take precedence
         try:
             handler = self._custom_handlers[key]
         except KeyError:
             pass
         else:
             return handler(value_type)
```

### Comparing `uniserde-0.3.8/uniserde/serde_class.py` & `uniserde-0.3.9/uniserde/serde_class.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.8/uniserde/typedefs.py` & `uniserde-0.3.9/uniserde/typedefs.py`

 * *Files identical despite different names*

### Comparing `uniserde-0.3.8/PKG-INFO` & `uniserde-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: uniserde
-Version: 0.3.8
+Version: 0.3.9
 Summary: Convention based, effortless serialization and deserialization
 Home-page: https://gitlab.com/Vivern/uniserde
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pymongo (>=4.4.0,<5.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Project-URL: Repository, https://gitlab.com/Vivern/uniserde
 Description-Content-Type: text/markdown
 
 # Convention based, effortless serialization and deserialization
```

