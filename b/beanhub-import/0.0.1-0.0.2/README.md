# Comparing `tmp/beanhub_import-0.0.1.tar.gz` & `tmp/beanhub_import-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_import-0.0.1.tar", max compression
+gzip compressed data, was "beanhub_import-0.0.2.tar", max compression
```

## Comparing `beanhub_import-0.0.1.tar` & `beanhub_import-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-05 03:38:56.394768 beanhub_import-0.0.1/LICENSE
--rw-r--r--   0        0        0      174 2024-05-05 03:38:56.394768 beanhub_import-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-05 03:41:06.535516 beanhub_import-0.0.1/beanhub_import/__init__.py
--rw-r--r--   0        0        0       28 2024-05-06 01:50:00.122988 beanhub_import-0.0.1/beanhub_import/constants.py
--rw-r--r--   0        0        0     3530 2024-05-06 00:55:26.368702 beanhub_import-0.0.1/beanhub_import/data_types.py
--rw-r--r--   0        0        0     6409 2024-05-06 01:54:22.477776 beanhub_import-0.0.1/beanhub_import/post_processor.py
--rw-r--r--   0        0        0     7245 2024-05-05 19:21:09.441474 beanhub_import-0.0.1/beanhub_import/processor.py
--rw-r--r--   0        0        0      752 2024-05-05 21:50:05.615921 beanhub_import-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1148 1970-01-01 00:00:00.000000 beanhub_import-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-06 02:11:53.115597 beanhub_import-0.0.2/LICENSE
+-rw-r--r--   0        0        0      174 2024-05-06 02:11:53.115597 beanhub_import-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 02:11:53.115597 beanhub_import-0.0.2/beanhub_import/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-06 02:11:53.115597 beanhub_import-0.0.2/beanhub_import/constants.py
+-rw-r--r--   0        0        0     3530 2024-05-06 02:11:53.115597 beanhub_import-0.0.2/beanhub_import/data_types.py
+-rw-r--r--   0        0        0     6235 2024-05-06 02:11:53.115597 beanhub_import-0.0.2/beanhub_import/post_processor.py
+-rw-r--r--   0        0        0     7245 2024-05-06 02:11:53.115597 beanhub_import-0.0.2/beanhub_import/processor.py
+-rw-r--r--   0        0        0      725 2024-05-06 02:11:53.115597 beanhub_import-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.0.2/PKG-INFO
```

### Comparing `beanhub_import-0.0.1/LICENSE` & `beanhub_import-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.0.1/beanhub_import/data_types.py` & `beanhub_import-0.0.2/beanhub_import/data_types.py`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.0.1/beanhub_import/post_processor.py` & `beanhub_import-0.0.2/beanhub_import/post_processor.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-import collections
-import copy
-import itertools
-import json
-import pathlib
-import typing
-
-from beancount_parser.data_types import Entry
-from beancount_parser.data_types import EntryType
-from beancount_parser.helpers import collect_entries
-from beancount_parser.parser import make_parser
-from beancount_parser.parser import traverse
-from lark import Lark
-from lark import Tree
-
-from . import constants
-from .data_types import ChangeSet
-from .data_types import GeneratedPosting
-from .data_types import GeneratedTransaction
-from .data_types import ImportedTransaction
-
-
-def extract_imported_transactions(
-    parser: Lark, bean_file: pathlib.Path, import_id_key: str = constants.IMPORT_ID_KEY
-) -> typing.Generator[ImportedTransaction, None, None]:
-    last_txn = None
-    for bean_path, tree in traverse(parser=parser, bean_file=bean_file):
-        if tree.data != "start":
-            raise ValueError("Expected start")
-        for child in tree.children:
-            if child is None:
-                continue
-            if child.data != "statement":
-                raise ValueError("Expected statement")
-            first_child = child.children[0]
-            if not isinstance(first_child, Tree):
-                continue
-            if first_child.data == "date_directive":
-                date_directive = first_child.children[0]
-                directive_type = date_directive.data.value
-                if directive_type != "txn":
-                    continue
-                last_txn = date_directive
-            elif first_child.data == "metadata_item":
-                metadata_key = first_child.children[0].value
-                metadata_value = json.loads(first_child.children[1].value)
-                if metadata_key == import_id_key:
-                    yield ImportedTransaction(
-                        file=bean_path, lineno=last_txn.meta.line, id=metadata_value
-                    )
-
-
-def compute_changes(
-    generated_txns: list[GeneratedTransaction], imported_txns: list[ImportedTransaction]
-) -> dict[pathlib.Path, ChangeSet]:
-    generated_id_txns = {txn.id: txn for txn in generated_txns}
-    imported_id_txns = {txn.id: txn for txn in imported_txns}
-
-    to_remove = collections.defaultdict(list)
-    for txn in imported_txns:
-        generated_txn = generated_id_txns.get(txn.id)
-        if generated_txn is not None and txn.file != pathlib.Path(generated_txn.file):
-            # it appears that the generated txn's file is different from the old one, let's remove it
-            to_remove[txn.file].append(txn)
-
-    to_add = collections.defaultdict(list)
-    to_update = collections.defaultdict(dict)
-    for txn in generated_txns:
-        imported_txn = imported_id_txns.get(txn.id)
-        generated_file = pathlib.Path(txn.file)
-        if imported_txn is not None and imported_txn.file == generated_file:
-            to_update[generated_file][imported_txn.lineno] = txn
-        else:
-            to_add[generated_file].append(txn)
-
-    all_files = frozenset(to_remove.keys()).union(to_add.keys()).union(to_update.keys())
-    return {
-        file_path: ChangeSet(
-            remove=to_remove[file_path],
-            add=to_add[file_path],
-            update=to_update[file_path],
-        )
-        for file_path in all_files
-    }
-
-
-def to_parser_entry(parser: Lark, text: str) -> Entry:
-    tree = parser.parse(text.strip())
-    entries, _ = collect_entries(tree)
-    if len(entries) != 1:
-        raise ValueError("Expected exactly only one entry")
-    return entries[0]
-
-
-def posting_to_text(posting: GeneratedPosting) -> str:
-    return (" " * 2) + " ".join([posting.account, posting.amount, posting.currency])
-
-
-def txn_to_text(
-    txn: GeneratedTransaction, import_id_key: str = constants.IMPORT_ID_KEY
-) -> str:
-    columns = [
-        txn.date,
-        txn.flag,
-        *((json.dumps(txn.payee),) if txn.payee is not None else ()),
-        json.dumps(txn.narration),
-    ]
-    line = " ".join(columns)
-    return "\n".join(
-        [
-            line,
-            f"  {import_id_key}: {json.dumps(txn.id)}",
-            *(map(posting_to_text, txn.postings)),
-        ]
-    )
-
-
-def apply_change_set(
-    tree: Lark, change_set: ChangeSet, import_id_key: str = constants.IMPORT_ID_KEY
-) -> Lark:
-    if tree.data != "start":
-        raise ValueError("expected start as the root rule")
-    parser = make_parser()
-
-    lines_to_remove = [txn.lineno for txn in change_set.remove]
-    line_to_entries = {
-        lineno: to_parser_entry(parser, txn_to_text(txn))
-        for lineno, txn in change_set.update.items()
-    }
-    entries_to_add = [
-        to_parser_entry(parser, txn_to_text(txn, import_id_key=import_id_key))
-        for txn in change_set.add
-    ]
-
-    new_tree = copy.deepcopy(tree)
-    entries, tail_comments = collect_entries(new_tree)
-
-    tailing_comments_entry: typing.Optional[Entry] = None
-    if tail_comments:
-        tailing_comments_entry = Entry(
-            type=EntryType.COMMENTS,
-            comments=tail_comments,
-            statement=None,
-            metadata=[],
-            postings=[],
-        )
-
-    new_children = []
-    for entry in itertools.chain(entries, entries_to_add):
-        if entry.type == EntryType.COMMENTS:
-            new_children.extend(entry.comments)
-            continue
-        if entry.statement.meta.line in lines_to_remove:
-            # We also drop the comments
-            continue
-        actual_entry = line_to_entries.get(entry.statement.meta.line, entry)
-        # use comments from existing entry regardless
-        new_children.extend(entry.comments)
-        new_children.append(actual_entry.statement)
-        for metadata in actual_entry.metadata:
-            new_children.extend(metadata.comments)
-            new_children.append(metadata.statement)
-        for posting in actual_entry.postings:
-            new_children.extend(posting.comments)
-            new_children.append(posting.statement)
-            for metadata in posting.metadata:
-                new_children.extend(metadata.comments)
-                new_children.append(metadata.statement)
-
-    if tailing_comments_entry is not None:
-        new_children.extend(tailing_comments_entry.comments)
-
-    new_tree.children = new_children
-    return new_tree
+import collections
+import copy
+import itertools
+import json
+import pathlib
+import typing
+
+from beancount_parser.data_types import Entry
+from beancount_parser.data_types import EntryType
+from beancount_parser.helpers import collect_entries
+from beancount_parser.parser import make_parser
+from beancount_parser.parser import traverse
+from lark import Lark
+from lark import Tree
+
+from . import constants
+from .data_types import ChangeSet
+from .data_types import GeneratedPosting
+from .data_types import GeneratedTransaction
+from .data_types import ImportedTransaction
+
+
+def extract_imported_transactions(
+    parser: Lark, bean_file: pathlib.Path, import_id_key: str = constants.IMPORT_ID_KEY
+) -> typing.Generator[ImportedTransaction, None, None]:
+    last_txn = None
+    for bean_path, tree in traverse(parser=parser, bean_file=bean_file):
+        if tree.data != "start":
+            raise ValueError("Expected start")
+        for child in tree.children:
+            if child is None:
+                continue
+            if child.data != "statement":
+                raise ValueError("Expected statement")
+            first_child = child.children[0]
+            if not isinstance(first_child, Tree):
+                continue
+            if first_child.data == "date_directive":
+                date_directive = first_child.children[0]
+                directive_type = date_directive.data.value
+                if directive_type != "txn":
+                    continue
+                last_txn = date_directive
+            elif first_child.data == "metadata_item":
+                metadata_key = first_child.children[0].value
+                metadata_value = json.loads(first_child.children[1].value)
+                if metadata_key == import_id_key:
+                    yield ImportedTransaction(
+                        file=bean_path, lineno=last_txn.meta.line, id=metadata_value
+                    )
+
+
+def compute_changes(
+    generated_txns: list[GeneratedTransaction], imported_txns: list[ImportedTransaction]
+) -> dict[pathlib.Path, ChangeSet]:
+    generated_id_txns = {txn.id: txn for txn in generated_txns}
+    imported_id_txns = {txn.id: txn for txn in imported_txns}
+
+    to_remove = collections.defaultdict(list)
+    for txn in imported_txns:
+        generated_txn = generated_id_txns.get(txn.id)
+        if generated_txn is not None and txn.file != pathlib.Path(generated_txn.file):
+            # it appears that the generated txn's file is different from the old one, let's remove it
+            to_remove[txn.file].append(txn)
+
+    to_add = collections.defaultdict(list)
+    to_update = collections.defaultdict(dict)
+    for txn in generated_txns:
+        imported_txn = imported_id_txns.get(txn.id)
+        generated_file = pathlib.Path(txn.file)
+        if imported_txn is not None and imported_txn.file == generated_file:
+            to_update[generated_file][imported_txn.lineno] = txn
+        else:
+            to_add[generated_file].append(txn)
+
+    all_files = frozenset(to_remove.keys()).union(to_add.keys()).union(to_update.keys())
+    return {
+        file_path: ChangeSet(
+            remove=to_remove[file_path],
+            add=to_add[file_path],
+            update=to_update[file_path],
+        )
+        for file_path in all_files
+    }
+
+
+def to_parser_entry(parser: Lark, text: str) -> Entry:
+    tree = parser.parse(text.strip())
+    entries, _ = collect_entries(tree)
+    if len(entries) != 1:
+        raise ValueError("Expected exactly only one entry")
+    return entries[0]
+
+
+def posting_to_text(posting: GeneratedPosting) -> str:
+    return (" " * 2) + " ".join([posting.account, posting.amount, posting.currency])
+
+
+def txn_to_text(
+    txn: GeneratedTransaction, import_id_key: str = constants.IMPORT_ID_KEY
+) -> str:
+    columns = [
+        txn.date,
+        txn.flag,
+        *((json.dumps(txn.payee),) if txn.payee is not None else ()),
+        json.dumps(txn.narration),
+    ]
+    line = " ".join(columns)
+    return "\n".join(
+        [
+            line,
+            f"  {import_id_key}: {json.dumps(txn.id)}",
+            *(map(posting_to_text, txn.postings)),
+        ]
+    )
+
+
+def apply_change_set(
+    tree: Lark, change_set: ChangeSet, import_id_key: str = constants.IMPORT_ID_KEY
+) -> Lark:
+    if tree.data != "start":
+        raise ValueError("expected start as the root rule")
+    parser = make_parser()
+
+    lines_to_remove = [txn.lineno for txn in change_set.remove]
+    line_to_entries = {
+        lineno: to_parser_entry(parser, txn_to_text(txn))
+        for lineno, txn in change_set.update.items()
+    }
+    entries_to_add = [
+        to_parser_entry(parser, txn_to_text(txn, import_id_key=import_id_key))
+        for txn in change_set.add
+    ]
+
+    new_tree = copy.deepcopy(tree)
+    entries, tail_comments = collect_entries(new_tree)
+
+    tailing_comments_entry: typing.Optional[Entry] = None
+    if tail_comments:
+        tailing_comments_entry = Entry(
+            type=EntryType.COMMENTS,
+            comments=tail_comments,
+            statement=None,
+            metadata=[],
+            postings=[],
+        )
+
+    new_children = []
+    for entry in itertools.chain(entries, entries_to_add):
+        if entry.type == EntryType.COMMENTS:
+            new_children.extend(entry.comments)
+            continue
+        if entry.statement.meta.line in lines_to_remove:
+            # We also drop the comments
+            continue
+        actual_entry = line_to_entries.get(entry.statement.meta.line, entry)
+        # use comments from existing entry regardless
+        new_children.extend(entry.comments)
+        new_children.append(actual_entry.statement)
+        for metadata in actual_entry.metadata:
+            new_children.extend(metadata.comments)
+            new_children.append(metadata.statement)
+        for posting in actual_entry.postings:
+            new_children.extend(posting.comments)
+            new_children.append(posting.statement)
+            for metadata in posting.metadata:
+                new_children.extend(metadata.comments)
+                new_children.append(metadata.statement)
+
+    if tailing_comments_entry is not None:
+        new_children.extend(tailing_comments_entry.comments)
+
+    new_tree.children = new_children
+    return new_tree
```

