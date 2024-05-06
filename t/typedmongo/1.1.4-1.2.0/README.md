# Comparing `tmp/typedmongo-1.1.4.tar.gz` & `tmp/typedmongo-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedmongo-1.1.4.tar", last modified: Tue Apr 30 09:12:24 2024, max compression
+gzip compressed data, was "typedmongo-1.2.0.tar", last modified: Mon May  6 01:46:10 2024, max compression
```

## Comparing `typedmongo-1.1.4.tar` & `typedmongo-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-04-30 09:12:10.990197 typedmongo-1.1.4/LICENSE
--rw-r--r--   0        0        0     3976 2024-04-30 09:12:10.990197 typedmongo-1.1.4/README.md
--rw-r--r--   0        0        0     1441 2024-04-30 09:12:24.022312 typedmongo-1.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-30 09:12:10.990197 typedmongo-1.1.4/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 09:12:10.990197 typedmongo-1.1.4/tests/asyncio/__init__.py
--rw-r--r--   0        0        0     5789 2024-04-30 09:12:10.990197 typedmongo-1.1.4/tests/asyncio/test_client.py
--rw-r--r--   0        0        0     4233 2024-04-30 09:12:10.990197 typedmongo-1.1.4/tests/asyncio/test_table.py
--rw-r--r--   0        0        0     1218 2024-04-30 09:12:10.990197 typedmongo-1.1.4/tests/sync.py
--rw-r--r--   0        0        0     5549 2024-04-30 09:12:10.990197 typedmongo-1.1.4/tests/test_client.py
--rw-r--r--   0        0        0     2930 2024-04-30 09:12:10.990197 typedmongo-1.1.4/tests/test_expressions.py
--rw-r--r--   0        0        0      582 2024-04-30 09:12:10.990197 typedmongo-1.1.4/tests/test_marshamallow.py
--rw-r--r--   0        0        0     4225 2024-04-30 09:12:10.990197 typedmongo-1.1.4/tests/test_table.py
--rw-r--r--   0        0        0      781 2024-04-30 09:12:10.990197 typedmongo-1.1.4/typedmongo/__init__.py
--rw-r--r--   0        0        0      781 2024-04-30 09:12:10.994197 typedmongo-1.1.4/typedmongo/asyncio/__init__.py
--rw-r--r--   0        0        0    11612 2024-04-30 09:12:10.994197 typedmongo-1.1.4/typedmongo/asyncio/client.py
--rw-r--r--   0        0        0     9999 2024-04-30 09:12:10.994197 typedmongo-1.1.4/typedmongo/asyncio/fields.py
--rw-r--r--   0        0        0     8342 2024-04-30 09:12:10.994197 typedmongo-1.1.4/typedmongo/asyncio/table.py
--rw-r--r--   0        0        0    11394 2024-04-30 09:12:10.994197 typedmongo-1.1.4/typedmongo/client.py
--rw-r--r--   0        0        0      163 2024-04-30 09:12:10.994197 typedmongo-1.1.4/typedmongo/exceptions.py
--rw-r--r--   0        0        0     5452 2024-04-30 09:12:10.994197 typedmongo-1.1.4/typedmongo/expressions.py
--rw-r--r--   0        0        0     9999 2024-04-30 09:12:10.994197 typedmongo-1.1.4/typedmongo/fields.py
--rw-r--r--   0        0        0      849 2024-04-30 09:12:10.994197 typedmongo-1.1.4/typedmongo/marshamallow.py
--rw-r--r--   0        0        0     1325 2024-04-30 09:12:10.994197 typedmongo-1.1.4/typedmongo/sync.py
--rw-r--r--   0        0        0     8342 2024-04-30 09:12:10.994197 typedmongo-1.1.4/typedmongo/table.py
--rw-r--r--   0        0        0     4349 1970-01-01 00:00:00.000000 typedmongo-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-06 01:45:52.892057 typedmongo-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3808 2024-05-06 01:45:52.892057 typedmongo-1.2.0/README.md
+-rw-r--r--   0        0        0     1441 2024-05-06 01:46:10.243988 typedmongo-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-06 01:45:52.892057 typedmongo-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 01:45:52.892057 typedmongo-1.2.0/tests/asyncio/__init__.py
+-rw-r--r--   0        0        0     5575 2024-05-06 01:45:52.892057 typedmongo-1.2.0/tests/asyncio/test_client.py
+-rw-r--r--   0        0        0     4233 2024-05-06 01:45:52.896057 typedmongo-1.2.0/tests/asyncio/test_table.py
+-rw-r--r--   0        0        0     1218 2024-05-06 01:45:52.896057 typedmongo-1.2.0/tests/sync.py
+-rw-r--r--   0        0        0     5335 2024-05-06 01:45:52.896057 typedmongo-1.2.0/tests/test_client.py
+-rw-r--r--   0        0        0     2930 2024-05-06 01:45:52.896057 typedmongo-1.2.0/tests/test_expressions.py
+-rw-r--r--   0        0        0      582 2024-05-06 01:45:52.896057 typedmongo-1.2.0/tests/test_marshamallow.py
+-rw-r--r--   0        0        0     4225 2024-05-06 01:45:52.896057 typedmongo-1.2.0/tests/test_table.py
+-rw-r--r--   0        0        0      811 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/__init__.py
+-rw-r--r--   0        0        0      811 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/asyncio/__init__.py
+-rw-r--r--   0        0        0    10328 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/asyncio/client.py
+-rw-r--r--   0        0        0     9999 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/asyncio/fields.py
+-rw-r--r--   0        0        0     8527 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/asyncio/table.py
+-rw-r--r--   0        0        0    10122 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/client.py
+-rw-r--r--   0        0        0      163 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/exceptions.py
+-rw-r--r--   0        0        0     5452 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/expressions.py
+-rw-r--r--   0        0        0     9999 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/fields.py
+-rw-r--r--   0        0        0      849 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/marshamallow.py
+-rw-r--r--   0        0        0     1325 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/sync.py
+-rw-r--r--   0        0        0     8527 2024-05-06 01:45:52.896057 typedmongo-1.2.0/typedmongo/table.py
+-rw-r--r--   0        0        0     4181 1970-01-01 00:00:00.000000 typedmongo-1.2.0/PKG-INFO
```

### Comparing `typedmongo-1.1.4/LICENSE` & `typedmongo-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.4/README.md` & `typedmongo-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: typedmongo
+Version: 1.2.0
+Summary: A production-ready modern Python MongoDB ODM
+Author-Email: abersheeran <me@abersheeran.com>
+License: Apache2.0
+Requires-Python: >=3.10
+Requires-Dist: pymongo>=4.6.3
+Requires-Dist: motor>=3.4.0
+Requires-Dist: marshmallow>=3.21.1
+Requires-Dist: typing-extensions>=4.11.0
+Description-Content-Type: text/markdown
+
 # Typed Mongo
 
 A production-ready modern Python MongoDB ODM
 
 In addition to synchronous mode, you can use asynchronous mode, just export from `typedmongo.asyncio`.
 
 ## Install
