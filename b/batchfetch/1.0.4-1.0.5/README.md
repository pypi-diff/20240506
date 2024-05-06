# Comparing `tmp/batchfetch-1.0.4.tar.gz` & `tmp/batchfetch-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchfetch-1.0.4.tar", last modified: Thu May  2 19:46:26 2024, max compression
+gzip compressed data, was "batchfetch-1.0.5.tar", last modified: Sun May  5 03:00:45 2024, max compression
```

## Comparing `batchfetch-1.0.4.tar` & `batchfetch-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,19 @@
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 19:46:26.056102 batchfetch-1.0.4/
--rw-r--r--   0 dev        (455) work      (1000)     2034 2024-05-02 12:24:09.000000 batchfetch-1.0.4/.gitignore
--rw-r--r--   0 dev        (455) work      (1000)    35149 2024-05-02 12:24:09.000000 batchfetch-1.0.4/LICENSE
--rw-r--r--   0 dev        (455) work      (1000)     4483 2024-05-02 19:46:26.056102 batchfetch-1.0.4/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)     3610 2024-05-02 18:37:55.000000 batchfetch-1.0.4/README.md
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 19:46:26.056102 batchfetch-1.0.4/batchfetch/
--rw-r--r--   0 dev        (455) work      (1000)      883 2024-05-02 12:24:09.000000 batchfetch-1.0.4/batchfetch/__init__.py
--rw-r--r--   0 dev        (455) work      (1000)     5519 2024-05-02 19:37:42.000000 batchfetch-1.0.4/batchfetch/batchfetch_base.py
--rw-r--r--   0 dev        (455) work      (1000)     8662 2024-05-02 18:39:20.000000 batchfetch-1.0.4/batchfetch/batchfetch_cli.py
--rw-r--r--   0 dev        (455) work      (1000)    12549 2024-05-02 19:43:31.000000 batchfetch-1.0.4/batchfetch/batchfetch_git.py
--rw-r--r--   0 dev        (455) work      (1000)     4081 2024-05-02 12:24:09.000000 batchfetch-1.0.4/batchfetch/helpers.py
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 19:46:26.056102 batchfetch-1.0.4/batchfetch.egg-info/
--rw-r--r--   0 dev        (455) work      (1000)     4483 2024-05-02 19:46:25.000000 batchfetch-1.0.4/batchfetch.egg-info/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)      468 2024-05-02 19:46:26.000000 batchfetch-1.0.4/batchfetch.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (455) work      (1000)        1 2024-05-02 19:46:25.000000 batchfetch-1.0.4/batchfetch.egg-info/dependency_links.txt
--rw-r--r--   0 dev        (455) work      (1000)       74 2024-05-02 19:46:25.000000 batchfetch-1.0.4/batchfetch.egg-info/entry_points.txt
--rw-r--r--   0 dev        (455) work      (1000)       36 2024-05-02 19:46:25.000000 batchfetch-1.0.4/batchfetch.egg-info/requires.txt
--rw-r--r--   0 dev        (455) work      (1000)       11 2024-05-02 19:46:25.000000 batchfetch-1.0.4/batchfetch.egg-info/top_level.txt
--rwxr-xr-x   0 dev        (455) work      (1000)      916 2024-05-02 12:24:09.000000 batchfetch-1.0.4/run_tests.sh
--rw-r--r--   0 dev        (455) work      (1000)       38 2024-05-02 19:46:26.056102 batchfetch-1.0.4/setup.cfg
--rwxr-xr-x   0 dev        (455) work      (1000)     2023 2024-05-02 19:45:27.000000 batchfetch-1.0.4/setup.py
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 19:46:26.056102 batchfetch-1.0.4/tests/
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 19:46:26.056102 batchfetch-1.0.4/tests/data/
--rw-r--r--   0 dev        (455) work      (1000)       24 2024-05-02 12:24:09.000000 batchfetch-1.0.4/tests/data/test-md5sum.txt
--rwxr-xr-x   0 dev        (455) work      (1000)      117 2024-05-02 12:24:09.000000 batchfetch-1.0.4/tests/data/test-run_simple.sh
--rw-r--r--   0 dev        (455) work      (1000)     1870 2024-05-02 12:24:09.000000 batchfetch-1.0.4/tests/test_helpers.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-05 03:00:45.975829 batchfetch-1.0.5/
+-rw-r--r--   0 dev        (455) work      (1000)    35149 2024-05-05 02:57:20.000000 batchfetch-1.0.5/LICENSE
+-rw-r--r--   0 dev        (455) work      (1000)     4367 2024-05-05 03:00:45.975829 batchfetch-1.0.5/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)     3590 2024-05-05 02:57:20.000000 batchfetch-1.0.5/README.md
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-05 03:00:45.975829 batchfetch-1.0.5/batchfetch/
+-rw-r--r--   0 dev        (455) work      (1000)      774 2024-05-05 02:57:20.000000 batchfetch-1.0.5/batchfetch/__init__.py
+-rw-r--r--   0 dev        (455) work      (1000)     5419 2024-05-05 02:57:20.000000 batchfetch-1.0.5/batchfetch/batchfetch_base.py
+-rw-r--r--   0 dev        (455) work      (1000)     9045 2024-05-05 02:57:20.000000 batchfetch-1.0.5/batchfetch/batchfetch_cli.py
+-rw-r--r--   0 dev        (455) work      (1000)    13029 2024-05-05 02:57:20.000000 batchfetch-1.0.5/batchfetch/batchfetch_git.py
+-rw-r--r--   0 dev        (455) work      (1000)     4081 2024-05-05 02:57:20.000000 batchfetch-1.0.5/batchfetch/helpers.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-05 03:00:45.975829 batchfetch-1.0.5/batchfetch.egg-info/
+-rw-r--r--   0 dev        (455) work      (1000)     4367 2024-05-05 03:00:45.000000 batchfetch-1.0.5/batchfetch.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)      365 2024-05-05 03:00:45.000000 batchfetch-1.0.5/batchfetch.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (455) work      (1000)        1 2024-05-05 03:00:45.000000 batchfetch-1.0.5/batchfetch.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (455) work      (1000)       80 2024-05-05 03:00:45.000000 batchfetch-1.0.5/batchfetch.egg-info/entry_points.txt
+-rw-r--r--   0 dev        (455) work      (1000)       36 2024-05-05 03:00:45.000000 batchfetch-1.0.5/batchfetch.egg-info/requires.txt
+-rw-r--r--   0 dev        (455) work      (1000)       11 2024-05-05 03:00:45.000000 batchfetch-1.0.5/batchfetch.egg-info/top_level.txt
+-rw-r--r--   0 dev        (455) work      (1000)       38 2024-05-05 03:00:45.975829 batchfetch-1.0.5/setup.cfg
+-rwxr-xr-x   0 dev        (455) work      (1000)     2029 2024-05-05 02:57:20.000000 batchfetch-1.0.5/setup.py
```

### Comparing `batchfetch-1.0.4/LICENSE` & `batchfetch-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.4/PKG-INFO` & `batchfetch-1.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchfetch
-Version: 1.0.4
+Version: 1.0.5
 Summary: Efficiently clone and pull multiple Git repositories.
 Home-page: https://github.com/jamescherti/batchfetch
 Author: James Cherti
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,18 +13,14 @@
 Classifier: Operating System :: POSIX :: Other
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: colorama
-Requires-Dist: schema
-Requires-Dist: setproctitle
-Requires-Dist: PyYAML
 
 # Batchfetch - Efficiently clone or pull multiple Git repositories in parallel
 
 ## Introduction
 
 Batchfetch is a command-line tool designed to clone, fetch, and merge multiple Git repositories simultaneously.
 
