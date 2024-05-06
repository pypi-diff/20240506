# Comparing `tmp/pd_extras-5.0.6.tar.gz` & `tmp/pd_extras-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pd_extras-5.0.6.tar", max compression
+gzip compressed data, was "pd_extras-6.0.0.tar", max compression
```

## Comparing `pd_extras-5.0.6.tar` & `pd_extras-6.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1069 2024-05-05 19:47:06.932467 pd_extras-5.0.6/LICENSE
--rw-r--r--   0        0        0     2930 2024-05-05 19:47:06.932467 pd_extras-5.0.6/README.md
--rw-r--r--   0        0        0        0 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/check/__init__.py
--rw-r--r--   0        0        0     3245 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/check/sanitize.py
--rw-r--r--   0        0        0        0 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/extra/__init__.py
--rw-r--r--   0        0        0     3794 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/extra/flattener.py
--rw-r--r--   0        0        0     2635 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/extra/operations.py
--rw-r--r--   0        0        0        0 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/optimize/__init__.py
--rw-r--r--   0        0        0     1775 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/optimize/df_ops.py
--rw-r--r--   0        0        0        0 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/write/__init__.py
--rw-r--r--   0        0        0     1388 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/write/common.py
--rw-r--r--   0        0        0     5682 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/write/nosql_writer.py
--rw-r--r--   0        0        0     8962 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/write/sql_writer.py
--rw-r--r--   0        0        0      724 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pyproject.toml
--rw-r--r--   0        0        0     3944 1970-01-01 00:00:00.000000 pd_extras-5.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-06 00:48:14.841913 pd_extras-6.0.0/LICENSE
+-rw-r--r--   0        0        0     2930 2024-05-06 00:48:14.841913 pd_extras-6.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 00:48:14.841913 pd_extras-6.0.0/pd_extras/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 00:48:14.841913 pd_extras-6.0.0/pd_extras/check/__init__.py
+-rw-r--r--   0        0        0     3245 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/check/sanitize.py
+-rw-r--r--   0        0        0        0 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/extra/__init__.py
+-rw-r--r--   0        0        0     3794 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/extra/flattener.py
+-rw-r--r--   0        0        0     2635 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/extra/operations.py
+-rw-r--r--   0        0        0        0 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/optimize/__init__.py
+-rw-r--r--   0        0        0     1775 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/optimize/df_ops.py
+-rw-r--r--   0        0        0        0 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/write/__init__.py
+-rw-r--r--   0        0        0     1388 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/write/common.py
+-rw-r--r--   0        0        0      169 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/write/driver.py
+-rw-r--r--   0        0        0     5682 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/write/nosql_writer.py
+-rw-r--r--   0        0        0     8955 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pd_extras/write/sql_writer.py
+-rw-r--r--   0        0        0      729 2024-05-06 00:48:14.845913 pd_extras-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3953 1970-01-01 00:00:00.000000 pd_extras-6.0.0/PKG-INFO
```

### Comparing `pd_extras-5.0.6/LICENSE` & `pd_extras-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.6/README.md` & `pd_extras-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.6/pd_extras/check/sanitize.py` & `pd_extras-6.0.0/pd_extras/check/sanitize.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.6/pd_extras/extra/flattener.py` & `pd_extras-6.0.0/pd_extras/extra/flattener.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.6/pd_extras/extra/operations.py` & `pd_extras-6.0.0/pd_extras/extra/operations.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.6/pd_extras/optimize/df_ops.py` & `pd_extras-6.0.0/pd_extras/optimize/df_ops.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.6/pd_extras/write/common.py` & `pd_extras-6.0.0/pd_extras/write/common.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.6/pd_extras/write/nosql_writer.py` & `pd_extras-6.0.0/pd_extras/write/nosql_writer.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.6/pd_extras/write/sql_writer.py` & `pd_extras-6.0.0/pd_extras/write/sql_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         self._check_name(name=self.__dbname)
         self._check_name(name=table_name)
 
         query: str = _saved_values["query"]["column_info"] % (
             self.__dbname,
             table_name,
         )
-        session = sa_session.execute(query)
+        session = sa_session.execute(text(query))
         cursor = session.cursor  # type: ignore
         cols = [detail[0] for detail in cursor.description]
         res = cursor.fetchall()
         res = [list(row) for row in res]
 
         info = pd.DataFrame(res, columns=cols)
         columns: list = [str(column.lower()) for column in info.columns.tolist()]
@@ -157,15 +157,15 @@
     def _get_table_from_dataframe(
         self,
         data: pd.DataFrame,
         table_name: str,
         id_col: str,
         max_length: int = 100,
     ):
-        metadata = MetaData(self.__engine)
+        metadata = MetaData()
         columns = []
 
         if id_col:
             columns.append(Column(id_col, Integer, primary_key=True, nullable=False))
 
         for column in data.columns:
             nullable_status = False
```

### Comparing `pd_extras-5.0.6/pyproject.toml` & `pd_extras-6.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pd-extras"
-version = "5.0.6"
+version = "6.0.0"
 description = "Some utility functions on top of pandas."
 authors = ["Masum Billal <billalmasum93@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/proafxin/pd-extras"
 documentation = "https://pd-extras.readthedocs.io/en/latest/"
 
@@ -13,15 +13,15 @@
 python = "^3.9"
 pandas = ">=1.5.3"
 pymongo = "^4.7.1"
 sqlalchemy-utils = "^0.41.2"
 mysqlclient = "^2.2.4"
 psycopg2 = "^2.9.9"
 pymssql = "^2.3.0"
-sqlalchemy = "^1"
+sqlalchemy = "^2.0.30"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.3.7"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
```

### Comparing `pd_extras-5.0.6/PKG-INFO` & `pd_extras-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pd-extras
-Version: 5.0.6
+Version: 6.0.0
 Summary: Some utility functions on top of pandas.
 Home-page: https://github.com/proafxin/pd-extras
 License: MIT
 Author: Masum Billal
 Author-email: billalmasum93@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: mysqlclient (>=2.2.4,<3.0.0)
 Requires-Dist: pandas (>=1.5.3)
 Requires-Dist: psycopg2 (>=2.9.9,<3.0.0)
 Requires-Dist: pymongo (>=4.7.1,<5.0.0)
 Requires-Dist: pymssql (>=2.3.0,<3.0.0)
-Requires-Dist: sqlalchemy (>=1,<2)
+Requires-Dist: sqlalchemy (>=2.0.30,<3.0.0)
 Requires-Dist: sqlalchemy-utils (>=0.41.2,<0.42.0)
 Project-URL: Documentation, https://pd-extras.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/proafxin/pd-extras
 Description-Content-Type: text/markdown
 
 # Pandas Extras
```

