# Comparing `tmp/sanctify-1.4.1.tar.gz` & `tmp/sanctify-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanctify-1.4.1.tar", last modified: Fri Apr 26 08:58:00 2024, max compression
+gzip compressed data, was "sanctify-1.4.2.tar", last modified: Mon May  6 12:40:58 2024, max compression
```

## Comparing `sanctify-1.4.1.tar` & `sanctify-1.4.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-04-26 08:58:00.953573 sanctify-1.4.1/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    11349 2023-07-24 05:34:49.000000 sanctify-1.4.1/LICENSE
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    19181 2024-04-26 08:58:00.953195 sanctify-1.4.1/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    18062 2023-09-20 08:58:16.000000 sanctify-1.4.1/README.md
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1814 2024-04-26 08:56:53.000000 sanctify-1.4.1/pyproject.toml
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-04-26 08:58:00.940561 sanctify-1.4.1/sanctify/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1286 2024-04-26 08:57:18.000000 sanctify-1.4.1/sanctify/__init__.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    18219 2024-04-26 08:49:28.000000 sanctify-1.4.1/sanctify/cleanser.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2805 2024-03-08 13:21:10.000000 sanctify-1.4.1/sanctify/constants.py
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-04-26 08:58:00.950364 sanctify-1.4.1/sanctify/examples/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      329 2024-04-26 08:57:18.000000 sanctify-1.4.1/sanctify/examples/__init__.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2155 2024-03-09 16:56:05.000000 sanctify-1.4.1/sanctify/examples/column_mapping_schema.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3238 2023-10-16 06:12:09.000000 sanctify-1.4.1/sanctify/examples/data_type_schema.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      332 2023-08-07 05:30:23.000000 sanctify-1.4.1/sanctify/exception.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    14964 2024-04-26 08:57:18.000000 sanctify-1.4.1/sanctify/processor.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4145 2023-08-07 05:30:23.000000 sanctify-1.4.1/sanctify/serializer.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    12902 2024-04-26 08:57:18.000000 sanctify-1.4.1/sanctify/transformer.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4922 2024-03-12 11:16:48.000000 sanctify-1.4.1/sanctify/utils.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    13172 2024-04-26 08:57:18.000000 sanctify-1.4.1/sanctify/validator.py
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-04-26 08:58:00.952337 sanctify-1.4.1/sanctify.egg-info/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    19181 2024-04-26 08:58:00.000000 sanctify-1.4.1/sanctify.egg-info/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      497 2024-04-26 08:58:00.000000 sanctify-1.4.1/sanctify.egg-info/SOURCES.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2024-04-26 08:58:00.000000 sanctify-1.4.1/sanctify.egg-info/dependency_links.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      256 2024-04-26 08:58:00.000000 sanctify-1.4.1/sanctify.egg-info/requires.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2024-04-26 08:58:00.000000 sanctify-1.4.1/sanctify.egg-info/top_level.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2024-04-26 08:58:00.953740 sanctify-1.4.1/setup.cfg
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-05-06 12:40:58.042117 sanctify-1.4.2/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    11349 2023-07-24 05:34:49.000000 sanctify-1.4.2/LICENSE
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    19181 2024-05-06 12:40:58.041804 sanctify-1.4.2/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    18062 2023-09-20 08:58:16.000000 sanctify-1.4.2/README.md
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1814 2024-05-06 12:40:45.000000 sanctify-1.4.2/pyproject.toml
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-05-06 12:40:58.039341 sanctify-1.4.2/sanctify/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1286 2024-05-06 12:38:35.000000 sanctify-1.4.2/sanctify/__init__.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    18285 2024-05-06 12:40:45.000000 sanctify-1.4.2/sanctify/cleanser.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2805 2024-03-08 13:21:10.000000 sanctify-1.4.2/sanctify/constants.py
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-05-06 12:40:58.041114 sanctify-1.4.2/sanctify/examples/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      329 2024-05-06 12:38:35.000000 sanctify-1.4.2/sanctify/examples/__init__.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2155 2024-03-09 16:56:05.000000 sanctify-1.4.2/sanctify/examples/column_mapping_schema.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3238 2023-10-16 06:12:09.000000 sanctify-1.4.2/sanctify/examples/data_type_schema.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      332 2023-08-07 05:30:23.000000 sanctify-1.4.2/sanctify/exception.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    14964 2024-05-06 12:38:35.000000 sanctify-1.4.2/sanctify/processor.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4145 2023-08-07 05:30:23.000000 sanctify-1.4.2/sanctify/serializer.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    12902 2024-05-06 12:38:35.000000 sanctify-1.4.2/sanctify/transformer.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     4922 2024-03-12 11:16:48.000000 sanctify-1.4.2/sanctify/utils.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    13172 2024-05-06 12:38:35.000000 sanctify-1.4.2/sanctify/validator.py
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2024-05-06 12:40:58.041527 sanctify-1.4.2/sanctify.egg-info/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    19181 2024-05-06 12:40:58.000000 sanctify-1.4.2/sanctify.egg-info/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      497 2024-05-06 12:40:58.000000 sanctify-1.4.2/sanctify.egg-info/SOURCES.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2024-05-06 12:40:58.000000 sanctify-1.4.2/sanctify.egg-info/dependency_links.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      256 2024-05-06 12:40:58.000000 sanctify-1.4.2/sanctify.egg-info/requires.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2024-05-06 12:40:58.000000 sanctify-1.4.2/sanctify.egg-info/top_level.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2024-05-06 12:40:58.042160 sanctify-1.4.2/setup.cfg
```

### Comparing `sanctify-1.4.1/LICENSE` & `sanctify-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.1/PKG-INFO` & `sanctify-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.4.1
+Version: 1.4.2
 Summary: Column Mapping based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sanctify-1.4.1/README.md` & `sanctify-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.1/pyproject.toml` & `sanctify-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 [tool.pytest.ini_options]
 log_cli=true
 log_cli_level='DEBUG'
 
 [project]
 name = "sanctify"