@@ -57,20 +53,20 @@
   # Clone the default branch of the general.el repository to the
   # './general.el' directory
   - git: https://github.com/noctuid/general.el
 
   # Clone the tag 1.5 of the consult repository to the './consult'
   # directory
   - git: https://github.com/minad/consult
-    branch: "1.5"
+    reference: "1.5"
 
   # Clone the s.el repository to the './another-name.el' directory
   - git: https://github.com/magnars/s.el
     path: another-name.el
-    branch: dda84d38fffdaf0c9b12837b504b402af910d01d
+    reference: dda84d38fffdaf0c9b12837b504b402af910d01d
 
   # Delete './impatient-mode'
   - git: https://github.com/skeeto/impatient-mode
     delete: true
 ```
 
 Execute the `batchfetch` command from the same directory as `batchfetch.yml` to make it clone or update the local copies of the repositories above.
@@ -82,20 +78,20 @@
 ```
 usage: batchfetch [--option] [args]
 
 Command line interface.
 
 options:
   -h, --help            show this help message and exit
-  -j JOBS, --jobs JOBS
-                        Run up to N Number of parallel git processes (Default: 5).
+  -j JOBS, --jobs JOBS  Run up to N Number of parallel processes (Default: 5).
   -v, --verbose         Enable verbose mode.
   -f BATCHFETCH_FILE, --batchfetch-file BATCHFETCH_FILE
                         Specify the batchfetch YAML file (default: './batchfetch.yaml').
 ```
+
 ## License
 
 Copyright (c) [James Cherti](https://www.jamescherti.com)
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
```

