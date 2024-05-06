# Comparing `tmp/cpgdata-0.3.0.tar.gz` & `tmp/cpgdata-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpgdata-0.3.0.tar", max compression
+gzip compressed data, was "cpgdata-0.4.0.tar", max compression
```

## Comparing `cpgdata-0.3.0.tar` & `cpgdata-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      830 2024-02-21 18:47:20.849285 cpgdata-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1126 2024-02-21 18:47:20.849285 cpgdata-0.3.0/README.md
--rw-r--r--   0        0        0      132 2024-02-21 18:47:20.849285 cpgdata-0.3.0/src/cpgdata/__init__.py
--rw-r--r--   0        0        0        0 2024-02-21 18:47:20.849285 cpgdata-0.3.0/src/cpgdata/cli/__init__.py
--rw-r--r--   0        0        0     1326 2024-02-21 18:47:20.849285 cpgdata-0.3.0/src/cpgdata/cli/index.py
--rw-r--r--   0        0        0     5762 2024-02-21 18:47:20.849285 cpgdata-0.3.0/src/cpgdata/cli/inventory.py
--rw-r--r--   0        0        0      308 2024-02-21 18:47:20.849285 cpgdata-0.3.0/src/cpgdata/cli/main.py
--rw-r--r--   0        0        0     1908 2024-02-21 18:47:20.849285 cpgdata-0.3.0/src/cpgdata/cli/report.py
--rw-r--r--   0        0        0     3271 2024-02-21 18:47:20.849285 cpgdata-0.3.0/src/cpgdata/key_parser.lark
--rw-r--r--   0        0        0     2766 2024-02-21 18:47:20.849285 cpgdata-0.3.0/src/cpgdata/measurement.py
--rw-r--r--   0        0        0     7387 2024-02-21 18:47:20.849285 cpgdata-0.3.0/src/cpgdata/parser.py
--rw-r--r--   0        0        0     8223 2024-02-21 18:47:20.849285 cpgdata-0.3.0/src/cpgdata/pipe.py
--rw-r--r--   0        0        0     3547 2024-02-21 18:47:20.849285 cpgdata-0.3.0/src/cpgdata/rule.py
--rw-r--r--   0        0        0     9346 2024-02-21 18:47:20.849285 cpgdata-0.3.0/src/cpgdata/utils.py
--rw-r--r--   0        0        0     1939 1970-01-01 00:00:00.000000 cpgdata-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      813 2024-05-06 03:13:00.255952 cpgdata-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1126 2024-05-06 03:13:00.255952 cpgdata-0.4.0/README.md
+-rw-r--r--   0        0        0      132 2024-05-06 03:13:00.255952 cpgdata-0.4.0/src/cpgdata/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 03:13:00.255952 cpgdata-0.4.0/src/cpgdata/cli/__init__.py
+-rw-r--r--   0        0        0     1326 2024-05-06 03:13:00.255952 cpgdata-0.4.0/src/cpgdata/cli/index.py
+-rw-r--r--   0        0        0     5762 2024-05-06 03:13:00.255952 cpgdata-0.4.0/src/cpgdata/cli/inventory.py
+-rw-r--r--   0        0        0      308 2024-05-06 03:13:00.255952 cpgdata-0.4.0/src/cpgdata/cli/main.py
+-rw-r--r--   0        0        0     1908 2024-05-06 03:13:00.255952 cpgdata-0.4.0/src/cpgdata/cli/report.py
+-rw-r--r--   0        0        0     3271 2024-05-06 03:13:00.255952 cpgdata-0.4.0/src/cpgdata/key_parser.lark
+-rw-r--r--   0        0        0     2766 2024-05-06 03:13:00.255952 cpgdata-0.4.0/src/cpgdata/measurement.py
+-rw-r--r--   0        0        0     7387 2024-05-06 03:13:00.271581 cpgdata-0.4.0/src/cpgdata/parser.py
+-rw-r--r--   0        0        0     8223 2024-05-06 03:13:00.271581 cpgdata-0.4.0/src/cpgdata/pipe.py
+-rw-r--r--   0        0        0     3547 2024-05-06 03:13:00.271581 cpgdata-0.4.0/src/cpgdata/rule.py
+-rw-r--r--   0        0        0     9342 2024-05-06 03:13:00.271581 cpgdata-0.4.0/src/cpgdata/utils.py
+-rw-r--r--   0        0        0     1804 1970-01-01 00:00:00.000000 cpgdata-0.4.0/PKG-INFO
```

### Comparing `cpgdata-0.3.0/pyproject.toml` & `cpgdata-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "cpgdata"
-version = "0.3.0"
+version = "0.4.0"
 description = "Cell painting gallery data handling and validation"
 authors = ["Ankur Kumar <ank@leoank.me>"]
 readme = "README.md"
 packages = [{ include = "cpgdata", from = "src" }]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.10"
 click = "^8.1"
 pydantic = "^2.4"
 polars = "^0.19"
 pyarrow = "^13.0"
 joblib = "^1.3.2"
 cpgparser = "^0.2"
