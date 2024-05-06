# Comparing `tmp/chess_scanparsers-0.0.6.tar.gz` & `tmp/chess_scanparsers-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_scanparsers-0.0.6.tar", last modified: Mon May  6 19:21:26 2024, max compression
+gzip compressed data, was "chess_scanparsers-0.0.7.tar", last modified: Mon May  6 19:23:07 2024, max compression
```

## Comparing `chess_scanparsers-0.0.6.tar` & `chess_scanparsers-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:21:26.912024 chess_scanparsers-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 19:21:26.912024 chess_scanparsers-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:21:21.000000 chess_scanparsers-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:21:26.908024 chess_scanparsers-0.0.6/chess-scanparsers/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-06 19:21:25.000000 chess_scanparsers-0.0.6/chess-scanparsers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51802 2024-05-06 19:21:21.000000 chess_scanparsers-0.0.6/chess-scanparsers/scanparsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:21:26.912024 chess_scanparsers-0.0.6/chess_scanparsers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 19:21:26.000000 chess_scanparsers-0.0.6/chess_scanparsers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-06 19:21:26.000000 chess_scanparsers-0.0.6/chess_scanparsers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:21:26.000000 chess_scanparsers-0.0.6/chess_scanparsers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-06 19:21:26.000000 chess_scanparsers-0.0.6/chess_scanparsers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 19:21:26.000000 chess_scanparsers-0.0.6/chess_scanparsers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:21:26.912024 chess_scanparsers-0.0.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1125 2024-05-06 19:21:25.000000 chess_scanparsers-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:23:07.178828 chess_scanparsers-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 19:23:07.178828 chess_scanparsers-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:23:01.000000 chess_scanparsers-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:23:07.178828 chess_scanparsers-0.0.7/chess-scanparsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-06 19:23:05.000000 chess_scanparsers-0.0.7/chess-scanparsers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51734 2024-05-06 19:23:01.000000 chess_scanparsers-0.0.7/chess-scanparsers/scanparsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:23:07.178828 chess_scanparsers-0.0.7/chess_scanparsers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 19:23:07.000000 chess_scanparsers-0.0.7/chess_scanparsers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-06 19:23:07.000000 chess_scanparsers-0.0.7/chess_scanparsers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:23:07.000000 chess_scanparsers-0.0.7/chess_scanparsers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-06 19:23:07.000000 chess_scanparsers-0.0.7/chess_scanparsers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 19:23:07.000000 chess_scanparsers-0.0.7/chess_scanparsers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:23:07.178828 chess_scanparsers-0.0.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1125 2024-05-06 19:23:05.000000 chess_scanparsers-0.0.7/setup.py
```

### Comparing `chess_scanparsers-0.0.6/chess-scanparsers/scanparsers.py` & `chess_scanparsers-0.0.7/chess-scanparsers/scanparsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,18 +51,15 @@
     some of its metadata.
 
     :param spec_file_name: path to a SPEC file on the CLASSE DAQ
     :type spec_file_name: str
     :param scan_number: the number of a scan in the SPEC file provided
         with `spec_file_name`
     :type scan_number: int
-    """
-    property_names = ['scan_path']
-    for name in property_names:
-        
+    """        
     
     def __init__(self,
                  spec_file_name:str,
                  scan_number:int):
         """Constructor method"""
 
         self.spec_file_name = spec_file_name
```

### Comparing `chess_scanparsers-0.0.6/setup.py` & `chess_scanparsers-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 to run tests : python setup.py test
 """
 
 import os
 import setuptools
 
 # [set version]
-version = 'v0.0.6'
+version = 'v0.0.7'
 # [version set]
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='chess-scanparsers',
```

