# Comparing `tmp/slicetca-1.0.1.tar.gz` & `tmp/slicetca-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slicetca-1.0.1.tar", last modified: Mon May  6 11:38:27 2024, max compression
+gzip compressed data, was "slicetca-1.0.2.tar", last modified: Mon May  6 11:42:10 2024, max compression
```

## Comparing `slicetca-1.0.1.tar` & `slicetca-1.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:38:27.306663 slicetca-1.0.1/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1116 2023-03-06 11:26:01.000000 slicetca-1.0.1/LICENSE.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2330 2024-05-06 11:38:27.306663 slicetca-1.0.1/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1810 2024-05-06 08:16:50.000000 slicetca-1.0.1/README.md
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       79 2024-05-06 11:38:27.306663 slicetca-1.0.1/setup.cfg
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      975 2024-05-06 11:38:26.000000 slicetca-1.0.1/setup.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:38:27.306663 slicetca-1.0.1/slicetca/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      227 2024-05-06 11:37:45.000000 slicetca-1.0.1/slicetca/__init__.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:38:27.306663 slicetca-1.0.1/slicetca/core/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       77 2023-01-03 10:29:24.000000 slicetca-1.0.1/slicetca/core/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    13265 2023-08-21 21:40:43.000000 slicetca-1.0.1/slicetca/core/decompositions.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      322 2023-08-21 21:40:43.000000 slicetca-1.0.1/slicetca/core/helper_functions.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:38:27.306663 slicetca-1.0.1/slicetca/invariance/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       80 2023-03-06 12:10:37.000000 slicetca-1.0.1/slicetca/invariance/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1352 2023-03-02 09:01:48.000000 slicetca-1.0.1/slicetca/invariance/analytic_invariance.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1179 2023-01-03 10:28:16.000000 slicetca-1.0.1/slicetca/invariance/criteria.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1865 2023-03-06 12:14:41.000000 slicetca-1.0.1/slicetca/invariance/helper.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1219 2023-08-21 21:46:56.000000 slicetca-1.0.1/slicetca/invariance/invariance.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2681 2023-03-06 12:14:41.000000 slicetca-1.0.1/slicetca/invariance/iterative_invariance.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     4323 2023-01-03 10:28:16.000000 slicetca-1.0.1/slicetca/invariance/transformations.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:38:27.306663 slicetca-1.0.1/slicetca/plotting/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       86 2024-05-06 09:28:28.000000 slicetca-1.0.1/slicetca/plotting/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2022-12-29 06:45:13.000000 slicetca-1.0.1/slicetca/plotting/additional.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     7034 2023-03-07 11:02:58.000000 slicetca-1.0.1/slicetca/plotting/factors.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     3765 2024-05-06 11:18:23.000000 slicetca-1.0.1/slicetca/plotting/grid.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:38:27.306663 slicetca-1.0.1/slicetca/run/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      127 2023-03-03 12:58:54.000000 slicetca-1.0.1/slicetca/run/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     3484 2023-08-21 21:40:43.000000 slicetca-1.0.1/slicetca/run/decompose.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     5085 2023-08-21 21:29:47.000000 slicetca-1.0.1/slicetca/run/grid_search.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2657 2023-03-03 14:21:07.000000 slicetca-1.0.1/slicetca/run/utils.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:38:27.306663 slicetca-1.0.1/slicetca/tests/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-03-02 08:55:06.000000 slicetca-1.0.1/slicetca/tests/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     3966 2023-03-06 12:14:41.000000 slicetca-1.0.1/slicetca/tests/tests.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:38:27.306663 slicetca-1.0.1/slicetca.egg-info/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2330 2024-05-06 11:38:27.000000 slicetca-1.0.1/slicetca.egg-info/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      835 2024-05-06 11:38:27.000000 slicetca-1.0.1/slicetca.egg-info/SOURCES.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2024-05-06 11:38:27.000000 slicetca-1.0.1/slicetca.egg-info/dependency_links.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       34 2024-05-06 11:38:27.000000 slicetca-1.0.1/slicetca.egg-info/requires.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        9 2024-05-06 11:38:27.000000 slicetca-1.0.1/slicetca.egg-info/top_level.txt
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:42:10.624626 slicetca-1.0.2/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1116 2023-03-06 11:26:01.000000 slicetca-1.0.2/LICENSE.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2330 2024-05-06 11:42:10.624626 slicetca-1.0.2/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1810 2024-05-06 08:16:50.000000 slicetca-1.0.2/README.md
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       79 2024-05-06 11:42:10.624626 slicetca-1.0.2/setup.cfg
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      975 2024-05-06 11:42:06.000000 slicetca-1.0.2/setup.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:42:10.624626 slicetca-1.0.2/slicetca/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      227 2024-05-06 11:37:45.000000 slicetca-1.0.2/slicetca/__init__.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:42:10.624626 slicetca-1.0.2/slicetca/core/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       77 2023-01-03 10:29:24.000000 slicetca-1.0.2/slicetca/core/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    13265 2023-08-21 21:40:43.000000 slicetca-1.0.2/slicetca/core/decompositions.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      322 2023-08-21 21:40:43.000000 slicetca-1.0.2/slicetca/core/helper_functions.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:42:10.624626 slicetca-1.0.2/slicetca/invariance/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       80 2023-03-06 12:10:37.000000 slicetca-1.0.2/slicetca/invariance/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1352 2023-03-02 09:01:48.000000 slicetca-1.0.2/slicetca/invariance/analytic_invariance.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1179 2023-01-03 10:28:16.000000 slicetca-1.0.2/slicetca/invariance/criteria.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1865 2023-03-06 12:14:41.000000 slicetca-1.0.2/slicetca/invariance/helper.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1219 2023-08-21 21:46:56.000000 slicetca-1.0.2/slicetca/invariance/invariance.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2681 2023-03-06 12:14:41.000000 slicetca-1.0.2/slicetca/invariance/iterative_invariance.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     4323 2023-01-03 10:28:16.000000 slicetca-1.0.2/slicetca/invariance/transformations.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:42:10.624626 slicetca-1.0.2/slicetca/plotting/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       86 2024-05-06 09:28:28.000000 slicetca-1.0.2/slicetca/plotting/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2022-12-29 06:45:13.000000 slicetca-1.0.2/slicetca/plotting/additional.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     7034 2023-03-07 11:02:58.000000 slicetca-1.0.2/slicetca/plotting/factors.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3943 2024-05-06 11:41:56.000000 slicetca-1.0.2/slicetca/plotting/grid.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:42:10.624626 slicetca-1.0.2/slicetca/run/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      127 2023-03-03 12:58:54.000000 slicetca-1.0.2/slicetca/run/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3484 2023-08-21 21:40:43.000000 slicetca-1.0.2/slicetca/run/decompose.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     5085 2023-08-21 21:29:47.000000 slicetca-1.0.2/slicetca/run/grid_search.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2657 2023-03-03 14:21:07.000000 slicetca-1.0.2/slicetca/run/utils.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:42:10.624626 slicetca-1.0.2/slicetca/tests/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-03-02 08:55:06.000000 slicetca-1.0.2/slicetca/tests/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3966 2023-03-06 12:14:41.000000 slicetca-1.0.2/slicetca/tests/tests.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:42:10.624626 slicetca-1.0.2/slicetca.egg-info/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2330 2024-05-06 11:42:10.000000 slicetca-1.0.2/slicetca.egg-info/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      835 2024-05-06 11:42:10.000000 slicetca-1.0.2/slicetca.egg-info/SOURCES.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2024-05-06 11:42:10.000000 slicetca-1.0.2/slicetca.egg-info/dependency_links.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       34 2024-05-06 11:42:10.000000 slicetca-1.0.2/slicetca.egg-info/requires.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        9 2024-05-06 11:42:10.000000 slicetca-1.0.2/slicetca.egg-info/top_level.txt
```

### Comparing `slicetca-1.0.1/LICENSE.txt` & `slicetca-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.1/PKG-INFO` & `slicetca-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slicetca
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package to perform Slice Tensor Component Analysis
 Home-page: https://github.com/arthur-pe/slicetca
 Author: Arthur Pellegrino
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `slicetca-1.0.1/README.md` & `slicetca-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.1/slicetca/core/decompositions.py` & `slicetca-1.0.2/slicetca/core/decompositions.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.1/slicetca/invariance/analytic_invariance.py` & `slicetca-1.0.2/slicetca/invariance/analytic_invariance.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.1/slicetca/invariance/criteria.py` & `slicetca-1.0.2/slicetca/invariance/criteria.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.1/slicetca/invariance/helper.py` & `slicetca-1.0.2/slicetca/invariance/helper.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.1/slicetca/invariance/invariance.py` & `slicetca-1.0.2/slicetca/invariance/invariance.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.1/slicetca/invariance/iterative_invariance.py` & `slicetca-1.0.2/slicetca/invariance/iterative_invariance.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.1/slicetca/invariance/transformations.py` & `slicetca-1.0.2/slicetca/invariance/transformations.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.1/slicetca/plotting/factors.py` & `slicetca-1.0.2/slicetca/plotting/factors.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.1/slicetca/plotting/grid.py` & `slicetca-1.0.2/slicetca/plotting/grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 
 from typing import Literal, Sequence
 
 
 def plot_grid(loss_grid: np.ndarray,
               min_rank: Sequence = (0, 0, 0),
               data: np.ndarray = None,
+              elbow: float = 0.9,
               quantile: float = 0.0,
               vmin: float = None,
               vmax: float = None,
               reduction: Literal['mean', 'min'] = 'min',
               variables: Sequence[str] = ('trial', 'neuron', 'time'),
             ):
     """
-    :param min_rank: minimum ranks of the gridsearch (default (0, 0, 0))
     :param loss_grid: (trial x neuron x time x batch) grid of cross-validated losses as a function of the number of components
+    :param min_rank: minimum ranks of the gridsearch (default (0, 0, 0))
+    :param data: to construct elbow
+    :param elbow: fraction of best model performance relative to data squared norm to use for elbow
     :param quantile:
     :param vmin:
     :param vmax:
     :param reduction:
     :param variables:
     :return:
     """
@@ -35,15 +38,15 @@
             reduced_loss_grid = loss_grid.min(axis=-1)
         case _:
             raise Exception('Reduction should be mean or min.')
 
     min_index = np.unravel_index(np.argmin(reduced_loss_grid), reduced_loss_grid.shape)
 
     if data is not None:
-        elbow_threshold = np.min(reduced_loss_grid)*0.9+np.mean(data**2)*0.1
+        elbow_threshold = np.min(reduced_loss_grid)*elbow+np.mean(data**2)*(1-elbow)
 
     nb_plot = reduced_loss_grid.shape[0]
     if vmin is None: vmin = np.quantile(reduced_loss_grid, quantile)
     if vmax is None: vmax = np.quantile(reduced_loss_grid, 1-quantile)
     print('vmin:', vmin, 'vmax:', vmax)
 
     fig = plt.figure(figsize=(3*nb_plot,3), constrained_layout=True)
```

### Comparing `slicetca-1.0.1/slicetca/run/decompose.py` & `slicetca-1.0.2/slicetca/run/decompose.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.1/slicetca/run/grid_search.py` & `slicetca-1.0.2/slicetca/run/grid_search.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.1/slicetca/run/utils.py` & `slicetca-1.0.2/slicetca/run/utils.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.1/slicetca/tests/tests.py` & `slicetca-1.0.2/slicetca/tests/tests.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.1/slicetca.egg-info/PKG-INFO` & `slicetca-1.0.2/slicetca.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slicetca
-Version: 1.0.1
+Version: 1.0.2
 Summary: Package to perform Slice Tensor Component Analysis
 Home-page: https://github.com/arthur-pe/slicetca
 Author: Arthur Pellegrino
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `slicetca-1.0.1/slicetca.egg-info/SOURCES.txt` & `slicetca-1.0.2/slicetca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

