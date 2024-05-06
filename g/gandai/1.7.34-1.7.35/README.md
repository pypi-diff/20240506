# Comparing `tmp/gandai-1.7.34.tar.gz` & `tmp/gandai-1.7.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.7.34.tar", last modified: Fri Mar 29 16:30:42 2024, max compression
+gzip compressed data, was "gandai-1.7.35.tar", last modified: Mon May  6 17:49:30 2024, max compression
```

## Comparing `gandai-1.7.34.tar` & `gandai-1.7.35.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-03-29 16:30:42.057410 gandai-1.7.34/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.34/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-03-29 16:30:42.057190 gandai-1.7.34/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-03-29 16:30:42.049444 gandai-1.7.34/gandai/
--rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.34/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-03-29 16:30:42.054883 gandai-1.7.34/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.34/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.34/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.34/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.34/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2600 2024-03-29 15:40:37.000000 gandai-1.7.34/gandai/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.34/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.34/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.34/gandai/__pycache__/google.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5009 2024-03-29 15:42:34.000000 gandai-1.7.34/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.34/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1394 2024-03-29 15:42:35.000000 gandai-1.7.34/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    19189 2024-03-29 16:29:36.000000 gandai-1.7.34/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    10335 2024-03-29 15:42:35.000000 gandai-1.7.34/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    40632 2024-03-29 16:27:30.000000 gandai-1.7.34/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.34/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.34/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.34/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1695 2024-03-29 16:07:35.000000 gandai-1.7.34/gandai/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.34/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1674 2024-03-29 15:34:07.000000 gandai-1.7.34/gandai/constants.py
--rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.34/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.34/gandai/google.py
--rw-r--r--   0 parker     (501) staff       (20)     4223 2024-03-29 15:34:07.000000 gandai-1.7.34/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.34/gandai/grata.py
--rw-r--r--   0 parker     (501) staff       (20)      452 2024-03-29 15:34:07.000000 gandai-1.7.34/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)    14496 2024-03-29 16:29:34.000000 gandai-1.7.34/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-03-29 16:30:42.055669 gandai-1.7.34/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.34/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-03-29 16:30:42.056036 gandai-1.7.34/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.34/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.34/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.34/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.34/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.34/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-03-29 16:30:42.056747 gandai-1.7.34/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.34/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.34/gandai/migrations/sql/230818-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3342 2024-03-29 15:34:07.000000 gandai-1.7.34/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     4307 2024-03-29 15:34:07.000000 gandai-1.7.34/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    27713 2024-03-29 16:27:28.000000 gandai-1.7.34/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.34/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)     1079 2024-03-29 16:07:32.000000 gandai-1.7.34/gandai/tasks.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-03-29 16:30:42.056995 gandai-1.7.34/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-03-29 16:30:42.000000 gandai-1.7.34/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1478 2024-03-29 16:30:42.000000 gandai-1.7.34/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2024-03-29 16:30:42.000000 gandai-1.7.34/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2024-03-29 16:30:42.000000 gandai-1.7.34/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2024-03-29 16:30:17.000000 gandai-1.7.34/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2024-03-29 16:30:42.057446 gandai-1.7.34/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.34/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 17:49:30.584470 gandai-1.7.35/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.35/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-06 17:49:30.584265 gandai-1.7.35/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 17:49:30.578303 gandai-1.7.35/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.35/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 17:49:30.582476 gandai-1.7.35/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.35/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.35/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.35/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.35/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2600 2024-03-29 15:40:37.000000 gandai-1.7.35/gandai/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.35/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.35/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.35/gandai/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5002 2024-05-06 16:10:12.000000 gandai-1.7.35/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.35/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1394 2024-03-29 15:42:35.000000 gandai-1.7.35/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    19189 2024-03-29 16:29:36.000000 gandai-1.7.35/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    10668 2024-05-06 17:41:54.000000 gandai-1.7.35/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    40632 2024-03-29 16:27:30.000000 gandai-1.7.35/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.35/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.35/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.35/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1695 2024-03-29 16:07:35.000000 gandai-1.7.35/gandai/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.35/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1674 2024-03-29 15:34:07.000000 gandai-1.7.35/gandai/constants.py
+-rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.35/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.35/gandai/google.py
+-rw-r--r--   0 parker     (501) staff       (20)     4216 2024-05-06 16:10:07.000000 gandai-1.7.35/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.35/gandai/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)      452 2024-03-29 15:34:07.000000 gandai-1.7.35/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)    14496 2024-03-29 16:29:34.000000 gandai-1.7.35/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 17:49:30.582980 gandai-1.7.35/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.35/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 17:49:30.583346 gandai-1.7.35/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.35/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.35/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.35/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.35/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.35/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 17:49:30.583910 gandai-1.7.35/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.35/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.35/gandai/migrations/sql/230818-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3342 2024-03-29 15:34:07.000000 gandai-1.7.35/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     4516 2024-05-06 17:41:51.000000 gandai-1.7.35/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    27713 2024-03-29 16:27:28.000000 gandai-1.7.35/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.35/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)     1079 2024-03-29 16:07:32.000000 gandai-1.7.35/gandai/tasks.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 17:49:30.584071 gandai-1.7.35/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-06 17:49:30.000000 gandai-1.7.35/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1478 2024-05-06 17:49:30.000000 gandai-1.7.35/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-06 17:49:30.000000 gandai-1.7.35/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-06 17:49:30.000000 gandai-1.7.35/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-06 17:49:11.000000 gandai-1.7.35/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-06 17:49:30.584518 gandai-1.7.35/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.35/setup.py
```

### Comparing `gandai-1.7.34/gandai/__pycache__/__init__.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/__pycache__/constants.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/__pycache__/google.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x6fdf0666 (Fri Mar 29 15:34:07 2024 UTC)
-files sz: 4223
+moddate:  0xdf003966 (Mon May  6 16:10:07 2024 UTC)
+files sz: 4216
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a02640064026c016d035a0301
@@ -115,15 +115,15 @@
           15           2 LOAD_GLOBAL              0 (client)
                       14 LOAD_ATTR                1 (chat)
                       24 LOAD_ATTR                2 (completions)
                       34 LOAD_METHOD              3 (create)
          
           16          56 LOAD_FAST                0 (messages)
          
-          17          58 LOAD_CONST               1 ('gpt-4-0125-preview')
+          17          58 LOAD_CONST               1 ('gpt-4-turbo')
          
           19          60 LOAD_CONST               2 (0.0)
          
           20          62 LOAD_CONST               3 ('type')
                       64 LOAD_CONST               4 ('json_object')
                       66 BUILD_MAP                1
          
