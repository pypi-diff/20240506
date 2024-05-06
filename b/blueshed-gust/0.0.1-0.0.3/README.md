# Comparing `tmp/blueshed_gust-0.0.1.tar.gz` & `tmp/blueshed_gust-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueshed_gust-0.0.1.tar", last modified: Mon May  6 13:53:11 2024, max compression
+gzip compressed data, was "blueshed_gust-0.0.3.tar", last modified: Mon May  6 14:03:36 2024, max compression
```

## Comparing `blueshed_gust-0.0.1.tar` & `blueshed_gust-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,25 @@
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 13:53:11.647491 blueshed_gust-0.0.1/
--rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-06 13:53:11.647310 blueshed_gust-0.0.1/PKG-INFO
--rw-r--r--   0 peterb     (501) staff       (20)      320 2024-05-06 13:29:02.000000 blueshed_gust-0.0.1/README.md
--rw-r--r--   0 peterb     (501) staff       (20)     1879 2024-05-06 13:53:04.000000 blueshed_gust-0.0.1/pyproject.toml
--rw-r--r--   0 peterb     (501) staff       (20)       38 2024-05-06 13:53:11.647530 blueshed_gust-0.0.1/setup.cfg
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 13:53:11.645767 blueshed_gust-0.0.1/src/
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 13:53:11.646782 blueshed_gust-0.0.1/src/blueshed_gust.egg-info/
--rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-06 13:53:11.000000 blueshed_gust-0.0.1/src/blueshed_gust.egg-info/PKG-INFO
--rw-r--r--   0 peterb     (501) staff       (20)      228 2024-05-06 13:53:11.000000 blueshed_gust-0.0.1/src/blueshed_gust.egg-info/SOURCES.txt
--rw-r--r--   0 peterb     (501) staff       (20)        1 2024-05-06 13:53:11.000000 blueshed_gust-0.0.1/src/blueshed_gust.egg-info/dependency_links.txt
--rw-r--r--   0 peterb     (501) staff       (20)      124 2024-05-06 13:53:11.000000 blueshed_gust-0.0.1/src/blueshed_gust.egg-info/requires.txt
--rw-r--r--   0 peterb     (501) staff       (20)        1 2024-05-06 13:53:11.000000 blueshed_gust-0.0.1/src/blueshed_gust.egg-info/top_level.txt
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 14:03:36.460554 blueshed_gust-0.0.3/
+-rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-06 14:03:36.460379 blueshed_gust-0.0.3/PKG-INFO
+-rw-r--r--   0 peterb     (501) staff       (20)      320 2024-05-06 13:29:02.000000 blueshed_gust-0.0.3/README.md
+-rw-r--r--   0 peterb     (501) staff       (20)     1879 2024-05-06 14:03:33.000000 blueshed_gust-0.0.3/pyproject.toml
+-rw-r--r--   0 peterb     (501) staff       (20)       38 2024-05-06 14:03:36.460588 blueshed_gust-0.0.3/setup.cfg
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 14:03:36.457898 blueshed_gust-0.0.3/src/
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 14:03:36.457839 blueshed_gust-0.0.3/src/blueshed/
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 14:03:36.459246 blueshed_gust-0.0.3/src/blueshed/gust/
+-rw-r--r--   0 peterb     (501) staff       (20)      145 2024-05-06 14:03:33.000000 blueshed_gust-0.0.3/src/blueshed/gust/__init__.py
+-rw-r--r--   0 peterb     (501) staff       (20)      754 2024-05-06 10:00:21.000000 blueshed_gust-0.0.3/src/blueshed/gust/configs.py
+-rw-r--r--   0 peterb     (501) staff       (20)      590 2024-05-06 10:00:21.000000 blueshed_gust-0.0.3/src/blueshed/gust/context.py
+-rw-r--r--   0 peterb     (501) staff       (20)     1416 2024-05-06 10:00:21.000000 blueshed_gust-0.0.3/src/blueshed/gust/json_utils.py
+-rw-r--r--   0 peterb     (501) staff       (20)     2494 2024-05-06 13:33:43.000000 blueshed_gust-0.0.3/src/blueshed/gust/main.py
+-rw-r--r--   0 peterb     (501) staff       (20)     3829 2024-05-06 13:33:43.000000 blueshed_gust-0.0.3/src/blueshed/gust/routes.py
+-rw-r--r--   0 peterb     (501) staff       (20)      919 2024-05-06 10:00:21.000000 blueshed_gust-0.0.3/src/blueshed/gust/static_file_handler.py
+-rw-r--r--   0 peterb     (501) staff       (20)     2599 2024-05-06 13:33:43.000000 blueshed_gust-0.0.3/src/blueshed/gust/utils.py
+-rw-r--r--   0 peterb     (501) staff       (20)       67 2024-05-06 13:33:43.000000 blueshed_gust-0.0.3/src/blueshed/gust/web.py
+-rw-r--r--   0 peterb     (501) staff       (20)     2263 2024-05-06 10:00:21.000000 blueshed_gust-0.0.3/src/blueshed/gust/web_handler.py
+-rw-r--r--   0 peterb     (501) staff       (20)     5670 2024-05-06 10:28:00.000000 blueshed_gust-0.0.3/src/blueshed/gust/websocket.py
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 14:03:36.459881 blueshed_gust-0.0.3/src/blueshed_gust.egg-info/
+-rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-06 14:03:36.000000 blueshed_gust-0.0.3/src/blueshed_gust.egg-info/PKG-INFO
+-rw-r--r--   0 peterb     (501) staff       (20)      559 2024-05-06 14:03:36.000000 blueshed_gust-0.0.3/src/blueshed_gust.egg-info/SOURCES.txt
+-rw-r--r--   0 peterb     (501) staff       (20)        1 2024-05-06 14:03:36.000000 blueshed_gust-0.0.3/src/blueshed_gust.egg-info/dependency_links.txt
+-rw-r--r--   0 peterb     (501) staff       (20)      124 2024-05-06 14:03:36.000000 blueshed_gust-0.0.3/src/blueshed_gust.egg-info/requires.txt
+-rw-r--r--   0 peterb     (501) staff       (20)        9 2024-05-06 14:03:36.000000 blueshed_gust-0.0.3/src/blueshed_gust.egg-info/top_level.txt
```

### Comparing `blueshed_gust-0.0.1/PKG-INFO` & `blueshed_gust-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueshed-gust
-Version: 0.0.1
+Version: 0.0.3
 Summary: a library.
 Author-email: Peter Bunyan <pete@blueshed.co.uk>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
```

### Comparing `blueshed_gust-0.0.1/pyproject.toml` & `blueshed_gust-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,14 @@
 
 [tool.coverage.run]
 data_file = ".venv/cache/.coverage"
 [tool.coverage.report]
 data_file = ".venv/cache/.coverage"
 
 [tool.bumpversion]
-current_version = "0.0.1"
+current_version = "0.0.3"
 commit = false
 tag = true
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "src/blueshed/gust/__init__.py"
```

### Comparing `blueshed_gust-0.0.1/src/blueshed_gust.egg-info/PKG-INFO` & `blueshed_gust-0.0.3/src/blueshed_gust.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueshed-gust
-Version: 0.0.1
+Version: 0.0.3
 Summary: a library.
 Author-email: Peter Bunyan <pete@blueshed.co.uk>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
```

