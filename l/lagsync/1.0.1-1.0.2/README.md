# Comparing `tmp/lagsync-1.0.1.tar.gz` & `tmp/lagsync-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lagsync-1.0.1.tar", last modified: Mon May  6 21:11:24 2024, max compression
+gzip compressed data, was "lagsync-1.0.2.tar", last modified: Mon May  6 21:25:42 2024, max compression
```

## Comparing `lagsync-1.0.1.tar` & `lagsync-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 21:11:24.558809 lagsync-1.0.1/
--rw-rw-rw-   0        0        0     1090 2024-05-05 18:03:53.000000 lagsync-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2086 2024-05-06 21:11:24.558809 lagsync-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       63 2024-05-06 21:10:44.000000 lagsync-1.0.1/README.md
--rw-rw-rw-   0        0        0      933 2024-05-06 21:10:44.000000 lagsync-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 21:11:24.558809 lagsync-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 21:11:24.542809 lagsync-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 21:11:24.545810 lagsync-1.0.1/src/lagsync/
--rw-rw-rw-   0        0        0        0 2024-05-06 20:44:08.000000 lagsync-1.0.1/src/lagsync/__init__.py
--rw-rw-rw-   0        0        0     5986 2024-05-06 20:57:59.000000 lagsync-1.0.1/src/lagsync/lagsync.py
-drwxrwxrwx   0        0        0        0 2024-05-06 21:11:24.557808 lagsync-1.0.1/src/lagsync.egg-info/
--rw-rw-rw-   0        0        0     2086 2024-05-06 21:11:24.000000 lagsync-1.0.1/src/lagsync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-05-06 21:11:24.000000 lagsync-1.0.1/src/lagsync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 21:11:24.000000 lagsync-1.0.1/src/lagsync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-06 21:11:24.000000 lagsync-1.0.1/src/lagsync.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2024-05-06 21:11:24.000000 lagsync-1.0.1/src/lagsync.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 21:25:42.215516 lagsync-1.0.2/
+-rw-rw-rw-   0        0        0     1090 2024-05-05 18:03:53.000000 lagsync-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2086 2024-05-06 21:25:42.214522 lagsync-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2024-05-06 21:10:44.000000 lagsync-1.0.2/README.md
+-rw-rw-rw-   0        0        0      933 2024-05-06 21:25:14.000000 lagsync-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 21:25:42.215516 lagsync-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 21:25:42.198494 lagsync-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 21:25:42.202523 lagsync-1.0.2/src/lagsync/
+-rw-rw-rw-   0        0        0        0 2024-05-06 20:44:08.000000 lagsync-1.0.2/src/lagsync/__init__.py
+-rw-rw-rw-   0        0        0     6169 2024-05-06 21:25:14.000000 lagsync-1.0.2/src/lagsync/lagsync.py
+drwxrwxrwx   0        0        0        0 2024-05-06 21:25:42.213491 lagsync-1.0.2/src/lagsync.egg-info/
+-rw-rw-rw-   0        0        0     2086 2024-05-06 21:25:42.000000 lagsync-1.0.2/src/lagsync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-05-06 21:25:42.000000 lagsync-1.0.2/src/lagsync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 21:25:42.000000 lagsync-1.0.2/src/lagsync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-06 21:25:42.000000 lagsync-1.0.2/src/lagsync.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-05-06 21:25:42.000000 lagsync-1.0.2/src/lagsync.egg-info/top_level.txt
```

### Comparing `lagsync-1.0.1/LICENSE` & `lagsync-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lagsync-1.0.1/PKG-INFO` & `lagsync-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lagsync
-Version: 1.0.1
+Version: 1.0.2
 Summary: A rsync based backup utility for laggy connections
 Author-email: bluePlatinum <jukic.rok@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 bluePlatinum
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lagsync-1.0.1/pyproject.toml` & `lagsync-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lagsync"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name="bluePlatinum", email="jukic.rok@gmail.com" },
 ]
 description="A rsync based backup utility for laggy connections"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
```

### Comparing `lagsync-1.0.1/src/lagsync/lagsync.py` & `lagsync-1.0.2/src/lagsync/lagsync.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,39 +81,44 @@
     try:
         dry_run = kwargs['dry_run']
     except KeyError:
         dry_run = False
 
     sync_objects = dirlist + filelist
 
-    remote, remote_dir = destination.split(":")
+    if len(destination.split(":")) == 2:
+        remote, remote_dir = destination.split(":")
+        remote += ":"       # add the : delimiter to the remote variable
+    else:
+        remote = ""
+        remote_dir = destination
 
     for sync_object in sync_objects:
         src = os.path.join(source, sync_object)
         dst = os.path.join(remote_dir, sync_object)
 
         logging.info(f"Syncing {src}")
 
         if not dry_run:
             retry = 0
-            proc = subprocess.run(["rsync", f"-{options} {src} {remote}:{dst}"])
+            proc = subprocess.run(["rsync", f"-{options} {src} {remote}{dst}"])
 
             while proc.returncode != 0:
                 logging.info(f"Failed sync of {src}. Retrying (retry={retry})")
                 retry += 1
                 proc = subprocess.run(["rsync",
-                                       f"-{options} {src} {remote}:{dst}"])
+                                       f"-{options} {src} {remote}{dst}"])
                 if retry >= max_retries:
                     logging.critical(f"Reached maximum amount of retries "
                                      f"(max_retries={max_retries}). Sync job "
                                      f"{sync_object} failed. Aborting.")
                     return 1
 
         else:
-            print(f"rsync -{options} {src} {remote}:{dst}")
+            print(f"rsync -{options} {src} {remote}{dst}")
 
     return 0
 
 
 def main():
     """
     The main function to be run for the script in cli mode.
```

### Comparing `lagsync-1.0.1/src/lagsync.egg-info/PKG-INFO` & `lagsync-1.0.2/src/lagsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lagsync
-Version: 1.0.1
+Version: 1.0.2
 Summary: A rsync based backup utility for laggy connections
 Author-email: bluePlatinum <jukic.rok@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 bluePlatinum
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

