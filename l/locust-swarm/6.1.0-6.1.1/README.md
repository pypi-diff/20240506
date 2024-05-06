# Comparing `tmp/locust-swarm-6.1.0.tar.gz` & `tmp/locust_swarm-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locust-swarm-6.1.0.tar", last modified: Tue Mar 19 19:03:31 2024, max compression
+gzip compressed data, was "locust_swarm-6.1.1.tar", last modified: Mon May  6 09:47:57 2024, max compression
```

## Comparing `locust-swarm-6.1.0.tar` & `locust_swarm-6.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:03:31.114204 locust-swarm-6.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:03:31.110204 locust-swarm-6.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:03:31.114204 locust-swarm-6.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/.travis.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:03:31.114204 locust-swarm-6.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-19 19:03:31.114204 locust-swarm-6.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:03:31.114204 locust-swarm-6.1.0/locust_swarm/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/locust_swarm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/locust_swarm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-19 19:03:30.000000 locust-swarm-6.1.0/locust_swarm/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    19060 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/locust_swarm/swarm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:03:31.114204 locust-swarm-6.1.0/locust_swarm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-19 19:03:31.000000 locust-swarm-6.1.0/locust_swarm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-19 19:03:31.000000 locust-swarm-6.1.0/locust_swarm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 19:03:31.000000 locust-swarm-6.1.0/locust_swarm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-19 19:03:31.000000 locust-swarm-6.1.0/locust_swarm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 19:03:31.000000 locust-swarm-6.1.0/locust_swarm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-19 19:03:31.000000 locust-swarm-6.1.0/locust_swarm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-19 19:03:31.000000 locust-swarm-6.1.0/locust_swarm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 19:03:31.114204 locust-swarm-6.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    46044 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/swarm.png
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/swarm.puml
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-19 19:03:22.000000 locust-swarm-6.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:47:57.010216 locust_swarm-6.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:47:57.006216 locust_swarm-6.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:47:57.006216 locust_swarm-6.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/.travis.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:47:57.010216 locust_swarm-6.1.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11390 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-06 09:47:57.010216 locust_swarm-6.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:47:57.010216 locust_swarm-6.1.1/locust_swarm/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/locust_swarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/locust_swarm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 09:47:56.000000 locust_swarm-6.1.1/locust_swarm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19060 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/locust_swarm/swarm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:47:57.010216 locust_swarm-6.1.1/locust_swarm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-06 09:47:56.000000 locust_swarm-6.1.1/locust_swarm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-06 09:47:57.000000 locust_swarm-6.1.1/locust_swarm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:47:56.000000 locust_swarm-6.1.1/locust_swarm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-06 09:47:56.000000 locust_swarm-6.1.1/locust_swarm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:47:56.000000 locust_swarm-6.1.1/locust_swarm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-06 09:47:56.000000 locust_swarm-6.1.1/locust_swarm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 09:47:56.000000 locust_swarm-6.1.1/locust_swarm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:47:57.010216 locust_swarm-6.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46044 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/swarm.png
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/swarm.puml
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-06 09:47:51.000000 locust_swarm-6.1.1/tox.ini
```

### Comparing `locust-swarm-6.1.0/.github/workflows/tests.yml` & `locust_swarm-6.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `locust-swarm-6.1.0/.pylintrc` & `locust_swarm-6.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `locust-swarm-6.1.0/.vscode/launch.json` & `locust_swarm-6.1.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `locust-swarm-6.1.0/.vscode/settings.json` & `locust_swarm-6.1.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `locust-swarm-6.1.0/LICENSE` & `locust_swarm-6.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `locust-swarm-6.1.0/PKG-INFO` & `locust_swarm-6.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust-swarm
-Version: 6.1.0
+Version: 6.1.1
 Summary: Load test + test data distribution & launching tool for Locust
 Home-page: https://github.com/SvenskaSpel/locust-swarm
 Author: Lars Holmberg
 License: Apache-2.0
 Classifier: Topic :: Software Development :: Testing :: Traffic Generation
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `locust-swarm-6.1.0/README.md` & `locust_swarm-6.1.1/README.md`

 * *Files identical despite different names*

### Comparing `locust-swarm-6.1.0/locust_swarm/swarm.py` & `locust_swarm-6.1.1/locust_swarm/swarm.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -427,18 +427,18 @@
         parser.error(
             f"--processes-per-loadgen has been removed in favour of locusts native --processes parameter (you had it set to {args.processes_per_loadgen})"
         )
     if args.skip_plugins:
         parser.error(
             "--skip-plugins has been removed, the default is now NOT to upload plugins (but you can enable it with --upload-plugins)"
         )
-    worker_process_count = args.processes * args.loadgens
     loadgen_list = args.loadgen_list.split(",")
     if args.loadgens < 0:
         args.loadgens = len(loadgen_list)
+    worker_process_count = args.processes * args.loadgens
 
     try:
         subprocess.check_output(
             f"ssh -o LogLevel=error -o BatchMode=yes {loadgen_list[0]} true 2>&1",
             shell=True,
             timeout=10,
         )
```

### Comparing `locust-swarm-6.1.0/locust_swarm.egg-info/PKG-INFO` & `locust_swarm-6.1.1/locust_swarm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locust-swarm
-Version: 6.1.0
+Version: 6.1.1
 Summary: Load test + test data distribution & launching tool for Locust
 Home-page: https://github.com/SvenskaSpel/locust-swarm
 Author: Lars Holmberg
 License: Apache-2.0
 Classifier: Topic :: Software Development :: Testing :: Traffic Generation
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `locust-swarm-6.1.0/locust_swarm.egg-info/SOURCES.txt` & `locust_swarm-6.1.1/locust_swarm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `locust-swarm-6.1.0/pyproject.toml` & `locust_swarm-6.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `locust-swarm-6.1.0/setup.py` & `locust_swarm-6.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `locust-swarm-6.1.0/swarm.png` & `locust_swarm-6.1.1/swarm.png`

 * *Files identical despite different names*

### Comparing `locust-swarm-6.1.0/swarm.puml` & `locust_swarm-6.1.1/swarm.puml`

 * *Files identical despite different names*

