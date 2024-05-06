# Comparing `tmp/slicetca-0.1.9.tar.gz` & `tmp/slicetca-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slicetca-0.1.9.tar", last modified: Mon Jul 17 02:31:32 2023, max compression
+gzip compressed data, was "slicetca-1.0.0.tar", last modified: Mon May  6 11:22:46 2024, max compression
```

## Comparing `slicetca-0.1.9.tar` & `slicetca-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-07-17 02:31:32.277612 slicetca-0.1.9/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1116 2023-03-06 11:26:01.000000 slicetca-0.1.9/LICENSE.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2312 2023-07-17 02:31:32.277612 slicetca-0.1.9/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1792 2023-03-07 11:52:39.000000 slicetca-0.1.9/README.md
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       79 2023-07-17 02:31:32.277612 slicetca-0.1.9/setup.cfg
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      944 2023-07-17 02:31:27.000000 slicetca-0.1.9/setup.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-07-17 02:31:32.277612 slicetca-0.1.9/slicetca/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      214 2023-03-07 11:24:31.000000 slicetca-0.1.9/slicetca/__init__.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-07-17 02:31:32.277612 slicetca-0.1.9/slicetca/core/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       77 2023-01-03 10:29:24.000000 slicetca-0.1.9/slicetca/core/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    12757 2023-07-12 00:19:14.000000 slicetca-0.1.9/slicetca/core/decompositions.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-07-17 02:31:32.277612 slicetca-0.1.9/slicetca/invariance/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       80 2023-03-06 12:10:37.000000 slicetca-0.1.9/slicetca/invariance/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1352 2023-03-02 09:01:48.000000 slicetca-0.1.9/slicetca/invariance/analytic_invariance.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1179 2023-01-03 10:28:16.000000 slicetca-0.1.9/slicetca/invariance/criteria.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1865 2023-03-06 12:14:41.000000 slicetca-0.1.9/slicetca/invariance/helper.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1272 2023-07-13 15:26:21.000000 slicetca-0.1.9/slicetca/invariance/invariance.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2681 2023-03-06 12:14:41.000000 slicetca-0.1.9/slicetca/invariance/iterative_invariance.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     4323 2023-01-03 10:28:16.000000 slicetca-0.1.9/slicetca/invariance/transformations.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-07-17 02:31:32.277612 slicetca-0.1.9/slicetca/plotting/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       45 2023-03-04 21:19:31.000000 slicetca-0.1.9/slicetca/plotting/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2022-12-29 06:45:13.000000 slicetca-0.1.9/slicetca/plotting/additional.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     7034 2023-03-07 11:02:58.000000 slicetca-0.1.9/slicetca/plotting/factors.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-07-17 02:31:32.277612 slicetca-0.1.9/slicetca/run/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      127 2023-03-03 12:58:54.000000 slicetca-0.1.9/slicetca/run/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     3125 2023-07-12 00:13:29.000000 slicetca-0.1.9/slicetca/run/decompose.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     5056 2023-07-12 00:15:06.000000 slicetca-0.1.9/slicetca/run/grid_search.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2657 2023-03-03 14:21:07.000000 slicetca-0.1.9/slicetca/run/utils.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-07-17 02:31:32.277612 slicetca-0.1.9/slicetca/tests/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-03-02 08:55:06.000000 slicetca-0.1.9/slicetca/tests/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     3966 2023-03-06 12:14:41.000000 slicetca-0.1.9/slicetca/tests/tests.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-07-17 02:31:32.277612 slicetca-0.1.9/slicetca.egg-info/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2312 2023-07-17 02:31:32.000000 slicetca-0.1.9/slicetca.egg-info/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      775 2023-07-17 02:31:32.000000 slicetca-0.1.9/slicetca.egg-info/SOURCES.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-07-17 02:31:32.000000 slicetca-0.1.9/slicetca.egg-info/dependency_links.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       28 2023-07-17 02:31:32.000000 slicetca-0.1.9/slicetca.egg-info/requires.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        9 2023-07-17 02:31:32.000000 slicetca-0.1.9/slicetca.egg-info/top_level.txt
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:22:46.253472 slicetca-1.0.0/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1116 2023-03-06 11:26:01.000000 slicetca-1.0.0/LICENSE.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2330 2024-05-06 11:22:46.253472 slicetca-1.0.0/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1810 2024-05-06 08:16:50.000000 slicetca-1.0.0/README.md
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       79 2024-05-06 11:22:46.253472 slicetca-1.0.0/setup.cfg
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      975 2024-05-06 11:22:44.000000 slicetca-1.0.0/setup.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:22:46.249472 slicetca-1.0.0/slicetca/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      214 2023-03-07 11:24:31.000000 slicetca-1.0.0/slicetca/__init__.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:22:46.253472 slicetca-1.0.0/slicetca/core/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       77 2023-01-03 10:29:24.000000 slicetca-1.0.0/slicetca/core/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    13265 2023-08-21 21:40:43.000000 slicetca-1.0.0/slicetca/core/decompositions.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      322 2023-08-21 21:40:43.000000 slicetca-1.0.0/slicetca/core/helper_functions.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:22:46.253472 slicetca-1.0.0/slicetca/invariance/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       80 2023-03-06 12:10:37.000000 slicetca-1.0.0/slicetca/invariance/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1352 2023-03-02 09:01:48.000000 slicetca-1.0.0/slicetca/invariance/analytic_invariance.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1179 2023-01-03 10:28:16.000000 slicetca-1.0.0/slicetca/invariance/criteria.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1865 2023-03-06 12:14:41.000000 slicetca-1.0.0/slicetca/invariance/helper.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1219 2023-08-21 21:46:56.000000 slicetca-1.0.0/slicetca/invariance/invariance.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2681 2023-03-06 12:14:41.000000 slicetca-1.0.0/slicetca/invariance/iterative_invariance.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     4323 2023-01-03 10:28:16.000000 slicetca-1.0.0/slicetca/invariance/transformations.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:22:46.253472 slicetca-1.0.0/slicetca/plotting/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       86 2024-05-06 09:28:28.000000 slicetca-1.0.0/slicetca/plotting/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2022-12-29 06:45:13.000000 slicetca-1.0.0/slicetca/plotting/additional.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     7034 2023-03-07 11:02:58.000000 slicetca-1.0.0/slicetca/plotting/factors.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3765 2024-05-06 11:18:23.000000 slicetca-1.0.0/slicetca/plotting/grid.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:22:46.253472 slicetca-1.0.0/slicetca/run/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      127 2023-03-03 12:58:54.000000 slicetca-1.0.0/slicetca/run/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3484 2023-08-21 21:40:43.000000 slicetca-1.0.0/slicetca/run/decompose.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     5085 2023-08-21 21:29:47.000000 slicetca-1.0.0/slicetca/run/grid_search.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2657 2023-03-03 14:21:07.000000 slicetca-1.0.0/slicetca/run/utils.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:22:46.253472 slicetca-1.0.0/slicetca/tests/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-03-02 08:55:06.000000 slicetca-1.0.0/slicetca/tests/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3966 2023-03-06 12:14:41.000000 slicetca-1.0.0/slicetca/tests/tests.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2024-05-06 11:22:46.253472 slicetca-1.0.0/slicetca.egg-info/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2330 2024-05-06 11:22:46.000000 slicetca-1.0.0/slicetca.egg-info/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      835 2024-05-06 11:22:46.000000 slicetca-1.0.0/slicetca.egg-info/SOURCES.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2024-05-06 11:22:46.000000 slicetca-1.0.0/slicetca.egg-info/dependency_links.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       34 2024-05-06 11:22:46.000000 slicetca-1.0.0/slicetca.egg-info/requires.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        9 2024-05-06 11:22:46.000000 slicetca-1.0.0/slicetca.egg-info/top_level.txt
```

### Comparing `slicetca-0.1.9/LICENSE.txt` & `slicetca-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.9/PKG-INFO` & `slicetca-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slicetca
-Version: 0.1.9
+Version: 1.0.0
 Summary: Package to perform Slice Tensor Component Analysis
 Home-page: https://github.com/arthur-pe/slicetca
 Author: Arthur Pellegrino
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -65,9 +65,9 @@
 
 <a target="_blank" href="https://colab.research.google.com/github/arthur-pe/slicetca/blob/master/sliceTCA_notebook_1.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 ## Reference
 
