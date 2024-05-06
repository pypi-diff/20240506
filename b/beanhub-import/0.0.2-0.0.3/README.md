# Comparing `tmp/beanhub_import-0.0.2.tar.gz` & `tmp/beanhub_import-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_import-0.0.2.tar", max compression
+gzip compressed data, was "beanhub_import-0.0.3.tar", max compression
```

## Comparing `beanhub_import-0.0.2.tar` & `beanhub_import-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-06 02:11:53.115597 beanhub_import-0.0.2/LICENSE
--rw-r--r--   0        0        0      174 2024-05-06 02:11:53.115597 beanhub_import-0.0.2/README.md
--rw-r--r--   0        0        0        0 2024-05-06 02:11:53.115597 beanhub_import-0.0.2/beanhub_import/__init__.py
--rw-r--r--   0        0        0       28 2024-05-06 02:11:53.115597 beanhub_import-0.0.2/beanhub_import/constants.py
--rw-r--r--   0        0        0     3530 2024-05-06 02:11:53.115597 beanhub_import-0.0.2/beanhub_import/data_types.py
--rw-r--r--   0        0        0     6235 2024-05-06 02:11:53.115597 beanhub_import-0.0.2/beanhub_import/post_processor.py
--rw-r--r--   0        0        0     7245 2024-05-06 02:11:53.115597 beanhub_import-0.0.2/beanhub_import/processor.py
--rw-r--r--   0        0        0      725 2024-05-06 02:11:53.115597 beanhub_import-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-06 03:21:54.899383 beanhub_import-0.0.3/LICENSE
+-rw-r--r--   0        0        0      174 2024-05-06 03:21:54.899383 beanhub_import-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 03:21:54.899383 beanhub_import-0.0.3/beanhub_import/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-06 03:21:54.899383 beanhub_import-0.0.3/beanhub_import/constants.py
+-rw-r--r--   0        0        0     3530 2024-05-06 03:21:54.903383 beanhub_import-0.0.3/beanhub_import/data_types.py
+-rw-r--r--   0        0        0     6318 2024-05-06 03:21:54.903383 beanhub_import-0.0.3/beanhub_import/post_processor.py
+-rw-r--r--   0        0        0     7245 2024-05-06 03:21:54.903383 beanhub_import-0.0.3/beanhub_import/processor.py
+-rw-r--r--   0        0        0      725 2024-05-06 03:21:54.903383 beanhub_import-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.0.3/PKG-INFO
```

### Comparing `beanhub_import-0.0.2/LICENSE` & `beanhub_import-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.0.2/beanhub_import/data_types.py` & `beanhub_import-0.0.3/beanhub_import/data_types.py`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.0.2/beanhub_import/post_processor.py` & `beanhub_import-0.0.3/beanhub_import/post_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,32 +47,36 @@
                 if metadata_key == import_id_key:
                     yield ImportedTransaction(
                         file=bean_path, lineno=last_txn.meta.line, id=metadata_value
                     )
 
 
 def compute_changes(
-    generated_txns: list[GeneratedTransaction], imported_txns: list[ImportedTransaction]
+    generated_txns: list[GeneratedTransaction],
+    imported_txns: list[ImportedTransaction],
+    work_dir: pathlib.Path,
 ) -> dict[pathlib.Path, ChangeSet]:
     generated_id_txns = {txn.id: txn for txn in generated_txns}
     imported_id_txns = {txn.id: txn for txn in imported_txns}
 
     to_remove = collections.defaultdict(list)
     for txn in imported_txns:
         generated_txn = generated_id_txns.get(txn.id)
-        if generated_txn is not None and txn.file != pathlib.Path(generated_txn.file):
+        if generated_txn is not None and txn.file.resolve() != (
+            work_dir / generated_txn.file
+        ):
             # it appears that the generated txn's file is different from the old one, let's remove it
             to_remove[txn.file].append(txn)
 
     to_add = collections.defaultdict(list)
     to_update = collections.defaultdict(dict)
     for txn in generated_txns:
         imported_txn = imported_id_txns.get(txn.id)
-        generated_file = pathlib.Path(txn.file)
-        if imported_txn is not None and imported_txn.file == generated_file:
+        generated_file = (work_dir / txn.file).resolve()
+        if imported_txn is not None and imported_txn.file.resolve() == generated_file:
             to_update[generated_file][imported_txn.lineno] = txn
         else:
             to_add[generated_file].append(txn)
 
     all_files = frozenset(to_remove.keys()).union(to_add.keys()).union(to_update.keys())
     return {
         file_path: ChangeSet(
```

### Comparing `beanhub_import-0.0.2/beanhub_import/processor.py` & `beanhub_import-0.0.3/beanhub_import/processor.py`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.0.2/pyproject.toml` & `beanhub_import-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beanhub-import"
-version = "0.0.2"
+version = "0.0.3"
 description = "The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `beanhub_import-0.0.2/PKG-INFO` & `beanhub_import-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanhub-import
-Version: 0.0.2
+Version: 0.0.3
 Summary: The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

