# Comparing `tmp/pygenuz-0.1.0.tar.gz` & `tmp/pygenuz-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenuz-0.1.0.tar", last modified: Mon May  6 09:36:56 2024, max compression
+gzip compressed data, was "pygenuz-0.1.1.tar", last modified: Mon May  6 09:56:20 2024, max compression
```

## Comparing `pygenuz-0.1.0.tar` & `pygenuz-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-06 09:36:56.350189 pygenuz-0.1.0/
--rw-r--r--   0 khezozbek   (501) staff       (20)      660 2024-05-06 09:36:56.350069 pygenuz-0.1.0/PKG-INFO
-drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-06 09:36:56.349898 pygenuz-0.1.0/pygenuz.egg-info/
--rw-r--r--   0 khezozbek   (501) staff       (20)      660 2024-05-06 09:36:56.000000 pygenuz-0.1.0/pygenuz.egg-info/PKG-INFO
--rw-r--r--   0 khezozbek   (501) staff       (20)      162 2024-05-06 09:36:56.000000 pygenuz-0.1.0/pygenuz.egg-info/SOURCES.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-06 09:36:56.000000 pygenuz-0.1.0/pygenuz.egg-info/dependency_links.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)      105 2024-05-06 09:36:56.000000 pygenuz-0.1.0/pygenuz.egg-info/requires.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-06 09:36:56.000000 pygenuz-0.1.0/pygenuz.egg-info/top_level.txt
--rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-06 09:36:56.350238 pygenuz-0.1.0/setup.cfg
--rw-r--r--   0 khezozbek   (501) staff       (20)     3894 2024-05-06 09:36:55.000000 pygenuz-0.1.0/setup.py
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-06 09:56:20.014936 pygenuz-0.1.1/
+-rw-r--r--   0 khezozbek   (501) staff       (20)     8967 2024-05-06 09:56:20.014750 pygenuz-0.1.1/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)     8336 2024-05-06 09:55:31.000000 pygenuz-0.1.1/README.md
+drwxr-xr-x   0 khezozbek   (501) staff       (20)        0 2024-05-06 09:56:20.014567 pygenuz-0.1.1/pygenuz.egg-info/
+-rw-r--r--   0 khezozbek   (501) staff       (20)     8967 2024-05-06 09:56:19.000000 pygenuz-0.1.1/pygenuz.egg-info/PKG-INFO
+-rw-r--r--   0 khezozbek   (501) staff       (20)      172 2024-05-06 09:56:19.000000 pygenuz-0.1.1/pygenuz.egg-info/SOURCES.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-06 09:56:19.000000 pygenuz-0.1.1/pygenuz.egg-info/dependency_links.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)      105 2024-05-06 09:56:19.000000 pygenuz-0.1.1/pygenuz.egg-info/requires.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)        1 2024-05-06 09:56:19.000000 pygenuz-0.1.1/pygenuz.egg-info/top_level.txt
+-rw-r--r--   0 khezozbek   (501) staff       (20)       38 2024-05-06 09:56:20.014993 pygenuz-0.1.1/setup.cfg
+-rw-r--r--   0 khezozbek   (501) staff       (20)     3894 2024-05-06 09:56:17.000000 pygenuz-0.1.1/setup.py
```

### Comparing `pygenuz-0.1.0/setup.py` & `pygenuz-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pygenuz'
 DESCRIPTION = 'My first Python web framework.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'cssezozbel@gmail.com'
 AUTHOR = "E'zozbek Kholbutayev"
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

