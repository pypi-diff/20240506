# Comparing `tmp/joker-mongodb-0.2.0.tar.gz` & `tmp/joker-mongodb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joker-mongodb-0.2.0.tar", last modified: Thu Apr 25 06:00:07 2024, max compression
+gzip compressed data, was "joker-mongodb-0.3.0.tar", last modified: Mon May  6 02:57:45 2024, max compression
```

## Comparing `joker-mongodb-0.2.0.tar` & `joker-mongodb-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-25 06:00:07.960088 joker-mongodb-0.2.0/
--rw-r--r--   0 Hailong    (502) staff       (20)    35149 2021-07-11 03:40:54.000000 joker-mongodb-0.2.0/LICENSE
--rw-r--r--   0 Hailong    (502) staff       (20)       41 2021-07-11 03:42:23.000000 joker-mongodb-0.2.0/MANIFEST.in
--rw-r--r--   0 Hailong    (502) staff       (20)     2578 2024-04-25 06:00:07.959333 joker-mongodb-0.2.0/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)     1574 2022-05-25 12:06:36.000000 joker-mongodb-0.2.0/README.md
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-25 06:00:07.946801 joker-mongodb-0.2.0/joker/
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-25 06:00:07.949415 joker-mongodb-0.2.0/joker/mongodb/
--rw-r--r--   0 Hailong    (502) staff       (20)      159 2024-04-25 05:56:42.000000 joker-mongodb-0.2.0/joker/mongodb/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     6408 2022-03-14 03:26:26.000000 joker-mongodb-0.2.0/joker/mongodb/interfaces.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1873 2021-10-24 02:15:04.000000 joker-mongodb-0.2.0/joker/mongodb/legacy.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-25 06:00:07.955064 joker-mongodb-0.2.0/joker/mongodb/tools/
--rw-r--r--   0 Hailong    (502) staff       (20)       39 2021-07-11 03:25:17.000000 joker-mongodb-0.2.0/joker/mongodb/tools/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1294 2022-01-26 16:25:20.000000 joker-mongodb-0.2.0/joker/mongodb/tools/cmdline.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1081 2022-01-26 15:39:10.000000 joker-mongodb-0.2.0/joker/mongodb/tools/dumping.py
--rw-r--r--   0 Hailong    (502) staff       (20)      208 2022-03-23 11:39:14.000000 joker-mongodb-0.2.0/joker/mongodb/tools/experimental.py
--rw-r--r--   0 Hailong    (502) staff       (20)      739 2021-07-11 10:35:01.000000 joker-mongodb-0.2.0/joker/mongodb/tools/filters.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1454 2021-07-15 15:19:30.000000 joker-mongodb-0.2.0/joker/mongodb/tools/integrity.py
--rw-r--r--   0 Hailong    (502) staff       (20)      639 2021-10-22 13:21:36.000000 joker-mongodb-0.2.0/joker/mongodb/tools/kvstore.py
--rw-r--r--   0 Hailong    (502) staff       (20)     9769 2021-11-24 13:07:47.000000 joker-mongodb-0.2.0/joker/mongodb/tools/misc.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1053 2022-02-24 13:25:47.000000 joker-mongodb-0.2.0/joker/mongodb/tools/mongoshell.py
--rw-r--r--   0 Hailong    (502) staff       (20)     5473 2022-12-02 03:57:24.000000 joker-mongodb-0.2.0/joker/mongodb/tools/oplog.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1173 2022-06-02 08:07:27.000000 joker-mongodb-0.2.0/joker/mongodb/tools/querying.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3917 2022-05-25 11:59:41.000000 joker-mongodb-0.2.0/joker/mongodb/tools/schema.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1160 2022-04-08 10:50:53.000000 joker-mongodb-0.2.0/joker/mongodb/tools/transactional.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3695 2022-01-26 15:43:57.000000 joker-mongodb-0.2.0/joker/mongodb/utils.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-25 06:00:07.958551 joker-mongodb-0.2.0/joker_mongodb.egg-info/
--rw-r--r--   0 Hailong    (502) staff       (20)     2578 2024-04-25 06:00:07.000000 joker-mongodb-0.2.0/joker_mongodb.egg-info/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)      837 2024-04-25 06:00:07.000000 joker-mongodb-0.2.0/joker_mongodb.egg-info/SOURCES.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2024-04-25 06:00:07.000000 joker-mongodb-0.2.0/joker_mongodb.egg-info/dependency_links.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-04-25 06:00:07.000000 joker-mongodb-0.2.0/joker_mongodb.egg-info/namespace_packages.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2022-05-25 12:01:12.000000 joker-mongodb-0.2.0/joker_mongodb.egg-info/not-zip-safe
--rw-r--r--   0 Hailong    (502) staff       (20)       86 2024-04-25 06:00:07.000000 joker-mongodb-0.2.0/joker_mongodb.egg-info/requires.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-04-25 06:00:07.000000 joker-mongodb-0.2.0/joker_mongodb.egg-info/top_level.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       86 2024-04-25 05:57:29.000000 joker-mongodb-0.2.0/requirements.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       38 2024-04-25 06:00:07.960228 joker-mongodb-0.2.0/setup.cfg
--rw-r--r--   0 Hailong    (502) staff       (20)     2205 2024-04-25 05:58:45.000000 joker-mongodb-0.2.0/setup.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-05-06 02:57:45.697944 joker-mongodb-0.3.0/
+-rw-r--r--   0 Hailong    (502) staff       (20)    35149 2021-07-11 03:40:54.000000 joker-mongodb-0.3.0/LICENSE
+-rw-r--r--   0 Hailong    (502) staff       (20)       41 2021-07-11 03:42:23.000000 joker-mongodb-0.3.0/MANIFEST.in
+-rw-r--r--   0 Hailong    (502) staff       (20)     2528 2024-05-06 02:57:45.697462 joker-mongodb-0.3.0/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)     1574 2022-05-25 12:06:36.000000 joker-mongodb-0.3.0/README.md
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-05-06 02:57:45.681595 joker-mongodb-0.3.0/joker/
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-05-06 02:57:45.684970 joker-mongodb-0.3.0/joker/mongodb/
+-rw-r--r--   0 Hailong    (502) staff       (20)      163 2024-05-06 02:51:05.000000 joker-mongodb-0.3.0/joker/mongodb/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     6378 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/interfaces.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1857 2024-04-25 06:15:26.000000 joker-mongodb-0.3.0/joker/mongodb/legacy.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-05-06 02:57:45.693579 joker-mongodb-0.3.0/joker/mongodb/tools/
+-rw-r--r--   0 Hailong    (502) staff       (20)       39 2021-07-11 03:25:17.000000 joker-mongodb-0.3.0/joker/mongodb/tools/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1329 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/cmdline.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1115 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/dumping.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      242 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/experimental.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      763 2024-04-25 06:14:37.000000 joker-mongodb-0.3.0/joker/mongodb/tools/filters.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1514 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/integrity.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      674 2024-04-25 06:18:35.000000 joker-mongodb-0.3.0/joker/mongodb/tools/kvstore.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     9804 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/misc.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1088 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/mongoshell.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     5520 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/oplog.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1709 2024-05-06 02:51:05.000000 joker-mongodb-0.3.0/joker/mongodb/tools/paginations.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1161 2024-04-25 06:08:49.000000 joker-mongodb-0.3.0/joker/mongodb/tools/querying.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     3917 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/schema.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1207 2024-04-25 06:16:01.000000 joker-mongodb-0.3.0/joker/mongodb/tools/transactional.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     3738 2024-04-25 06:13:43.000000 joker-mongodb-0.3.0/joker/mongodb/utils.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-05-06 02:57:45.697100 joker-mongodb-0.3.0/joker_mongodb.egg-info/
+-rw-r--r--   0 Hailong    (502) staff       (20)     2528 2024-05-06 02:57:45.000000 joker-mongodb-0.3.0/joker_mongodb.egg-info/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)      872 2024-05-06 02:57:45.000000 joker-mongodb-0.3.0/joker_mongodb.egg-info/SOURCES.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2024-05-06 02:57:45.000000 joker-mongodb-0.3.0/joker_mongodb.egg-info/dependency_links.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-05-06 02:57:45.000000 joker-mongodb-0.3.0/joker_mongodb.egg-info/namespace_packages.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2022-05-25 12:01:12.000000 joker-mongodb-0.3.0/joker_mongodb.egg-info/not-zip-safe
+-rw-r--r--   0 Hailong    (502) staff       (20)       86 2024-05-06 02:57:45.000000 joker-mongodb-0.3.0/joker_mongodb.egg-info/requires.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-05-06 02:57:45.000000 joker-mongodb-0.3.0/joker_mongodb.egg-info/top_level.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       86 2024-04-25 05:57:29.000000 joker-mongodb-0.3.0/requirements.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       38 2024-05-06 02:57:45.698008 joker-mongodb-0.3.0/setup.cfg
+-rw-r--r--   0 Hailong    (502) staff       (20)     2147 2024-04-25 06:23:26.000000 joker-mongodb-0.3.0/setup.py
```

### Comparing `joker-mongodb-0.2.0/LICENSE` & `joker-mongodb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.2.0/PKG-INFO` & `joker-mongodb-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: joker-mongodb
-Version: 0.2.0
+Version: 0.3.0
 Summary: access mongodb with handy utilities and fun
 Home-page: https://github.com/frozflame/joker-mongodb
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joker-cast>=0.5.0
 Requires-Dist: joker-textmanip>=0.3.1
 Requires-Dist: joker>=0.3.3
 Requires-Dist: pymongo>=3.11.0
 Requires-Dist: volkanic>=0.5.1