-A. Pellegrino<sub>@</sub><sup>†</sup>, H. Stein<sup>†</sup>, N. A. Cayco-Gaijc<sub>@</sub>. (2023). Disentangling Mixed Classes of Covariability in Large-Scale Neural Data. [https://www.biorxiv.org/content/10.1101/2023.03.01.530616v1](https://www.biorxiv.org/content/10.1101/2023.03.01.530616v1).
+A. Pellegrino<sub>@</sub><sup>†</sup>, H. Stein<sup>†</sup>, N. A. Cayco-Gaijc<sub>@</sub>. (2024). Dimensionality reduction beyond neural subspaces with slice tensor component analysis. *Nature Neuroscience* [https://www.nature.com/articles/s41593-024-01626-2](https://www.nature.com/articles/s41593-024-01626-2).
```

### Comparing `slicetca-0.1.9/README.md` & `slicetca-1.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -49,8 +49,8 @@
 
 <a target="_blank" href="https://colab.research.google.com/github/arthur-pe/slicetca/blob/master/sliceTCA_notebook_1.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 ## Reference
 
-A. Pellegrino<sub>@</sub><sup>†</sup>, H. Stein<sup>†</sup>, N. A. Cayco-Gaijc<sub>@</sub>. (2023). Disentangling Mixed Classes of Covariability in Large-Scale Neural Data. [https://www.biorxiv.org/content/10.1101/2023.03.01.530616v1](https://www.biorxiv.org/content/10.1101/2023.03.01.530616v1).
+A. Pellegrino<sub>@</sub><sup>†</sup>, H. Stein<sup>†</sup>, N. A. Cayco-Gaijc<sub>@</sub>. (2024). Dimensionality reduction beyond neural subspaces with slice tensor component analysis. *Nature Neuroscience* [https://www.nature.com/articles/s41593-024-01626-2](https://www.nature.com/articles/s41593-024-01626-2).
```

### Comparing `slicetca-0.1.9/setup.py` & `slicetca-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='slicetca',
     packages=find_packages(exclude=['tests*']),
-    version='0.1.9',
+    version='1.0.0',
 
     description='Package to perform Slice Tensor Component Analysis',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     url='https://github.com/arthur-pe/slicetca',
     author='Arthur Pellegrino',
     license='MIT',
     install_requires=['torch',
                       'numpy',
                       'matplotlib',
-                      'tqdm'
+                      'tqdm',
+                      'scipy'
                       ],
     python_requires='>=3.8',
     classifiers=[
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Mathematics',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
```

### Comparing `slicetca-0.1.9/slicetca/core/decompositions.py` & `slicetca-1.0.0/slicetca/core/decompositions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from .helper_functions import squared_difference
+
 import torch
 from torch import nn
 import numpy as np
 import tqdm
 from collections.abc import Iterable
 
 from typing import Sequence, Union, Callable
@@ -192,29 +194,31 @@
                 with torch.no_grad():
                     if isinstance(components[i][j], torch.Tensor):
                         self.vectors[i][j].copy_(components[i][j].to(self.device))
                     else:
                         self.vectors[i][j].copy_(torch.tensor(components[i][j], device=self.device))
         self.zero_grad()
 
-    def fit(self, 
-            X: torch.Tensor, 
-            optimizer: torch.optim.Optimizer, 
-            batch_prop: float = 0.2, 
-            max_iter: int = 10000, 
-            min_std: float = 10**-3, 
-            iter_std: int = 100, 
-            mask: torch.Tensor = None, 
+    def fit(self,
+            X: torch.Tensor,
+            optimizer: torch.optim.Optimizer,
+            loss_function: Callable = squared_difference,
+            batch_prop: float = 0.2,
+            max_iter: int = 10000,
+            min_std: float = 10 ** -3,
+            iter_std: int = 100,
+            mask: torch.Tensor = None,
             verbose: bool = False,
             progress_bar: bool = True):
         """
         Fits the model to data.
-        
+
         :param X: The data tensor.
         :param optimizer: A torch optimizer.
+        :param loss_function: The final loss if torch.mean(loss_function(X, X_hat)). That is, loss_function: R^n -> R^n.
         :param batch_prop: Proportion of entries used to compute the gradient at every training iteration.
         :param max_iter: Maximum training iterations.
         :param min_std: Minimum std of the loss under which to return.
         :param iter_std: Number of iterations over which this std is computed.
         :param mask: Entries which are not used to compute the gradient at any training iteration.
         :param verbose: Whether to print the loss at every step.
         :param progress_bar: Whether to have a tqdm progress bar.
@@ -224,37 +228,47 @@
 
         iterator = tqdm.tqdm(range(max_iter)) if progress_bar else range(max_iter)
 
         for iteration in iterator:
 
             X_hat = self.construct()
 
-            dX = X-X_hat
+            loss_entries = loss_function(X, X_hat)
 
-            if mask is not None: dX = dX * mask
+            total_loss = torch.mean(loss_entries)
 
-            with torch.no_grad(): total_loss = torch.mean(torch.square(dX)).item() #should be divided by prop masked entries
+            if batch_prop != 1.0: batch_mask = torch.rand(self.dimensions, device=self.device) < batch_prop
 
-            if batch_prop != 1.0:
-                dX = dX*(torch.rand(self.dimensions, device=self.device)<batch_prop)
-                loss = torch.mean(torch.square(dX))/batch_prop
+            if mask is None and batch_prop == 1.0:
+                loss = total_loss
             else:
-                loss = torch.mean(torch.square(dX))
+                if mask is None:
+                    total_mask = batch_mask
+                else:
+                    if batch_prop == 1.0:
+                        total_mask = mask
+                    else:
+                        total_mask = mask & batch_mask
+
+                total_entries = torch.sum(total_mask)
+                loss = torch.sum(loss_entries * total_mask) / total_entries
 
             optimizer.zero_grad()
             loss.backward()
             optimizer.step()
 
+            total_loss = total_loss.item()
+
             losses.append(total_loss)
 
-            if verbose: print('Iteration:', iteration, 'MSE loss:', total_loss)
-            if progress_bar: iterator.set_description('MSE loss: ' + str(total_loss) + ' ')
+            if verbose: print('Iteration:', iteration, 'Loss:', total_loss)
+            if progress_bar: iterator.set_description('Loss: ' + str(total_loss) + ' ')
 
-            if len(losses)>iter_std and np.array(losses[-iter_std:]).std()<min_std:
-                if progress_bar: iterator.set_description('The model converged. MSE loss: ' + str(total_loss) + ' ')
+            if len(losses) > iter_std and np.array(losses[-iter_std:]).std() < min_std:
+                if progress_bar: iterator.set_description('The model converged. Loss: ' + str(total_loss) + ' ')
                 break
 
         self.losses += losses
 
 
 class SliceTCA(PartitionTCA):
     def __init__(self,
```

### Comparing `slicetca-0.1.9/slicetca/invariance/analytic_invariance.py` & `slicetca-1.0.0/slicetca/invariance/analytic_invariance.py`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.9/slicetca/invariance/criteria.py` & `slicetca-1.0.0/slicetca/invariance/criteria.py`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.9/slicetca/invariance/helper.py` & `slicetca-1.0.0/slicetca/invariance/helper.py`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.9/slicetca/invariance/invariance.py` & `slicetca-1.0.0/slicetca/invariance/invariance.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,13 +17,12 @@
     :param model: A sliceTCA model.
     :param L2: String, currently only supports 'regularization', you may add additional objectives.
     :param L3: String, currently only supports 'svd'.
     :param kwargs: Key-word arguments to be passed to L2 and L3 optimization functions. See iterative_function.py
     :return: model with modified components.
     """
 
-    # Add check for model with single component type
     if sum([r!=0 for r in model.ranks])>1:
         model = sgd_invariance(model, objective_function=dict_L2_invariance_objectives[L2], **kwargs)
     model = dict_L3_invariance_functions[L3](model, **kwargs)
 
     return model
```

### Comparing `slicetca-0.1.9/slicetca/invariance/iterative_invariance.py` & `slicetca-1.0.0/slicetca/invariance/iterative_invariance.py`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.9/slicetca/invariance/transformations.py` & `slicetca-1.0.0/slicetca/invariance/transformations.py`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.9/slicetca/plotting/factors.py` & `slicetca-1.0.0/slicetca/plotting/factors.py`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.9/slicetca/run/grid_search.py` & `slicetca-1.0.0/slicetca/run/grid_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 
 from typing import Sequence, Union
 
 
 # To be fixed: high memory usage when using GPU.
 
-def grid_search(data: Union[torch.Tensor, np.array], #Only works with torch.Tensor atm
+def grid_search(data: Union[torch.Tensor], # Only works with torch.Tensor atm
                 max_ranks: Sequence[int],
                 mask_train: torch.Tensor = None,
                 mask_test: torch.Tensor = None,
                 min_ranks: Sequence[int] = None,
                 sample_size: int = 1,
                 processes_sample: int = 1,
                 processes_grid: int = 1,
@@ -116,12 +116,13 @@
     else: loss = torch.mean(((data-data_hat)[mask_test])**2).item()
 
     return loss
 
 
 def get_grid_sample(min_dims, max_dims):
 
-    grid = np.meshgrid(*[np.array([i for i in range(min_dims[j],max_dims[j])]) for j in range(len(max_dims))])
+    grid = np.meshgrid(*[np.array([i for i in range(min_dims[j],max_dims[j])]) for j in range(len(max_dims))],
+                       indexing='ij')
 
     grid = np.stack(grid)
 
     return grid.reshape(grid.shape[0], -1).T
```

### Comparing `slicetca-0.1.9/slicetca/run/utils.py` & `slicetca-1.0.0/slicetca/run/utils.py`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.9/slicetca/tests/tests.py` & `slicetca-1.0.0/slicetca/tests/tests.py`

 * *Files identical despite different names*

### Comparing `slicetca-0.1.9/slicetca.egg-info/PKG-INFO` & `slicetca-1.0.0/slicetca.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slicetca
-Version: 0.1.9
+Version: 1.0.0
 Summary: Package to perform Slice Tensor Component Analysis
 Home-page: https://github.com/arthur-pe/slicetca
 Author: Arthur Pellegrino
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -65,9 +65,9 @@
 
 <a target="_blank" href="https://colab.research.google.com/github/arthur-pe/slicetca/blob/master/sliceTCA_notebook_1.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 ## Reference
 
-A. Pellegrino<sub>@</sub><sup>†</sup>, H. Stein<sup>†</sup>, N. A. Cayco-Gaijc<sub>@</sub>. (2023). Disentangling Mixed Classes of Covariability in Large-Scale Neural Data. [https://www.biorxiv.org/content/10.1101/2023.03.01.530616v1](https://www.biorxiv.org/content/10.1101/2023.03.01.530616v1).
+A. Pellegrino<sub>@</sub><sup>†</sup>, H. Stein<sup>†</sup>, N. A. Cayco-Gaijc<sub>@</sub>. (2024). Dimensionality reduction beyond neural subspaces with slice tensor component analysis. *Nature Neuroscience* [https://www.nature.com/articles/s41593-024-01626-2](https://www.nature.com/articles/s41593-024-01626-2).
```

### Comparing `slicetca-0.1.9/slicetca.egg-info/SOURCES.txt` & `slicetca-1.0.0/slicetca.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 slicetca.egg-info/PKG-INFO
 slicetca.egg-info/SOURCES.txt
 slicetca.egg-info/dependency_links.txt
 slicetca.egg-info/requires.txt
 slicetca.egg-info/top_level.txt
 slicetca/core/__init__.py
 slicetca/core/decompositions.py
+slicetca/core/helper_functions.py
 slicetca/invariance/__init__.py
 slicetca/invariance/analytic_invariance.py
 slicetca/invariance/criteria.py
 slicetca/invariance/helper.py
 slicetca/invariance/invariance.py
 slicetca/invariance/iterative_invariance.py
 slicetca/invariance/transformations.py
 slicetca/plotting/__init__.py
 slicetca/plotting/additional.py
 slicetca/plotting/factors.py
+slicetca/plotting/grid.py
 slicetca/run/__init__.py
 slicetca/run/decompose.py
 slicetca/run/grid_search.py
 slicetca/run/utils.py
 slicetca/tests/__init__.py
 slicetca/tests/tests.py
```