@@ -148,15 +148,15 @@
                      172 LOAD_ATTR                9 (message)
                      182 LOAD_ATTR               10 (content)
                      192 PRECALL                  1
                      196 CALL                     1
                      206 RETURN_VALUE
          consts
             None
-            'gpt-4-0125-preview'
+            'gpt-4-turbo'
             0.0
             'type'
             'json_object'
             ('messages', 'model', 'temperature', 'response_format')
             0
          names      ('client', 'chat', 'completions', 'create', 'print', 'usage', 'json', 'loads', 'choices', 'message', 'content')
          varnames   ('messages', 'chat_completion')
```

### Comparing `gandai-1.7.34/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/models.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,35 +1,35 @@
 magic:    0xa70d0d0a
-moddate:  0x6fdf0666 (Fri Mar 29 15:34:07 2024 UTC)
-files sz: 4307
+moddate:  0x5f163966 (Mon May  6 17:41:51 2024 UTC)
+files sz: 4516
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a026d035a036d045a0401
       00640064036c056d065a066d075a070100640064046c086d095a096d0a5a
-      0a0100650302004700640584006406a6020000ab020000000000000000a6
-      000000ab0000000000000000005a0b020065036407ac08a6010000ab0100
-      000000000000000200470064098400640aa6020000ab0200000000000000
-      00a6000000ab0000000000000000005a0c02004700640b8400640c650d65
-      06a6040000ab0400000000000000005a0e650302004700640d8400640ea6
-      020000ab020000000000000000a6000000ab0000000000000000005a0f65
-      0302004700640f84006410650fa6030000ab030000000000000000a60000
-      00ab0000000000000000005a10650302004700641184006412650fa60300
-      00ab030000000000000000a6000000ab0000000000000000005a11650302
-      004700641384006414a6020000ab020000000000000000a6000000ab0000
-      000000000000005a12650302004700641584006416a6020000ab02000000
-      0000000000a6000000ab0000000000000000005a13650302004700641784
-      006418a6020000ab020000000000000000a6000000ab0000000000000000
-      005a1465030200470064198400641aa6020000ab020000000000000000a6
-      000000ab0000000000000000005a15650302004700641b8400641ca60200
-      00ab020000000000000000a6000000ab0000000000000000005a16640153
-      00
+      0a6d0b5a0b0100650302004700640584006406a6020000ab020000000000
+      000000a6000000ab0000000000000000005a0c020065036407ac08a60100
+      00ab0100000000000000000200470064098400640aa6020000ab02000000
+      0000000000a6000000ab0000000000000000005a0d02004700640b840064
+      0c650e6506a6040000ab0400000000000000005a0f650302004700640d84
+      00640ea6020000ab020000000000000000a6000000ab0000000000000000
+      005a10650302004700640f840064106510a6030000ab0300000000000000
+      00a6000000ab0000000000000000005a1165030200470064118400641265
+      10a6030000ab030000000000000000a6000000ab0000000000000000005a
+      12650302004700641384006414a6020000ab020000000000000000a60000
+      00ab0000000000000000005a13650302004700641584006416a6020000ab
+      020000000000000000a6000000ab0000000000000000005a146503020047
+      00641784006418a6020000ab020000000000000000a6000000ab00000000
+      00000000005a1565030200470064198400641aa6020000ab020000000000
+      000000a6000000ab0000000000000000005a16650302004700641b840064
+      1ca6020000ab020000000000000000a6000000ab0000000000000000005a
+      1764015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (hashlib)
                  8 STORE_NAME               0 (hashlib)
    
@@ -50,197 +50,199 @@
                 36 IMPORT_FROM              6 (Enum)
                 38 STORE_NAME               6 (Enum)
                 40 IMPORT_FROM              7 (auto)
                 42 STORE_NAME               7 (auto)
                 44 POP_TOP
    
      4          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               4 (('List', 'Optional'))
+                48 LOAD_CONST               4 (('Any', 'List', 'Optional'))
                 50 IMPORT_NAME              8 (typing)