```

### Comparing `joker-mongodb-0.2.0/README.md` & `joker-mongodb-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `joker-mongodb-0.2.0/joker/mongodb/interfaces.py` & `joker-mongodb-0.3.0/joker/mongodb/interfaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 # coding: utf-8
+from __future__ import annotations
 
 from collections import defaultdict
 from typing import Union
 
 import pymongo.errors
 from bson import ObjectId, json_util
 from gridfs import GridFS
@@ -30,15 +31,15 @@
         return kvstore.kv_load(self._coll, key)
 
     def kv_save(self, key: str, val):
         return kvstore.kv_save(self._coll, key, val)
 
     def find_recent_by_count(self, count=50) -> Cursor:
         cursor = self._coll.find(self.filtr, projection=self.projection)
-        return cursor.sort([('_id', -1)]).limit(count)
+        return cursor.sort([("_id", -1)]).limit(count)
 
     def find_most_recent_one(self) -> dict:
         recs = list(self.find_recent_by_count(1))
         if recs:
             return recs[0]
 
     def _insert(self, records):
@@ -46,109 +47,106 @@
             self._coll.insert_many(records, ordered=False)
 
     @staticmethod
     def _check_for_uniqueness(records, uk):
         vals = [r.get(uk) for r in records]
         uniq_vals = set(vals)
         if len(vals) != len(uniq_vals):
-            raise ValueError('records contain duplicating keys')
+            raise ValueError("records contain duplicating keys")
 
     def make_fusion_record(self):
         fusion_record = {}
         contiguous_stale_count = -1
         for skip in range(1000):
-            record = self._coll.find_one(sort=[('$natural', -1)], skip=skip)
+            record = self._coll.find_one(sort=[("$natural", -1)], skip=skip)
             if not record:
                 continue
             contiguous_stale_count += 1
             for key, val in record.items():
                 if not record.get(key):
                     fusion_record[key] = val
                     contiguous_stale_count = -1
             if contiguous_stale_count > 10:
                 return fusion_record
         return fusion_record
 
     def query_uniq_values(self, fields: list, limit=1000):
-        latest = [('_id', -1)]
+        latest = [("_id", -1)]
         records = self._coll.find(sort=latest, projection=fields, limit=limit)
         uniq = defaultdict(set)
         for key in fields:
             for rec in records:
                 val = rec.get(key)
                 uniq[key].add(val)
         return uniq
 
 
 class MongoInterface:
     """A interface for multiple mongodb clusters."""
 
     def __init__(
-            self, hosts: dict,
-            default: str = 'localhost.default',
-            aliases: dict = None):
-        self.default_host, self.default_db_name = default.split('.')
+        self, hosts: dict, default: str = "localhost.default", aliases: dict = None
+    ):
+        self.default_host, self.default_db_name = default.split(".")
         self.hosts = hosts
         self.aliases = aliases or {}
         self._clients = {}
 
     @classmethod
     def from_config(cls, options: dict):
         params = {
-            'default': options.pop('_default', None),
-            'aliases': options.pop('_aliases', None),
+            "default": options.pop("_default", None),
+            "aliases": options.pop("_aliases", None),
         }
         return cls(options, **params)
 
     def get_mongo(self, host: str = None) -> MongoClient:
         if host is None:
             host = self.default_host
         try:
             return self._clients[host]
         except KeyError:
             pass
         # host pass through as MongoClient argument
         params = self.hosts.get(host, host)
         if isinstance(params, str):
-            params = {'host': params}
+            params = {"host": params}
         return self._clients.setdefault(host, MongoClient(**params))
 
     @property
     def db(self) -> Database:
         return self.get_db(self.default_host, self.default_db_name)
 
     def _check_coll_triple(self, names: tuple) -> tuple:
         n = len(names)
         if n == 1:
             return self.default_host, self.default_db_name, names[0]
         elif n == 3:
             return names
         else:
             c = self.__class__.__name__
-            msg = 'requires 1 or 3 arguments, got {}'.format(c, n)
+            msg = "requires 1 or 3 arguments, got {}".format(c, n)
             raise ValueError(msg)
 
     def __call__(self, *names) -> Collection:
         names = self._check_coll_triple(names)
         return self.get_coll(*names)
 
     def get_db(self, host: str, db_name: str) -> Database:
         mongo = self.get_mongo(host)
         db_name = self.aliases.get(db_name, db_name)
         return mongo.get_database(db_name)
 
-    def get_coll(self, host: str, db_name: str, coll_name: str) \
-            -> Collection:
+    def get_coll(self, host: str, db_name: str, coll_name: str) -> Collection:
         db = self.get_db(host, db_name)
         return db.get_collection(coll_name)
 
-    def get_gridfs(self, host: str, db_name: str, coll_name: str = 'fs') \
-            -> GridFS:
-        assert not coll_name.endswith('.files')
-        assert not coll_name.endswith('.chunks')
+    def get_gridfs(self, host: str, db_name: str, coll_name: str = "fs") -> GridFS:
+        assert not coll_name.endswith(".files")
+        assert not coll_name.endswith(".chunks")
         db = self.get_db(host, db_name)
         return GridFS(db, collection=coll_name)
 
 
 class MongoInterfaceExtended(MongoInterface):
     def _get_target(self, host: str, db_name: str = None):
         if db_name is None:
@@ -165,25 +163,24 @@
 
     def get_ci(self, *names, **kwargs) -> CollectionInterface:
         coll = self.__call__(*names)
         return CollectionInterface(coll, **kwargs)
 
     # TODO: support BSON
     def restore_a_file(self, lines, inner_path: str, empty_coll_only=True):
-        host, db_name, coll_name = \
-            utils.infer_coll_triple_from_filename(inner_path)
-        if coll_name == 'system.indexes':
+        host, db_name, coll_name = utils.infer_coll_triple_from_filename(inner_path)
+        if coll_name == "system.indexes":
             return
         coll = self.get_coll(host, db_name, coll_name)
         if empty_coll_only and coll.find_one(projection=[]):
-            printerr(inner_path, 'skipped')
+            printerr(inner_path, "skipped")
             return
         for ix, line in enumerate(lines):
             doc = json_util.loads(line)
-            id_ = doc.get('_id', '')
-            printerr(inner_path, ix, id_, '...', end=' ')
+            id_ = doc.get("_id", "")
+            printerr(inner_path, ix, id_, "...", end=" ")
             try:
                 coll.insert_one(doc)
             except pymongo.errors.DuplicateKeyError:
-                printerr('DuplicateKeyError')
+                printerr("DuplicateKeyError")
             else:
-                printerr('completed')
+                printerr("completed")
```

