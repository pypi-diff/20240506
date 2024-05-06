# Comparing `tmp/some_aiohttp_middleware-0.1.4.tar.gz` & `tmp/some_aiohttp_middleware-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "some_aiohttp_middleware-0.1.4.tar", max compression
+gzip compressed data, was "some_aiohttp_middleware-0.1.5.tar", max compression
```

## Comparing `some_aiohttp_middleware-0.1.4.tar` & `some_aiohttp_middleware-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2024-03-26 18:53:20.363004 some_aiohttp_middleware-0.1.4/LICENSE
--rw-r--r--   0        0        0      563 2024-03-26 18:53:20.363004 some_aiohttp_middleware-0.1.4/README.md
--rw-r--r--   0        0        0     1435 2024-03-26 18:53:41.715297 some_aiohttp_middleware-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      153 2024-03-26 18:53:20.367004 some_aiohttp_middleware-0.1.4/src/some_aiohttp_middleware/__init__.py
--rw-r--r--   0        0        0     1585 2024-03-26 18:53:20.367004 some_aiohttp_middleware-0.1.4/src/some_aiohttp_middleware/admin_auth_handler.py
--rw-r--r--   0        0        0     4854 2024-03-26 18:53:20.367004 some_aiohttp_middleware-0.1.4/src/some_aiohttp_middleware/base.py
--rw-r--r--   0        0        0     2760 2024-03-26 18:53:20.367004 some_aiohttp_middleware-0.1.4/src/some_aiohttp_middleware/db.py
--rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 some_aiohttp_middleware-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-06 07:49:13.003096 some_aiohttp_middleware-0.1.5/LICENSE
+-rw-r--r--   0        0        0      563 2024-05-06 07:49:13.003096 some_aiohttp_middleware-0.1.5/README.md
+-rw-r--r--   0        0        0     1435 2024-05-06 07:49:32.158970 some_aiohttp_middleware-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      153 2024-05-06 07:49:13.003096 some_aiohttp_middleware-0.1.5/src/some_aiohttp_middleware/__init__.py
+-rw-r--r--   0        0        0     1762 2024-05-06 07:49:13.003096 some_aiohttp_middleware-0.1.5/src/some_aiohttp_middleware/admin_auth_handler.py
+-rw-r--r--   0        0        0     4854 2024-05-06 07:49:13.003096 some_aiohttp_middleware-0.1.5/src/some_aiohttp_middleware/base.py
+-rw-r--r--   0        0        0     2760 2024-05-06 07:49:13.003096 some_aiohttp_middleware-0.1.5/src/some_aiohttp_middleware/db.py
+-rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 some_aiohttp_middleware-0.1.5/PKG-INFO
```

### Comparing `some_aiohttp_middleware-0.1.4/LICENSE` & `some_aiohttp_middleware-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `some_aiohttp_middleware-0.1.4/README.md` & `some_aiohttp_middleware-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `some_aiohttp_middleware-0.1.4/pyproject.toml` & `some_aiohttp_middleware-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "some-aiohttp-middleware"
-version = "0.1.4"
+version = "0.1.5"
 license = "MIT"
 description = "Middleware framework for aiohttp"
 authors = ["tommmlij <tommmlij@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/tommmlij/some-aiohttp-middleware"
 packages = [{ include = "some_aiohttp_middleware", from = "src" }]
```

### Comparing `some_aiohttp_middleware-0.1.4/src/some_aiohttp_middleware/admin_auth_handler.py` & `some_aiohttp_middleware-0.1.5/src/some_aiohttp_middleware/admin_auth_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,15 +31,21 @@
     async def handle(request, *args, admin_token=None, token_location=None, **kwargs):
 
         if token_location is None:
             token_location = ["admin_token"]
 
         try:
             admin_token = admin_token or reduce(
-                operator.getitem, token_location, request.app.config
+                operator.getitem,
+                (
+                    token_location
+                    if isinstance(token_location, list)
+                    else [token_location]
+                ),
+                dict(request.app.config),
             )
         except (KeyError, TypeError, AttributeError):
             raise HTTPInternalServerError(
                 reason="Missing configuration, either pass 'admin_token' or 'token_location'"
             )
 
         try:
```

### Comparing `some_aiohttp_middleware-0.1.4/src/some_aiohttp_middleware/base.py` & `some_aiohttp_middleware-0.1.5/src/some_aiohttp_middleware/base.py`

 * *Files identical despite different names*

### Comparing `some_aiohttp_middleware-0.1.4/src/some_aiohttp_middleware/db.py` & `some_aiohttp_middleware-0.1.5/src/some_aiohttp_middleware/db.py`

 * *Files identical despite different names*

### Comparing `some_aiohttp_middleware-0.1.4/PKG-INFO` & `some_aiohttp_middleware-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: some-aiohttp-middleware
-Version: 0.1.4
+Version: 0.1.5
 Summary: Middleware framework for aiohttp
 Home-page: https://github.com/tommmlij/some-aiohttp-middleware
 License: MIT
 Author: tommmlij
 Author-email: tommmlij@gmail.com
 Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

