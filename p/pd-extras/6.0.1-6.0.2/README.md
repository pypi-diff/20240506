# Comparing `tmp/pd_extras-6.0.1.tar.gz` & `tmp/pd_extras-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pd_extras-6.0.1.tar", max compression
+gzip compressed data, was "pd_extras-6.0.2.tar", max compression
```

## Comparing `pd_extras-6.0.1.tar` & `pd_extras-6.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2024-05-06 02:51:53.691577 pd_extras-6.0.1/LICENSE
--rw-r--r--   0        0        0     3093 2024-05-06 02:51:53.691577 pd_extras-6.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/check/__init__.py
--rw-r--r--   0        0        0     3245 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/check/sanitize.py
--rw-r--r--   0        0        0        0 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/extra/__init__.py
--rw-r--r--   0        0        0     3794 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/extra/flattener.py
--rw-r--r--   0        0        0     2635 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/extra/operations.py
--rw-r--r--   0        0        0        0 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/optimize/__init__.py
--rw-r--r--   0        0        0     1775 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/optimize/df_ops.py
--rw-r--r--   0        0        0        0 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/write/__init__.py
--rw-r--r--   0        0        0     1388 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/write/common.py
--rw-r--r--   0        0        0     5670 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/write/nosql_writer.py
--rw-r--r--   0        0        0     8955 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pd_extras/write/sql_writer.py
--rw-r--r--   0        0        0      729 2024-05-06 02:51:53.691577 pd_extras-6.0.1/pyproject.toml
--rw-r--r--   0        0        0     4116 1970-01-01 00:00:00.000000 pd_extras-6.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-06 03:21:21.517070 pd_extras-6.0.2/LICENSE
+-rw-r--r--   0        0        0     3093 2024-05-06 03:21:21.517070 pd_extras-6.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 03:21:21.521070 pd_extras-6.0.2/pd_extras/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 03:21:21.521070 pd_extras-6.0.2/pd_extras/check/__init__.py
+-rw-r--r--   0        0        0     3245 2024-05-06 03:21:21.521070 pd_extras-6.0.2/pd_extras/check/sanitize.py
+-rw-r--r--   0        0        0        0 2024-05-06 03:21:21.521070 pd_extras-6.0.2/pd_extras/extra/__init__.py
+-rw-r--r--   0        0        0     3794 2024-05-06 03:21:21.521070 pd_extras-6.0.2/pd_extras/extra/flattener.py
+-rw-r--r--   0        0        0     2635 2024-05-06 03:21:21.521070 pd_extras-6.0.2/pd_extras/extra/operations.py
+-rw-r--r--   0        0        0        0 2024-05-06 03:21:21.521070 pd_extras-6.0.2/pd_extras/optimize/__init__.py
+-rw-r--r--   0        0        0     1775 2024-05-06 03:21:21.521070 pd_extras-6.0.2/pd_extras/optimize/df_ops.py
+-rw-r--r--   0        0        0        0 2024-05-06 03:21:21.521070 pd_extras-6.0.2/pd_extras/write/__init__.py
+-rw-r--r--   0        0        0     1388 2024-05-06 03:21:21.521070 pd_extras-6.0.2/pd_extras/write/common.py
+-rw-r--r--   0        0        0     5670 2024-05-06 03:21:21.521070 pd_extras-6.0.2/pd_extras/write/nosql_writer.py
+-rw-r--r--   0        0        0     8955 2024-05-06 03:21:21.521070 pd_extras-6.0.2/pd_extras/write/sql_writer.py
+-rw-r--r--   0        0        0      729 2024-05-06 03:21:21.521070 pd_extras-6.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4116 1970-01-01 00:00:00.000000 pd_extras-6.0.2/PKG-INFO
```

### Comparing `pd_extras-6.0.1/LICENSE` & `pd_extras-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.1/README.md` & `pd_extras-6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.1/pd_extras/check/sanitize.py` & `pd_extras-6.0.2/pd_extras/check/sanitize.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.1/pd_extras/extra/flattener.py` & `pd_extras-6.0.2/pd_extras/extra/flattener.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.1/pd_extras/extra/operations.py` & `pd_extras-6.0.2/pd_extras/extra/operations.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.1/pd_extras/optimize/df_ops.py` & `pd_extras-6.0.2/pd_extras/optimize/df_ops.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.1/pd_extras/write/common.py` & `pd_extras-6.0.2/pd_extras/write/common.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.1/pd_extras/write/nosql_writer.py` & `pd_extras-6.0.2/pd_extras/write/nosql_writer.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.1/pd_extras/write/sql_writer.py` & `pd_extras-6.0.2/pd_extras/write/sql_writer.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.0.1/pyproject.toml` & `pd_extras-6.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pd-extras"
-version = "6.0.1"
+version = "6.0.2"
 description = "Some utility functions on top of pandas."
 authors = ["Masum Billal <billalmasum93@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/proafxin/pd-extras"
 documentation = "https://pd-extras.readthedocs.io/en/latest/"
```

### Comparing `pd_extras-6.0.1/PKG-INFO` & `pd_extras-6.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pd-extras
-Version: 6.0.1
+Version: 6.0.2
 Summary: Some utility functions on top of pandas.
 Home-page: https://github.com/proafxin/pd-extras
 License: MIT
 Author: Masum Billal
 Author-email: billalmasum93@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```