@@ -17,25 +30,21 @@
 <details markdown="1">
 <summary>Example</summary>
 
 ```python
 from motor.motor_asyncio import AsyncIOMotorClient as MongoClient
 
 import typedmongo.asyncio as mongo
-from typedmongo.marshamallow import MarshamallowObjectId
 
 
 class Wallet(mongo.Table):
     balance: mongo.DecimalField
 
 
-class User(mongo.Table):
-    _id: mongo.ObjectIdField = mongo.ObjectIdField(
-        marshamallow=MarshamallowObjectId(required=False)
-    )
+class User(mongo.MongoTable):
     name: mongo.StringField
     age: mongo.IntegerField
     tags: mongo.ListField[str]
     wallet: mongo.EmbeddedField[Wallet]
     created_at: mongo.DateTimeField = mongo.DateTimeField(
         default=lambda: datetime.datetime.now(datetime.timezone.utc)
     )
```

### Comparing `typedmongo-1.1.4/pyproject.toml` & `typedmongo-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "typedmongo"
-version = "1.1.4"
+version = "1.2.0"
 description = "A production-ready modern Python MongoDB ODM"
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "pymongo>=4.6.3",
     "motor>=3.4.0",
```

### Comparing `typedmongo-1.1.4/tests/asyncio/test_client.py` & `typedmongo-1.2.0/tests/asyncio/test_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,30 +2,21 @@
 
 from decimal import Decimal
 
 import pytest
 from motor.motor_asyncio import AsyncIOMotorClient as MongoClient
 
 import typedmongo.asyncio as mongo
