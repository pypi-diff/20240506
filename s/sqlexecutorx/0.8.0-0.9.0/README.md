# Comparing `tmp/sqlexecutorx-0.8.0.tar.gz` & `tmp/sqlexecutorx-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlexecutorx-0.8.0.tar", last modified: Sun May  5 02:08:23 2024, max compression
+gzip compressed data, was "sqlexecutorx-0.9.0.tar", last modified: Mon May  6 02:42:30 2024, max compression
```

## Comparing `sqlexecutorx-0.8.0.tar` & `sqlexecutorx-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-05 02:08:23.358988 sqlexecutorx-0.8.0/
--rw-rw-r--   0 summy      (501) staff       (20)    11357 2024-03-14 05:16:15.000000 sqlexecutorx-0.8.0/LICENSE
--rw-r--r--   0 summy      (501) staff       (20)     2027 2024-05-05 02:08:23.355869 sqlexecutorx-0.8.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)     1577 2024-05-04 03:23:13.000000 sqlexecutorx-0.8.0/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-05 02:08:23.359277 sqlexecutorx-0.8.0/setup.cfg
--rw-rw-r--   0 summy      (501) staff       (20)     1168 2024-05-05 02:08:04.000000 sqlexecutorx-0.8.0/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-05 02:08:23.344237 sqlexecutorx-0.8.0/sqlexecutorx/
--rw-rw-r--   0 summy      (501) staff       (20)     1373 2024-05-05 01:28:17.000000 sqlexecutorx-0.8.0/sqlexecutorx/__init__.py
--rw-rw-r--   0 summy      (501) staff       (20)      209 2024-05-04 03:22:15.000000 sqlexecutorx-0.8.0/sqlexecutorx/constant.py
--rw-rw-r--   0 summy      (501) staff       (20)    11285 2024-05-05 01:22:27.000000 sqlexecutorx-0.8.0/sqlexecutorx/core.py
--rw-r--r--   0 summy      (501) staff       (20)      901 2024-03-23 15:57:10.000000 sqlexecutorx-0.8.0/sqlexecutorx/engine.py
--rw-rw-r--   0 summy      (501) staff       (20)     2063 2024-05-05 02:01:30.000000 sqlexecutorx-0.8.0/sqlexecutorx/init_import.py
--rw-rw-r--   0 summy      (501) staff       (20)      740 2024-03-25 03:02:59.000000 sqlexecutorx-0.8.0/sqlexecutorx/log_support.py
--rw-rw-r--   0 summy      (501) staff       (20)     1031 2024-05-04 03:22:15.000000 sqlexecutorx-0.8.0/sqlexecutorx/pooling.py
--rw-r--r--   0 summy      (501) staff       (20)      422 2024-03-29 05:50:43.000000 sqlexecutorx-0.8.0/sqlexecutorx/sql_support.py
--rw-rw-r--   0 summy      (501) staff       (20)     3892 2024-03-25 02:25:33.000000 sqlexecutorx-0.8.0/sqlexecutorx/support.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-05 02:08:23.354198 sqlexecutorx-0.8.0/sqlexecutorx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     2027 2024-05-05 02:08:23.000000 sqlexecutorx-0.8.0/sqlexecutorx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      432 2024-05-05 02:08:23.000000 sqlexecutorx-0.8.0/sqlexecutorx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-05 02:08:23.000000 sqlexecutorx-0.8.0/sqlexecutorx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-05 02:08:23.000000 sqlexecutorx-0.8.0/sqlexecutorx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-05 02:08:23.000000 sqlexecutorx-0.8.0/sqlexecutorx.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-06 02:42:30.584761 sqlexecutorx-0.9.0/
+-rw-rw-r--   0 summy      (501) staff       (20)    11357 2024-03-14 05:16:15.000000 sqlexecutorx-0.9.0/LICENSE
+-rw-r--r--   0 summy      (501) staff       (20)     2027 2024-05-06 02:42:30.584046 sqlexecutorx-0.9.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     1577 2024-05-04 03:23:13.000000 sqlexecutorx-0.9.0/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-06 02:42:30.585092 sqlexecutorx-0.9.0/setup.cfg
+-rw-rw-r--   0 summy      (501) staff       (20)     1168 2024-05-06 02:42:23.000000 sqlexecutorx-0.9.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-06 02:42:30.574273 sqlexecutorx-0.9.0/sqlexecutorx/
+-rw-rw-r--   0 summy      (501) staff       (20)     1373 2024-05-05 01:28:17.000000 sqlexecutorx-0.9.0/sqlexecutorx/__init__.py
+-rw-rw-r--   0 summy      (501) staff       (20)      209 2024-05-04 03:22:15.000000 sqlexecutorx-0.9.0/sqlexecutorx/constant.py
+-rw-rw-r--   0 summy      (501) staff       (20)    11285 2024-05-05 01:22:27.000000 sqlexecutorx-0.9.0/sqlexecutorx/core.py
+-rw-r--r--   0 summy      (501) staff       (20)      901 2024-03-23 15:57:10.000000 sqlexecutorx-0.9.0/sqlexecutorx/engine.py
+-rw-rw-r--   0 summy      (501) staff       (20)     2063 2024-05-05 02:01:30.000000 sqlexecutorx-0.9.0/sqlexecutorx/init_import.py
+-rw-rw-r--   0 summy      (501) staff       (20)      739 2024-05-06 02:41:09.000000 sqlexecutorx-0.9.0/sqlexecutorx/log_support.py
+-rw-rw-r--   0 summy      (501) staff       (20)     1031 2024-05-04 03:22:15.000000 sqlexecutorx-0.9.0/sqlexecutorx/pooling.py
+-rw-r--r--   0 summy      (501) staff       (20)      422 2024-03-29 05:50:43.000000 sqlexecutorx-0.9.0/sqlexecutorx/sql_support.py
+-rw-rw-r--   0 summy      (501) staff       (20)     3892 2024-03-25 02:25:33.000000 sqlexecutorx-0.9.0/sqlexecutorx/support.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-06 02:42:30.582888 sqlexecutorx-0.9.0/sqlexecutorx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     2027 2024-05-06 02:42:30.000000 sqlexecutorx-0.9.0/sqlexecutorx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      432 2024-05-06 02:42:30.000000 sqlexecutorx-0.9.0/sqlexecutorx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-06 02:42:30.000000 sqlexecutorx-0.9.0/sqlexecutorx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-05 02:08:23.000000 sqlexecutorx-0.9.0/sqlexecutorx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-06 02:42:30.000000 sqlexecutorx-0.9.0/sqlexecutorx.egg-info/top_level.txt
```

### Comparing `sqlexecutorx-0.8.0/LICENSE` & `sqlexecutorx-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.8.0/PKG-INFO` & `sqlexecutorx-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlexecutorx
-Version: 0.8.0
+Version: 0.9.0
 Summary: A simple thread safe sql executor for Python with connection pool. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlexecutorx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
