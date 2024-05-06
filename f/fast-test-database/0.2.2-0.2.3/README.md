# Comparing `tmp/fast_test_database-0.2.2.tar.gz` & `tmp/fast_test_database-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_test_database-0.2.2.tar", max compression
+gzip compressed data, was "fast_test_database-0.2.3.tar", max compression
```

## Comparing `fast_test_database-0.2.2.tar` & `fast_test_database-0.2.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1121 2024-04-04 05:58:37.078868 fast_test_database-0.2.2/README.rst
--rw-r--r--   0        0        0     4341 2024-04-04 05:58:37.078868 fast_test_database-0.2.2/fast_test_database/__init__.py
--rw-r--r--   0        0        0      525 2024-04-04 05:59:13.051068 fast_test_database-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1676 1970-01-01 00:00:00.000000 fast_test_database-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1121 2024-05-06 21:19:23.112848 fast_test_database-0.2.3/README.rst
+-rw-r--r--   0        0        0     4341 2024-05-06 21:19:23.112848 fast_test_database-0.2.3/fast_test_database/__init__.py
+-rw-r--r--   0        0        0      525 2024-05-06 21:20:03.672668 fast_test_database-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1676 1970-01-01 00:00:00.000000 fast_test_database-0.2.3/PKG-INFO
```

### Comparing `fast_test_database-0.2.2/README.rst` & `fast_test_database-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `fast_test_database-0.2.2/fast_test_database/__init__.py` & `fast_test_database-0.2.3/fast_test_database/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_test_database-0.2.2/pyproject.toml` & `fast_test_database-0.2.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fast-test-database"
-version = "0.2.2"
+version = "0.2.3"
 description = "Configure an in-memory database for running Django tests"
 authors = ["Alexey Kotlyarov <a@koterpillar.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `fast_test_database-0.2.2/PKG-INFO` & `fast_test_database-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-test-database
-Version: 0.2.2
+Version: 0.2.3
 Summary: Configure an in-memory database for running Django tests
 License: GPL-3.0-or-later
 Author: Alexey Kotlyarov
 Author-email: a@koterpillar.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