### Comparing `joker-mongodb-0.2.0/joker/mongodb/legacy.py` & `joker-mongodb-0.3.0/joker/mongodb/legacy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 #!/usr/bin/env python3
 # coding: utf-8
-
-"""
-This module is DEPRECATED.
-"""
+"""This module is DEPRECATED."""
 
 from gridfs import GridFS
 from pymongo import MongoClient
 from pymongo.collection import Collection
 from pymongo.database import Database
 
 from joker.mongodb import utils
@@ -48,14 +45,13 @@
         db = self.get_database(db_name)
         return db.get_collection(coll_name)
 
     def get_ci(self, db_name: str, coll_name: str) -> CollectionInterface:
         coll = self.get_coll(db_name, coll_name)
         return CollectionInterface(coll)
 
-    def get_gridfs(self, db_name: str, coll_name: str = 'fs') \
-            -> GridFS:
+    def get_gridfs(self, db_name: str, coll_name: str = "fs") -> GridFS:
         # avoid names like "images.files.files"
-        if coll_name.endswith('.files') or coll_name.endswith('.chunks'):
-            coll_name = coll_name.rsplit('.', 1)[0]
+        if coll_name.endswith(".files") or coll_name.endswith(".chunks"):
+            coll_name = coll_name.rsplit(".", 1)[0]
         db = self.get_database(db_name)