### Comparing `batchfetch-1.0.4/README.md` & `batchfetch-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,20 +33,20 @@
   # Clone the default branch of the general.el repository to the
   # './general.el' directory
   - git: https://github.com/noctuid/general.el
 
   # Clone the tag 1.5 of the consult repository to the './consult'
   # directory
   - git: https://github.com/minad/consult
-    branch: "1.5"
+    reference: "1.5"
 
   # Clone the s.el repository to the './another-name.el' directory
   - git: https://github.com/magnars/s.el
     path: another-name.el
-    branch: dda84d38fffdaf0c9b12837b504b402af910d01d
+    reference: dda84d38fffdaf0c9b12837b504b402af910d01d
 
   # Delete './impatient-mode'
   - git: https://github.com/skeeto/impatient-mode
     delete: true
 ```
 
 Execute the `batchfetch` command from the same directory as `batchfetch.yml` to make it clone or update the local copies of the repositories above.
@@ -58,20 +58,20 @@
 ```
 usage: batchfetch [--option] [args]
 
 Command line interface.
 
 options:
   -h, --help            show this help message and exit
-  -j JOBS, --jobs JOBS
-                        Run up to N Number of parallel git processes (Default: 5).
+  -j JOBS, --jobs JOBS  Run up to N Number of parallel processes (Default: 5).
   -v, --verbose         Enable verbose mode.
   -f BATCHFETCH_FILE, --batchfetch-file BATCHFETCH_FILE
                         Specify the batchfetch YAML file (default: './batchfetch.yaml').
 ```
+
 ## License
 
 Copyright (c) [James Cherti](https://www.jamescherti.com)
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
```

### Comparing `batchfetch-1.0.4/batchfetch/__init__.py` & `batchfetch-1.0.5/batchfetch/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,12 +12,7 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program. If not, see <https://www.gnu.org/licenses/>.
 #
 """The entry-point of batchfetch."""
-
-from .batchfetch_cli import command_line_interface
-
-if __name__ == "__main__":
-    command_line_interface()
```

### Comparing `batchfetch-1.0.4/batchfetch/batchfetch_base.py` & `batchfetch-1.0.5/batchfetch/batchfetch_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,27 +27,21 @@
 from .helpers import run_indent_str
 
 
 class BatchFetchError(Exception):
     """Exception raised by Downloader()."""
 
 
-class GitBranchDoesNotExist(Exception):
-    """Exception raised by Name()."""
-
-
 class BatchFetchBase:
     """Plugin downloader base class."""
 
-    env = os.environ.copy()
-    env["GIT_TERMINAL_PROMPT"] = "0"
-
-    indent = 4
-
     def __init__(self, data: Dict[str, Any], options: Dict[str, Any]):
