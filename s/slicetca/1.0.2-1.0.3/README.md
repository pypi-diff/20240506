# Comparing `tmp/slicetca-1.0.2.tar.gz` & `tmp/slicetca-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slicetca-1.0.2.tar", last modified: Mon May  6 11:42:10 2024, max compression
+gzip compressed data, was "slicetca-1.0.3.tar", last modified: Mon May  6 12:14:06 2024, max compression
```

## Comparing `slicetca-1.0.2.tar` & `slicetca-1.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:42:10.624626 slicetca-1.0.2/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1116 2023-03-06 11:26:01.000000 slicetca-1.0.2/LICENSE.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2330 2024-05-06 11:42:10.624626 slicetca-1.0.2/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1810 2024-05-06 08:16:50.000000 slicetca-1.0.2/README.md
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       79 2024-05-06 11:42:10.624626 slicetca-1.0.2/setup.cfg
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      975 2024-05-06 11:42:06.000000 slicetca-1.0.2/setup.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:42:10.624626 slicetca-1.0.2/slicetca/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      227 2024-05-06 11:37:45.000000 slicetca-1.0.2/slicetca/__init__.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:42:10.624626 slicetca-1.0.2/slicetca/core/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       77 2023-01-03 10:29:24.000000 slicetca-1.0.2/slicetca/core/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    13265 2023-08-21 21:40:43.000000 slicetca-1.0.2/slicetca/core/decompositions.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      322 2023-08-21 21:40:43.000000 slicetca-1.0.2/slicetca/core/helper_functions.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:42:10.624626 slicetca-1.0.2/slicetca/invariance/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       80 2023-03-06 12:10:37.000000 slicetca-1.0.2/slicetca/invariance/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1352 2023-03-02 09:01:48.000000 slicetca-1.0.2/slicetca/invariance/analytic_invariance.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1179 2023-01-03 10:28:16.000000 slicetca-1.0.2/slicetca/invariance/criteria.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1865 2023-03-06 12:14:41.000000 slicetca-1.0.2/slicetca/invariance/helper.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1219 2023-08-21 21:46:56.000000 slicetca-1.0.2/slicetca/invariance/invariance.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2681 2023-03-06 12:14:41.000000 slicetca-1.0.2/slicetca/invariance/iterative_invariance.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     4323 2023-01-03 10:28:16.000000 slicetca-1.0.2/slicetca/invariance/transformations.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:42:10.624626 slicetca-1.0.2/slicetca/plotting/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       86 2024-05-06 09:28:28.000000 slicetca-1.0.2/slicetca/plotting/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2022-12-29 06:45:13.000000 slicetca-1.0.2/slicetca/plotting/additional.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     7034 2023-03-07 11:02:58.000000 slicetca-1.0.2/slicetca/plotting/factors.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     3943 2024-05-06 11:41:56.000000 slicetca-1.0.2/slicetca/plotting/grid.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:42:10.624626 slicetca-1.0.2/slicetca/run/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      127 2023-03-03 12:58:54.000000 slicetca-1.0.2/slicetca/run/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     3484 2023-08-21 21:40:43.000000 slicetca-1.0.2/slicetca/run/decompose.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     5085 2023-08-21 21:29:47.000000 slicetca-1.0.2/slicetca/run/grid_search.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2657 2023-03-03 14:21:07.000000 slicetca-1.0.2/slicetca/run/utils.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:42:10.624626 slicetca-1.0.2/slicetca/tests/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-03-02 08:55:06.000000 slicetca-1.0.2/slicetca/tests/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     3966 2023-03-06 12:14:41.000000 slicetca-1.0.2/slicetca/tests/tests.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:42:10.624626 slicetca-1.0.2/slicetca.egg-info/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2330 2024-05-06 11:42:10.000000 slicetca-1.0.2/slicetca.egg-info/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      835 2024-05-06 11:42:10.000000 slicetca-1.0.2/slicetca.egg-info/SOURCES.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2024-05-06 11:42:10.000000 slicetca-1.0.2/slicetca.egg-info/dependency_links.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       34 2024-05-06 11:42:10.000000 slicetca-1.0.2/slicetca.egg-info/requires.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        9 2024-05-06 11:42:10.000000 slicetca-1.0.2/slicetca.egg-info/top_level.txt
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 12:14:06.566895 slicetca-1.0.3/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1116 2023-03-06 11:26:01.000000 slicetca-1.0.3/LICENSE.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2330 2024-05-06 12:14:06.566895 slicetca-1.0.3/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1810 2024-05-06 08:16:50.000000 slicetca-1.0.3/README.md
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       79 2024-05-06 12:14:06.566895 slicetca-1.0.3/setup.cfg
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      975 2024-05-06 12:13:50.000000 slicetca-1.0.3/setup.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 12:14:06.562894 slicetca-1.0.3/slicetca/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      227 2024-05-06 11:37:45.000000 slicetca-1.0.3/slicetca/__init__.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 12:14:06.562894 slicetca-1.0.3/slicetca/core/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       77 2023-01-03 10:29:24.000000 slicetca-1.0.3/slicetca/core/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    13265 2023-08-21 21:40:43.000000 slicetca-1.0.3/slicetca/core/decompositions.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      322 2023-08-21 21:40:43.000000 slicetca-1.0.3/slicetca/core/helper_functions.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 12:14:06.562894 slicetca-1.0.3/slicetca/invariance/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       80 2023-03-06 12:10:37.000000 slicetca-1.0.3/slicetca/invariance/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1352 2023-03-02 09:01:48.000000 slicetca-1.0.3/slicetca/invariance/analytic_invariance.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1179 2023-01-03 10:28:16.000000 slicetca-1.0.3/slicetca/invariance/criteria.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1865 2023-03-06 12:14:41.000000 slicetca-1.0.3/slicetca/invariance/helper.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1219 2023-08-21 21:46:56.000000 slicetca-1.0.3/slicetca/invariance/invariance.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2681 2023-03-06 12:14:41.000000 slicetca-1.0.3/slicetca/invariance/iterative_invariance.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     4323 2023-01-03 10:28:16.000000 slicetca-1.0.3/slicetca/invariance/transformations.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 12:14:06.566895 slicetca-1.0.3/slicetca/plotting/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       86 2024-05-06 09:28:28.000000 slicetca-1.0.3/slicetca/plotting/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2022-12-29 06:45:13.000000 slicetca-1.0.3/slicetca/plotting/additional.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     7034 2023-03-07 11:02:58.000000 slicetca-1.0.3/slicetca/plotting/factors.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3943 2024-05-06 11:41:56.000000 slicetca-1.0.3/slicetca/plotting/grid.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 12:14:06.566895 slicetca-1.0.3/slicetca/run/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      127 2023-03-03 12:58:54.000000 slicetca-1.0.3/slicetca/run/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3484 2023-08-21 21:40:43.000000 slicetca-1.0.3/slicetca/run/decompose.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     5085 2023-08-21 21:29:47.000000 slicetca-1.0.3/slicetca/run/grid_search.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3048 2024-05-06 12:13:46.000000 slicetca-1.0.3/slicetca/run/utils.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 12:14:06.566895 slicetca-1.0.3/slicetca/tests/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-03-02 08:55:06.000000 slicetca-1.0.3/slicetca/tests/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3966 2023-03-06 12:14:41.000000 slicetca-1.0.3/slicetca/tests/tests.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 12:14:06.562894 slicetca-1.0.3/slicetca.egg-info/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2330 2024-05-06 12:14:06.000000 slicetca-1.0.3/slicetca.egg-info/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      835 2024-05-06 12:14:06.000000 slicetca-1.0.3/slicetca.egg-info/SOURCES.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2024-05-06 12:14:06.000000 slicetca-1.0.3/slicetca.egg-info/dependency_links.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       34 2024-05-06 12:14:06.000000 slicetca-1.0.3/slicetca.egg-info/requires.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        9 2024-05-06 12:14:06.000000 slicetca-1.0.3/slicetca.egg-info/top_level.txt
```

### Comparing `slicetca-1.0.2/LICENSE.txt` & `slicetca-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.2/PKG-INFO` & `slicetca-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slicetca
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package to perform Slice Tensor Component Analysis
 Home-page: https://github.com/arthur-pe/slicetca
 Author: Arthur Pellegrino
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `slicetca-1.0.2/README.md` & `slicetca-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.2/setup.py` & `slicetca-1.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='slicetca',
     packages=find_packages(exclude=['tests*']),
-    version='1.0.2',
+    version='1.0.3',
 
     description='Package to perform Slice Tensor Component Analysis',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     url='https://github.com/arthur-pe/slicetca',
     author='Arthur Pellegrino',
```

