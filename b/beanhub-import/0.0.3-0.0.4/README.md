# Comparing `tmp/beanhub_import-0.0.3.tar.gz` & `tmp/beanhub_import-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_import-0.0.3.tar", max compression
+gzip compressed data, was "beanhub_import-0.0.4.tar", max compression
```

## Comparing `beanhub_import-0.0.3.tar` & `beanhub_import-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-06 03:21:54.899383 beanhub_import-0.0.3/LICENSE
--rw-r--r--   0        0        0      174 2024-05-06 03:21:54.899383 beanhub_import-0.0.3/README.md
--rw-r--r--   0        0        0        0 2024-05-06 03:21:54.899383 beanhub_import-0.0.3/beanhub_import/__init__.py
--rw-r--r--   0        0        0       28 2024-05-06 03:21:54.899383 beanhub_import-0.0.3/beanhub_import/constants.py
--rw-r--r--   0        0        0     3530 2024-05-06 03:21:54.903383 beanhub_import-0.0.3/beanhub_import/data_types.py
--rw-r--r--   0        0        0     6318 2024-05-06 03:21:54.903383 beanhub_import-0.0.3/beanhub_import/post_processor.py
--rw-r--r--   0        0        0     7245 2024-05-06 03:21:54.903383 beanhub_import-0.0.3/beanhub_import/processor.py
--rw-r--r--   0        0        0      725 2024-05-06 03:21:54.903383 beanhub_import-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-06 05:22:50.139170 beanhub_import-0.0.4/LICENSE
+-rw-r--r--   0        0        0      174 2024-05-06 05:22:50.139170 beanhub_import-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 05:22:50.139170 beanhub_import-0.0.4/beanhub_import/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-06 05:22:50.139170 beanhub_import-0.0.4/beanhub_import/constants.py
+-rw-r--r--   0        0        0     3551 2024-05-06 05:22:50.139170 beanhub_import-0.0.4/beanhub_import/data_types.py
+-rw-r--r--   0        0        0     6614 2024-05-06 05:22:50.139170 beanhub_import-0.0.4/beanhub_import/post_processor.py
+-rw-r--r--   0        0        0     7989 2024-05-06 05:22:50.139170 beanhub_import-0.0.4/beanhub_import/processor.py
+-rw-r--r--   0        0        0      725 2024-05-06 05:22:50.139170 beanhub_import-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.0.4/PKG-INFO
```

### Comparing `beanhub_import-0.0.3/LICENSE` & `beanhub_import-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.0.3/beanhub_import/data_types.py` & `beanhub_import-0.0.4/beanhub_import/data_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,42 +57,47 @@
 
 
 @enum.unique
 class ActionType(str, enum.Enum):
     add_txn = "add_txn"
 
 
+class AmountTemplate(ImportBaseModel):
+    number: str | None = None
+    currency: str | None = None
+
+
 class PostingTemplate(ImportBaseModel):
     # account of the posting
     account: str | None = None
-    # amount of the posting
-    amount: str | None = None
-    # currency of the posting
-    currency: str | None = None
-    # TODO: support cost / price and etc
+    amount: AmountTemplate | None = None
+    price: AmountTemplate | None = None
+    cost: str | None = None
 
 
 class TransactionTemplate(ImportBaseModel):
     # the import-id for de-duplication
     id: str | None = None
     date: str | None = None
     flag: str | None = None
     narration: str | None = None
     payee: str | None = None
     postings: list[PostingTemplate] | None = None
 
 
+class Amount(ImportBaseModel):
+    number: str
+    currency: str
+
+
 class GeneratedPosting(ImportBaseModel):
-    # account of the posting
     account: str
-    # amount of the posting
-    amount: str | None = None
-    # currency of the posting
-    currency: str | None = None
-    # TODO: support cost / price and etc
+    amount: Amount | None = None
+    price: Amount | None = None
+    cost: str | None = None
 
 
 class GeneratedTransaction(ImportBaseModel):
     file: str
     # the import-id for de-duplication
     id: str
     date: str
