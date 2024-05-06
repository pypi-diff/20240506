# Comparing `tmp/lagsync-1.0.3.tar.gz` & `tmp/lagsync-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lagsync-1.0.3.tar", last modified: Mon May  6 21:34:19 2024, max compression
+gzip compressed data, was "lagsync-1.1.0.tar", last modified: Mon May  6 21:49:27 2024, max compression
```

## Comparing `lagsync-1.0.3.tar` & `lagsync-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 21:34:19.065298 lagsync-1.0.3/
--rw-rw-rw-   0        0        0     1090 2024-05-05 18:03:53.000000 lagsync-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2086 2024-05-06 21:34:19.065298 lagsync-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       63 2024-05-06 21:10:44.000000 lagsync-1.0.3/README.md
--rw-rw-rw-   0        0        0      933 2024-05-06 21:34:08.000000 lagsync-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 21:34:19.065298 lagsync-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 21:34:19.048300 lagsync-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 21:34:19.051299 lagsync-1.0.3/src/lagsync/
--rw-rw-rw-   0        0        0        0 2024-05-06 20:44:08.000000 lagsync-1.0.3/src/lagsync/__init__.py
--rw-rw-rw-   0        0        0     6175 2024-05-06 21:34:08.000000 lagsync-1.0.3/src/lagsync/lagsync.py
-drwxrwxrwx   0        0        0        0 2024-05-06 21:34:19.064299 lagsync-1.0.3/src/lagsync.egg-info/
--rw-rw-rw-   0        0        0     2086 2024-05-06 21:34:19.000000 lagsync-1.0.3/src/lagsync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-05-06 21:34:19.000000 lagsync-1.0.3/src/lagsync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 21:34:19.000000 lagsync-1.0.3/src/lagsync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-06 21:34:19.000000 lagsync-1.0.3/src/lagsync.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2024-05-06 21:34:19.000000 lagsync-1.0.3/src/lagsync.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 21:49:27.672261 lagsync-1.1.0/
+-rw-rw-rw-   0        0        0     1090 2024-05-05 18:03:53.000000 lagsync-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2086 2024-05-06 21:49:27.672261 lagsync-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2024-05-06 21:10:44.000000 lagsync-1.1.0/README.md
+-rw-rw-rw-   0        0        0      933 2024-05-06 21:49:14.000000 lagsync-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 21:49:27.672261 lagsync-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 21:49:27.654721 lagsync-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 21:49:27.658263 lagsync-1.1.0/src/lagsync/
+-rw-rw-rw-   0        0        0        0 2024-05-06 20:44:08.000000 lagsync-1.1.0/src/lagsync/__init__.py
+-rw-rw-rw-   0        0        0     6527 2024-05-06 21:49:14.000000 lagsync-1.1.0/src/lagsync/lagsync.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:49:27.671262 lagsync-1.1.0/src/lagsync.egg-info/
+-rw-rw-rw-   0        0        0     2086 2024-05-06 21:49:27.000000 lagsync-1.1.0/src/lagsync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-05-06 21:49:27.000000 lagsync-1.1.0/src/lagsync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 21:49:27.000000 lagsync-1.1.0/src/lagsync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-06 21:49:27.000000 lagsync-1.1.0/src/lagsync.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-05-06 21:49:27.000000 lagsync-1.1.0/src/lagsync.egg-info/top_level.txt
```

### Comparing `lagsync-1.0.3/LICENSE` & `lagsync-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lagsync-1.0.3/PKG-INFO` & `lagsync-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lagsync
-Version: 1.0.3
+Version: 1.1.0
 Summary: A rsync based backup utility for laggy connections
 Author-email: bluePlatinum <jukic.rok@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 bluePlatinum
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lagsync-1.0.3/pyproject.toml` & `lagsync-1.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lagsync"
-version = "1.0.3"
+version = "1.1.0"
 authors = [
     { name="bluePlatinum", email="jukic.rok@gmail.com" },
 ]
 description="A rsync based backup utility for laggy connections"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

### Comparing `lagsync-1.0.3/src/lagsync/lagsync.py` & `lagsync-1.1.0/src/lagsync/lagsync.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 import argparse
 import logging
 import os
 import subprocess
+import time
 
 
 def get_depth(rootpath, path):
     """
     Get the depth of a given path. Only works if the given path is an
     abspath (os.path.abspath).
 
@@ -54,15 +55,15 @@
                     abspath = os.path.join(root, file)
                     filelist.append(abspath[len(path)+len(os.path.sep):])
 
     return dirlist, filelist
 
 
 def perform_sync(source, destination, dirlist, filelist, options,
-                 max_retries=10, *args, **kwargs):
+                 max_retries=10, fail_delay=3, *args, **kwargs):
     """
     Perform the syncronization with rsync.
 
     :param source: the source directory
     :type source: str
     :param destination: the destination to sync to
     :type destination: str
@@ -71,14 +72,16 @@
     :type dirlist: list
     :param filelist: The list of all files to be synched. Needs to be a list of
         paths relative to src.
     :param options: The options to pass to rsync.
     :type options: str
     :param max_retries: the maximum amount of retries before the job fails
     :type max_retries: int
+    :param fail_delay: the time to delay after failed sync
+    :type fail_delay: float
     :return: exit code
     :rtype: int
     """
     try:
         dry_run = kwargs['dry_run']
     except KeyError:
         dry_run = False
@@ -101,14 +104,15 @@
         if not dry_run:
             retry = 0
             proc = subprocess.run(
                 ["rsync", f"-{options}", src, f"{remote}{dst}"])
 
             while proc.returncode != 0:
                 logging.info(f"Failed sync of {src}. Retrying (retry={retry})")
+                time.sleep(fail_delay)
                 retry += 1
                 proc = subprocess.run(
                     ["rsync", f"-{options}", src, f"{remote}{dst}"])
                 if retry >= max_retries:
                     logging.critical(f"Reached maximum amount of retries "
                                      f"(max_retries={max_retries}). Sync job "
                                      f"{sync_object} failed. Aborting.")
@@ -148,23 +152,26 @@
                         help="The maximum amount of retries for the rsync job"
                              "per chunk")
     parser.add_argument("--dry-run", action="store_true",
                         help="Perform a dry run, which will only print out"
                              "the resync jobs instead of running them.")
     parser.add_argument("-v", "--verbose", action="store_true",
                         help="verbose mode")
+    parser.add_argument("--delay", default=3,
+                        help="Time to delay (in seconds) after failed chunk."
+                             "Default is 3.")
 
     args = parser.parse_args()
 
     # enable verbose logging
     if args.verbose:
         logging.basicConfig(level=logging.INFO)
 
     # perform sync
     dirlist, filelist = get_sync(args.source, args.depth)
     return perform_sync(args.source, args.destination, dirlist, filelist,
                         args.rsync_options, max_retries=args.max_retries,
-                        dry_run=args.dry_run)
+                        fail_delay=args.delay, dry_run=args.dry_run)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `lagsync-1.0.3/src/lagsync.egg-info/PKG-INFO` & `lagsync-1.1.0/src/lagsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lagsync
-Version: 1.0.3
+Version: 1.1.0
 Summary: A rsync based backup utility for laggy connections
 Author-email: bluePlatinum <jukic.rok@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 bluePlatinum
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

