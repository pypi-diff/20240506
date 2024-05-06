# Comparing `tmp/sqla_utils-0.6.0.tar.gz` & `tmp/sqla_utils-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqla_utils-0.6.0.tar", max compression
+gzip compressed data, was "sqla_utils-0.6.1.tar", max compression
```

## Comparing `sqla_utils-0.6.0.tar` & `sqla_utils-0.6.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1073 2021-01-29 16:05:17.021703 sqla_utils-0.6.0/LICENSE
--rw-r--r--   0        0        0     2992 2023-10-02 12:50:15.610477 sqla_utils-0.6.0/NEWS.md
--rw-r--r--   0        0        0     2316 2023-01-11 13:02:21.065705 sqla_utils-0.6.0/README.md
--rw-r--r--   0        0        0     1391 2023-10-02 12:50:31.854926 sqla_utils-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      364 2022-02-17 14:22:09.234230 sqla_utils-0.6.0/sqla_utils/__init__.py
--rw-r--r--   0        0        0     6915 2023-10-02 12:41:48.047548 sqla_utils-0.6.0/sqla_utils/base.py
--rw-r--r--   0        0        0     3143 2023-01-18 18:06:26.262373 sqla_utils-0.6.0/sqla_utils/builder.py
--rw-r--r--   0        0        0     2035 2022-02-16 12:46:42.075623 sqla_utils-0.6.0/sqla_utils/exc.py
--rw-r--r--   0        0        0        0 2021-02-01 14:38:40.080730 sqla_utils-0.6.0/sqla_utils/py.typed
--rw-r--r--   0        0        0     1998 2021-09-21 13:29:00.798312 sqla_utils-0.6.0/sqla_utils/session.py
--rw-r--r--   0        0        0     2475 2021-06-21 13:13:15.233169 sqla_utils-0.6.0/sqla_utils/split_sql.py
--rw-r--r--   0        0        0    11335 2023-01-30 12:43:17.150266 sqla_utils-0.6.0/sqla_utils/test.py
--rw-r--r--   0        0        0     3920 2023-09-04 09:00:45.490111 sqla_utils-0.6.0/sqla_utils/transaction.py
--rw-r--r--   0        0        0      104 2023-01-18 18:38:41.154970 sqla_utils-0.6.0/sqla_utils/types.py
--rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 sqla_utils-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2969 2024-05-06 11:17:23.528412 sqla_utils-0.6.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1073 2021-01-29 16:05:17.021703 sqla_utils-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2316 2023-01-11 13:02:21.065705 sqla_utils-0.6.1/README.md
+-rw-r--r--   0        0        0     1397 2024-05-06 11:17:28.866631 sqla_utils-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      364 2022-02-17 14:22:09.234230 sqla_utils-0.6.1/sqla_utils/__init__.py
+-rw-r--r--   0        0        0     6915 2023-10-02 12:41:48.047548 sqla_utils-0.6.1/sqla_utils/base.py
+-rw-r--r--   0        0        0     3143 2023-01-18 18:06:26.262373 sqla_utils-0.6.1/sqla_utils/builder.py
+-rw-r--r--   0        0        0     2035 2022-02-16 12:46:42.075623 sqla_utils-0.6.1/sqla_utils/exc.py
+-rw-r--r--   0        0        0        0 2021-02-01 14:38:40.080730 sqla_utils-0.6.1/sqla_utils/py.typed
+-rw-r--r--   0        0        0     1998 2021-09-21 13:29:00.798312 sqla_utils-0.6.1/sqla_utils/session.py
+-rw-r--r--   0        0        0     2475 2021-06-21 13:13:15.233169 sqla_utils-0.6.1/sqla_utils/split_sql.py
+-rw-r--r--   0        0        0    11421 2024-05-06 10:58:26.510851 sqla_utils-0.6.1/sqla_utils/test.py
+-rw-r--r--   0        0        0     3896 2024-05-06 10:58:26.513851 sqla_utils-0.6.1/sqla_utils/transaction.py
+-rw-r--r--   0        0        0      104 2023-01-18 18:38:41.154970 sqla_utils-0.6.1/sqla_utils/types.py
+-rw-r--r--   0        0        0     3252 1970-01-01 00:00:00.000000 sqla_utils-0.6.1/PKG-INFO
```

### Comparing `sqla_utils-0.6.0/LICENSE` & `sqla_utils-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqla_utils-0.6.0/README.md` & `sqla_utils-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `sqla_utils-0.6.0/pyproject.toml` & `sqla_utils-0.6.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "sqla-utils"
-version = "0.6.0"
+version = "0.6.1"
 description = "Opinionated utilities for working with SQLAlchemy"
 readme = "README.md"
 keywords = ["sqlalchemy", "orm"]
 authors = ["Sebastian Rittau <srittau@rittau.biz>"]
 license = "MIT"
 homepage = "https://github.com/srittau/sqla-utils"
 repository = "https://github.com/srittau/sqla-utils"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Topic :: Software Development",
     "Typing :: Typed",
 ]
-include = ["NEWS.md", "*/py.typed"]
+include = ["CHANGELOG.md", "*/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">= 3.8, < 4"
 SQLAlchemy = ">= 1.4, < 3"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.1.0"
-flake8 = { version = "^6.0.0", python = ">= 3.8.1" }
+black = "^24.4.2"
+flake8 = { version = "^7.0.0", python = ">= 3.8.1" }
 isort = "^5.9.2"
-mypy = "~1.5.1"
+mypy = "~1.10.0"
 pytest = "*"
 
 [tool.black]
 target-version = ["py38"]
 line-length = 79
 
 [tool.isort]
```