-from typedmongo.marshamallow import MarshamallowObjectId
-
-
-class MongoTable(mongo.Table):
-    __abstract__ = True
-
-    _id: mongo.ObjectIdField = mongo.ObjectIdField(
-        marshamallow=MarshamallowObjectId(required=False)
-    )
 
 
 class Wallet(mongo.Table):
     balance: mongo.DecimalField
 
 
-class User(MongoTable):
+class User(mongo.MongoTable):
     name: mongo.StringField
     age: mongo.IntegerField
     tags: mongo.ListField[str]
     wallet: mongo.EmbeddedField[Wallet]
     children: mongo.ListField[User]
 
     @classmethod
@@ -38,15 +29,15 @@
 @pytest.fixture(scope="function", autouse=True)
 async def init_models():
     await mongo.initial_collections(
         MongoClient().mongo,
         User,
     )
     yield
-    await User.objects.drop()
+    await User.objects.collection.drop()
 
 
 async def test_use_objects_in_instance():
     with pytest.raises(AttributeError):
         User.load({}, partial=True).objects
```

### Comparing `typedmongo-1.1.4/tests/asyncio/test_table.py` & `typedmongo-1.2.0/tests/asyncio/test_table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.4/tests/sync.py` & `typedmongo-1.2.0/tests/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.4/tests/test_client.py` & `typedmongo-1.2.0/tests/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,30 +2,21 @@
 
 from decimal import Decimal
 
 import pytest
 from pymongo import MongoClient
 
 import typedmongo as mongo
-from typedmongo.marshamallow import MarshamallowObjectId
-
-
-class MongoTable(mongo.Table):
-    __abstract__ = True
-
-    _id: mongo.ObjectIdField = mongo.ObjectIdField(
-        marshamallow=MarshamallowObjectId(required=False)
-    )
 
 
 class Wallet(mongo.Table):
     balance: mongo.DecimalField
 
 
-class User(MongoTable):
+class User(mongo.MongoTable):
     name: mongo.StringField
     age: mongo.IntegerField
     tags: mongo.ListField[str]
     wallet: mongo.EmbeddedField[Wallet]
     children: mongo.ListField[User]
 
     @classmethod
@@ -38,15 +29,15 @@
 @pytest.fixture(scope="function", autouse=True)
 def init_models():
     mongo.initial_collections(
         MongoClient().mongo,
         User,
     )
     yield
-    User.objects.drop()
+    User.objects.collection.drop()
 
 
 def test_use_objects_in_instance():
     with pytest.raises(AttributeError):
         User.load({}, partial=True).objects
```

### Comparing `typedmongo-1.1.4/tests/test_expressions.py` & `typedmongo-1.2.0/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.4/tests/test_marshamallow.py` & `typedmongo-1.2.0/tests/test_marshamallow.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.4/tests/test_table.py` & `typedmongo-1.2.0/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.4/typedmongo/__init__.py` & `typedmongo-1.2.0/typedmongo/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,25 +16,26 @@
     FieldParamters,
     FloatField,
     IntegerField,
     ListField,
     ObjectIdField,
     StringField,
 )
