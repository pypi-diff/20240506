# Comparing `tmp/anydi-0.24.0.tar.gz` & `tmp/anydi-0.25.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anydi-0.24.0.tar", max compression
+gzip compressed data, was "anydi-0.25.0a0.tar", max compression
```

## Comparing `anydi-0.24.0.tar` & `anydi-0.25.0a0.tar`

### file list

```diff
@@ -1,18 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.24.0/LICENSE
--rw-r--r--   0        0        0     2625 2024-03-11 08:19:19.508853 anydi-0.24.0/README.md
--rw-r--r--   0        0        0      562 2024-03-04 13:20:12.097070 anydi-0.24.0/anydi/__init__.py
--rw-r--r--   0        0        0    28347 2024-04-07 18:01:12.996941 anydi-0.24.0/anydi/_container.py
--rw-r--r--   0        0        0    10258 2024-02-28 07:17:37.315755 anydi-0.24.0/anydi/_context.py
--rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.24.0/anydi/_logger.py
--rw-r--r--   0        0        0     3712 2024-03-04 13:20:12.098039 anydi-0.24.0/anydi/_module.py
--rw-r--r--   0        0        0     6781 2024-03-04 13:20:12.098430 anydi-0.24.0/anydi/_scanner.py
--rw-r--r--   0        0        0     3240 2024-02-28 07:17:37.316974 anydi-0.24.0/anydi/_types.py
--rw-r--r--   0        0        0     3152 2024-03-04 13:20:12.098746 anydi-0.24.0/anydi/_utils.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.24.0/anydi/ext/__init__.py
--rw-r--r--   0        0        0     5311 2024-04-20 17:59:50.473425 anydi-0.24.0/anydi/ext/fastapi.py
--rw-r--r--   0        0        0     3976 2024-03-20 12:47:26.894485 anydi-0.24.0/anydi/ext/pytest_plugin.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.24.0/anydi/ext/starlette/__init__.py
--rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.24.0/anydi/ext/starlette/middleware.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.24.0/anydi/py.typed
--rw-r--r--   0        0        0     2777 2024-04-20 17:59:58.443230 anydi-0.24.0/pyproject.toml
--rw-r--r--   0        0        0     4371 1970-01-01 00:00:00.000000 anydi-0.24.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.25.0a0/LICENSE
+-rw-r--r--   0        0        0     2625 2024-03-11 08:19:19.508853 anydi-0.25.0a0/README.md
+-rw-r--r--   0        0        0      562 2024-03-04 13:20:12.097070 anydi-0.25.0a0/anydi/__init__.py
+-rw-r--r--   0        0        0    28347 2024-04-07 18:01:12.996941 anydi-0.25.0a0/anydi/_container.py
+-rw-r--r--   0        0        0    10258 2024-02-28 07:17:37.315755 anydi-0.25.0a0/anydi/_context.py
+-rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.25.0a0/anydi/_logger.py
+-rw-r--r--   0        0        0     3712 2024-03-04 13:20:12.098039 anydi-0.25.0a0/anydi/_module.py
+-rw-r--r--   0        0        0     6781 2024-03-04 13:20:12.098430 anydi-0.25.0a0/anydi/_scanner.py
+-rw-r--r--   0        0        0     3240 2024-02-28 07:17:37.316974 anydi-0.25.0a0/anydi/_types.py
+-rw-r--r--   0        0        0     3152 2024-03-04 13:20:12.098746 anydi-0.25.0a0/anydi/_utils.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.25.0a0/anydi/ext/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-05 18:26:46.598768 anydi-0.25.0a0/anydi/ext/django/__init__.py
+-rw-r--r--   0        0        0      418 2024-05-05 18:26:47.962644 anydi-0.25.0a0/anydi/ext/django/_container.py
+-rw-r--r--   0        0        0      430 2024-05-05 18:27:49.545197 anydi-0.25.0a0/anydi/ext/django/_utils.py
+-rw-r--r--   0        0        0     4739 2024-05-05 18:50:18.088878 anydi-0.25.0a0/anydi/ext/django/apps.py
+-rw-r--r--   0        0        0      520 2024-05-05 18:27:26.714331 anydi-0.25.0a0/anydi/ext/django/ninja/__init__.py
+-rw-r--r--   0        0        0     2660 2024-05-05 18:27:49.545197 anydi-0.25.0a0/anydi/ext/django/ninja/_operation.py
+-rw-r--r--   0        0        0     2177 2024-05-05 18:27:47.544088 anydi-0.25.0a0/anydi/ext/django/ninja/_signature.py
+-rw-r--r--   0        0        0     5311 2024-04-20 17:59:50.473425 anydi-0.25.0a0/anydi/ext/fastapi.py
+-rw-r--r--   0        0        0     3976 2024-03-20 12:47:26.894485 anydi-0.25.0a0/anydi/ext/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.25.0a0/anydi/ext/starlette/__init__.py
+-rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.25.0a0/anydi/ext/starlette/middleware.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.25.0a0/anydi/py.typed
+-rw-r--r--   0        0        0     2905 2024-05-05 18:49:20.165988 anydi-0.25.0a0/pyproject.toml
+-rw-r--r--   0        0        0     4373 1970-01-01 00:00:00.000000 anydi-0.25.0a0/PKG-INFO
```

### Comparing `anydi-0.24.0/LICENSE` & `anydi-0.25.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `anydi-0.24.0/README.md` & `anydi-0.25.0a0/README.md`

 * *Files identical despite different names*