### Comparing `slicetca-1.0.2/slicetca/core/decompositions.py` & `slicetca-1.0.3/slicetca/core/decompositions.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.2/slicetca/invariance/analytic_invariance.py` & `slicetca-1.0.3/slicetca/invariance/analytic_invariance.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.2/slicetca/invariance/criteria.py` & `slicetca-1.0.3/slicetca/invariance/criteria.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.2/slicetca/invariance/helper.py` & `slicetca-1.0.3/slicetca/invariance/helper.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.2/slicetca/invariance/invariance.py` & `slicetca-1.0.3/slicetca/invariance/invariance.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.2/slicetca/invariance/iterative_invariance.py` & `slicetca-1.0.3/slicetca/invariance/iterative_invariance.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.2/slicetca/invariance/transformations.py` & `slicetca-1.0.3/slicetca/invariance/transformations.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.2/slicetca/plotting/factors.py` & `slicetca-1.0.3/slicetca/plotting/factors.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.2/slicetca/plotting/grid.py` & `slicetca-1.0.3/slicetca/plotting/grid.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.2/slicetca/run/decompose.py` & `slicetca-1.0.3/slicetca/run/decompose.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.2/slicetca/run/grid_search.py` & `slicetca-1.0.3/slicetca/run/grid_search.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.2/slicetca/run/utils.py` & `slicetca-1.0.3/slicetca/run/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 import torch
 import numpy as np
 from typing import Iterable