-                52 IMPORT_FROM              9 (List)
-                54 STORE_NAME               9 (List)
-                56 IMPORT_FROM             10 (Optional)
-                58 STORE_NAME              10 (Optional)
-                60 POP_TOP
-   
-     7          62 LOAD_NAME                3 (dataclass)
-   
-     8          64 PUSH_NULL
-                66 LOAD_BUILD_CLASS
-                68 LOAD_CONST               5 (<code object Actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 7>)
-                70 MAKE_FUNCTION            0
-                72 LOAD_CONST               6 ('Actor')
-                74 PRECALL                  2
-                78 CALL                     2
-   
-     7          88 PRECALL                  0
-                92 CALL                     0
-   
-     8         102 STORE_NAME              11 (Actor)
-   
-    18         104 PUSH_NULL
-               106 LOAD_NAME                3 (dataclass)
-               108 LOAD_CONST               7 (True)
-               110 KW_NAMES                 8
-               112 PRECALL                  1
-               116 CALL                     1
-   
-    19         126 PUSH_NULL
-               128 LOAD_BUILD_CLASS
-               130 LOAD_CONST               9 (<code object Company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 18>)
-               132 MAKE_FUNCTION            0
-               134 LOAD_CONST              10 ('Company')
-               136 PRECALL                  2
-               140 CALL                     2
-   
-    18         150 PRECALL                  0
-               154 CALL                     0
-   
-    19         164 STORE_NAME              12 (Company)
-   
-    58         166 PUSH_NULL
-               168 LOAD_BUILD_CLASS
-               170 LOAD_CONST              11 (<code object EventType, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 58>)
-               172 MAKE_FUNCTION            0
-               174 LOAD_CONST              12 ('EventType')
-               176 LOAD_NAME               13 (str)
-               178 LOAD_NAME                6 (Enum)
-               180 PRECALL                  4
-               184 CALL                     4
-               194 STORE_NAME              14 (EventType)
-   
-    70         196 LOAD_NAME                3 (dataclass)
-   
-    71         198 PUSH_NULL
-               200 LOAD_BUILD_CLASS
-               202 LOAD_CONST              13 (<code object Event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 70>)
-               204 MAKE_FUNCTION            0
-               206 LOAD_CONST              14 ('Event')
-               208 PRECALL                  2
-               212 CALL                     2
-   
-    70         222 PRECALL                  0
-               226 CALL                     0
-   
-    71         236 STORE_NAME              15 (Event)
-   
-    81         238 LOAD_NAME                3 (dataclass)
-   
-    82         240 PUSH_NULL
-               242 LOAD_BUILD_CLASS
-               244 LOAD_CONST              15 (<code object Comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 81>)
-               246 MAKE_FUNCTION            0
-               248 LOAD_CONST              16 ('Comment')
-               250 LOAD_NAME               15 (Event)
-               252 PRECALL                  3
-               256 CALL                     3
-   
-    81         266 PRECALL                  0
-               270 CALL                     0
-   
-    82         280 STORE_NAME              16 (Comment)
-   
-    88         282 LOAD_NAME                3 (dataclass)
-   
-    89         284 PUSH_NULL
-               286 LOAD_BUILD_CLASS
-               288 LOAD_CONST              17 (<code object Rating, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 88>)
-               290 MAKE_FUNCTION            0
-               292 LOAD_CONST              18 ('Rating')
-               294 LOAD_NAME               15 (Event)
-               296 PRECALL                  3
-               300 CALL                     3
-   
-    88         310 PRECALL                  0
-               314 CALL                     0
-   
-    89         324 STORE_NAME              17 (Rating)
-   
-    94         326 LOAD_NAME                3 (dataclass)
-   
-    95         328 PUSH_NULL
-               330 LOAD_BUILD_CLASS
-               332 LOAD_CONST              19 (<code object Inclusion, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 94>)
-               334 MAKE_FUNCTION            0
-               336 LOAD_CONST              20 ('Inclusion')
-               338 PRECALL                  2
-               342 CALL                     2
-   
-    94         352 PRECALL                  0
-               356 CALL                     0
-   
-    95         366 STORE_NAME              18 (Inclusion)
-   
-   104         368 LOAD_NAME                3 (dataclass)
-   
-   105         370 PUSH_NULL
-               372 LOAD_BUILD_CLASS
-               374 LOAD_CONST              21 (<code object Exclusion, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 104>)
-               376 MAKE_FUNCTION            0
-               378 LOAD_CONST              22 ('Exclusion')
-               380 PRECALL                  2
-               384 CALL                     2
-   
-   104         394 PRECALL                  0
-               398 CALL                     0
-   
-   105         408 STORE_NAME              19 (Exclusion)
-   
-   110         410 LOAD_NAME                3 (dataclass)
-   
-   111         412 PUSH_NULL
-               414 LOAD_BUILD_CLASS
-               416 LOAD_CONST              23 (<code object Criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 110>)
-               418 MAKE_FUNCTION            0
-               420 LOAD_CONST              24 ('Criteria')
-               422 PRECALL                  2
-               426 CALL                     2
-   
-   110         436 PRECALL                  0
-               440 CALL                     0
-   
-   111         450 STORE_NAME              20 (Criteria)
-   
-   118         452 LOAD_NAME                3 (dataclass)
-   
-   119         454 PUSH_NULL
-               456 LOAD_BUILD_CLASS
-               458 LOAD_CONST              25 (<code object Maps, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 118>)
-               460 MAKE_FUNCTION            0
-               462 LOAD_CONST              26 ('Maps')
-               464 PRECALL                  2
-               468 CALL                     2
-   
-   118         478 PRECALL                  0
-               482 CALL                     0
-   
-   119         492 STORE_NAME              21 (Maps)
-   
-   127         494 LOAD_NAME                3 (dataclass)
-   
-   128         496 PUSH_NULL
-               498 LOAD_BUILD_CLASS
-               500 LOAD_CONST              27 (<code object Search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 127>)
-               502 MAKE_FUNCTION            0
-               504 LOAD_CONST              28 ('Search')
-               506 PRECALL                  2
-               510 CALL                     2
-   
-   127         520 PRECALL                  0
-               524 CALL                     0
-   
-   128         534 STORE_NAME              22 (Search)
-               536 LOAD_CONST               1 (None)
-               538 RETURN_VALUE
+                52 IMPORT_FROM              9 (Any)
+                54 STORE_NAME               9 (Any)
+                56 IMPORT_FROM             10 (List)
+                58 STORE_NAME              10 (List)
+                60 IMPORT_FROM             11 (Optional)
+                62 STORE_NAME              11 (Optional)
+                64 POP_TOP
+   
+     7          66 LOAD_NAME                3 (dataclass)
+   
+     8          68 PUSH_NULL
+                70 LOAD_BUILD_CLASS
+                72 LOAD_CONST               5 (<code object Actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 7>)
+                74 MAKE_FUNCTION            0
+                76 LOAD_CONST               6 ('Actor')
+                78 PRECALL                  2
+                82 CALL                     2
+   
+     7          92 PRECALL                  0
+                96 CALL                     0
+   
+     8         106 STORE_NAME              12 (Actor)
+   
+    18         108 PUSH_NULL
+               110 LOAD_NAME                3 (dataclass)
+               112 LOAD_CONST               7 (True)
+               114 KW_NAMES                 8
+               116 PRECALL                  1
+               120 CALL                     1
+   
+    19         130 PUSH_NULL
+               132 LOAD_BUILD_CLASS
+               134 LOAD_CONST               9 (<code object Company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 18>)
+               136 MAKE_FUNCTION            0
+               138 LOAD_CONST              10 ('Company')
+               140 PRECALL                  2
+               144 CALL                     2
+   
+    18         154 PRECALL                  0
+               158 CALL                     0
+   
+    19         168 STORE_NAME              13 (Company)
+   
+    58         170 PUSH_NULL
+               172 LOAD_BUILD_CLASS
+               174 LOAD_CONST              11 (<code object EventType, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 58>)
+               176 MAKE_FUNCTION            0
+               178 LOAD_CONST              12 ('EventType')
+               180 LOAD_NAME               14 (str)
+               182 LOAD_NAME                6 (Enum)
+               184 PRECALL                  4
+               188 CALL                     4
+               198 STORE_NAME              15 (EventType)
+   
+    70         200 LOAD_NAME                3 (dataclass)
+   
+    71         202 PUSH_NULL
+               204 LOAD_BUILD_CLASS
+               206 LOAD_CONST              13 (<code object Event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 70>)
+               208 MAKE_FUNCTION            0
+               210 LOAD_CONST              14 ('Event')
+               212 PRECALL                  2
+               216 CALL                     2
+   
+    70         226 PRECALL                  0
+               230 CALL                     0
+   
+    71         240 STORE_NAME              16 (Event)
+   
+    81         242 LOAD_NAME                3 (dataclass)
+   
+    82         244 PUSH_NULL
+               246 LOAD_BUILD_CLASS
+               248 LOAD_CONST              15 (<code object Comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 81>)
+               250 MAKE_FUNCTION            0
+               252 LOAD_CONST              16 ('Comment')
+               254 LOAD_NAME               16 (Event)
+               256 PRECALL                  3
+               260 CALL                     3
+   
+    81         270 PRECALL                  0
+               274 CALL                     0
+   
+    82         284 STORE_NAME              17 (Comment)
+   
+    88         286 LOAD_NAME                3 (dataclass)
+   
+    89         288 PUSH_NULL
+               290 LOAD_BUILD_CLASS
+               292 LOAD_CONST              17 (<code object Rating, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 88>)
+               294 MAKE_FUNCTION            0
+               296 LOAD_CONST              18 ('Rating')
+               298 LOAD_NAME               16 (Event)
+               300 PRECALL                  3
+               304 CALL                     3
+   
+    88         314 PRECALL                  0
+               318 CALL                     0
+   
+    89         328 STORE_NAME              18 (Rating)
+   
+    94         330 LOAD_NAME                3 (dataclass)
+   
+    95         332 PUSH_NULL
+               334 LOAD_BUILD_CLASS
+               336 LOAD_CONST              19 (<code object Inclusion, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 94>)
+               338 MAKE_FUNCTION            0
+               340 LOAD_CONST              20 ('Inclusion')
+               342 PRECALL                  2
+               346 CALL                     2
+   
+    94         356 PRECALL                  0
+               360 CALL                     0
+   
+    95         370 STORE_NAME              19 (Inclusion)
+   
+   110         372 LOAD_NAME                3 (dataclass)
+   
+   111         374 PUSH_NULL
+               376 LOAD_BUILD_CLASS
+               378 LOAD_CONST              21 (<code object Exclusion, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 110>)
+               380 MAKE_FUNCTION            0
+               382 LOAD_CONST              22 ('Exclusion')
+               384 PRECALL                  2
+               388 CALL                     2
+   
+   110         398 PRECALL                  0
+               402 CALL                     0
+   
+   111         412 STORE_NAME              20 (Exclusion)
+   
+   116         414 LOAD_NAME                3 (dataclass)
+   
+   117         416 PUSH_NULL
+               418 LOAD_BUILD_CLASS
+               420 LOAD_CONST              23 (<code object Criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 116>)
+               422 MAKE_FUNCTION            0
+               424 LOAD_CONST              24 ('Criteria')
+               426 PRECALL                  2
+               430 CALL                     2
+   
+   116         440 PRECALL                  0
+               444 CALL                     0
+   
+   117         454 STORE_NAME              21 (Criteria)
+   
+   124         456 LOAD_NAME                3 (dataclass)
+   
+   125         458 PUSH_NULL
+               460 LOAD_BUILD_CLASS
+               462 LOAD_CONST              25 (<code object Maps, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 124>)
+               464 MAKE_FUNCTION            0
+               466 LOAD_CONST              26 ('Maps')
+               468 PRECALL                  2
+               472 CALL                     2
+   
+   124         482 PRECALL                  0
+               486 CALL                     0
+   
+   125         496 STORE_NAME              22 (Maps)
+   
+   133         498 LOAD_NAME                3 (dataclass)
+   
+   134         500 PUSH_NULL
+               502 LOAD_BUILD_CLASS
+               504 LOAD_CONST              27 (<code object Search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 133>)
+               506 MAKE_FUNCTION            0
+               508 LOAD_CONST              28 ('Search')
+               510 PRECALL                  2
+               514 CALL                     2
+   
+   133         524 PRECALL                  0
+               528 CALL                     0
+   
+   134         538 STORE_NAME              23 (Search)
+               540 LOAD_CONST               1 (None)
+               542 RETURN_VALUE
    consts
       0
       None
       ('asdict', 'dataclass', 'field')
       ('Enum', 'auto')
