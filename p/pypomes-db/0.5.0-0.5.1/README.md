# Comparing `tmp/pypomes_db-0.5.0.tar.gz` & `tmp/pypomes_db-0.5.1.tar.gz`

## Comparing `pypomes_db-0.5.0.tar` & `pypomes_db-0.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    20010 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    12532 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    10670 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/README.md
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 pypomes_db-0.5.1/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 pypomes_db-0.5.1/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    26033 2020-02-02 00:00:00.000000 pypomes_db-0.5.1/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.1/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    12367 2020-02-02 00:00:00.000000 pypomes_db-0.5.1/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    10156 2020-02-02 00:00:00.000000 pypomes_db-0.5.1/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    10433 2020-02-02 00:00:00.000000 pypomes_db-0.5.1/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.5.1/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.5.1/README.md
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 pypomes_db-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.5.1/PKG-INFO
```

### Comparing `pypomes_db-0.5.0/src/pypomes_db/__init__.py` & `pypomes_db-0.5.1/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.0/src/pypomes_db/db_common.py` & `pypomes_db-0.5.1/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.0/src/pypomes_db/db_pomes.py` & `pypomes_db-0.5.1/src/pypomes_db/db_pomes.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     :param db_name: the database or service name
     :param db_user: the logon user
     :param db_pwd: the logon password
     :param db_host: the host URL
     :param db_port: the connection port (a positive integer)
     :param db_driver: the database driver (SQLServer only)
     :param db_client: the path to the client software (optional, Oracle only)
-    :return: True if data was accepted, False otherwise
+    :return: True if the data was accepted, False otherwise
     """
     # initialize the return variable
     result: bool = False
 
     # are the parameters compliant ?
     if (engine in ["mysql", "oracle", "postgres", "sqlserver"] and
         db_name and db_user and db_pwd and db_host and
@@ -96,22 +96,26 @@
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: True if the trial connection succeeded, False otherwise
     """
     # initialize the return variable
     result: bool = False
 
-    curr_engine: str = _assert_engine(errors, engine)
+    curr_engine: str = _assert_engine(errors=errors,
+                                      engine=engine)
     proceed: bool = True
     if curr_engine == "oracle":
         from . import oracle_pomes
         # noinspection PyProtectedMember
-        proceed = oracle_pomes._initialize(errors, logger)
+        proceed = oracle_pomes._initialize(errors=errors,
+                                           logger=logger)
     if proceed:
-        conn: Any = db_connect(errors, curr_engine, logger)
+        conn: Any = db_connect(errors=errors,
+                               engine=curr_engine,
+                               logger=logger)
         if conn:
             conn.close()
             result = True
 
     return result
 
 
