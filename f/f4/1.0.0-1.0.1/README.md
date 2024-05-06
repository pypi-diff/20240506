# Comparing `tmp/f4-1.0.0.tar.gz` & `tmp/f4-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f4-1.0.0.tar", last modified: Fri Apr 26 13:28:25 2024, max compression
+gzip compressed data, was "f4-1.0.1.tar", last modified: Mon May  6 13:05:07 2024, max compression
```

## Comparing `f4-1.0.0.tar` & `f4-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-26 13:28:25.538488 f4-1.0.0/
--rw-r--r--   0 srp33      (503) staff       (20)    11357 2023-12-07 22:20:43.000000 f4-1.0.0/LICENSE
--rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-26 13:28:25.538429 f4-1.0.0/PKG-INFO
--rwxr-xr-x   0 srp33      (503) staff       (20)       67 2023-12-07 22:20:43.000000 f4-1.0.0/README.md
--rw-r--r--   0 srp33      (503) staff       (20)      104 2023-12-07 22:20:43.000000 f4-1.0.0/pyproject.toml
--rw-r--r--   0 srp33      (503) staff       (20)      733 2024-04-26 13:28:25.538805 f4-1.0.0/setup.cfg
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-26 13:28:25.532731 f4-1.0.0/src/
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-26 13:28:25.536526 f4-1.0.0/src/f4/
--rwxr-xr-x   0 srp33      (503) staff       (20)    43623 2024-04-19 19:32:05.000000 f4-1.0.0/src/f4/Builder.py
--rwxr-xr-x   0 srp33      (503) staff       (20)    64912 2024-04-25 15:35:56.000000 f4-1.0.0/src/f4/Parser.py
--rw-r--r--   0 srp33      (503) staff       (20)    16866 2024-04-26 13:04:42.000000 f4-1.0.0/src/f4/Transformer.py
--rwxr-xr-x   0 srp33      (503) staff       (20)     8669 2024-04-26 13:08:43.000000 f4-1.0.0/src/f4/Utilities.py
--rwxr-xr-x   0 srp33      (503) staff       (20)      390 2024-04-20 14:32:09.000000 f4-1.0.0/src/f4/__init__.py
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-26 13:28:25.538204 f4-1.0.0/src/f4.egg-info/
--rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-26 13:28:25.000000 f4-1.0.0/src/f4.egg-info/PKG-INFO
--rw-r--r--   0 srp33      (503) staff       (20)      300 2024-04-26 13:28:25.000000 f4-1.0.0/src/f4.egg-info/SOURCES.txt
--rw-r--r--   0 srp33      (503) staff       (20)        1 2024-04-26 13:28:25.000000 f4-1.0.0/src/f4.egg-info/dependency_links.txt
--rw-r--r--   0 srp33      (503) staff       (20)       67 2024-04-26 13:28:25.000000 f4-1.0.0/src/f4.egg-info/requires.txt
--rw-r--r--   0 srp33      (503) staff       (20)        3 2024-04-26 13:28:25.000000 f4-1.0.0/src/f4.egg-info/top_level.txt
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-26 13:28:25.537439 f4-1.0.0/test/
--rwxr-xr-x   0 srp33      (503) staff       (20)    61473 2024-04-26 13:15:06.000000 f4-1.0.0/test/test.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-05-06 13:05:07.624354 f4-1.0.1/
+-rw-r--r--   0 srp33      (503) staff       (20)    11357 2023-12-07 22:20:43.000000 f4-1.0.1/LICENSE
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-05-06 13:05:07.624294 f4-1.0.1/PKG-INFO
+-rwxr-xr-x   0 srp33      (503) staff       (20)       67 2023-12-07 22:20:43.000000 f4-1.0.1/README.md
+-rw-r--r--   0 srp33      (503) staff       (20)      104 2023-12-07 22:20:43.000000 f4-1.0.1/pyproject.toml
+-rw-r--r--   0 srp33      (503) staff       (20)      733 2024-05-06 13:05:07.624643 f4-1.0.1/setup.cfg
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-05-06 13:05:07.619825 f4-1.0.1/src/
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-05-06 13:05:07.622579 f4-1.0.1/src/f4/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    43623 2024-04-19 19:32:05.000000 f4-1.0.1/src/f4/Builder.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)    64912 2024-04-25 15:35:56.000000 f4-1.0.1/src/f4/Parser.py
+-rw-r--r--   0 srp33      (503) staff       (20)    18358 2024-05-06 12:34:35.000000 f4-1.0.1/src/f4/Transformer.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)     8669 2024-05-06 12:56:18.000000 f4-1.0.1/src/f4/Utilities.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)      390 2024-04-20 14:32:09.000000 f4-1.0.1/src/f4/__init__.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-05-06 13:05:07.624092 f4-1.0.1/src/f4.egg-info/
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-05-06 13:05:07.000000 f4-1.0.1/src/f4.egg-info/PKG-INFO
+-rw-r--r--   0 srp33      (503) staff       (20)      300 2024-05-06 13:05:07.000000 f4-1.0.1/src/f4.egg-info/SOURCES.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        1 2024-05-06 13:05:07.000000 f4-1.0.1/src/f4.egg-info/dependency_links.txt
+-rw-r--r--   0 srp33      (503) staff       (20)       67 2024-05-06 13:05:07.000000 f4-1.0.1/src/f4.egg-info/requires.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        3 2024-05-06 13:05:07.000000 f4-1.0.1/src/f4.egg-info/top_level.txt
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-05-06 13:05:07.623459 f4-1.0.1/test/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    61473 2024-04-26 13:15:06.000000 f4-1.0.1/test/test.py
```

### Comparing `f4-1.0.0/LICENSE` & `f4-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `f4-1.0.0/PKG-INFO` & `f4-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-1.0.0/setup.cfg` & `f4-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = f4
-version = 1.0.0
+version = 1.0.1
 author = Stephen R. Piccolo
 author_email = stephen.piccolo.byu@gmail.com
 description = A Python package for the Fast Fixed-width File Format (F4)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/srp33/f4py
 project_urls =
```