-      ('List', 'Optional')
+      ('Any', 'List', 'Optional')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c0000006503650464023c
@@ -946,15 +948,16 @@
             00650364038400ac01a6010000ab0100000000000000005a096506650a19
             000000000000000000650864043c0000000200650364058400ac01a60100
             00ab0100000000000000005a0b6506650719000000000000000000650864
             063c0000000200650364078400ac01a6010000ab0100000000000000005a
             0c6506650719000000000000000000650864083c000000020065036504ac
             01a6010000ab0100000000000000005a0d65066507190000000000000000
             00650864093c000000020065036504ac01a6010000ab0100000000000000
-            005a0e65066507190000000000000000006508640a3c000000640b5300
+            005a0e65066507190000000000000000006508640a3c000000640b84005a
+            0f640c5300
           94           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Inclusion')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
@@ -977,15 +980,15 @@
                       62 LOAD_CONST               3 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 97>)
                       64 MAKE_FUNCTION            0
                       66 KW_NAMES                 1
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_NAME               9 (employees_range)
                       84 LOAD_NAME                6 (List)
-                      86 LOAD_NAME               10 (int)
+                      86 LOAD_NAME               10 (Any)
                       88 BINARY_SUBSCR
                       98 LOAD_NAME                8 (__annotations__)
                      100 LOAD_CONST               4 ('employees_range')
                      102 STORE_SUBSCR
          
           98         106 PUSH_NULL
                      108 LOAD_NAME                3 (field)
@@ -1040,16 +1043,20 @@
                      270 STORE_NAME              14 (city)
                      272 LOAD_NAME                6 (List)
                      274 LOAD_NAME                7 (str)
                      276 BINARY_SUBSCR
                      286 LOAD_NAME                8 (__annotations__)
                      288 LOAD_CONST              10 ('city')
                      290 STORE_SUBSCR
-                     294 LOAD_CONST              11 (None)
-                     296 RETURN_VALUE
+         
+         103         294 LOAD_CONST              11 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 103>)
+                     296 MAKE_FUNCTION            0
+                     298 STORE_NAME              15 (__post_init__)
+                     300 LOAD_CONST              12 (None)
+                     302 RETURN_VALUE
          consts
             'Inclusion'
             ('default_factory',)
             'keywords'
             code
                argcount  : 0
                nlocals   : 0