### Comparing `anydi-0.24.0/anydi/__init__.py` & `anydi-0.25.0a0/anydi/__init__.py`

 * *Files identical despite different names*

### Comparing `anydi-0.24.0/anydi/_container.py` & `anydi-0.25.0a0/anydi/_container.py`

 * *Files identical despite different names*

### Comparing `anydi-0.24.0/anydi/_context.py` & `anydi-0.25.0a0/anydi/_context.py`

 * *Files identical despite different names*

### Comparing `anydi-0.24.0/anydi/_module.py` & `anydi-0.25.0a0/anydi/_module.py`

 * *Files identical despite different names*

### Comparing `anydi-0.24.0/anydi/_scanner.py` & `anydi-0.25.0a0/anydi/_scanner.py`

 * *Files identical despite different names*

### Comparing `anydi-0.24.0/anydi/_types.py` & `anydi-0.25.0a0/anydi/_types.py`

 * *Files identical despite different names*

### Comparing `anydi-0.24.0/anydi/_utils.py` & `anydi-0.25.0a0/anydi/_utils.py`

 * *Files identical despite different names*

### Comparing `anydi-0.24.0/anydi/ext/fastapi.py` & `anydi-0.25.0a0/anydi/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `anydi-0.24.0/anydi/ext/pytest_plugin.py` & `anydi-0.25.0a0/anydi/ext/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `anydi-0.24.0/anydi/ext/starlette/middleware.py` & `anydi-0.25.0a0/anydi/ext/starlette/middleware.py`

 * *Files identical despite different names*

### Comparing `anydi-0.24.0/pyproject.toml` & `anydi-0.25.0a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anydi"
-version = "0.24.0"
+version = "0.25.0a0"
 description = "Dependency Injection library"
 authors = ["Anton Ruhlov <antonruhlov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/antonrh/anydi"
 keywords = ["dependency injection", "dependencies", "di", "async", "asyncio", "application"]
 classifiers = [
@@ -42,20 +42,22 @@
 mkdocs-material = { version = "^9.1.13", optional = true }
 
 [tool.poetry.extras]
 docs = ["mkdocs", "mkdocs-material"]
 async = ["anyio"]
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^1.9.0"
-ruff = "^0.4.1"
+mypy = "^1.10.0"
+ruff = "^0.4.3"
 pytest = "^8.1.0"
 pytest-cov = "^5.0.0"
-fastapi = "^0.95.1"
+fastapi = "^0.100.0"
 httpx = "^0.26.0"
+django = "^4.2"
+django-ninja = "^1.1.0"
 
 [tool.poetry.plugins.pytest11]
 anydi = "anydi.ext.pytest_plugin"
 
 [tool.ruff]
 line-length = 88
 
@@ -70,14 +72,20 @@
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.mypy]
 python_version = "3.10"
 strict = true
 
+[[tool.mypy.overrides]]
+module = [
+    "django.*",
+]
+ignore_missing_imports = true
+
 [tool.pytest.ini_options]
 addopts = [
     "--strict-config",
     "--strict-markers",
 ]
 xfail_strict = true
 junit_family = "xunit2"
```

### Comparing `anydi-0.24.0/PKG-INFO` & `anydi-0.25.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anydi
-Version: 0.24.0
+Version: 0.25.0a0
 Summary: Dependency Injection library
 Home-page: https://github.com/antonrh/anydi
 License: MIT
 Keywords: dependency injection,dependencies,di,async,asyncio,application
 Author: Anton Ruhlov
 Author-email: antonruhlov@gmail.com
 Requires-Python: >=3.8,<4.0
```

