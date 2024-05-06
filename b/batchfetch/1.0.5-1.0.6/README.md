# Comparing `tmp/batchfetch-1.0.5.tar.gz` & `tmp/batchfetch-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchfetch-1.0.5.tar", last modified: Sun May  5 03:00:45 2024, max compression
+gzip compressed data, was "batchfetch-1.0.6.tar", last modified: Mon May  6 02:21:46 2024, max compression
```

## Comparing `batchfetch-1.0.5.tar` & `batchfetch-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-05 03:00:45.975829 batchfetch-1.0.5/
--rw-r--r--   0 dev        (455) work      (1000)    35149 2024-05-05 02:57:20.000000 batchfetch-1.0.5/LICENSE
--rw-r--r--   0 dev        (455) work      (1000)     4367 2024-05-05 03:00:45.975829 batchfetch-1.0.5/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)     3590 2024-05-05 02:57:20.000000 batchfetch-1.0.5/README.md
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-05 03:00:45.975829 batchfetch-1.0.5/batchfetch/
--rw-r--r--   0 dev        (455) work      (1000)      774 2024-05-05 02:57:20.000000 batchfetch-1.0.5/batchfetch/__init__.py
--rw-r--r--   0 dev        (455) work      (1000)     5419 2024-05-05 02:57:20.000000 batchfetch-1.0.5/batchfetch/batchfetch_base.py
--rw-r--r--   0 dev        (455) work      (1000)     9045 2024-05-05 02:57:20.000000 batchfetch-1.0.5/batchfetch/batchfetch_cli.py
--rw-r--r--   0 dev        (455) work      (1000)    13029 2024-05-05 02:57:20.000000 batchfetch-1.0.5/batchfetch/batchfetch_git.py
--rw-r--r--   0 dev        (455) work      (1000)     4081 2024-05-05 02:57:20.000000 batchfetch-1.0.5/batchfetch/helpers.py
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-05 03:00:45.975829 batchfetch-1.0.5/batchfetch.egg-info/
--rw-r--r--   0 dev        (455) work      (1000)     4367 2024-05-05 03:00:45.000000 batchfetch-1.0.5/batchfetch.egg-info/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)      365 2024-05-05 03:00:45.000000 batchfetch-1.0.5/batchfetch.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (455) work      (1000)        1 2024-05-05 03:00:45.000000 batchfetch-1.0.5/batchfetch.egg-info/dependency_links.txt
--rw-r--r--   0 dev        (455) work      (1000)       80 2024-05-05 03:00:45.000000 batchfetch-1.0.5/batchfetch.egg-info/entry_points.txt
--rw-r--r--   0 dev        (455) work      (1000)       36 2024-05-05 03:00:45.000000 batchfetch-1.0.5/batchfetch.egg-info/requires.txt
--rw-r--r--   0 dev        (455) work      (1000)       11 2024-05-05 03:00:45.000000 batchfetch-1.0.5/batchfetch.egg-info/top_level.txt
--rw-r--r--   0 dev        (455) work      (1000)       38 2024-05-05 03:00:45.975829 batchfetch-1.0.5/setup.cfg
--rwxr-xr-x   0 dev        (455) work      (1000)     2029 2024-05-05 02:57:20.000000 batchfetch-1.0.5/setup.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-06 02:21:46.771929 batchfetch-1.0.6/
+-rw-r--r--   0 dev        (455) work      (1000)    35149 2024-05-06 02:21:40.000000 batchfetch-1.0.6/LICENSE
+-rw-r--r--   0 dev        (455) work      (1000)     4337 2024-05-06 02:21:46.771929 batchfetch-1.0.6/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)     3560 2024-05-06 02:21:40.000000 batchfetch-1.0.6/README.md
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-06 02:21:46.767929 batchfetch-1.0.6/batchfetch/
+-rw-r--r--   0 dev        (455) work      (1000)      774 2024-05-06 02:21:40.000000 batchfetch-1.0.6/batchfetch/__init__.py
+-rw-r--r--   0 dev        (455) work      (1000)     5421 2024-05-06 02:21:40.000000 batchfetch-1.0.6/batchfetch/batchfetch_base.py
+-rw-r--r--   0 dev        (455) work      (1000)     9551 2024-05-06 02:21:40.000000 batchfetch-1.0.6/batchfetch/batchfetch_cli.py
+-rw-r--r--   0 dev        (455) work      (1000)    13084 2024-05-06 02:21:40.000000 batchfetch-1.0.6/batchfetch/batchfetch_git.py
+-rw-r--r--   0 dev        (455) work      (1000)     4101 2024-05-06 02:21:40.000000 batchfetch-1.0.6/batchfetch/helpers.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-06 02:21:46.771929 batchfetch-1.0.6/batchfetch.egg-info/
+-rw-r--r--   0 dev        (455) work      (1000)     4337 2024-05-06 02:21:46.000000 batchfetch-1.0.6/batchfetch.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)      365 2024-05-06 02:21:46.000000 batchfetch-1.0.6/batchfetch.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (455) work      (1000)        1 2024-05-06 02:21:46.000000 batchfetch-1.0.6/batchfetch.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (455) work      (1000)       80 2024-05-06 02:21:46.000000 batchfetch-1.0.6/batchfetch.egg-info/entry_points.txt
+-rw-r--r--   0 dev        (455) work      (1000)       36 2024-05-06 02:21:46.000000 batchfetch-1.0.6/batchfetch.egg-info/requires.txt
+-rw-r--r--   0 dev        (455) work      (1000)       11 2024-05-06 02:21:46.000000 batchfetch-1.0.6/batchfetch.egg-info/top_level.txt
+-rw-r--r--   0 dev        (455) work      (1000)       38 2024-05-06 02:21:46.771929 batchfetch-1.0.6/setup.cfg
+-rwxr-xr-x   0 dev        (455) work      (1000)     2029 2024-05-06 02:21:40.000000 batchfetch-1.0.6/setup.py
```

### Comparing `batchfetch-1.0.5/LICENSE` & `batchfetch-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.5/PKG-INFO` & `batchfetch-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchfetch
-Version: 1.0.5
+Version: 1.0.6
 Summary: Efficiently clone and pull multiple Git repositories.
 Home-page: https://github.com/jamescherti/batchfetch
 Author: James Cherti
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -76,20 +76,21 @@
 Here are the various options that `batchfetch` provides, along with descriptions of their usage:
 
 ```
 usage: batchfetch [--option] [args]
 
 Command line interface.
 
+positional arguments:
+  N                     Specify the batchfetch YAML file(s) (default: './batchfetch.yaml').
+
 options:
   -h, --help            show this help message and exit
   -j JOBS, --jobs JOBS  Run up to N Number of parallel processes (Default: 5).
   -v, --verbose         Enable verbose mode.
-  -f BATCHFETCH_FILE, --batchfetch-file BATCHFETCH_FILE
-                        Specify the batchfetch YAML file (default: './batchfetch.yaml').
 ```
 
 ## License
 
 Copyright (c) [James Cherti](https://www.jamescherti.com)
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
```

### Comparing `batchfetch-1.0.5/README.md` & `batchfetch-1.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -56,20 +56,21 @@
 Here are the various options that `batchfetch` provides, along with descriptions of their usage:
 
 ```
 usage: batchfetch [--option] [args]
 
 Command line interface.
 
+positional arguments:
+  N                     Specify the batchfetch YAML file(s) (default: './batchfetch.yaml').
+
 options:
   -h, --help            show this help message and exit
   -j JOBS, --jobs JOBS  Run up to N Number of parallel processes (Default: 5).
   -v, --verbose         Enable verbose mode.
-  -f BATCHFETCH_FILE, --batchfetch-file BATCHFETCH_FILE
-                        Specify the batchfetch YAML file (default: './batchfetch.yaml').
 ```
 
 ## License
 
 Copyright (c) [James Cherti](https://www.jamescherti.com)
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
```

### Comparing `batchfetch-1.0.5/batchfetch/__init__.py` & `batchfetch-1.0.6/batchfetch/__init__.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.5/batchfetch/batchfetch_base.py` & `batchfetch-1.0.6/batchfetch/batchfetch_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
-# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more
+# details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program. If not, see <https://www.gnu.org/licenses/>.
 #
 "Base class used to run tasks in parallel."
 
 import os
```

### Comparing `batchfetch-1.0.5/batchfetch/batchfetch_cli.py` & `batchfetch-1.0.6/batchfetch/batchfetch_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
-# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more
+# details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program. If not, see <https://www.gnu.org/licenses/>.
 #
 """Command line interface."""
 
 import argparse
 import logging
 import os
 import subprocess
 import sys
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from pathlib import Path
-from typing import Any, Dict, Set, TypeVar
+from typing import Any, Dict, Set
 
 import colorama
 import yaml  # type: ignore
 from colorama import Fore
 from schema import Optional, Or, Schema, SchemaError
 from setproctitle import setproctitle
 
@@ -44,16 +45,14 @@
         self.folder = Path(".")
         self.managed_filenames: Set[str] = set()
         self.verbose = verbose
         self.max_workers = max_workers
         self._logger = logging.getLogger(self.__class__.__name__)
         self.dirs_relative_to_batchfetch: Set[str] = set()
 
-        self.main_key = "git"
-
         # Plugin
         self.batchfetch_schemas: Dict[Any, Any] = {}
         self.batchfetch_classes: Dict[str, BatchFetchBase] = {}
         self.cfg_schema: Dict[Any, Any] = {}
         self._plugin_add("git", BatchFetchGit)
 
     def _plugin_add(self, keyword: str, batchfetch_class: Any):
@@ -130,25 +129,24 @@
                     options=self.cfg["options"],
                 )
                 self.cfg["tasks"].append(batchfetch_instance)
             except SchemaError as err:
                 print(f"Schema error: {err}.", file=sys.stderr)
                 sys.exit(1)
 
-            if batchfetch_instance["path"] in dict_local_dir:
-                err_str = ("more than one repository have the " +
-                           "destination path '" +
-                           str(batchfetch_instance["path"]) + "' (" +
+            dest_path = Path(batchfetch_instance["path"]).resolve()
+            if str(dest_path) in dict_local_dir:
+                err_str = ("More than one task have the " +
+                           f"destination path '{dest_path}' (" +
                            str(task[keyword]) + " and " +
-                           str(dict_local_dir[batchfetch_instance["path"]]) +
+                           str(dict_local_dir[(str(dest_path))]) +
                            ")")
                 raise BatchFetchError(err_str)
 
-            dict_local_dir[batchfetch_instance["path"]] = \
-                batchfetch_instance[keyword]
+            dict_local_dir[str(dest_path)] = batchfetch_instance[keyword]
 
     def run_tasks(self) -> bool:
         failed = []
         error = False
         threads = []
         num_success = 0
         self.managed_filenames = set()
@@ -199,76 +197,90 @@
                     print("  -", failed_result["path"])
             else:
                 print("Failed.")
 
             return False
         else:
             if num_success == 0:
-                print("Already up to date.")
+                print("Nothing to do.")
             elif not self.verbose:
                 print("Success.")
 
         return True
 
 
 def parse_args():
     """Parse the command line arguments."""
     desc = __doc__
     usage = "%(prog)s [--option] [args]"
     parser = argparse.ArgumentParser(description=desc, usage=usage)
 
+    parser.add_argument("batchfetch_files", metavar="N", type=str, nargs="*",
+                        help=("Specify the batchfetch YAML file(s) "
+                              "(default: './batchfetch.yaml')."))
+
     parser.add_argument(
         "-j", "--jobs", default="5", required=False,
         help="Run up to N Number of parallel processes (Default: 5).",
     )
 
     parser.add_argument(
         "-v", "--verbose", action="store_true", default=False,
         help="Enable verbose mode.",
     )
 
-    parser.add_argument(
-        "-f",
-        "--batchfetch-file",
-        default="./batchfetch.yaml",
-        required=False,
-        help="Specify the batchfetch YAML file (default: './batchfetch.yaml').",
-    )
-
     args = parser.parse_args()
 
-    if not Path(args.batchfetch_file).is_file():
-        print(f"Error: File not found: {args.batchfetch_file}",
-              file=sys.stderr)
-        sys.exit(1)
+    for batchfetch_file in args.batchfetch_files:
+        if not Path(batchfetch_file).is_file():
+            print(f"Error: File not found: {batchfetch_file}",
+                  file=sys.stderr)
+            sys.exit(1)
 
     return args
 
 
-def command_line_interface():
-    """Command line interface."""
+def run_batchfetch_procedure(batchfetch_file: Path, args) -> int:
     errno = 0
-    logging.basicConfig(level=logging.INFO, stream=sys.stdout,
-                        format="%(asctime)s %(name)s: %(message)s")
-
-    colorama.init()
-    setproctitle(subprocess.list2cmdline([Path(sys.argv[0]).name] +
-                                         sys.argv[1:]))
-
-    args = parse_args()
     batchfetch_cli = BatchFetchCli(verbose=args.verbose,
                                    max_workers=int(args.jobs))
-
-    batchfetch_cli.load(args.batchfetch_file)
-    os.chdir(os.path.dirname(args.batchfetch_file))
+    batchfetch_cli.load(batchfetch_file)
+    os.chdir(batchfetch_file.parent)
 
     try:
         if not batchfetch_cli.run_tasks():
             errno = 1
     except KeyboardInterrupt:
         print("Interrupted.", file=sys.stderr)
         errno = 1
     except BatchFetchError as err:
         print(f"Error: {err}.", file=sys.stderr)
         errno = 1
 
-    sys.exit(errno)
+    return errno
+
+
+def command_line_interface():
+    """Command line interface."""
+    try:
+        errno = 0
+        logging.basicConfig(level=logging.INFO, stream=sys.stdout,
+                            format="%(asctime)s %(name)s: %(message)s")
+
+        colorama.init()
+        setproctitle(subprocess.list2cmdline([Path(sys.argv[0]).name] +
+                                             sys.argv[1:]))
+
+        args = parse_args()
+        done = []
+        for batchfetch_file in args.batchfetch_files:
+            batchfetch_file = Path(batchfetch_file)
+            batchfetch_file_resolved = batchfetch_file.resolve()
+            if batchfetch_file_resolved in done:
+                continue
+
+            done.append(batchfetch_file_resolved)
+            errno |= run_batchfetch_procedure(batchfetch_file, args)
+
+        sys.exit(errno)
+    except BrokenPipeError:
+        pass
```

### Comparing `batchfetch-1.0.5/batchfetch/batchfetch_git.py` & `batchfetch-1.0.6/batchfetch/batchfetch_git.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
-# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more
+# details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program. If not, see <https://www.gnu.org/licenses/>.
 #
 "Clone and update Git repositories."
 
 
@@ -154,15 +155,15 @@
             self.add_output(self.indent_spaces + "[ERROR] " + str(err) + "\n")
             self.add_output(self.indent_spaces +
                             textwrap.indent(err.stdout, " " * self.indent) +
                             "\n" +
                             textwrap.indent(err.stderr, " " * self.indent))
 
         if not self.is_error() and not self.is_changed():
-            self.add_output(self.indent_spaces + "# Already up to date\n")
+            self.add_output(self.indent_spaces + "[INFO] Nothing to do.\n")
 
         return self.values
 
     def _update_current_branch(self):
         try:
             self.current_branch, _ = run_simple(
                 ["git", "symbolic-ref", "--short", "HEAD"],
@@ -171,26 +172,26 @@
             )
         except subprocess.CalledProcessError:
             # Not a symbolic ref
             self.current_branch = None
 
     def _repo_delete(self):
         if not self.git_local_dir.exists():
-            self.add_output(self.indent_spaces + "# Already deleted\n")
+            self.add_output(self.indent_spaces + "[INFO] Already deleted\n")
         elif not self.git_local_dir.joinpath(".git").is_dir():
             self.add_output(
                 self.indent_spaces +
                 f"# Cannot be deleted because '{self.git_local_dir}' is "
                 "not a Git repository\n"
             )
             self.set_error(True)
         elif self.git_local_dir.is_dir():
             shutil.rmtree(str(self.git_local_dir))
             self.add_output(self.indent_spaces +
-                            f"# Deleted: '{self.git_local_dir}'")
+                            f"[INFO] Deleted: '{self.git_local_dir}'")
             self.set_changed(True)
 
     def _repo_clone(self):
         git_clone_args = self["clone_args"]
         git_clone_args += ["--recurse-submodules"]
 
         cmd = ["git", "clone"] + git_clone_args + \
@@ -236,15 +237,15 @@
                 # 2. Ignore Git pull if it is not a local branch
                 if (not ignore_git_pull and
                         not self._git_is_local_branch(self["reference"])):
                     ignore_git_pull = True
 
         if ignore_git_pull:
             self.add_output(self.indent_spaces +
-                            "# git pull ignored\n")
+                            "[INFO] git pull ignored\n")
         else:
             cmd = ["git", "fetch", "origin"]
             self._run(cmd, cwd=str(self.git_local_dir), env=self.env)
 
             # TODO: only merge when difference from upstream
             commit_ref = self._git_ref(cwd=self.git_local_dir)
             self._run(["git", "merge", "--ff-only"],
@@ -313,15 +314,16 @@
                                       "does not exist.") from err
 
             if git_ref_after_merge != git_ref_branch and \
                     self["reference"] not in git_tags:
                 # Update the branch
                 self._run(["git", "checkout"] + [self["reference"]],
                           cwd=str(self.git_local_dir), env=self.env)