+import warnings
 
 
 def block_mask(dimensions: Iterable[int],
-                train_blocks_dimensions: Iterable[int],
-                test_blocks_dimensions: Iterable[int],
-                number_blocks:int,
-                exact:bool = True,
-                device:str = 'cpu'):
+               train_blocks_dimensions: Iterable[int],
+               test_blocks_dimensions: Iterable[int],
+               number_blocks: int = None,
+               fraction_test: float = 0.1,
+               exact:bool = True,
+               device:str = 'cpu'):
     """
     Builds train and test masks.
     The train mask has block of entries masked.
     The test mask has the opposite entries masked, plus the boundaries of the blocks.
 
     :param dimensions: Dimensions of the mask.
-    :param train_blocks_dimensions: Dimensions of the blocks discarded for training will be 2*train_block_dimensions+1
-    :param test_blocks_dimensions: Dimensions of the blocks retained for testing will be 2*test_block_dimensions+1
-    :param number_blocks: The number of blocks.
+    :param train_blocks_dimensions: Dimensions of the blocks discarded for training will be 2*train_blocks_dimensions+1
+    :param test_blocks_dimensions: Dimensions of the blocks retained for testing will be 2*test_blocks_dimensions+1
+    :param number_blocks: The number of blocks. Deprecated, use fraction_test.
+    :param fraction_test: The maximum fraction of entries in the test_mask
     :param exact:   If exact then the number of blocks will be number_blocks (slower).
                     If not exact, the number of blocks will be on average number_blocks (faster).
     :param device: torch device (e.g. 'cuda' or 'cpu').
     :return: train_mask, test_mask
     """
 
     valence = len(dimensions)
 
     flattened_max_dim = np.prod(dimensions)
 
     if not np.prod((np.array(train_blocks_dimensions)-np.array(test_blocks_dimensions))>=0):
         raise Exception('For all i it should be that train_blocks_dimensions[i]>=test_blocks_dimensions[i].')
 
+    if number_blocks is None:
+        number_blocks = int(fraction_test * flattened_max_dim / np.prod(2*np.array(test_blocks_dimensions)+1))
+    else:
+        warnings.warn('The parameter number_blocks is deprecated, use fraction_test instead.', DeprecationWarning)
+
     if exact:
         start = torch.zeros(flattened_max_dim, device=device)
         start[:number_blocks] = 1
         start = start[torch.randperm(flattened_max_dim, device=device)]
         start = start.reshape(dimensions)
     else:
-        density = number_blocks / flattened_max_dim
-        start = (torch.rand(tuple(dimensions), device=device) < density).long()
+        start = (torch.rand(tuple(dimensions), device=device) < fraction_test).long()
 
     start_index = start.nonzero()
     number_blocks = len(start_index)
 
     # Build outer-blocks mask
     a = [[slice(torch.clip(start_index[j][i]-train_blocks_dimensions[i],min=0, max=dimensions[i]),
                 torch.clip(start_index[j][i]+train_blocks_dimensions[i]+1,min=0, max=dimensions[i]))
```

### Comparing `slicetca-1.0.2/slicetca/tests/tests.py` & `slicetca-1.0.3/slicetca/tests/tests.py`

 * *Files identical despite different names*

### Comparing `slicetca-1.0.2/slicetca.egg-info/PKG-INFO` & `slicetca-1.0.3/slicetca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slicetca
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package to perform Slice Tensor Component Analysis
 Home-page: https://github.com/arthur-pe/slicetca
 Author: Arthur Pellegrino
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `slicetca-1.0.2/slicetca.egg-info/SOURCES.txt` & `slicetca-1.0.3/slicetca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

