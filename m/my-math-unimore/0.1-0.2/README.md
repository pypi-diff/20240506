# Comparing `tmp/my_math_unimore-0.1.tar.gz` & `tmp/my_math_unimore-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_math_unimore-0.1.tar", last modified: Mon May  6 07:42:06 2024, max compression
+gzip compressed data, was "my_math_unimore-0.2.tar", last modified: Mon May  6 07:57:01 2024, max compression
```

## Comparing `my_math_unimore-0.1.tar` & `my_math_unimore-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:42:06.593406 my_math_unimore-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 07:42:06.593406 my_math_unimore-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 07:42:02.000000 my_math_unimore-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:42:06.593406 my_math_unimore-0.1/my_math_unimore/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 07:42:02.000000 my_math_unimore-0.1/my_math_unimore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-06 07:42:02.000000 my_math_unimore-0.1/my_math_unimore/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-06 07:42:02.000000 my_math_unimore-0.1/my_math_unimore/test_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:42:06.593406 my_math_unimore-0.1/my_math_unimore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 07:42:06.000000 my_math_unimore-0.1/my_math_unimore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 07:42:06.000000 my_math_unimore-0.1/my_math_unimore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 07:42:06.000000 my_math_unimore-0.1/my_math_unimore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 07:42:06.000000 my_math_unimore-0.1/my_math_unimore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 07:42:06.000000 my_math_unimore-0.1/my_math_unimore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 07:42:06.593406 my_math_unimore-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-06 07:42:02.000000 my_math_unimore-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:57:01.754320 my_math_unimore-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 07:57:01.754320 my_math_unimore-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 07:56:57.000000 my_math_unimore-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:57:01.750320 my_math_unimore-0.2/my_math_unimore/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 07:56:57.000000 my_math_unimore-0.2/my_math_unimore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-06 07:56:57.000000 my_math_unimore-0.2/my_math_unimore/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-06 07:56:57.000000 my_math_unimore-0.2/my_math_unimore/test_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:57:01.754320 my_math_unimore-0.2/my_math_unimore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 07:57:01.000000 my_math_unimore-0.2/my_math_unimore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 07:57:01.000000 my_math_unimore-0.2/my_math_unimore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 07:57:01.000000 my_math_unimore-0.2/my_math_unimore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 07:57:01.000000 my_math_unimore-0.2/my_math_unimore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 07:57:01.000000 my_math_unimore-0.2/my_math_unimore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 07:57:01.754320 my_math_unimore-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-06 07:56:57.000000 my_math_unimore-0.2/setup.py
```

### Comparing `my_math_unimore-0.1/my_math_unimore/test_calculator.py` & `my_math_unimore-0.2/my_math_unimore/test_calculator.py`

 * *Files identical despite different names*

