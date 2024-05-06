# Comparing `tmp/db2pq-0.0.4.tar.gz` & `tmp/db2pq-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db2pq-0.0.4.tar", last modified: Sun Mar 10 01:48:57 2024, max compression
+gzip compressed data, was "db2pq-0.0.5.tar", last modified: Mon May  6 20:33:11 2024, max compression
```

## Comparing `db2pq-0.0.4.tar` & `db2pq-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 iangow     (501) staff       (20)        0 2024-03-10 01:48:57.613293 db2pq-0.0.4/
--rw-r--r--   0 iangow     (501) staff       (20)     1064 2023-12-30 20:58:38.000000 db2pq-0.0.4/LICENSE
--rw-r--r--   0 iangow     (501) staff       (20)      989 2024-03-10 01:48:57.613099 db2pq-0.0.4/PKG-INFO
--rw-r--r--   0 iangow     (501) staff       (20)      472 2024-01-01 20:22:42.000000 db2pq-0.0.4/README.md
-drwxr-xr-x   0 iangow     (501) staff       (20)        0 2024-03-10 01:48:57.612121 db2pq-0.0.4/db2pq/
--rw-r--r--   0 iangow     (501) staff       (20)      160 2024-03-10 01:48:44.000000 db2pq-0.0.4/db2pq/__init__.py
--rw-r--r--   0 iangow     (501) staff       (20)    17545 2024-03-10 01:48:44.000000 db2pq-0.0.4/db2pq/db2pq.py
-drwxr-xr-x   0 iangow     (501) staff       (20)        0 2024-03-10 01:48:57.612911 db2pq-0.0.4/db2pq.egg-info/
--rw-r--r--   0 iangow     (501) staff       (20)      989 2024-03-10 01:48:57.000000 db2pq-0.0.4/db2pq.egg-info/PKG-INFO
--rw-r--r--   0 iangow     (501) staff       (20)      203 2024-03-10 01:48:57.000000 db2pq-0.0.4/db2pq.egg-info/SOURCES.txt
--rw-r--r--   0 iangow     (501) staff       (20)        1 2024-03-10 01:48:57.000000 db2pq-0.0.4/db2pq.egg-info/dependency_links.txt
--rw-r--r--   0 iangow     (501) staff       (20)       49 2024-03-10 01:48:57.000000 db2pq-0.0.4/db2pq.egg-info/requires.txt
--rw-r--r--   0 iangow     (501) staff       (20)        6 2024-03-10 01:48:57.000000 db2pq-0.0.4/db2pq.egg-info/top_level.txt
--rw-r--r--   0 iangow     (501) staff       (20)       38 2024-03-10 01:48:57.613335 db2pq-0.0.4/setup.cfg
--rw-r--r--   0 iangow     (501) staff       (20)      747 2024-03-10 01:48:44.000000 db2pq-0.0.4/setup.py
+drwxr-xr-x   0 iangow     (501) staff       (20)        0 2024-05-06 20:33:11.726198 db2pq-0.0.5/
+-rw-r--r--   0 iangow     (501) staff       (20)     1064 2023-12-30 20:58:38.000000 db2pq-0.0.5/LICENSE
+-rw-r--r--   0 iangow     (501) staff       (20)     2719 2024-05-06 20:33:11.726021 db2pq-0.0.5/PKG-INFO
+-rw-r--r--   0 iangow     (501) staff       (20)     2202 2024-03-10 07:50:03.000000 db2pq-0.0.5/README.md
+drwxr-xr-x   0 iangow     (501) staff       (20)        0 2024-05-06 20:33:11.724843 db2pq-0.0.5/db2pq/
+-rw-r--r--   0 iangow     (501) staff       (20)      160 2024-03-10 01:48:44.000000 db2pq-0.0.5/db2pq/__init__.py
+-rw-r--r--   0 iangow     (501) staff       (20)    17548 2024-05-06 18:24:20.000000 db2pq-0.0.5/db2pq/db2pq.py
+drwxr-xr-x   0 iangow     (501) staff       (20)        0 2024-05-06 20:33:11.725859 db2pq-0.0.5/db2pq.egg-info/
+-rw-r--r--   0 iangow     (501) staff       (20)     2719 2024-05-06 20:33:11.000000 db2pq-0.0.5/db2pq.egg-info/PKG-INFO
+-rw-r--r--   0 iangow     (501) staff       (20)      203 2024-05-06 20:33:11.000000 db2pq-0.0.5/db2pq.egg-info/SOURCES.txt
+-rw-r--r--   0 iangow     (501) staff       (20)        1 2024-05-06 20:33:11.000000 db2pq-0.0.5/db2pq.egg-info/dependency_links.txt
+-rw-r--r--   0 iangow     (501) staff       (20)       49 2024-05-06 20:33:11.000000 db2pq-0.0.5/db2pq.egg-info/requires.txt
+-rw-r--r--   0 iangow     (501) staff       (20)        6 2024-05-06 20:33:11.000000 db2pq-0.0.5/db2pq.egg-info/top_level.txt
+-rw-r--r--   0 iangow     (501) staff       (20)       38 2024-05-06 20:33:11.726235 db2pq-0.0.5/setup.cfg
+-rw-r--r--   0 iangow     (501) staff       (20)      747 2024-05-06 20:30:46.000000 db2pq-0.0.5/setup.py
```

### Comparing `db2pq-0.0.4/LICENSE` & `db2pq-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `db2pq-0.0.4/db2pq/db2pq.py` & `db2pq-0.0.5/db2pq/db2pq.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     >>> db_to_pq("feed21_bankruptcy_notification", "audit")
     """
     if not alt_table_name:
         alt_table_name = table_name
     
     con = ibis.duckdb.connect()
     uri = f"postgres://{user}@{host}:{port}/{database}"
-    df = con.read_postgres(uri = uri, table_name=table_name, schema=schema)
+    df = con.read_postgres(uri = uri, table_name=table_name, database=schema)
     data_dir = os.path.expanduser(data_dir)
     pq_dir = os.path.join(data_dir, schema)
     if not os.path.exists(pq_dir):
         os.makedirs(pq_dir)
     pq_file = os.path.join(data_dir, schema, alt_table_name + '.parquet')
     tmp_pq_file = os.path.join(data_dir, schema, '.temp_' + alt_table_name + '.parquet')
     
@@ -498,8 +498,8 @@
     if not os.path.exists(schema_dir):
         os.makedirs(schema_dir)
         
     pq_file = Path(data_dir, schema, table_name).with_suffix('.parquet')
     return pq_file
 
 def get_now():
-    return strftime("%Y-%m-%d %H:%M:%S", gmtime())
+    return strftime("%Y-%m-%d %H:%M:%S", gmtime())
```

### Comparing `db2pq-0.0.4/setup.py` & `db2pq-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
     print(long_description)
 
 setuptools.setup(
     name="db2pq",
-    version="0.0.4",
+    version="0.0.5",
     author="Ian Gow",
     author_email="iandgow@gmail.com",
     description="Convert database tables to parquet tables.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iangow/db2pq/",
     packages=setuptools.find_packages(),
```

