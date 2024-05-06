# Comparing `tmp/my_math_unimore-0.2.tar.gz` & `tmp/my_math_unimore-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_math_unimore-0.2.tar", last modified: Mon May  6 07:57:01 2024, max compression
+gzip compressed data, was "my_math_unimore-0.3.tar", last modified: Mon May  6 08:06:17 2024, max compression
```

## Comparing `my_math_unimore-0.2.tar` & `my_math_unimore-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:57:01.754320 my_math_unimore-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 07:57:01.754320 my_math_unimore-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 07:56:57.000000 my_math_unimore-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:57:01.750320 my_math_unimore-0.2/my_math_unimore/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 07:56:57.000000 my_math_unimore-0.2/my_math_unimore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-06 07:56:57.000000 my_math_unimore-0.2/my_math_unimore/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-06 07:56:57.000000 my_math_unimore-0.2/my_math_unimore/test_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:57:01.754320 my_math_unimore-0.2/my_math_unimore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 07:57:01.000000 my_math_unimore-0.2/my_math_unimore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 07:57:01.000000 my_math_unimore-0.2/my_math_unimore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 07:57:01.000000 my_math_unimore-0.2/my_math_unimore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 07:57:01.000000 my_math_unimore-0.2/my_math_unimore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 07:57:01.000000 my_math_unimore-0.2/my_math_unimore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 07:57:01.754320 my_math_unimore-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-06 07:56:57.000000 my_math_unimore-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:06:17.356411 my_math_unimore-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 08:06:17.356411 my_math_unimore-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 08:06:13.000000 my_math_unimore-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:06:17.356411 my_math_unimore-0.3/my_math_unimore/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 08:06:13.000000 my_math_unimore-0.3/my_math_unimore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-06 08:06:13.000000 my_math_unimore-0.3/my_math_unimore/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-06 08:06:13.000000 my_math_unimore-0.3/my_math_unimore/test_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:06:17.356411 my_math_unimore-0.3/my_math_unimore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 08:06:17.000000 my_math_unimore-0.3/my_math_unimore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-06 08:06:17.000000 my_math_unimore-0.3/my_math_unimore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:06:17.000000 my_math_unimore-0.3/my_math_unimore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 08:06:17.000000 my_math_unimore-0.3/my_math_unimore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 08:06:17.000000 my_math_unimore-0.3/my_math_unimore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:06:17.356411 my_math_unimore-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-06 08:06:13.000000 my_math_unimore-0.3/setup.py
```

### Comparing `my_math_unimore-0.2/my_math_unimore/test_calculator.py` & `my_math_unimore-0.3/my_math_unimore/test_calculator.py`

 * *Files identical despite different names*

