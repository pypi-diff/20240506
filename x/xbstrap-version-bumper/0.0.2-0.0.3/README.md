# Comparing `tmp/xbstrap_version_bumper-0.0.2.tar.gz` & `tmp/xbstrap_version_bumper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbstrap_version_bumper-0.0.2.tar", last modified: Sun May  5 22:18:34 2024, max compression
+gzip compressed data, was "xbstrap_version_bumper-0.0.3.tar", last modified: Sun May  5 23:11:48 2024, max compression
```

## Comparing `xbstrap_version_bumper-0.0.2.tar` & `xbstrap_version_bumper-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 22:18:34.839440 xbstrap_version_bumper-0.0.2/
--rw-r--r--   0 alexander  (1000) wheel      (998)     1075 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.2/LICENSE
--rw-r--r--   0 alexander  (1000) wheel      (998)      840 2024-05-05 22:18:34.839440 xbstrap_version_bumper-0.0.2/PKG-INFO
--rw-r--r--   0 alexander  (1000) wheel      (998)      181 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.2/README.md
--rw-r--r--   0 alexander  (1000) wheel      (998)      807 2024-05-05 22:17:48.000000 xbstrap_version_bumper-0.0.2/pyproject.toml
--rw-r--r--   0 alexander  (1000) wheel      (998)       38 2024-05-05 22:18:34.839440 xbstrap_version_bumper-0.0.2/setup.cfg
-drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 22:18:34.838440 xbstrap_version_bumper-0.0.2/src/
-drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 22:18:34.838440 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper/
--rw-r--r--   0 alexander  (1000) wheel      (998)        0 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper/__init__.py
--rw-r--r--   0 alexander  (1000) wheel      (998)      102 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper/__main__.py
--rw-r--r--   0 alexander  (1000) wheel      (998)     8430 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper/linecounted_yaml.py
--rw-r--r--   0 alexander  (1000) wheel      (998)    11360 2024-05-05 22:16:01.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper/main.py
-drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 22:18:34.839440 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper.egg-info/
--rw-r--r--   0 alexander  (1000) wheel      (998)      840 2024-05-05 22:18:34.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper.egg-info/PKG-INFO
--rw-r--r--   0 alexander  (1000) wheel      (998)      494 2024-05-05 22:18:34.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper.egg-info/SOURCES.txt
--rw-r--r--   0 alexander  (1000) wheel      (998)        1 2024-05-05 22:18:34.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper.egg-info/dependency_links.txt
--rw-r--r--   0 alexander  (1000) wheel      (998)       76 2024-05-05 22:18:34.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper.egg-info/entry_points.txt
--rw-r--r--   0 alexander  (1000) wheel      (998)       55 2024-05-05 22:18:34.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper.egg-info/requires.txt
--rw-r--r--   0 alexander  (1000) wheel      (998)       23 2024-05-05 22:18:34.000000 xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper.egg-info/top_level.txt
+drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 23:11:48.465746 xbstrap_version_bumper-0.0.3/
+-rw-r--r--   0 alexander  (1000) wheel      (998)     1075 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.3/LICENSE
+-rw-r--r--   0 alexander  (1000) wheel      (998)      840 2024-05-05 23:11:48.465746 xbstrap_version_bumper-0.0.3/PKG-INFO
+-rw-r--r--   0 alexander  (1000) wheel      (998)      181 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.3/README.md
+-rw-r--r--   0 alexander  (1000) wheel      (998)      807 2024-05-05 23:11:34.000000 xbstrap_version_bumper-0.0.3/pyproject.toml
+-rw-r--r--   0 alexander  (1000) wheel      (998)       38 2024-05-05 23:11:48.465746 xbstrap_version_bumper-0.0.3/setup.cfg
+drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 23:11:48.463745 xbstrap_version_bumper-0.0.3/src/
+drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 23:11:48.464746 xbstrap_version_bumper-0.0.3/src/xbstrap_version_bumper/
+-rw-r--r--   0 alexander  (1000) wheel      (998)        0 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.3/src/xbstrap_version_bumper/__init__.py
+-rw-r--r--   0 alexander  (1000) wheel      (998)      102 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.3/src/xbstrap_version_bumper/__main__.py
+-rw-r--r--   0 alexander  (1000) wheel      (998)     8430 2024-05-05 21:56:22.000000 xbstrap_version_bumper-0.0.3/src/xbstrap_version_bumper/linecounted_yaml.py
+-rw-r--r--   0 alexander  (1000) wheel      (998)    13455 2024-05-05 23:10:50.000000 xbstrap_version_bumper-0.0.3/src/xbstrap_version_bumper/main.py
+drwxr-xr-x   0 alexander  (1000) wheel      (998)        0 2024-05-05 23:11:48.465746 xbstrap_version_bumper-0.0.3/src/xbstrap_version_bumper.egg-info/
+-rw-r--r--   0 alexander  (1000) wheel      (998)      840 2024-05-05 23:11:48.000000 xbstrap_version_bumper-0.0.3/src/xbstrap_version_bumper.egg-info/PKG-INFO
+-rw-r--r--   0 alexander  (1000) wheel      (998)      494 2024-05-05 23:11:48.000000 xbstrap_version_bumper-0.0.3/src/xbstrap_version_bumper.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander  (1000) wheel      (998)        1 2024-05-05 23:11:48.000000 xbstrap_version_bumper-0.0.3/src/xbstrap_version_bumper.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander  (1000) wheel      (998)       76 2024-05-05 23:11:48.000000 xbstrap_version_bumper-0.0.3/src/xbstrap_version_bumper.egg-info/entry_points.txt
+-rw-r--r--   0 alexander  (1000) wheel      (998)       55 2024-05-05 23:11:48.000000 xbstrap_version_bumper-0.0.3/src/xbstrap_version_bumper.egg-info/requires.txt
+-rw-r--r--   0 alexander  (1000) wheel      (998)       23 2024-05-05 23:11:48.000000 xbstrap_version_bumper-0.0.3/src/xbstrap_version_bumper.egg-info/top_level.txt
```

### Comparing `xbstrap_version_bumper-0.0.2/LICENSE` & `xbstrap_version_bumper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xbstrap_version_bumper-0.0.2/PKG-INFO` & `xbstrap_version_bumper-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbstrap_version_bumper
-Version: 0.0.2
+Version: 0.0.3
 Summary: xbstrap distro auto version bumper
 Author-email: Alexander Richards <electrodeyt@gmail.com>
 Project-URL: Homepage, https://github.com/ElectrodeYT/xbstrap_version_bumper
 Project-URL: Issues, https://github.com/ElectrodeYT/xbstrap_version_bumper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xbstrap_version_bumper-0.0.2/pyproject.toml` & `xbstrap_version_bumper-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xbstrap_version_bumper"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Alexander Richards", email="electrodeyt@gmail.com" },
 ]
 requires-python = ">=3.8"
 description="xbstrap distro auto version bumper"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper/linecounted_yaml.py` & `xbstrap_version_bumper-0.0.3/src/xbstrap_version_bumper/linecounted_yaml.py`

 * *Files identical despite different names*

### Comparing `xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper/main.py` & `xbstrap_version_bumper-0.0.3/src/xbstrap_version_bumper/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 import os
 import pathlib
