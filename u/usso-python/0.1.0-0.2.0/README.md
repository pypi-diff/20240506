# Comparing `tmp/usso_python-0.1.0.tar.gz` & `tmp/usso_python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usso_python-0.1.0.tar", last modified: Mon May  6 07:12:23 2024, max compression
+gzip compressed data, was "usso_python-0.2.0.tar", last modified: Mon May  6 07:16:34 2024, max compression
```

## Comparing `usso_python-0.1.0.tar` & `usso_python-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:12:23.563487 usso_python-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 07:12:18.000000 usso_python-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-06 07:12:23.563487 usso_python-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-06 07:12:18.000000 usso_python-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-06 07:12:18.000000 usso_python-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 07:12:23.563487 usso_python-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:12:23.559487 usso_python-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:12:23.563487 usso_python-0.1.0/src/usso/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-06 07:12:18.000000 usso_python-0.1.0/src/usso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-06 07:12:18.000000 usso_python-0.1.0/src/usso/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-06 07:12:18.000000 usso_python-0.1.0/src/usso/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 07:12:18.000000 usso_python-0.1.0/src/usso/package_data.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:12:23.563487 usso_python-0.1.0/src/usso_fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 07:12:18.000000 usso_python-0.1.0/src/usso_fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-06 07:12:18.000000 usso_python-0.1.0/src/usso_fastapi/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:12:23.563487 usso_python-0.1.0/src/usso_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-06 07:12:23.000000 usso_python-0.1.0/src/usso_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-06 07:12:23.000000 usso_python-0.1.0/src/usso_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 07:12:23.000000 usso_python-0.1.0/src/usso_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 07:12:23.000000 usso_python-0.1.0/src/usso_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 07:12:23.000000 usso_python-0.1.0/src/usso_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 07:12:23.000000 usso_python-0.1.0/src/usso_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:12:23.563487 usso_python-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-06 07:12:18.000000 usso_python-0.1.0/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:16:34.618478 usso_python-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 07:16:25.000000 usso_python-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-06 07:16:34.618478 usso_python-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-06 07:16:25.000000 usso_python-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-06 07:16:25.000000 usso_python-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 07:16:34.618478 usso_python-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:16:34.614478 usso_python-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:16:34.614478 usso_python-0.2.0/src/usso/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-06 07:16:25.000000 usso_python-0.2.0/src/usso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-06 07:16:25.000000 usso_python-0.2.0/src/usso/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-06 07:16:25.000000 usso_python-0.2.0/src/usso/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 07:16:25.000000 usso_python-0.2.0/src/usso/package_data.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:16:34.614478 usso_python-0.2.0/src/usso_fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 07:16:25.000000 usso_python-0.2.0/src/usso_fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-06 07:16:25.000000 usso_python-0.2.0/src/usso_fastapi/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:16:34.614478 usso_python-0.2.0/src/usso_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-06 07:16:34.000000 usso_python-0.2.0/src/usso_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-06 07:16:34.000000 usso_python-0.2.0/src/usso_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 07:16:34.000000 usso_python-0.2.0/src/usso_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 07:16:34.000000 usso_python-0.2.0/src/usso_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 07:16:34.000000 usso_python-0.2.0/src/usso_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 07:16:34.000000 usso_python-0.2.0/src/usso_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:16:34.614478 usso_python-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-06 07:16:25.000000 usso_python-0.2.0/tests/test_simple.py
```

### Comparing `usso_python-0.1.0/LICENSE.txt` & `usso_python-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `usso_python-0.1.0/PKG-INFO` & `usso_python-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usso-python
-Version: 0.1.0
+Version: 0.2.0
 Summary: A plug-and-play client for integrating universal single sign-on (SSO) with Python frameworks, enabling secure and seamless authentication across microservices.
 Author-email: Mahdi Kiani <mahdikiany@gmail.com>
 Maintainer-email: Mahdi Kiani <mahdikiany@gmail.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `usso_python-0.1.0/README.md` & `usso_python-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `usso_python-0.1.0/pyproject.toml` & `usso_python-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "usso-python"
-version = "0.1.0"
+version = "0.2.0"
 description = "A plug-and-play client for integrating universal single sign-on (SSO) with Python frameworks, enabling secure and seamless authentication across microservices."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["usso", "sso", "authentication", "security", "fastapi", "django"]
 authors = [
   {name = "Mahdi Kiani", email = "mahdikiany@gmail.com"}
```

### Comparing `usso_python-0.1.0/src/usso/core.py` & `usso_python-0.2.0/src/usso/core.py`

 * *Files identical despite different names*

### Comparing `usso_python-0.1.0/src/usso_fastapi/integration.py` & `usso_python-0.2.0/src/usso_fastapi/integration.py`

 * *Files identical despite different names*

### Comparing `usso_python-0.1.0/src/usso_python.egg-info/PKG-INFO` & `usso_python-0.2.0/src/usso_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usso-python
-Version: 0.1.0
+Version: 0.2.0
 Summary: A plug-and-play client for integrating universal single sign-on (SSO) with Python frameworks, enabling secure and seamless authentication across microservices.
 Author-email: Mahdi Kiani <mahdikiany@gmail.com>
 Maintainer-email: Mahdi Kiani <mahdikiany@gmail.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