@@ -1116,56 +1123,109 @@
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       '<lambda>'
                firstlineno 99
                lnotab 0x
             'country'
             'state'
             'city'
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007c006a000000000000000000640119000000000000000000800a64
+                  017c006a00000000000000000064013c0000007c006a0000000000000000
+                  00640219000000000000000000800c64037c006a00000000000000000064
+                  023c0000006400530064005300
+               103           0 RESUME                   0
+               
+               104           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (employees_range)
+                            14 LOAD_CONST               1 (0)
+                            16 BINARY_SUBSCR
+                            26 POP_JUMP_FORWARD_IF_NOT_NONE    10 (to 48)
+               
+               105          28 LOAD_CONST               1 (0)
+                            30 LOAD_FAST                0 (self)
+                            32 LOAD_ATTR                0 (employees_range)
+                            42 LOAD_CONST               1 (0)
+                            44 STORE_SUBSCR
+               
+               106     >>   48 LOAD_FAST                0 (self)
+                            50 LOAD_ATTR                0 (employees_range)
+                            60 LOAD_CONST               2 (1)
+                            62 BINARY_SUBSCR
+                            72 POP_JUMP_FORWARD_IF_NOT_NONE    12 (to 98)
+               
+               107          74 LOAD_CONST               3 (100000)
+                            76 LOAD_FAST                0 (self)
+                            78 LOAD_ATTR                0 (employees_range)
+                            88 LOAD_CONST               2 (1)
+                            90 STORE_SUBSCR
+                            94 LOAD_CONST               0 (None)
+                            96 RETURN_VALUE
+               
+               106     >>   98 LOAD_CONST               0 (None)
+                           100 RETURN_VALUE
+               consts
+                  None
+                  0
+                  1
+                  100000
+               names      ('employees_range',)
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
+               name       '__post_init__'
+               firstlineno 103
+               lnotab 0x02011a0114011a0118ff
             None
-         names      ('__name__', '__module__', '__qualname__', 'field', 'list', 'keywords', 'List', 'str', '__annotations__', 'employees_range', 'int', 'ownership', 'country', 'state', 'city')
+         names      ('__name__', '__module__', '__qualname__', 'field', 'list', 'keywords', 'List', 'str', '__annotations__', 'employees_range', 'Any', 'ownership', 'country', 'state', 'city', '__post_init__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Inclusion'
          firstlineno 94
-         lnotab 0x0c022e013001300130012e01
+         lnotab 0x0c022e013001300130012e012e02
       'Inclusion'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a025500020065036504ac01a6010000ab01000000
             00000000005a056506650719000000000000000000650864023c00000002
             0065036504ac01a6010000ab0100000000000000005a0965066507190000
             00000000000000650864033c00000064045300
-         104           0 RESUME                   0
+         110           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Exclusion')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         106          12 PUSH_NULL
+         112          12 PUSH_NULL
                       14 LOAD_NAME                3 (field)
                       16 LOAD_NAME                4 (list)
                       18 KW_NAMES                 1
                       20 PRECALL                  1
                       24 CALL                     1
                       34 STORE_NAME               5 (keywords)
                       36 LOAD_NAME                6 (List)
                       38 LOAD_NAME                7 (str)
                       40 BINARY_SUBSCR
                       50 LOAD_NAME                8 (__annotations__)
                       52 LOAD_CONST               2 ('keywords')
                       54 STORE_SUBSCR
          
-         107          58 PUSH_NULL
+         113          58 PUSH_NULL
                       60 LOAD_NAME                3 (field)
                       62 LOAD_NAME                4 (list)
                       64 KW_NAMES                 1
                       66 PRECALL                  1
                       70 CALL                     1
                       80 STORE_NAME               9 (state)
                       82 LOAD_NAME                6 (List)
@@ -1184,66 +1244,66 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'field', 'list', 'keywords', 'List', 'str', '__annotations__', 'state')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Exclusion'
-         firstlineno 104
+         firstlineno 110
          lnotab 0x0c022e01
       'Exclusion'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a025500020065036504ac01a6010000ab01000000
             00000000005a056504650664023c000000020065036507ac01a6010000ab
             0100000000000000005a086507650664033c00000064045a09650a650664
             053c00000064065a0b650c650664073c00000064085300
-         110           0 RESUME                   0
+         116           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Criteria')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         112          12 PUSH_NULL
+         118          12 PUSH_NULL
                       14 LOAD_NAME                3 (field)
                       16 LOAD_NAME                4 (Inclusion)
                       18 KW_NAMES                 1
                       20 PRECALL                  1
                       24 CALL                     1
                       34 STORE_NAME               5 (inclusion)
                       36 LOAD_NAME                4 (Inclusion)
                       38 LOAD_NAME                6 (__annotations__)
                       40 LOAD_CONST               2 ('inclusion')
                       42 STORE_SUBSCR
          
-         113          46 PUSH_NULL
+         119          46 PUSH_NULL
                       48 LOAD_NAME                3 (field)
                       50 LOAD_NAME                7 (Exclusion)
                       52 KW_NAMES                 1
                       54 PRECALL                  1
                       58 CALL                     1
                       68 STORE_NAME               8 (exclusion)
                       70 LOAD_NAME                7 (Exclusion)
                       72 LOAD_NAME                6 (__annotations__)
                       74 LOAD_CONST               3 ('exclusion')
                       76 STORE_SUBSCR
          
-         114          80 LOAD_CONST               4 (25)
+         120          80 LOAD_CONST               4 (25)
                       82 STORE_NAME               9 (result_count)
                       84 LOAD_NAME               10 (int)
                       86 LOAD_NAME                6 (__annotations__)
                       88 LOAD_CONST               5 ('result_count')
                       90 STORE_SUBSCR
          
-         115          94 LOAD_CONST               6 ('any')
+         121          94 LOAD_CONST               6 ('any')
                       96 STORE_NAME              11 (operator)
                       98 LOAD_NAME               12 (str)
                      100 LOAD_NAME                6 (__annotations__)
                      102 LOAD_CONST               7 ('operator')
                      104 STORE_SUBSCR
                      108 LOAD_CONST               8 (None)
                      110 RETURN_VALUE
@@ -1259,70 +1319,70 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'field', 'Inclusion', 'inclusion', '__annotations__', 'Exclusion', 'exclusion', 'result_count', 'int', 'operator', 'str')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Criteria'
-         firstlineno 110
+         firstlineno 116
          lnotab 0x0c02220122010e01
       'Criteria'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a02550064015a036504650564023c000000020065
             066507ac03a6010000ab0100000000000000005a08650965041900000000
             0000000000650564043c00000064055a0a650b650564063c00000064075a
             0c650b650564083c00000064015a0d6504650564093c000000640a5300
