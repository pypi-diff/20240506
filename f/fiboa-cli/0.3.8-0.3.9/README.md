# Comparing `tmp/fiboa_cli-0.3.8.tar.gz` & `tmp/fiboa_cli-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiboa_cli-0.3.8.tar", last modified: Sat Apr 27 20:21:36 2024, max compression
+gzip compressed data, was "fiboa_cli-0.3.9.tar", last modified: Wed May  1 21:44:17 2024, max compression
```

## Comparing `fiboa_cli-0.3.8.tar` & `fiboa_cli-0.3.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:21:36.363953 fiboa_cli-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-27 20:21:36.363953 fiboa_cli-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:21:36.363953 fiboa_cli-0.3.8/fiboa_cli/
--rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/convert_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/create_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/create_geoparquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/describe.py
--rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/geopandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/jsonschema_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/rename_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/validate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/validate_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/fiboa_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:21:36.363953 fiboa_cli-0.3.8/fiboa_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-04-27 20:21:36.000000 fiboa_cli-0.3.8/fiboa_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-27 20:21:36.000000 fiboa_cli-0.3.8/fiboa_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 20:21:36.000000 fiboa_cli-0.3.8/fiboa_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-27 20:21:36.000000 fiboa_cli-0.3.8/fiboa_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-27 20:21:36.000000 fiboa_cli-0.3.8/fiboa_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 20:21:36.000000 fiboa_cli-0.3.8/fiboa_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 20:21:36.363953 fiboa_cli-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 20:21:36.363953 fiboa_cli-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-27 20:21:29.000000 fiboa_cli-0.3.8/tests/test_jsonschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:44:17.776101 fiboa_cli-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-01 21:44:17.776101 fiboa_cli-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:44:17.776101 fiboa_cli-0.3.9/fiboa_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/convert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/create_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/create_geoparquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/describe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/jsonschema_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/rename_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10417 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/validate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/validate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/fiboa_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:44:17.776101 fiboa_cli-0.3.9/fiboa_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-01 21:44:17.000000 fiboa_cli-0.3.9/fiboa_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-01 21:44:17.000000 fiboa_cli-0.3.9/fiboa_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:44:17.000000 fiboa_cli-0.3.9/fiboa_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-01 21:44:17.000000 fiboa_cli-0.3.9/fiboa_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-01 21:44:17.000000 fiboa_cli-0.3.9/fiboa_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 21:44:17.000000 fiboa_cli-0.3.9/fiboa_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:44:17.776101 fiboa_cli-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:44:17.776101 fiboa_cli-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-01 21:44:13.000000 fiboa_cli-0.3.9/tests/test_jsonschema.py
```

### Comparing `fiboa_cli-0.3.8/LICENSE` & `fiboa_cli-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.8/PKG-INFO` & `fiboa_cli-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.3.8
+Version: 0.3.9
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: jsonschema>=4.20
+Requires-Dist: jsonschema[format]>=4.20
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: pyarrow>=14.0
 Requires-Dist: fsspec>=2024.0
 Requires-Dist: click>=8.1
 Requires-Dist: geopandas>=0.14
 Requires-Dist: requests>=2.30
 Requires-Dist: aiohttp>=3.9