+        self.indent = 4
+        self.env = os.environ.copy()
+
         # Default
         self.global_options_schema: Dict[Any, Any] = {
             Optional("pre_exec"): Or([str], str),
             Optional("post_exec"): Or([str], str),
         }
 
         self.item_schema: Dict[Any, Any] = {
```

### Comparing `batchfetch-1.0.4/batchfetch/batchfetch_cli.py` & `batchfetch-1.0.5/batchfetch/batchfetch_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,133 +20,154 @@
 import argparse
 import logging
 import os
 import subprocess
 import sys
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from pathlib import Path
-from typing import Set
+from typing import Any, Dict, Set, TypeVar
 
 import colorama
 import yaml  # type: ignore
 from colorama import Fore
 from schema import Optional, Or, Schema, SchemaError
 from setproctitle import setproctitle
 
-from .batchfetch_base import BatchFetchError
+from .batchfetch_base import BatchFetchBase, BatchFetchError
 from .batchfetch_git import BatchFetchGit
 
 
 class BatchFetchCli:
     """Command-line-interface that downloads."""
 
-    main_key = "git"
-
-    # TODO: Make this automatic
-    empty_downloader_git = BatchFetchGit(
-        data={main_key: "http://www.domain.com"},
-        options={},
-    )
-    empty_downloader_git.validate_schema()  # Gen structure
-
-    cfg_schema = {
-        Optional("options"):
-            empty_downloader_git.global_options_schema,  # type: ignore
-        # TODO: Make this added automatically
-        Optional("tasks"): [
-            Or(str, empty_downloader_git.item_schema)
-        ]
-    }
-
     def __init__(self, max_workers: int, verbose: bool = False):
         self.cfg: dict = {}
         self.folder = Path(".")
         self.managed_filenames: Set[str] = set()
         self.verbose = verbose
         self.max_workers = max_workers
         self._logger = logging.getLogger(self.__class__.__name__)
         self.dirs_relative_to_batchfetch: Set[str] = set()
 
+        self.main_key = "git"
+
+        # Plugin
+        self.batchfetch_schemas: Dict[Any, Any] = {}
+        self.batchfetch_classes: Dict[str, BatchFetchBase] = {}
+        self.cfg_schema: Dict[Any, Any] = {}
+        self._plugin_add("git", BatchFetchGit)
+
+    def _plugin_add(self, keyword: str, batchfetch_class: Any):
+        batchfetch_instance = batchfetch_class(data={},
+                                               options={})
+        batchfetch_instance.validate_schema()
+
+        self.batchfetch_schemas[keyword] = batchfetch_instance.item_schema
+        self.batchfetch_classes[keyword] = batchfetch_class
+        self.cfg_schema = {
+            Optional("options"):
+                batchfetch_instance.global_options_schema,  # type: ignore
+            Optional("tasks"): [
+                Or(*list(self.batchfetch_schemas.values()))
+            ]
+        }
+
+    def _plugin_get(self, raw_data: dict) -> str:
+        keyword_found = None
+        for keyword in self.batchfetch_classes:
+            if keyword in raw_data:
+                if keyword_found is not None:
+                    err_str = (f"The keywords {keyword} and {keyword_found} "
+                               f"are mutually exclusive. Error in: {raw_data}")
+                    raise BatchFetchError(err_str)
+                keyword_found = keyword
+
+        if not keyword_found:
+            err_str = "None of the keywords " + \
+                ", ".join(self.batchfetch_classes.keys()) + \
+                f" have been found in: {raw_data}"
+            raise BatchFetchError(err_str)
+
+        return keyword_found
+
     def load(self, path: Path):
         try:
             with open(path, "r", encoding="utf-8") as fhandler:
                 yaml_dict = yaml.load(fhandler, Loader=yaml.FullLoader)
-                self.loads(dict(yaml_dict))
+                self._loads(dict(yaml_dict))
         except OSError as err:
             raise BatchFetchError(str(err)) from err
 
-    def loads(self, data: dict):
-        schema = Schema(BatchFetchCli.cfg_schema)
+    def _loads(self, data: dict):
+        schema = Schema(self.cfg_schema)
         try:
             schema.validate(data)
         except SchemaError as err:
             print(f"Schema error: {err}.", file=sys.stderr)
             sys.exit(1)
 
         self.cfg = {
             "options": {"clone_args": []},
-            # TODO: Make this added automatically
             "tasks": [],
         }
 
         if "options" in data:
             self.cfg["options"].update(data["options"])
 
-        # TODO: Make this automatic
-        self._loads_git(data)
+        self._loads_tasks(data)
 
-    def _loads_git(self, data: dict):
+    def _loads_tasks(self, data: dict):
         if "tasks" not in data:
             return
 
         dict_local_dir = {}  # type: ignore
-        for git_repo_raw in data["tasks"]:
-            if isinstance(git_repo_raw, str):
-                git_repo_raw = {BatchFetchCli.main_key: git_repo_raw}
+        for task in data["tasks"]:
+            keyword = self._plugin_get(task)
+            batchfetch_class = self.batchfetch_classes[keyword]
 
             try:
-                plugin_downloader_git = BatchFetchGit(
-                    data=git_repo_raw,
+                batchfetch_instance = batchfetch_class(  # type: ignore
+                    data=task,
                     options=self.cfg["options"],
                 )
-                self.cfg["tasks"].append(plugin_downloader_git)
+                self.cfg["tasks"].append(batchfetch_instance)
             except SchemaError as err:
                 print(f"Schema error: {err}.", file=sys.stderr)
                 sys.exit(1)
 
-            if plugin_downloader_git["path"] in dict_local_dir:
-                err_str = ("more than one repository will be cloned " +
-                           "to the directory '" +
-                           str(plugin_downloader_git["path"]) + "' (" +
-                           str(git_repo_raw[BatchFetchCli.main_key]) + " and " +
-                           str(dict_local_dir[plugin_downloader_git["path"]]) +
+            if batchfetch_instance["path"] in dict_local_dir:
+                err_str = ("more than one repository have the " +
+                           "destination path '" +
+                           str(batchfetch_instance["path"]) + "' (" +
+                           str(task[keyword]) + " and " +
+                           str(dict_local_dir[batchfetch_instance["path"]]) +
                            ")")
                 raise BatchFetchError(err_str)
-            dict_local_dir[plugin_downloader_git["path"]] = \
-                plugin_downloader_git[BatchFetchCli.main_key]
 
-    def download(self) -> bool:
+            dict_local_dir[batchfetch_instance["path"]] = \
+                batchfetch_instance[keyword]
+
+    def run_tasks(self) -> bool:
         failed = []
         error = False
         threads = []
         num_success = 0
         self.managed_filenames = set()
 
         executor_update = ThreadPoolExecutor(max_workers=self.max_workers)
 
         try:
             self.dirs_relative_to_batchfetch = set()
 
-            # TODO: Make adding to all downloads automatic
-            all_downloads = self.cfg["tasks"]
-            for download_item in all_downloads:
-                self.dirs_relative_to_batchfetch.add(str(download_item["path"]))
-                if not download_item["delete"]:
-                    self.managed_filenames.add(download_item["path"])
-                threads.append(executor_update.submit(download_item.update))
+            all_tasks = self.cfg["tasks"]
+            for task in all_tasks:
+                self.dirs_relative_to_batchfetch.add(str(task["path"]))
+                if not task["delete"]:
+                    self.managed_filenames.add(task["path"])
+                threads.append(executor_update.submit(task.update))
 
             for future in as_completed(threads):
                 data = future.result()
                 if data["result"]["error"]:
                     print(Fore.RED, end="")
                 elif data["result"]["changed"]:
                     print(Fore.YELLOW, end="")
@@ -170,47 +191,38 @@
         except KeyboardInterrupt:
             error = True
             executor_update.shutdown(cancel_futures=True)  # type: ignore
 
         if error:
             if failed:
                 print("Failed:")
-                for git_update_result in failed:
-                    print("  - url:", git_update_result[BatchFetchCli.main_key])
-                    print("    dir:", git_update_result["path"])
+                for failed_result in failed:
+                    print("  -", failed_result["path"])
             else:
                 print("Failed.")
 
             return False
         else:
             if num_success == 0:
                 print("Already up to date.")
             elif not self.verbose:
                 print("Success.")
 
         return True
 
-    # def check_managed_directories(self):
-    #     # managed_downloads = {Path(item).resolve()
-    #     #                      for item in self.managed_filenames}
-    #     # managed_directories = {item.parent
-    #     #                        for item in managed_downloads}
-    #     # TODO Implement checker
-    #     pass
-
 
 def parse_args():
     """Parse the command line arguments."""
     desc = __doc__
     usage = "%(prog)s [--option] [args]"
     parser = argparse.ArgumentParser(description=desc, usage=usage)
 
     parser.add_argument(
         "-j", "--jobs", default="5", required=False,
-        help="Run up to N Number of parallel git processes (Default: 5).",
+        help="Run up to N Number of parallel processes (Default: 5).",
     )
 
     parser.add_argument(
         "-v", "--verbose", action="store_true", default=False,
         help="Enable verbose mode.",
     )
 
@@ -239,26 +251,24 @@
                         format="%(asctime)s %(name)s: %(message)s")
 
     colorama.init()
     setproctitle(subprocess.list2cmdline([Path(sys.argv[0]).name] +
                                          sys.argv[1:]))
 
     args = parse_args()
-    downloader_cli = BatchFetchCli(verbose=args.verbose,
+    batchfetch_cli = BatchFetchCli(verbose=args.verbose,
                                    max_workers=int(args.jobs))
 
-    downloader_cli.load(args.batchfetch_file)
+    batchfetch_cli.load(args.batchfetch_file)
     os.chdir(os.path.dirname(args.batchfetch_file))
 
     try:
-        if not downloader_cli.download():
+        if not batchfetch_cli.run_tasks():
             errno = 1
     except KeyboardInterrupt:
         print("Interrupted.", file=sys.stderr)
         errno = 1
     except BatchFetchError as err:
         print(f"Error: {err}.", file=sys.stderr)
         errno = 1
-    # else:
-    #     downloader_cli.check_managed_directories()
 
     sys.exit(errno)
```

### Comparing `batchfetch-1.0.4/batchfetch/batchfetch_git.py` & `batchfetch-1.0.5/batchfetch/batchfetch_git.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,33 +23,36 @@
 import subprocess
 import textwrap
 from pathlib import Path
 from typing import List, Union
 
 from schema import Optional
 
-from .batchfetch_base import (BatchFetchBase, BatchFetchError,
-                              GitBranchDoesNotExist)
+from .batchfetch_base import BatchFetchBase, BatchFetchError
 from .helpers import run_simple
 
 
+class GitReferenceDoesNotExist(Exception):
+    """Exception raised by Name()."""
+
+
 class BatchFetchGit(BatchFetchBase):
     """Clone or update a Git repository."""
 
-    indent_spaces = " " * BatchFetchBase.indent
-    main_key = "git"
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        self.env["GIT_TERMINAL_PROMPT"] = "0"
+        self.indent_spaces = " " * self.indent
+        self.main_key = "git"
 
         # Schema
         self.item_schema.update({
             # Local options
-            BatchFetchGit.main_key: str,
-            Optional("branch"): str,
+            self.main_key: str,
+            Optional("reference"): str,
 
             # Same as global options
             Optional("clone_args"): [str],
             Optional("git_pull"): bool,
         })
 
         self.global_options_schema.update({
@@ -59,36 +62,39 @@
         })
 
         # Data
         self.global_options_values.update({"clone_args": [],
                                            "git_pull": True})
 
         self.item_default_values.update({
-            BatchFetchGit.main_key: "",
-            "branch": "",
+            self.main_key: "",
+            "reference": "",
             "delete": False,
         })
 
         self.git_local_dir = Path(self["path"])
         self.current_branch = None
         self.current_commit_ref = None
 
     def _initialize_data(self):
         super()._initialize_data()
 
-        self.values[BatchFetchGit.main_key] = \
-            self.values[BatchFetchGit.main_key].rstrip("/")
+        self.values[self.main_key] = \
+            self.values[self.main_key].rstrip("/")
 
         if "path" not in self.values:
             self.values["path"] = \
                 posixpath.basename(
-                    self.values[BatchFetchGit.main_key])  # type: ignore
+                    self.values[self.main_key])  # type: ignore
 
     def _git_ref(self, cwd: Union[None, Path] = None) -> str:
-        """Get the commit reference of HEAD."""
+        """Get the commit reference of HEAD.
+
+        The command will fail if the branch is detached.
+        """
         cmd = "git show-ref --head --verify HEAD"
         try:
             stdout, _ = run_simple(cmd, cwd=cwd, env=self.env)
             output = stdout[0].split(" ")[0]
         except IndexError:
             return ""
         return output
@@ -108,16 +114,16 @@
         elif is_clone:
             update_type = "CLONE"
         else:
             update_type = "UPDATE"
 
         self.add_output(
             f"[GIT {update_type}] {self[self.main_key]}" +
-            (f" (branch: {self['branch']})"
-             if self["branch"] else "") + "\n"
+            (f" (Reference: {self['reference']})"
+             if self["reference"] else "") + "\n"
         )
 
         try:
             # Delete
             if self["delete"]:
                 self._repo_delete()
             # Clone
@@ -184,15 +190,15 @@
             self.set_changed(True)
 
     def _repo_clone(self):
         git_clone_args = self["clone_args"]
         git_clone_args += ["--recurse-submodules"]
 
         cmd = ["git", "clone"] + git_clone_args + \
-            [self[BatchFetchGit.main_key], str(self.git_local_dir)]
+            [self[self.main_key], str(self.git_local_dir)]
         self._run(cmd, env=self.env)
         self.set_changed(True)
 
     def _repo_reset(self):
         # Remove local changes
         cmd = ["git", "reset", "--hard", "HEAD"]
         self._run(cmd, cwd=str(self.git_local_dir), env=self.env)
@@ -200,31 +206,40 @@
     def _repo_pull(self):
         git_merge = False
 
         # Merge
         ignore_git_pull = False
         if not self["git_pull"]:
             ignore_git_pull = True
-        elif self["branch"]:
+
+        if self["reference"]:
+            ignore_git_pull = False
             # Check if the new branch exists
             try:
-                self._git_tags(self["branch"])
-            except GitBranchDoesNotExist:
+                self._git_tags(self["reference"])
+            except GitReferenceDoesNotExist:
                 pass
             else:
-                # The branch exists
-
-                # Ignore Git pull when the git reference is the same
-                commit_ref = self._git_ref(cwd=self.git_local_dir)
-                if (self.current_branch and
-                    (commit_ref == self["branch"] or
-                     self.current_branch == self["branch"])):
-                    ignore_git_pull = True
-                # Ignore Git pull if it is not a local branch
-                elif not self._git_is_local_branch(self["branch"]):
+                # The branch exists:
+                # 1. Ignore Git pull when the git reference is the same
+                # as the "branch:" key
+                try:
+                    commit_ref = self._git_ref(cwd=self.git_local_dir)
+                except subprocess.CalledProcessError:
+                    # Ignore git pull because the head is detached
+                    pass
+                else:
+                    if (self.current_branch and
+                        (commit_ref == self["reference"] or
+                         self.current_branch == self["reference"])):
+                        ignore_git_pull = True
+
+                # 2. Ignore Git pull if it is not a local branch
+                if (not ignore_git_pull and
+                        not self._git_is_local_branch(self["reference"])):
                     ignore_git_pull = True
 
         if ignore_git_pull:
             self.add_output(self.indent_spaces +
                             "# git pull ignored\n")
         else:
             cmd = ["git", "fetch", "origin"]
@@ -268,46 +283,46 @@
         stdout: List[str] = []
         try:
             stdout, _ = run_simple(
                 ["git", "rev-parse", "--verify", branch],
                 env=self.env,
                 cwd=self.git_local_dir)
         except subprocess.CalledProcessError as err:
-            raise GitBranchDoesNotExist(
-                f"The branch '{branch}' does not exist.") from err
+            raise GitReferenceDoesNotExist(
+                f"The reference '{branch}' does not exist.") from err
 
         return stdout
 
     def _repo_fix_branch(self) -> bool:
         git_ref_after_merge = self._git_ref(cwd=self.git_local_dir)
         branch_changed = False
-        if self["branch"]:
+        if self["reference"]:
             # We also need tags because sometimes, a branch
             # returns a different commit reference
             git_tags, _ = run_simple(
                 ["git", "tag", "--points-at", "HEAD"],
                 env=self.env,
                 cwd=self.git_local_dir,
             )
 
             # Also check the commit reference in case
             # branch is a commit reference instead of a tag
             try:
-                git_ref_branch = self._git_tags(self["branch"])[0]
-            except GitBranchDoesNotExist as err:
+                git_ref_branch = self._git_tags(self["reference"])[0]
+            except GitReferenceDoesNotExist as err:
                 raise BatchFetchError(f"The branch '{self['branch']}' "
                                       "does not exist.") from err
 
             if git_ref_after_merge != git_ref_branch and \
-                    self["branch"] not in git_tags:
+                    self["reference"] not in git_tags:
                 # Update the branch
-                self._run(["git", "checkout"] + [self["branch"]],
+                self._run(["git", "checkout"] + [self["reference"]],
                           cwd=str(self.git_local_dir), env=self.env)
                 self.add_output(self.indent_spaces + "# Branch changed to " +
-                                self["branch"] + "\n")
+                                self["reference"] + "\n")
                 self.set_changed(True)
                 branch_changed = True
 
                 # Read branch again
                 self._update_current_branch()
 
         return branch_changed
@@ -335,15 +350,15 @@
             stdout, _ = run_simple(cmd,
                                    env=self.env,
                                    cwd=self.git_local_dir)
             origin_url = stdout[0]
         except IndexError:
             origin_url = ""
 
-        if origin_url != self[BatchFetchGit.main_key]:
+        if origin_url != self[self.main_key]:
             self.set_error(True)
             self.add_output(
                 self.indent_spaces +
                 "[ERROR] The Git remote origin URL is incorrect: "
                 f"'{origin_url}' (It is supposed to "
                 f"be '{self[self.main_key]}')\n")
             raise BatchFetchError
```

### Comparing `batchfetch-1.0.4/batchfetch/helpers.py` & `batchfetch-1.0.5/batchfetch/helpers.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.4/batchfetch.egg-info/PKG-INFO` & `batchfetch-1.0.5/batchfetch.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchfetch
-Version: 1.0.4
+Version: 1.0.5
 Summary: Efficiently clone and pull multiple Git repositories.
 Home-page: https://github.com/jamescherti/batchfetch
 Author: James Cherti
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,18 +13,14 @@
 Classifier: Operating System :: POSIX :: Other
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: colorama
-Requires-Dist: schema
-Requires-Dist: setproctitle
-Requires-Dist: PyYAML
 
 # Batchfetch - Efficiently clone or pull multiple Git repositories in parallel
 
 ## Introduction
 
 Batchfetch is a command-line tool designed to clone, fetch, and merge multiple Git repositories simultaneously.
 
@@ -57,20 +53,20 @@
   # Clone the default branch of the general.el repository to the
   # './general.el' directory
   - git: https://github.com/noctuid/general.el
 
   # Clone the tag 1.5 of the consult repository to the './consult'
   # directory
   - git: https://github.com/minad/consult
-    branch: "1.5"
+    reference: "1.5"
 
   # Clone the s.el repository to the './another-name.el' directory
   - git: https://github.com/magnars/s.el
     path: another-name.el
-    branch: dda84d38fffdaf0c9b12837b504b402af910d01d
+    reference: dda84d38fffdaf0c9b12837b504b402af910d01d
 
   # Delete './impatient-mode'
   - git: https://github.com/skeeto/impatient-mode
     delete: true
 ```
 
 Execute the `batchfetch` command from the same directory as `batchfetch.yml` to make it clone or update the local copies of the repositories above.
@@ -82,20 +78,20 @@
 ```
 usage: batchfetch [--option] [args]
 
 Command line interface.
 
 options:
   -h, --help            show this help message and exit
-  -j JOBS, --jobs JOBS
-                        Run up to N Number of parallel git processes (Default: 5).
+  -j JOBS, --jobs JOBS  Run up to N Number of parallel processes (Default: 5).
   -v, --verbose         Enable verbose mode.
   -f BATCHFETCH_FILE, --batchfetch-file BATCHFETCH_FILE
                         Specify the batchfetch YAML file (default: './batchfetch.yaml').
 ```
+
 ## License
 
 Copyright (c) [James Cherti](https://www.jamescherti.com)
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
```

### Comparing `batchfetch-1.0.4/setup.py` & `batchfetch-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 setup(
     name="batchfetch",
-    version="1.0.4",
+    version="1.0.5",
     packages=find_packages(),
     description="Efficiently clone and pull multiple Git repositories.",
     license="GPLv3",
     long_description=((Path(__file__).parent.resolve().joinpath("README.md"))
                       .read_text(encoding="utf-8")),
     long_description_content_type="text/markdown",
     url="https://github.com/jamescherti/batchfetch",
@@ -47,11 +47,11 @@
         "Operating System :: POSIX :: Other",
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Version Control :: Git",
         "Topic :: Utilities",
     ],
     entry_points={
         "console_scripts": [
-            "batchfetch=batchfetch.__init__:command_line_interface",
+            "batchfetch=batchfetch.batchfetch_cli:command_line_interface",
         ],
     },
 )
```