### Comparing `f4-1.0.0/src/f4/Builder.py` & `f4-1.0.1/src/f4/Builder.py`

 * *Files identical despite different names*

### Comparing `f4-1.0.0/src/f4/Parser.py` & `f4-1.0.1/src/f4/Parser.py`

 * *Files identical despite different names*

### Comparing `f4-1.0.0/src/f4/Transformer.py` & `f4-1.0.1/src/f4/Transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         parse_row_values_function = get_parse_row_values_function(src_file_data)
 
         all_column_coords = parse_data_coords(src_file_data, "", column_range)
 
         # We can't compress this file because we have to navigate around it later.
         with open(tmp_fw_file_path, "wb") as fw_file:
             if chunk_number == 0:
-                print_message(f"Filling temp file {tmp_fw_file_path} with new column names for chunk {chunk_number} when transposing {f4_src_file_path}.", verbose)
+                print_message(f"Filling temp file {tmp_fw_file_path} with lnew column names for chunk {chunk_number} when transposing {f4_src_file_path}.", verbose)
                 # Write the value to the top-left cell.
                 fw_file.write(format_string_as_fixed_width(src_column_for_names.encode(), max_column_width) + b"\t")
 
                 # Write the transposed column names (except the last one).
                 for row_index in range(num_rows - 1):
                     src_column_for_names_value = parse_row_value_function(src_file_data, "", row_index, src_column_for_names_coords)
                     fw_file.write(format_string_as_fixed_width(src_column_for_names_value, max_column_width) + b"\t")
@@ -207,80 +207,89 @@
         tmp_dir_path = mkdtemp()
 
     tmp_dir_path = fix_dir_path_ending(tmp_dir_path)
     tmp_tsv_file_path = f"{tmp_dir_path}tmp.tsv.zstd"
 
     with initialize(f4_left_src_file_path, use_memory_mapping) as left_file_data:
         with initialize(f4_right_src_file_path, use_memory_mapping) as right_file_data:
+            print_message(f"Getting join column info when inner joining {f4_left_src_file_path} and {f4_right_src_file_path} and saving to {f4_dest_file_path}.", verbose)
+
             # Determine which functions are suitable for parsing the join column info.
             left_parse_row_value_function = get_parse_row_value_function(left_file_data)
             right_parse_row_value_function = get_parse_row_value_function(right_file_data)
 
             # Find the index of the join column in each file.
             left_join_column_index = get_column_index_from_name(left_file_data, join_column)
             right_join_column_index = get_column_index_from_name(right_file_data, join_column)
 
             # Find the coordinates of the join column in each file.
             left_join_column_coord = parse_data_coord(left_file_data, "", left_join_column_index)
             right_join_column_coord = parse_data_coord(right_file_data, "", right_join_column_index)
 
             # Determine which column values overlap for the join column between the two files.
+            print_message(f"Finding overlapping values in join column when inner joining {f4_left_src_file_path} and {f4_right_src_file_path} and saving to {f4_dest_file_path}.", verbose)
             left_join_column_values = []
             for row_index in range(left_file_data.cache_dict["num_rows"]):
                 value = left_parse_row_value_function(left_file_data, "", row_index, left_join_column_coord)
                 left_join_column_values.append(value)
 
             right_join_column_values = []
             for row_index in range(right_file_data.cache_dict["num_rows"]):
                 value = right_parse_row_value_function(right_file_data, "", row_index, right_join_column_coord)
                 right_join_column_values.append(value)
 
             common_join_values = set(left_join_column_values) & set(right_join_column_values)
 
             # Get column names from the left file.
