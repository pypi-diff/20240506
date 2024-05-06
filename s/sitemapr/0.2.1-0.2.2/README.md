# Comparing `tmp/sitemapr-0.2.1.tar.gz` & `tmp/sitemapr-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitemapr-0.2.1.tar", max compression
+gzip compressed data, was "sitemapr-0.2.2.tar", max compression
```

## Comparing `sitemapr-0.2.1.tar` & `sitemapr-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2024-03-15 03:45:40.662308 sitemapr-0.2.1/LICENSE
--rw-r--r--   0        0        0     2060 2024-03-15 03:45:40.662308 sitemapr-0.2.1/README.md
--rw-r--r--   0        0        0     1065 2024-03-15 03:45:40.662308 sitemapr-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      126 2024-03-15 03:45:40.662308 sitemapr-0.2.1/sitemapr/__init__.py
--rw-r--r--   0        0        0     4610 2024-03-15 03:45:40.662308 sitemapr-0.2.1/sitemapr/core.py
--rw-r--r--   0        0        0      741 2024-03-15 03:45:40.662308 sitemapr-0.2.1/sitemapr/models.py
--rw-r--r--   0        0        0     2642 1970-01-01 00:00:00.000000 sitemapr-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-06 05:15:34.752604 sitemapr-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2060 2024-05-06 05:15:34.752604 sitemapr-0.2.2/README.md
+-rw-r--r--   0        0        0     1065 2024-05-06 05:15:34.752604 sitemapr-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-05-06 05:15:34.752604 sitemapr-0.2.2/sitemapr/__init__.py
+-rw-r--r--   0        0        0     4610 2024-05-06 05:15:34.752604 sitemapr-0.2.2/sitemapr/core.py
+-rw-r--r--   0        0        0      741 2024-05-06 05:15:34.752604 sitemapr-0.2.2/sitemapr/models.py
+-rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 sitemapr-0.2.2/PKG-INFO
```

### Comparing `sitemapr-0.2.1/LICENSE` & `sitemapr-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sitemapr-0.2.1/README.md` & `sitemapr-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sitemapr-0.2.1/pyproject.toml` & `sitemapr-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "sitemapr"
-version = "0.2.1"
+version = "0.2.2"
 description = "sitemapr is a library that generates sitemaps for SPA websites with declaritve configuration in Python."
 authors = ["sjquant <seonujang92@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 typer = "^0.9.0"
 pydantic = "^2.6.3"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.2.2"
 pyright = "^1.1.351"
 pytest = "^8.0.2"
```

### Comparing `sitemapr-0.2.1/sitemapr/core.py` & `sitemapr-0.2.2/sitemapr/core.py`

 * *Files identical despite different names*

### Comparing `sitemapr-0.2.1/sitemapr/models.py` & `sitemapr-0.2.2/sitemapr/models.py`

 * *Files identical despite different names*

### Comparing `sitemapr-0.2.1/PKG-INFO` & `sitemapr-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: sitemapr
-Version: 0.2.1
+Version: 0.2.2
 Summary: sitemapr is a library that generates sitemaps for SPA websites with declaritve configuration in Python.
 License: MIT
 Author: sjquant
 Author-email: seonujang92@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # sitemapr
```

