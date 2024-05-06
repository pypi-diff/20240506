# Comparing `tmp/snapcat-0.1.0.tar.gz` & `tmp/snapcat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapcat-0.1.0.tar", max compression
+gzip compressed data, was "snapcat-0.1.1.tar", max compression
```

## Comparing `snapcat-0.1.0.tar` & `snapcat-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     5276 2024-05-06 06:59:08.584540 snapcat-0.1.0/README.md
--rw-r--r--   0        0        0      627 2024-05-06 06:58:10.451155 snapcat-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      796 2024-04-19 09:13:11.118805 snapcat-0.1.0/src/snapcat/__init__.py
--rw-r--r--   0        0        0     2522 2024-05-05 15:13:34.891954 snapcat-0.1.0/src/snapcat/cat_utils.py
--rw-r--r--   0        0        0     1100 2024-05-03 14:32:56.419258 snapcat-0.1.0/src/snapcat/config.py
--rw-r--r--   0        0        0     4662 2024-05-06 06:54:58.688397 snapcat-0.1.0/src/snapcat/export_cmd/__init__.py
--rw-r--r--   0        0        0     2364 2024-05-06 06:09:51.832467 snapcat-0.1.0/src/snapcat/show_cmd/__init__.py
--rw-r--r--   0        0        0     5572 2024-05-05 15:14:12.169263 snapcat-0.1.0/src/snapcat/sync_cmd/__init__.py
--rw-r--r--   0        0        0     4524 2024-05-02 07:47:28.803074 snapcat-0.1.0/src/snapcat/sync_cmd/sync.py
--rw-r--r--   0        0        0     5694 1970-01-01 00:00:00.000000 snapcat-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5394 2024-05-06 07:17:25.741501 snapcat-0.1.1/README.md
+-rw-r--r--   0        0        0      728 2024-05-06 07:13:33.957845 snapcat-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      796 2024-04-19 09:13:11.118805 snapcat-0.1.1/src/snapcat/__init__.py
+-rw-r--r--   0        0        0     2522 2024-05-05 15:13:34.891954 snapcat-0.1.1/src/snapcat/cat_utils.py
+-rw-r--r--   0        0        0     1100 2024-05-03 14:32:56.419258 snapcat-0.1.1/src/snapcat/config.py
+-rw-r--r--   0        0        0     4662 2024-05-06 06:54:58.688397 snapcat-0.1.1/src/snapcat/export_cmd/__init__.py
+-rw-r--r--   0        0        0     2364 2024-05-06 06:09:51.832467 snapcat-0.1.1/src/snapcat/show_cmd/__init__.py
+-rw-r--r--   0        0        0     5572 2024-05-05 15:14:12.169263 snapcat-0.1.1/src/snapcat/sync_cmd/__init__.py
+-rw-r--r--   0        0        0     4524 2024-05-02 07:47:28.803074 snapcat-0.1.1/src/snapcat/sync_cmd/sync.py
+-rw-r--r--   0        0        0     5913 1970-01-01 00:00:00.000000 snapcat-0.1.1/PKG-INFO
```

### Comparing `snapcat-0.1.0/README.md` & `snapcat-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # SnapCAT
 
-**snapcat** is a Python command-line tool that helps manage Chia Address Tokens (CATs). The tool communicates locally with the Chia Full Node RPC. The tool also leverages code from [chia-network](https://twitter.com/chia_project)'s [CAT-addresses](https://github.com/Chia-Network/CAT-addresses).
+**snapcat** is a Python command-line tool that helps monitor [CATs](https://docs.chia.net/guides/crash-course/cats-offers-nfts/#what-is-a-cat) (Chia Asset Tokens) on Chia Blockchain. It retrieves the latest CAT holder data by communicating with your local Chia Full Node RPC. The tool also leverages code from [chia-network](https://www.chia.net/)'s [CAT-addresses](https://github.com/Chia-Network/CAT-addresses).
 
 ```
 ❯ snapcat --help
 
  Usage: snapcat [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ──────────────────────────────────────────────────────────────────────────╮
```

### Comparing `snapcat-0.1.0/pyproject.toml` & `snapcat-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "snapcat"
-version = "0.1.0"
-description = ""
+version = "0.1.1"
+description = "snapcat is a Python command-line tool that helps monitor CATs (Chia Asset Tokens) on Chia Blockchain."
 authors = ["Dexie Contributors <pypi@dexie.space>"]
 readme = "README.md"
 packages = [{include = "snapcat", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 rich-click = "^1.8.0"
```

### Comparing `snapcat-0.1.0/src/snapcat/__init__.py` & `snapcat-0.1.1/src/snapcat/__init__.py`

 * *Files identical despite different names*

### Comparing `snapcat-0.1.0/src/snapcat/cat_utils.py` & `snapcat-0.1.1/src/snapcat/cat_utils.py`

 * *Files identical despite different names*

### Comparing `snapcat-0.1.0/src/snapcat/config.py` & `snapcat-0.1.1/src/snapcat/config.py`

 * *Files identical despite different names*

### Comparing `snapcat-0.1.0/src/snapcat/export_cmd/__init__.py` & `snapcat-0.1.1/src/snapcat/export_cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `snapcat-0.1.0/src/snapcat/show_cmd/__init__.py` & `snapcat-0.1.1/src/snapcat/show_cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `snapcat-0.1.0/src/snapcat/sync_cmd/__init__.py` & `snapcat-0.1.1/src/snapcat/sync_cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `snapcat-0.1.0/src/snapcat/sync_cmd/sync.py` & `snapcat-0.1.1/src/snapcat/sync_cmd/sync.py`

 * *Files identical despite different names*

### Comparing `snapcat-0.1.0/PKG-INFO` & `snapcat-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: snapcat
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: snapcat is a Python command-line tool that helps monitor CATs (Chia Asset Tokens) on Chia Blockchain.
 Author: Dexie Contributors
 Author-email: pypi@dexie.space
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: rich-click (>=1.8.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # SnapCAT
 
-**snapcat** is a Python command-line tool that helps manage Chia Address Tokens (CATs). The tool communicates locally with the Chia Full Node RPC. The tool also leverages code from [chia-network](https://twitter.com/chia_project)'s [CAT-addresses](https://github.com/Chia-Network/CAT-addresses).
+**snapcat** is a Python command-line tool that helps monitor [CATs](https://docs.chia.net/guides/crash-course/cats-offers-nfts/#what-is-a-cat) (Chia Asset Tokens) on Chia Blockchain. It retrieves the latest CAT holder data by communicating with your local Chia Full Node RPC. The tool also leverages code from [chia-network](https://www.chia.net/)'s [CAT-addresses](https://github.com/Chia-Network/CAT-addresses).
 
 ```
 ❯ snapcat --help
 
  Usage: snapcat [OPTIONS] COMMAND [ARGS]...
 
 ╭─ Options ──────────────────────────────────────────────────────────────────────────╮
```