```

### Comparing `beanhub_import-0.0.3/beanhub_import/post_processor.py` & `beanhub_import-0.0.4/beanhub_import/post_processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -93,15 +93,24 @@
     entries, _ = collect_entries(tree)
     if len(entries) != 1:
         raise ValueError("Expected exactly only one entry")
     return entries[0]
 
 
 def posting_to_text(posting: GeneratedPosting) -> str:
-    return (" " * 2) + " ".join([posting.account, posting.amount, posting.currency])
+    columns = [
+        posting.account,
+    ]
+    if posting.amount is not None:
+        columns.append(f"{posting.amount.number} {posting.amount.currency}")
+    if posting.cost is not None:
+        columns.append(posting.cost)
+    if posting.price is not None:
+        columns.append(f"@ {posting.price.number} {posting.price.currency}")
+    return (" " * 2) + " ".join(columns)
 
 
 def txn_to_text(
     txn: GeneratedTransaction, import_id_key: str = constants.IMPORT_ID_KEY
 ) -> str:
     columns = [
         txn.date,
```

### Comparing `beanhub_import-0.0.3/beanhub_import/processor.py` & `beanhub_import-0.0.4/beanhub_import/processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from beanhub_extract.data_types import Transaction
 from beanhub_extract.extractors import ALL_EXTRACTORS
 from beanhub_extract.utils import strip_txn_base_path
 from jinja2.sandbox import SandboxedEnvironment
 
 from .data_types import ActionType
+from .data_types import Amount
 from .data_types import GeneratedPosting
 from .data_types import GeneratedTransaction
 from .data_types import ImportDoc
 from .data_types import ImportRule
 from .data_types import InputConfigDetails
 from .data_types import PostingTemplate
 from .data_types import SimpleFileMatch
@@ -27,15 +28,15 @@
 from .data_types import StrSuffixMatch
 
 
 DEFAULT_TXN_TEMPLATE = dict(
     id="{{ file }}:{{ lineno }}",
     date="{{ date }}",
     flag="*",
-    narration="{{ desc | default(bank_desc) }}",
+    narration="{{ desc | default(bank_desc, true) }}",
 )
 
 
 def walk_dir_files(
     target_dir: pathlib.Path,
 ) -> typing.Generator[pathlib.Path, None, None]:
     for root, dirs, files in os.walk(target_dir):
@@ -131,19 +132,35 @@
             elif default_txn is not None and default_txn.postings is not None:
                 posting_templates.extend(default_txn.postings)
             if input_config.appending_postings is not None:
                 posting_templates.extend(input_config.appending_postings)
 
             generated_postings = []
             for posting_template in posting_templates:
+                amount = None
+                if posting_template.amount is not None:
+                    amount = Amount(
+                        number=render_str(posting_template.amount.number),
+                        currency=render_str(posting_template.amount.currency),
+                    )
+                price = None
+                if posting_template.price is not None:
+                    price = Amount(
+                        number=render_str(posting_template.price.number),
+                        currency=render_str(posting_template.price.currency),
+                    )
+                cost = None
+                if posting_template.cost is not None:
+                    cost = render_str(posting_template.cost)
                 generated_postings.append(
                     GeneratedPosting(
                         account=render_str(posting_template.account),
-                        amount=render_str(posting_template.amount),
-                        currency=render_str(posting_template.currency),
+                        amount=amount,
+                        price=price,
+                        cost=cost,
                     )
                 )
 
             yield GeneratedTransaction(
                 file=render_str(action.file),
                 postings=generated_postings,
                 **{key: render_str(value) for key, value in template_values.items()},
```

### Comparing `beanhub_import-0.0.3/pyproject.toml` & `beanhub_import-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beanhub-import"
-version = "0.0.3"
+version = "0.0.4"
 description = "The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `beanhub_import-0.0.3/PKG-INFO` & `beanhub_import-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanhub-import
-Version: 0.0.3
+Version: 0.0.4
 Summary: The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

