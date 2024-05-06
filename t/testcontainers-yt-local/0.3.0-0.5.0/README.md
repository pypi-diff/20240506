# Comparing `tmp/testcontainers_yt_local-0.3.0.tar.gz` & `tmp/testcontainers_yt_local-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testcontainers_yt_local-0.3.0.tar", last modified: Mon May  6 20:42:25 2024, max compression
+gzip compressed data, was "testcontainers_yt_local-0.5.0.tar", last modified: Mon May  6 20:55:30 2024, max compression
```

## Comparing `testcontainers_yt_local-0.3.0.tar` & `testcontainers_yt_local-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:42:25.641788 testcontainers_yt_local-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 20:42:08.000000 testcontainers_yt_local-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-06 20:42:25.641788 testcontainers_yt_local-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-06 20:42:08.000000 testcontainers_yt_local-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-06 20:42:17.000000 testcontainers_yt_local-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:42:25.641788 testcontainers_yt_local-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:42:25.637788 testcontainers_yt_local-0.3.0/testcontainers_yt_local/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 20:42:17.000000 testcontainers_yt_local-0.3.0/testcontainers_yt_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-06 20:42:08.000000 testcontainers_yt_local-0.3.0/testcontainers_yt_local/container.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:42:25.637788 testcontainers_yt_local-0.3.0/testcontainers_yt_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-06 20:42:25.000000 testcontainers_yt_local-0.3.0/testcontainers_yt_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-06 20:42:25.000000 testcontainers_yt_local-0.3.0/testcontainers_yt_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:42:25.000000 testcontainers_yt_local-0.3.0/testcontainers_yt_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-06 20:42:25.000000 testcontainers_yt_local-0.3.0/testcontainers_yt_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 20:42:25.000000 testcontainers_yt_local-0.3.0/testcontainers_yt_local.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:42:25.637788 testcontainers_yt_local-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-06 20:42:08.000000 testcontainers_yt_local-0.3.0/tests/test_yt_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:55:30.854424 testcontainers_yt_local-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 20:55:12.000000 testcontainers_yt_local-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-06 20:55:30.854424 testcontainers_yt_local-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-06 20:55:12.000000 testcontainers_yt_local-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-06 20:55:22.000000 testcontainers_yt_local-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:55:30.854424 testcontainers_yt_local-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:55:30.854424 testcontainers_yt_local-0.5.0/testcontainers_yt_local/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 20:55:22.000000 testcontainers_yt_local-0.5.0/testcontainers_yt_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-06 20:55:12.000000 testcontainers_yt_local-0.5.0/testcontainers_yt_local/container.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:55:30.854424 testcontainers_yt_local-0.5.0/testcontainers_yt_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-06 20:55:30.000000 testcontainers_yt_local-0.5.0/testcontainers_yt_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-06 20:55:30.000000 testcontainers_yt_local-0.5.0/testcontainers_yt_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:55:30.000000 testcontainers_yt_local-0.5.0/testcontainers_yt_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-06 20:55:30.000000 testcontainers_yt_local-0.5.0/testcontainers_yt_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 20:55:30.000000 testcontainers_yt_local-0.5.0/testcontainers_yt_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:55:30.854424 testcontainers_yt_local-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-06 20:55:12.000000 testcontainers_yt_local-0.5.0/tests/test_yt_local.py
```

### Comparing `testcontainers_yt_local-0.3.0/LICENSE` & `testcontainers_yt_local-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `testcontainers_yt_local-0.3.0/PKG-INFO` & `testcontainers_yt_local-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testcontainers-yt-local
-Version: 0.3.0
+Version: 0.5.0
 Summary: Testcontainer for Yt
 Author: Dmitriy Fedorov
 License: Apache 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: testcontainers<3.8
```

### Comparing `testcontainers_yt_local-0.3.0/pyproject.toml` & `testcontainers_yt_local-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 [tool.setuptools.packages.find]
 where = ["."]
 
 [tool.setuptools.dynamic]
 version = {attr = "testcontainers_yt_local.__version__"}
 
 [tool.bumpversion]
-current_version = "0.3.0"
+current_version = "0.5.0"
 commit = true
 commit_args = "--no-verify"
 tag = true
 tag_name = "{new_version}"
 message = "New version: {new_version} [changelog-ignore]"
 allow_dirty = true
```

### Comparing `testcontainers_yt_local-0.3.0/testcontainers_yt_local/container.py` & `testcontainers_yt_local-0.5.0/testcontainers_yt_local/container.py`

 * *Files identical despite different names*

### Comparing `testcontainers_yt_local-0.3.0/testcontainers_yt_local.egg-info/PKG-INFO` & `testcontainers_yt_local-0.5.0/testcontainers_yt_local.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testcontainers-yt-local
-Version: 0.3.0
+Version: 0.5.0
 Summary: Testcontainer for Yt
 Author: Dmitriy Fedorov
 License: Apache 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: testcontainers<3.8
```

### Comparing `testcontainers_yt_local-0.3.0/tests/test_yt_local.py` & `testcontainers_yt_local-0.5.0/tests/test_yt_local.py`

 * *Files identical despite different names*

