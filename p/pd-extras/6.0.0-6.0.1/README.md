# Comparing `tmp/pd_extras-6.0.0.tar.gz` & `tmp/pd_extras-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pd_extras-6.0.0.tar", max compression
+gzip compressed data, was "pd_extras-6.0.1.tar", max compression
```

## Comparing `pd_extras-6.0.0.tar` & `pd_extras-6.0.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1069 2024-05-06 00:48:14.841913 pd_extras-6.0.0/LICENSE
--rw-r--r--   0        0        0     2930 2024-05-06 00:48:14.841913 pd_extras-6.0.0/README.md
--rw-r--r--   0        0        0        0 2024-05-06 00:48:14.841913 pd_extras-6.0.0/pd_extras/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 00:48:14.841913 pd_extras-6.0.0/pd_extras/check/__init__.py
--rw-r--r--   0        0        0     3245 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/check/sanitize.py
--rw-r--r--   0        0        0        0 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/extra/__init__.py
--rw-r--r--   0        0        0     3794 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/extra/flattener.py
--rw-r--r--   0        0        0     2635 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/extra/operations.py
--rw-r--r--   0        0        0        0 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/optimize/__init__.py
--rw-r--r--   0        0        0     1775 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/optimize/df_ops.py
--rw-r--r--   0        0        0        0 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/write/__init__.py
--rw-r--r--   0        0        0     1388 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/write/common.py
--rw-r--r--   0        0        0      169 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/write/driver.py
--rw-r--r--   0        0        0     5682 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/write/nosql_writer.py
--rw-r--r--   0        0        0     8955 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/write/sql_writer.py
--rw-r--r--   0        0        0      729 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pyproject.toml
--rw-r--r--   0        0        0     3953 1970-01-01 00:00:00.000000 pd_extras-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-06 02:51:53.691577 pd_extras-6.0.1/LICENSE
+-rw-r--r--   0        0        0     3093 2024-05-06 02:51:53.691577 pd_extras-6.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/check/__init__.py
+-rw-r--r--   0        0        0     3245 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/check/sanitize.py
+-rw-r--r--   0        0        0        0 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/extra/__init__.py
+-rw-r--r--   0        0        0     3794 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/extra/flattener.py
+-rw-r--r--   0        0        0     2635 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/extra/operations.py
+-rw-r--r--   0        0        0        0 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/optimize/__init__.py
+-rw-r--r--   0        0        0     1775 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/optimize/df_ops.py
+-rw-r--r--   0        0        0        0 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/write/__init__.py
+-rw-r--r--   0        0        0     1388 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/write/common.py
+-rw-r--r--   0        0        0     5670 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/write/nosql_writer.py
+-rw-r--r--   0        0        0     8955 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/write/sql_writer.py
+-rw-r--r--   0        0        0      729 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4116 1970-01-01 00:00:00.000000 pd_extras-6.0.1/PKG-INFO
```

### Comparing `pd_extras-6.0.0/LICENSE` & `pd_extras-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.0/README.md` & `pd_extras-6.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Pandas Extras
 
