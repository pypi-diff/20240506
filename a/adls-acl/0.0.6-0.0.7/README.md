# Comparing `tmp/adls_acl-0.0.6.tar.gz` & `tmp/adls_acl-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adls_acl-0.0.6.tar", last modified: Wed Apr 24 22:10:15 2024, max compression
+gzip compressed data, was "adls_acl-0.0.7.tar", last modified: Mon May  6 08:22:21 2024, max compression
```

## Comparing `adls_acl-0.0.6.tar` & `adls_acl-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:10:15.950793 adls_acl-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-24 22:10:10.000000 adls_acl-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 22:10:10.000000 adls_acl-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-04-24 22:10:15.950793 adls_acl-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-04-24 22:10:10.000000 adls_acl-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-24 22:10:10.000000 adls_acl-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 22:10:15.950793 adls_acl-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-24 22:10:10.000000 adls_acl-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:10:15.946793 adls_acl-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:10:15.946793 adls_acl-0.0.6/src/adls_acl/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 22:10:10.000000 adls_acl-0.0.6/src/adls_acl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-24 22:10:10.000000 adls_acl-0.0.6/src/adls_acl/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-24 22:10:10.000000 adls_acl-0.0.6/src/adls_acl/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-24 22:10:10.000000 adls_acl-0.0.6/src/adls_acl/input_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-24 22:10:10.000000 adls_acl-0.0.6/src/adls_acl/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-24 22:10:10.000000 adls_acl-0.0.6/src/adls_acl/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-04-24 22:10:10.000000 adls_acl-0.0.6/src/adls_acl/orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:10:15.946793 adls_acl-0.0.6/src/adls_acl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-04-24 22:10:15.000000 adls_acl-0.0.6/src/adls_acl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-24 22:10:15.000000 adls_acl-0.0.6/src/adls_acl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 22:10:15.000000 adls_acl-0.0.6/src/adls_acl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-24 22:10:15.000000 adls_acl-0.0.6/src/adls_acl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 22:10:15.000000 adls_acl-0.0.6/src/adls_acl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 22:10:15.000000 adls_acl-0.0.6/src/adls_acl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 22:10:15.946793 adls_acl-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 22:10:10.000000 adls_acl-0.0.6/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-04-24 22:10:10.000000 adls_acl-0.0.6/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-24 22:10:10.000000 adls_acl-0.0.6/tests/test_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:22:21.477711 adls_acl-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-06 08:22:09.000000 adls_acl-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-06 08:22:09.000000 adls_acl-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-05-06 08:22:21.477711 adls_acl-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-05-06 08:22:09.000000 adls_acl-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-06 08:22:09.000000 adls_acl-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:22:21.477711 adls_acl-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-06 08:22:09.000000 adls_acl-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:22:21.473711 adls_acl-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:22:21.477711 adls_acl-0.0.7/src/adls_acl/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 08:22:09.000000 adls_acl-0.0.7/src/adls_acl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-06 08:22:09.000000 adls_acl-0.0.7/src/adls_acl/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-06 08:22:09.000000 adls_acl-0.0.7/src/adls_acl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-06 08:22:09.000000 adls_acl-0.0.7/src/adls_acl/input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-06 08:22:09.000000 adls_acl-0.0.7/src/adls_acl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-05-06 08:22:09.000000 adls_acl-0.0.7/src/adls_acl/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-06 08:22:09.000000 adls_acl-0.0.7/src/adls_acl/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 08:22:09.000000 adls_acl-0.0.7/src/adls_acl/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:22:21.477711 adls_acl-0.0.7/src/adls_acl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-05-06 08:22:21.000000 adls_acl-0.0.7/src/adls_acl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-06 08:22:21.000000 adls_acl-0.0.7/src/adls_acl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:22:21.000000 adls_acl-0.0.7/src/adls_acl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-06 08:22:21.000000 adls_acl-0.0.7/src/adls_acl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 08:22:21.000000 adls_acl-0.0.7/src/adls_acl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 08:22:21.000000 adls_acl-0.0.7/src/adls_acl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:22:21.477711 adls_acl-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-06 08:22:09.000000 adls_acl-0.0.7/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-06 08:22:09.000000 adls_acl-0.0.7/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-06 08:22:09.000000 adls_acl-0.0.7/tests/test_orchestrator.py
```

### Comparing `adls_acl-0.0.6/LICENSE` & `adls_acl-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.6/PKG-INFO` & `adls_acl-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adls_acl
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small tool for managing Azure DataLake Store (ADLS) Access Control Lists (ACLs).
 Home-page: https://github.com/karolusz/adls-acl
 Author: Karol Luszczek
 Author-email: karol.luszczek@reinsight.se
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `adls_acl-0.0.6/README.md` & `adls_acl-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.6/pyproject.toml` & `adls_acl-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.bumpver]
-current_version = "0.0.6"
+current_version = "0.0.7"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `adls_acl-0.0.6/setup.py` & `adls_acl-0.0.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 readme = open("README.md", encoding="utf-8").read()
 
 setup(
     name="adls_acl",
-    version="0.0.6",
+    version="0.0.7",
     url="https://github.com/karolusz/adls-acl",
     author="Karol Luszczek",
     author_email="karol.luszczek@reinsight.se",
     description="A small tool for managing Azure DataLake Store (ADLS) Access Control Lists (ACLs).",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `adls_acl-0.0.6/src/adls_acl/auth.py` & `adls_acl-0.0.7/src/adls_acl/auth.py`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.6/src/adls_acl/cli.py` & `adls_acl-0.0.7/src/adls_acl/cli.py`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.6/src/adls_acl/input_parser.py` & `adls_acl-0.0.7/src/adls_acl/input_parser.py`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.6/src/adls_acl/logger.py` & `adls_acl-0.0.7/src/adls_acl/logger.py`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.6/src/adls_acl/nodes.py` & `adls_acl-0.0.7/src/adls_acl/nodes.py`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.6/src/adls_acl/orchestrator.py` & `adls_acl-0.0.7/src/adls_acl/orchestrator.py`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.6/src/adls_acl.egg-info/PKG-INFO` & `adls_acl-0.0.7/src/adls_acl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adls_acl
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small tool for managing Azure DataLake Store (ADLS) Access Control Lists (ACLs).
 Home-page: https://github.com/karolusz/adls-acl
 Author: Karol Luszczek
 Author-email: karol.luszczek@reinsight.se
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `adls_acl-0.0.6/tests/test_auth.py` & `adls_acl-0.0.7/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.6/tests/test_nodes.py` & `adls_acl-0.0.7/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `adls_acl-0.0.6/tests/test_orchestrator.py` & `adls_acl-0.0.7/tests/test_orchestrator.py`

 * *Files identical despite different names*

