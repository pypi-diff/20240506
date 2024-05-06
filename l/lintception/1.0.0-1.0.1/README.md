# Comparing `tmp/lintception-1.0.0.tar.gz` & `tmp/lintception-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lintception-1.0.0.tar", last modified: Fri May  3 20:48:08 2024, max compression
+gzip compressed data, was "lintception-1.0.1.tar", last modified: Mon May  6 04:48:02 2024, max compression
```

## Comparing `lintception-1.0.0.tar` & `lintception-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:48:08.351182 lintception-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-03 20:48:04.000000 lintception-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-03 20:48:08.351182 lintception-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-03 20:48:04.000000 lintception-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:48:08.347182 lintception-1.0.0/lintception/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:48:04.000000 lintception-1.0.0/lintception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-03 20:48:04.000000 lintception-1.0.0/lintception/linters.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-03 20:48:04.000000 lintception-1.0.0/lintception/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-03 20:48:04.000000 lintception-1.0.0/lintception/my_linter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:48:08.351182 lintception-1.0.0/lintception.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-03 20:48:08.000000 lintception-1.0.0/lintception.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-03 20:48:08.000000 lintception-1.0.0/lintception.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:48:08.000000 lintception-1.0.0/lintception.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 20:48:08.000000 lintception-1.0.0/lintception.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 20:48:08.000000 lintception-1.0.0/lintception.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-03 20:48:08.000000 lintception-1.0.0/lintception.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-03 20:48:04.000000 lintception-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:48:08.351182 lintception-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:48:02.834377 lintception-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-06 04:47:58.000000 lintception-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-06 04:48:02.834377 lintception-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-06 04:47:58.000000 lintception-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:48:02.830377 lintception-1.0.1/lintception/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-06 04:47:58.000000 lintception-1.0.1/lintception/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 04:47:58.000000 lintception-1.0.1/lintception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-06 04:47:58.000000 lintception-1.0.1/lintception/linters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-06 04:47:58.000000 lintception-1.0.1/lintception/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-06 04:47:58.000000 lintception-1.0.1/lintception/my_linter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:48:02.834377 lintception-1.0.1/lintception.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-06 04:48:02.000000 lintception-1.0.1/lintception.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-06 04:48:02.000000 lintception-1.0.1/lintception.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 04:48:02.000000 lintception-1.0.1/lintception.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 04:48:02.000000 lintception-1.0.1/lintception.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-06 04:48:02.000000 lintception-1.0.1/lintception.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 04:48:02.000000 lintception-1.0.1/lintception.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-06 04:47:58.000000 lintception-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 04:48:02.834377 lintception-1.0.1/setup.cfg
```

### Comparing `lintception-1.0.0/LICENSE` & `lintception-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lintception-1.0.0/PKG-INFO` & `lintception-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lintception
-Version: 1.0.0
+Version: 1.0.1
 Summary: Runs a few popular linters in series (mypy, vulture, vermin), and also does some other checks.
 Author-email: John Doknjas <jdoknjas@sfu.ca>
 Project-URL: Homepage, https://github.com/johndoknjas/lintception
 Keywords: linter,mypy,vulture,vermin,testing,linting,lintception
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `lintception-1.0.0/lintception/my_linter.py` & `lintception-1.0.1/lintception/my_linter.py`

 * *Files identical despite different names*

### Comparing `lintception-1.0.0/lintception.egg-info/PKG-INFO` & `lintception-1.0.1/lintception.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lintception
-Version: 1.0.0
+Version: 1.0.1
 Summary: Runs a few popular linters in series (mypy, vulture, vermin), and also does some other checks.
 Author-email: John Doknjas <jdoknjas@sfu.ca>
 Project-URL: Homepage, https://github.com/johndoknjas/lintception
 Keywords: linter,mypy,vulture,vermin,testing,linting,lintception
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `lintception-1.0.0/pyproject.toml` & `lintception-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 requires-python = ">= 3.8"
 name = "lintception"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="John Doknjas", email="jdoknjas@sfu.ca" },
 ]
 description = "Runs a few popular linters in series (mypy, vulture, vermin), and also does some other checks."
 keywords = ["linter", "mypy", "vulture", "vermin", "testing", "linting", "lintception"]
 dependencies = [
   "mypy",
```