@@ -127,106 +131,117 @@
     :param engine: the database engine to use (uses the default engine, if not specified)
     :param logger: optional logger
     :return: the connection to the database
     """
     # initialize the return variable
     result: Any = None
 
-    curr_engine: str = _assert_engine(errors, engine)
+    curr_engine: str = _assert_engine(errors=errors,
+                                      engine=engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_connect(errors, logger)
+        result = oracle_pomes.db_connect(errors=errors,
+                                         logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        result = postgres_pomes.db_connect(errors, logger)
+        result = postgres_pomes.db_connect(errors=errors,
+                                           logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_connect(errors, logger)
+        result = sqlserver_pomes.db_connect(errors=errors,
+                                            logger=logger)
 
     return result
 
 
 def db_exists(errors: list[str],
               table: str,
               where_attrs: list[str] = None,
               where_vals: tuple = None,
               engine: str = None,
+              conn: Any = None,
               logger: Logger = None) -> bool:
     """
     Determine whether the table *table* in the database contains at least one tuple.
 
     For this determination, *where_attrs* are made equal to *where_values* in the query, respectively.
     If more than one, the attributes are concatenated by the *AND* logical connector.
     The targer database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param table: the table to be searched
     :param where_attrs: the search attributes
     :param where_vals: the values for the search attributes
     :param engine: the database engine to use (uses the default engine, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: True if at least one tuple was found
     """
     # noinspection PyDataSource
     sel_stmt: str = "SELECT * FROM " + table
     if where_attrs:
         sel_stmt += " WHERE " + "".join(f"{attr} = %s AND " for attr in where_attrs)[0:-5]
     rec: tuple = db_select_one(errors=errors,
                                sel_stmt=sel_stmt,
                                where_vals=where_vals,
                                require_nonempty=False,
                                engine = engine,
+                               conn=conn,
                                logger=logger)
     result: bool = None if errors else rec is not None
 
     return result
 
 
 def db_select_one(errors: list[str] | None,
                   sel_stmt: str,
                   where_vals: tuple = None,
                   require_nonempty: bool = False,
                   engine: str = None,
+                  conn: Any = None,
                   logger: Logger = None) -> tuple:
     """
     Search the database and return the first tuple that satisfies the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. In case of error, or if the search is empty, *None* is returned.
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: values to be associated with the search criteria
     :param require_nonempty: defines whether an empty search should be considered an error
     :param engine: the database engine to use (uses the default engine, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: tuple containing the search result, or None if there was an error, or if the search was empty
     """
     require_min: int = 1 if require_nonempty else None
     reply: list[tuple] = db_select_all(errors=errors,
                                        sel_stmt=sel_stmt,
                                        where_vals=where_vals,
                                        require_min=require_min,
                                        require_max=1,
                                        engine = engine,
+                                       conn=conn,
                                        logger=logger)
 
     return reply[0] if reply else None
 
 
 def db_select_all(errors: list[str] | None,
                   sel_stmt: str,
                   where_vals: tuple = None,
                   require_min: int = None,
                   require_max: int = None,
                   engine: str = None,
+                  conn: Any = None,
                   logger: Logger = None) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
@@ -235,151 +250,204 @@
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param engine: the database engine to use (uses the default engine, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] | None = None
 
-    curr_engine: str = _assert_engine(errors, engine)
+    curr_engine: str = _assert_engine(errors=errors,
+                                      engine=engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_select_all(errors, sel_stmt, where_vals,
-                                            require_min, require_max,  logger)
+        result = oracle_pomes.db_select_all(errors=errors,
+                                            sel_stmt=sel_stmt,
+                                            where_vals=where_vals,
+                                            require_min=require_min,
+                                            require_max=require_max,
+                                            conn=conn,
+                                            logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        result = postgres_pomes.db_select_all(errors, sel_stmt, where_vals,
-                                              require_min, require_max, logger)
+        result = postgres_pomes.db_select_all(errors=errors,
+                                              sel_stmt=sel_stmt,
+                                              where_vals=where_vals,
+                                              require_min=require_min,
+                                              require_max=require_max,
+                                              conn=conn,
+                                              logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_select_all(errors, sel_stmt, where_vals,
-                                               require_min, require_max, logger)
+        result = sqlserver_pomes.db_select_all(errors=errors,
+                                               sel_stmt=sel_stmt,
+                                               where_vals=where_vals,
+                                               require_min=require_min,
+                                               require_max=require_max,
+                                               conn=conn,
+                                               logger=logger)
 
     return result
 
 
 def db_insert(errors: list[str] | None,
               insert_stmt: str,
               insert_vals: tuple,
               engine: str = None,
+              conn: Any = None,
               logger: Logger = None) -> int:
     """
     Insert a tuple, with values defined in *insert_vals*, into the database.
 
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the values to be inserted
     :param engine: the database engine to use (uses the default engine, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the number of inserted tuples (0 ou 1), or None if an error occurred
     """
-    return db_execute(errors, insert_stmt, insert_vals, engine, logger)
+    return db_execute(errors=errors,
+                      exc_stmt=insert_stmt,
+                      bind_vals=insert_vals,
+                      engine=engine,
+                      conn=conn,
+                      logger=logger)
 
 
 def db_update(errors: list[str] | None,
               update_stmt: str,
               update_vals: tuple = None,
               where_vals: tuple = None,
               engine: str = None,
+              conn: Any = None,
               logger: Logger = None) -> int:
     """
     Update one or more tuples in the database, as defined by the command *update_stmt*.
 
     The values for this update are in *update_vals*.
     The values for selecting the tuples to be updated are in *where_vals*.
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param update_stmt: the UPDATE command
     :param update_vals: the values for the update operation
     :param where_vals: the values to be associated with the search criteria
     :param engine: the database engine to use (uses the default engine, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the number of updated tuples, or None if an error occurred
     """
     bind_vals: tuple | None = None
     if update_vals and where_vals:
         bind_vals = update_vals + where_vals
     elif update_vals:
         bind_vals = update_vals
     elif where_vals:
         bind_vals = where_vals
-    return db_execute(errors, update_stmt, bind_vals, engine, logger)
+    return db_execute(errors=errors,
+                      exc_stmt=update_stmt,
+                      bind_vals=bind_vals,
+                      engine=engine,
+                      conn=conn,
+                      logger=logger)
 
 
 def db_delete(errors: list[str] | None,
               delete_stmt: str,
               where_vals: tuple = None,
               engine: str = None,
+              conn: Any = None,
               logger: Logger = None) -> int:
     """
     Delete one or more tuples in the database, as defined by the *delete_stmt* command.
 
     The values for selecting the tuples to be deleted are in *where_vals*.
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param delete_stmt: the DELETE command
     :param where_vals: the values to be associated with the search criteria
     :param engine: the database engine to use (uses the default engine, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the number of deleted tuples, or None if an error occurred
     """
-    return db_execute(errors, delete_stmt, where_vals, engine, logger)
+    return db_execute(errors=errors,
+                      exc_stmt=delete_stmt,
+                      bind_vals=where_vals,
+                      engine=engine,
+                      conn=conn,
+                      logger=logger)
 
 
 def db_bulk_insert(errors: list[str] | None,
                    insert_stmt: str,
                    insert_vals: list[tuple],
                    engine: str = None,
+                   conn: Any = None,
                    logger: Logger = None) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param engine: the database engine to use (uses the default engine, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     curr_engine: str = _assert_engine(errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
+        result = oracle_pomes.db_bulk_insert(errors=errors,
+                                             insert_stmt=insert_stmt,
+                                             insert_vals=insert_vals,
+                                             conn=conn,
+                                             logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        result = postgres_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
+        result = postgres_pomes.db_bulk_insert(errors=errors,
+                                               insert_stmt=insert_stmt,
+                                               insert_vals=insert_vals,
+                                               conn=conn,
+                                               logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_bulk_insert(errors, insert_stmt, insert_vals, logger)
+        result = sqlserver_pomes.db_bulk_insert(errors=errors,
+                                                insert_stmt=insert_stmt,
+                                                insert_vals=insert_vals,
+                                                conn=conn,
+                                                logger=logger)
 
     return result
 
 
 def db_execute(errors: list[str] | None,
                exc_stmt: str,
                bind_vals: tuple = None,
                engine: str = None,
+               conn: Any = None,
                logger: Logger = None) -> int:
     """
     Execute the command *exc_stmt* on the database.
 
     This command might be a DML ccommand modifying the database, such as
     inserting, updating or deleting tuples, or it might be a DDL statement,
     or it might even be an environment-related command.
@@ -388,99 +456,140 @@
     It might be the number of inserted, modified, or deleted tuples,
     ou None if an error occurred.
 
     :param errors: incidental error messages
     :param exc_stmt: the command to execute
     :param bind_vals: optional bind values
     :param engine: the database engine to use (uses the default engine, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
     curr_engine: str = _assert_engine(errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_execute(errors, exc_stmt, bind_vals, logger)
+        result = oracle_pomes.db_execute(errors=errors,
+                                         exc_stmt=exc_stmt,
+                                         bind_vals=bind_vals,
+                                         conn=conn,
+                                         logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        result = postgres_pomes.db_execute(errors, exc_stmt, bind_vals, logger)
+        result = postgres_pomes.db_execute(errors=errors,
+                                           exc_stmt=exc_stmt,
+                                           bind_vals=bind_vals,
+                                           conn=conn,
+                                           logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_execute(errors, exc_stmt, bind_vals, logger)
+        result = sqlserver_pomes.db_execute(errors=errors,
+                                            exc_stmt=exc_stmt,
+                                            bind_vals=bind_vals,
+                                            conn=conn,
+                                            logger=logger)
 
     return result
 
 
 def db_call_function(errors: list[str] | None,
                      func_name: str,
                      func_vals: tuple = None,
                      engine: str = None,
+                     conn: Any = None,
                      logger: Logger = None) -> list[tuple]:
     """
     Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
 
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param func_name: name of the stored function
     :param func_vals: parameters for the stored function
     :param engine: the database engine to use (uses the default engine, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the data returned by the function
     """
     # initialize the return variable
     result: Any = None
 
     curr_engine: str = _assert_engine(errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_call_function(errors, func_name, func_vals, logger)
+        result = oracle_pomes.db_call_function(errors=errors,
+                                               func_name=func_name,
+                                               func_vals=func_vals,
+                                               conn=conn,
+                                               logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        result = postgres_pomes.db_call_procedure(errors, func_name, func_vals, logger)
+        result = postgres_pomes.db_call_procedure(errors=errors,
+                                                  proc_name=func_name,
+                                                  proc_vals=func_vals,
+                                                  conn=conn,
+                                                  logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_call_procedure(errors, func_name, func_vals, logger)
+        result = sqlserver_pomes.db_call_procedure(errors=errors,
+                                                   proc_name=func_name,
+                                                   proc_vals=func_vals,
+                                                   conn=conn,
+                                                   logger=logger)
 
     return result
 
 
 def db_call_procedure(errors: list[str] | None,
                       proc_name: str,
                       proc_vals: tuple = None,
                       engine: str = None,
+                      conn: Any = None,
                       logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param engine: the database engine to use (uses the default engine, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: Any = None
 
     curr_engine: str = _assert_engine(errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
+        result = oracle_pomes.db_call_procedure(errors=errors,
+                                                proc_name=proc_name,
+                                                proc_vals=proc_vals,
+                                                conn=conn,
+                                                logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        result = postgres_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
+        result = postgres_pomes.db_call_procedure(errors=errors,
+                                                  proc_name=proc_name,
+                                                  proc_vals=proc_vals,
+                                                  conn=conn,
+                                                  logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_call_procedure(errors, proc_name, proc_vals, logger)
+        result = sqlserver_pomes.db_call_procedure(errors=errors,
+                                                   proc_name=proc_name,
+                                                   proc_vals=proc_vals,
+                                                   conn=conn,
+                                                   logger=logger)
 
     return result
```

### Comparing `pypomes_db-0.5.0/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.5.1/src/pypomes_db/oracle_pomes.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     _assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
 
 # TODO: db_call_function, db_call_procedure
 
 
 def db_connect(errors: list[str],
-               logger: Logger = None) -> Connection:
+               logger: Logger) -> Connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
@@ -43,149 +43,146 @@
             query_stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def db_select_all(errors: list[str],
                   sel_stmt: str,
-                  where_vals: tuple = None,
-                  require_min: int = None,
-                  require_max: int = None,
-                  logger: Logger = None) -> list[tuple]:
+                  where_vals: tuple,
+                  require_min: int,
+                  require_max: int,
+                  conn: Connection,
+                  logger: Logger) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
     If the search is empty, an empty list is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
 
-    # retrieve the connection parameters
-    name, user, pwd, host, port = _db_get_params("oracle")
+    # make sure to have a connection
+    curr_conn: Connection = conn or db_connect(errors=errors,
+                                               logger=logger)
 
     if isinstance(require_max, int) and require_max > 0:
         sel_stmt: str = f"{sel_stmt} FETCH NEXT {require_max} ROWS ONLY"
 
     err_msg: str | None = None
     try:
-        # obtain the connection
-        with  connect(service_name=name,
-                      host=host,
-                      port=port,
-                      user=user,
-                      password=pwd) as conn:
-            # make sure the connection is not in autocommit mode
-            conn.autocommit = False
-
-            # obtain a cursor and perform the operation
-            with conn.cursor() as cursor:
-                # execute the query
-                cursor.execute(statement=sel_stmt,
-                               parameters=where_vals)
-                # obtain the number of tuples returned
-                count: int = cursor.rowcount
-
-                # has the query quota been satisfied ?
-                if _assert_query_quota(errors=errors,
-                                       query=sel_stmt,
-                                       where_vals=where_vals,
-                                       count=count,
-                                       require_min=require_min,
-                                       require_max=require_max):
-                    # yes, retrieve the returned tuples
-                    rows: list = cursor.fetchall()
-                    result = [tuple(row) for row in rows]
-            # commit the transaction
-            conn.commit()
+        # obtain a cursor and perform the operation
+        with curr_conn.cursor() as cursor:
+            # execute the query
+            cursor.execute(statement=sel_stmt,
+                           parameters=where_vals)
+            # obtain the number of tuples returned
+            count: int = cursor.rowcount
+
+            # has the query quota been satisfied ?
+            if _assert_query_quota(errors=errors,
+                                   query=sel_stmt,
+                                   where_vals=where_vals,
+                                   count=count,
+                                   require_min=require_min,
+                                   require_max=require_max):
+                # yes, retrieve the returned tuples
+                rows: list = cursor.fetchall()
+                result = [tuple(row) for row in rows]
+        # commit the transaction
+        curr_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
 
 def db_bulk_insert(errors: list[str],
                    insert_stmt: str,
                    insert_vals: list[tuple],
-                   logger: Logger = None) -> int:
+                   conn: Connection,
+                   logger: Logger) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     The binding must be done by position. Thus, the *VALUES* clause in *insert_stmt*
     must contain as many ':n' placeholders as there are elements in the tuples found in the
     list provided in *insert_vals*, where 'n' is the 1-based position of the data in the tuple.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
-    # retrieve the connection parameters
-    name, user, pwd, host, port = _db_get_params("oracle")
+    # make sure to have a connection
+    curr_conn: Connection = conn or db_connect(errors=errors,
+                                               logger=logger)
 
     err_msg: str | None = None
     try:
-        # obtain the connection
-        with  connect(service_name=name,
-                      host=host,
-                      port=port,
-                      user=user,
-                      password=pwd) as conn:
-            # make sure the connection is not in autocommit mode
-            conn.autocommit = False
-
-            # obtain a cursor and perform the operation
-            with conn.cursor() as cursor:
-                try:
-                    cursor.executemany(statement=insert_stmt,
-                                       parameters=insert_vals)
-                    result = len(insert_vals)
-                except Exception:
-                    conn.rollback()
-                    raise
-            conn.commit()
+        # obtain a cursor and perform the operation
+        with curr_conn.cursor() as cursor:
+            try:
+                cursor.executemany(statement=insert_stmt,
+                                   parameters=insert_vals)
+                result = len(insert_vals)
+            except Exception:
+                conn.rollback()
+                raise
+        curr_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
             query_stmt=insert_stmt,
             bind_vals=insert_vals[0])
 
     return result
 
 
 def db_execute(errors: list[str],
                exc_stmt: str,
                bind_vals: tuple,
+               conn: Connection,
                logger: Logger) -> int:
     """
     Execute the command *exc_stmt* on the database.
 
     This command might be a DML ccommand modifying the database, such as
     inserting, updating or deleting tuples, or it might be a DDL statement,
     or it might even be an environment-related command.
@@ -193,43 +190,41 @@
     The value returned is the value obtained from the execution of *exc_stmt*.
     It might be the number of inserted, modified, or deleted tuples,
     ou None if an error occurred.
 
     :param errors: incidental error messages
     :param exc_stmt: the command to execute
     :param bind_vals: optional bind values
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
-    # retrieve the connection parameters
-    name, user, pwd, host, port = _db_get_params("oracle")
+    # make sure to have a connection
+    curr_conn: Connection = conn or db_connect(errors=errors,
+                                               logger=logger)
 
     err_msg: str | None = None
     try:
-        # obtain a connection
-        with  connect(service_name=name,
-                      host=host,
-                      port=port,
-                      user=user,
-                      password=pwd) as conn:
-            # make sure the connection is not in autocommit mode
-            conn.autocommit = False
-            # obtain the cursor and execute the operation
-            with conn.cursor() as cursor:
-                cursor.execute(statement=exc_stmt,
-                               parameters=bind_vals)
-                result = cursor.rowcount
-            # commit the transaction
-            conn.commit()
+        # obtain a cursor and execute the operation
+        with curr_conn.cursor() as cursor:
+            cursor.execute(statement=exc_stmt,
+                           parameters=bind_vals)
+            result = cursor.rowcount
+        # commit the transaction
+        curr_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
             query_stmt=exc_stmt,
             bind_vals=bind_vals)
@@ -238,74 +233,75 @@
 
 
 # TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 # noinspection PyUnusedLocal
 def db_call_function(errors: list[str],
                      func_name: str,
                      func_vals: tuple,
-                     logger: Logger = None) -> list[tuple]:
+                     conn: Connection,
+                     logger: Logger) -> list[tuple]:
     """
     Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
 
     :param errors: incidental error messages
     :param func_name: name of the stored function
     :param func_vals: parameters for the stored function
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the data returned by the function
     """
     # initialize the return variable
     result: list[tuple] = []
 
     return result
 
 
 # TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 def db_call_procedure(errors: list[str],
                       proc_name: str,
                       proc_vals: tuple,
-                      logger: Logger = None) -> list[tuple]:
+                      conn: Connection,
+                      logger: Logger) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     # noinspection DuplicatedCode
     result: list[tuple] = []
 
-    # retrieve the connection parameters
-    name, user, pwd, host, port = _db_get_params("oracle")
+    # make sure to have a connection
+    curr_conn: Connection = conn or db_connect(errors=errors,
+                                               logger=logger)
 
     # execute the stored procedure
     err_msg: str | None = None
     try:
-        # obtain a connection
-        with  connect(service_name=name,
-                      host=host,
-                      port=port,
-                      user=user,
-                      password=pwd) as conn:
-            # make sure the connection is not in autocommit mode
-            conn.autocommit = False
-            # obtain a cursor and perform the operation
-            with conn.cursor() as cursor:
-                cursor.callproc(name=proc_name,
-                                parameters=proc_vals)
-
-                # retrieve the returned tuples
-                result = list(cursor)
-            # commit the transaction
-            conn.commit()
+        # obtain a cursor and perform the operation
+        with curr_conn.cursor() as cursor:
+            cursor.callproc(name=proc_name,
+                            parameters=proc_vals)
+
+            # retrieve the returned tuples
+            result = list(cursor)
+        # commit the transaction
+        curr_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="oracle")
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
             query_stmt=proc_name,
             bind_vals=proc_vals)
```

### Comparing `pypomes_db-0.5.0/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.5.1/src/pypomes_db/postgres_pomes.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,145 +42,143 @@
             query_stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def db_select_all(errors: list[str],
                   sel_stmt: str,
-                  where_vals: tuple = None,
-                  require_min: int = None,
-                  require_max: int = None,
-                  logger: Logger = None) -> list[tuple]:
+                  where_vals: tuple,
+                  require_min: int,
+                  require_max: int,
+                  conn: connection,
+                  logger: Logger) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
     If the search is empty, an empty list is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
 
-    # retrieve the connection parameters
-    name, user, pwd, host, port = _db_get_params("postgres")
+    # make sure to have a connection
+    curr_conn: connection = conn or db_connect(errors=errors,
+                                               logger=logger)
 
     if isinstance(require_max, int) and require_max >= 0:
         sel_stmt += f" LIMIT {require_max}"
 
     err_msg: str | None = None
     try:
-        # obtain a connection
-        with connect(host=host,
-                     port=port,
-                     database=name,
-                     user=user,
-                     password=pwd) as conn:
-            # make sure the connection is not in autocommit mode
-            conn.autocommit = False
-
-            # obtain a cursor and execute the operation
-            with conn.cursor() as cursor:
-                cursor.execute(query=f"{sel_stmt};",
-                               vars=where_vals)
-                # obtain the number of tuples returned
-                count: int = cursor.rowcount
-
-                # has the query quota been satisfied ?
-                if _assert_query_quota(errors=errors,
-                                       query=sel_stmt,
-                                       where_vals=where_vals,
-                                       count=count,
-                                       require_min=require_min,
-                                       require_max=require_max):
-                    # yes, retrieve the returned tuples
-                    result = list(cursor)
+        # obtain a cursor and execute the operation
+        with curr_conn.cursor() as cursor:
+            cursor.execute(query=f"{sel_stmt};",
+                           vars=where_vals)
+            # obtain the number of tuples returned
+            count: int = cursor.rowcount
+
+            # has the query quota been satisfied ?
+            if _assert_query_quota(errors=errors,
+                                   query=sel_stmt,
+                                   where_vals=where_vals,
+                                   count=count,
+                                   require_min=require_min,
+                                   require_max=require_max):
+                # yes, retrieve the returned tuples
+                result = list(cursor)
 
-            # commit the transaction
-            conn.commit()
+        # commit the transaction
+        curr_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
 
 def db_bulk_insert(errors: list[str],
                    insert_stmt: str,
                    insert_vals: list[tuple],
-                   logger: Logger = None) -> int:
+                   conn: connection,
+                   logger: Logger) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     The *VALUES* clause in *insert_stmt* must be simply *VALUES %s*.
     Note that, after the execution of *execute_values*, the *cursor.rowcount* property
     will not contain a total result, and thus the value 1 (one) is returned on success.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
-    # retrieve the connection parameters
-    name, user, pwd, host, port = _db_get_params("postgres")
+    # make sure to have a connection
+    curr_conn: connection = conn or db_connect(errors=errors,
+                                               logger=logger)
 
     # execute the bulk insert
     err_msg: str | None = None
     try:
-        # obtain a connection
-        with connect(host=host,
-                     port=port,
-                     database=name,
-                     user=user,
-                     password=pwd) as conn:
-            # make sure the connection is not in autocommit mode
-            conn.autocommit = False
-            # obtain a cursor and perform the operation
-            with conn.cursor() as cursor:
-                execute_values(cur=cursor,
-                               sql=insert_stmt,
-                               argslist=insert_vals)
-                result = len(insert_vals)
-            # commit the transaction
-            conn.commit()
+        # obtain a cursor and perform the operation
+        with curr_conn.cursor() as cursor:
+            execute_values(cur=cursor,
+                           sql=insert_stmt,
+                           argslist=insert_vals)
+            result = len(insert_vals)
+        # commit the transaction
+        curr_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
             query_stmt=insert_stmt)
 
     return result
 
 
 def db_execute(errors: list[str],
                exc_stmt: str,
                bind_vals: tuple,
+               conn: connection,
                logger: Logger) -> int:
     """
     Execute the command *exc_stmt* on the database.
 
     This command might be a DML ccommand modifying the database, such as
     inserting, updating or deleting tuples, or it might be a DDL statement,
     or it might even be an environment-related command.
@@ -188,99 +186,95 @@
     The value returned is the value obtained from the execution of *exc_stmt*.
     It might be the number of inserted, modified, or deleted tuples,
     ou None if an error occurred.
 
     :param errors: incidental error messages
     :param exc_stmt: the command to execute
     :param bind_vals: optional bind values
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
-    # retrieve the connection parameters
-    name, user, pwd, host, port = _db_get_params("postgres")
+    # make sure to have a connection
+    curr_conn: connection = conn or db_connect(errors=errors,
+                                               logger=logger)
 
     err_msg: str | None = None
     try:
-        # obtain a connection
-        with connect(host=host,
-                     port=port,
-                     database=name,
-                     user=user,
-                     password=pwd) as conn:
-            # make sure the connection is not in autocommit mode
-            conn.autocommit = False
-            # obtain the cursor and execute the operation
-            with conn.cursor() as cursor:
-                cursor.execute(query=f"{exc_stmt};",
-                               vars=bind_vals)
-                result = cursor.rowcount
-            # commit the transaction
-            conn.commit()
+        # obtain a cursor and execute the operation
+        with curr_conn.cursor() as cursor:
+            cursor.execute(query=f"{exc_stmt};",
+                           vars=bind_vals)
+            result = cursor.rowcount
+        # commit the transaction
+        curr_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
             query_stmt=exc_stmt,
             bind_vals=bind_vals)
 
     return result
 
 
 def db_call_procedure(errors: list[str],
                       proc_name: str,
                       proc_vals: tuple,
-                      logger: Logger = None) -> list[tuple]:
+                      conn: connection,
+                      logger: Logger) -> list[tuple]:
     """
     Execute the stored procedure *proc_name*, with the arguments given in *proc_vals*.
 
     :param errors:  incidental error messages
     :param proc_name: the name of the sotred procedure
     :param proc_vals: the arguments to be passed
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: list[tuple] = [()]
 
-    # retrieve the connection parameters
-    name, user, pwd, host, port = _db_get_params("postgres")
+    # make sure to have a connection
+    curr_conn: connection = conn or db_connect(errors=errors,
+                                               logger=logger)
 
     # build the command
     proc_stmt: str = f"{proc_name}(" + "%s, " * (len(proc_vals) - 1) + "%s)"
 
     # execute the stored procedure
     err_msg: str | None = None
     try:
-        # obtain a connection
-        with connect(host=host,
-                     port=port,
-                     database=name,
-                     user=user,
-                     password=pwd) as conn:
-            # make sure the connection is not in autocommit mode
-            conn.autocommit = False
-
-            # obtain a cursor and perform the operation
-            with conn.cursor() as cursor:
-                cursor.execute(query=proc_stmt,
-                               argslist=proc_vals)
-                # retrieve the returned tuples
-                result = list(cursor)
-            # commit the transaction
-            conn.commit()
+        # obtain a cursor and perform the operation
+        with curr_conn.cursor() as cursor:
+            cursor.execute(query=proc_stmt,
+                           argslist=proc_vals)
+            # retrieve the returned tuples
+            result = list(cursor)
+        # commit the transaction
+        curr_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
             query_stmt=proc_stmt,
             bind_vals=proc_vals)
```

### Comparing `pypomes_db-0.5.0/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.5.1/src/pypomes_db/sqlserver_pomes.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,21 +14,27 @@
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
     # initialize the return valiable
     result: Connection | None = None
 
-    # obtain the connection string
-    connection_kwargs: str = _get_connection_kwargs()
+    # retrieve the connection parameters and build the connection string
+    name, user, pwd, host, port, driver = _db_get_params("sqlserver")
+    connection_kwargs: str = (
+        f"DRIVER={{{driver}}};SERVER={host},{port};"
+        f"DATABASE={name};UID={user};PWD={pwd};TrustServerCertificate=yes;"
+    )
 
     # Obtain a connection to the database
     err_msg: str | None = None
     try:
         result = connect(connection_kwargs)
+        # make sure the connection is not in autocommit mode
+        result.autocommit = False
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
 
     # log the results
     name, _user, _pwd, host, _port = _db_get_params("sqlserver")
     _db_log(errors=errors,
@@ -37,138 +43,143 @@
             query_stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
 def db_select_all(errors: list[str],
                   sel_stmt: str,
-                  where_vals: tuple = None,
-                  require_min: int = None,
-                  require_max: int = None,
-                  logger: Logger = None) -> list[tuple]:
+                  where_vals: tuple,
+                  require_min: int,
+                  require_max: int,
+                  conn: Connection,
+                  logger: Logger) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
     If the search is empty, an empty list is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
 
-    # obtain the connection string
-    connection_kwargs: str = _get_connection_kwargs()
+    # make sure to have a connection
+    curr_conn: Connection = conn or db_connect(errors=errors,
+                                               logger=logger)
 
     err_msg: str | None = None
     if isinstance(require_max, int) and require_max > 0:
         sel_stmt: str = sel_stmt.replace("SELECT", f"SELECT TOP {require_max}", 1)
 
     try:
-        # obtain a connection
-        with connect(connection_kwargs) as conn:
-            # make sure the connection is not in autocommit mode
-            conn.autocommit = False
-
-            # obtain a cursor and execute the operation
-            with conn.cursor() as cursor:
-                cursor.execute(sel_stmt, where_vals)
-                # obtain the number of tuples returned
-                count: int = cursor.rowcount
-
-                # has the query quota been satisfied ?
-                if _assert_query_quota(errors=errors,
-                                       query=sel_stmt,
-                                       where_vals=where_vals,
-                                       count=count,
-                                       require_min=require_min,
-                                       require_max=require_max):
-                    # yes, retrieve the returned tuples
-                    rows: list[Row] = cursor.fetchall()
-                    result = [tuple(row) for row in rows]
-            # commit the transaction
-            conn.commit()
+        # obtain a cursor and execute the operation
+        with curr_conn.cursor() as cursor:
+            cursor.execute(sel_stmt, where_vals)
+            # obtain the number of tuples returned
+            count: int = cursor.rowcount
+
+            # has the query quota been satisfied ?
+            if _assert_query_quota(errors=errors,
+                                   query=sel_stmt,
+                                   where_vals=where_vals,
+                                   count=count,
+                                   require_min=require_min,
+                                   require_max=require_max):
+                # yes, retrieve the returned tuples
+                rows: list[Row] = cursor.fetchall()
+                result = [tuple(row) for row in rows]
+        # commit the transaction
+        curr_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
             query_stmt=sel_stmt,
             bind_vals=where_vals)
 
     return result
 
 
 def db_bulk_insert(errors: list[str],
                    insert_stmt: str,
                    insert_vals: list[tuple],
-                   logger: Logger = None) -> int:
+                   conn: Connection,
+                   logger: Logger) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     The *VALUES* clause in *insert_stmt* must contain as many '%s' placeholders
     as there are elements in the tuples found in the list provided in *insert_vals*.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
-    # obtain the connection string
-    connection_kwargs: str = _get_connection_kwargs()
+    # make sure to have a connection
+    curr_conn: Connection = conn or db_connect(errors=errors,
+                                               logger=logger)
 
     err_msg: str | None = None
     try:
-        # obtain a connection
-        with connect(connection_kwargs) as conn:
-            # make sure the connection is not in autocommit mode
-            conn.autocommit = False
-
-            # obtain the cursor and perform the operation
-            with conn.cursor() as cursor:
-                cursor.fast_executemany = True
-                try:
-                    cursor.executemany(insert_stmt, insert_vals)
-                    result = len(insert_vals)
-                except Exception:
-                    conn.rollback()
-                    raise
-            conn.commit()
+        # obtain a cursor and perform the operation
+        with curr_conn.cursor() as cursor:
+            cursor.fast_executemany = True
+            try:
+                cursor.executemany(insert_stmt, insert_vals)
+                result = len(insert_vals)
+            except Exception:
+                conn.rollback()
+                raise
+        curr_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
             query_stmt=insert_stmt,
             bind_vals=insert_vals[0])
 
     return result
 
 
 def db_execute(errors: list[str],
                exc_stmt: str,
                bind_vals: tuple,
+               conn: Connection,
                logger: Logger) -> int:
     """
     Execute the command *exc_stmt* on the database.
 
     This command might be a DML ccommand modifying the database, such as
     inserting, updating or deleting tuples, or it might be a DDL statement,
     or it might even be an environment-related command.
@@ -176,112 +187,97 @@
     The value returned is the value obtained from the execution of *exc_stmt*.
     It might be the number of inserted, modified, or deleted tuples,
     ou None if an error occurred.
 
     :param errors: incidental error messages
     :param exc_stmt: the command to execute
     :param bind_vals: optional bind values
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
-    # obtain the connection string
-    connection_kwargs: str = _get_connection_kwargs()
+    # make sure to have a connection
+    curr_conn: Connection = conn or db_connect(errors=errors,
+                                               logger=logger)
 
     err_msg: str | None = None
     try:
-        # obtain a connection
-        with connect(connection_kwargs) as conn:
-            # make sure the connection is not in autocommit mode
-            conn.autocommit = False
-            # obtain the cursor and execute the operation
-            with conn.cursor() as cursor:
-                cursor.execute(exc_stmt, bind_vals)
-                result = cursor.rowcount
-            # commit the transaction
-            conn.commit()
+        # obtain a cursor and execute the operation
+        with curr_conn.cursor() as cursor:
+            cursor.execute(exc_stmt, bind_vals)
+            result = cursor.rowcount
+        # commit the transaction
+        curr_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
             query_stmt=exc_stmt,
             bind_vals=bind_vals)
 
     return result
 
 
 def db_call_procedure(errors: list[str],
                       proc_name: str,
                       proc_vals: tuple,
-                      require_min: int = None,
-                      require_max: int = None,
+                      conn: Connection,
                       logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
-    :param require_min: optionally defines the minimum number of tuples to be returned
-    :param require_max: optionally defines the maximum number of tuples to be returned
+    :param conn: optional connection to use (obtains a new one, if not specified)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: list[tuple] | None = None
 
-    # obtain the connection string
-    connection_kwargs: str = _get_connection_kwargs()
+    # make sure to have a connection
+    curr_conn: Connection = conn or db_connect(errors=errors,
+                                               logger=logger)
 
     # build the command
     proc_stmt: str | None = None
 
     # execute the stored procedure
     err_msg: str | None = None
     try:
-        # obtain a connection
-        with connect(connection_kwargs) as conn:
-            # make sure the connection is not in autocommit mode
-            conn.autocommit = False
-            # obtain the cursor and execute the operation
-            with conn.cursor() as cursor:
-                proc_stmt = f"SET NOCOUNT ON; EXEC {proc_name} {','.join(('?',) * len(proc_vals))}"
-                cursor.execute(proc_stmt, proc_vals)
-                # obtain the number of tuples returned
-                count: int = cursor.rowcount
-
-                # has the query quota been satisfied ?
-                # noinspection PyTypeChecker
-                if _assert_query_quota(errors, proc_name, None, count, require_min, require_max):
-                    # yes, retrieve the returned tuples
-                    rows: list[Row] = cursor.fetchall()
-                    result = [tuple(row) for row in rows]
-            # commit the transaction
-            conn.commit()
+        # obtain a cursor and execute the operation
+        with curr_conn.cursor() as cursor:
+            proc_stmt = f"SET NOCOUNT ON; EXEC {proc_name} {','.join(('?',) * len(proc_vals))}"
+            cursor.execute(proc_stmt, proc_vals)
+            # retrieve the returned tuples
+            rows: list[Row] = cursor.fetchall()
+            result = [tuple(row) for row in rows]
+        # commit the transaction
+        curr_conn.commit()
     except Exception as e:
         err_msg = _db_except_msg(exception=e,
                                  engine="sqlserver")
+    finally:
+        # close the connection, if locally acquired
+        if not conn:
+            curr_conn.close()
 
     # log the results
     _db_log(errors=errors,
             err_msg=err_msg,
             logger=logger,
             query_stmt=proc_stmt,
             bind_vals=proc_vals)
 
     return result
-
-
-def _get_connection_kwargs() -> str:
-
-    # retrieve the connection parameters
-    name, user, pwd, host, port, driver = _db_get_params("sqlserver")
-    return (
-        f"DRIVER={{{driver}}};SERVER={host},{port};"
-        f"DATABASE={name};UID={user};PWD={pwd};TrustServerCertificate=yes;"
-    )
```

### Comparing `pypomes_db-0.5.0/LICENSE` & `pypomes_db-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.5.0/pyproject.toml` & `pypomes_db-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.5.0/PKG-INFO` & `pypomes_db-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.5.0
+Version: 0.5.1
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

