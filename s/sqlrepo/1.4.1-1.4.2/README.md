# Comparing `tmp/sqlrepo-1.4.1.tar.gz` & `tmp/sqlrepo-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlrepo-1.4.1.tar", last modified: Fri Apr 26 12:05:12 2024, max compression
+gzip compressed data, was "sqlrepo-1.4.2.tar", last modified: Mon May  6 09:19:40 2024, max compression
```

## Comparing `sqlrepo-1.4.1.tar` & `sqlrepo-1.4.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    10244 2024-04-22 06:04:46.394911 sqlrepo-1.4.1/README.md
--rw-r--r--   0        0        0     3054 2024-04-26 12:05:12.060707 sqlrepo-1.4.1/pyproject.toml
--rw-r--r--   0        0        0       37 2024-01-16 08:47:35.121506 sqlrepo-1.4.1/sqlrepo/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2024-01-16 08:47:35.121506 sqlrepo-1.4.1/sqlrepo/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2024-01-16 08:47:35.121506 sqlrepo-1.4.1/sqlrepo/.pytest_cache/README.md
--rw-r--r--   0        0        0      130 2024-01-16 08:47:35.121506 sqlrepo-1.4.1/sqlrepo/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2024-01-16 08:47:35.121506 sqlrepo-1.4.1/sqlrepo/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      463 2024-04-15 09:56:07.307086 sqlrepo-1.4.1/sqlrepo/__init__.py
--rw-r--r--   0        0        0      828 2024-04-22 06:04:46.395911 sqlrepo-1.4.1/sqlrepo/exc.py
--rw-r--r--   0        0        0      798 2024-04-15 09:17:49.278046 sqlrepo-1.4.1/sqlrepo/logging.py
--rw-r--r--   0        0        0        0 2024-04-16 08:40:42.695391 sqlrepo-1.4.1/sqlrepo/py.typed
--rw-r--r--   0        0        0    32880 2024-04-22 06:04:46.396911 sqlrepo-1.4.1/sqlrepo/queries.py
--rw-r--r--   0        0        0    23853 2024-04-22 06:04:46.396911 sqlrepo-1.4.1/sqlrepo/repositories.py
--rw-r--r--   0        0        0     4696 2024-04-22 06:04:46.396911 sqlrepo-1.4.1/sqlrepo/uow.py
--rw-r--r--   0        0        0     1057 2024-04-22 06:04:46.396911 sqlrepo-1.4.1/sqlrepo/wrappers.py
--rw-r--r--   0        0        0        0 2023-12-29 20:17:14.670751 sqlrepo-1.4.1/tests/__init__.py
--rw-r--r--   0        0        0     8306 2024-04-18 09:54:19.867457 sqlrepo-1.4.1/tests/conftest.py
--rw-r--r--   0        0        0    14662 2024-04-19 14:00:47.946165 sqlrepo-1.4.1/tests/test_async_queries.py
--rw-r--r--   0        0        0    11193 2024-04-19 13:59:20.466566 sqlrepo-1.4.1/tests/test_async_repositories.py
--rw-r--r--   0        0        0     1771 2024-04-22 06:04:46.396911 sqlrepo-1.4.1/tests/test_async_uow.py
--rw-r--r--   0        0        0    17037 2024-04-22 06:04:46.397911 sqlrepo-1.4.1/tests/test_base_queries.py
--rw-r--r--   0        0        0     2983 2024-04-22 06:04:46.397911 sqlrepo-1.4.1/tests/test_base_repositories.py
--rw-r--r--   0        0        0    13863 2024-04-19 13:47:29.322240 sqlrepo-1.4.1/tests/test_sync_queries.py
--rw-r--r--   0        0        0    10428 2024-04-19 13:50:29.889774 sqlrepo-1.4.1/tests/test_sync_repositories.py
--rw-r--r--   0        0        0     1540 2024-04-22 06:04:46.397911 sqlrepo-1.4.1/tests/test_sync_uow.py
--rw-r--r--   0        0        0     1061 2024-04-22 06:04:46.397911 sqlrepo-1.4.1/tests/test_wrappers.py
--rw-r--r--   0        0        0      804 2024-04-15 06:16:49.991950 sqlrepo-1.4.1/tests/types.py
--rw-r--r--   0        0        0     7155 2024-04-19 14:04:27.333651 sqlrepo-1.4.1/tests/utils.py
--rw-r--r--   0        0        0    10597 1970-01-01 00:00:00.000000 sqlrepo-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    10244 2024-04-22 06:04:46.394911 sqlrepo-1.4.2/README.md
+-rw-r--r--   0        0        0     3054 2024-05-06 09:19:40.069292 sqlrepo-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-01-16 08:47:35.121506 sqlrepo-1.4.2/sqlrepo/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2024-01-16 08:47:35.121506 sqlrepo-1.4.2/sqlrepo/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2024-01-16 08:47:35.121506 sqlrepo-1.4.2/sqlrepo/.pytest_cache/README.md
+-rw-r--r--   0        0        0      130 2024-01-16 08:47:35.121506 sqlrepo-1.4.2/sqlrepo/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2024-01-16 08:47:35.121506 sqlrepo-1.4.2/sqlrepo/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      463 2024-04-15 09:56:07.307086 sqlrepo-1.4.2/sqlrepo/__init__.py
+-rw-r--r--   0        0        0      828 2024-04-22 06:04:46.395911 sqlrepo-1.4.2/sqlrepo/exc.py
+-rw-r--r--   0        0        0      798 2024-04-15 09:17:49.278046 sqlrepo-1.4.2/sqlrepo/logging.py
+-rw-r--r--   0        0        0        0 2024-04-16 08:40:42.695391 sqlrepo-1.4.2/sqlrepo/py.typed
+-rw-r--r--   0        0        0    32880 2024-04-22 06:04:46.396911 sqlrepo-1.4.2/sqlrepo/queries.py
+-rw-r--r--   0        0        0    23853 2024-04-22 06:04:46.396911 sqlrepo-1.4.2/sqlrepo/repositories.py
+-rw-r--r--   0        0        0     4696 2024-04-22 06:04:46.396911 sqlrepo-1.4.2/sqlrepo/uow.py
+-rw-r--r--   0        0        0     1057 2024-04-22 06:04:46.396911 sqlrepo-1.4.2/sqlrepo/wrappers.py
+-rw-r--r--   0        0        0        0 2023-12-29 20:17:14.670751 sqlrepo-1.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     8306 2024-04-18 09:54:19.867457 sqlrepo-1.4.2/tests/conftest.py
+-rw-r--r--   0        0        0    14662 2024-04-19 14:00:47.946165 sqlrepo-1.4.2/tests/test_async_queries.py
+-rw-r--r--   0        0        0    11193 2024-04-19 13:59:20.466566 sqlrepo-1.4.2/tests/test_async_repositories.py
+-rw-r--r--   0        0        0     1771 2024-04-22 06:04:46.396911 sqlrepo-1.4.2/tests/test_async_uow.py
+-rw-r--r--   0        0        0    17037 2024-04-22 06:04:46.397911 sqlrepo-1.4.2/tests/test_base_queries.py
+-rw-r--r--   0        0        0     2983 2024-04-22 06:04:46.397911 sqlrepo-1.4.2/tests/test_base_repositories.py
+-rw-r--r--   0        0        0    13863 2024-04-19 13:47:29.322240 sqlrepo-1.4.2/tests/test_sync_queries.py
+-rw-r--r--   0        0        0    10428 2024-04-19 13:50:29.889774 sqlrepo-1.4.2/tests/test_sync_repositories.py
+-rw-r--r--   0        0        0     1540 2024-04-22 06:04:46.397911 sqlrepo-1.4.2/tests/test_sync_uow.py
+-rw-r--r--   0        0        0     1061 2024-04-22 06:04:46.397911 sqlrepo-1.4.2/tests/test_wrappers.py
+-rw-r--r--   0        0        0      804 2024-04-15 06:16:49.991950 sqlrepo-1.4.2/tests/types.py
+-rw-r--r--   0        0        0     7155 2024-04-19 14:04:27.333651 sqlrepo-1.4.2/tests/utils.py
+-rw-r--r--   0        0        0    10597 1970-01-01 00:00:00.000000 sqlrepo-1.4.2/PKG-INFO
```

### Comparing `sqlrepo-1.4.1/README.md` & `sqlrepo-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/pyproject.toml` & `sqlrepo-1.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -172,24 +172,24 @@
     "httpx>=0.27.0",
     "pyment>=0.3.3",
     "ipython>=8.19.0",
 ]
 
 [project]
 name = "sqlrepo"
