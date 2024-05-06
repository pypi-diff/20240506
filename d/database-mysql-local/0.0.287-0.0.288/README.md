# Comparing `tmp/database-mysql-local-0.0.287.tar.gz` & `tmp/database_mysql_local-0.0.288.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-mysql-local-0.0.287.tar", last modified: Thu Apr 11 17:20:14 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.288.tar", last modified: Mon May  6 20:44:29 2024, max compression
```

## Comparing `database-mysql-local-0.0.287.tar` & `database_mysql_local-0.0.288.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:20:14.553295 database-mysql-local-0.0.287/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:19:22.000000 database-mysql-local-0.0.287/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-11 17:20:14.553295 database-mysql-local-0.0.287/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-11 17:19:22.000000 database-mysql-local-0.0.287/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:20:14.549295 database-mysql-local-0.0.287/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:20:14.553295 database-mysql-local-0.0.287/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:19:22.000000 database-mysql-local-0.0.287/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-11 17:19:22.000000 database-mysql-local-0.0.287/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-11 17:19:22.000000 database-mysql-local-0.0.287/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-11 17:19:22.000000 database-mysql-local-0.0.287/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-04-11 17:19:47.000000 database-mysql-local-0.0.287/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31705 2024-04-11 17:19:22.000000 database-mysql-local-0.0.287/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-11 17:19:22.000000 database-mysql-local-0.0.287/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-11 17:19:22.000000 database-mysql-local-0.0.287/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-11 17:19:22.000000 database-mysql-local-0.0.287/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-04-11 17:19:43.000000 database-mysql-local-0.0.287/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-11 17:19:22.000000 database-mysql-local-0.0.287/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-11 17:19:22.000000 database-mysql-local-0.0.287/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:20:14.553295 database-mysql-local-0.0.287/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-11 17:20:14.000000 database-mysql-local-0.0.287/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-11 17:20:14.000000 database-mysql-local-0.0.287/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:20:14.000000 database-mysql-local-0.0.287/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-11 17:20:14.000000 database-mysql-local-0.0.287/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-11 17:20:14.000000 database-mysql-local-0.0.287/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-11 17:19:47.000000 database-mysql-local-0.0.287/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 17:20:14.557295 database-mysql-local-0.0.287/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-11 17:19:47.000000 database-mysql-local-0.0.287/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:44:29.777999 database_mysql_local-0.0.288/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-06 20:44:29.777999 database_mysql_local-0.0.288/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:44:29.773998 database_mysql_local-0.0.288/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:44:29.777999 database_mysql_local-0.0.288/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39424 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31705 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-06 20:43:48.000000 database_mysql_local-0.0.288/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:44:29.777999 database_mysql_local-0.0.288/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-06 20:44:29.000000 database_mysql_local-0.0.288/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-06 20:44:29.000000 database_mysql_local-0.0.288/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:44:29.000000 database_mysql_local-0.0.288/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 20:44:29.000000 database_mysql_local-0.0.288/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 20:44:29.000000 database_mysql_local-0.0.288/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:44:29.777999 database_mysql_local-0.0.288/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-06 20:43:27.000000 database_mysql_local-0.0.288/setup.py
```

### Comparing `database-mysql-local-0.0.287/PKG-INFO` & `database_mysql_local-0.0.288/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.287
+Version: 0.0.288
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database-mysql-local-0.0.287/README.md` & `database_mysql_local-0.0.288/README.md`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.287/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.288/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.287/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.288/database_mysql_local/src/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,19 @@
+from enum import Enum
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 
 DEFAULT_SQL_SELECT_LIMIT = 100
 
+
+class UpdateStatus(Enum):
+    UPDATE_DATA_SOURCE = -1
+    DONT_UPDATE = 0
+    UPDATE_CIRCLEZ = 1
+
+
 # connector / cursor
 DATABASE_MYSQL_PYTHON_PACKAGE_COMPONENT_ID = 112
 DATABASE_MYSQL_PYTHON_PACKAGE_COMPONENT_NAME = 'database_mysql_local\\connector'
 CONNECTOR_DEVELOPER_EMAIL = 'idan.a@circ.zone'
 LOGGER_CONNECTOR_CODE_OBJECT = {
     'component_id': DATABASE_MYSQL_PYTHON_PACKAGE_COMPONENT_ID,
     'component_name': DATABASE_MYSQL_PYTHON_PACKAGE_COMPONENT_NAME,
```

### Comparing `database-mysql-local-0.0.287/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.288/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.287/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.288/database_mysql_local/src/generic_crud.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.287/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.288/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.287/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.288/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.287/database_mysql_local/src/point.py` & `database_mysql_local-0.0.288/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.287/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.288/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.287/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.288/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.287/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.288/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.287/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.288/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.287/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.288/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.287
+Version: 0.0.288
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database-mysql-local-0.0.287/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.288/database_mysql_local.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,10 +12,11 @@
 database_mysql_local/src/constants.py
 database_mysql_local/src/cursor.py
 database_mysql_local/src/generic_crud.py
 database_mysql_local/src/generic_crud_ml.py
 database_mysql_local/src/generic_mapping.py
 database_mysql_local/src/point.py
 database_mysql_local/src/polygon.py
+database_mysql_local/src/sync_conflict_resolution.py
 database_mysql_local/src/table_definition.py
 database_mysql_local/src/to_sql_interface.py
 database_mysql_local/src/utils.py
```

### Comparing `database-mysql-local-0.0.287/pyproject.toml` & `database_mysql_local-0.0.288/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.287" # https://pypi.org/project/database-mysql-local
+version = "0.0.288" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database-mysql-local-0.0.287/setup.py` & `database_mysql_local-0.0.288/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 # TODO: we are migrating from circles_local_database_python to database_mysql_local
 #  but in the meantime we want to keep both names
 old_name = "circles_local_database_python"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.287',
+    version='0.0.288',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

