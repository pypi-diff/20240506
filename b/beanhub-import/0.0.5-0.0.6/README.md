# Comparing `tmp/beanhub_import-0.0.5.tar.gz` & `tmp/beanhub_import-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_import-0.0.5.tar", max compression
+gzip compressed data, was "beanhub_import-0.0.6.tar", max compression
```

## Comparing `beanhub_import-0.0.5.tar` & `beanhub_import-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-06 05:49:52.619195 beanhub_import-0.0.5/LICENSE
--rw-r--r--   0        0        0      174 2024-05-06 05:49:52.619195 beanhub_import-0.0.5/README.md
--rw-r--r--   0        0        0        0 2024-05-06 05:49:52.619195 beanhub_import-0.0.5/beanhub_import/__init__.py
--rw-r--r--   0        0        0       28 2024-05-06 05:49:52.619195 beanhub_import-0.0.5/beanhub_import/constants.py
--rw-r--r--   0        0        0     3551 2024-05-06 05:49:52.619195 beanhub_import-0.0.5/beanhub_import/data_types.py
--rw-r--r--   0        0        0     6767 2024-05-06 05:49:52.619195 beanhub_import-0.0.5/beanhub_import/post_processor.py
--rw-r--r--   0        0        0     7989 2024-05-06 05:49:52.619195 beanhub_import-0.0.5/beanhub_import/processor.py
--rw-r--r--   0        0        0      725 2024-05-06 05:49:52.619195 beanhub_import-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-06 06:12:48.001412 beanhub_import-0.0.6/LICENSE
+-rw-r--r--   0        0        0      174 2024-05-06 06:12:48.001412 beanhub_import-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 06:12:48.001412 beanhub_import-0.0.6/beanhub_import/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-06 06:12:48.001412 beanhub_import-0.0.6/beanhub_import/constants.py
+-rw-r--r--   0        0        0     3551 2024-05-06 06:12:48.001412 beanhub_import-0.0.6/beanhub_import/data_types.py
+-rw-r--r--   0        0        0     6767 2024-05-06 06:12:48.001412 beanhub_import-0.0.6/beanhub_import/post_processor.py
+-rw-r--r--   0        0        0     8134 2024-05-06 06:12:48.001412 beanhub_import-0.0.6/beanhub_import/processor.py
+-rw-r--r--   0        0        0      725 2024-05-06 06:12:48.001412 beanhub_import-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.0.6/PKG-INFO
```

### Comparing `beanhub_import-0.0.5/LICENSE` & `beanhub_import-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.0.5/beanhub_import/data_types.py` & `beanhub_import-0.0.6/beanhub_import/data_types.py`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.0.5/beanhub_import/post_processor.py` & `beanhub_import-0.0.6/beanhub_import/post_processor.py`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.0.5/beanhub_import/processor.py` & `beanhub_import-0.0.6/beanhub_import/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 def process_transaction(
     template_env: SandboxedEnvironment,
     input_config: InputConfigDetails,
     import_rules: list[ImportRule],
     txn: Transaction,
     default_import_id: str | None = None,
 ) -> typing.Generator[GeneratedTransaction, None, None]:
+    logger = logging.getLogger(__name__)
     txn_ctx = dataclasses.asdict(txn)
     default_txn = input_config.default_txn
 
     def render_str(value: str | None) -> str | None:
         if value is None:
             return None
         return template_env.from_string(value).render(**txn_ctx)
@@ -162,14 +163,17 @@
 
             yield GeneratedTransaction(
                 file=render_str(action.file),
                 postings=generated_postings,
                 **{key: render_str(value) for key, value in template_values.items()},
             )
         break
+    logger.debug(
+        "No match found for transaction %s at %s:%s", txn, txn.file, txn.lineno
+    )
 
 
 def process_imports(
     import_doc: ImportDoc,
     input_dir: pathlib.Path,
 ) -> typing.Generator[GeneratedTransaction, None, None]:
     logger = logging.getLogger(__name__)
```

### Comparing `beanhub_import-0.0.5/pyproject.toml` & `beanhub_import-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beanhub-import"
-version = "0.0.5"
+version = "0.0.6"
 description = "The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `beanhub_import-0.0.5/PKG-INFO` & `beanhub_import-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanhub-import
-Version: 0.0.5
+Version: 0.0.6
 Summary: The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