-        return GridFS(db, collection=coll_name)
+        return GridFS(db, collection=coll_name)
```

### Comparing `joker-mongodb-0.2.0/joker/mongodb/tools/cmdline.py` & `joker-mongodb-0.3.0/joker/mongodb/tools/cmdline.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 #!/usr/bin/env python3
 # coding: utf-8
+from __future__ import annotations
 
 import argparse
 
 from volkanic.cmdline import CommandOptionDict
 
 
 def _add_hyphens(parts: list) -> list:
     if not parts:
         return parts
     key = str(parts[0])
-    if not key.startswith('-'):
-        prefix = '--' if len(key) > 1 else '-'
+    if not key.startswith("-"):
+        prefix = "--" if len(key) > 1 else "-"
         key = prefix + key
     return [key] + parts[1:]
 
 
 class CommandOptionDictMongoish(CommandOptionDict):
     @classmethod
     def _explode(cls, key, val):
         parts = super()._explode(key, val)
         parts = _add_hyphens(parts)
         if len(parts) != 2:
             return parts
         key, val = parts
-        if key.startswith('--'):
-            return [f'{key}={val}']
+        if key.startswith("--"):
+            return [f"{key}={val}"]
 
 
 class ArgumentParserMongoish(argparse.ArgumentParser):
     def add_argument_mongoi_host(self):
-        self.add_argument('-H', '--host', help='host as in MongoInterface')
+        self.add_argument("-H", "--host", help="host as in MongoInterface")
 
-    def add_arguments_host_port(self, hostname='127.0.0.1'):
+    def add_arguments_host_port(self, hostname="127.0.0.1"):
         add = self.add_argument
-        add('-H', '--hostname', default=hostname, help='hostname')
-        add('-p', '--port', type=int, default=27017, help='port number')
+        add("-H", "--hostname", default=hostname, help="hostname")
+        add("-p", "--port", type=int, default=27017, help="port number")
 
     def add_argument_db_name(self):
-        self.add_argument('-d', '--db-name', help='database name')
+        self.add_argument("-d", "--db-name", help="database name")
 
     def add_argument_coll_name(self):
-        self.add_argument('-c', '--coll-name', help='collection name')
+        self.add_argument("-c", "--coll-name", help="collection name")
```

### Comparing `joker-mongodb-0.2.0/joker/mongodb/tools/dumping.py` & `joker-mongodb-0.3.0/joker/mongodb/tools/dumping.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # coding: utf-8
-
+from __future__ import annotations
 
 from typing import List
 from joker.mongodb.tools.cmdline import CommandOptionDictMongoish
 
 import re
 from pymongo.database import Database
 from joker.mongodb import utils
```

### Comparing `joker-mongodb-0.2.0/joker/mongodb/tools/filters.py` & `joker-mongodb-0.3.0/joker/mongodb/tools/filters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 #!/usr/bin/env python3
 # coding: utf-8
+from __future__ import annotations
 
 import datetime
 
 from bson import ObjectId
 
 
 def in_(vals):
-    return {'$in': vals}
+    return {"$in": vals}
 
 
 def exclude(keys):
     return {k: False for k in keys}
 
 
 def exists(*keys):
-    return {k: {'$exists': True} for k in keys}
+    return {k: {"$exists": True} for k in keys}
 
 
 def oid_filter_by_datetime(
-        start: datetime.datetime = None,
-        end: datetime.datetime = None) -> dict:
+    start: datetime.datetime = None, end: datetime.datetime = None
+) -> dict:
     filtr = {}
     if start is not None:
-        filtr['$gt'] = ObjectId.from_datetime(start)
+        filtr["$gt"] = ObjectId.from_datetime(start)
     if end:
-        filtr['$lt'] = ObjectId.from_datetime(end)
+        filtr["$lt"] = ObjectId.from_datetime(end)
     return filtr
 
 
 def oid_filter_recent(days=30, seconds=0):
     delta = datetime.timedelta(days=days, seconds=seconds)
     start = datetime.datetime.now() - delta
     return oid_filter_by_datetime(start, None)
```

### Comparing `joker-mongodb-0.2.0/joker/mongodb/tools/integrity.py` & `joker-mongodb-0.3.0/joker/mongodb/tools/integrity.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 #!/usr/bin/env python3
 # coding: utf-8
+from __future__ import annotations
+
 
 import datetime
 
 from pymongo.collection import Collection, ReturnDocument
 from pymongo.errors import DuplicateKeyError
 
 
 class SerialNumber:
-    __slots__ = ['prefix', 'number', 'length']
+    __slots__ = ["prefix", "number", "length"]
 
     @staticmethod
     def _get_collection() -> Collection:
         raise NotImplementedError
 
-    def __init__(self, prefix='ID', length=6):
+    def __init__(self, prefix="ID", length=6):
         coll = self._get_collection()
         doc = coll.find_one_and_update(
-            {'_id': prefix}, {'$inc': {'i': 1}},
-            upsert=True, return_document=ReturnDocument.AFTER,
+            {"_id": prefix},
+            {"$inc": {"i": 1}},
+            upsert=True,
+            return_document=ReturnDocument.AFTER,
         )
         self.prefix = prefix
-        self.number = doc['i']
+        self.number = doc["i"]
         self.length = length
 
     def __str__(self):
         return self.prefix + str(self.number).zfill(self.length)
 
 
 class NamedLock(object):
@@ -37,17 +41,17 @@
         self.name = name
         self.coll = self._get_collection()
         self.ttl = ttl
 
     def acquire(self):
         now = datetime.datetime.now()
         expire_at = now + datetime.timedelta(seconds=self.ttl)
