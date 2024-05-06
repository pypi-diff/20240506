# Comparing `tmp/chess_scanparsers-0.0.8.tar.gz` & `tmp/chess_scanparsers-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_scanparsers-0.0.8.tar", last modified: Mon May  6 19:25:53 2024, max compression
+gzip compressed data, was "chess_scanparsers-0.0.9.tar", last modified: Mon May  6 19:27:46 2024, max compression
```

## Comparing `chess_scanparsers-0.0.8.tar` & `chess_scanparsers-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:25:53.360324 chess_scanparsers-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 19:25:53.360324 chess_scanparsers-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:25:47.000000 chess_scanparsers-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:25:53.360324 chess_scanparsers-0.0.8/chess-scanparsers/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-06 19:25:51.000000 chess_scanparsers-0.0.8/chess-scanparsers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51762 2024-05-06 19:25:47.000000 chess_scanparsers-0.0.8/chess-scanparsers/scanparsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:25:53.360324 chess_scanparsers-0.0.8/chess_scanparsers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 19:25:53.000000 chess_scanparsers-0.0.8/chess_scanparsers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-06 19:25:53.000000 chess_scanparsers-0.0.8/chess_scanparsers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:25:53.000000 chess_scanparsers-0.0.8/chess_scanparsers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-06 19:25:53.000000 chess_scanparsers-0.0.8/chess_scanparsers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 19:25:53.000000 chess_scanparsers-0.0.8/chess_scanparsers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:25:53.360324 chess_scanparsers-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1125 2024-05-06 19:25:51.000000 chess_scanparsers-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:27:46.787171 chess_scanparsers-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 19:27:46.787171 chess_scanparsers-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:27:40.000000 chess_scanparsers-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:27:46.783172 chess_scanparsers-0.0.9/chess-scanparsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-06 19:27:44.000000 chess_scanparsers-0.0.9/chess-scanparsers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51762 2024-05-06 19:27:40.000000 chess_scanparsers-0.0.9/chess-scanparsers/scanparsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:27:46.787171 chess_scanparsers-0.0.9/chess_scanparsers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 19:27:46.000000 chess_scanparsers-0.0.9/chess_scanparsers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-06 19:27:46.000000 chess_scanparsers-0.0.9/chess_scanparsers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:27:46.000000 chess_scanparsers-0.0.9/chess_scanparsers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-06 19:27:46.000000 chess_scanparsers-0.0.9/chess_scanparsers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 19:27:46.000000 chess_scanparsers-0.0.9/chess_scanparsers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:27:46.787171 chess_scanparsers-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1125 2024-05-06 19:27:44.000000 chess_scanparsers-0.0.9/setup.py
```

### Comparing `chess_scanparsers-0.0.8/chess-scanparsers/scanparsers.py` & `chess_scanparsers-0.0.9/chess-scanparsers/scanparsers.py`

 * *Files identical despite different names*

### Comparing `chess_scanparsers-0.0.8/setup.py` & `chess_scanparsers-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 to run tests : python setup.py test
 """
 
 import os
 import setuptools
 
 # [set version]
-version = 'v0.0.8'
+version = 'v0.0.9'
 # [version set]
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='chess-scanparsers',
```