```

### Comparing `fiboa_cli-0.3.8/README.md` & `fiboa_cli-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.8/fiboa_cli/__init__.py` & `fiboa_cli-0.3.9/fiboa_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.8/fiboa_cli/convert.py` & `fiboa_cli-0.3.9/fiboa_cli/convert.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.8/fiboa_cli/convert_utils.py` & `fiboa_cli-0.3.9/fiboa_cli/convert_utils.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.8/fiboa_cli/create_geojson.py` & `fiboa_cli-0.3.9/fiboa_cli/create_geojson.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.8/fiboa_cli/create_geoparquet.py` & `fiboa_cli-0.3.9/fiboa_cli/create_geoparquet.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.8/fiboa_cli/describe.py` & `fiboa_cli-0.3.9/fiboa_cli/describe.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.8/fiboa_cli/geopandas.py` & `fiboa_cli-0.3.9/fiboa_cli/geopandas.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.8/fiboa_cli/jsonschema.py` & `fiboa_cli-0.3.9/fiboa_cli/jsonschema.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.8/fiboa_cli/jsonschema_template.py` & `fiboa_cli-0.3.9/fiboa_cli/jsonschema_template.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.8/fiboa_cli/parquet.py` & `fiboa_cli-0.3.9/fiboa_cli/parquet.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.8/fiboa_cli/rename_extension.py` & `fiboa_cli-0.3.9/fiboa_cli/rename_extension.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.8/fiboa_cli/types.py` & `fiboa_cli-0.3.9/fiboa_cli/types.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.8/fiboa_cli/util.py` & `fiboa_cli-0.3.9/fiboa_cli/util.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.8/fiboa_cli/validate.py` & `fiboa_cli-0.3.9/fiboa_cli/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import pyarrow.types as pat
 
-from jsonschema.validators import Draft7Validator
+from jsonschema.validators import Draft202012Validator
 from .types import PA_TYPE_CHECK
 from .jsonschema import create_jsonschema
 from .util import get_collection, log as log_, log_extensions, load_datatypes, load_file, load_fiboa_schema, load_parquet_data, load_parquet_schema, merge_schemas, parse_metadata, load_collection_schema, load_geoparquet_schema
 from .validate_data import validate_column
 
 def log(text: str, status="info", bullet = True):
     # Indent logs
@@ -289,10 +289,10 @@
 
     return False
 
 def validate_json_schema(obj, schema):
     if isinstance(obj, (bytearray, bytes, str)):
         obj = json.loads(obj)
 
-    validator = Draft7Validator(schema)
+    validator = Draft202012Validator(schema, format_checker=Draft202012Validator.FORMAT_CHECKER)
     errors = sorted(validator.iter_errors(obj), key=lambda e: e.path)
     return errors
```

### Comparing `fiboa_cli-0.3.8/fiboa_cli/validate_data.py` & `fiboa_cli-0.3.9/fiboa_cli/validate_data.py`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.8/fiboa_cli/validate_schema.py` & `fiboa_cli-0.3.9/fiboa_cli/validate_schema.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,10 +29,10 @@
             log(error, "error")
         return False
     else:
         log("VALID", "success")
         return True
 
 def validate_json_schema(obj, schema):
-    validator = Draft202012Validator(schema)
+    validator = Draft202012Validator(schema, format_checker=Draft202012Validator.FORMAT_CHECKER)
     errors = sorted(validator.iter_errors(obj), key=lambda e: e.path)
     return errors
```

### Comparing `fiboa_cli-0.3.8/fiboa_cli.egg-info/PKG-INFO` & `fiboa_cli-0.3.9/fiboa_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.3.8
+Version: 0.3.9
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: jsonschema>=4.20
+Requires-Dist: jsonschema[format]>=4.20
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: pyarrow>=14.0
 Requires-Dist: fsspec>=2024.0
 Requires-Dist: click>=8.1
 Requires-Dist: geopandas>=0.14
 Requires-Dist: requests>=2.30
 Requires-Dist: aiohttp>=3.9
```

### Comparing `fiboa_cli-0.3.8/fiboa_cli.egg-info/SOURCES.txt` & `fiboa_cli-0.3.9/fiboa_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiboa_cli-0.3.8/setup.py` & `fiboa_cli-0.3.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     license="Apache-2.0",
     description="CLI tools such as validation and file format conversion for fiboa.",
     long_description=get_description(),
     long_description_content_type="text/markdown",
     author="Matthias Mohr",
     url="https://github.com/fiboa/cli",
     install_requires=[
-        "jsonschema>=4.20",
+        "jsonschema[format]>=4.20",
         "pyyaml>=6.0",
         "pyarrow>=14.0",
         "fsspec>=2024.0",
         "click>=8.1",
         "geopandas>=0.14",
         "requests>=2.30",
         "aiohttp>=3.9",
```

