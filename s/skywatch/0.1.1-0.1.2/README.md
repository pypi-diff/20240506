# Comparing `tmp/skywatch-0.1.1.tar.gz` & `tmp/skywatch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skywatch-0.1.1.tar", last modified: Sun Apr  7 01:37:56 2024, max compression
+gzip compressed data, was "skywatch-0.1.2.tar", last modified: Mon May  6 02:44:08 2024, max compression
```

## Comparing `skywatch-0.1.1.tar` & `skywatch-0.1.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-04-07 01:37:56.580981 skywatch-0.1.1/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1070 2024-04-04 01:44:39.000000 skywatch-0.1.1/LICENSE.md
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      485 2024-04-07 01:37:56.580981 skywatch-0.1.1/PKG-INFO
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      743 2024-04-04 04:24:08.000000 skywatch-0.1.1/README.md
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       38 2024-04-07 01:37:56.580981 skywatch-0.1.1/setup.cfg
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      601 2024-04-07 01:37:33.000000 skywatch-0.1.1/setup.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-04-07 01:37:56.576981 skywatch-0.1.1/skywatch/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       89 2024-04-07 01:35:29.000000 skywatch-0.1.1/skywatch/__init__.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-04-07 01:37:56.580981 skywatch-0.1.1/skywatch/access/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      110 2024-03-26 04:27:30.000000 skywatch-0.1.1/skywatch/access/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    11714 2024-04-07 01:12:09.000000 skywatch-0.1.1/skywatch/access/access.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      810 2024-04-04 01:53:30.000000 skywatch-0.1.1/skywatch/access/base_constraint.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-04-07 01:37:56.580981 skywatch-0.1.1/skywatch/access/constraints/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      105 2024-03-26 04:27:30.000000 skywatch-0.1.1/skywatch/access/constraints/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     3004 2024-03-26 04:27:30.000000 skywatch-0.1.1/skywatch/access/constraints/az_el_range.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6186 2024-03-26 04:27:30.000000 skywatch-0.1.1/skywatch/access/constraints/line_of_sight.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2189 2024-03-26 04:27:30.000000 skywatch-0.1.1/skywatch/access/constraints/temporal.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      644 2024-04-04 02:02:12.000000 skywatch-0.1.1/skywatch/access/time_interval.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-04-07 01:37:56.580981 skywatch-0.1.1/skywatch/attitude/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       72 2024-03-26 04:27:30.000000 skywatch-0.1.1/skywatch/attitude/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      677 2024-03-26 04:27:30.000000 skywatch-0.1.1/skywatch/attitude/base_attitude.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-04-07 01:37:56.580981 skywatch-0.1.1/skywatch/attitude/builtins/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       77 2024-03-26 04:27:30.000000 skywatch-0.1.1/skywatch/attitude/builtins/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      525 2024-03-26 04:27:30.000000 skywatch-0.1.1/skywatch/attitude/builtins/fixed.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     4437 2024-03-28 04:43:15.000000 skywatch-0.1.1/skywatch/attitude/builtins/lvlh.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      640 2024-03-26 04:27:30.000000 skywatch-0.1.1/skywatch/attitude/builtins/slerped.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-04-07 01:37:56.580981 skywatch-0.1.1/skywatch/look_angles/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      107 2024-03-26 22:07:28.000000 skywatch-0.1.1/skywatch/look_angles/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      195 2024-03-17 22:41:05.000000 skywatch-0.1.1/skywatch/look_angles/aert.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      680 2024-04-04 02:04:42.000000 skywatch-0.1.1/skywatch/look_angles/base_look_angle.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-04-07 01:37:56.580981 skywatch-0.1.1/skywatch/look_angles/builtins/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      102 2024-04-04 02:45:14.000000 skywatch-0.1.1/skywatch/look_angles/builtins/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     6306 2024-04-04 02:44:33.000000 skywatch-0.1.1/skywatch/look_angles/builtins/default_look_strategy.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     2390 2024-04-04 02:44:16.000000 skywatch-0.1.1/skywatch/look_angles/builtins/local_tangent_enu.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-04-07 01:37:56.580981 skywatch-0.1.1/skywatch/skypath/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       29 2024-03-26 04:27:30.000000 skywatch-0.1.1/skywatch/skypath/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     5378 2024-04-04 02:42:47.000000 skywatch-0.1.1/skywatch/skypath/creation.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     8338 2024-04-04 02:43:16.000000 skywatch-0.1.1/skywatch/skypath/skypath.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-04-07 01:37:56.580981 skywatch-0.1.1/skywatch/utils/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       30 2024-03-17 22:41:05.000000 skywatch-0.1.1/skywatch/utils/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)    11345 2024-04-04 02:44:46.000000 skywatch-0.1.1/skywatch/utils/coverage.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     4103 2024-04-04 03:45:44.000000 skywatch-0.1.1/skywatch/utils/funcs.py
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-04-07 01:37:56.576981 skywatch-0.1.1/skywatch.egg-info/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)      485 2024-04-07 01:37:56.000000 skywatch-0.1.1/skywatch.egg-info/PKG-INFO
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1231 2024-04-07 01:37:56.000000 skywatch-0.1.1/skywatch.egg-info/SOURCES.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        1 2024-04-07 01:37:56.000000 skywatch-0.1.1/skywatch.egg-info/dependency_links.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       36 2024-04-07 01:37:56.000000 skywatch-0.1.1/skywatch.egg-info/requires.txt
--rw-rw-r--   0 nathan    (1000) nathan    (1000)       15 2024-04-07 01:37:56.000000 skywatch-0.1.1/skywatch.egg-info/top_level.txt
-drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-04-07 01:37:56.580981 skywatch-0.1.1/tests/
--rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2024-03-26 04:36:18.000000 skywatch-0.1.1/tests/__init__.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1811 2024-04-04 01:37:37.000000 skywatch-0.1.1/tests/geovista_example.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     9876 2024-04-04 02:56:41.000000 skywatch-0.1.1/tests/test_look_angles.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     7334 2024-04-07 00:54:54.000000 skywatch-0.1.1/tests/test_smoke.py
--rw-rw-r--   0 nathan    (1000) nathan    (1000)     1583 2024-03-26 04:27:30.000000 skywatch-0.1.1/tests/utils.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 02:44:08.743999 skywatch-0.1.2/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1070 2024-04-04 01:44:39.000000 skywatch-0.1.2/LICENSE.md
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      485 2024-05-06 02:44:08.743999 skywatch-0.1.2/PKG-INFO
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      743 2024-04-04 04:24:08.000000 skywatch-0.1.2/README.md
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       38 2024-05-06 02:44:08.743999 skywatch-0.1.2/setup.cfg
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      609 2024-05-06 02:41:47.000000 skywatch-0.1.2/setup.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 02:44:08.739999 skywatch-0.1.2/skywatch/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       89 2024-05-06 02:41:19.000000 skywatch-0.1.2/skywatch/__init__.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 02:44:08.739999 skywatch-0.1.2/skywatch/access/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      110 2024-03-26 04:27:30.000000 skywatch-0.1.2/skywatch/access/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    11714 2024-05-06 02:41:19.000000 skywatch-0.1.2/skywatch/access/access.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      810 2024-04-04 01:53:30.000000 skywatch-0.1.2/skywatch/access/base_constraint.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 02:44:08.739999 skywatch-0.1.2/skywatch/access/constraints/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      105 2024-03-26 04:27:30.000000 skywatch-0.1.2/skywatch/access/constraints/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     3004 2024-05-06 02:41:19.000000 skywatch-0.1.2/skywatch/access/constraints/az_el_range.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6186 2024-03-26 04:27:30.000000 skywatch-0.1.2/skywatch/access/constraints/line_of_sight.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2189 2024-03-26 04:27:30.000000 skywatch-0.1.2/skywatch/access/constraints/temporal.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      644 2024-04-04 02:02:12.000000 skywatch-0.1.2/skywatch/access/time_interval.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 02:44:08.739999 skywatch-0.1.2/skywatch/attitude/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       72 2024-03-26 04:27:30.000000 skywatch-0.1.2/skywatch/attitude/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      677 2024-03-26 04:27:30.000000 skywatch-0.1.2/skywatch/attitude/base_attitude.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 02:44:08.743999 skywatch-0.1.2/skywatch/attitude/builtins/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       77 2024-03-26 04:27:30.000000 skywatch-0.1.2/skywatch/attitude/builtins/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      525 2024-03-26 04:27:30.000000 skywatch-0.1.2/skywatch/attitude/builtins/fixed.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     4437 2024-03-28 04:43:15.000000 skywatch-0.1.2/skywatch/attitude/builtins/lvlh.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      640 2024-03-26 04:27:30.000000 skywatch-0.1.2/skywatch/attitude/builtins/slerped.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 02:44:08.743999 skywatch-0.1.2/skywatch/look_angles/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      107 2024-03-26 22:07:28.000000 skywatch-0.1.2/skywatch/look_angles/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      195 2024-03-17 22:41:05.000000 skywatch-0.1.2/skywatch/look_angles/aert.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      680 2024-04-04 02:04:42.000000 skywatch-0.1.2/skywatch/look_angles/base_look_angle.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 02:44:08.743999 skywatch-0.1.2/skywatch/look_angles/builtins/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      102 2024-04-04 02:45:14.000000 skywatch-0.1.2/skywatch/look_angles/builtins/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     6306 2024-04-04 02:44:33.000000 skywatch-0.1.2/skywatch/look_angles/builtins/default_look_strategy.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2390 2024-04-04 02:44:16.000000 skywatch-0.1.2/skywatch/look_angles/builtins/local_tangent_enu.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 02:44:08.743999 skywatch-0.1.2/skywatch/skypath/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       29 2024-03-26 04:27:30.000000 skywatch-0.1.2/skywatch/skypath/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5378 2024-04-04 02:42:47.000000 skywatch-0.1.2/skywatch/skypath/creation.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     8338 2024-04-04 02:43:16.000000 skywatch-0.1.2/skywatch/skypath/skypath.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 02:44:08.743999 skywatch-0.1.2/skywatch/utils/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       30 2024-03-17 22:41:05.000000 skywatch-0.1.2/skywatch/utils/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    11345 2024-05-06 02:41:19.000000 skywatch-0.1.2/skywatch/utils/coverage.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     4103 2024-04-04 03:45:44.000000 skywatch-0.1.2/skywatch/utils/funcs.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 02:44:08.739999 skywatch-0.1.2/skywatch.egg-info/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      485 2024-05-06 02:44:08.000000 skywatch-0.1.2/skywatch.egg-info/PKG-INFO
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1231 2024-05-06 02:44:08.000000 skywatch-0.1.2/skywatch.egg-info/SOURCES.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        1 2024-05-06 02:44:08.000000 skywatch-0.1.2/skywatch.egg-info/dependency_links.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       41 2024-05-06 02:44:08.000000 skywatch-0.1.2/skywatch.egg-info/requires.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       15 2024-05-06 02:44:08.000000 skywatch-0.1.2/skywatch.egg-info/top_level.txt
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-06 02:44:08.743999 skywatch-0.1.2/tests/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        0 2024-03-26 04:36:18.000000 skywatch-0.1.2/tests/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1811 2024-04-04 01:37:37.000000 skywatch-0.1.2/tests/geovista_example.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     9876 2024-04-04 02:56:41.000000 skywatch-0.1.2/tests/test_look_angles.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     7334 2024-05-06 02:41:19.000000 skywatch-0.1.2/tests/test_smoke.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1583 2024-03-26 04:27:30.000000 skywatch-0.1.2/tests/utils.py
```

### Comparing `skywatch-0.1.1/LICENSE.md` & `skywatch-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/README.md` & `skywatch-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/setup.py` & `skywatch-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import find_packages, setup
 
 setup(
     name="skywatch",
-    version="0.1.1",
+    version="0.1.2",
     url="https://github.com/nsspencer/SkyWatch",
     author="Nathan Spencer",
     description="Aerospace/astrodynamics analysis library providing high level interfaces for coordinate, attitude, access, and look angle calculations.",
     packages=find_packages(),
-    install_requires=["astropy", "numpy", "portion", "scipy", "pymap3d"],
+    install_requires=["astropy", "numpy", "portion", "scipy", "pymap3d", "tqdm"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `skywatch-0.1.1/skywatch/access/access.py` & `skywatch-0.1.2/skywatch/access/access.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/skywatch/access/base_constraint.py` & `skywatch-0.1.2/skywatch/access/base_constraint.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/skywatch/access/constraints/az_el_range.py` & `skywatch-0.1.2/skywatch/access/constraints/az_el_range.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/skywatch/access/constraints/line_of_sight.py` & `skywatch-0.1.2/skywatch/access/constraints/line_of_sight.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/skywatch/access/constraints/temporal.py` & `skywatch-0.1.2/skywatch/access/constraints/temporal.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/skywatch/access/time_interval.py` & `skywatch-0.1.2/skywatch/access/time_interval.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/skywatch/attitude/base_attitude.py` & `skywatch-0.1.2/skywatch/attitude/base_attitude.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/skywatch/attitude/builtins/fixed.py` & `skywatch-0.1.2/skywatch/attitude/builtins/fixed.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/skywatch/attitude/builtins/lvlh.py` & `skywatch-0.1.2/skywatch/attitude/builtins/lvlh.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/skywatch/attitude/builtins/slerped.py` & `skywatch-0.1.2/skywatch/attitude/builtins/slerped.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/skywatch/look_angles/base_look_angle.py` & `skywatch-0.1.2/skywatch/look_angles/base_look_angle.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/skywatch/look_angles/builtins/default_look_strategy.py` & `skywatch-0.1.2/skywatch/look_angles/builtins/default_look_strategy.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/skywatch/look_angles/builtins/local_tangent_enu.py` & `skywatch-0.1.2/skywatch/look_angles/builtins/local_tangent_enu.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/skywatch/skypath/creation.py` & `skywatch-0.1.2/skywatch/skypath/creation.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/skywatch/skypath/skypath.py` & `skywatch-0.1.2/skywatch/skypath/skypath.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/skywatch/utils/coverage.py` & `skywatch-0.1.2/skywatch/utils/coverage.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/skywatch/utils/funcs.py` & `skywatch-0.1.2/skywatch/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/skywatch.egg-info/SOURCES.txt` & `skywatch-0.1.2/skywatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/tests/geovista_example.py` & `skywatch-0.1.2/tests/geovista_example.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/tests/test_look_angles.py` & `skywatch-0.1.2/tests/test_look_angles.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/tests/test_smoke.py` & `skywatch-0.1.2/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skywatch-0.1.1/tests/utils.py` & `skywatch-0.1.2/tests/utils.py`

 * *Files identical despite different names*