-version = "1.4.1"
+version = "1.4.2"
 description = "sqlalchemy repositories with crud operations and other utils for it."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = [
     "sqlalchemy>=2.0.29",
-    "python-dev-utils[sqlalchemy_filters]>=1.5.0",
+    "python-dev-utils[sqlalchemy_filters]>=1.8.3",
 ]
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
```

### Comparing `sqlrepo-1.4.1/sqlrepo/exc.py` & `sqlrepo-1.4.2/sqlrepo/exc.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/sqlrepo/logging.py` & `sqlrepo-1.4.2/sqlrepo/logging.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/sqlrepo/queries.py` & `sqlrepo-1.4.2/sqlrepo/queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/sqlrepo/repositories.py` & `sqlrepo-1.4.2/sqlrepo/repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/sqlrepo/uow.py` & `sqlrepo-1.4.2/sqlrepo/uow.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/sqlrepo/wrappers.py` & `sqlrepo-1.4.2/sqlrepo/wrappers.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/tests/conftest.py` & `sqlrepo-1.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/tests/test_async_queries.py` & `sqlrepo-1.4.2/tests/test_async_queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/tests/test_async_repositories.py` & `sqlrepo-1.4.2/tests/test_async_repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/tests/test_async_uow.py` & `sqlrepo-1.4.2/tests/test_async_uow.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/tests/test_base_queries.py` & `sqlrepo-1.4.2/tests/test_base_queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/tests/test_base_repositories.py` & `sqlrepo-1.4.2/tests/test_base_repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/tests/test_sync_queries.py` & `sqlrepo-1.4.2/tests/test_sync_queries.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/tests/test_sync_repositories.py` & `sqlrepo-1.4.2/tests/test_sync_repositories.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/tests/test_sync_uow.py` & `sqlrepo-1.4.2/tests/test_sync_uow.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/tests/test_wrappers.py` & `sqlrepo-1.4.2/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/tests/types.py` & `sqlrepo-1.4.2/tests/types.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/tests/utils.py` & `sqlrepo-1.4.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `sqlrepo-1.4.1/PKG-INFO` & `sqlrepo-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: sqlrepo
-Version: 1.4.1
+Version: 1.4.2
 Summary: sqlalchemy repositories with crud operations and other utils for it.
 Author-Email: Dmitriy Lunev <dima.lunev14@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: sqlalchemy>=2.0.29
-Requires-Dist: python-dev-utils[sqlalchemy_filters]>=1.5.0
+Requires-Dist: python-dev-utils[sqlalchemy_filters]>=1.8.3
 Description-Content-Type: text/markdown
 
 # sqlrepo
 
 ![coverage](./coverage.svg)
 
 > Repository pattern implementation for SQLAlchemy models.
```