-version = "1.4.1"
+version = "1.4.2"
 authors = [{name = "Avijeet Diwaker", email = "avijeetdiwaker@gmail.com"}]
 description = "Column Mapping based cleansing and validations for a given pandas dataframe"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `sanctify-1.4.1/sanctify/__init__.py` & `sanctify-1.4.2/sanctify/__init__.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.1/sanctify/cleanser.py` & `sanctify-1.4.2/sanctify/cleanser.py`

 * *Files 2% similar despite different names*

```diff
@@ -396,23 +396,23 @@
 
         # Remove aggregated columns
         if remove_agg_cols is True:
             self.df = self.df.drop(columns=list(agg_cols_map.keys()), inplace=False)
 
         return self.df
 
-    def merge_same_data_type_column(self, merge_column_name: str) -> pd.DataFrame:
-        cell_phone_columns = [
-            key
-            for key, value in self.column_mapping_schema.items()
-            if merge_column_name == value.get(Constants.STANDARD_COLUMN.value)
+    def merge_same_data_type_column(self, merge_column_data_type: str) -> pd.DataFrame:
+        same_data_type_columns = [
+            raw_column
+            for raw_column, column_config in self.column_mapping_schema.items()
+            if merge_column_data_type.lower() == column_config.get(Constants.DATA_TYPE.value).lower()
         ]
 
-        for col in cell_phone_columns[1:]:
-            self.df[cell_phone_columns[0]] = (
-                self.df[cell_phone_columns[0]].replace("", pd.NA).combine_first(self.df[col])
+        for col in same_data_type_columns[1:]:
+            self.df[same_data_type_columns[0]] = (
+                self.df[same_data_type_columns[0]].replace("", pd.NA).combine_first(self.df[col])
             )
             self.column_mapping_schema[col][Constants.DATA_TYPE.value] = PrimitiveDataTypes.STRING.value
             self.column_mapping_schema[col].pop(Constants.STANDARD_COLUMN.value, None)
         self.input_vs_standard_column_mapping = self.extract_input_vs_standard_column_mapping()
 
         return self.df
```

### Comparing `sanctify-1.4.1/sanctify/constants.py` & `sanctify-1.4.2/sanctify/constants.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.1/sanctify/examples/column_mapping_schema.py` & `sanctify-1.4.2/sanctify/examples/column_mapping_schema.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.1/sanctify/examples/data_type_schema.py` & `sanctify-1.4.2/sanctify/examples/data_type_schema.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.1/sanctify/processor.py` & `sanctify-1.4.2/sanctify/processor.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.1/sanctify/serializer.py` & `sanctify-1.4.2/sanctify/serializer.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.1/sanctify/transformer.py` & `sanctify-1.4.2/sanctify/transformer.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.1/sanctify/utils.py` & `sanctify-1.4.2/sanctify/utils.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.1/sanctify/validator.py` & `sanctify-1.4.2/sanctify/validator.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.4.1/sanctify.egg-info/PKG-INFO` & `sanctify-1.4.2/sanctify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.4.1
+Version: 1.4.2
 Summary: Column Mapping based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