-                self.add_output(self.indent_spaces + "# Branch changed to " +
+                self.add_output(self.indent_spaces +
+                                "[INFO] Branch changed to " +
                                 self["reference"] + "\n")
                 self.set_changed(True)
                 branch_changed = True
 
                 # Read branch again
                 self._update_current_branch()
```

### Comparing `batchfetch-1.0.5/batchfetch/helpers.py` & `batchfetch-1.0.6/batchfetch/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+#!/usr/bin/env python
 #
 # Copyright (c) James Cherti
 # URL: https://github.com/jamescherti/batchfetch
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
-# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+# FOR A PARTICULAR PURPOSE. See the GNU General Public License for more
+# details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program. If not, see <https://www.gnu.org/licenses/>.
 #
 "Batchfetch helper functions."
 
 import hashlib
@@ -24,15 +26,15 @@
 
 
 def md5sum(filename: os.PathLike):
     """
     Calculate and return the MD5 checksum of a file.
 
     Args:
-        filename: The path to the file for which the MD5 checksum is calculated.
+        filename: Path to the file for which the MD5 checksum is calculated.
 
     Returns:
         str: The MD5 checksum of the file.
 
     """
     md5 = hashlib.md5()
     with open(filename, "rb") as file:
```

### Comparing `batchfetch-1.0.5/batchfetch.egg-info/PKG-INFO` & `batchfetch-1.0.6/batchfetch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchfetch
-Version: 1.0.5
+Version: 1.0.6
 Summary: Efficiently clone and pull multiple Git repositories.
 Home-page: https://github.com/jamescherti/batchfetch
 Author: James Cherti
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -76,20 +76,21 @@
 Here are the various options that `batchfetch` provides, along with descriptions of their usage:
 
 ```
 usage: batchfetch [--option] [args]
 
 Command line interface.
 
+positional arguments:
+  N                     Specify the batchfetch YAML file(s) (default: './batchfetch.yaml').
+
 options:
   -h, --help            show this help message and exit
   -j JOBS, --jobs JOBS  Run up to N Number of parallel processes (Default: 5).
   -v, --verbose         Enable verbose mode.
-  -f BATCHFETCH_FILE, --batchfetch-file BATCHFETCH_FILE
-                        Specify the batchfetch YAML file (default: './batchfetch.yaml').
 ```
 
 ## License
 
 Copyright (c) [James Cherti](https://www.jamescherti.com)
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
```

### Comparing `batchfetch-1.0.5/setup.py` & `batchfetch-1.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 setup(
     name="batchfetch",
-    version="1.0.5",
+    version="1.0.6",
     packages=find_packages(),
     description="Efficiently clone and pull multiple Git repositories.",
     license="GPLv3",
     long_description=((Path(__file__).parent.resolve().joinpath("README.md"))
                       .read_text(encoding="utf-8")),
     long_description_content_type="text/markdown",
     url="https://github.com/jamescherti/batchfetch",
```

