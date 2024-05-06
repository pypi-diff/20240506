# Comparing `tmp/beanhub_import-0.0.6.tar.gz` & `tmp/beanhub_import-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_import-0.0.6.tar", max compression
+gzip compressed data, was "beanhub_import-0.0.7.tar", max compression
```

## Comparing `beanhub_import-0.0.6.tar` & `beanhub_import-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-06 06:12:48.001412 beanhub_import-0.0.6/LICENSE
--rw-r--r--   0        0        0      174 2024-05-06 06:12:48.001412 beanhub_import-0.0.6/README.md
--rw-r--r--   0        0        0        0 2024-05-06 06:12:48.001412 beanhub_import-0.0.6/beanhub_import/__init__.py
--rw-r--r--   0        0        0       28 2024-05-06 06:12:48.001412 beanhub_import-0.0.6/beanhub_import/constants.py
--rw-r--r--   0        0        0     3551 2024-05-06 06:12:48.001412 beanhub_import-0.0.6/beanhub_import/data_types.py
--rw-r--r--   0        0        0     6767 2024-05-06 06:12:48.001412 beanhub_import-0.0.6/beanhub_import/post_processor.py
--rw-r--r--   0        0        0     8134 2024-05-06 06:12:48.001412 beanhub_import-0.0.6/beanhub_import/processor.py
--rw-r--r--   0        0        0      725 2024-05-06 06:12:48.001412 beanhub_import-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-06 06:38:21.463721 beanhub_import-0.0.7/LICENSE
+-rw-r--r--   0        0        0      174 2024-05-06 06:38:21.463721 beanhub_import-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 06:38:21.463721 beanhub_import-0.0.7/beanhub_import/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-06 06:38:21.463721 beanhub_import-0.0.7/beanhub_import/constants.py
+-rw-r--r--   0        0        0     3583 2024-05-06 06:38:21.463721 beanhub_import-0.0.7/beanhub_import/data_types.py
+-rw-r--r--   0        0        0     6767 2024-05-06 06:38:21.463721 beanhub_import-0.0.7/beanhub_import/post_processor.py
+-rw-r--r--   0        0        0     8229 2024-05-06 06:38:21.463721 beanhub_import-0.0.7/beanhub_import/processor.py
+-rw-r--r--   0        0        0      725 2024-05-06 06:38:21.463721 beanhub_import-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.0.7/PKG-INFO
```

### Comparing `beanhub_import-0.0.6/LICENSE` & `beanhub_import-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.0.6/beanhub_import/data_types.py` & `beanhub_import-0.0.7/beanhub_import/data_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 
 class ImportRule(ImportBaseModel):
     match: TxnMatchRule
     actions: list[Action]
 
 
 class ImportDoc(ImportBaseModel):
+    context: dict | None = None
     inputs: list[InputConfig]
     imports: list[ImportRule]
     outputs: list[OutputConfig] | None = None
 
 
 @dataclasses.dataclass(frozen=True)
 class ImportedTransaction:
```

### Comparing `beanhub_import-0.0.6/beanhub_import/post_processor.py` & `beanhub_import-0.0.7/beanhub_import/post_processor.py`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.0.6/beanhub_import/processor.py` & `beanhub_import-0.0.7/beanhub_import/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,16 @@
 
 def process_imports(
     import_doc: ImportDoc,
     input_dir: pathlib.Path,
 ) -> typing.Generator[GeneratedTransaction, None, None]:
     logger = logging.getLogger(__name__)
     template_env = SandboxedEnvironment()
+    if import_doc.context is not None:
+        template_env.globals.update(import_doc.context)
     for filepath in walk_dir_files(input_dir):
         processed = False
         for input_config in import_doc.inputs:
             if not match_file(input_config.match, filepath):
                 continue
             rel_filepath = filepath.relative_to(input_dir)
             extractor_name = input_config.config.extractor
```

### Comparing `beanhub_import-0.0.6/pyproject.toml` & `beanhub_import-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beanhub-import"
-version = "0.0.6"
+version = "0.0.7"
 description = "The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `beanhub_import-0.0.6/PKG-INFO` & `beanhub_import-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanhub-import
-Version: 0.0.6
+Version: 0.0.7
 Summary: The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