+            print_message(f"Getting column names from the left file when inner joining {f4_left_src_file_path} and {f4_right_src_file_path} and saving to {f4_dest_file_path}.", verbose)
             left_cn_current, left_cn_end = advance_to_column_names(left_file_data, -1)
             left_columns = []
             for column_index in range(left_file_data.cache_dict["num_cols"]):
                 left_cn_current, column_name = get_next_column_name(left_file_data, left_cn_current, left_cn_end)
                 left_columns.append(column_name)
 
             # Get column names from the right file (excluding the join column).
+            print_message(f"Getting column names from the right file when inner joining {f4_left_src_file_path} and {f4_right_src_file_path} and saving to {f4_dest_file_path}.", verbose)
             right_cn_current, right_cn_end = advance_to_column_names(right_file_data, -1)
             right_columns = []
             for column_index in range(right_file_data.cache_dict["num_cols"]):
                 right_cn_current, column_name = get_next_column_name(right_file_data, right_cn_current, right_cn_end)
                 if column_name != join_column:
                     right_columns.append(column_name)
 
             # Parse the column coordinates for all columns that will be saved.
+            print_message(f"Parsing column coordinatates for all columns when inner joining {f4_left_src_file_path} and {f4_right_src_file_path} and saving to {f4_dest_file_path}.", verbose)
             left_column_coords = [parse_data_coord(left_file_data, "", get_column_index_from_name(left_file_data, name)) for name in left_columns]
             right_column_coords = [parse_data_coord(right_file_data, "", get_column_index_from_name(right_file_data, name)) for name in right_columns]
 
             # Rename columns that are duplicated between left (x) and right (y).
+            print_message(f"Renaming duplicated columns when inner joining {f4_left_src_file_path} and {f4_right_src_file_path} and saving to {f4_dest_file_path}.", verbose)
             for left_i, column_name in enumerate(left_columns):
                 if column_name in right_columns:
                     right_i = right_columns.index(column_name)
                     left_columns[left_i] = (f"{column_name.decode()}.x").encode()
                     right_columns[right_i] = (f"{right_columns[right_i].decode()}.y").encode()
 
             # Create a cache of the right row index for each join value. This speeds up a later step.
+            print_message(f"Creating a cache of the right row index when inner joining {f4_left_src_file_path} and {f4_right_src_file_path} and saving to {f4_dest_file_path}.", verbose)
             right_index_dict = {}
             for i, value in enumerate(right_join_column_values):
                 if value in common_join_values:
                     right_index_dict.setdefault(value, []).append(i)
 
             # Determine which functions are suitable for parsing all columns.
             left_parse_row_values_function = get_parse_row_values_function(left_file_data)
             right_parse_row_values_function = get_parse_row_values_function(right_file_data)
 
             #TODO: Parallelize this?
             with open_temp_file_to_compress(tmp_tsv_file_path) as tmp_tsv_file:
                 tmp_tsv_file.write(b"\t".join(left_columns + right_columns) + b"\n")
 
                 for left_row_index, left_value in enumerate(left_join_column_values):
+                    print_message(f"Joining rows and saving to temp file when inner joining {f4_left_src_file_path} and {f4_right_src_file_path} and saving to {f4_dest_file_path}.", verbose, left_row_index)
                     if left_value in common_join_values:
                         for right_row_index in right_index_dict[left_value]:
                             left_save_values = left_parse_row_values_function(left_file_data, "", left_row_index, left_column_coords)
                             right_save_values = right_parse_row_values_function(right_file_data, "", right_row_index, right_column_coords)
 
                             tmp_tsv_file.write(b"\t".join(left_save_values + right_save_values) + b"\n")
```

### Comparing `f4-1.0.0/src/f4/Utilities.py` & `f4-1.0.1/src/f4/Utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import sqlite3
 import sys
 from tempfile import mkdtemp
 from uuid import uuid4
 from zstandard import ZstdCompressor, ZstdDecompressor
 
 def get_current_version():
-    return "1.0.0"
+    return "1.0.1"
 
 #####################################################
 # Constants
 #####################################################
 
 def get_current_version_major():
     return get_current_version().split(".")[0]
```

### Comparing `f4-1.0.0/src/f4.egg-info/PKG-INFO` & `f4-1.0.1/src/f4.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-1.0.0/test/test.py` & `f4-1.0.1/test/test.py`

 * *Files identical despite different names*

