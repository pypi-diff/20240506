# Comparing `tmp/beanhub_import-0.0.4.tar.gz` & `tmp/beanhub_import-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_import-0.0.4.tar", max compression
+gzip compressed data, was "beanhub_import-0.0.5.tar", max compression
```

## Comparing `beanhub_import-0.0.4.tar` & `beanhub_import-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-06 05:22:50.139170 beanhub_import-0.0.4/LICENSE
--rw-r--r--   0        0        0      174 2024-05-06 05:22:50.139170 beanhub_import-0.0.4/README.md
--rw-r--r--   0        0        0        0 2024-05-06 05:22:50.139170 beanhub_import-0.0.4/beanhub_import/__init__.py
--rw-r--r--   0        0        0       28 2024-05-06 05:22:50.139170 beanhub_import-0.0.4/beanhub_import/constants.py
--rw-r--r--   0        0        0     3551 2024-05-06 05:22:50.139170 beanhub_import-0.0.4/beanhub_import/data_types.py
--rw-r--r--   0        0        0     6614 2024-05-06 05:22:50.139170 beanhub_import-0.0.4/beanhub_import/post_processor.py
--rw-r--r--   0        0        0     7989 2024-05-06 05:22:50.139170 beanhub_import-0.0.4/beanhub_import/processor.py
--rw-r--r--   0        0        0      725 2024-05-06 05:22:50.139170 beanhub_import-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-06 05:49:52.619195 beanhub_import-0.0.5/LICENSE
+-rw-r--r--   0        0        0      174 2024-05-06 05:49:52.619195 beanhub_import-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 05:49:52.619195 beanhub_import-0.0.5/beanhub_import/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-06 05:49:52.619195 beanhub_import-0.0.5/beanhub_import/constants.py
+-rw-r--r--   0        0        0     3551 2024-05-06 05:49:52.619195 beanhub_import-0.0.5/beanhub_import/data_types.py
+-rw-r--r--   0        0        0     6767 2024-05-06 05:49:52.619195 beanhub_import-0.0.5/beanhub_import/post_processor.py
+-rw-r--r--   0        0        0     7989 2024-05-06 05:49:52.619195 beanhub_import-0.0.5/beanhub_import/processor.py
+-rw-r--r--   0        0        0      725 2024-05-06 05:49:52.619195 beanhub_import-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.0.5/PKG-INFO
```

### Comparing `beanhub_import-0.0.4/LICENSE` & `beanhub_import-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.0.4/beanhub_import/data_types.py` & `beanhub_import-0.0.5/beanhub_import/data_types.py`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.0.4/beanhub_import/post_processor.py` & `beanhub_import-0.0.5/beanhub_import/post_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,18 +39,23 @@
                 date_directive = first_child.children[0]
                 directive_type = date_directive.data.value
                 if directive_type != "txn":
                     continue
                 last_txn = date_directive
             elif first_child.data == "metadata_item":
                 metadata_key = first_child.children[0].value
-                metadata_value = json.loads(first_child.children[1].value)
-                if metadata_key == import_id_key:
+                metadata_value = first_child.children[1]
+                if (
+                    metadata_key == import_id_key
+                    and metadata_value.type == "ESCAPED_STRING"
+                ):
                     yield ImportedTransaction(
-                        file=bean_path, lineno=last_txn.meta.line, id=metadata_value
+                        file=bean_path,
+                        lineno=last_txn.meta.line,
+                        id=json.loads(metadata_value.value),
                     )
 
 
 def compute_changes(
     generated_txns: list[GeneratedTransaction],
     imported_txns: list[ImportedTransaction],
     work_dir: pathlib.Path,
```

### Comparing `beanhub_import-0.0.4/beanhub_import/processor.py` & `beanhub_import-0.0.5/beanhub_import/processor.py`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.0.4/pyproject.toml` & `beanhub_import-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beanhub-import"
-version = "0.0.4"
+version = "0.0.5"
 description = "The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `beanhub_import-0.0.4/PKG-INFO` & `beanhub_import-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanhub-import
-Version: 0.0.4
+Version: 0.0.5
 Summary: The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

