# Comparing `tmp/pd_extras-5.0.5.tar.gz` & `tmp/pd_extras-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pd_extras-5.0.5.tar", max compression
+gzip compressed data, was "pd_extras-5.0.6.tar", max compression
```

## Comparing `pd_extras-5.0.5.tar` & `pd_extras-5.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2024-05-05 19:15:07.161022 pd_extras-5.0.5/LICENSE
--rw-r--r--   0        0        0     2845 2024-05-05 19:15:07.161022 pd_extras-5.0.5/README.md
--rw-r--r--   0        0        0        0 2024-05-05 19:15:07.161022 pd_extras-5.0.5/pd_extras/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 19:15:07.161022 pd_extras-5.0.5/pd_extras/check/__init__.py
--rw-r--r--   0        0        0     3245 2024-05-05 19:15:07.161022 pd_extras-5.0.5/pd_extras/check/sanitize.py
--rw-r--r--   0        0        0        0 2024-05-05 19:15:07.161022 pd_extras-5.0.5/pd_extras/extra/__init__.py
--rw-r--r--   0        0        0     3794 2024-05-05 19:15:07.161022 pd_extras-5.0.5/pd_extras/extra/flattener.py
--rw-r--r--   0        0        0     2635 2024-05-05 19:15:07.161022 pd_extras-5.0.5/pd_extras/extra/operations.py
--rw-r--r--   0        0        0        0 2024-05-05 19:15:07.165022 pd_extras-5.0.5/pd_extras/optimize/__init__.py
--rw-r--r--   0        0        0     1775 2024-05-05 19:15:07.165022 pd_extras-5.0.5/pd_extras/optimize/df_ops.py
--rw-r--r--   0        0        0        0 2024-05-05 19:15:07.165022 pd_extras-5.0.5/pd_extras/write/__init__.py
--rw-r--r--   0        0        0     1388 2024-05-05 19:15:07.165022 pd_extras-5.0.5/pd_extras/write/common.py
--rw-r--r--   0        0        0     5682 2024-05-05 19:15:07.165022 pd_extras-5.0.5/pd_extras/write/nosql_writer.py
--rw-r--r--   0        0        0     8962 2024-05-05 19:15:07.165022 pd_extras-5.0.5/pd_extras/write/sql_writer.py
--rw-r--r--   0        0        0      724 2024-05-05 19:15:07.165022 pd_extras-5.0.5/pyproject.toml
--rw-r--r--   0        0        0     3859 1970-01-01 00:00:00.000000 pd_extras-5.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-05 19:47:06.932467 pd_extras-5.0.6/LICENSE
+-rw-r--r--   0        0        0     2930 2024-05-05 19:47:06.932467 pd_extras-5.0.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/check/__init__.py
+-rw-r--r--   0        0        0     3245 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/check/sanitize.py
+-rw-r--r--   0        0        0        0 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/extra/__init__.py
+-rw-r--r--   0        0        0     3794 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/extra/flattener.py
+-rw-r--r--   0        0        0     2635 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/extra/operations.py
+-rw-r--r--   0        0        0        0 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/optimize/__init__.py
+-rw-r--r--   0        0        0     1775 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/optimize/df_ops.py
+-rw-r--r--   0        0        0        0 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/write/__init__.py
+-rw-r--r--   0        0        0     1388 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/write/common.py
+-rw-r--r--   0        0        0     5682 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/write/nosql_writer.py
+-rw-r--r--   0        0        0     8962 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pd_extras/write/sql_writer.py
+-rw-r--r--   0        0        0      724 2024-05-05 19:47:06.932467 pd_extras-5.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3944 1970-01-01 00:00:00.000000 pd_extras-5.0.6/PKG-INFO
```

### Comparing `pd_extras-5.0.5/LICENSE` & `pd_extras-5.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.5/README.md` & `pd_extras-5.0.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # Pandas Extras
 
 [![Code check, Test and Coverage, Build and deploy](https://github.com/proafxin/pd-extras/actions/workflows/build_deploy.yml/badge.svg)](https://github.com/proafxin/pd-extras/actions/workflows/build_deploy.yml)
 [![codecov](https://codecov.io/gh/proafxin/pd-extras/graph/badge.svg?token=AQA0IJY4N1)](https://codecov.io/gh/proafxin/pd-extras)
 [![Documentation Status](https://readthedocs.org/projects/pd-extras/badge/?version=latest)](https://pd-extras.readthedocs.io/en/latest/?badge=latest)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pd-extras)
-![PyPI - Version](https://img.shields.io/pypi/v/pd-extras)
-![PyPI - Format](https://img.shields.io/pypi/format/pd-extras)
-![PyPI - Implementation](https://img.shields.io/pypi/implementation/pd-extras)
-![Docker Image Version (tag)](https://img.shields.io/docker/v/_/postgres/latest?arch=amd64)
-![Docker Image Version (tag)](https://img.shields.io/docker/v/_/mysql/latest?arch=amd64)
+
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pd-extras?logo=python&logoColor=yellow&style=for-the-badge)
+![PyPI - Version](https://img.shields.io/pypi/v/pd-extras?logo=python&logoColor=yellow&style=for-the-badge)
+![Docker Image Version (tag)](https://img.shields.io/docker/v/_/postgres/latest?arch=amd64&style=for-the-badge&logo=postgresql&logoColor=white&label=Postgresql)
+![Docker Image Version (tag)](https://img.shields.io/docker/v/_/mysql/latest?arch=amd64&style=for-the-badge&logo=mysql&logoColor=white&label=mysql)
 
 Some functions on top of pandas.
 
 ## Install Environment
 
 For local development:
```

### Comparing `pd_extras-5.0.5/pd_extras/check/sanitize.py` & `pd_extras-5.0.6/pd_extras/check/sanitize.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.5/pd_extras/extra/flattener.py` & `pd_extras-5.0.6/pd_extras/extra/flattener.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.5/pd_extras/extra/operations.py` & `pd_extras-5.0.6/pd_extras/extra/operations.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.5/pd_extras/optimize/df_ops.py` & `pd_extras-5.0.6/pd_extras/optimize/df_ops.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.5/pd_extras/write/common.py` & `pd_extras-5.0.6/pd_extras/write/common.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.5/pd_extras/write/nosql_writer.py` & `pd_extras-5.0.6/pd_extras/write/nosql_writer.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.5/pd_extras/write/sql_writer.py` & `pd_extras-5.0.6/pd_extras/write/sql_writer.py`

 * *Files identical despite different names*

### Comparing `pd_extras-5.0.5/pyproject.toml` & `pd_extras-5.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pd-extras"
-version = "5.0.5"
+version = "5.0.6"
 description = "Some utility functions on top of pandas."
 authors = ["Masum Billal <billalmasum93@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/proafxin/pd-extras"
 documentation = "https://pd-extras.readthedocs.io/en/latest/"
```

### Comparing `pd_extras-5.0.5/PKG-INFO` & `pd_extras-5.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pd-extras
-Version: 5.0.5
+Version: 5.0.6
 Summary: Some utility functions on top of pandas.
 Home-page: https://github.com/proafxin/pd-extras
 License: MIT
 Author: Masum Billal
 Author-email: billalmasum93@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -25,20 +25,19 @@
 Description-Content-Type: text/markdown
 
 # Pandas Extras
 
 [![Code check, Test and Coverage, Build and deploy](https://github.com/proafxin/pd-extras/actions/workflows/build_deploy.yml/badge.svg)](https://github.com/proafxin/pd-extras/actions/workflows/build_deploy.yml)
 [![codecov](https://codecov.io/gh/proafxin/pd-extras/graph/badge.svg?token=AQA0IJY4N1)](https://codecov.io/gh/proafxin/pd-extras)
 [![Documentation Status](https://readthedocs.org/projects/pd-extras/badge/?version=latest)](https://pd-extras.readthedocs.io/en/latest/?badge=latest)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pd-extras)
-![PyPI - Version](https://img.shields.io/pypi/v/pd-extras)
-![PyPI - Format](https://img.shields.io/pypi/format/pd-extras)
-![PyPI - Implementation](https://img.shields.io/pypi/implementation/pd-extras)
-![Docker Image Version (tag)](https://img.shields.io/docker/v/_/postgres/latest?arch=amd64)
-![Docker Image Version (tag)](https://img.shields.io/docker/v/_/mysql/latest?arch=amd64)
+
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pd-extras?logo=python&logoColor=yellow&style=for-the-badge)
+![PyPI - Version](https://img.shields.io/pypi/v/pd-extras?logo=python&logoColor=yellow&style=for-the-badge)
+![Docker Image Version (tag)](https://img.shields.io/docker/v/_/postgres/latest?arch=amd64&style=for-the-badge&logo=postgresql&logoColor=white&label=Postgresql)
+![Docker Image Version (tag)](https://img.shields.io/docker/v/_/mysql/latest?arch=amd64&style=for-the-badge&logo=mysql&logoColor=white&label=mysql)
 
 Some functions on top of pandas.
 
 ## Install Environment
 
 For local development:
```