-cpgaws = "^2.15"
 tqdm = "^4.66"
 lark = "^1.1.9"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4"
 black = "^23.10"
```

### Comparing `cpgdata-0.3.0/README.md` & `cpgdata-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cpgdata-0.3.0/src/cpgdata/cli/index.py` & `cpgdata-0.4.0/src/cpgdata/cli/index.py`

 * *Files identical despite different names*

### Comparing `cpgdata-0.3.0/src/cpgdata/cli/inventory.py` & `cpgdata-0.4.0/src/cpgdata/cli/inventory.py`

 * *Files identical despite different names*

### Comparing `cpgdata-0.3.0/src/cpgdata/cli/report.py` & `cpgdata-0.4.0/src/cpgdata/cli/report.py`

 * *Files identical despite different names*

### Comparing `cpgdata-0.3.0/src/cpgdata/key_parser.lark` & `cpgdata-0.4.0/src/cpgdata/key_parser.lark`

 * *Files identical despite different names*

### Comparing `cpgdata-0.3.0/src/cpgdata/measurement.py` & `cpgdata-0.4.0/src/cpgdata/measurement.py`

 * *Files identical despite different names*

### Comparing `cpgdata-0.3.0/src/cpgdata/parser.py` & `cpgdata-0.4.0/src/cpgdata/parser.py`

 * *Files identical despite different names*

### Comparing `cpgdata-0.3.0/src/cpgdata/pipe.py` & `cpgdata-0.4.0/src/cpgdata/pipe.py`

 * *Files identical despite different names*

### Comparing `cpgdata-0.3.0/src/cpgdata/rule.py` & `cpgdata-0.4.0/src/cpgdata/rule.py`

 * *Files identical despite different names*

### Comparing `cpgdata-0.3.0/src/cpgdata/utils.py` & `cpgdata-0.4.0/src/cpgdata/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 This module provide utility functions shared by other modules in the package.
 """
 
 import json
 import os
 import re
+import subprocess
 from collections.abc import Sequence
 from contextlib import redirect_stdout
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Any, Callable, List, Optional
 
-from awscli.clidriver import AWSCLIEntryPoint
 from joblib import Parallel, cpu_count, delayed
 from tqdm import tqdm
 
 
 def slice_iterable(iterable: Sequence, count: int) -> List[slice]:
     """Create slices of the given iterable.
 
@@ -27,14 +27,15 @@
     count : int
         Number of slices to create.
 
     Returns
     -------
     List[slice]
         A list of slice.
