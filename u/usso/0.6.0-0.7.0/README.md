# Comparing `tmp/usso-0.6.0.tar.gz` & `tmp/usso-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usso-0.6.0.tar", last modified: Mon May  6 08:09:27 2024, max compression
+gzip compressed data, was "usso-0.7.0.tar", last modified: Mon May  6 10:33:07 2024, max compression
```

## Comparing `usso-0.6.0.tar` & `usso-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:09:27.543438 usso-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 08:09:17.000000 usso-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-06 08:09:27.543438 usso-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-06 08:09:17.000000 usso-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-06 08:09:17.000000 usso-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:09:27.543438 usso-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:09:27.539438 usso-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:09:27.539438 usso-0.6.0/src/usso/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-06 08:09:17.000000 usso-0.6.0/src/usso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-06 08:09:17.000000 usso-0.6.0/src/usso/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-06 08:09:17.000000 usso-0.6.0/src/usso/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:09:17.000000 usso-0.6.0/src/usso/package_data.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:09:27.543438 usso-0.6.0/src/usso/usso_fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:09:17.000000 usso-0.6.0/src/usso/usso_fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-06 08:09:17.000000 usso-0.6.0/src/usso/usso_fastapi/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:09:27.543438 usso-0.6.0/src/usso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-06 08:09:27.000000 usso-0.6.0/src/usso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-06 08:09:27.000000 usso-0.6.0/src/usso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:09:27.000000 usso-0.6.0/src/usso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 08:09:27.000000 usso-0.6.0/src/usso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 08:09:27.000000 usso-0.6.0/src/usso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 08:09:27.000000 usso-0.6.0/src/usso.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:09:27.543438 usso-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-06 08:09:17.000000 usso-0.6.0/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:33:07.025847 usso-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 10:33:02.000000 usso-0.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-06 10:33:07.025847 usso-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-06 10:33:02.000000 usso-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-06 10:33:02.000000 usso-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 10:33:07.025847 usso-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:33:07.021846 usso-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:33:07.021846 usso-0.7.0/src/usso/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 10:33:02.000000 usso-0.7.0/src/usso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-06 10:33:02.000000 usso-0.7.0/src/usso/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-06 10:33:02.000000 usso-0.7.0/src/usso/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:33:07.025847 usso-0.7.0/src/usso/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-06 10:33:02.000000 usso-0.7.0/src/usso/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-06 10:33:02.000000 usso-0.7.0/src/usso/fastapi/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:33:02.000000 usso-0.7.0/src/usso/package_data.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:33:07.025847 usso-0.7.0/src/usso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-06 10:33:07.000000 usso-0.7.0/src/usso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-06 10:33:07.000000 usso-0.7.0/src/usso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:33:07.000000 usso-0.7.0/src/usso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 10:33:07.000000 usso-0.7.0/src/usso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 10:33:07.000000 usso-0.7.0/src/usso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 10:33:07.000000 usso-0.7.0/src/usso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:33:07.025847 usso-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-06 10:33:02.000000 usso-0.7.0/tests/test_simple.py
```

### Comparing `usso-0.6.0/LICENSE.txt` & `usso-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `usso-0.6.0/PKG-INFO` & `usso-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usso
-Version: 0.6.0
+Version: 0.7.0
 Summary: A plug-and-play client for integrating universal single sign-on (SSO) with Python frameworks, enabling secure and seamless authentication across microservices.
 Author-email: Mahdi Kiani <mahdikiany@gmail.com>
 Maintainer-email: Mahdi Kiani <mahdikiany@gmail.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `usso-0.6.0/README.md` & `usso-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `usso-0.6.0/pyproject.toml` & `usso-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "usso"
-version = "0.6.0"
+version = "0.7.0"
 description = "A plug-and-play client for integrating universal single sign-on (SSO) with Python frameworks, enabling secure and seamless authentication across microservices."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["usso", "sso", "authentication", "security", "fastapi", "django"]
 authors = [
   {name = "Mahdi Kiani", email = "mahdikiany@gmail.com"}
```

### Comparing `usso-0.6.0/src/usso/core.py` & `usso-0.7.0/src/usso/core.py`

 * *Files identical despite different names*

### Comparing `usso-0.6.0/src/usso/usso_fastapi/integration.py` & `usso-0.7.0/src/usso/fastapi/integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,21 +36,24 @@
             raise USSOException(
                 status_code=HTTP_401_UNAUTHORIZED, error="invalid_signature"
             )
         return None
     except jwt.exceptions.InvalidTokenError:
         if kwargs.get("raise_exception"):
             raise USSOException(
-                status_code=HTTP_401_UNAUTHORIZED, error="invalid_token"
+                status_code=HTTP_401_UNAUTHORIZED,
+                error="invalid_token",
             )
         return None
     except Exception as e:
         if kwargs.get("raise_exception"):
             raise USSOException(
-                status_code=HTTP_401_UNAUTHORIZED, error="error", message=str(e)
+                status_code=HTTP_401_UNAUTHORIZED,
+                error="error",
+                message=str(e),
             )
         logger.error(e)
         return None
 
     return UserData(**decoded)
 
 
@@ -65,9 +68,12 @@
             return await user_data_from_token(token, **kwargs)
 
     cookie_token = request.cookies.get("access_token")
     if cookie_token:
         return await user_data_from_token(cookie_token, **kwargs)
 
     if kwargs.get("raise_exception", True):
-        raise USSOException(status_code=HTTP_401_UNAUTHORIZED, error="unauthorized")
+        raise USSOException(
+            status_code=HTTP_401_UNAUTHORIZED,
+            error="unauthorized",
+        )
     return None
```

### Comparing `usso-0.6.0/src/usso.egg-info/PKG-INFO` & `usso-0.7.0/src/usso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usso
-Version: 0.6.0
+Version: 0.7.0
 Summary: A plug-and-play client for integrating universal single sign-on (SSO) with Python frameworks, enabling secure and seamless authentication across microservices.
 Author-email: Mahdi Kiani <mahdikiany@gmail.com>
 Maintainer-email: Mahdi Kiani <mahdikiany@gmail.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