-        self.coll.delete_many({'expire_at': {'$lt': now}})
-        record = {'_id': self.name, 'expire_at': expire_at}
+        self.coll.delete_many({"expire_at": {"$lt": now}})
+        record = {"_id": self.name, "expire_at": expire_at}
         try:
             self.coll.insert_one(record)
         except DuplicateKeyError:
             return False
         return True
 
     def release(self):
-        self.coll.delete_one({'_id': self.name})
+        self.coll.delete_one({"_id": self.name})
```

### Comparing `joker-mongodb-0.2.0/joker/mongodb/tools/kvstore.py` & `joker-mongodb-0.3.0/joker/mongodb/tools/kvstore.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python3
 # coding: utf-8
+from __future__ import annotations
 
 from pymongo.collection import Collection
 
 
 def kv_load(coll: Collection, key: str):
-    doc = coll.find_one({'_id': key}, projection={'_id': False})
+    doc = coll.find_one({"_id": key}, projection={"_id": False})
     if doc is None:
         return
     try:
-        return doc['_']
+        return doc["_"]
     except KeyError:
         return doc
 
 
 def kv_save(coll: Collection, key: str, val):
-    filtr = {'_id': key}
+    filtr = {"_id": key}
     # explode dict if '_' and '_id' are not in it -- be less nested
-    if isinstance(val, dict) and '_' not in val and '_id' not in val:
+    if isinstance(val, dict) and "_" not in val and "_id" not in val:
         replacement = val
     else:
-        replacement = {'_': val}
+        replacement = {"_": val}
     return coll.replace_one(filtr, replacement, upsert=True)
```

### Comparing `joker-mongodb-0.2.0/joker/mongodb/tools/misc.py` & `joker-mongodb-0.3.0/joker/mongodb/tools/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 # coding: utf-8
+from __future__ import annotations
 
 import csv
 import datetime
 import functools
 import logging
 import sys
 import traceback
```

### Comparing `joker-mongodb-0.2.0/joker/mongodb/tools/mongoshell.py` & `joker-mongodb-0.3.0/joker/mongodb/tools/mongoshell.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 # coding: utf-8
+from __future__ import annotations
 
 import re
 import json
 
 from bson.json_util import loads
 import datetime
```

### Comparing `joker-mongodb-0.2.0/joker/mongodb/tools/oplog.py` & `joker-mongodb-0.3.0/joker/mongodb/tools/oplog.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,154 +17,160 @@
 
 _logger = logging.getLogger(__name__)
 
 
 class OplogRecord(UserDict):
     @property
     def op(self) -> str:
-        return self.data.get('op')
+        return self.data.get("op")
 
     @property
     def ns(self) -> str:
-        return self.data.get('ns')
+        return self.data.get("ns")
 
     @property
     def ts(self) -> Timestamp:
-        return self.data.get('ts')
+        return self.data.get("ts")
 
     def to_mongo_doc(self):
         doc = self.data.copy()
-        doc['ns'] = self.ns
-        if 'o' in doc:
-            doc['o'] = json_util.dumps(doc['o'])
+        doc["ns"] = self.ns
+        if "o" in doc:
+            doc["o"] = json_util.dumps(doc["o"])
         return doc
 
     @classmethod
     def from_mongo_doc(cls, doc: dict):
         doc = dict(doc)
-        if 'o' in doc:
-            doc['o'] = json_util.loads(doc['o'])
+        if "o" in doc:
+            doc["o"] = json_util.loads(doc["o"])
         return cls(doc)
 
     @property
     def upstream_id(self) -> str:
         try:
-            return str(self.data['o']['_id'])
+            return str(self.data["o"]["_id"])
         except (KeyError, TypeError):
             pass
         try:
-            return str(self.data['o2']['_id'])
+            return str(self.data["o2"]["_id"])
         except (KeyError, TypeError):
             pass
 
     @property
     def id_(self) -> ObjectId:
-        if id_ := self.data.get('_id'):
+        if id_ := self.data.get("_id"):
             return ObjectId(id_)
 
 
 # Caution: do NOT run multiple threads / processes of this!!
 # TODO: consider thread safety
 class OplogTailer(object):
     _ns_exclude = {}
-    _db_exclude = {'config', 'local', 'admin'}
+    _db_exclude = {"config", "local", "admin"}
     record_cls = OplogRecord
 
     def __init__(
-            self, upstream_client: MongoClient, ts: Timestamp,
-            ns_pattern: str = None, ns_exclude: str = None):
+        self,
+        upstream_client: MongoClient,
+        ts: Timestamp,
+        ns_pattern: str = None,
+        ns_exclude: str = None,
+    ):
         """
         Args:
             upstream_client:
             ts: starting timestamp (seconds since epoch), e.g. 1642477123
             ns_pattern: regex
             ns_exclude: regex
         """
-        db = upstream_client.get_database('local')
-        self.oplog_coll = db.get_collection('oplog.rs')
+        db = upstream_client.get_database("local")
+        self.oplog_coll = db.get_collection("oplog.rs")
         self.ts = ts
         self.ns_pattern = ns_pattern
         self.ns_exclude = ns_exclude
         self._cursor = self._get_cursor()
 
     def _get_where_clause(self):
         tests = ['this.op != "n"']
         if self.ns_pattern is not None:
-            tests.append('this.ns.match(/{}/)'.format(self.ns_pattern))
+            tests.append("this.ns.match(/{}/)".format(self.ns_pattern))
             # tests.append(f'this.ns.match(/{self.ns_pattern}/)')
         if self.ns_exclude is not None:
-            tests.append('!this.ns.match(/{}/)'.format(self.ns_exclude))
+            tests.append("!this.ns.match(/{}/)".format(self.ns_exclude))
             # tests.append(f'!this.ns.match(/{self.ns_exclude}/)')
-        return '&&'.join(tests)
+        return "&&".join(tests)
 
     def _get_cursor(self):
