# Comparing `tmp/smb_sync-0.0.4.tar.gz` & `tmp/smb_sync-0.0.5.tar.gz`

## Comparing `smb_sync-0.0.4.tar` & `smb_sync-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smb_sync-0.0.4/smb_sync/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 smb_sync-0.0.4/smb_sync/__main__.py
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 smb_sync-0.0.4/smb_sync/cli.py
--rw-r--r--   0        0        0     6755 2020-02-02 00:00:00.000000 smb_sync-0.0.4/smb_sync/file_base.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 smb_sync-0.0.4/smb_sync/file_factory.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 smb_sync-0.0.4/smb_sync/file_local.py
--rw-r--r--   0        0        0     5222 2020-02-02 00:00:00.000000 smb_sync-0.0.4/smb_sync/file_samba.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 smb_sync-0.0.4/.gitignore
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 smb_sync-0.0.4/README.md
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 smb_sync-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 smb_sync-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smb_sync-0.0.5/smb_sync/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 smb_sync-0.0.5/smb_sync/__main__.py
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 smb_sync-0.0.5/smb_sync/cli.py
+-rw-r--r--   0        0        0     6755 2020-02-02 00:00:00.000000 smb_sync-0.0.5/smb_sync/file_base.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 smb_sync-0.0.5/smb_sync/file_factory.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 smb_sync-0.0.5/smb_sync/file_local.py
+-rw-r--r--   0        0        0     5222 2020-02-02 00:00:00.000000 smb_sync-0.0.5/smb_sync/file_samba.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 smb_sync-0.0.5/.gitignore
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 smb_sync-0.0.5/README.md
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 smb_sync-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 smb_sync-0.0.5/PKG-INFO
```

### Comparing `smb_sync-0.0.4/smb_sync/cli.py` & `smb_sync-0.0.5/smb_sync/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 smb_sync.cli
 """
 
 import logging
 import sys
 
+from importlib import metadata
+from importlib.metadata import PackageNotFoundError
 from argparse import ArgumentParser, BooleanOptionalAction
 from smb_sync.file_base import FileSyncOptions
 from smb_sync.file_factory import create_file_context_manager
 
 
 def setup_logger():
     """
@@ -29,14 +31,24 @@
     # Set the logging level for the root logger (DEBUG, INFO, WARNING, ERROR, CRITICAL)
     logging.basicConfig(level=logging.INFO, handlers=[console_handler])
 
     # Only show error logs from pysmb.
     logging.getLogger("SMB.SMBConnection").setLevel(logging.ERROR)
 
 
+def current_version() -> str:
+    """
+    Returns the current version of smb-sync
+    """
+    try:
+        return metadata.version("smb-sync")
+    except PackageNotFoundError:
+        return "unknown"
+
+
 def arg_parser():
     """
     Build argument parser.
     """
     parser = ArgumentParser(
         prog="smb-sync",
         description="A tool for copying files between local drive and smb network drive",
@@ -48,14 +60,20 @@
     parser.add_argument(
         "--auto-delete",
         action=BooleanOptionalAction,
         help="automatically delete extraneous files from target directories",
         default=False,
     )
 
+    parser.add_argument(
+        "--version",
+        action="version",
+        version=f"%(prog)s {current_version()}",
+    )
+
     return parser
 
 
 def main():
     """
     Main.
     """
```

### Comparing `smb_sync-0.0.4/smb_sync/file_base.py` & `smb_sync-0.0.5/smb_sync/file_base.py`

 * *Files identical despite different names*

### Comparing `smb_sync-0.0.4/smb_sync/file_factory.py` & `smb_sync-0.0.5/smb_sync/file_factory.py`

 * *Files identical despite different names*

### Comparing `smb_sync-0.0.4/smb_sync/file_local.py` & `smb_sync-0.0.5/smb_sync/file_local.py`

 * *Files identical despite different names*

### Comparing `smb_sync-0.0.4/smb_sync/file_samba.py` & `smb_sync-0.0.5/smb_sync/file_samba.py`

 * *Files identical despite different names*

