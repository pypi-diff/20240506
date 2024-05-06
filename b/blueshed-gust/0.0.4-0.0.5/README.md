# Comparing `tmp/blueshed_gust-0.0.4.tar.gz` & `tmp/blueshed_gust-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueshed_gust-0.0.4.tar", last modified: Mon May  6 16:43:10 2024, max compression
+gzip compressed data, was "blueshed_gust-0.0.5.tar", last modified: Mon May  6 16:45:46 2024, max compression
```

## Comparing `blueshed_gust-0.0.4.tar` & `blueshed_gust-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:43:10.485919 blueshed_gust-0.0.4/
--rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-06 16:43:10.485739 blueshed_gust-0.0.4/PKG-INFO
--rw-r--r--   0 peterb     (501) staff       (20)      320 2024-05-06 13:29:02.000000 blueshed_gust-0.0.4/README.md
--rw-r--r--   0 peterb     (501) staff       (20)     1879 2024-05-06 16:43:04.000000 blueshed_gust-0.0.4/pyproject.toml
--rw-r--r--   0 peterb     (501) staff       (20)       38 2024-05-06 16:43:10.485955 blueshed_gust-0.0.4/setup.cfg
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:43:10.483008 blueshed_gust-0.0.4/src/
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:43:10.482949 blueshed_gust-0.0.4/src/blueshed/
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:43:10.484519 blueshed_gust-0.0.4/src/blueshed/gust/
--rw-r--r--   0 peterb     (501) staff       (20)      145 2024-05-06 16:43:04.000000 blueshed_gust-0.0.4/src/blueshed/gust/__init__.py
--rw-r--r--   0 peterb     (501) staff       (20)      754 2024-05-06 10:00:21.000000 blueshed_gust-0.0.4/src/blueshed/gust/configs.py
--rw-r--r--   0 peterb     (501) staff       (20)      590 2024-05-06 10:00:21.000000 blueshed_gust-0.0.4/src/blueshed/gust/context.py
--rw-r--r--   0 peterb     (501) staff       (20)     1416 2024-05-06 10:00:21.000000 blueshed_gust-0.0.4/src/blueshed/gust/json_utils.py
--rw-r--r--   0 peterb     (501) staff       (20)     2474 2024-05-06 16:40:48.000000 blueshed_gust-0.0.4/src/blueshed/gust/main.py
--rw-r--r--   0 peterb     (501) staff       (20)     3829 2024-05-06 14:08:50.000000 blueshed_gust-0.0.4/src/blueshed/gust/routes.py
--rw-r--r--   0 peterb     (501) staff       (20)      919 2024-05-06 10:00:21.000000 blueshed_gust-0.0.4/src/blueshed/gust/static_file_handler.py
--rw-r--r--   0 peterb     (501) staff       (20)     2599 2024-05-06 13:33:43.000000 blueshed_gust-0.0.4/src/blueshed/gust/utils.py
--rw-r--r--   0 peterb     (501) staff       (20)       67 2024-05-06 13:33:43.000000 blueshed_gust-0.0.4/src/blueshed/gust/web.py
--rw-r--r--   0 peterb     (501) staff       (20)     2263 2024-05-06 10:00:21.000000 blueshed_gust-0.0.4/src/blueshed/gust/web_handler.py
--rw-r--r--   0 peterb     (501) staff       (20)     5670 2024-05-06 10:28:00.000000 blueshed_gust-0.0.4/src/blueshed/gust/websocket.py
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:43:10.485216 blueshed_gust-0.0.4/src/blueshed_gust.egg-info/
--rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-06 16:43:10.000000 blueshed_gust-0.0.4/src/blueshed_gust.egg-info/PKG-INFO
--rw-r--r--   0 peterb     (501) staff       (20)      559 2024-05-06 16:43:10.000000 blueshed_gust-0.0.4/src/blueshed_gust.egg-info/SOURCES.txt
--rw-r--r--   0 peterb     (501) staff       (20)        1 2024-05-06 16:43:10.000000 blueshed_gust-0.0.4/src/blueshed_gust.egg-info/dependency_links.txt
--rw-r--r--   0 peterb     (501) staff       (20)      124 2024-05-06 16:43:10.000000 blueshed_gust-0.0.4/src/blueshed_gust.egg-info/requires.txt
--rw-r--r--   0 peterb     (501) staff       (20)        9 2024-05-06 16:43:10.000000 blueshed_gust-0.0.4/src/blueshed_gust.egg-info/top_level.txt
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:45:46.954635 blueshed_gust-0.0.5/
+-rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-06 16:45:46.954460 blueshed_gust-0.0.5/PKG-INFO
+-rw-r--r--   0 peterb     (501) staff       (20)      320 2024-05-06 13:29:02.000000 blueshed_gust-0.0.5/README.md
+-rw-r--r--   0 peterb     (501) staff       (20)     1879 2024-05-06 16:45:44.000000 blueshed_gust-0.0.5/pyproject.toml
+-rw-r--r--   0 peterb     (501) staff       (20)       38 2024-05-06 16:45:46.954670 blueshed_gust-0.0.5/setup.cfg
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:45:46.951951 blueshed_gust-0.0.5/src/
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:45:46.951892 blueshed_gust-0.0.5/src/blueshed/
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:45:46.953322 blueshed_gust-0.0.5/src/blueshed/gust/
+-rw-r--r--   0 peterb     (501) staff       (20)      145 2024-05-06 16:45:44.000000 blueshed_gust-0.0.5/src/blueshed/gust/__init__.py
+-rw-r--r--   0 peterb     (501) staff       (20)      754 2024-05-06 10:00:21.000000 blueshed_gust-0.0.5/src/blueshed/gust/configs.py
+-rw-r--r--   0 peterb     (501) staff       (20)      590 2024-05-06 10:00:21.000000 blueshed_gust-0.0.5/src/blueshed/gust/context.py
+-rw-r--r--   0 peterb     (501) staff       (20)     1416 2024-05-06 10:00:21.000000 blueshed_gust-0.0.5/src/blueshed/gust/json_utils.py
+-rw-r--r--   0 peterb     (501) staff       (20)     2428 2024-05-06 16:44:57.000000 blueshed_gust-0.0.5/src/blueshed/gust/main.py
+-rw-r--r--   0 peterb     (501) staff       (20)     3829 2024-05-06 14:08:50.000000 blueshed_gust-0.0.5/src/blueshed/gust/routes.py
+-rw-r--r--   0 peterb     (501) staff       (20)      919 2024-05-06 10:00:21.000000 blueshed_gust-0.0.5/src/blueshed/gust/static_file_handler.py
+-rw-r--r--   0 peterb     (501) staff       (20)     2599 2024-05-06 13:33:43.000000 blueshed_gust-0.0.5/src/blueshed/gust/utils.py
+-rw-r--r--   0 peterb     (501) staff       (20)       67 2024-05-06 13:33:43.000000 blueshed_gust-0.0.5/src/blueshed/gust/web.py
+-rw-r--r--   0 peterb     (501) staff       (20)     2263 2024-05-06 10:00:21.000000 blueshed_gust-0.0.5/src/blueshed/gust/web_handler.py
+-rw-r--r--   0 peterb     (501) staff       (20)     5670 2024-05-06 10:28:00.000000 blueshed_gust-0.0.5/src/blueshed/gust/websocket.py
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:45:46.953981 blueshed_gust-0.0.5/src/blueshed_gust.egg-info/
+-rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-06 16:45:46.000000 blueshed_gust-0.0.5/src/blueshed_gust.egg-info/PKG-INFO
+-rw-r--r--   0 peterb     (501) staff       (20)      559 2024-05-06 16:45:46.000000 blueshed_gust-0.0.5/src/blueshed_gust.egg-info/SOURCES.txt
+-rw-r--r--   0 peterb     (501) staff       (20)        1 2024-05-06 16:45:46.000000 blueshed_gust-0.0.5/src/blueshed_gust.egg-info/dependency_links.txt
+-rw-r--r--   0 peterb     (501) staff       (20)      124 2024-05-06 16:45:46.000000 blueshed_gust-0.0.5/src/blueshed_gust.egg-info/requires.txt
+-rw-r--r--   0 peterb     (501) staff       (20)        9 2024-05-06 16:45:46.000000 blueshed_gust-0.0.5/src/blueshed_gust.egg-info/top_level.txt
```

### Comparing `blueshed_gust-0.0.4/PKG-INFO` & `blueshed_gust-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueshed-gust
-Version: 0.0.4
+Version: 0.0.5
 Summary: a library.
 Author-email: Peter Bunyan <pete@blueshed.co.uk>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
