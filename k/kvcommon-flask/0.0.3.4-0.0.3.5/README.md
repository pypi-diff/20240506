# Comparing `tmp/kvcommon_flask-0.0.3.4.tar.gz` & `tmp/kvcommon_flask-0.0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kvcommon_flask-0.0.3.4.tar", max compression
+gzip compressed data, was "kvcommon_flask-0.0.3.5.tar", max compression
```

## Comparing `kvcommon_flask-0.0.3.4.tar` & `kvcommon_flask-0.0.3.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2024-04-22 11:04:46.030532 kvcommon_flask-0.0.3.4/LICENSE
--rw-r--r--   0        0        0     1046 2024-04-22 11:04:46.030532 kvcommon_flask-0.0.3.4/README.md
--rw-r--r--   0        0        0     1233 2024-04-22 11:04:46.030532 kvcommon_flask-0.0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1212 2024-04-22 11:04:46.030532 kvcommon_flask-0.0.3.4/src/kvcommon_flask/context.py
--rw-r--r--   0        0        0      100 2024-04-22 11:04:46.030532 kvcommon_flask-0.0.3.4/src/kvcommon_flask/exceptions.py
--rw-r--r--   0        0        0      601 2024-04-22 11:04:46.030532 kvcommon_flask-0.0.3.4/src/kvcommon_flask/metrics/__init__.py
--rw-r--r--   0        0        0     1182 2024-04-22 11:04:46.030532 kvcommon_flask-0.0.3.4/src/kvcommon_flask/metrics/metrics.py
--rw-r--r--   0        0        0     1727 2024-04-22 11:04:46.034532 kvcommon_flask-0.0.3.4/src/kvcommon_flask/middleware.py
--rw-r--r--   0        0        0     2560 2024-04-22 11:04:46.034532 kvcommon_flask-0.0.3.4/src/kvcommon_flask/scheduler.py
--rw-r--r--   0        0        0      106 2024-04-22 11:04:46.034532 kvcommon_flask-0.0.3.4/src/kvcommon_flask/traces/__init__.py
--rw-r--r--   0        0        0      302 2024-04-22 11:04:46.034532 kvcommon_flask-0.0.3.4/src/kvcommon_flask/vars.py
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 kvcommon_flask-0.0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/LICENSE
+-rw-r--r--   0        0        0     1046 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/README.md
+-rw-r--r--   0        0        0     1233 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1212 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/src/kvcommon_flask/context.py
+-rw-r--r--   0        0        0      100 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/src/kvcommon_flask/exceptions.py
+-rw-r--r--   0        0        0      601 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/src/kvcommon_flask/metrics/__init__.py
+-rw-r--r--   0        0        0     1182 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/src/kvcommon_flask/metrics/metrics.py
+-rw-r--r--   0        0        0     1727 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/src/kvcommon_flask/middleware.py
+-rw-r--r--   0        0        0     2560 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/src/kvcommon_flask/scheduler.py
+-rw-r--r--   0        0        0      106 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/src/kvcommon_flask/traces/__init__.py
+-rw-r--r--   0        0        0      302 2024-05-06 20:48:27.002417 kvcommon_flask-0.0.3.5/src/kvcommon_flask/vars.py
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 kvcommon_flask-0.0.3.5/PKG-INFO
```

### Comparing `kvcommon_flask-0.0.3.4/LICENSE` & `kvcommon_flask-0.0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kvcommon_flask-0.0.3.4/README.md` & `kvcommon_flask-0.0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `kvcommon_flask-0.0.3.4/pyproject.toml` & `kvcommon_flask-0.0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kvcommon-flask"
-version = "0.0.3.4"
+version = "0.0.3.5"
 description = "Library of various Flask utils that aren't worthy of their own dedicated libs."
 authors = ["Rob Voigt <code@ravoigt.com>"]
 readme = "README.md"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kvcommon_flask-0.0.3.4/src/kvcommon_flask/context.py` & `kvcommon_flask-0.0.3.5/src/kvcommon_flask/context.py`

 * *Files identical despite different names*

### Comparing `kvcommon_flask-0.0.3.4/src/kvcommon_flask/metrics/__init__.py` & `kvcommon_flask-0.0.3.5/src/kvcommon_flask/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kvcommon_flask-0.0.3.4/src/kvcommon_flask/metrics/metrics.py` & `kvcommon_flask-0.0.3.5/src/kvcommon_flask/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `kvcommon_flask-0.0.3.4/src/kvcommon_flask/middleware.py` & `kvcommon_flask-0.0.3.5/src/kvcommon_flask/middleware.py`

 * *Files identical despite different names*

### Comparing `kvcommon_flask-0.0.3.4/src/kvcommon_flask/scheduler.py` & `kvcommon_flask-0.0.3.5/src/kvcommon_flask/scheduler.py`

 * *Files identical despite different names*

### Comparing `kvcommon_flask-0.0.3.4/PKG-INFO` & `kvcommon_flask-0.0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvcommon-flask
-Version: 0.0.3.4
+Version: 0.0.3.5
 Summary: Library of various Flask utils that aren't worthy of their own dedicated libs.
 Author: Rob Voigt
 Author-email: code@ravoigt.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