-[![Code check, Test and Coverage, Build and deploy](https://github.com/proafxin/pd-extras/actions/workflows/build_deploy.yml/badge.svg)](https://github.com/proafxin/pd-extras/actions/workflows/build_deploy.yml)
+[![Test code and upload coverage](https://github.com/proafxin/pd-extras/actions/workflows/build_test.yaml/badge.svg)](https://github.com/proafxin/pd-extras/actions/workflows/build_test.yaml)
+[![Test code and upload coverage](https://github.com/proafxin/pd-extras/actions/workflows/deploy.yaml/badge.svg)](https://github.com/proafxin/pd-extras/actions/workflows/deploy.yaml)
 [![codecov](https://codecov.io/gh/proafxin/pd-extras/graph/badge.svg?token=AQA0IJY4N1)](https://codecov.io/gh/proafxin/pd-extras)
 [![Documentation Status](https://readthedocs.org/projects/pd-extras/badge/?version=latest)](https://pd-extras.readthedocs.io/en/latest/?badge=latest)
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pd-extras?logo=python&logoColor=yellow&style=for-the-badge)
 ![PyPI - Version](https://img.shields.io/pypi/v/pd-extras?logo=python&logoColor=yellow&style=for-the-badge)
 ![Docker Image Version (tag)](https://img.shields.io/docker/v/_/postgres/latest?arch=amd64&style=for-the-badge&logo=postgresql&logoColor=white&label=Postgresql)
 ![Docker Image Version (tag)](https://img.shields.io/docker/v/_/mysql/latest?arch=amd64&style=for-the-badge&logo=mysql&logoColor=white&label=mysql)
```

### Comparing `pd_extras-6.0.0/pd_extras/check/sanitize.py` & `pd_extras-6.0.1/pd_extras/check/sanitize.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.0/pd_extras/extra/flattener.py` & `pd_extras-6.0.1/pd_extras/extra/flattener.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.0/pd_extras/extra/operations.py` & `pd_extras-6.0.1/pd_extras/extra/operations.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.0/pd_extras/optimize/df_ops.py` & `pd_extras-6.0.1/pd_extras/optimize/df_ops.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.0/pd_extras/write/common.py` & `pd_extras-6.0.1/pd_extras/write/common.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.0/pd_extras/write/nosql_writer.py` & `pd_extras-6.0.1/pd_extras/write/nosql_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Write a pandas dataframe to a NoSQL database collection"""
 
-
 import pandas as pd
 import pymongo
+from pymongo.collection import Collection
+
 from pd_extras.write.common import nosql_dbtypes
 
 __all__ = ["NoSQLDatabaseWriter"]
 
 
 class MongoDatabaseWriter:
     """Writer class for Mongo databases"""
@@ -47,15 +48,15 @@
 
     def _get_list_of_databases(self):
         return self.__client.list_database_names()
 
     def _get_list_of_collections(self):
         return self.__db.list_collection_names()
 
-    def _get_or_create_collection(self, collection_name: str):
+    def _get_or_create_collection(self, collection_name: str) -> Collection:
         collection = self.__db[collection_name]
 
         return collection
 
     def _write_data_to_collection(self, data: pd.DataFrame, collection_name: str):
         collection = self._get_or_create_collection(collection_name=collection_name)
         documents = data.to_dict("records")
@@ -65,21 +66,21 @@
         return res
 
     def _get_document_count(self, collection_name: str):
         collection = self._get_or_create_collection(collection_name=collection_name)
 
         return collection.count_documents({})
 
-    def _delete_collection(self, collection_name: str):
+    def _delete_collection(self, collection_name: str) -> None:
         self.__db.drop_collection(collection_name)
 
-    def _delete_database(self):
+    def _delete_database(self) -> None:
         self.__client.drop_database(name_or_database=self.__dbname)
 
-    def _close_connection(self):
+    def _close_connection(self) -> None:
         self.__client.close()
 
 
 class NoSQLDatabaseWriter:
     """Writer class for NoSQL Database"""
 
     def __init__(
@@ -89,15 +90,15 @@
         dbname: str,
         user: str,
         password: str,
         port: int,
         dns_seed_list: bool = False,
     ) -> None:
         if dbtype not in nosql_dbtypes:
-            raise ValueError(f"{dbtype} not in {nosql_dbtypes}")
+            raise KeyError(f"{dbtype} not in {nosql_dbtypes}")
 
         self.__dbtype = dbtype
 
         self.__writer = self._get_writer(
             host=host,
             dbname=dbname,
             user=user,
@@ -111,25 +112,22 @@
         host: str,
         dbname: str,
         user: str,
         password: str,
         port: int,
         dns_seed_list: bool = False,
     ):
-        if self.__dbtype == "mongo":
-            return MongoDatabaseWriter(
-                host=host,
-                dbname=dbname,
-                user=user,
-                password=password,
-                port=port,
-                dns_seed_list=dns_seed_list,
-            )
-
-        return None
+        return MongoDatabaseWriter(
+            host=host,
+            dbname=dbname,
+            user=user,
+            password=password,
+            port=port,
+            dns_seed_list=dns_seed_list,
+        )
 
     def get_list_of_databases(self):
         """List names of databses in this connection.
 
         :return: Database names.
         :rtype: `list[str]`
         """
```

### Comparing `pd_extras-6.0.0/pd_extras/write/sql_writer.py` & `pd_extras-6.0.1/pd_extras/write/sql_writer.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.0/pyproject.toml` & `pd_extras-6.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pd-extras"
-version = "6.0.0"
+version = "6.0.1"
 description = "Some utility functions on top of pandas."
 authors = ["Masum Billal <billalmasum93@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/proafxin/pd-extras"
 documentation = "https://pd-extras.readthedocs.io/en/latest/"
```

### Comparing `pd_extras-6.0.0/PKG-INFO` & `pd_extras-6.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pd-extras
-Version: 6.0.0
+Version: 6.0.1
 Summary: Some utility functions on top of pandas.
 Home-page: https://github.com/proafxin/pd-extras
 License: MIT
 Author: Masum Billal
 Author-email: billalmasum93@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,16 @@
 Requires-Dist: sqlalchemy-utils (>=0.41.2,<0.42.0)
 Project-URL: Documentation, https://pd-extras.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/proafxin/pd-extras
 Description-Content-Type: text/markdown
 
 # Pandas Extras
 
-[![Code check, Test and Coverage, Build and deploy](https://github.com/proafxin/pd-extras/actions/workflows/build_deploy.yml/badge.svg)](https://github.com/proafxin/pd-extras/actions/workflows/build_deploy.yml)
+[![Test code and upload coverage](https://github.com/proafxin/pd-extras/actions/workflows/build_test.yaml/badge.svg)](https://github.com/proafxin/pd-extras/actions/workflows/build_test.yaml)
+[![Test code and upload coverage](https://github.com/proafxin/pd-extras/actions/workflows/deploy.yaml/badge.svg)](https://github.com/proafxin/pd-extras/actions/workflows/deploy.yaml)
 [![codecov](https://codecov.io/gh/proafxin/pd-extras/graph/badge.svg?token=AQA0IJY4N1)](https://codecov.io/gh/proafxin/pd-extras)
 [![Documentation Status](https://readthedocs.org/projects/pd-extras/badge/?version=latest)](https://pd-extras.readthedocs.io/en/latest/?badge=latest)
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pd-extras?logo=python&logoColor=yellow&style=for-the-badge)
 ![PyPI - Version](https://img.shields.io/pypi/v/pd-extras?logo=python&logoColor=yellow&style=for-the-badge)
 ![Docker Image Version (tag)](https://img.shields.io/docker/v/_/postgres/latest?arch=amd64&style=for-the-badge&logo=postgresql&logoColor=white&label=Postgresql)
 ![Docker Image Version (tag)](https://img.shields.io/docker/v/_/mysql/latest?arch=amd64&style=for-the-badge&logo=mysql&logoColor=white&label=mysql)
```