```

### Comparing `blueshed_gust-0.0.4/pyproject.toml` & `blueshed_gust-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,14 @@
 
 [tool.coverage.run]
 data_file = ".venv/cache/.coverage"
 [tool.coverage.report]
 data_file = ".venv/cache/.coverage"
 
 [tool.bumpversion]
-current_version = "0.0.4"
+current_version = "0.0.5"
 commit = false
 tag = true
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "src/blueshed/gust/__init__.py"
```

### Comparing `blueshed_gust-0.0.4/src/blueshed/gust/configs.py` & `blueshed_gust-0.0.5/src/blueshed/gust/configs.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.4/src/blueshed/gust/context.py` & `blueshed_gust-0.0.5/src/blueshed/gust/context.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.4/src/blueshed/gust/json_utils.py` & `blueshed_gust-0.0.5/src/blueshed/gust/json_utils.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.4/src/blueshed/gust/main.py` & `blueshed_gust-0.0.5/src/blueshed/gust/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,11 +74,7 @@
 
     def run(self):  # pragma: no cover
         try:
             asyncio.run(self._run_())
         except (KeyboardInterrupt, SystemExit):
             # graceful shutdown
             pass
-
-
-if __name__ == "__main__":
-    Gust().run()
```

### Comparing `blueshed_gust-0.0.4/src/blueshed/gust/routes.py` & `blueshed_gust-0.0.5/src/blueshed/gust/routes.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.4/src/blueshed/gust/static_file_handler.py` & `blueshed_gust-0.0.5/src/blueshed/gust/static_file_handler.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.4/src/blueshed/gust/utils.py` & `blueshed_gust-0.0.5/src/blueshed/gust/utils.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.4/src/blueshed/gust/web_handler.py` & `blueshed_gust-0.0.5/src/blueshed/gust/web_handler.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.4/src/blueshed/gust/websocket.py` & `blueshed_gust-0.0.5/src/blueshed/gust/websocket.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.4/src/blueshed_gust.egg-info/PKG-INFO` & `blueshed_gust-0.0.5/src/blueshed_gust.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueshed-gust
-Version: 0.0.4
+Version: 0.0.5
 Summary: a library.
 Author-email: Peter Bunyan <pete@blueshed.co.uk>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
```

### Comparing `blueshed_gust-0.0.4/src/blueshed_gust.egg-info/SOURCES.txt` & `blueshed_gust-0.0.5/src/blueshed_gust.egg-info/SOURCES.txt`

 * *Files identical despite different names*