-         118           0 RESUME                   0
+         124           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Maps')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         120          12 LOAD_CONST               1 ('')
+         126          12 LOAD_CONST               1 ('')
                       14 STORE_NAME               3 (phrase)
                       16 LOAD_NAME                4 (str)
                       18 LOAD_NAME                5 (__annotations__)
                       20 LOAD_CONST               2 ('phrase')
                       22 STORE_SUBSCR
          
-         121          26 PUSH_NULL
+         127          26 PUSH_NULL
                       28 LOAD_NAME                6 (field)
                       30 LOAD_NAME                7 (list)
                       32 KW_NAMES                 3
                       34 PRECALL                  1
                       38 CALL                     1
                       48 STORE_NAME               8 (areas)
                       50 LOAD_NAME                9 (List)
                       52 LOAD_NAME                4 (str)
                       54 BINARY_SUBSCR
                       64 LOAD_NAME                5 (__annotations__)
                       66 LOAD_CONST               4 ('areas')
                       68 STORE_SUBSCR
          
-         122          72 LOAD_CONST               5 (1)
+         128          72 LOAD_CONST               5 (1)
                       74 STORE_NAME              10 (top_n)
                       76 LOAD_NAME               11 (int)
                       78 LOAD_NAME                5 (__annotations__)
                       80 LOAD_CONST               6 ('top_n')
                       82 STORE_SUBSCR
          
-         123          86 LOAD_CONST               7 (25)
+         129          86 LOAD_CONST               7 (25)
                       88 STORE_NAME              12 (radius)
                       90 LOAD_NAME               11 (int)
                       92 LOAD_NAME                5 (__annotations__)
                       94 LOAD_CONST               8 ('radius')
                       96 STORE_SUBSCR
          
-         124         100 LOAD_CONST               1 ('')
+         130         100 LOAD_CONST               1 ('')
                      102 STORE_NAME              13 (prompt)
                      104 LOAD_NAME                4 (str)
                      106 LOAD_NAME                5 (__annotations__)
                      108 LOAD_CONST               9 ('prompt')
                      110 STORE_SUBSCR
                      114 LOAD_CONST              10 (None)
                      116 RETURN_VALUE
@@ -1340,15 +1400,15 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'phrase', 'str', '__annotations__', 'field', 'list', 'areas', 'List', 'top_n', 'int', 'radius', 'prompt')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Maps'
-         firstlineno 118
+         firstlineno 124
          lnotab 0x0c020e012e010e010e01
       'Maps'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
@@ -1360,158 +1420,158 @@
             000000000000005a0c650b64066505660264088404a6000000ab00000000
             00000000005a0d650b64066505660264098404a6000000ab000000000000
             0000005a0e650b640665056602640a8404a6000000ab0000000000000000
             005a0f650b640665056602640b8404a6000000ab0000000000000000005a
             10650b640665056602640c8404a6000000ab0000000000000000005a1165
             0b640665056602640d8404a6000000ab0000000000000000005a12650b64
             0665056602640e8404a6000000ab0000000000000000005a13640f5300
-         127           0 RESUME                   0
+         133           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Search')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         129          12 LOAD_NAME                3 (int)
+         135          12 LOAD_NAME                3 (int)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('uid')
                       18 STORE_SUBSCR
          
-         130          22 LOAD_NAME                5 (str)
+         136          22 LOAD_NAME                5 (str)
                       24 LOAD_NAME                4 (__annotations__)
                       26 LOAD_CONST               2 ('label')
                       28 STORE_SUBSCR
          
-         131          32 PUSH_NULL
+         137          32 PUSH_NULL
                       34 LOAD_NAME                6 (field)
                       36 LOAD_NAME                7 (dict)
                       38 KW_NAMES                 3
                       40 PRECALL                  1
                       44 CALL                     1
                       54 STORE_NAME               8 (meta)
                       56 LOAD_NAME                7 (dict)
                       58 LOAD_NAME                4 (__annotations__)
                       60 LOAD_CONST               4 ('meta')
                       62 STORE_SUBSCR
          
-         132          66 PUSH_NULL
+         138          66 PUSH_NULL
                       68 LOAD_NAME                6 (field)
                       70 LOAD_NAME                9 (Criteria)
                       72 KW_NAMES                 3
                       74 PRECALL                  1
                       78 CALL                     1
                       88 STORE_NAME              10 (criteria)
                       90 LOAD_NAME                9 (Criteria)
                       92 LOAD_NAME                4 (__annotations__)
                       94 LOAD_CONST               5 ('criteria')
                       96 STORE_SUBSCR
          
-         136         100 LOAD_NAME               11 (property)
+         142         100 LOAD_NAME               11 (property)
          
-         137         102 LOAD_CONST               6 ('return')
+         143         102 LOAD_CONST               6 ('return')
                      104 LOAD_NAME                5 (str)
                      106 BUILD_TUPLE              2
-                     108 LOAD_CONST               7 (<code object notes, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 136>)
+                     108 LOAD_CONST               7 (<code object notes, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 142>)
                      110 MAKE_FUNCTION            4 (annotations)
          
-         136         112 PRECALL                  0
+         142         112 PRECALL                  0
                      116 CALL                     0
          
-         137         126 STORE_NAME              12 (notes)
+         143         126 STORE_NAME              12 (notes)
          
-         140         128 LOAD_NAME               11 (property)
+         146         128 LOAD_NAME               11 (property)
          
-         141         130 LOAD_CONST               6 ('return')
+         147         130 LOAD_CONST               6 ('return')
                      132 LOAD_NAME                5 (str)
                      134 BUILD_TUPLE              2
-                     136 LOAD_CONST               8 (<code object type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 140>)
+                     136 LOAD_CONST               8 (<code object type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 146>)
                      138 MAKE_FUNCTION            4 (annotations)
          
-         140         140 PRECALL                  0
+         146         140 PRECALL                  0
                      144 CALL                     0
          
-         141         154 STORE_NAME              13 (type)
+         147         154 STORE_NAME              13 (type)
          
-         144         156 LOAD_NAME               11 (property)
+         150         156 LOAD_NAME               11 (property)
          
-         145         158 LOAD_CONST               6 ('return')
+         151         158 LOAD_CONST               6 ('return')
                      160 LOAD_NAME                5 (str)
                      162 BUILD_TUPLE              2