```

### Comparing `sqlexecutorx-0.8.0/README.rst` & `sqlexecutorx-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.8.0/setup.py` & `sqlexecutorx-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 setup(
     name='sqlexecutorx',
     packages=['sqlexecutorx'],
     description="A simple thread safe sql executor for Python with connection pool. Support MySQL, PostgreSQL, SQLite etc.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.8.0',
+    version='0.9.0',
     url='https://gitee.com/summry/sqlexecutorx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Database', 'Python', 'RDB'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlexecutorx-0.8.0/sqlexecutorx/__init__.py` & `sqlexecutorx-0.9.0/sqlexecutorx/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.8.0/sqlexecutorx/core.py` & `sqlexecutorx-0.9.0/sqlexecutorx/core.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.8.0/sqlexecutorx/engine.py` & `sqlexecutorx-0.9.0/sqlexecutorx/engine.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.8.0/sqlexecutorx/init_import.py` & `sqlexecutorx-0.9.0/sqlexecutorx/init_import.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.8.0/sqlexecutorx/log_support.py` & `sqlexecutorx-0.9.0/sqlexecutorx/log_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from logging import basicConfig, INFO, getLogger
 
 logger = getLogger(__name__)
-basicConfig(level=INFO, format='[%(asctime)s %(levelname)s]: %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+basicConfig(level=INFO, format='[%(asctime)s %(levelname)s] %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
 
 
 def db_ctx_log(action, connection):
     logger.debug("%s connection <%s>..." % (action, hex(id(connection))))
 
 
 def do_sql_log(module: str, function: str, sql: str, *args):
```

### Comparing `sqlexecutorx-0.8.0/sqlexecutorx/pooling.py` & `sqlexecutorx-0.9.0/sqlexecutorx/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.8.0/sqlexecutorx/support.py` & `sqlexecutorx-0.9.0/sqlexecutorx/support.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.8.0/sqlexecutorx.egg-info/PKG-INFO` & `sqlexecutorx-0.9.0/sqlexecutorx.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlexecutorx
-Version: 0.8.0
+Version: 0.9.0
 Summary: A simple thread safe sql executor for Python with connection pool. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlexecutorx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
```

