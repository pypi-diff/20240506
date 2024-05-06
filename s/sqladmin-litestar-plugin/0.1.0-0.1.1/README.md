# Comparing `tmp/sqladmin_litestar_plugin-0.1.0.tar.gz` & `tmp/sqladmin_litestar_plugin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqladmin_litestar_plugin-0.1.0.tar", max compression
+gzip compressed data, was "sqladmin_litestar_plugin-0.1.1.tar", max compression
```

## Comparing `sqladmin_litestar_plugin-0.1.0.tar` & `sqladmin_litestar_plugin-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     2426 2024-04-28 08:14:27.086983 sqladmin_litestar_plugin-0.1.0/README.md
--rw-r--r--   0        0        0     4225 2024-04-28 08:14:27.086983 sqladmin_litestar_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4859 2024-04-28 08:14:27.086983 sqladmin_litestar_plugin-0.1.0/src/sqladmin_litestar_plugin/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 08:14:27.086983 sqladmin_litestar_plugin-0.1.0/src/sqladmin_litestar_plugin/py.typed
--rw-r--r--   0        0        0     3014 1970-01-01 00:00:00.000000 sqladmin_litestar_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-05-06 09:28:14.370864 sqladmin_litestar_plugin-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2497 2024-05-06 09:28:14.370864 sqladmin_litestar_plugin-0.1.1/README.md
+-rw-r--r--   0        0        0     4225 2024-05-06 09:28:14.370864 sqladmin_litestar_plugin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5718 2024-05-06 09:28:14.370864 sqladmin_litestar_plugin-0.1.1/src/sqladmin_litestar_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 09:28:14.370864 sqladmin_litestar_plugin-0.1.1/src/sqladmin_litestar_plugin/py.typed
+-rw-r--r--   0        0        0     3085 1970-01-01 00:00:00.000000 sqladmin_litestar_plugin-0.1.1/PKG-INFO
```

### Comparing `sqladmin_litestar_plugin-0.1.0/README.md` & `sqladmin_litestar_plugin-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 pip install sqladmin-litestar-plugin
 ```
 
 ## Usage
 
 To use the plugin, import the `SQLAdminPlugin` class and pass it to the `Litestar` application.
 
+By default, the plugin will create a new admin interface at `/admin`.
+
 ### Example
 
 ```python
 from litestar import Litestar
 from sqladmin import ModelView
 from sqladmin_litestar_plugin import SQLAdminPlugin
 from sqlalchemy import Column, Integer, String
```

### Comparing `sqladmin_litestar_plugin-0.1.0/pyproject.toml` & `sqladmin_litestar_plugin-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqladmin-litestar-plugin"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Peter Schutt <peter.github@proton.me>"]
 readme = "README.md"
 packages = [
     { include = "sqladmin_litestar_plugin", from = "src" },
 ]
```

### Comparing `sqladmin_litestar_plugin-0.1.0/PKG-INFO` & `sqladmin_litestar_plugin-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqladmin-litestar-plugin
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Peter Schutt
 Author-email: peter.github@proton.me
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -30,14 +30,16 @@
 pip install sqladmin-litestar-plugin
 ```
 
 ## Usage
 
 To use the plugin, import the `SQLAdminPlugin` class and pass it to the `Litestar` application.
 
+By default, the plugin will create a new admin interface at `/admin`.
+
 ### Example
 
 ```python
 from litestar import Litestar
 from sqladmin import ModelView
 from sqladmin_litestar_plugin import SQLAdminPlugin
 from sqlalchemy import Column, Integer, String
```

