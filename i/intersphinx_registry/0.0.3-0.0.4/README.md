# Comparing `tmp/intersphinx_registry-0.0.3.tar.gz` & `tmp/intersphinx_registry-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intersphinx_registry-0.0.3.tar", last modified: Fri May  3 15:36:37 2024, max compression
+gzip compressed data, was "intersphinx_registry-0.0.4.tar", last modified: Mon May  6 08:28:29 2024, max compression
```

## Comparing `intersphinx_registry-0.0.3.tar` & `intersphinx_registry-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      698 2024-05-03 15:35:42.574589 intersphinx_registry-0.0.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0        6 2024-05-03 12:40:56.982097 intersphinx_registry-0.0.3/.gitignore
--rw-r--r--   0        0        0     1086 2024-05-03 07:52:01.783580 intersphinx_registry-0.0.3/LICENSE
--rw-r--r--   0        0        0      975 2024-05-03 09:31:21.573054 intersphinx_registry-0.0.3/README.md
--rw-r--r--   0        0        0     1278 2024-05-03 15:35:49.106561 intersphinx_registry-0.0.3/intersphinx_registry/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 07:55:04.206909 intersphinx_registry-0.0.3/intersphinx_registry/py.typed
--rw-r--r--   0        0        0     9834 2024-05-03 15:35:42.575441 intersphinx_registry-0.0.3/intersphinx_registry/registry.json
--rw-r--r--   0        0        0      637 2024-05-03 13:38:36.749859 intersphinx_registry-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      884 2024-05-03 15:35:42.576100 intersphinx_registry-0.0.3/tests/test_basic.py
--rw-r--r--   0        0        0     1514 1970-01-01 00:00:00.000000 intersphinx_registry-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      698 2024-05-03 15:35:42.574589 intersphinx_registry-0.0.4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0        6 2024-05-03 12:40:56.982097 intersphinx_registry-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1086 2024-05-03 07:52:01.783580 intersphinx_registry-0.0.4/LICENSE
+-rw-r--r--   0        0        0      975 2024-05-03 09:31:21.573054 intersphinx_registry-0.0.4/README.md
+-rw-r--r--   0        0        0     1328 2024-05-06 08:27:56.979465 intersphinx_registry-0.0.4/intersphinx_registry/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 07:55:04.206909 intersphinx_registry-0.0.4/intersphinx_registry/py.typed
+-rw-r--r--   0        0        0     9824 2024-05-06 08:27:56.974573 intersphinx_registry-0.0.4/intersphinx_registry/registry.json
+-rw-r--r--   0        0        0      637 2024-05-03 13:38:36.749859 intersphinx_registry-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      884 2024-05-03 15:35:42.576100 intersphinx_registry-0.0.4/tests/test_basic.py
+-rw-r--r--   0        0        0     1514 1970-01-01 00:00:00.000000 intersphinx_registry-0.0.4/PKG-INFO
```

### Comparing `intersphinx_registry-0.0.3/.github/workflows/tests.yml` & `intersphinx_registry-0.0.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `intersphinx_registry-0.0.3/LICENSE` & `intersphinx_registry-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `intersphinx_registry-0.0.3/README.md` & `intersphinx_registry-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `intersphinx_registry-0.0.3/intersphinx_registry/__init__.py` & `intersphinx_registry-0.0.4/intersphinx_registry/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 from __future__ import annotations
 
 from pathlib import Path
 import json
 from typing import Dict, Tuple, Set, Optional, cast
 
-__version__ = "0.0.3"
+# I'm thinking of going YEAR.month.releasenumber
+
+__version__ = "0.0.4"
 
 registry_file = Path(__file__).parent / "registry.json"
 
 
 def get_intersphinx_mapping(
     *, only: Optional[Set[str]] = None
 ) -> Dict[str, Tuple[str, Optional[str]]]:
```

### Comparing `intersphinx_registry-0.0.3/intersphinx_registry/registry.json` & `intersphinx_registry-0.0.4/intersphinx_registry/registry.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978213507625273%*

 * *Differences: {"'scipy'": "{insert: [(0, 'https://docs.scipy.org/doc/scipy/')], delete: [0]}"}*

```diff
@@ -480,15 +480,15 @@
         null
     ],
     "scanpy": [
         "https://scanpy.readthedocs.io/en/stable/",
         null
     ],
     "scipy": [
-        "https://docs.scipy.org/doc/scipy/reference/",
+        "https://docs.scipy.org/doc/scipy/",
         null
     ],
     "scipy-lecture-notes": [
         "https://scipy-lectures.org/",
         null
     ],
     "scriptconfig": [
```

### Comparing `intersphinx_registry-0.0.3/pyproject.toml` & `intersphinx_registry-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `intersphinx_registry-0.0.3/tests/test_basic.py` & `intersphinx_registry-0.0.4/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `intersphinx_registry-0.0.3/PKG-INFO` & `intersphinx_registry-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intersphinx_registry
-Version: 0.0.3
+Version: 0.0.4
 Summary: This package provides convenient utilities and data to write a sphinx config file.
 Author-email: Matthias Bussonnier <bussonniermatthias@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pytest>=7.0 ; extra == "tests"
 Requires-Dist: pytest-xdist ; extra == "tests"
 Requires-Dist: requests ; extra == "tests"
```