+
     """
     slices = []
     if count == 0:
         slices.append(slice(0, len(iterable)))
         return slices
     if len(iterable) < count:
         raise Exception(
@@ -67,14 +68,15 @@
     timeout: float, optional
         Timeout for worker processes.
 
     Returns
     -------
     Any
         A list of outputs genetated by function.
+
     """
     jobs = jobs or cpu_count()
     if len(iterable) <= jobs:
         jobs = len(iterable)
     slices = slice_iterable(iterable, jobs)
     return Parallel(n_jobs=jobs, timeout=timeout)(
         delayed(func)(chunk, *args, idx % jobs)
@@ -85,14 +87,15 @@
 def get_package_root_path() -> Path:
     """Get path of the package root.
 
     Returns
     -------
         Path
             Package root path
+
     """
     return Path(__file__).parents[1].absolute()
 
 
 def download_s3_file(
     bucket: str, key: str, out_path: Path, no_progress: bool = True
 ) -> None:
@@ -104,25 +107,26 @@
         S3 bucket identifier.
     key : str
         S3 bucket full key.
     out_path : Path
         Path to save the object.
     no_progress: bool
         Flag to control progress bar.
+
     """
     cli_args = [
         "s3",
         "cp",
         f"s3://{bucket.rstrip('/')}/{key.lstrip('/')}",
         str(out_path.absolute()),
     ]
     if no_progress is True:
         cli_args = cli_args + ["--no-progress"]
     cli_args = cli_args + ["--no-sign-request"]
-    AWSCLIEntryPoint().main(cli_args)
+    subprocess.run(["aws"] + cli_args)
 
 
 def download_s3_files(
     key_list: List[str],
     bucket: str,
     out_path: Path,
     flatten: bool = False,
@@ -138,14 +142,15 @@
         Name of the S3 bucket.
     out_path : Path
         Path to save files.
     flatten : bool
         Save all files in single directory ignoring prefix structure.
     idx : int
         Index of the worker if available.
+
     """
     w_id = os.getpid()
     for key in tqdm(key_list, desc=f"Downloading files: Worker {w_id}", position=idx):
         if flatten is True:
             write_path = out_path.joinpath(key.split("/")[-1])
         else:
             write_path = out_path.joinpath(key)
@@ -172,14 +177,15 @@
         Path to save the object.
     include: Optional[str]
         regex pattern to include files to download.
     exclude: Optional[str]
         regex pattern to exclude files to download.
     no_progress: bool
         Flag to control display of transfer progress. Defaults to False.
+
     """
     cli_args = [
         "s3",
         "cp",
         f"s3://{bucket.rstrip('/')}/{prefix.lstrip('/')}",
         str(out_path.absolute()),
         "--recursive",
@@ -187,15 +193,15 @@
     if include is not None:
         cli_args = cli_args + ["--include", include]
     if exclude is not None:
         cli_args = cli_args + ["--exclude", exclude]
     if no_progress is True:
         cli_args = cli_args + ["--no-progress"]
     cli_args = cli_args + ["--no-sign-request"]
-    AWSCLIEntryPoint().main(cli_args)
+    subprocess.run(["aws"] + cli_args)
 
 
 def sync_s3_prefix(
     bucket: str,
     prefix: str,
     out_path: Path,
     include: Optional[str] = None,
@@ -214,29 +220,30 @@
         Path to save the object.
     include: Optional[str]
         regex pattern to include files to download.
     exclude: Optional[str]
         regex pattern to exclude files to download.
     no_progress: bool
         Flag to control display of transfer progress. Defaults to False.
+
     """
     cli_args = [
         "s3",
         "sync",
         f"s3://{bucket.rstrip('/')}/{prefix.lstrip('/')}",
         str(out_path.absolute()),
     ]
     if exclude is not None:
         cli_args = cli_args + ["--exclude", exclude]
     if include is not None:
         cli_args = cli_args + ["--include", include]
     if no_progress is True:
         cli_args = cli_args + ["--no-progress"]
     cli_args = cli_args + ["--no-sign-request"]
-    AWSCLIEntryPoint().main(cli_args)
+    subprocess.run(["aws"] + cli_args)
 
 
 BLANK_RGX = re.compile(r" +")
 
 
 def parse_ls_out(line: str) -> str:
     """Parse s3 prefix path from aws cli ls output.
@@ -246,14 +253,15 @@
     line : str
         AWS Cli ls output line.
 
     Returns
     -------
     str
         Parsed S3 prefix path
+
     """
     line = line.rstrip("\n")
     line = line.replace("//", "/")
     elems = BLANK_RGX.split(line, maxsplit=3)
     return elems[-1]
 
 
@@ -270,14 +278,15 @@
         S3 bucket identifier.
     prefix : str
         S3 bucket full prefix.
     out_path : Path
         Path to save the object.
     recursive: bool
         Flag to allow recursive listing of files. Defaults to False.
+
     """
     bucket = bucket.strip("/")
     prefix = prefix.lstrip("/")
     cli_args = [
         "s3",
         "ls",
         f"s3://{bucket}/{prefix}",
@@ -285,15 +294,15 @@
     out_list = []
     if recursive is not False:
         cli_args = cli_args + ["--recursive"]
     cli_args = cli_args + ["--no-sign-request"]
     with NamedTemporaryFile() as temp_file:
         with Path(temp_file.name).open("w") as f:
             with redirect_stdout(f):
-                AWSCLIEntryPoint().main(cli_args)
+                subprocess.run(["aws"] + cli_args)
         for line in Path(temp_file.name).open("r").readlines():
             out_list.append(f"{parse_ls_out(line)}")
     return out_list
 
 
 def sync_inventory(bucket: str, prefix: str, out_path: Path, revision: int = 0) -> None:
     """Sync inventory files of a specific revision.
@@ -304,14 +313,15 @@
         Name of the bucket.
     prefix : str
         Prefix for the revisions.
     out_path : Path
         Path to save synced files.
     revision : int
         Revision to sync. 0 is the latest revision.
+
     """
     dirs = ls_s3_prefix(bucket, prefix)
     dirs.sort()
     manifest_revision = dirs[-(abs(revision) + 3)]
     print(manifest_revision)
     sync_s3_prefix(
         bucket,
```

### Comparing `cpgdata-0.3.0/PKG-INFO` & `cpgdata-0.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: cpgdata
-Version: 0.3.0
+Version: 0.4.0
 Summary: Cell painting gallery data handling and validation
 Author: Ankur Kumar
 Author-email: ank@leoank.me
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1,<9.0)
-Requires-Dist: cpgaws (>=2.15,<3.0)
 Requires-Dist: cpgparser (>=0.2,<0.3)
 Requires-Dist: joblib (>=1.3.2,<2.0.0)
 Requires-Dist: lark (>=1.1.9,<2.0.0)
 Requires-Dist: polars (>=0.19,<0.20)
 Requires-Dist: pyarrow (>=13.0,<14.0)
 Requires-Dist: pydantic (>=2.4,<3.0)
 Requires-Dist: tqdm (>=4.66,<5.0)
```