### Comparing `sqla_utils-0.6.0/sqla_utils/base.py` & `sqla_utils-0.6.1/sqla_utils/base.py`

 * *Files identical despite different names*

### Comparing `sqla_utils-0.6.0/sqla_utils/builder.py` & `sqla_utils-0.6.1/sqla_utils/builder.py`

 * *Files identical despite different names*

### Comparing `sqla_utils-0.6.0/sqla_utils/exc.py` & `sqla_utils-0.6.1/sqla_utils/exc.py`

 * *Files identical despite different names*

### Comparing `sqla_utils-0.6.0/sqla_utils/session.py` & `sqla_utils-0.6.1/sqla_utils/session.py`

 * *Files identical despite different names*

### Comparing `sqla_utils-0.6.0/sqla_utils/split_sql.py` & `sqla_utils-0.6.1/sqla_utils/split_sql.py`

 * *Files identical despite different names*

### Comparing `sqla_utils-0.6.0/sqla_utils/test.py` & `sqla_utils-0.6.1/sqla_utils/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,15 +292,17 @@
     ) -> None:
         """Assert that the expected rows are in table and no other rows."""
         __tracebackhide__ = True
 
         fetched_rows = self.select_all_rows(table_name)
         if not fetched_rows and not expected_rows:
             return
-        assert len(fetched_rows) == len(expected_rows)
+        assert len(fetched_rows) == len(
+            expected_rows
+        ), f"expected {len(expected_rows)} rows, got {len(fetched_rows)}"
 
         def find_one(
             rs: Sequence[Row[_TP]], expected: Mapping[str, Any]
         ) -> list[Row[_TP]]:
             __tracebackhide__ = True
             for i, tr in enumerate(rs):
                 try:
```

### Comparing `sqla_utils-0.6.0/sqla_utils/transaction.py` & `sqla_utils-0.6.1/sqla_utils/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,34 +54,31 @@
             raise
         if exc_type:
             self.session.rollback()
         else:
             self.session.commit()
 
     @overload
-    def query(self, entities: Table, **kwargs: Any) -> Query[Any]:
-        ...
+    def query(self, entities: Table, **kwargs: Any) -> Query[Any]: ...
 
     @overload  # noqa: F811
     def query(
         self, *entities: type[_T], **kwargs: Any
     ) -> Query[_T]:  # noqa: F811
         ...
 
     @overload  # noqa: F811
     def query(  # type: ignore  # noqa: F811
         self, entities: ColumnElement[_T], **kwargs: Any
-    ) -> Query[tuple[_T]]:
-        ...
+    ) -> Query[tuple[_T]]: ...
 
     @overload  # noqa: F811
     def query(  # noqa: F811
         self, *entities: ColumnElement[_T], **kwargs: Any
-    ) -> Query[tuple[_T, ...]]:
-        ...
+    ) -> Query[tuple[_T, ...]]: ...
 
     def query(self, *entities: Any, **kwargs: Any) -> Any:  # noqa: F811
         """Wrapper around Session.query()."""
         return self.session.query(*entities, **kwargs)
 
     def add(self, *instances: Any) -> None:
         """Save one or more objects to the database."""
```

### Comparing `sqla_utils-0.6.0/PKG-INFO` & `sqla_utils-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqla-utils
-Version: 0.6.0
+Version: 0.6.1
 Summary: Opinionated utilities for working with SQLAlchemy
 Home-page: https://github.com/srittau/sqla-utils
 License: MIT
 Keywords: sqlalchemy,orm
 Author: Sebastian Rittau
 Author-email: srittau@rittau.biz
 Requires-Python: >=3.8,<4
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Dist: SQLAlchemy (>=1.4,<3)
 Project-URL: Repository, https://github.com/srittau/sqla-utils
 Description-Content-Type: text/markdown
 
 # sqla-utils
```