+from functools import cmp_to_key
 from typing import Any
 import hashlib
 import argparse
 
+import git
+import libversion
 import ruamel.yaml
 import requests
 from git import Repo, Actor
 from pprint import pprint
 from git import RemoteProgress
 
 import xbstrap_version_bumper.linecounted_yaml
 
 global_yaml = ruamel.yaml.YAML(typ='safe')
 global_yaml.Constructor = xbstrap_version_bumper.linecounted_yaml.MyConstructor
 
 
+def sort_versions(version_list: list) -> str:
+    return sorted(version_list, key=cmp_to_key(libversion.version_compare2))[-1]
+
+
 class ProgressPrinter(RemoteProgress):
     def update(self, op_code, cur_count, max_count=None, message=""):
         print(
             op_code,
             cur_count,
             max_count,
             cur_count / (max_count or 100.0),
@@ -222,14 +229,44 @@
 
         if 'build' in package:
             for build in package['build']:
                 changes += self.__args_to_changes(build['args'], old_version, new_version)
 
         self.__add_changes_to_stapfile(strapfile, changes)
 
+    def __get_latest_git_version(self, source):
+        if 'git' not in source:
+            return False
+        g = git.cmd.Git()
+        blob = g.ls_remote(source['git'], sort='-v:refname', tags=True)
+        available_versions = []
+        for line in blob.split('\n'):
+            available_versions.append(line.split('/')[-1])
+        newest_version = sort_versions(available_versions)
+        print(f'---> Latest git tag: {newest_version}')
+
+        if newest_version[0] == 'v':
+            newest_version = newest_version[1:]
+        print(f'---> Latest version: {newest_version}')
+
+        return newest_version
+
+    def get_latest_git_version_of_package(self, package_name):
+        strapfile, package = self.__locate_package(package_name)
+        if 'source' in package:
+            return self.__get_latest_git_version(package['source'])
+        else:
+            assert 'from_source' in package
+            strapfile, source_in_package, source = self.__locate_source(package['from_source'])
+            return self.__get_latest_git_version(source)
+
+    def get_latest_git_version_of_source(self, source_name):
+        strapfile, source_in_package, source = self.__locate_source(source_name)
+        return self.__get_latest_git_version(source)
+
     def emit_modified_yaml(self):
         for strapfile in self.strapfiles:
             if strapfile.path not in self.modified_files.keys():
                 continue
 
             strapfile.emit()
 
@@ -242,20 +279,21 @@
     parser.add_argument('--is-source', action='store_true')
     parser.add_argument('--set-version')
     parser.add_argument('--bootstrap-dir', required=True)
     parser.add_argument('--pull-from-master', action='store_true')
     parser.add_argument('--create-branch', action='store_true')
     parser.add_argument('--commiter-name')
     parser.add_argument('--commiter-email')
+    parser.add_argument('--attempt-latest-version-autodetect', action='store_true')
     args = parser.parse_args()
 
     pprint(args)
 
-    if not (args.set_version):
-        parser.error('--set-version is required')
+    if not (args.set_version or args.attempt_latest_version_autodetect):
+        parser.error('--set-version or --attempt-latest-version-autodetect is required')
 
     if args.create_branch and (args.commiter_name is None or args.commiter_email is None):
         parser.error('--commiter-name and --commiter-email is required when creating a branch')
 
     repo = Repo(args.bootstrap_dir)
     assert not repo.bare
 
@@ -265,20 +303,32 @@
                 # Pull master from origin
                 print(f'--> Pulling from origin ({remote.url})')
                 #remote.pull(progress=ProgressPrinter())
 
     print('-> Reading bootstrap files')
     distro = Distro(args.bootstrap_dir)
 
+    version_to_set = args.set_version
+    if args.attempt_latest_version_autodetect:
+        if not args.is_source:
+            attempt_version_find = distro.get_latest_git_version_of_package(args.to_modify)
+        else:
+            attempt_version_find = distro.get_latest_git_version_of_source(args.to_modify)
+        if attempt_version_find:
+            version_to_set = attempt_version_find
+
+    if version_to_set is None:
+        print('----> Failed to determine a version to set!')
+
     if args.is_source:
-        if args.set_version is not None:
-            distro.modify_source_version(args.to_modify, args.set_version)
+        if version_to_set is not None:
+            distro.modify_source_version(args.to_modify, version_to_set)
     else:
-        if args.set_version is not None:
-            distro.modify_package_version(args.to_modify, args.set_version)
+        if version_to_set is not None:
+            distro.modify_package_version(args.to_modify, version_to_set)
 
     if args.create_branch:
         print('-> Stashing current git changes and checking out new branch from master')
         repo.git.stash('save')
         repo.git.checkout('master')
         repo.git.checkout('-b', f'xbstrap_version_bumper_{args.to_modify}_to_{args.set_version}')
```

### Comparing `xbstrap_version_bumper-0.0.2/src/xbstrap_version_bumper.egg-info/PKG-INFO` & `xbstrap_version_bumper-0.0.3/src/xbstrap_version_bumper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbstrap_version_bumper
-Version: 0.0.2
+Version: 0.0.3
 Summary: xbstrap distro auto version bumper
 Author-email: Alexander Richards <electrodeyt@gmail.com>
 Project-URL: Homepage, https://github.com/ElectrodeYT/xbstrap_version_bumper
 Project-URL: Issues, https://github.com/ElectrodeYT/xbstrap_version_bumper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