-        filtr = {'ts': {'$gt': self.ts}}
+        filtr = {"ts": {"$gt": self.ts}}
         # https://pymongo.readthedocs.io/en/stable/examples/tailable.html
         # TODO: consider using $expr for mongo >= 3.6
-        _logger.info('OplogTailer._get_cursor, filtr=%s', filtr)
+        _logger.info("OplogTailer._get_cursor, filtr=%s", filtr)
         cursor = self.oplog_coll.find(
-            filtr, oplog_replay=True,
+            filtr,
+            oplog_replay=True,
             cursor_type=pymongo.CursorType.TAILABLE_AWAIT,
         )
         where_clause = self._get_where_clause()
         if where_clause:
             cursor = cursor.where(where_clause)
         return cursor
 
     def _reset_cursor(self):
         self._cursor.close()
         self._cursor = self._get_cursor()
 
     def _check_ns(self, doc: dict):
-        ns = doc.get('ns')
+        ns = doc.get("ns")
         if not ns:
             return False
         if ns in self._ns_exclude:
             return False
-        db_name = ns.split('.')[0]
+        db_name = ns.split(".")[0]
         if db_name in self._db_exclude:
             return False
         return True
 
     def _fetch_next(self):
         try:
             return self._cursor.next()
         except (StopIteration, ConnectionResetError):
             self._reset_cursor()
 
     def __iter__(self):
         return self
 
-    def __next__(self) -> 'record_cls':
+    def __next__(self) -> "record_cls":
         while True:
             doc = self._fetch_next()
             if doc is None:
                 time.sleep(1)
                 continue
             if not self._check_ns(doc):
                 continue
-            self.ts = doc.get('ts')
+            self.ts = doc.get("ts")
             return self.record_cls(doc)
 
 
 class ChangeStreamRegistry:
     def __init__(self, db: Database):
         self.db = db
         self.handlers = defaultdict(list)
 
     @staticmethod
     def apply(handler: Callable, coll_name: str, event: dict):
         try:
-            id_ = event['documentKey']['_id']
+            id_ = event["documentKey"]["_id"]
         except KeyError:
             id_ = None
         _logger.info(
-            'applying %s() to change event of collection %r, %s',
-            getattr(handler, '__name__', None) or str(handler),
-            coll_name, id_
+            "applying %s() to change event of collection %r, %s",
+            getattr(handler, "__name__", None) or str(handler),
+            coll_name,
+            id_,
         )
         # noinspection PyBroadException
         try:
             handler(event)
         except Exception:
             traceback.print_exc()
```

### Comparing `joker-mongodb-0.2.0/joker/mongodb/tools/querying.py` & `joker-mongodb-0.3.0/joker/mongodb/tools/querying.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 
 _logger = logging.getLogger(__name__)
 
 
 def _namemap_to_project(namemap: dict):
     project = {}
     for new_name, old_name in namemap.items():
-        if not old_name.startswith('$'):
-            old_name = '$' + old_name
-        project[new_name] = {'$ifNull': [old_name, None]}
+        if not old_name.startswith("$"):
+            old_name = "$" + old_name
+        project[new_name] = {"$ifNull": [old_name, None]}
     return project
 
 
 def _namemap_from_fieldlist(fieldlist: list):
-    return {k.split('.')[-1]: k for k in fieldlist}
+    return {k.split(".")[-1]: k for k in fieldlist}
 
 
-def find_with_renaming(
-        coll: Collection, filtr: dict, namemap: dict, sort: dict = None):
+def find_with_renaming(coll: Collection, filtr: dict, namemap: dict, sort: dict = None):
     pipelines = [
-        {'$match': filtr},
-        {'$sort': sort or {'_id': -1}},
-        {'$project': _namemap_to_project(namemap)},
+        {"$match": filtr},
+        {"$sort": sort or {"_id": -1}},
+        {"$project": _namemap_to_project(namemap)},
     ]
     return coll.aggregate(pipelines)
 
 
 def find_one_with_renaming(
-        coll: Collection, filtr: dict, namemap: dict, sort: dict = None):
+    coll: Collection, filtr: dict, namemap: dict, sort: dict = None
+):
     pipelines = [
-        {'$match': filtr},
-        {'$sort': sort or {'_id': -1}},
-        {'$limit': 1},
-        {'$project': _namemap_to_project(namemap)},
+        {"$match": filtr},
+        {"$sort": sort or {"_id": -1}},
+        {"$limit": 1},
+        {"$project": _namemap_to_project(namemap)},
     ]
-    _logger.debug('pipelines: %s', pipelines)
+    _logger.debug("pipelines: %s", pipelines)
     docs = list(coll.aggregate(pipelines))
     if docs:
         return docs[0]
```

### Comparing `joker-mongodb-0.2.0/joker/mongodb/tools/schema.py` & `joker-mongodb-0.3.0/joker/mongodb/tools/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 from bson import ObjectId
 from pymongo.collection import Collection
 
 
 class MongoFieldSchemator:
     _bsontype_of_pytypes = {
-        str: 'string',
-        dict: 'object',
-        type(None): 'null',
-        datetime.datetime: 'date',
-        int: 'long',
-        bool: 'bool',
-        ObjectId: 'objectId',
+        str: "string",
+        dict: "object",
+        type(None): "null",
+        datetime.datetime: "date",
+        int: "long",
+        bool: "bool",
+        ObjectId: "objectId",
     }
 
     _max_enum_length = 7
     _max_type_length = 3
 
     def __init__(self):
         self._bsontypes = set()
