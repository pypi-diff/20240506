# Comparing `tmp/osc-ingest-tools-0.5.2rc1.tar.gz` & `tmp/osc_ingest_tools-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osc-ingest-tools-0.5.2rc1.tar", last modified: Sat Oct 21 21:18:30 2023, max compression
+gzip compressed data, was "osc_ingest_tools-0.5.3.tar", last modified: Mon May  6 19:59:46 2024, max compression
```

## Comparing `osc-ingest-tools-0.5.2rc1.tar` & `osc_ingest_tools-0.5.3.tar`

### file list

```diff
@@ -1,24 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:18:30.300083 osc-ingest-tools-0.5.2rc1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-21 21:18:19.000000 osc-ingest-tools-0.5.2rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2023-10-21 21:18:30.300083 osc-ingest-tools-0.5.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2023-10-21 21:18:19.000000 osc-ingest-tools-0.5.2rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:18:30.300083 osc-ingest-tools-0.5.2rc1/osc_ingest_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2023-10-21 21:18:29.000000 osc-ingest-tools-0.5.2rc1/osc_ingest_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      557 2023-10-21 21:18:30.000000 osc-ingest-tools-0.5.2rc1/osc_ingest_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-21 21:18:29.000000 osc-ingest-tools-0.5.2rc1/osc_ingest_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-21 21:18:29.000000 osc-ingest-tools-0.5.2rc1/osc_ingest_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-21 21:18:29.000000 osc-ingest-tools-0.5.2rc1/osc_ingest_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-21 21:18:29.000000 osc-ingest-tools-0.5.2rc1/osc_ingest_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:18:30.300083 osc-ingest-tools-0.5.2rc1/osc_ingest_trino/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-10-21 21:18:19.000000 osc-ingest-tools-0.5.2rc1/osc_ingest_trino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2023-10-21 21:18:19.000000 osc-ingest-tools-0.5.2rc1/osc_ingest_trino/boto3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-10-21 21:18:19.000000 osc-ingest-tools-0.5.2rc1/osc_ingest_trino/dotenv_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2023-10-21 21:18:19.000000 osc-ingest-tools-0.5.2rc1/osc_ingest_trino/sqlcols.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2023-10-21 21:18:19.000000 osc-ingest-tools-0.5.2rc1/osc_ingest_trino/sqltypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2023-10-21 21:18:19.000000 osc-ingest-tools-0.5.2rc1/osc_ingest_trino/trino_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 21:18:30.300083 osc-ingest-tools-0.5.2rc1/osc_ingest_trino/unmanaged/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-10-21 21:18:19.000000 osc-ingest-tools-0.5.2rc1/osc_ingest_trino/unmanaged/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2023-10-21 21:18:19.000000 osc-ingest-tools-0.5.2rc1/osc_ingest_trino/unmanaged/unmanaged_hive_ingest.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2023-10-21 21:18:19.000000 osc-ingest-tools-0.5.2rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-21 21:18:30.300083 osc-ingest-tools-0.5.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-10-21 21:18:19.000000 osc-ingest-tools-0.5.2rc1/setup.py
+-rw-r--r--   0        0        0    11357 2024-05-06 19:59:22.677855 osc_ingest_tools-0.5.3/LICENSE
+-rw-r--r--   0        0        0     3280 2024-05-06 19:59:22.677855 osc_ingest_tools-0.5.3/README.md
+-rw-r--r--   0        0        0      869 2024-05-06 19:59:22.677855 osc_ingest_tools-0.5.3/osc_ingest_trino/__init__.py
+-rw-r--r--   0        0        0     1466 2024-05-06 19:59:22.677855 osc_ingest_tools-0.5.3/osc_ingest_trino/boto3_utils.py
+-rw-r--r--   0        0        0      695 2024-05-06 19:59:22.677855 osc_ingest_tools-0.5.3/osc_ingest_trino/dotenv_utils.py
+-rw-r--r--   0        0        0     2621 2024-05-06 19:59:22.677855 osc_ingest_tools-0.5.3/osc_ingest_trino/sqlcols.py
+-rw-r--r--   0        0        0     2064 2024-05-06 19:59:22.677855 osc_ingest_tools-0.5.3/osc_ingest_trino/sqltypes.py
+-rw-r--r--   0        0        0    11911 2024-05-06 19:59:22.677855 osc_ingest_tools-0.5.3/osc_ingest_trino/trino_utils.py
+-rw-r--r--   0        0        0      348 2024-05-06 19:59:22.677855 osc_ingest_tools-0.5.3/osc_ingest_trino/unmanaged/__init__.py
+-rw-r--r--   0        0        0     3963 2024-05-06 19:59:22.677855 osc_ingest_tools-0.5.3/osc_ingest_trino/unmanaged/unmanaged_hive_ingest.py
+-rw-r--r--   0        0        0     2926 2024-05-06 19:59:46.674063 osc_ingest_tools-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-05-06 19:59:22.681855 osc_ingest_tools-0.5.3/tests/__init__.py
+-rw-r--r--   0        0        0     4101 2024-05-06 19:59:22.681855 osc_ingest_tools-0.5.3/tests/test_trino_utils.py
+-rw-r--r--   0        0        0     5068 1970-01-01 00:00:00.000000 osc_ingest_tools-0.5.3/PKG-INFO
```

### Comparing `osc-ingest-tools-0.5.2rc1/LICENSE` & `osc_ingest_tools-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `osc-ingest-tools-0.5.2rc1/README.md` & `osc_ingest_tools-0.5.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # osc-ingest-tools
+
 python tools to assist with standardized data ingestion workflows
 
+## Installation, Usage, and Release Management
+
 ### Install from PyPi
 
-```
+```python
 pip install osc-ingest-tools
 ```
 
 ### Examples
 
 ```python
 >>> from osc_ingest_trino import *
@@ -38,44 +41,45 @@
 1       nick            15
 2       juli            14
 
 >>> df.info(verbose=True)
 <class 'pandas.core.frame.DataFrame'>
 RangeIndex: 3 entries, 0 to 2
 Data columns (total 2 columns):
- #   Column        Non-Null Count  Dtype 
----  ------        --------------  ----- 
+ #   Column        Non-Null Count  Dtype
+---  ------        --------------  -----
  0   first_name    3 non-null      string
- 1   age_in_years  3 non-null      Int64 
+ 1   age_in_years  3 non-null      Int64
 dtypes: Int64(1), string(1)
 memory usage: 179.0 bytes
 
 >>> p = create_table_schema_pairs(df)
 
 >>> print(p)
     first_name varchar,
     age_in_years bigint
 
->>> 
+>>>
 ```
 
 #### Adding custom type mappings to `create_table_schema_pairs`
