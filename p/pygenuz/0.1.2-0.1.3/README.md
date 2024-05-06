# Comparing `tmp/pygenuz-0.1.2.tar.gz` & `tmp/pygenuz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenuz-0.1.2.tar", last modified: Mon May  6 10:00:21 2024, max compression
+gzip compressed data, was "pygenuz-0.1.3.tar", last modified: Mon May  6 10:08:39 2024, max compression
```

## Comparing `pygenuz-0.1.2.tar` & `pygenuz-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,16 @@
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-06 10:00:21.870694 pygenuz-0.1.2/
--rw-r--r--   0 khezozbek   (501) staff       (20)     9038 2024-05-06 10:00:21.870206 pygenuz-0.1.2/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)     8407 2024-05-06 10:00:00.000000 pygenuz-0.1.2/README.md
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-06 10:00:21.869892 pygenuz-0.1.2/pygenuz.egg-info/
--rw-r--r--   0 khezozbek   (501) staff       (20)     9038 2024-05-06 10:00:21.000000 pygenuz-0.1.2/pygenuz.egg-info/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)      172 2024-05-06 10:00:21.000000 pygenuz-0.1.2/pygenuz.egg-info/SOURCES.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-06 10:00:21.000000 pygenuz-0.1.2/pygenuz.egg-info/dependency_links.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)      105 2024-05-06 10:00:21.000000 pygenuz-0.1.2/pygenuz.egg-info/requires.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-06 10:00:21.000000 pygenuz-0.1.2/pygenuz.egg-info/top_level.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-06 10:00:21.870792 pygenuz-0.1.2/setup.cfg
--rw-r--r--   0 khezozbek   (501) staff       (20)     3894 2024-05-06 10:00:17.000000 pygenuz-0.1.2/setup.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-06 10:08:39.264345 pygenuz-0.1.3/
+-rw-r--r--   0 khezozbek   (501) staff       (20)     9038 2024-05-06 10:08:39.264062 pygenuz-0.1.3/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)     8407 2024-05-06 10:00:00.000000 pygenuz-0.1.3/README.md
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-06 10:08:39.262987 pygenuz-0.1.3/pygenuz/
+-rw-r--r--   0 khezozbek   (501) staff       (20)        0 2024-05-06 10:08:02.000000 pygenuz-0.1.3/pygenuz/__init__.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3785 2024-05-06 09:20:00.000000 pygenuz-0.1.3/pygenuz/app.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      680 2024-05-06 07:56:45.000000 pygenuz-0.1.3/pygenuz/middelware.py
+-rw-r--r--   0 khezozbek   (501) staff       (20)      953 2024-05-06 09:07:08.000000 pygenuz-0.1.3/pygenuz/response.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-06 10:08:39.263851 pygenuz-0.1.3/pygenuz.egg-info/
+-rw-r--r--   0 khezozbek   (501) staff       (20)     9038 2024-05-06 10:08:39.000000 pygenuz-0.1.3/pygenuz.egg-info/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)      249 2024-05-06 10:08:39.000000 pygenuz-0.1.3/pygenuz.egg-info/SOURCES.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-06 10:08:39.000000 pygenuz-0.1.3/pygenuz.egg-info/dependency_links.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)      105 2024-05-06 10:08:39.000000 pygenuz-0.1.3/pygenuz.egg-info/requires.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        8 2024-05-06 10:08:39.000000 pygenuz-0.1.3/pygenuz.egg-info/top_level.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-06 10:08:39.264405 pygenuz-0.1.3/setup.cfg
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3894 2024-05-06 10:08:24.000000 pygenuz-0.1.3/setup.py
```

### Comparing `pygenuz-0.1.2/PKG-INFO` & `pygenuz-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenuz
-Version: 0.1.2
+Version: 0.1.3
 Summary: My first Python web framework.
 Home-page: https://github.com/me/myproject
 Author: E'zozbek Kholbutayev
 Author-email: cssezozbel@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygenuz-0.1.2/README.md` & `pygenuz-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pygenuz-0.1.2/pygenuz.egg-info/PKG-INFO` & `pygenuz-0.1.3/pygenuz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenuz
-Version: 0.1.2
+Version: 0.1.3
 Summary: My first Python web framework.
 Home-page: https://github.com/me/myproject
 Author: E'zozbek Kholbutayev
 Author-email: cssezozbel@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygenuz-0.1.2/setup.py` & `pygenuz-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pygenuz'
 DESCRIPTION = 'My first Python web framework.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'cssezozbel@gmail.com'
 AUTHOR = "E'zozbek Kholbutayev"
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