-from .table import Index, Table
+from .table import Index, MongoTable, Table
 
 __all__ = [
     "DeleteMany",
     "DeleteOne",
     "InsertOne",
     "ReplaceOne",
     "UpdateMany",
     "UpdateOne",
     "initial_collections",
     "Index",
+    "MongoTable",
     "Table",
     "BooleanField",
     "DateTimeField",
     "DecimalField",
     "DictField",
     "EmbeddedField",
     "FieldParamters",
```

### Comparing `typedmongo-1.1.4/typedmongo/asyncio/__init__.py` & `typedmongo-1.2.0/typedmongo/asyncio/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,25 +16,26 @@
     FieldParamters,
     FloatField,
     IntegerField,
     ListField,
     ObjectIdField,
     StringField,
 )
-from .table import Index, Table
+from .table import Index, MongoTable, Table
 
 __all__ = [
     "DeleteMany",
     "DeleteOne",
     "InsertOne",
     "ReplaceOne",
     "UpdateMany",
     "UpdateOne",
     "initial_collections",
     "Index",
+    "MongoTable",
     "Table",
     "BooleanField",
     "DateTimeField",
     "DecimalField",
     "DictField",
     "EmbeddedField",
     "FieldParamters",
```

### Comparing `typedmongo-1.1.4/typedmongo/asyncio/client.py` & `typedmongo-1.2.0/typedmongo/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import dataclasses
 import decimal
 from typing import (
     TYPE_CHECKING,
     Any,
-    AsyncIterable,
+    Iterable,
     Generic,
     Literal,
     Mapping,
     NoReturn,
     Optional,
     TypeAlias,
     TypeVar,
@@ -22,16 +22,16 @@
 from pymongo.operations import DeleteOne as MongoDeleteOne
 from pymongo.operations import InsertOne as MongoInsertOne
 from pymongo.operations import ReplaceOne as MongoReplaceOne
 from pymongo.operations import UpdateMany as MongoUpdateMany
 from pymongo.operations import UpdateOne as MongoUpdateOne
 
 if TYPE_CHECKING:
-    from motor.motor_asyncio import AsyncIOMotorCollection as MongoCollection
-    from motor.motor_asyncio import AsyncIOMotorDatabase as MongoDatabase
+    from pymongo.collection import Collection as MongoCollection
+    from pymongo.database import Database as MongoDatabase
     from pymongo.results import BulkWriteResult as MongoBlukWriteResult
     from pymongo.results import DeleteResult as MongoDeleteResult
     from pymongo.results import UpdateResult as MongoUpdateResult
 
     from .table import Table
 
 from typedmongo.expressions import Expression, OrderBy, compile_expression
@@ -52,26 +52,26 @@
 
     def transform_bson(self, value: Decimal128) -> decimal.Decimal:
         """Function that transforms a vanilla BSON type value into our
         custom type."""
         return value.to_decimal()
 
 
-async def initial_collections(db: MongoDatabase, *tables: type[Table]) -> None:
+def initial_collections(db: MongoDatabase, *tables: type[Table]) -> None:
     for table in tables:
         table.__lazy_init_fields__()
         table.__database__ = db
         type_registry = TypeRegistry([DecimalCodec()])
         codec_options = CodecOptions(type_registry=type_registry)
         table.__collection__ = collection = db.get_collection(
             table.__collection_name__, codec_options=codec_options
         )
         indexes = table.indexes()
         if indexes:
-            await collection.create_indexes(
+            collection.create_indexes(
                 [index.to_index_model() for index in indexes]
             )
 
 
 class Manager:
     @overload
     def __get__(self, instance: None, cls: type[T]) -> Objects[T]: ...
@@ -117,219 +117,181 @@
 )
 
 
 class Objects(Generic[T]):
     def __init__(self, table: type[T]) -> None:
         self.table = table
 
-    async def insert_one(self, document: T) -> DocumentId:
-        # Just for IDE display method docs
-        collection: MongoCollection = self.table.__collection__
+    @property
+    def collection(self) -> MongoCollection:
+        return self.table.__collection__
 
-        insert_result = await collection.insert_one(document.to_mongo())
+    def insert_one(self, document: T) -> DocumentId:
+        insert_result = self.collection.insert_one(document.to_mongo())
         return insert_result.inserted_id
 
-    async def insert_many(
+    def insert_many(
         self, *documents: T, ordered: bool = True
     ) -> list[DocumentId]:
-        # Just for IDE display method docs
-        collection: MongoCollection = self.table.__collection__
-
-        insert_result = await collection.insert_many(
+        insert_result = self.collection.insert_many(
             [document.to_mongo() for document in documents], ordered=ordered
         )
         return insert_result.inserted_ids
 
-    async def find(
+    def find(
         self,
         filter: Optional[Filter] = None,
         projection: Optional[Projection] = None,
         skip: int = 0,
         limit: int = 0,
         sort: Optional[Sort] = None,
         allow_disk_use: Optional[bool] = None,
-    ) -> AsyncIterable[T]:
-        # Just for IDE display method docs
-        collection: MongoCollection = self.table.__collection__
-
-        async for document in collection.find(
+    ) -> Iterable[T]:
+        for document in self.collection.find(
             filter=translate_filter(filter),
             projection=translate_projection(projection),
             skip=skip,
             limit=limit,
             sort=translate_sort(sort),
             allow_disk_use=allow_disk_use,
         ):
             yield self.table.load(document, partial=True)
 
-    async def find_one(
+    def find_one(
         self,
         filter: Optional[Filter] = None,
         projection: Optional[Projection] = None,
         skip: int = 0,
         sort: Optional[Sort] = None,
         allow_disk_use: Optional[bool] = None,
     ) -> T | None:
-        # Just for IDE display method docs
-        collection: MongoCollection = self.table.__collection__
-
-        document = await collection.find_one(
+        document = self.collection.find_one(
             filter=translate_filter(filter),
             projection=translate_projection(projection),
             skip=skip,
             sort=translate_sort(sort),
             allow_disk_use=allow_disk_use,
         )
         if document is None:
             return None
         return self.table.load(document, partial=True)
 
-    async def find_one_and_delete(
+    def find_one_and_delete(
         self,
         filter: Filter,
         projection: Optional[Projection] = None,
         sort: Optional[Sort] = None,
     ) -> T | None:
-        collection: MongoCollection = self.table.__collection__
-
-        document = await collection.find_one_and_delete(
+        document = self.collection.find_one_and_delete(
             filter=translate_filter(filter),
             projection=translate_projection(projection),
             sort=translate_sort(sort),
         )
         if document is None:
             return None
         return self.table.load(document, partial=True)
 
-    async def find_one_and_replace(
+    def find_one_and_replace(
         self,
         filter: Filter,
         replacement: T,
         projection: Optional[Projection] = None,
         sort: Optional[Sort] = None,
         upsert: bool = False,
         after_document: bool = False,
     ) -> T | None:
-        collection: MongoCollection = self.table.__collection__
-
-        document = await collection.find_one_and_replace(
+        document = self.collection.find_one_and_replace(
             filter=translate_filter(filter),
             replacement=replacement.to_mongo(),
             projection=translate_projection(projection),
             sort=translate_sort(sort),
             upsert=upsert,
             return_document=after_document,
         )
         if document is None:
             return None
         return self.table.load(document, partial=True)
 
-    async def find_one_and_update(
+    def find_one_and_update(
         self,
         filter: Filter,
         update: Mapping[str, Any] | list[Mapping[str, Any]],
         projection: Optional[Projection] = None,
         sort: Optional[Sort] = None,
         upsert: bool = False,
         after_document: bool = False,
     ) -> T | None:
-        collection: MongoCollection = self.table.__collection__
-
-        document = await collection.find_one_and_update(
+        document = self.collection.find_one_and_update(
             filter=translate_filter(filter),
             update=update,
             projection=translate_projection(projection),
             sort=translate_sort(sort),
             upsert=upsert,
             return_document=after_document,
         )
         if document is None:
             return None
         return self.table.load(document, partial=True)
 
-    async def delete_one(
+    def delete_one(
         self,
         filter: Optional[Filter] = None,
     ) -> MongoDeleteResult:
-        # Just for IDE display method docs
-        collection: MongoCollection = self.table.__collection__
-
-        return await collection.delete_one(translate_filter(filter))
+        return self.collection.delete_one(translate_filter(filter))
 
-    async def delete_many(
+    def delete_many(
         self,
         filter: Optional[Filter] = None,
     ) -> MongoDeleteResult:
-        # Just for IDE display method docs
-        collection: MongoCollection = self.table.__collection__
+        return self.collection.delete_many(translate_filter(filter))
 
-        return await collection.delete_many(translate_filter(filter))
-
-    async def update_one(
+    def update_one(
         self,
         filter: Filter,
         update: Mapping[str, Any] | list[Mapping[str, Any]],
         upsert: bool = False,
     ) -> MongoUpdateResult:
-        # Just for IDE display method docs
-        collection: MongoCollection = self.table.__collection__
-
-        return await collection.update_one(
+        return self.collection.update_one(
             translate_filter(filter),
             update,
             upsert=upsert,
         )
 
-    async def update_many(
+    def update_many(
         self,
         filter: Filter,
         update: Mapping[str, Any] | list[Mapping[str, Any]],
         upsert: bool = False,
     ) -> MongoUpdateResult:
-        # Just for IDE display method docs
-        collection: MongoCollection = self.table.__collection__
-
-        return await collection.update_many(
+        return self.collection.update_many(
             translate_filter(filter),
             update,
             upsert=upsert,
         )
 
-    async def count_documents(
+    def count_documents(
         self,
         filter: Filter,
     ) -> int:
-        # Just for IDE display method docs
-        collection: MongoCollection = self.table.__collection__
-
-        return await collection.count_documents(translate_filter(filter))
+        return self.collection.count_documents(translate_filter(filter))
 
-    async def bulk_write(
+    def bulk_write(
         self,
         *requests: DeleteMany
         | DeleteOne
         | InsertOne[T]
         | ReplaceOne[T]
         | UpdateMany
         | UpdateOne,
         ordered: bool = True,
     ) -> MongoBlukWriteResult:
-        # Just for IDE display method docs
-        collection: MongoCollection = self.table.__collection__
-
-        return await collection.bulk_write(
+        return self.collection.bulk_write(
             [r.to_mongo() for r in requests], ordered=ordered
         )
 
-    async def drop(self) -> None:
-        # Just for IDE display method docs
-        collection: MongoCollection = self.table.__collection__
-
-        await collection.drop()
-
 
 @dataclasses.dataclass
 class DeleteMany:
     filter: Filter
 
     def to_mongo(self) -> MongoDeleteMany:
         return MongoDeleteMany(translate_filter(self.filter))
```

### Comparing `typedmongo-1.1.4/typedmongo/asyncio/fields.py` & `typedmongo-1.2.0/typedmongo/asyncio/fields.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.4/typedmongo/asyncio/table.py` & `typedmongo-1.2.0/typedmongo/asyncio/table.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 )
 
 from marshmallow import Schema
 from pymongo import IndexModel
 from typing_extensions import Self, dataclass_transform
 
 from typedmongo.exceptions import TableDefineError
+from typedmongo.marshamallow import MarshamallowObjectId
 
 from .client import Manager
-from .fields import Field, ListField, type_to_field
+from .fields import Field, ListField, ObjectIdField, type_to_field
 
 
 def snake_case(name: str) -> str:
     """
     convert "SomeWords" to "some_words"
     """
     return "".join(
@@ -150,60 +151,56 @@
         for name, field in fields.items():
             setattr(cls, name, field)
             field.__set_name__(cls, name)
 
         cls.__schema__ = cls.__create_schema__(cls.__name__, cls.__fields__)
         return fields
 
-    def __call__(cls, **kwargs: Any):
-        instance = super().__call__()
+    def __setattr__(cls, name, value):
+        if name == "__abstract__":
+            raise AttributeError(
+                "Can't modify the `__abstract__` attribute dynamically."
+            )
+        return super().__setattr__(name, value)
+
+
+class Table(metaclass=TableMetaClass):
+    __abstract__ = True
+
+    objects = Manager()
 
-        if instance.__abstract__:
+    def __init__(self, **kwargs):
+        if self.__abstract__:
             raise RuntimeError(
                 "The class {} cannot be instantiated, because it's __abstract__ is True.".format(
-                    cls.__name__
+                    self.__class__.__name__
                 )
             )
 
-        for name, field in cls.__fields__.items():
+        for name, field in self.__class__.__fields__.items():
             if name in kwargs:
                 value = kwargs.pop(name)
             else:
                 if field.default is None:
                     continue
                 default_value = field.default
                 if callable(default_value):
                     value = default_value()
                 else:
                     value = default_value
-            setattr(instance, name, value)
+            setattr(self, name, value)
 
         if kwargs:
             raise TypeError(
                 "{class_name}() got unexpected keyword arguments '{unexpected}'".format(
-                    class_name=cls.__name__,
+                    class_name=self.__class__.__name__,
                     unexpected="', '".join(kwargs.keys()),
                 )
             )
 
-        return instance
-
-    def __setattr__(cls, name, value):
-        if name == "__abstract__":
-            raise AttributeError(
-                "Can't modify the `__abstract__` attribute dynamically."
-            )
-        return super().__setattr__(name, value)
-
-
-class Table(metaclass=TableMetaClass):
-    __abstract__ = True
-
-    objects = Manager()
-
     def __repr__(self) -> str:
         return "{class_name}({fields})".format(
             class_name=self.__class__.__name__,
             fields=", ".join(
                 f"{name}={repr(self.__dict__[name])}"
                 for name, _ in self.__fields__.items()
                 if name in self.__dict__
@@ -253,7 +250,15 @@
         """
         Dump the instance to dict for mongo.
         """
         return {
             key: getattr(self.__fields__[key], "to_mongo")(value)
             for key, value in self.__dict__.items()
         }
+
+
+class MongoTable(Table):
+    __abstract__ = True
+
+    _id: ObjectIdField = ObjectIdField(
+        marshamallow=MarshamallowObjectId(required=False)
+    )
```

### Comparing `typedmongo-1.1.4/typedmongo/expressions.py` & `typedmongo-1.2.0/typedmongo/expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.4/typedmongo/fields.py` & `typedmongo-1.2.0/typedmongo/fields.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.4/typedmongo/marshamallow.py` & `typedmongo-1.2.0/typedmongo/marshamallow.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.4/typedmongo/sync.py` & `typedmongo-1.2.0/typedmongo/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.1.4/typedmongo/table.py` & `typedmongo-1.2.0/typedmongo/table.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 )
 
 from marshmallow import Schema
 from pymongo import IndexModel
 from typing_extensions import Self, dataclass_transform
 
 from typedmongo.exceptions import TableDefineError
+from typedmongo.marshamallow import MarshamallowObjectId
 
 from .client import Manager
-from .fields import Field, ListField, type_to_field
+from .fields import Field, ListField, ObjectIdField, type_to_field
 
 
 def snake_case(name: str) -> str:
     """
     convert "SomeWords" to "some_words"
     """
     return "".join(
@@ -150,60 +151,56 @@
         for name, field in fields.items():
             setattr(cls, name, field)
             field.__set_name__(cls, name)
 
         cls.__schema__ = cls.__create_schema__(cls.__name__, cls.__fields__)
         return fields
 
-    def __call__(cls, **kwargs: Any):
-        instance = super().__call__()
+    def __setattr__(cls, name, value):
+        if name == "__abstract__":
+            raise AttributeError(
+                "Can't modify the `__abstract__` attribute dynamically."
+            )
+        return super().__setattr__(name, value)
+
+
+class Table(metaclass=TableMetaClass):
+    __abstract__ = True
+
+    objects = Manager()
 
-        if instance.__abstract__:
+    def __init__(self, **kwargs):
+        if self.__abstract__:
             raise RuntimeError(
                 "The class {} cannot be instantiated, because it's __abstract__ is True.".format(
-                    cls.__name__
+                    self.__class__.__name__
                 )
             )
 
-        for name, field in cls.__fields__.items():
+        for name, field in self.__class__.__fields__.items():
             if name in kwargs:
                 value = kwargs.pop(name)
             else:
                 if field.default is None:
                     continue
                 default_value = field.default
                 if callable(default_value):
                     value = default_value()
                 else:
                     value = default_value
-            setattr(instance, name, value)
+            setattr(self, name, value)
 
         if kwargs:
             raise TypeError(
                 "{class_name}() got unexpected keyword arguments '{unexpected}'".format(
-                    class_name=cls.__name__,
+                    class_name=self.__class__.__name__,
                     unexpected="', '".join(kwargs.keys()),
                 )
             )
 
-        return instance
-
-    def __setattr__(cls, name, value):
-        if name == "__abstract__":
-            raise AttributeError(
-                "Can't modify the `__abstract__` attribute dynamically."
-            )
-        return super().__setattr__(name, value)
-
-
-class Table(metaclass=TableMetaClass):
-    __abstract__ = True
-
-    objects = Manager()
-
     def __repr__(self) -> str:
         return "{class_name}({fields})".format(
             class_name=self.__class__.__name__,
             fields=", ".join(
                 f"{name}={repr(self.__dict__[name])}"
                 for name, _ in self.__fields__.items()
                 if name in self.__dict__
@@ -253,7 +250,15 @@
         """
         Dump the instance to dict for mongo.
         """
         return {
             key: getattr(self.__fields__[key], "to_mongo")(value)
             for key, value in self.__dict__.items()
         }
+
+
+class MongoTable(Table):
+    __abstract__ = True
+
+    _id: ObjectIdField = ObjectIdField(
+        marshamallow=MarshamallowObjectId(required=False)
+    )
```

### Comparing `typedmongo-1.1.4/PKG-INFO` & `typedmongo-1.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: typedmongo
-Version: 1.1.4
-Summary: A production-ready modern Python MongoDB ODM
-Author-Email: abersheeran <me@abersheeran.com>
-License: Apache2.0
-Requires-Python: >=3.10
-Requires-Dist: pymongo>=4.6.3
-Requires-Dist: motor>=3.4.0
-Requires-Dist: marshmallow>=3.21.1
-Requires-Dist: typing-extensions>=4.11.0
-Description-Content-Type: text/markdown
-
 # Typed Mongo
 
 A production-ready modern Python MongoDB ODM
 
 In addition to synchronous mode, you can use asynchronous mode, just export from `typedmongo.asyncio`.
 
 ## Install
@@ -30,25 +17,21 @@
 <details markdown="1">
 <summary>Example</summary>
 
 ```python
 from motor.motor_asyncio import AsyncIOMotorClient as MongoClient
 
 import typedmongo.asyncio as mongo
-from typedmongo.marshamallow import MarshamallowObjectId
 
 
 class Wallet(mongo.Table):
     balance: mongo.DecimalField
 
 
-class User(mongo.Table):
-    _id: mongo.ObjectIdField = mongo.ObjectIdField(
-        marshamallow=MarshamallowObjectId(required=False)
-    )
+class User(mongo.MongoTable):
     name: mongo.StringField
     age: mongo.IntegerField
     tags: mongo.ListField[str]
     wallet: mongo.EmbeddedField[Wallet]
     created_at: mongo.DateTimeField = mongo.DateTimeField(
         default=lambda: datetime.datetime.now(datetime.timezone.utc)
     )
```

