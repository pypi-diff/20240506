# Comparing `tmp/pathurl-0.7.0.tar.gz` & `tmp/pathurl-0.7.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathurl-0.7.0.tar", max compression
+gzip compressed data, was "pathurl-0.7.0.post1.tar", max compression
```

## Comparing `pathurl-0.7.0.tar` & `pathurl-0.7.0.post1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7696 2024-05-02 20:57:25.591775 pathurl-0.7.0/LICENSE.md
--rw-r--r--   0        0        0     1467 2024-05-03 10:22:04.659219 pathurl-0.7.0/docs/README.md
--rw-r--r--   0        0        0     2927 2024-05-03 11:00:42.727304 pathurl-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      126 2023-11-13 14:40:49.702634 pathurl-0.7.0/src/pathurl/__init__.py
--rw-r--r--   0        0        0      458 2023-11-13 14:40:49.702634 pathurl-0.7.0/src/pathurl/_constants.py
--rw-r--r--   0        0        0     1250 2023-11-13 14:40:49.702634 pathurl-0.7.0/src/pathurl/path.py
--rw-r--r--   0        0        0        0 2023-11-13 14:40:49.702634 pathurl-0.7.0/src/pathurl/py.typed
--rw-r--r--   0        0        0     3028 2024-05-02 20:57:25.595108 pathurl-0.7.0/src/pathurl/query.py
--rw-r--r--   0        0        0     3960 2024-05-02 20:57:25.595108 pathurl-0.7.0/src/pathurl/url.py
--rw-r--r--   0        0        0     2372 1970-01-01 00:00:00.000000 pathurl-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     7696 2024-05-02 20:57:25.591775 pathurl-0.7.0.post1/LICENSE.md
+-rw-r--r--   0        0        0     1615 2024-05-06 20:07:01.382152 pathurl-0.7.0.post1/docs/README.md
+-rw-r--r--   0        0        0     2933 2024-05-06 21:29:37.117060 pathurl-0.7.0.post1/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-11-13 14:40:49.702634 pathurl-0.7.0.post1/src/pathurl/__init__.py
+-rw-r--r--   0        0        0      458 2024-05-06 19:42:35.493117 pathurl-0.7.0.post1/src/pathurl/_constants.py
+-rw-r--r--   0        0        0     1250 2023-11-13 14:40:49.702634 pathurl-0.7.0.post1/src/pathurl/path.py
+-rw-r--r--   0        0        0        0 2023-11-13 14:40:49.702634 pathurl-0.7.0.post1/src/pathurl/py.typed
+-rw-r--r--   0        0        0     3028 2024-05-02 20:57:25.595108 pathurl-0.7.0.post1/src/pathurl/query.py
+-rw-r--r--   0        0        0     3960 2024-05-02 20:57:25.595108 pathurl-0.7.0.post1/src/pathurl/url.py
+-rw-r--r--   0        0        0     2526 1970-01-01 00:00:00.000000 pathurl-0.7.0.post1/PKG-INFO
```

### Comparing `pathurl-0.7.0/LICENSE.md` & `pathurl-0.7.0.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pathurl-0.7.0/docs/README.md` & `pathurl-0.7.0.post1/docs/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 [![license][licence_badge]][licence_url]
 [![pypi][pypi_badge]][pypi_url]
 [![downloads][pepy_badge]][pepy_url]
 [![code style: black][black_badge]][black_url]
 [![build automation: yam][yam_badge]][yam_url]
 [![Lint: ruff][ruff_badge]][ruff_url]
 
-`pathurl` is an objected-oriented way of manipulating URLs.
+`pathurl` is an objected-oriented way of manipulating URLs. It is heavily inspired by
+the improvements that were brought to the standard library by `pathlib` and aims to provide
+a similar interface for URLs.
 
 ## Links
 
 -   [Documentation]
 -   [Changelog]
 
 [test_badge]: https://github.com/spapanik/pathurl/actions/workflows/tests.yml/badge.svg
```

### Comparing `pathurl-0.7.0/pyproject.toml` & `pathurl-0.7.0.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "pathurl"
-version = "0.7.0"
+version = "0.7.0.post1"
 description = "url manipulation"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "docs/README.md"
```

### Comparing `pathurl-0.7.0/src/pathurl/path.py` & `pathurl-0.7.0.post1/src/pathurl/path.py`

 * *Files identical despite different names*

### Comparing `pathurl-0.7.0/src/pathurl/query.py` & `pathurl-0.7.0.post1/src/pathurl/query.py`

 * *Files identical despite different names*

### Comparing `pathurl-0.7.0/src/pathurl/url.py` & `pathurl-0.7.0.post1/src/pathurl/url.py`

 * *Files identical despite different names*

### Comparing `pathurl-0.7.0/PKG-INFO` & `pathurl-0.7.0.post1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathurl
-Version: 0.7.0
+Version: 0.7.0.post1
 Summary: url manipulation
 Home-page: https://pathurl.readthedocs.io/en/stable/
 License: LGPL-3.0+
 Keywords: url
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
 Requires-Python: >=3.8,<4.0
@@ -27,15 +27,17 @@
 [![license][licence_badge]][licence_url]
 [![pypi][pypi_badge]][pypi_url]
 [![downloads][pepy_badge]][pepy_url]
 [![code style: black][black_badge]][black_url]
 [![build automation: yam][yam_badge]][yam_url]
 [![Lint: ruff][ruff_badge]][ruff_url]
 
-`pathurl` is an objected-oriented way of manipulating URLs.
+`pathurl` is an objected-oriented way of manipulating URLs. It is heavily inspired by
+the improvements that were brought to the standard library by `pathlib` and aims to provide
+a similar interface for URLs.
 
 ## Links
 
 -   [Documentation]
 -   [Changelog]
 
 [test_badge]: https://github.com/spapanik/pathurl/actions/workflows/tests.yml/badge.svg
```

