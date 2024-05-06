# Comparing `tmp/usso-0.4.0.tar.gz` & `tmp/usso-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usso-0.4.0.tar", last modified: Mon May  6 07:42:45 2024, max compression
+gzip compressed data, was "usso-0.5.0.tar", last modified: Mon May  6 08:07:00 2024, max compression
```

## Comparing `usso-0.4.0.tar` & `usso-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:42:45.965528 usso-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 07:42:41.000000 usso-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-06 07:42:45.965528 usso-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-06 07:42:41.000000 usso-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-06 07:42:41.000000 usso-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 07:42:45.965528 usso-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:42:45.961528 usso-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:42:45.961528 usso-0.4.0/src/usso/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-06 07:42:41.000000 usso-0.4.0/src/usso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-06 07:42:41.000000 usso-0.4.0/src/usso/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-06 07:42:41.000000 usso-0.4.0/src/usso/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 07:42:41.000000 usso-0.4.0/src/usso/package_data.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:42:45.961528 usso-0.4.0/src/usso/usso_fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-06 07:42:41.000000 usso-0.4.0/src/usso/usso_fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-06 07:42:41.000000 usso-0.4.0/src/usso/usso_fastapi/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:42:45.965528 usso-0.4.0/src/usso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-06 07:42:45.000000 usso-0.4.0/src/usso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-06 07:42:45.000000 usso-0.4.0/src/usso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 07:42:45.000000 usso-0.4.0/src/usso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 07:42:45.000000 usso-0.4.0/src/usso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 07:42:45.000000 usso-0.4.0/src/usso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 07:42:45.000000 usso-0.4.0/src/usso.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:42:45.965528 usso-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-06 07:42:41.000000 usso-0.4.0/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:07:00.079046 usso-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-06 08:06:55.000000 usso-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-06 08:07:00.079046 usso-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-06 08:06:55.000000 usso-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-06 08:06:55.000000 usso-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:07:00.079046 usso-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:07:00.075046 usso-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:07:00.075046 usso-0.5.0/src/usso/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-06 08:06:55.000000 usso-0.5.0/src/usso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-06 08:06:55.000000 usso-0.5.0/src/usso/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-06 08:06:55.000000 usso-0.5.0/src/usso/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:06:55.000000 usso-0.5.0/src/usso/package_data.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:07:00.079046 usso-0.5.0/src/usso/usso_fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:06:55.000000 usso-0.5.0/src/usso/usso_fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-06 08:06:55.000000 usso-0.5.0/src/usso/usso_fastapi/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:07:00.079046 usso-0.5.0/src/usso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-06 08:07:00.000000 usso-0.5.0/src/usso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-06 08:07:00.000000 usso-0.5.0/src/usso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:07:00.000000 usso-0.5.0/src/usso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 08:07:00.000000 usso-0.5.0/src/usso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-06 08:07:00.000000 usso-0.5.0/src/usso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 08:07:00.000000 usso-0.5.0/src/usso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:07:00.079046 usso-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-06 08:06:55.000000 usso-0.5.0/tests/test_simple.py
```

### Comparing `usso-0.4.0/LICENSE.txt` & `usso-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `usso-0.4.0/PKG-INFO` & `usso-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usso
-Version: 0.4.0
+Version: 0.5.0
 Summary: A plug-and-play client for integrating universal single sign-on (SSO) with Python frameworks, enabling secure and seamless authentication across microservices.
 Author-email: Mahdi Kiani <mahdikiany@gmail.com>
 Maintainer-email: Mahdi Kiani <mahdikiany@gmail.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `usso-0.4.0/README.md` & `usso-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `usso-0.4.0/pyproject.toml` & `usso-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "usso"
-version = "0.4.0"
+version = "0.5.0"
 description = "A plug-and-play client for integrating universal single sign-on (SSO) with Python frameworks, enabling secure and seamless authentication across microservices."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["usso", "sso", "authentication", "security", "fastapi", "django"]
 authors = [
   {name = "Mahdi Kiani", email = "mahdikiany@gmail.com"}
```

### Comparing `usso-0.4.0/src/usso/core.py` & `usso-0.5.0/src/usso/core.py`

 * *Files identical despite different names*

### Comparing `usso-0.4.0/src/usso/usso_fastapi/integration.py` & `usso-0.5.0/src/usso/usso_fastapi/integration.py`

 * *Files identical despite different names*

### Comparing `usso-0.4.0/src/usso.egg-info/PKG-INFO` & `usso-0.5.0/src/usso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usso
-Version: 0.4.0
+Version: 0.5.0
 Summary: A plug-and-play client for integrating universal single sign-on (SSO) with Python frameworks, enabling secure and seamless authentication across microservices.
 Author-email: Mahdi Kiani <mahdikiany@gmail.com>
 Maintainer-email: Mahdi Kiani <mahdikiany@gmail.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