@@ -75,19 +75,19 @@
         Returns:
             e.g.
             {
                "bsonType": "string",
                "enum": ["low", "mid", "high"],
             }
         """
-        p = {'bsonType': self.bsontype, 'enum': self.enum}
+        p = {"bsonType": self.bsontype, "enum": self.enum}
         return {k: v for k, v in p.items() if v is not None}
 
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class MongoDocumentSchemator:
     def __init__(self, fieldnames: set[str]):
         if not isinstance(fieldnames, set):
             fieldnames = set(fieldnames)
         self._fieldnames = fieldnames
@@ -128,14 +128,14 @@
     def get_required(self) -> list[str]:
         return list(sorted(self._required))
 
     def to_jsonschema(self) -> dict:
         return {
             # $jsonSchema keyword '$schema' is not currently supported
             # "$schema": "http://json-schema.org/draft-04/schema#",
-            'type': 'object',
-            'properties': self.get_properties(),
-            'required': self.get_required(),
+            "type": "object",
+            "properties": self.get_properties(),
+            "required": self.get_required(),
         }
 
 
-__all__ = ['MongoFieldSchemator', 'MongoDocumentSchemator']
+__all__ = ["MongoFieldSchemator", "MongoDocumentSchemator"]
```

### Comparing `joker-mongodb-0.2.0/joker/mongodb/tools/transactional.py` & `joker-mongodb-0.3.0/joker/mongodb/tools/transactional.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 # coding: utf-8
+from __future__ import annotations
 
 import datetime
 
 import pymongo.errors
 from pymongo import ReturnDocument
 from pymongo.collection import Collection
 
@@ -12,30 +13,31 @@
     def __init__(self, coll: Collection):
         self.coll = coll
 
     def lock(self, name: str, ttl: int = 60):
         now = datetime.datetime.now()
         expire_at = now + datetime.timedelta(seconds=ttl)
         self.coll.delete_many(
-            {'expire_at': {'$lt': now}, 'type': 'lock'},
+            {"expire_at": {"$lt": now}, "type": "lock"},
         )
         record = {
-            '_id': name,
-            'type': 'lock',
-            'expire_at': expire_at,
+            "_id": name,
+            "type": "lock",
+            "expire_at": expire_at,
         }
         try:
             self.coll.insert_one(record)
         except pymongo.errors.DuplicateKeyError:
             return False
         return True
 
     def unlock(self, name: str):
-        self.coll.delete_one({'_id': name, 'type': 'lock'})
+        self.coll.delete_one({"_id": name, "type": "lock"})
 
-    def get_next_serial_code(self, prefix='ID', length=6):
+    def get_next_serial_code(self, prefix="ID", length=6):
         doc = self.coll.find_one_and_update(
-            {'_id': prefix, 'type': 'serial'},
-            {'$inc': {'i': 1}},
-            upsert=True, return_document=ReturnDocument.AFTER,
+            {"_id": prefix, "type": "serial"},
+            {"$inc": {"i": 1}},
+            upsert=True,
+            return_document=ReturnDocument.AFTER,
         )
-        return prefix + str(doc['i']).zfill(length)
+        return prefix + str(doc["i"]).zfill(length)
```

### Comparing `joker-mongodb-0.2.0/joker/mongodb/utils.py` & `joker-mongodb-0.3.0/joker/mongodb/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 #!/usr/bin/env python3
 # coding: utf-8
+from __future__ import annotations
 
 import logging
 import os.path
 from typing import Union
 
 import bson.json_util
 import volkanic.utils
 from joker.cast.numeric import human_filesize
 from joker.textmanip.tabular import tabular_format
 from pymongo import MongoClient
 from pymongo.database import Database
 from pymongo.monitoring import (
-    CommandListener, CommandStartedEvent,
-    CommandFailedEvent, CommandSucceededEvent,
+    CommandListener,
+    CommandStartedEvent,
+    CommandFailedEvent,
+    CommandSucceededEvent,
 )
 
 
 def is_in_replset(mongo: MongoClient) -> bool:
-    db = mongo.get_database('admin')
-    return 'replication' in db.command('getCmdLineOpts')['parsed']
+    db = mongo.get_database("admin")
+    return "replication" in db.command("getCmdLineOpts")["parsed"]
 
 
 def inspect_mongo_storage_sizes(target: Union[MongoClient, Database]):
     if isinstance(target, MongoClient):
-        return {r['name']: r['sizeOnDisk'] for r in target.list_databases()}
+        return {r["name"]: r["sizeOnDisk"] for r in target.list_databases()}
     size_of_collections = {}
     for coll_name in target.list_collection_names():
-        info = target.command('collStats', coll_name)
-        size_of_collections[info['ns']] = info['storageSize']
+        info = target.command("collStats", coll_name)
+        size_of_collections[info["ns"]] = info["storageSize"]
     return size_of_collections
 
 
 def print_mongo_storage_sizes(target: Union[MongoClient, Database]):
     s_rows = list(inspect_mongo_storage_sizes(target).items())
     s_rows.sort(key=lambda r: r[1], reverse=True)
     rows = []
@@ -40,82 +43,82 @@
         num, unit = human_filesize(v)
         rows.append([round(num), unit, k])
     for row in tabular_format(rows):
         print(*row)
 
 
 def indented_json_dumps(obj, **kwargs):
-    kwargs.setdefault('dumps', bson.json_util.dumps)
+    kwargs.setdefault("dumps", bson.json_util.dumps)
     return volkanic.utils.indented_json_dumps(obj, **kwargs)
 
 
 def indented_json_print(obj, **kwargs):
-    kwargs.setdefault('dumps', indented_json_dumps)
+    kwargs.setdefault("dumps", indented_json_dumps)
     return volkanic.utils.indented_json_print(obj, **kwargs)
 
 
 def infer_coll_triple_from_filename(path: str):
     """
     >>> p = "somedir/local.retail.customers.6789.json"
     >>> infer_coll_triple_from_filename(p)
     ['local', 'retail', 'customers']
     """
     filename = os.path.split(path)[1]
-    coll_fullname = filename.rsplit('.', 2)[0]
-    return coll_fullname.split('.', 2)
+    coll_fullname = filename.rsplit(".", 2)[0]
+    return coll_fullname.split(".", 2)
 
 
 def infer_params(mongo: MongoClient):
-    params = dict(zip(['host', 'port'], mongo.address))
+    params = dict(zip(["host", "port"], mongo.address))
     params.update(mongo._MongoClient__options._options)  # noqa
     return params
 
 
 class MongoCommandLogger(CommandListener):
     _registered = False
-    _logger = logging.getLogger('_mongodb')
+    _logger = logging.getLogger("_mongodb")
     _level = logging.DEBUG
 
     @staticmethod
     def _fmt_opid(event):
         if event.request_id == event.operation_id:
             return event.request_id
-        return '{}.{}'.format(event.request_id, event.operation_id)
+        return "{}.{}".format(event.request_id, event.operation_id)
 
     @staticmethod
     def _fmt_url(event):
-        addr = ':'.join(str(s) for s in event.connection_id)
-        return '{}/{}'.format(addr, event.database_name)
+        addr = ":".join(str(s) for s in event.connection_id)
+        return "{}/{}".format(addr, event.database_name)
 
     def started(self, event: CommandStartedEvent):
         if not self._logger.isEnabledFor(self._level):
             return
         parts = [
             self._fmt_opid(event),
-            'started',
+            "started",
             self._fmt_url(event),
             event.command,
         ]
         msg = " ".join(str(s) for s in parts)
         self._logger.debug(msg)
 
     def succeeded(self, event: CommandSucceededEvent):
         if not self._logger.isEnabledFor(self._level):
             return
         parts = [
             self._fmt_opid(event),
-            'succeeded',
+            "succeeded",
             int(event.duration_micros / 1000),
         ]
         msg = " ".join(str(s) for s in parts)
         self._logger.debug(msg)
 
     def failed(self, event: CommandFailedEvent):
         if not self._logger.isEnabledFor(self._level):
             return
         parts = [
             self._fmt_opid(event),
-            'failed',
+            "failed",
             event.duration_micros,
         ]
         msg = " ".join(str(s) for s in parts)
         self._logger.debug(msg)
```

### Comparing `joker-mongodb-0.2.0/joker_mongodb.egg-info/PKG-INFO` & `joker-mongodb-0.3.0/joker_mongodb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: joker-mongodb
-Version: 0.2.0
+Version: 0.3.0
 Summary: access mongodb with handy utilities and fun
 Home-page: https://github.com/frozflame/joker-mongodb
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: joker-cast>=0.5.0
 Requires-Dist: joker-textmanip>=0.3.1
 Requires-Dist: joker>=0.3.3
 Requires-Dist: pymongo>=3.11.0
 Requires-Dist: volkanic>=0.5.1
```

### Comparing `joker-mongodb-0.2.0/joker_mongodb.egg-info/SOURCES.txt` & `joker-mongodb-0.3.0/joker_mongodb.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 joker/mongodb/tools/experimental.py
 joker/mongodb/tools/filters.py
 joker/mongodb/tools/integrity.py
 joker/mongodb/tools/kvstore.py
 joker/mongodb/tools/misc.py
 joker/mongodb/tools/mongoshell.py
 joker/mongodb/tools/oplog.py
+joker/mongodb/tools/paginations.py
 joker/mongodb/tools/querying.py
 joker/mongodb/tools/schema.py
 joker/mongodb/tools/transactional.py
 joker_mongodb.egg-info/PKG-INFO
 joker_mongodb.egg-info/SOURCES.txt
 joker_mongodb.egg-info/dependency_links.txt
 joker_mongodb.egg-info/namespace_packages.txt
```

### Comparing `joker-mongodb-0.2.0/setup.py` & `joker-mongodb-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,60 +5,58 @@
 
 import setuptools
 from setuptools import find_namespace_packages
 
 # CAUTION:
 # Do NOT import your package from your setup.py
 
-_nsp = 'joker'
-_pkg = 'mongodb'
+_nsp = "joker"
+_pkg = "mongodb"
 _names = [_nsp, _pkg]
 _names = [s for s in _names if s]
 
 
 def read(filename):
     with open(filename) as f:
         return f.read()
 
 
 def _find_version():
-    names = _names + ['__init__.py']
+    names = _names + ["__init__.py"]
     path = os.path.join(*names)
     root = os.path.dirname(__file__)
     path = os.path.join(root, path)
-    regex = re.compile(
-        r'''^__version__\s*=\s*('|"|'{3}|"{3})([.\w]+)\1\s*(#|$)''')
+    regex = re.compile(r"""^__version__\s*=\s*('|"|'{3}|"{3})([.\w]+)\1\s*(#|$)""")
     with open(path) as fin:
         for line in fin:
             line = line.strip()
-            if not line or line.startswith('#'):
+            if not line or line.startswith("#"):
                 continue
             mat = regex.match(line)
             if mat:
                 return mat.groups()[1]
-    raise ValueError('__version__ definition not found')
+    raise ValueError("__version__ definition not found")
 
 
 config = {
     "name": "joker-mongodb",
     "version": _find_version(),
     "description": "access mongodb with handy utilities and fun",
     "keywords": "",
     "url": "https://github.com/frozflame/joker-mongodb",
     "author": "frozflame",
     "author_email": "frozflame@outlook.com",
     "license": "GNU General Public License (GPL)",
     "packages": find_namespace_packages(include=["joker.*"]),
     "zip_safe": False,
     "install_requires": read("requirements.txt"),
-    "python_requires": ">=3.6.0",
+    "python_requires": ">=3.7.0",
     "classifiers": [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
@@ -66,10 +64,10 @@
     # ensure copy static file to runtime directory
     "include_package_data": True,
     "long_description": read("README.md"),
     "long_description_content_type": "text/markdown",
 }
 
 if _nsp:
-    config['namespace_packages'] = [_nsp]
+    config["namespace_packages"] = [_nsp]
 
 setuptools.setup(**config)
```

