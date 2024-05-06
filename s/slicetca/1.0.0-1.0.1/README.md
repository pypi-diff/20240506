# Comparing `tmp/slicetca-1.0.0.tar.gz` & `tmp/slicetca-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slicetca-1.0.0.tar", last modified: Mon May  6 11:22:46 2024, max compression
+gzip compressed data, was "slicetca-1.0.1.tar", last modified: Mon May  6 11:38:27 2024, max compression
```

## Comparing `slicetca-1.0.0.tar` & `slicetca-1.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:22:46.253472 slicetca-1.0.0/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1116 2023-03-06 11:26:01.000000 slicetca-1.0.0/LICENSE.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2330 2024-05-06 11:22:46.253472 slicetca-1.0.0/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1810 2024-05-06 08:16:50.000000 slicetca-1.0.0/README.md
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       79 2024-05-06 11:22:46.253472 slicetca-1.0.0/setup.cfg
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      975 2024-05-06 11:22:44.000000 slicetca-1.0.0/setup.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:22:46.249472 slicetca-1.0.0/slicetca/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      214 2023-03-07 11:24:31.000000 slicetca-1.0.0/slicetca/__init__.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:22:46.253472 slicetca-1.0.0/slicetca/core/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       77 2023-01-03 10:29:24.000000 slicetca-1.0.0/slicetca/core/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    13265 2023-08-21 21:40:43.000000 slicetca-1.0.0/slicetca/core/decompositions.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      322 2023-08-21 21:40:43.000000 slicetca-1.0.0/slicetca/core/helper_functions.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:22:46.253472 slicetca-1.0.0/slicetca/invariance/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       80 2023-03-06 12:10:37.000000 slicetca-1.0.0/slicetca/invariance/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1352 2023-03-02 09:01:48.000000 slicetca-1.0.0/slicetca/invariance/analytic_invariance.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1179 2023-01-03 10:28:16.000000 slicetca-1.0.0/slicetca/invariance/criteria.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1865 2023-03-06 12:14:41.000000 slicetca-1.0.0/slicetca/invariance/helper.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1219 2023-08-21 21:46:56.000000 slicetca-1.0.0/slicetca/invariance/invariance.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2681 2023-03-06 12:14:41.000000 slicetca-1.0.0/slicetca/invariance/iterative_invariance.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     4323 2023-01-03 10:28:16.000000 slicetca-1.0.0/slicetca/invariance/transformations.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:22:46.253472 slicetca-1.0.0/slicetca/plotting/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       86 2024-05-06 09:28:28.000000 slicetca-1.0.0/slicetca/plotting/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2022-12-29 06:45:13.000000 slicetca-1.0.0/slicetca/plotting/additional.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     7034 2023-03-07 11:02:58.000000 slicetca-1.0.0/slicetca/plotting/factors.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     3765 2024-05-06 11:18:23.000000 slicetca-1.0.0/slicetca/plotting/grid.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:22:46.253472 slicetca-1.0.0/slicetca/run/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      127 2023-03-03 12:58:54.000000 slicetca-1.0.0/slicetca/run/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     3484 2023-08-21 21:40:43.000000 slicetca-1.0.0/slicetca/run/decompose.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     5085 2023-08-21 21:29:47.000000 slicetca-1.0.0/slicetca/run/grid_search.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2657 2023-03-03 14:21:07.000000 slicetca-1.0.0/slicetca/run/utils.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:22:46.253472 slicetca-1.0.0/slicetca/tests/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-03-02 08:55:06.000000 slicetca-1.0.0/slicetca/tests/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     3966 2023-03-06 12:14:41.000000 slicetca-1.0.0/slicetca/tests/tests.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:22:46.253472 slicetca-1.0.0/slicetca.egg-info/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2330 2024-05-06 11:22:46.000000 slicetca-1.0.0/slicetca.egg-info/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      835 2024-05-06 11:22:46.000000 slicetca-1.0.0/slicetca.egg-info/SOURCES.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2024-05-06 11:22:46.000000 slicetca-1.0.0/slicetca.egg-info/dependency_links.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       34 2024-05-06 11:22:46.000000 slicetca-1.0.0/slicetca.egg-info/requires.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        9 2024-05-06 11:22:46.000000 slicetca-1.0.0/slicetca.egg-info/top_level.txt
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:38:27.306663 slicetca-1.0.1/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1116 2023-03-06 11:26:01.000000 slicetca-1.0.1/LICENSE.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2330 2024-05-06 11:38:27.306663 slicetca-1.0.1/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1810 2024-05-06 08:16:50.000000 slicetca-1.0.1/README.md
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       79 2024-05-06 11:38:27.306663 slicetca-1.0.1/setup.cfg
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      975 2024-05-06 11:38:26.000000 slicetca-1.0.1/setup.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:38:27.306663 slicetca-1.0.1/slicetca/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      227 2024-05-06 11:37:45.000000 slicetca-1.0.1/slicetca/__init__.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:38:27.306663 slicetca-1.0.1/slicetca/core/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       77 2023-01-03 10:29:24.000000 slicetca-1.0.1/slicetca/core/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    13265 2023-08-21 21:40:43.000000 slicetca-1.0.1/slicetca/core/decompositions.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      322 2023-08-21 21:40:43.000000 slicetca-1.0.1/slicetca/core/helper_functions.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:38:27.306663 slicetca-1.0.1/slicetca/invariance/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       80 2023-03-06 12:10:37.000000 slicetca-1.0.1/slicetca/invariance/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1352 2023-03-02 09:01:48.000000 slicetca-1.0.1/slicetca/invariance/analytic_invariance.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1179 2023-01-03 10:28:16.000000 slicetca-1.0.1/slicetca/invariance/criteria.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1865 2023-03-06 12:14:41.000000 slicetca-1.0.1/slicetca/invariance/helper.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1219 2023-08-21 21:46:56.000000 slicetca-1.0.1/slicetca/invariance/invariance.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2681 2023-03-06 12:14:41.000000 slicetca-1.0.1/slicetca/invariance/iterative_invariance.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     4323 2023-01-03 10:28:16.000000 slicetca-1.0.1/slicetca/invariance/transformations.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:38:27.306663 slicetca-1.0.1/slicetca/plotting/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       86 2024-05-06 09:28:28.000000 slicetca-1.0.1/slicetca/plotting/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2022-12-29 06:45:13.000000 slicetca-1.0.1/slicetca/plotting/additional.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     7034 2023-03-07 11:02:58.000000 slicetca-1.0.1/slicetca/plotting/factors.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3765 2024-05-06 11:18:23.000000 slicetca-1.0.1/slicetca/plotting/grid.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:38:27.306663 slicetca-1.0.1/slicetca/run/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      127 2023-03-03 12:58:54.000000 slicetca-1.0.1/slicetca/run/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3484 2023-08-21 21:40:43.000000 slicetca-1.0.1/slicetca/run/decompose.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     5085 2023-08-21 21:29:47.000000 slicetca-1.0.1/slicetca/run/grid_search.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2657 2023-03-03 14:21:07.000000 slicetca-1.0.1/slicetca/run/utils.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:38:27.306663 slicetca-1.0.1/slicetca/tests/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-03-02 08:55:06.000000 slicetca-1.0.1/slicetca/tests/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3966 2023-03-06 12:14:41.000000 slicetca-1.0.1/slicetca/tests/tests.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:38:27.306663 slicetca-1.0.1/slicetca.egg-info/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2330 2024-05-06 11:38:27.000000 slicetca-1.0.1/slicetca.egg-info/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      835 2024-05-06 11:38:27.000000 slicetca-1.0.1/slicetca.egg-info/SOURCES.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2024-05-06 11:38:27.000000 slicetca-1.0.1/slicetca.egg-info/dependency_links.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       34 2024-05-06 11:38:27.000000 slicetca-1.0.1/slicetca.egg-info/requires.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        9 2024-05-06 11:38:27.000000 slicetca-1.0.1/slicetca.egg-info/top_level.txt
```

### Comparing `slicetca-1.0.0/LICENSE.txt` & `slicetca-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.0/PKG-INFO` & `slicetca-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slicetca
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package to perform Slice Tensor Component Analysis
 Home-page: https://github.com/arthur-pe/slicetca
 Author: Arthur Pellegrino
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `slicetca-1.0.0/README.md` & `slicetca-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.0/setup.py` & `slicetca-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='slicetca',
     packages=find_packages(exclude=['tests*']),
-    version='1.0.0',
+    version='1.0.1',
 
     description='Package to perform Slice Tensor Component Analysis',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     url='https://github.com/arthur-pe/slicetca',
     author='Arthur Pellegrino',
```