-                     164 LOAD_CONST               9 (<code object prompt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 144>)
+                     164 LOAD_CONST               9 (<code object prompt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 150>)
                      166 MAKE_FUNCTION            4 (annotations)
          
-         144         168 PRECALL                  0
+         150         168 PRECALL                  0
                      172 CALL                     0
          
-         145         182 STORE_NAME              14 (prompt)
+         151         182 STORE_NAME              14 (prompt)
          
-         148         184 LOAD_NAME               11 (property)
+         154         184 LOAD_NAME               11 (property)
          
-         149         186 LOAD_CONST               6 ('return')
+         155         186 LOAD_CONST               6 ('return')
                      188 LOAD_NAME                5 (str)
                      190 BUILD_TUPLE              2
-                     192 LOAD_CONST              10 (<code object products, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 148>)
+                     192 LOAD_CONST              10 (<code object products, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 154>)
                      194 MAKE_FUNCTION            4 (annotations)
          
-         148         196 PRECALL                  0
+         154         196 PRECALL                  0
                      200 CALL                     0
          
-         149         210 STORE_NAME              15 (products)
+         155         210 STORE_NAME              15 (products)
          
-         153         212 LOAD_NAME               11 (property)
+         159         212 LOAD_NAME               11 (property)
          
-         154         214 LOAD_CONST               6 ('return')
+         160         214 LOAD_CONST               6 ('return')
                      216 LOAD_NAME                5 (str)
                      218 BUILD_TUPLE              2
-                     220 LOAD_CONST              11 (<code object services, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 153>)
+                     220 LOAD_CONST              11 (<code object services, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 159>)
                      222 MAKE_FUNCTION            4 (annotations)
          
-         153         224 PRECALL                  0
+         159         224 PRECALL                  0
                      228 CALL                     0
          
-         154         238 STORE_NAME              16 (services)
+         160         238 STORE_NAME              16 (services)
          
-         158         240 LOAD_NAME               11 (property)
+         164         240 LOAD_NAME               11 (property)
          
-         159         242 LOAD_CONST               6 ('return')
+         165         242 LOAD_CONST               6 ('return')
                      244 LOAD_NAME                5 (str)
                      246 BUILD_TUPLE              2
-                     248 LOAD_CONST              12 (<code object customers, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 158>)
+                     248 LOAD_CONST              12 (<code object customers, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 164>)
                      250 MAKE_FUNCTION            4 (annotations)
          
-         158         252 PRECALL                  0
+         164         252 PRECALL                  0
                      256 CALL                     0
          
-         159         266 STORE_NAME              17 (customers)
+         165         266 STORE_NAME              17 (customers)
          
-         163         268 LOAD_NAME               11 (property)
+         169         268 LOAD_NAME               11 (property)
          
-         164         270 LOAD_CONST               6 ('return')
+         170         270 LOAD_CONST               6 ('return')
                      272 LOAD_NAME                5 (str)
                      274 BUILD_TUPLE              2
-                     276 LOAD_CONST              13 (<code object was_acquired, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 163>)
+                     276 LOAD_CONST              13 (<code object was_acquired, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 169>)
                      278 MAKE_FUNCTION            4 (annotations)
          
-         163         280 PRECALL                  0
+         169         280 PRECALL                  0
                      284 CALL                     0
          
-         164         294 STORE_NAME              18 (was_acquired)
+         170         294 STORE_NAME              18 (was_acquired)
          
-         168         296 LOAD_NAME               11 (property)
+         174         296 LOAD_NAME               11 (property)
          
-         169         298 LOAD_CONST               6 ('return')
+         175         298 LOAD_CONST               6 ('return')
                      300 LOAD_NAME                5 (str)
                      302 BUILD_TUPLE              2
-                     304 LOAD_CONST              14 (<code object token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 168>)
+                     304 LOAD_CONST              14 (<code object token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 174>)
                      306 MAKE_FUNCTION            4 (annotations)
          
-         168         308 PRECALL                  0
+         174         308 PRECALL                  0
                      312 CALL                     0
          
-         169         322 STORE_NAME              19 (token)
+         175         322 STORE_NAME              19 (token)
                      324 LOAD_CONST              15 (None)
                      326 RETURN_VALUE
          consts
             'Search'
             'uid'
             'label'
             ('default_factory',)
@@ -1522,17 +1582,17 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016400a6020000ab0200000000000000005300
-               136           0 RESUME                   0
+               142           0 RESUME                   0
                
-               138           2 LOAD_FAST                0 (self)
+               144           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (meta)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('notes')
                             38 LOAD_CONST               0 (None)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 RETURN_VALUE
