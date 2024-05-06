# Comparing `tmp/python_json_patch_rules-0.2.0.tar.gz` & `tmp/python_json_patch_rules-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_json_patch_rules-0.2.0.tar", last modified: Fri May  3 00:54:40 2024, max compression
+gzip compressed data, was "python_json_patch_rules-0.3.0.tar", last modified: Sun May  5 12:26:30 2024, max compression
```

## Comparing `python_json_patch_rules-0.2.0.tar` & `python_json_patch_rules-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 bagutoli   (503) staff       (20)        0 2024-05-03 00:54:40.188796 python_json_patch_rules-0.2.0/
--rw-r--r--   0 bagutoli   (503) staff       (20)     1069 2024-05-02 14:21:33.000000 python_json_patch_rules-0.2.0/LICENSE
--rw-r--r--   0 bagutoli   (503) staff       (20)     4967 2024-05-03 00:54:40.187038 python_json_patch_rules-0.2.0/PKG-INFO
--rw-r--r--   0 bagutoli   (503) staff       (20)     4438 2024-05-02 14:20:35.000000 python_json_patch_rules-0.2.0/README.md
-drwxr-xr-x   0 bagutoli   (503) staff       (20)        0 2024-05-03 00:54:40.096470 python_json_patch_rules-0.2.0/json_patch_rules/
--rw-r--r--   0 bagutoli   (503) staff       (20)     6926 2024-05-03 00:46:44.000000 python_json_patch_rules-0.2.0/json_patch_rules/__init__.py
--rw-r--r--   0 bagutoli   (503) staff       (20)      382 2024-05-02 14:27:47.000000 python_json_patch_rules-0.2.0/pyproject.toml
-drwxr-xr-x   0 bagutoli   (503) staff       (20)        0 2024-05-03 00:54:40.185219 python_json_patch_rules-0.2.0/python_json_patch_rules.egg-info/
--rw-r--r--   0 bagutoli   (503) staff       (20)     4967 2024-05-03 00:54:39.000000 python_json_patch_rules-0.2.0/python_json_patch_rules.egg-info/PKG-INFO
--rw-r--r--   0 bagutoli   (503) staff       (20)      380 2024-05-03 00:54:39.000000 python_json_patch_rules-0.2.0/python_json_patch_rules.egg-info/SOURCES.txt
--rw-r--r--   0 bagutoli   (503) staff       (20)        1 2024-05-03 00:54:39.000000 python_json_patch_rules-0.2.0/python_json_patch_rules.egg-info/dependency_links.txt
--rw-r--r--   0 bagutoli   (503) staff       (20)        7 2024-05-03 00:54:39.000000 python_json_patch_rules-0.2.0/python_json_patch_rules.egg-info/requires.txt
--rw-r--r--   0 bagutoli   (503) staff       (20)       23 2024-05-03 00:54:39.000000 python_json_patch_rules-0.2.0/python_json_patch_rules.egg-info/top_level.txt
--rw-r--r--   0 bagutoli   (503) staff       (20)      553 2024-05-03 00:54:40.191442 python_json_patch_rules-0.2.0/setup.cfg
--rw-r--r--   0 bagutoli   (503) staff       (20)     1281 2024-05-03 00:54:20.000000 python_json_patch_rules-0.2.0/setup.py
-drwxr-xr-x   0 bagutoli   (503) staff       (20)        0 2024-05-03 00:54:40.178747 python_json_patch_rules-0.2.0/tests/
--rw-r--r--   0 bagutoli   (503) staff       (20)        0 2024-05-02 12:17:58.000000 python_json_patch_rules-0.2.0/tests/__init__.py
--rw-r--r--   0 bagutoli   (503) staff       (20)     3004 2024-05-03 00:39:01.000000 python_json_patch_rules-0.2.0/tests/test_module.py
+drwxr-xr-x   0 bagutoli   (503) staff       (20)        0 2024-05-05 12:26:30.355584 python_json_patch_rules-0.3.0/
+-rw-r--r--   0 bagutoli   (503) staff       (20)     1069 2024-05-02 14:21:33.000000 python_json_patch_rules-0.3.0/LICENSE
+-rw-r--r--   0 bagutoli   (503) staff       (20)     8898 2024-05-05 12:26:30.349603 python_json_patch_rules-0.3.0/PKG-INFO
+-rw-r--r--   0 bagutoli   (503) staff       (20)     8369 2024-05-05 12:18:46.000000 python_json_patch_rules-0.3.0/README.md
+drwxr-xr-x   0 bagutoli   (503) staff       (20)        0 2024-05-05 12:26:30.305641 python_json_patch_rules-0.3.0/json_patch_rules/
+-rw-r--r--   0 bagutoli   (503) staff       (20)     6382 2024-05-05 12:20:20.000000 python_json_patch_rules-0.3.0/json_patch_rules/__init__.py
+-rw-r--r--   0 bagutoli   (503) staff       (20)      482 2024-05-05 12:18:46.000000 python_json_patch_rules-0.3.0/json_patch_rules/__symbols__.py
+-rw-r--r--   0 bagutoli   (503) staff       (20)      519 2024-05-03 15:38:44.000000 python_json_patch_rules-0.3.0/json_patch_rules/paths.py
+-rw-r--r--   0 bagutoli   (503) staff       (20)      382 2024-05-02 14:27:47.000000 python_json_patch_rules-0.3.0/pyproject.toml
+drwxr-xr-x   0 bagutoli   (503) staff       (20)        0 2024-05-05 12:26:30.346382 python_json_patch_rules-0.3.0/python_json_patch_rules.egg-info/
+-rw-r--r--   0 bagutoli   (503) staff       (20)     8898 2024-05-05 12:26:30.000000 python_json_patch_rules-0.3.0/python_json_patch_rules.egg-info/PKG-INFO
+-rw-r--r--   0 bagutoli   (503) staff       (20)      442 2024-05-05 12:26:30.000000 python_json_patch_rules-0.3.0/python_json_patch_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 bagutoli   (503) staff       (20)        1 2024-05-05 12:26:30.000000 python_json_patch_rules-0.3.0/python_json_patch_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 bagutoli   (503) staff       (20)        7 2024-05-05 12:26:30.000000 python_json_patch_rules-0.3.0/python_json_patch_rules.egg-info/requires.txt
+-rw-r--r--   0 bagutoli   (503) staff       (20)       23 2024-05-05 12:26:30.000000 python_json_patch_rules-0.3.0/python_json_patch_rules.egg-info/top_level.txt
+-rw-r--r--   0 bagutoli   (503) staff       (20)      553 2024-05-05 12:26:30.357610 python_json_patch_rules-0.3.0/setup.cfg
+-rw-r--r--   0 bagutoli   (503) staff       (20)     1281 2024-05-05 12:26:01.000000 python_json_patch_rules-0.3.0/setup.py
+drwxr-xr-x   0 bagutoli   (503) staff       (20)        0 2024-05-05 12:26:30.340991 python_json_patch_rules-0.3.0/tests/
+-rw-r--r--   0 bagutoli   (503) staff       (20)        0 2024-05-02 12:17:58.000000 python_json_patch_rules-0.3.0/tests/__init__.py
+-rw-r--r--   0 bagutoli   (503) staff       (20)    11219 2024-05-05 12:19:55.000000 python_json_patch_rules-0.3.0/tests/test_module.py
```

### Comparing `python_json_patch_rules-0.2.0/LICENSE` & `python_json_patch_rules-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_json_patch_rules-0.2.0/setup.cfg` & `python_json_patch_rules-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-json-patch-rules
-version = 0.2.0
+version = 0.3.0
 author = Bruno Agutoli
 author_email = bruno.agutoli@gmail.com
 description = A library to apply JSON patches with rule-based access control.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/agutoli/python-json-patch-rules
 license = MIT
```

### Comparing `python_json_patch_rules-0.2.0/setup.py` & `python_json_patch_rules-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="python-json-patch-rules",
-    version="0.2.0",
+    version="0.3.0",
     author="Bruno Agutoli",
     author_email="bruno.agutoli@gmail.com",
     description="A library to apply JSON patches with rule-based access control.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/agutoli/python-json-patch-rules",
     # Correct the package_dir to point to 'json_patch_rules' since your actual package code is there
```