### Comparing `slicetca-1.0.0/slicetca/core/decompositions.py` & `slicetca-1.0.1/slicetca/core/decompositions.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.0/slicetca/invariance/analytic_invariance.py` & `slicetca-1.0.1/slicetca/invariance/analytic_invariance.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.0/slicetca/invariance/criteria.py` & `slicetca-1.0.1/slicetca/invariance/criteria.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.0/slicetca/invariance/helper.py` & `slicetca-1.0.1/slicetca/invariance/helper.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.0/slicetca/invariance/invariance.py` & `slicetca-1.0.1/slicetca/invariance/invariance.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.0/slicetca/invariance/iterative_invariance.py` & `slicetca-1.0.1/slicetca/invariance/iterative_invariance.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.0/slicetca/invariance/transformations.py` & `slicetca-1.0.1/slicetca/invariance/transformations.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.0/slicetca/plotting/factors.py` & `slicetca-1.0.1/slicetca/plotting/factors.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.0/slicetca/plotting/grid.py` & `slicetca-1.0.1/slicetca/plotting/grid.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.0/slicetca/run/decompose.py` & `slicetca-1.0.1/slicetca/run/decompose.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.0/slicetca/run/grid_search.py` & `slicetca-1.0.1/slicetca/run/grid_search.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.0/slicetca/run/utils.py` & `slicetca-1.0.1/slicetca/run/utils.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.0/slicetca/tests/tests.py` & `slicetca-1.0.1/slicetca/tests/tests.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.0/slicetca.egg-info/PKG-INFO` & `slicetca-1.0.1/slicetca.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slicetca
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package to perform Slice Tensor Component Analysis
 Home-page: https://github.com/arthur-pe/slicetca
 Author: Arthur Pellegrino
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `slicetca-1.0.0/slicetca.egg-info/SOURCES.txt` & `slicetca-1.0.1/slicetca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