@@ -1541,27 +1601,27 @@
                   'notes'
                names      ('meta', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'notes'
-               firstlineno 136
+               firstlineno 142
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016400a6020000ab0200000000000000005300
-               140           0 RESUME                   0
+               146           0 RESUME                   0
                
-               142           2 LOAD_FAST                0 (self)
+               148           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (meta)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('search_type')
                             38 LOAD_CONST               0 (None)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 RETURN_VALUE
@@ -1570,27 +1630,27 @@
                   'search_type'
                names      ('meta', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'type'
-               firstlineno 140
+               firstlineno 146
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016400a6020000ab0200000000000000005300
-               144           0 RESUME                   0
+               150           0 RESUME                   0
                
-               146           2 LOAD_FAST                0 (self)
+               152           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (meta)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('prompt')
                             38 LOAD_CONST               0 (None)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 RETURN_VALUE
@@ -1599,27 +1659,27 @@
                   'prompt'
                names      ('meta', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'prompt'
-               firstlineno 144
+               firstlineno 150
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016400a6020000ab0200000000000000005300
-               148           0 RESUME                   0
+               154           0 RESUME                   0
                
-               151           2 LOAD_FAST                0 (self)
+               157           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (meta)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('products')
                             38 LOAD_CONST               0 (None)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 RETURN_VALUE
@@ -1628,27 +1688,27 @@
                   'products'
                names      ('meta', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'products'
-               firstlineno 148
+               firstlineno 154
                lnotab 0x0203
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016400a6020000ab0200000000000000005300
-               153           0 RESUME                   0
+               159           0 RESUME                   0
                
-               156           2 LOAD_FAST                0 (self)
+               162           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (meta)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('services')
                             38 LOAD_CONST               0 (None)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 RETURN_VALUE
@@ -1657,27 +1717,27 @@
                   'services'
                names      ('meta', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'services'
-               firstlineno 153
+               firstlineno 159
                lnotab 0x0203
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016400a6020000ab0200000000000000005300
-               158           0 RESUME                   0
+               164           0 RESUME                   0
                
-               161           2 LOAD_FAST                0 (self)
+               167           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (meta)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('customers')
                             38 LOAD_CONST               0 (None)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 RETURN_VALUE
@@ -1686,27 +1746,27 @@
                   'customers'
                names      ('meta', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'customers'
-               firstlineno 158
+               firstlineno 164
                lnotab 0x0203
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016400a6020000ab0200000000000000005300
-               163           0 RESUME                   0
+               169           0 RESUME                   0
                
-               166           2 LOAD_FAST                0 (self)
+               172           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (meta)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('was_acquired')
                             38 LOAD_CONST               0 (None)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 RETURN_VALUE
@@ -1715,31 +1775,31 @@
                   'was_acquired'
                names      ('meta', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'was_acquired'
-               firstlineno 163
+               firstlineno 169
                lnotab 0x0203
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007405000000
                   000000000000007c006a030000000000000000a6010000ab010000000000
                   000000a00400000000000000000000000000000000000000006401a60100
                   00ab010000000000000000a6010000ab010000000000000000a005000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   005300
-               168           0 RESUME                   0
+               174           0 RESUME                   0
                
-               171           2 LOAD_GLOBAL              1 (NULL + hashlib)
+               177           2 LOAD_GLOBAL              1 (NULL + hashlib)
                             14 LOAD_ATTR                1 (md5)
                             24 LOAD_GLOBAL              5 (NULL + str)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                3 (uid)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 LOAD_METHOD              4 (encode)
@@ -1757,34 +1817,34 @@
                   'utf-8'
                names      ('hashlib', 'md5', 'str', 'uid', 'encode', 'hexdigest')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'token'
-               firstlineno 168
+               firstlineno 174
                lnotab 0x0203
             None
          names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'str', 'field', 'dict', 'meta', 'Criteria', 'criteria', 'property', 'notes', 'type', 'prompt', 'products', 'services', 'customers', 'was_acquired', 'token')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Search'
-         firstlineno 127
+         firstlineno 133
          lnotab
             0x0c020a010a012201220402010aff0e01020302010aff0e01020302010a
             ff0e01020302010aff0e01020402010aff0e01020402010aff0e01020402
             010aff0e01020402010aff0e01
       'Search'
-   names      ('hashlib', 'dataclasses', 'asdict', 'dataclass', 'field', 'enum', 'Enum', 'auto', 'typing', 'List', 'Optional', 'Actor', 'Company', 'str', 'EventType', 'Event', 'Comment', 'Rating', 'Inclusion', 'Exclusion', 'Criteria', 'Maps', 'Search')
+   names      ('hashlib', 'dataclasses', 'asdict', 'dataclass', 'field', 'enum', 'Enum', 'auto', 'typing', 'Any', 'List', 'Optional', 'Actor', 'Company', 'str', 'EventType', 'Event', 'Comment', 'Rating', 'Inclusion', 'Exclusion', 'Criteria', 'Maps', 'Search')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010801140110011003020118ff0e01020a160118ff0e0102271e
+      0x00ff02010801140110011403020118ff0e01020a160118ff0e0102271e
       0c020118ff0e01020a02011aff0e01020602011aff0e010205020118ff0e
-      010209020118ff0e010205020118ff0e010207020118ff0e010208020118
+      01020f020118ff0e010205020118ff0e010207020118ff0e010208020118
       ff0e01
```

### Comparing `gandai-1.7.34/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/query.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/__pycache__/tasks.cpython-311.pyc` & `gandai-1.7.35/gandai/__pycache__/tasks.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/analytics.py` & `gandai-1.7.35/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/constants.py` & `gandai-1.7.35/gandai/constants.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/db.py` & `gandai-1.7.35/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/google.py` & `gandai-1.7.35/gandai/google.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/gpt.py` & `gandai-1.7.35/gandai/gpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ## gpt4
 
 
 def ask_gpt4(messages: list) -> json:
     chat_completion = client.chat.completions.create(
         messages=messages,
-        model="gpt-4-0125-preview",
+        model="gpt-4-turbo",
         # model="gpt-4",
         temperature=0.0,
         response_format={"type": "json_object"},
     )
     #
     print(chat_completion.usage)
     return json.loads(chat_completion.choices[0].message.content)
```

### Comparing `gandai-1.7.34/gandai/grata.py` & `gandai-1.7.35/gandai/grata.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/main.py` & `gandai-1.7.35/gandai/main.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.7.35/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/migrations/db_seed.py` & `gandai-1.7.35/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/migrations/dealcloud.py` & `gandai-1.7.35/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/migrations/sql/230818-alter.sql` & `gandai-1.7.35/gandai/migrations/sql/230818-alter.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/migrations/sql/schema.sql` & `gandai-1.7.35/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/models.py` & `gandai-1.7.35/gandai/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import hashlib
 from dataclasses import asdict, dataclass, field
 from enum import Enum, auto
-from typing import List, Optional
+from typing import Any, List, Optional
 
 
 @dataclass
 class Actor:
     # id: int = field(init=False)  # pk
     key: str  # phone number
     type: str
@@ -90,20 +90,26 @@
     def __post_init__(self):
         assert isinstance(self.data["rating"], int)
 
 
 @dataclass
 class Inclusion:
     keywords: List[str] = field(default_factory=list)
-    employees_range: List[int] = field(default_factory=lambda: [100, 500])
+    employees_range: List[Any] = field(default_factory=lambda: [100, 500])
     ownership: List[str] = field(default_factory=lambda: ["bootstrapped"])
     country: List[str] = field(default_factory=lambda: ["USA"])
     state: List[str] = field(default_factory=list)
     city: List[str] = field(default_factory=list)
 
+    def __post_init__(self):
+        if self.employees_range[0] is None:
+            self.employees_range[0] = 0
+        if self.employees_range[1] is None:
+            self.employees_range[1] = 100_000
+
 
 @dataclass
 class Exclusion:
     keywords: List[str] = field(default_factory=list)
     state: List[str] = field(default_factory=list)
```

### Comparing `gandai-1.7.34/gandai/query.py` & `gandai-1.7.35/gandai/query.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/secrets.py` & `gandai-1.7.35/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai/tasks.py` & `gandai-1.7.35/gandai/tasks.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.34/gandai.egg-info/SOURCES.txt` & `gandai-1.7.35/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

