# Comparing `tmp/chess_scanparsers-0.0.7.tar.gz` & `tmp/chess_scanparsers-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_scanparsers-0.0.7.tar", last modified: Mon May  6 19:23:07 2024, max compression
+gzip compressed data, was "chess_scanparsers-0.0.8.tar", last modified: Mon May  6 19:25:53 2024, max compression
```

## Comparing `chess_scanparsers-0.0.7.tar` & `chess_scanparsers-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:23:07.178828 chess_scanparsers-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 19:23:07.178828 chess_scanparsers-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:23:01.000000 chess_scanparsers-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:23:07.178828 chess_scanparsers-0.0.7/chess-scanparsers/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-06 19:23:05.000000 chess_scanparsers-0.0.7/chess-scanparsers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51734 2024-05-06 19:23:01.000000 chess_scanparsers-0.0.7/chess-scanparsers/scanparsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:23:07.178828 chess_scanparsers-0.0.7/chess_scanparsers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 19:23:07.000000 chess_scanparsers-0.0.7/chess_scanparsers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-06 19:23:07.000000 chess_scanparsers-0.0.7/chess_scanparsers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:23:07.000000 chess_scanparsers-0.0.7/chess_scanparsers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-06 19:23:07.000000 chess_scanparsers-0.0.7/chess_scanparsers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 19:23:07.000000 chess_scanparsers-0.0.7/chess_scanparsers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:23:07.178828 chess_scanparsers-0.0.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1125 2024-05-06 19:23:05.000000 chess_scanparsers-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:25:53.360324 chess_scanparsers-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 19:25:53.360324 chess_scanparsers-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:25:47.000000 chess_scanparsers-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:25:53.360324 chess_scanparsers-0.0.8/chess-scanparsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-06 19:25:51.000000 chess_scanparsers-0.0.8/chess-scanparsers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51762 2024-05-06 19:25:47.000000 chess_scanparsers-0.0.8/chess-scanparsers/scanparsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:25:53.360324 chess_scanparsers-0.0.8/chess_scanparsers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-06 19:25:53.000000 chess_scanparsers-0.0.8/chess_scanparsers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-06 19:25:53.000000 chess_scanparsers-0.0.8/chess_scanparsers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:25:53.000000 chess_scanparsers-0.0.8/chess_scanparsers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-06 19:25:53.000000 chess_scanparsers-0.0.8/chess_scanparsers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 19:25:53.000000 chess_scanparsers-0.0.8/chess_scanparsers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:25:53.360324 chess_scanparsers-0.0.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1125 2024-05-06 19:25:51.000000 chess_scanparsers-0.0.8/setup.py
```

### Comparing `chess_scanparsers-0.0.7/chess-scanparsers/scanparsers.py` & `chess_scanparsers-0.0.8/chess-scanparsers/scanparsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -454,33 +454,33 @@
             m1_end = float(self.spec_args[2])
             m1_npt = int(self.spec_args[3]) + 1
             try:
                 # Try post-summer-2022 format                                   
                 dwell = float(self.spec_args[4])
             except:
                 # Accommodate pre-summer-2022 format                            
-		m2_start_i = 5
+                m2_start_i = 5
                 m2_end_i = 6
                 m2_nint_i = 7
             else:
                 m2_start_i = 6
                 m2_end_i = 7
                 m2_nint_i = 8
             m2_start = float(self.spec_args[m2_start_i])
             m2_end = float(self.spec_args[m2_end_i])
             m2_npt = int(self.spec_args[m2_nint_i]) + 1
             fast_mot_vals = np.linspace(m1_start, m1_end, m1_npt)
-	    slow_mot_vals = np.linspace(m2_start, m2_end, m2_npt)
+            slow_mot_vals = np.linspace(m2_start, m2_end, m2_npt)
             return (fast_mot_vals, slow_mot_vals)
         if self.spec_macro in ('flyscan', 'ascan'):
             mot_vals = np.linspace(float(self.spec_args[1]),
                                    float(self.spec_args[2]),
                                    int(self.spec_args[3])+1)
             return (mot_vals,)
-	if self.spec_macro in ('tseries', 'loopscan'):
+        if self.spec_macro in ('tseries', 'loopscan'):
             return (self.spec_scan.data[:,0],)
         raise RuntimeError(f'{self.scan_title}: cannot determine scan motors '
                            f'for scans of type {self.spec_macro}')
 
     @cached_property
     def spec_scan_shape(self):
         """A tuple representing the shape of the spec scan -- how many
```

### Comparing `chess_scanparsers-0.0.7/setup.py` & `chess_scanparsers-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 to run tests : python setup.py test
 """
 
 import os
 import setuptools
 
 # [set version]
-version = 'v0.0.7'
+version = 'v0.0.8'
 # [version set]
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='chess-scanparsers',
```

