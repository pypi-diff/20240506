# Comparing `tmp/pypomes_db-0.4.9.tar.gz` & `tmp/pypomes_db-0.5.0.tar.gz`

## Comparing `pypomes_db-0.4.9.tar` & `pypomes_db-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    19806 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    12532 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    10670 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    20010 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    12532 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    10670 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/PKG-INFO
```

### Comparing `pypomes_db-0.4.9/src/pypomes_db/__init__.py` & `pypomes_db-0.5.0/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.9/src/pypomes_db/db_common.py` & `pypomes_db-0.5.0/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.9/src/pypomes_db/db_pomes.py` & `pypomes_db-0.5.0/src/pypomes_db/db_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         sel_stmt += " WHERE " + "".join(f"{attr} = %s AND " for attr in where_attrs)[0:-5]
     rec: tuple = db_select_one(errors=errors,
                                sel_stmt=sel_stmt,
                                where_vals=where_vals,
                                require_nonempty=False,
                                engine = engine,
                                logger=logger)
-    result: bool = None if len(errors) > 0 else rec is not None
+    result: bool = None if errors else rec is not None
 
     return result
 
 
 def db_select_one(errors: list[str] | None,
                   sel_stmt: str,
                   where_vals: tuple = None,
@@ -301,15 +301,22 @@
     :param update_stmt: the UPDATE command
     :param update_vals: the values for the update operation
     :param where_vals: the values to be associated with the search criteria
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the number of updated tuples, or None if an error occurred
     """
-    return db_execute(errors, update_stmt, update_vals + where_vals, engine, logger)
+    bind_vals: tuple | None = None
+    if update_vals and where_vals:
+        bind_vals = update_vals + where_vals
+    elif update_vals:
+        bind_vals = update_vals
+    elif where_vals:
+        bind_vals = where_vals
+    return db_execute(errors, update_stmt, bind_vals, engine, logger)
 
 
 def db_delete(errors: list[str] | None,
               delete_stmt: str,
               where_vals: tuple = None,
               engine: str = None,
               logger: Logger = None) -> int:
```

### Comparing `pypomes_db-0.4.9/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.5.0/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.9/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.5.0/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.9/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.5.0/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.9/LICENSE` & `pypomes_db-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.4.9/pyproject.toml` & `pypomes_db-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.4.9"
+version = "0.5.0"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.4.9/PKG-INFO` & `pypomes_db-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.4.9
+Version: 0.5.0
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