+
 ```python
 >>> df = pd.DataFrame(data, columns = ['First Name', 'Age In Years'])
 
 >>> enforce_sql_column_names(df, inplace=True)
 
 >>> df.info(verbose=True)
 <class 'pandas.core.frame.DataFrame'>
 RangeIndex: 3 entries, 0 to 2
 Data columns (total 2 columns):
- #   Column        Non-Null Count  Dtype 
----  ------        --------------  ----- 
+ #   Column        Non-Null Count  Dtype
+---  ------        --------------  -----
  0   first_name    3 non-null      object
- 1   age_in_years  3 non-null      int64 
+ 1   age_in_years  3 non-null      int64
 dtypes: int64(1), object(1)
 memory usage: 176.0+ bytes
 
 >>> p = create_table_schema_pairs(df, typemap={'object':'varchar'})
 
 >>> print(p)
     first_name varchar,
@@ -83,58 +87,64 @@
 
 >>>
 ```
 
 ### Development
 
 Patches may be contributed via pull requests to
-https://github.com/os-climate/osc-ingest-tools.
+<https://github.com/os-climate/osc-ingest-tools>.
 
 All changes must pass the automated test suite, along with various static
 checks.
 
 [Black](https://black.readthedocs.io/) code style and
 [isort](https://pycqa.github.io/isort/) import ordering are enforced.
 
 Enabling automatic formatting via [pre-commit](https://pre-commit.com/) is
 recommended:
-```
+
+```shell
 pip install black isort pre-commit
 pre-commit install
 ```
 
 To ensure compliance with static check tools, developers may wish to run;
-```
+
+```shell
 pip install black isort
 # auto-sort imports
 isort .
 # auto-format code
 black .
 ```
 
 Code can then be tested using tox.
-```
+
+```shell
 # run static checks and tests
 tox
 # run only tests
 tox -e py3
 # run only static checks
 tox -e static
 # run tests and produce a code coverage report
 tox -e cov
 ```
 
 ### Releasing
+
 To release a new version of this library, authorized developers should;
+
 - Prepare a signed release commit updating `version` in setup.py
 - Tag the commit using [Semantic Versioning](https://semver.org/spec/v2.0.0.html)
-prepended with "v"
+  prepended with "v"
 - Push the tag
 
 E.g.,
-```
+
+```shell
 git commit -sm "Release v0.3.4"
 git tag v0.3.4
 git push --follow-tags
 ```
 
 A Github workflow will then automatically release the version to PyPI.
```

### Comparing `osc-ingest-tools-0.5.2rc1/osc_ingest_trino/__init__.py` & `osc_ingest_tools-0.5.3/osc_ingest_trino/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,23 @@
+"""Functions to simplify use of S3-based data, Pandas dataframes, and Trino SQL tables."""
+
 from .boto3_utils import attach_s3_bucket, upload_directory_to_s3
 from .dotenv_utils import load_credentials_dotenv
-from .sqlcols import enforce_partition_column_order, enforce_sql_column_names, sql_compliant_name
+from .sqlcols import (
+    enforce_partition_column_order,
+    enforce_sql_column_names,
+    sql_compliant_name,
+)
 from .sqltypes import create_table_schema_pairs, pandas_type_to_sql
-from .trino_utils import TrinoBatchInsert, _do_sql, attach_trino_engine, fast_pandas_ingest_via_hive
+from .trino_utils import (
+    TrinoBatchInsert,
+    _do_sql,
+    attach_trino_engine,
+    fast_pandas_ingest_via_hive,
+)
 
 __all__ = [
     "sql_compliant_name",
     "enforce_sql_column_names",
     "enforce_partition_column_order",
     "pandas_type_to_sql",
     "create_table_schema_pairs",
```

### Comparing `osc-ingest-tools-0.5.2rc1/osc_ingest_trino/sqlcols.py` & `osc_ingest_tools-0.5.3/osc_ingest_trino/sqlcols.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+"""Functions to translate Pandas column names to SQL column names."""
+
 import re
+from typing import List, Union, cast
 
 import pandas as pd
 
 __all__ = [
     "sql_compliant_name",
     "enforce_sql_column_names",
     "enforce_partition_column_order",
@@ -10,17 +13,18 @@
 
 _wsdedup = re.compile(r"\s+")
 _usdedup = re.compile(r"__+")
 _rmpunc = re.compile(r"[,.()&$/+-]+")
 
 
 # 63 seems to be a common max column name length
-def sql_compliant_name(name, maxlen=63):
+def sql_compliant_name(name: Union[List[str], str], maxlen=63) -> Union[List[str], str]:
+    """Convert name to a SQL-compliant table or column name, abbreviating some common words."""
     if isinstance(name, list):
-        return [sql_compliant_name(e, maxlen=maxlen) for e in name]
+        return [cast(str, sql_compliant_name(e, maxlen=maxlen)) for e in name]
     w = str(name).casefold().rstrip().lstrip()
     w = w.replace("-", "_")
     w = _rmpunc.sub("", w)
     w = _wsdedup.sub("_", w)
     w = _usdedup.sub("_", w)
     w = w.replace("average", "avg")
     w = w.replace("maximum", "max")
@@ -34,26 +38,28 @@
     # w = w.replace("intensity", "int")
     # w = w.replace("reported", "rep")
     # w = w.replace("revenue", "rev")
     w = w[:maxlen]
     return w
 
 
-def enforce_sql_column_names(df, inplace=False, maxlen=63):
+def enforce_sql_column_names(df: pd.DataFrame, inplace: bool = False, maxlen: int = 63) -> pd.DataFrame:
+    """Ensure that all column names for df are SQL-compliant."""
     if not isinstance(df, pd.DataFrame):
         raise ValueError("df must be a pandas DataFrame")
     icols = df.columns.to_list()
     ocols = sql_compliant_name(icols, maxlen=maxlen)
     if len(set(ocols)) < len(ocols):
         raise ValueError("remapped column names were not unique!")
     rename_map = dict(list(zip(icols, ocols)))
     return df.rename(columns=rename_map, inplace=inplace)
 
 
-def enforce_partition_column_order(df, pcols, inplace=False):
+def enforce_partition_column_order(df: pd.DataFrame, pcols: List[str], inplace: bool = False) -> pd.DataFrame:
+    """Reorder columns names of df to match the order given by pcols."""
     if not isinstance(df, pd.DataFrame):
         raise ValueError("df must be a pandas DataFrame")
     if not isinstance(pcols, list):
         raise ValueError("pcols must be list of column names")
     pcols = [str(e) for e in pcols]
     cols = list(df.columns.values)
     for c in pcols:
@@ -61,7 +67,8 @@
         cols.append(c)
     if not inplace:
         return df[cols]
     for c in cols:
         s = df[c]
         df.drop(columns=[c], inplace=True)
         df[c] = s
+    return df
```

### Comparing `osc-ingest-tools-0.5.2rc1/osc_ingest_trino/trino_utils.py` & `osc_ingest_tools-0.5.3/osc_ingest_trino/trino_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,50 @@
+"""Trino interoperability functions."""
+
 import math
 import os
 import uuid
 from datetime import datetime
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
+import pandas as pd
 import sqlalchemy
 import trino
-from sqlalchemy.engine import create_engine
+from mypy_boto3_s3.service_resource import Bucket
+from sqlalchemy import Connection, Engine, Row, Table, create_engine
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.sql import text
 
 import osc_ingest_trino as osc
 import osc_ingest_trino.unmanaged as oscu
 
+# from sqlalchemy.sql.schema import Table as Table
+
+
 __all__ = [
     "attach_trino_engine",
     "fast_pandas_ingest_via_hive",
     "TrinoBatchInsert",
     "_do_sql",
 ]
 
 
-def attach_trino_engine(env_var_prefix="TRINO", catalog=None, schema=None, verbose=False):
+def attach_trino_engine(
+    env_var_prefix: str = "TRINO",
+    catalog: Optional[str] = None,
+    schema: Optional[str] = None,
+    verbose: Optional[bool] = False,
+) -> Engine:
+    """Return a SQLAlchemy engine object representing a Trino instance.
+
+    env_var_prefix -- a prefix for all environment variables related to the Trino instance.
+    catalog -- the Trino catalog.
+    schema -- the Trino schema.
+    verbose -- if True, print the full string used to connect.
+    """
     sqlstring = "trino://{user}@{host}:{port}".format(
         user=os.environ[f"{env_var_prefix}_USER"],
         host=os.environ[f"{env_var_prefix}_HOST"],
         port=os.environ[f"{env_var_prefix}_PORT"],
     )
     if catalog is not None:
         sqlstring += f"/{catalog}"
@@ -39,15 +59,23 @@
         print(f"using connect string: {sqlstring}")
 
     engine = create_engine(sqlstring, connect_args=sqlargs)
     engine.connect()
     return engine
 
 
-def _do_sql(sql, engine, verbose=False):
+def _do_sql(
+    sql: Union[sqlalchemy.sql.elements.TextClause, str], engine: Engine, verbose: bool = False
+) -> Optional[Sequence[Row[Any]]]:
+    """Execute SQL query, returning the query result.
+
+    sql -- the SQL query.
+    engine -- the SQLAlchemy engine representing the Trino database.
+    verbose -- if True, print the values returned from executing the string.
+    """
     if type(sql) is not sqlalchemy.sql.elements.TextClause:
         sql = text(str(sql))
     if verbose:
         print(sql)
     with engine.begin() as cxn:
         qres = cxn.execute(sql)
     res = None
@@ -55,44 +83,61 @@
         res = qres.fetchall()
         if verbose:
             print(res)
     return res
 
 
 def fast_pandas_ingest_via_hive(  # noqa: C901
-    df,
-    engine,
-    catalog,
-    schema,
-    table,
-    hive_bucket,
-    hive_catalog,
-    hive_schema,
-    partition_columns=[],
-    overwrite=False,
-    typemap={},
-    colmap={},
-    verbose=False,
-):
+    df: pd.DataFrame,
+    engine: Engine,
+    catalog: str,
+    schema: str,
+    table: str,
+    hive_bucket: Bucket,
+    hive_catalog: str,
+    hive_schema: str,
+    partition_columns: List[str] = [],
+    overwrite: bool = False,
+    typemap: Dict[str, str] = {},
+    colmap: Dict[str, str] = {},
+    verbose: bool = False,
+) -> None:
+    """Efficiently export a dataframe into a Trino database.
+
+    df -- the dataframe to export.
+    engine -- the SQLAlchemy engine representing the Trino database.
+    catalog -- the Trino catalog.
+    schema -- the Trino schema.
+    table -- the name of the table created in the schema.
+    hive_bucket -- the backing store of the Hive metastore.
+    hive_catalog -- the Hive metastore catalog (where schemas are created).
+    hive_schema -- the Hive metastore schema (where tables will be created).
+    partition_columns -- if not empty, defines the partition columns of the table created.
+    overwrite -- if True, an existing table will be overwritten.
+    typemap -- used to format types that cannot otherwise be properly inferred.
+    colmap -- used to format column names that cannot otherwise be properly inferred.
+    verbose -- if True, print the queries being executed and the results of those queries.
+    """
     uh8 = uuid.uuid4().hex[:8]
     hive_table = f"ingest_temp_{uh8}"
 
     dfw = df
     if len(partition_columns) > 0:
         if verbose:
             print("enforcing dataframe partition column order")
         dfw = osc.enforce_partition_column_order(dfw, partition_columns)
 
     # do this after any changes to DF column orderings above
     columnschema = osc.create_table_schema_pairs(dfw, typemap=typemap, colmap=colmap)
 
     # verify destination table first, to fail early and avoid creation of hive tables
+    fq_tablename = ".".join([catalog, schema, table][(catalog is None) :])
     if verbose:
-        print(f"\nverifying existence of table {catalog}.{schema}.{table}")
-    tabledef = f"create table if not exists {catalog}.{schema}.{table} (\n"
+        print(f"\nverifying existence of table {fq_tablename}")
+    tabledef = f"create table if not exists {fq_tablename} (\n"
     tabledef += f"{columnschema}\n"
     tabledef += ") with (\n    format = 'parquet'"
     if len(partition_columns) > 0:
         tabledef += ",\n"
         tabledef += f"    partitioning = array{partition_columns}"
     tabledef += "\n)"
     _do_sql(tabledef, engine, verbose=verbose)
@@ -118,48 +163,59 @@
             print("\nsyncing partition metadata on intermediate hive table")
         if len(partition_columns) > 0:
             sql = text(f"call {hive_catalog}.system.sync_partition_metadata('{hive_schema}', '{hive_table}', 'FULL')")
             _do_sql(sql, engine, verbose=verbose)
 
         if overwrite:
             if verbose:
-                print(f"\noverwriting data in {catalog}.{schema}.{table}")
-            sql = f"delete from {catalog}.{schema}.{table}"
+                print(f"\noverwriting data in {fq_tablename}")
+            sql = text(f"delete from {fq_tablename}")
             _do_sql(sql, engine, verbose=verbose)
 
         if verbose:
-            print(f"\ntransferring data: {hive_catalog}.{hive_schema}.{hive_table} -> {catalog}.{schema}.{table}")
-        sql = f"insert into {catalog}.{schema}.{table}\nselect * from {hive_catalog}.{hive_schema}.{hive_table}"
+            print(f"\ntransferring data: {hive_catalog}.{hive_schema}.{hive_table} -> {fq_tablename}")
+        sql = text(f"insert into {fq_tablename}\nselect * from {hive_catalog}.{hive_schema}.{hive_table}")
         _do_sql(sql, engine, verbose=verbose)
 
         if verbose:
             print(f"\ndeleting table and data for intermediate table {hive_catalog}.{hive_schema}.{hive_table}")
         oscu.drop_unmanaged_table(hive_catalog, hive_schema, hive_table, engine, hive_bucket, verbose=verbose)
     except SQLAlchemyError:
         # Clean up table that will otherwise be orphaned
         if verbose:
             print(f"\ndeleting table and data for intermediate table {hive_catalog}.{hive_schema}.{hive_table}")
         oscu.drop_unmanaged_table(hive_catalog, hive_schema, hive_table, engine, hive_bucket, verbose=verbose)
         raise
 
 
 class TrinoBatchInsert(object):
-    def __init__(self, catalog=None, schema=None, batch_size=1000, optimize=False, verbose=False):
+    """A class used to bundle together basic Trino parameters."""
+
+    def __init__(
+        self,
+        catalog: Optional[str] = None,
+        schema: Optional[str] = None,
+        batch_size: int = 1000,
+        optimize: bool = False,
+        verbose: bool = False,
+    ):
+        """Initialize TrinoBatchInsert objects."""
         self.catalog = catalog
         self.schema = schema
         self.batch_size = batch_size
         self.optimize = optimize
         self.verbose = verbose
 
     # conforms to signature expected by pandas 'callable' value for method kw arg
     # https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.to_sql.html
     # https://pandas.pydata.org/docs/user_guide/io.html#io-sql-method
-    def __call__(self, sqltbl, dbcxn, columns, data_iter):
+    def __call__(self, sqltbl: Table, dbcxn: Connection, columns: List[str], data_iter: List[Tuple]) -> None:
+        """Implement `callable` interface for row-by-row insertion."""
         fqname = self._full_table_name(sqltbl)
-        batch = []
+        batch: List[str] = []
         self.ninserts = 0
         for r in data_iter:
             # each row of data_iter is a python tuple
             # I cannot currently make good use of sqlalchemy ':params'
             # and so I have to do my own "manual" value formatting for insertions
             row = ", ".join([TrinoBatchInsert._sqlform(e) for e in r])
             row = f"({row})"
@@ -175,15 +231,16 @@
                 print("optimizing table files")
             sql = text(f"alter table {fqname} execute optimize")
             qres = dbcxn.execute(sql)
             x = qres.fetchall()
             if self.verbose:
                 print(f"execute optimize: {x}")
 
-    def _do_insert(self, dbcxn, fqname, batch):
+    def _do_insert(self, dbcxn: Connection, fqname: str, batch: List[str]) -> None:
+        """Implement actual row-by-row insertion of BATCH data into table FQNAME using DBCXN database connection."""
         if self.verbose:
             print(f"inserting {len(batch)} records")
             TrinoBatchInsert._print_batch(batch)
         # trino is not currently supporting sqlalchemy cursor.executemany()
         # and so I am generating an insert command with no ':params' that
         # includes all batch data as literal sql values
         valclause = ",\n".join(batch)
@@ -192,28 +249,30 @@
         sql = text(f"insert into {fqname} values\n{valclause}")
         # if self.verbose: print(f'{sql}')
         qres = dbcxn.execute(sql)
         x = qres.fetchall()
         if self.verbose:
             print(f"batch insert result: {x}")
 
-    def _full_table_name(self, sqltbl):
+    def _full_table_name(self, sqltbl: Table) -> str:
+        """Return fully qualified table name for SQLTBL table within this TrinoBatchInsert object."""
         # start with table name
-        name = f"{sqltbl.name}"
+        name: str = f"{sqltbl.name}"
         # prepend schema - allow override from this class
         name = f"{self.schema or sqltbl.schema}.{name}"
         # prepend catalog, if provided
         if self.catalog is not None:
             name = f"{self.catalog}.{name}"
         if self.verbose:
             print(f'constructed fully qualified table name as: "{name}"')
         return name
 
     @staticmethod
-    def _sqlform(x):
+    def _sqlform(x: Any) -> str:
+        """Format the value of x so it can appear in a SQL Values context."""
         if x is None:
             return "NULL"
         if isinstance(x, str):
             # escape any single quotes in the string
             t = x.replace("'", "''")
             # colons are mostly a problem for ':some_id_name', which is interpreted as
             # a parameter requiring binding, but just escaping them all works
@@ -228,14 +287,15 @@
             if math.isinf(x):
                 if x < 0:
                     return "-infinity()"
                 return "infinity()"
         return str(x)
 
     @staticmethod
-    def _print_batch(batch):
+    def _print_batch(batch: List[str]) -> None:
+        """For batch, a list of SQL query lines, print up to the first 5 such."""
         if len(batch) > 5:
             print("\n".join(f"  {e}" for e in batch[:3]))
             print("  ...")
             print(f"  {batch[-1]}")
         else:
             print("\n".join(f"  {e}" for e in batch))
```

### Comparing `osc-ingest-tools-0.5.2rc1/osc_ingest_trino/unmanaged/unmanaged_hive_ingest.py` & `osc_ingest_tools-0.5.3/osc_ingest_trino/unmanaged/unmanaged_hive_ingest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Functions to create, ingest, and drop unmanaged Hive tables."""
+
 import shutil
 import uuid
 
 import pandas as pd
 from sqlalchemy import text
 
 from osc_ingest_trino import create_table_schema_pairs, upload_directory_to_s3
@@ -13,46 +15,51 @@
     "unmanaged_parquet_tabledef",
 ]
 
 _default_prefix = "trino/{schema}/{table}"
 
 
 def _remove_trailing_slash(s):
+    """Remove trailing slash from s."""
     s = str(s)
     if len(s) == 0:
         return s
     if s[-1] != "/":
         return s
     return _remove_trailing_slash(s[:-1])
 
 
 def _prefix(pfx, schema, table):
+    """Translate pfx, schema, and table names into S3 bucket name."""
     return _remove_trailing_slash(pfx).format(schema=schema, table=table)
 
 
 def drop_unmanaged_table(catalog, schema, table, engine, bucket, prefix=_default_prefix, verbose=False):
+    """Drop catalog.schema.table from Hive metastore and also delete its S3 backing store."""
     sql = text(f"drop table if exists {catalog}.{schema}.{table}")
     with engine.begin() as cxn:
         qres = cxn.execute(sql)
     dres = bucket.objects.filter(Prefix=f"{_prefix(prefix, schema, table)}/").delete()
     if verbose:
         print(dres)
     return qres
 
 
 def drop_unmanaged_data(schema, table, bucket, prefix=_default_prefix, verbose=False):
+    """Delete data that may have been orphaned when its table was dropped in Hive metastore."""
     dres = bucket.objects.filter(Prefix=f"{_prefix(prefix, schema, table)}/").delete()
     if verbose:
         print(dres)
     return dres
 
 
 def ingest_unmanaged_parquet(
     df, schema, table, bucket, partition_columns=[], append=True, workdir="/tmp", prefix=_default_prefix, verbose=False
 ):
+    """Ingest data from df into Hive metastore table with backing store bucket."""
     if not isinstance(df, pd.DataFrame):
         raise ValueError("df must be a pandas DataFrame")
     if not isinstance(partition_columns, list):
         raise ValueError("partition_columns must be list of column names")
 
     s3pfx = _prefix(prefix, schema, table)
 
@@ -79,14 +86,15 @@
             print(f"{tmp}  -->  {dst}")
         bucket.upload_file(tmp, dst)
 
 
 def unmanaged_parquet_tabledef(
     df, catalog, schema, table, bucket, partition_columns=[], typemap={}, colmap={}, verbose=False
 ):
+    """Return a SQL string that would create a table suitable for ingesting df into Hive metastore backed by bucket."""
     if not isinstance(df, pd.DataFrame):
         raise ValueError("df must be a pandas DataFrame")
     if not isinstance(partition_columns, list):
         raise ValueError("partition_columns must be list of column names")
 
     columnschema = create_table_schema_pairs(df, typemap=typemap, colmap=colmap)
```