### Comparing `beanhub_import-0.0.1/beanhub_import/processor.py` & `beanhub_import-0.0.2/beanhub_import/processor.py`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.0.1/pyproject.toml` & `beanhub_import-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-[tool.poetry]
-name = "beanhub-import"
-version = "0.0.1"
-description = "The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules"
-authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
-license = "MIT"
-readme = "README.md"
-
-[tool.poetry.dependencies]
-python = "^3.9"
-pytz = "^2024.1"
-beanhub-extract = "^0.0.5"
-pydantic = "^2.7.1"
-pyyaml = "^6.0.1"
-jinja2 = "^3.1.3"
-beancount-black = "^1.0.2"
-beancount-parser = "^1.1.0"
-
-[tool.poetry.dev-dependencies]
-
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.4.1"
-pytest-mock = "^3.11.1"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "beanhub-import"
+version = "0.0.2"
+description = "The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules"
+authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
+license = "MIT"
+readme = "README.md"
+
+[tool.poetry.dependencies]
+python = "^3.9"
+pytz = "^2024.1"
+beanhub-extract = "^0.0.5"
+pydantic = "^2.7.1"
+pyyaml = "^6.0.1"
+jinja2 = "^3.1.3"
+beancount-black = "^1.0.2"
+beancount-parser = "^1.1.0"
+
+[tool.poetry.dev-dependencies]
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.1"
+pytest-mock = "^3.11.1"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `beanhub_import-0.0.1/PKG-INFO` & `beanhub_import-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: beanhub-import
-Version: 0.0.1
+Version: 0.0.2
 Summary: The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beancount-black (>=1.0.2,<2.0.0)
 Requires-Dist: beancount-parser (>=1.1.0,<2.0.0)
 Requires-Dist: beanhub-extract (>=0.0.5,<0.0.6)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
```

