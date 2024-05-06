# Comparing `tmp/as_seg-0.1.5.tar.gz` & `tmp/as_seg-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "as_seg-0.1.5.tar", last modified: Thu Apr 25 15:34:36 2024, max compression
+gzip compressed data, was "as_seg-0.1.6.tar", last modified: Mon May  6 15:22:27 2024, max compression
```

## Comparing `as_seg-0.1.5.tar` & `as_seg-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:34:36.736010 as_seg-0.1.5/
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)       90 2023-11-15 10:18:55.000000 as_seg-0.1.5/AUTHORS
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     1516 2023-11-15 10:18:55.000000 as_seg-0.1.5/LICENSE.md
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     4182 2024-04-25 15:34:36.736010 as_seg-0.1.5/PKG-INFO
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     3440 2023-12-18 15:34:55.000000 as_seg-0.1.5/README.md
-drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:34:36.736010 as_seg-0.1.5/as_seg/
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)    24645 2023-11-15 10:18:55.000000 as_seg-0.1.5/as_seg/CBM_algorithm.py
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)      289 2023-11-16 18:06:00.000000 as_seg-0.1.5/as_seg/__init__.py
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     9650 2023-11-15 10:18:55.000000 as_seg-0.1.5/as_seg/autosimilarity_computation.py
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     7606 2023-12-20 10:11:43.000000 as_seg-0.1.5/as_seg/barwise_input.py
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)    26568 2023-12-20 14:33:07.000000 as_seg-0.1.5/as_seg/data_manipulation.py
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     6765 2023-11-15 11:49:38.000000 as_seg-0.1.5/as_seg/example.py
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)    15361 2023-11-20 15:28:34.000000 as_seg-0.1.5/as_seg/foote_novelty.py
-drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:34:36.736010 as_seg-0.1.5/as_seg/model/
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)       78 2023-11-15 10:18:55.000000 as_seg-0.1.5/as_seg/model/__init__.py
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     6046 2023-11-15 10:18:55.000000 as_seg-0.1.5/as_seg/model/current_plot.py
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     1773 2023-11-17 10:45:00.000000 as_seg-0.1.5/as_seg/model/display_results.py
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)      568 2023-11-15 10:18:55.000000 as_seg-0.1.5/as_seg/model/errors.py
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)    17519 2023-11-15 11:53:20.000000 as_seg-0.1.5/as_seg/model/features.py
-drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:34:36.736010 as_seg-0.1.5/as_seg/scripts/
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)        0 2023-11-15 10:18:55.000000 as_seg-0.1.5/as_seg/scripts/__init__.py
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     1965 2024-01-10 12:12:43.000000 as_seg-0.1.5/as_seg/scripts/default_path.py
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)    30588 2023-11-16 19:04:30.000000 as_seg-0.1.5/as_seg/scripts/overall_scripts.py
-drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-04-25 15:34:36.736010 as_seg-0.1.5/as_seg.egg-info/
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     4182 2024-04-25 15:34:36.000000 as_seg-0.1.5/as_seg.egg-info/PKG-INFO
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      586 2024-04-25 15:34:36.000000 as_seg-0.1.5/as_seg.egg-info/SOURCES.txt
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        1 2024-04-25 15:34:36.000000 as_seg-0.1.5/as_seg.egg-info/dependency_links.txt
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      147 2024-04-25 15:34:36.000000 as_seg-0.1.5/as_seg.egg-info/requires.txt
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        7 2024-04-25 15:34:36.000000 as_seg-0.1.5/as_seg.egg-info/top_level.txt
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       38 2024-04-25 15:34:36.736010 as_seg-0.1.5/setup.cfg
--rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     1359 2024-04-25 15:31:49.000000 as_seg-0.1.5/setup.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-06 15:22:27.357170 as_seg-0.1.6/
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)       90 2023-11-15 10:18:55.000000 as_seg-0.1.6/AUTHORS
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     1516 2023-11-15 10:18:55.000000 as_seg-0.1.6/LICENSE.md
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     4182 2024-05-06 15:22:27.357170 as_seg-0.1.6/PKG-INFO
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     3440 2023-12-18 15:34:55.000000 as_seg-0.1.6/README.md
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-06 15:22:27.357170 as_seg-0.1.6/as_seg/
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)    24152 2023-07-26 16:37:36.000000 as_seg-0.1.6/as_seg/CBM_algorithm.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)      303 2024-05-06 14:44:50.000000 as_seg-0.1.6/as_seg/__init__.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     9599 2024-02-12 16:21:29.000000 as_seg-0.1.6/as_seg/autosimilarity_computation.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)    10077 2024-05-06 14:38:31.000000 as_seg-0.1.6/as_seg/barwise_input.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)    27033 2024-05-06 15:16:02.000000 as_seg-0.1.6/as_seg/data_manipulation.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     6783 2024-05-06 15:05:35.000000 as_seg-0.1.6/as_seg/example.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)    15361 2023-11-20 15:28:34.000000 as_seg-0.1.6/as_seg/foote_novelty.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-06 15:22:27.357170 as_seg-0.1.6/as_seg/model/
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)       78 2020-08-04 14:47:49.000000 as_seg-0.1.6/as_seg/model/__init__.py
+-rwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)     6046 2024-03-07 15:55:54.000000 as_seg-0.1.6/as_seg/model/current_plot.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    18823 2024-05-06 15:16:45.000000 as_seg-0.1.6/as_seg/model/dataloaders.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     1773 2023-11-17 10:45:00.000000 as_seg-0.1.6/as_seg/model/display_results.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)      568 2022-12-15 14:51:26.000000 as_seg-0.1.6/as_seg/model/errors.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     6777 2024-05-06 14:43:50.000000 as_seg-0.1.6/as_seg/model/signal_to_spectrogram.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-06 15:22:27.357170 as_seg-0.1.6/as_seg/scripts/
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)        0 2023-11-15 10:18:55.000000 as_seg-0.1.6/as_seg/scripts/__init__.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     1965 2024-01-10 12:12:43.000000 as_seg-0.1.6/as_seg/scripts/default_path.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)    30588 2023-11-16 19:04:30.000000 as_seg-0.1.6/as_seg/scripts/overall_scripts.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-06 15:22:27.357170 as_seg-0.1.6/as_seg.egg-info/
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     4182 2024-05-06 15:22:27.000000 as_seg-0.1.6/as_seg.egg-info/PKG-INFO
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      627 2024-05-06 15:22:27.000000 as_seg-0.1.6/as_seg.egg-info/SOURCES.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        1 2024-05-06 15:22:27.000000 as_seg-0.1.6/as_seg.egg-info/dependency_links.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      147 2024-05-06 15:22:27.000000 as_seg-0.1.6/as_seg.egg-info/requires.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        7 2024-05-06 15:22:27.000000 as_seg-0.1.6/as_seg.egg-info/top_level.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       38 2024-05-06 15:22:27.357170 as_seg-0.1.6/setup.cfg
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     1359 2024-05-06 15:18:17.000000 as_seg-0.1.6/setup.py
```

### Comparing `as_seg-0.1.5/LICENSE.md` & `as_seg-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `as_seg-0.1.5/PKG-INFO` & `as_seg-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: as_seg
-Version: 0.1.5
+Version: 0.1.6
 Summary: Package for the segmentation of autosimilarity matrices. This version is related to a stable vesion on PyPi, for installation in MSAF.
 Home-page: https://gitlab.inria.fr/amarmore/autosimilarity_segmentation
 Author: Marmoret Axel
 Author-email: axel.marmoret@imt-atlantique.fr
 License: BSD
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `as_seg-0.1.5/README.md` & `as_seg-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `as_seg-0.1.5/as_seg/CBM_algorithm.py` & `as_seg-0.1.6/as_seg/CBM_algorithm.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,493 +1,493 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Feb 24 11:01:42 2020
-
-@author: amarmore
-
-Convolutive "Block-Matching" (CBM) algorithm.
-This algorithm is designed to segment barwise autosimilarities.
-
-In short, this algorithm focuses on the criteria of homogeneity to estimate segments, 
-and computes an optimal segmentation via dynamic programming.
-
-See [1] for more details.
-
-References
-----------
-[1] Marmoret, A., Cohen, J. E., & Bimbot, F., "Convolutive Block-Matching Segmentation Algorithm with Application to Music Structure Analysis", 2022, arXiv preprint arXiv:2210.15356.
-"""
-
-import as_seg.model.errors as err
-
-import math
-import numpy as np
-from scipy.sparse import diags
-import warnings
-
-def compute_cbm(autosimilarity, min_size = 1, max_size = 32, penalty_weight = 1, penalty_func = "modulo8", bands_number = None):
-    """
-    Dynamic programming algorithm, maximizing an overall score at the song scale, sum of all segments' scores on the autosimilarity.
-    Each segment' score is a combination of
-     - the convolution score on this the segment, dependong on the kernel, 
-     - a penalty cost, function of the size of the segment, to enforce specific sizes (with prior knowledge),
-
-    The penalty cost is computed in the function "penalty_cost_from_arg()".
-    See this function for further details.
-
-    It returns the optimal segmentation according to this score.
-    
-    This algortihm is also described in [1].
-    
-    IDEAS FOR FUTURE DEVELOPMENT: 
-        - May be optimized using scipy.signal.fftconvolve(), but requires a different approach in parsing all segments.
-    (i.e. parsing all possible segments for a specified kernel size and then retrieve the indexes of the diagonally-centered values)
-        - Taking into account values which are not around the diagonal but everywhere in the matrix in order to account for the repetition principle.
-
-    Parameters
-    ----------
-    autosimilarity : list of list of float (list of columns)
-        The autosimilarity to segment.
-    min_size : integer, optional
-        The minimal length of segments.
-        The default is 1.
-    max_size : integer, optional
-        The maximal length of segments.
-        The default is 32.
-    penalty_weight : float, optional
-        The ponderation parameter for the penalty function
-    penalty_func : string
-        The type of penalty function to use.
-        See "penalty_cost_from_arg()" for further details.
-    bands_number : positive integer or None, optional
-        The number of bands in the kernel. 
-        For the full kernel, bands_number must be set to None
-        (or higher than the maximal size, but cumbersome)
-        See [1] for details. 
-        The default is None.
-
-    Raises
-    ------
-    ToDebugException
-        If the program fails, generally meaning that the autosimilarity is incorrect.
-
-    Returns
-    -------
-    list of tuples
-        The segments, as a list of tuples (start, end).
-    integer
-        Global cost (the maximum among all).
-    """
-    scores = [-math.inf for i in range(len(autosimilarity))]
-    segments_best_starts = [None for i in range(len(autosimilarity))]
-    segments_best_starts[0] = 0
-    scores[0] = 0
-    kernels = compute_all_kernels(max_size, bands_number = bands_number)
-    max_conv_eight = np.amax(convolution_entire_matrix_computation(autosimilarity, kernels))
-    
-    for current_idx in range(1, len(autosimilarity)): # Parse all indexes of the autosimilarity
-        for possible_start_idx in possible_segment_start(current_idx, min_size = min_size, max_size = max_size):
-            if possible_start_idx < 0:
-                raise err.ToDebugException("Invalid value of start index, shouldn't happen.") from None
-                
-            # Convolutionnal cost between the possible start of the segment and the current index (entire segment)
-            conv_cost = convolutionnal_cost(autosimilarity[possible_start_idx:current_idx,possible_start_idx:current_idx], kernels)
-                        
-            segment_length = current_idx - possible_start_idx
-            penalty_cost = penalty_cost_from_arg(penalty_func, segment_length)            
-            
-            this_segment_cost = conv_cost * segment_length - penalty_cost * penalty_weight * max_conv_eight
-            # Note: conv_eight is not normalized by its size (not a problem in itself as size is contant, but generally not specified in formulas).
-
-            if possible_start_idx == 0: # Avoiding errors, as scores values are initially set to -inf.
-                if this_segment_cost > scores[current_idx]: # This segment is of larger score
-                    scores[current_idx] = this_segment_cost
-                    segments_best_starts[current_idx] = 0
-            else:
-                if scores[possible_start_idx] + this_segment_cost > scores[current_idx]: # This segment is of larger score
-                    scores[current_idx] = scores[possible_start_idx] + this_segment_cost
-                    segments_best_starts[current_idx] = possible_start_idx
-
-    segments = [(segments_best_starts[len(autosimilarity) - 1], len(autosimilarity) - 1)]
-    precedent_frontier = segments_best_starts[len(autosimilarity) - 1] # Because a segment's start is the previous one's end.
-    while precedent_frontier > 0:
-        segments.append((segments_best_starts[precedent_frontier], precedent_frontier))
-        precedent_frontier = segments_best_starts[precedent_frontier]
-        if precedent_frontier == None:
-            raise err.ToDebugException("Well... The dynamic programming algorithm took an impossible path, so it failed. Understand why.") from None
-    return segments[::-1], scores[-1]
-
-def compute_all_kernels(max_size, bands_number = None):
-    """
-    Precomputes all kernels of size 0 ([0]) to max_size, to be reused in the CBM algorithm.
-    
-    This is used for acceleration purposes.
-
-    Parameters
-    ----------
-    max_size : integer
-        The maximal size (included) for kernels.
-    bands_number : positive integer or None, optional
-        The number of bands in the kernel. 
-        For the full kernel, bands_number must be set to None
-        (or higher than the maximal size, but cumbersome)
-        See [1] for details. 
-        The default is None.
-        
-    Returns
-    -------
-    kernels : array of arrays (which are kernels)
-        All the kernels, of size 0 ([0]) to max_size.
-
-    """
-    kernels = [[0]]
-    for p in range(1,max_size + 1):
-        if bands_number is None or p < bands_number:
-            kern = np.ones((p,p)) - np.identity(p)
-        else:
-            k = np.array([np.ones(p-i) for i in np.abs(range(-bands_number, bands_number + 1))],dtype=object)
-            offset = [i for i in range(-bands_number, bands_number + 1)]
-            kern = diags(k,offset).toarray() - np.identity(p)
-        kernels.append(kern)
-    return kernels
-
-def convolutionnal_cost(cropped_autosimilarity, kernels):
-    """
-    The convolution measure on this part of the autosimilarity matrix.
-
-    Parameters
-    ----------
-    cropped_autosimilarity : list of list of floats or numpy array (matrix representation)
-        The part of the autosimilarity which convolution measure is to compute.
-    kernels : list of arrays
-        Acceptable kernels.
-
-    Returns
-    -------
-    float
-        The convolution measure.
-
-    """
-    p = len(cropped_autosimilarity)
-    kern = kernels[p]
-    #return np.mean(np.multiply(kern,cropped_autosimilarity))
-    return np.sum(np.multiply(kern,cropped_autosimilarity)) / p**2
-    
-    
-def compute_cbm_sum_normalization(autosimilarity, min_size = 1, max_size = 32, penalty_weight = 1, penalty_func = "modulo8", bands_number = None):
-    scores = [-math.inf for i in range(len(autosimilarity))]
-    segments_best_starts = [None for i in range(len(autosimilarity))]
-    segments_best_starts[0] = 0
-    scores[0] = 0
-    kernels = compute_all_kernels(max_size, bands_number = bands_number)
-    max_conv_eight = np.amax(convolution_entire_matrix_computation(autosimilarity, kernels))
-    
-    for current_idx in range(1, len(autosimilarity)): # Parse all indexes of the autosimilarity
-        for possible_start_idx in possible_segment_start(current_idx, min_size = min_size, max_size = max_size):
-            if possible_start_idx < 0:
-                raise err.ToDebugException("Invalid value of start index, shouldn't happen.") from None
-                
-            # Convolutionnal cost between the possible start of the segment and the current index (entire segment)
-            cropped_autosimilarity = autosimilarity[possible_start_idx:current_idx,possible_start_idx:current_idx]
-            kern = kernels[len(cropped_autosimilarity)]
-            if np.sum(kern) == 0:
-                conv_cost = 0
-            else:
-                conv_cost = np.sum(np.multiply(kern,cropped_autosimilarity)) / (np.sum(kern) + len(cropped_autosimilarity))
-                        
-            segment_length = current_idx - possible_start_idx
-            penalty_cost = penalty_cost_from_arg(penalty_func, segment_length)            
-            
-            this_segment_cost = conv_cost * segment_length - penalty_cost * penalty_weight * max_conv_eight
-            # Note: conv_eight is not normalized by its size (not a problem in itself as size is contant, but generally not specified in formulas).
-
-            if possible_start_idx == 0: # Avoiding errors, as scores values are initially set to -inf.
-                if this_segment_cost > scores[current_idx]: # This segment is of larger score
-                    scores[current_idx] = this_segment_cost
-                    segments_best_starts[current_idx] = 0
-            else:
-                if scores[possible_start_idx] + this_segment_cost > scores[current_idx]: # This segment is of larger score
-                    scores[current_idx] = scores[possible_start_idx] + this_segment_cost
-                    segments_best_starts[current_idx] = possible_start_idx
-
-    segments = [(segments_best_starts[len(autosimilarity) - 1], len(autosimilarity) - 1)]
-    precedent_frontier = segments_best_starts[len(autosimilarity) - 1] # Because a segment's start is the previous one's end.
-    while precedent_frontier > 0:
-        segments.append((segments_best_starts[precedent_frontier], precedent_frontier))
-        precedent_frontier = segments_best_starts[precedent_frontier]
-        if precedent_frontier == None:
-            raise err.ToDebugException("Well... The dynamic programming algorithm took an impossible path, so it failed. Understand why.") from None
-    return segments[::-1], scores[-1]
-
-def convolution_entire_matrix_computation(autosimilarity_array, kernels, kernel_size = 8):
-    """
-    Computes the convolution measure on the entire autosimilarity matrix, with a defined and fixed kernel size.
-    
-    Parameters
-    ----------
-    autosimilarity_array : list of list of floats or numpy array (matrix representation)
-        The autosimilarity matrix.
-    kernels : list of arrays
-        All acceptable kernels.
-    kernel_size : integer
-        The size of the kernel for this measure.
-
-    Returns
-    -------
-    cost : list of float
-        List of convolution measures, at each bar of the autosimilarity.
-
-    """
-    cost = np.zeros(len(autosimilarity_array))
-    for i in range(kernel_size, len(autosimilarity_array)):
-        cost[i] = convolutionnal_cost(autosimilarity_array[i - kernel_size:i,i - kernel_size:i], kernels)
-    return cost
-
-def penalty_cost_from_arg(penalty_func, segment_length):
-    """
-    Returns a penalty cost, function of the size of the segment.
-    The penalty function has to be specified, and is bound to evolve in the near future,
-    so this docstring won't explain it.
-    Instead, you'll have to read the code, sorry! It is pretty straightforward though.
-    
-    The ``modulo'' functions are based on empirical prior knowledge,
-    following the fact that pop music is generally composed of segments of 4 or 8 bars.
-    Still, penalty values are empirically set.
-
-    Parameters
-    ----------
-    penalty_func : string
-        Identifier of the penalty function.
-    segment_length : integer
-        Size of the segment.
-
-    Returns
-    -------
-    float
-        The penalty cost.
-
-    """
-    if penalty_func == "modulo8":        
-        if segment_length == 8:
-            return 0
-        elif segment_length %4 == 0:
-            return 1/4
-        elif segment_length %2 == 0:
-            return 1/2
-        else:
-            return 1
-    if penalty_func == "modulo4":
-        if segment_length %4 == 0:
-            return 0
-        elif segment_length %2 == 0:
-            return 1/2
-        else:
-            return 1
-    if penalty_func == "modulo8modulo4":        
-        if segment_length == 8:
-            return 0
-        elif segment_length == 4:
-            return 1/4
-        elif segment_length %2 == 0:
-            return 1/2
-        else:
-            return 1
-    if penalty_func == "target_deviation_8_alpha_half": 
-         return abs(segment_length - 8) ** (1/2)
-    if penalty_func == "target_deviation_8_alpha_one": 
-         return abs(segment_length - 8)
-    if penalty_func == "target_deviation_8_alpha_two": 
-         return abs(segment_length - 8) ** 2
-    else:
-        raise err.InvalidArgumentValueException(f"Penalty function not understood {penalty_func}.")
-
-def possible_segment_start(idx, min_size = 1, max_size = None):
-    """
-    Generates the list of all possible starts of segments given the index of its end.
-    
-    Parameters
-    ----------
-    idx: integer
-        The end of a segment.
-    min_size: integer
-        Minimal length of a segment.
-    max_size: integer
-        Maximal length of a segment.
-        
-    Returns
-    -------
-    list of integers
-        All potentials starts of structural segments.
-    """
-    if min_size < 1: # No segment should be allowed to be 0 size
-        raise err.InvalidArgumentValueException(f"Invalid minimal size: {min_size} (No segment should be allowed to be 0 or negative size).")
-        #min_size = 1
-    if max_size == None:
-        return range(0, idx - min_size + 1)
-    else:
-        if idx >= max_size:
-            return range(idx - max_size, idx - min_size + 1)
-        elif idx >= min_size:
-            return range(0, idx - min_size + 1)
-        else:
-            return []
-
-# %% Sandbox
-def dynamic_convolution_computation_test_line(autosimilarity, line_conv_weight = 1, min_size = 2, max_size = 36, novelty_kernel_size = 16, penalty_weight = 1, penalty_func = "modulo8", convolution_type = "eight_bands"):
-    """
-    Segmentation algo with inline convolution test, doesn't work that much in practice.
-    """
-    costs = [-math.inf for i in range(len(autosimilarity))]
-    segments_best_starts = [None for i in range(len(autosimilarity))]
-    segments_best_starts[0] = 0
-    costs[0] = 0
-
-    kernels = compute_all_kernels(max_size, convolution_type = convolution_type)
-    full_kernels = compute_full_kernels(max_size, convolution_type = convolution_type)
-    #novelty = novelty_computation(autosimilarity, novelty_kernel_size)
-    conv_eight = convolution_entire_matrix_computation(autosimilarity, kernels)
-    
-    for current_idx in range(1, len(autosimilarity)): # Parse all indexes of the autosimilarity
-        for possible_start_idx in possible_segment_start(current_idx, min_size = min_size, max_size = max_size):
-            if possible_start_idx < 0:
-                raise err.ToDebugException("Invalid value of start index.")
-                
-            # Convolutionnal cost between the possible start of the segment and the current index (entire segment)
-            conv_cost = convolutionnal_cost(autosimilarity[possible_start_idx:current_idx,possible_start_idx:current_idx], kernels)
-
-            # Novelty cost, computed with a fixed kernel (doesn't make sense otherwise), on the end of the segment
-            #nov_cost = novelty[current_idx]
-            
-            segment_length = current_idx - possible_start_idx
-            penalty_cost = penalty_cost_from_arg(penalty_func, segment_length)            
-            
-            current_line_conv_max = 0
-            # if possible_start_idx >= segment_length:
-            #     for before_start in range(0, possible_start_idx - segment_length + 1):
-            #         line_conv_cost = convolutionnal_cost(autosimilarity[possible_start_idx:current_idx,before_start:before_start + segment_length], full_kernels)
-            #         if line_conv_cost > current_line_conv_max:
-            #             current_line_conv_max = line_conv_cost
-            
-            # if current_idx + segment_length < len(autosimilarity):
-            #     for after_start in range(current_idx, len(autosimilarity) - segment_length):
-            #         line_conv_cost = convolutionnal_cost(autosimilarity[possible_start_idx:current_idx,after_start:after_start + segment_length], full_kernels)
-            #         if line_conv_cost > current_line_conv_max:
-            #             current_line_conv_max = line_conv_cost
-            
-            mat_vec = []
-            if possible_start_idx >= segment_length:
-                for before_start in range(0, possible_start_idx - segment_length + 1):
-                    mat_vec.append(autosimilarity[possible_start_idx:current_idx,before_start:before_start + segment_length].flatten())
-
-            if current_idx + segment_length < len(autosimilarity):
-                for after_start in range(current_idx, len(autosimilarity) - segment_length):
-                    mat_vec.append(autosimilarity[possible_start_idx:current_idx,after_start:after_start + segment_length].flatten())
-
-            if mat_vec == []:
-                current_line_conv_max = 0
-            else:
-                kern = full_kernels[segment_length]
-                convs_on_line = np.matmul(kern.reshape(1,segment_length**2), np.array(mat_vec).T)                
-                current_line_conv_max = np.amax(convs_on_line) / segment_length**2
-            
-            this_segment_cost = (conv_cost + line_conv_weight * current_line_conv_max) * segment_length - penalty_cost * penalty_weight * np.max(conv_eight)
-            # Note: the length of the segment does not appear in conv_eight (not a problem in itself as size is contant, but generally not specified in formulas).
-
-            # Avoiding errors, as segment_cost are initially set to -inf.
-            if possible_start_idx == 0:
-                if this_segment_cost > costs[current_idx]:
-                    costs[current_idx] = this_segment_cost
-                    segments_best_starts[current_idx] = 0
-            else:
-                if costs[possible_start_idx] + this_segment_cost > costs[current_idx]:
-                    costs[current_idx] = costs[possible_start_idx] + this_segment_cost
-                    segments_best_starts[current_idx] = possible_start_idx
-
-    segments = [(segments_best_starts[len(autosimilarity) - 1], len(autosimilarity) - 1)]
-    precedent_frontier = segments_best_starts[len(autosimilarity) - 1] # Because a segment's start is the previous one's end.
-    while precedent_frontier > 0:
-        segments.append((segments_best_starts[precedent_frontier], precedent_frontier))
-        precedent_frontier = segments_best_starts[precedent_frontier]
-        if precedent_frontier == None:
-            raise err.ToDebugException("Well... Viterbi took an impossible path, so it failed. Understand why.") from None
-    return segments[::-1], costs[-1]
-
-
-def compute_all_kernels_oldway(max_size, convolution_type = "full"):
-    """
-    DEPRECATED but some ideas may be worth the shot.
-    
-    Precomputes all kernels of size 0 ([0]) to max_size, and feed them to the Dynamic Progamming algorithm.
-    
-    This is used for acceleration purposes.
-
-    Parameters
-    ----------
-    max_size : integer
-        The maximal size (included) for kernels.
-    convolution_type: string
-        The type of convolution. (to explicit)
-        Possibilities are :
-            - "full" : squared matrix entirely composed of one, except on the diagonal where it's zero.
-            The associated convolution cost for a segment (b_1, b_2) will be
-            .. math::
-                c_{b_1,b_2} = \\frac{1}{b_2 - b_1 + 1}\\sum_{i,j = 0, i \\ne j}^{n - 1}  a_{i + b_1, j + b_1}
-            - "4_bands" : squared matrix where the only nonzero values are ones on the 
-            4 upper- and 4 sub-diagonals surrounding the main diagonal.
-            The associated convolution cost for a segment (b_1, b_2) will be
-            .. math::
-                c_{b_1,b_2} = \\frac{1}{b_2 - b_1 + 1}\\sum_{i,j = 0, 1 \\leq |i - j| \\leq 4}^{n - 1}  a_{i + b_1, j + b_1}
-            - "mixed" : sum of both previous kernels, i.e. values are zero on the diagonal,
-            2 on the 4 upper- and 4 sub-diagonals surrounding the main diagonal, and 1 elsewhere.
-            The associated convolution cost for a segment (b_1, b_2) will be
-            .. math::
-                c_{b_1,b_2} = \\frac{1}{b_2 - b_1 + 1}(2*\\sum_{i,j = 0, 1 \\leq |i - j| \\leq 4}^{n - 1}  a_{i + b_1, j + b_1} \\ + \sum_{i,j = 0, |i - j| > 4}^{n - 1}  a_{i + b_1, j + b_1})
-        
-    Returns
-    -------
-    kernels : array of arrays (which are kernels)
-        All the kernels, of size 0 ([0]) to max_size.
-
-    """
-    kernels = [[0]]
-    for p in range(1,max_size + 1):
-        if p < 4:
-            kern = np.ones((p,p)) - np.identity(p)
-        # elif convolution_type == "7_bands" or convolution_type == "mixed_7_bands":
-        #     if p < 8:
-        #         kern = np.ones((p,p)) - np.identity(p)
-        #     else:
-        #         # Diagonal where only the six subdiagonals surrounding the main diagonal is one
-        #         k = np.array([np.ones(p-7),np.ones(p-6),np.ones(p-5),np.ones(p-4),np.ones(p-3),np.ones(p-2),np.ones(p-1),np.zeros(p),np.ones(p-1),np.ones(p-2),np.ones(p-3),np.ones(p-4),np.ones(p-5),np.ones(p-6),np.ones(p-7)], dtype=object)
-        #         offset = [-7,-6,-5,-4,-3,-2,-1,0,1,2,3, 4, 5, 6, 7]
-        #         if convolution_type == "14_bands":
-        #             kern = diags(k,offset).toarray()
-        #         else:
-        #             kern = np.ones((p,p)) - np.identity(p) + diags(k,offset).toarray()
-        else:
-            if convolution_type == "full":
-                # Full kernel (except for the diagonal)
-                kern = np.ones((p,p)) - np.identity(p)
-            elif convolution_type == "4_bands":
-                # Diagonal where only the eight subdiagonals surrounding the main diagonal is one
-                k = np.array([np.ones(p-4),np.ones(p-3),np.ones(p-2),np.ones(p-1),np.zeros(p),np.ones(p-1),np.ones(p-2),np.ones(p-3),np.ones(p-4)],dtype=object)
-                offset = [-4,-3,-2,-1,0,1,2,3,4]
-                kern = diags(k,offset).toarray()
-            elif convolution_type == "mixed":
-                # Sum of both previous kernels
-                k = np.array([np.ones(p-4),np.ones(p-3),np.ones(p-2),np.ones(p-1),np.zeros(p),np.ones(p-1),np.ones(p-2),np.ones(p-3),np.ones(p-4)],dtype=object)
-                offset = [-4,-3,-2,-1,0,1,2,3,4]
-                kern = np.ones((p,p)) - np.identity(p) + diags(k,offset).toarray()
-            elif convolution_type == "3_bands":
-                # Diagonal where only the six subdiagonals surrounding the main diagonal is one
-                k = np.array([np.ones(p-3),np.ones(p-2),np.ones(p-1),np.zeros(p),np.ones(p-1),np.ones(p-2),np.ones(p-3)],dtype=object)
-                offset = [-3,-2,-1,0,1,2,3]
-                kern = diags(k,offset).toarray()
-            elif convolution_type == "mixed_3_bands":
-                # Sum of both previous kernels
-                k = np.array([np.ones(p-3),np.ones(p-2),np.ones(p-1),np.zeros(p),np.ones(p-1),np.ones(p-2),np.ones(p-3)],dtype=object)
-                offset = [-3,-2,-1,0,1,2,3]
-                kern = np.ones((p,p)) - np.identity(p) + diags(k,offset).toarray()
-            else:
-                raise err.InvalidArgumentValueException(f"Convolution type not understood: {convolution_type}.")
-        kernels.append(kern)
-    return kernels
+# -*- coding: utf-8 -*-
+"""
+Created on Mon Feb 24 11:01:42 2020
+
+@author: amarmore
+
+Convolutive "Block-Matching" (CBM) algorithm.
+This algorithm is designed to segment barwise autosimilarities.
+
+In short, this algorithm focuses on the criteria of homogeneity to estimate segments, 
+and computes an optimal segmentation via dynamic programming.
+
+See [1] for more details.
+
+References
+----------
+[1] Marmoret, A., Cohen, J. E., & Bimbot, F., "Convolutive Block-Matching Segmentation Algorithm with Application to Music Structure Analysis", 2022, arXiv preprint arXiv:2210.15356.
+"""
+
+import as_seg.model.errors as err
+
+import math
+import numpy as np
+from scipy.sparse import diags
+import warnings
+
+def compute_cbm(autosimilarity, min_size = 1, max_size = 32, penalty_weight = 1, penalty_func = "modulo8", bands_number = None):
+    """
+    Dynamic programming algorithm, maximizing an overall score at the song scale, sum of all segments' scores on the autosimilarity.
+    Each segment' score is a combination of
+     - the convolution score on this the segment, dependong on the kernel, 
+     - a penalty cost, function of the size of the segment, to enforce specific sizes (with prior knowledge),
+
+    The penalty cost is computed in the function "penalty_cost_from_arg()".
+    See this function for further details.
+
+    It returns the optimal segmentation according to this score.
+    
+    This algortihm is also described in [1].
+    
+    IDEAS FOR FUTURE DEVELOPMENT: 
+        - May be optimized using scipy.signal.fftconvolve(), but requires a different approach in parsing all segments.
+    (i.e. parsing all possible segments for a specified kernel size and then retrieve the indexes of the diagonally-centered values)
+        - Taking into account values which are not around the diagonal but everywhere in the matrix in order to account for the repetition principle.
+
+    Parameters
+    ----------
+    autosimilarity : list of list of float (list of columns)
+        The autosimilarity to segment.
+    min_size : integer, optional
+        The minimal length of segments.
+        The default is 1.
+    max_size : integer, optional
+        The maximal length of segments.
+        The default is 32.
+    penalty_weight : float, optional
+        The ponderation parameter for the penalty function
+    penalty_func : string
+        The type of penalty function to use.
+        See "penalty_cost_from_arg()" for further details.
+    bands_number : positive integer or None, optional
+        The number of bands in the kernel. 
+        For the full kernel, bands_number must be set to None
+        (or higher than the maximal size, but cumbersome)
+        See [1] for details. 
+        The default is None.
+
+    Raises
+    ------
+    ToDebugException
+        If the program fails, generally meaning that the autosimilarity is incorrect.
+
+    Returns
+    -------
+    list of tuples
+        The segments, as a list of tuples (start, end).
+    integer
+        Global cost (the maximum among all).
+    """
+    scores = [-math.inf for i in range(len(autosimilarity))]
+    segments_best_starts = [None for i in range(len(autosimilarity))]
+    segments_best_starts[0] = 0
+    scores[0] = 0
+    kernels = compute_all_kernels(max_size, bands_number = bands_number)
+    max_conv_eight = np.amax(convolution_entire_matrix_computation(autosimilarity, kernels))
+    
+    for current_idx in range(1, len(autosimilarity)): # Parse all indexes of the autosimilarity
+        for possible_start_idx in possible_segment_start(current_idx, min_size = min_size, max_size = max_size):
+            if possible_start_idx < 0:
+                raise err.ToDebugException("Invalid value of start index, shouldn't happen.") from None
+                
+            # Convolutionnal cost between the possible start of the segment and the current index (entire segment)
+            conv_cost = convolutionnal_cost(autosimilarity[possible_start_idx:current_idx,possible_start_idx:current_idx], kernels)
+                        
+            segment_length = current_idx - possible_start_idx
+            penalty_cost = penalty_cost_from_arg(penalty_func, segment_length)            
+            
+            this_segment_cost = conv_cost * segment_length - penalty_cost * penalty_weight * max_conv_eight
+            # Note: conv_eight is not normalized by its size (not a problem in itself as size is contant, but generally not specified in formulas).
+
+            if possible_start_idx == 0: # Avoiding errors, as scores values are initially set to -inf.
+                if this_segment_cost > scores[current_idx]: # This segment is of larger score
+                    scores[current_idx] = this_segment_cost
+                    segments_best_starts[current_idx] = 0
+            else:
+                if scores[possible_start_idx] + this_segment_cost > scores[current_idx]: # This segment is of larger score
+                    scores[current_idx] = scores[possible_start_idx] + this_segment_cost
+                    segments_best_starts[current_idx] = possible_start_idx
+
+    segments = [(segments_best_starts[len(autosimilarity) - 1], len(autosimilarity) - 1)]
+    precedent_frontier = segments_best_starts[len(autosimilarity) - 1] # Because a segment's start is the previous one's end.
+    while precedent_frontier > 0:
+        segments.append((segments_best_starts[precedent_frontier], precedent_frontier))
+        precedent_frontier = segments_best_starts[precedent_frontier]
+        if precedent_frontier == None:
+            raise err.ToDebugException("Well... The dynamic programming algorithm took an impossible path, so it failed. Understand why.") from None
+    return segments[::-1], scores[-1]
+
+def compute_all_kernels(max_size, bands_number = None):
+    """
+    Precomputes all kernels of size 0 ([0]) to max_size, to be reused in the CBM algorithm.
+    
+    This is used for acceleration purposes.
+
+    Parameters
+    ----------
+    max_size : integer
+        The maximal size (included) for kernels.
+    bands_number : positive integer or None, optional
+        The number of bands in the kernel. 
+        For the full kernel, bands_number must be set to None
+        (or higher than the maximal size, but cumbersome)
+        See [1] for details. 
+        The default is None.
+        
+    Returns
+    -------
+    kernels : array of arrays (which are kernels)
+        All the kernels, of size 0 ([0]) to max_size.
+
+    """
+    kernels = [[0]]
+    for p in range(1,max_size + 1):
+        if bands_number is None or p < bands_number:
+            kern = np.ones((p,p)) - np.identity(p)
+        else:
+            k = np.array([np.ones(p-i) for i in np.abs(range(-bands_number, bands_number + 1))],dtype=object)
+            offset = [i for i in range(-bands_number, bands_number + 1)]
+            kern = diags(k,offset).toarray() - np.identity(p)
+        kernels.append(kern)
+    return kernels
+
+def convolutionnal_cost(cropped_autosimilarity, kernels):
+    """
+    The convolution measure on this part of the autosimilarity matrix.
+
+    Parameters
+    ----------
+    cropped_autosimilarity : list of list of floats or numpy array (matrix representation)
+        The part of the autosimilarity which convolution measure is to compute.
+    kernels : list of arrays
+        Acceptable kernels.
+
+    Returns
+    -------
+    float
+        The convolution measure.
+
+    """
+    p = len(cropped_autosimilarity)
+    kern = kernels[p]
+    #return np.mean(np.multiply(kern,cropped_autosimilarity))
+    return np.sum(np.multiply(kern,cropped_autosimilarity)) / p**2
+    
+    
+def compute_cbm_sum_normalization(autosimilarity, min_size = 1, max_size = 32, penalty_weight = 1, penalty_func = "modulo8", bands_number = None):
+    scores = [-math.inf for i in range(len(autosimilarity))]
+    segments_best_starts = [None for i in range(len(autosimilarity))]
+    segments_best_starts[0] = 0
+    scores[0] = 0
+    kernels = compute_all_kernels(max_size, bands_number = bands_number)
+    max_conv_eight = np.amax(convolution_entire_matrix_computation(autosimilarity, kernels))
+    
+    for current_idx in range(1, len(autosimilarity)): # Parse all indexes of the autosimilarity
+        for possible_start_idx in possible_segment_start(current_idx, min_size = min_size, max_size = max_size):
+            if possible_start_idx < 0:
+                raise err.ToDebugException("Invalid value of start index, shouldn't happen.") from None
+                
+            # Convolutionnal cost between the possible start of the segment and the current index (entire segment)
+            cropped_autosimilarity = autosimilarity[possible_start_idx:current_idx,possible_start_idx:current_idx]
+            kern = kernels[len(cropped_autosimilarity)]
+            if np.sum(kern) == 0:
+                conv_cost = 0
+            else:
+                conv_cost = np.sum(np.multiply(kern,cropped_autosimilarity)) / (np.sum(kern) + len(cropped_autosimilarity))
+                        
+            segment_length = current_idx - possible_start_idx
+            penalty_cost = penalty_cost_from_arg(penalty_func, segment_length)            
+            
+            this_segment_cost = conv_cost * segment_length - penalty_cost * penalty_weight * max_conv_eight
+            # Note: conv_eight is not normalized by its size (not a problem in itself as size is contant, but generally not specified in formulas).
+
+            if possible_start_idx == 0: # Avoiding errors, as scores values are initially set to -inf.
+                if this_segment_cost > scores[current_idx]: # This segment is of larger score
+                    scores[current_idx] = this_segment_cost
+                    segments_best_starts[current_idx] = 0
+            else:
+                if scores[possible_start_idx] + this_segment_cost > scores[current_idx]: # This segment is of larger score
+                    scores[current_idx] = scores[possible_start_idx] + this_segment_cost
+                    segments_best_starts[current_idx] = possible_start_idx
+
+    segments = [(segments_best_starts[len(autosimilarity) - 1], len(autosimilarity) - 1)]
+    precedent_frontier = segments_best_starts[len(autosimilarity) - 1] # Because a segment's start is the previous one's end.
+    while precedent_frontier > 0:
+        segments.append((segments_best_starts[precedent_frontier], precedent_frontier))
+        precedent_frontier = segments_best_starts[precedent_frontier]
+        if precedent_frontier == None:
+            raise err.ToDebugException("Well... The dynamic programming algorithm took an impossible path, so it failed. Understand why.") from None
+    return segments[::-1], scores[-1]
+
+def convolution_entire_matrix_computation(autosimilarity_array, kernels, kernel_size = 8):
+    """
+    Computes the convolution measure on the entire autosimilarity matrix, with a defined and fixed kernel size.
+    
+    Parameters
+    ----------
+    autosimilarity_array : list of list of floats or numpy array (matrix representation)
+        The autosimilarity matrix.
+    kernels : list of arrays
+        All acceptable kernels.
+    kernel_size : integer
+        The size of the kernel for this measure.
+
+    Returns
+    -------
+    cost : list of float
+        List of convolution measures, at each bar of the autosimilarity.
+
+    """
+    cost = np.zeros(len(autosimilarity_array))
+    for i in range(kernel_size, len(autosimilarity_array)):
+        cost[i] = convolutionnal_cost(autosimilarity_array[i - kernel_size:i,i - kernel_size:i], kernels)
+    return cost
+
+def penalty_cost_from_arg(penalty_func, segment_length):
+    """
+    Returns a penalty cost, function of the size of the segment.
+    The penalty function has to be specified, and is bound to evolve in the near future,
+    so this docstring won't explain it.
+    Instead, you'll have to read the code, sorry! It is pretty straightforward though.
+    
+    The ``modulo'' functions are based on empirical prior knowledge,
+    following the fact that pop music is generally composed of segments of 4 or 8 bars.
+    Still, penalty values are empirically set.
+
+    Parameters
+    ----------
+    penalty_func : string
+        Identifier of the penalty function.
+    segment_length : integer
+        Size of the segment.
+
+    Returns
+    -------
+    float
+        The penalty cost.
+
+    """
+    if penalty_func == "modulo8":        
+        if segment_length == 8:
+            return 0
+        elif segment_length %4 == 0:
+            return 1/4
+        elif segment_length %2 == 0:
+            return 1/2
+        else:
+            return 1
+    if penalty_func == "modulo4":
+        if segment_length %4 == 0:
+            return 0
+        elif segment_length %2 == 0:
+            return 1/2
+        else:
+            return 1
+    if penalty_func == "modulo8modulo4":        
+        if segment_length == 8:
+            return 0
+        elif segment_length == 4:
+            return 1/4
+        elif segment_length %2 == 0:
+            return 1/2
+        else:
+            return 1
+    if penalty_func == "target_deviation_8_alpha_half": 
+         return abs(segment_length - 8) ** (1/2)
+    if penalty_func == "target_deviation_8_alpha_one": 
+         return abs(segment_length - 8)
+    if penalty_func == "target_deviation_8_alpha_two": 
+         return abs(segment_length - 8) ** 2
+    else:
+        raise err.InvalidArgumentValueException(f"Penalty function not understood {penalty_func}.")
+
+def possible_segment_start(idx, min_size = 1, max_size = None):
+    """
+    Generates the list of all possible starts of segments given the index of its end.
+    
+    Parameters
+    ----------
+    idx: integer
+        The end of a segment.
+    min_size: integer
+        Minimal length of a segment.
+    max_size: integer
+        Maximal length of a segment.
+        
+    Returns
+    -------
+    list of integers
+        All potentials starts of structural segments.
+    """
+    if min_size < 1: # No segment should be allowed to be 0 size
+        raise err.InvalidArgumentValueException(f"Invalid minimal size: {min_size} (No segment should be allowed to be 0 or negative size).")
+        #min_size = 1
+    if max_size == None:
+        return range(0, idx - min_size + 1)
+    else:
+        if idx >= max_size:
+            return range(idx - max_size, idx - min_size + 1)
+        elif idx >= min_size:
+            return range(0, idx - min_size + 1)
+        else:
+            return []
+
+# %% Sandbox
+def dynamic_convolution_computation_test_line(autosimilarity, line_conv_weight = 1, min_size = 2, max_size = 36, novelty_kernel_size = 16, penalty_weight = 1, penalty_func = "modulo8", convolution_type = "eight_bands"):
+    """
+    Segmentation algo with inline convolution test, doesn't work that much in practice.
+    """
+    costs = [-math.inf for i in range(len(autosimilarity))]
+    segments_best_starts = [None for i in range(len(autosimilarity))]
+    segments_best_starts[0] = 0
+    costs[0] = 0
+
+    kernels = compute_all_kernels(max_size, convolution_type = convolution_type)
+    full_kernels = compute_full_kernels(max_size, convolution_type = convolution_type)
+    #novelty = novelty_computation(autosimilarity, novelty_kernel_size)
+    conv_eight = convolution_entire_matrix_computation(autosimilarity, kernels)
+    
+    for current_idx in range(1, len(autosimilarity)): # Parse all indexes of the autosimilarity
+        for possible_start_idx in possible_segment_start(current_idx, min_size = min_size, max_size = max_size):
+            if possible_start_idx < 0:
+                raise err.ToDebugException("Invalid value of start index.")
+                
+            # Convolutionnal cost between the possible start of the segment and the current index (entire segment)
+            conv_cost = convolutionnal_cost(autosimilarity[possible_start_idx:current_idx,possible_start_idx:current_idx], kernels)
+
+            # Novelty cost, computed with a fixed kernel (doesn't make sense otherwise), on the end of the segment
+            #nov_cost = novelty[current_idx]
+            
+            segment_length = current_idx - possible_start_idx
+            penalty_cost = penalty_cost_from_arg(penalty_func, segment_length)            
+            
+            current_line_conv_max = 0
+            # if possible_start_idx >= segment_length:
+            #     for before_start in range(0, possible_start_idx - segment_length + 1):
+            #         line_conv_cost = convolutionnal_cost(autosimilarity[possible_start_idx:current_idx,before_start:before_start + segment_length], full_kernels)
+            #         if line_conv_cost > current_line_conv_max:
+            #             current_line_conv_max = line_conv_cost
+            
+            # if current_idx + segment_length < len(autosimilarity):
+            #     for after_start in range(current_idx, len(autosimilarity) - segment_length):
+            #         line_conv_cost = convolutionnal_cost(autosimilarity[possible_start_idx:current_idx,after_start:after_start + segment_length], full_kernels)
+            #         if line_conv_cost > current_line_conv_max:
+            #             current_line_conv_max = line_conv_cost
+            
+            mat_vec = []
+            if possible_start_idx >= segment_length:
+                for before_start in range(0, possible_start_idx - segment_length + 1):
+                    mat_vec.append(autosimilarity[possible_start_idx:current_idx,before_start:before_start + segment_length].flatten())
+
+            if current_idx + segment_length < len(autosimilarity):
+                for after_start in range(current_idx, len(autosimilarity) - segment_length):
+                    mat_vec.append(autosimilarity[possible_start_idx:current_idx,after_start:after_start + segment_length].flatten())
+
+            if mat_vec == []:
+                current_line_conv_max = 0
+            else:
+                kern = full_kernels[segment_length]
+                convs_on_line = np.matmul(kern.reshape(1,segment_length**2), np.array(mat_vec).T)                
+                current_line_conv_max = np.amax(convs_on_line) / segment_length**2
+            
+            this_segment_cost = (conv_cost + line_conv_weight * current_line_conv_max) * segment_length - penalty_cost * penalty_weight * np.max(conv_eight)
+            # Note: the length of the segment does not appear in conv_eight (not a problem in itself as size is contant, but generally not specified in formulas).
+
+            # Avoiding errors, as segment_cost are initially set to -inf.
+            if possible_start_idx == 0:
+                if this_segment_cost > costs[current_idx]:
+                    costs[current_idx] = this_segment_cost
+                    segments_best_starts[current_idx] = 0
+            else:
+                if costs[possible_start_idx] + this_segment_cost > costs[current_idx]:
+                    costs[current_idx] = costs[possible_start_idx] + this_segment_cost
+                    segments_best_starts[current_idx] = possible_start_idx
+
+    segments = [(segments_best_starts[len(autosimilarity) - 1], len(autosimilarity) - 1)]
+    precedent_frontier = segments_best_starts[len(autosimilarity) - 1] # Because a segment's start is the previous one's end.
+    while precedent_frontier > 0:
+        segments.append((segments_best_starts[precedent_frontier], precedent_frontier))
+        precedent_frontier = segments_best_starts[precedent_frontier]
+        if precedent_frontier == None:
+            raise err.ToDebugException("Well... Viterbi took an impossible path, so it failed. Understand why.") from None
+    return segments[::-1], costs[-1]
+
+
+def compute_all_kernels_oldway(max_size, convolution_type = "full"):
+    """
+    DEPRECATED but some ideas may be worth the shot.
+    
+    Precomputes all kernels of size 0 ([0]) to max_size, and feed them to the Dynamic Progamming algorithm.
+    
+    This is used for acceleration purposes.
+
+    Parameters
+    ----------
+    max_size : integer
+        The maximal size (included) for kernels.
+    convolution_type: string
+        The type of convolution. (to explicit)
+        Possibilities are :
+            - "full" : squared matrix entirely composed of one, except on the diagonal where it's zero.
+            The associated convolution cost for a segment (b_1, b_2) will be
+            .. math::
+                c_{b_1,b_2} = \\frac{1}{b_2 - b_1 + 1}\\sum_{i,j = 0, i \\ne j}^{n - 1}  a_{i + b_1, j + b_1}
+            - "4_bands" : squared matrix where the only nonzero values are ones on the 
+            4 upper- and 4 sub-diagonals surrounding the main diagonal.
+            The associated convolution cost for a segment (b_1, b_2) will be
+            .. math::
+                c_{b_1,b_2} = \\frac{1}{b_2 - b_1 + 1}\\sum_{i,j = 0, 1 \\leq |i - j| \\leq 4}^{n - 1}  a_{i + b_1, j + b_1}
+            - "mixed" : sum of both previous kernels, i.e. values are zero on the diagonal,
+            2 on the 4 upper- and 4 sub-diagonals surrounding the main diagonal, and 1 elsewhere.
+            The associated convolution cost for a segment (b_1, b_2) will be
+            .. math::
+                c_{b_1,b_2} = \\frac{1}{b_2 - b_1 + 1}(2*\\sum_{i,j = 0, 1 \\leq |i - j| \\leq 4}^{n - 1}  a_{i + b_1, j + b_1} \\ + \sum_{i,j = 0, |i - j| > 4}^{n - 1}  a_{i + b_1, j + b_1})
+        
+    Returns
+    -------
+    kernels : array of arrays (which are kernels)
+        All the kernels, of size 0 ([0]) to max_size.
+
+    """
+    kernels = [[0]]
+    for p in range(1,max_size + 1):
+        if p < 4:
+            kern = np.ones((p,p)) - np.identity(p)
+        # elif convolution_type == "7_bands" or convolution_type == "mixed_7_bands":
+        #     if p < 8:
+        #         kern = np.ones((p,p)) - np.identity(p)
+        #     else:
+        #         # Diagonal where only the six subdiagonals surrounding the main diagonal is one
+        #         k = np.array([np.ones(p-7),np.ones(p-6),np.ones(p-5),np.ones(p-4),np.ones(p-3),np.ones(p-2),np.ones(p-1),np.zeros(p),np.ones(p-1),np.ones(p-2),np.ones(p-3),np.ones(p-4),np.ones(p-5),np.ones(p-6),np.ones(p-7)], dtype=object)
+        #         offset = [-7,-6,-5,-4,-3,-2,-1,0,1,2,3, 4, 5, 6, 7]
+        #         if convolution_type == "14_bands":
+        #             kern = diags(k,offset).toarray()
+        #         else:
+        #             kern = np.ones((p,p)) - np.identity(p) + diags(k,offset).toarray()
+        else:
+            if convolution_type == "full":
+                # Full kernel (except for the diagonal)
+                kern = np.ones((p,p)) - np.identity(p)
+            elif convolution_type == "4_bands":
+                # Diagonal where only the eight subdiagonals surrounding the main diagonal is one
+                k = np.array([np.ones(p-4),np.ones(p-3),np.ones(p-2),np.ones(p-1),np.zeros(p),np.ones(p-1),np.ones(p-2),np.ones(p-3),np.ones(p-4)],dtype=object)
+                offset = [-4,-3,-2,-1,0,1,2,3,4]
+                kern = diags(k,offset).toarray()
+            elif convolution_type == "mixed":
+                # Sum of both previous kernels
+                k = np.array([np.ones(p-4),np.ones(p-3),np.ones(p-2),np.ones(p-1),np.zeros(p),np.ones(p-1),np.ones(p-2),np.ones(p-3),np.ones(p-4)],dtype=object)
+                offset = [-4,-3,-2,-1,0,1,2,3,4]
+                kern = np.ones((p,p)) - np.identity(p) + diags(k,offset).toarray()
+            elif convolution_type == "3_bands":
+                # Diagonal where only the six subdiagonals surrounding the main diagonal is one
+                k = np.array([np.ones(p-3),np.ones(p-2),np.ones(p-1),np.zeros(p),np.ones(p-1),np.ones(p-2),np.ones(p-3)],dtype=object)
+                offset = [-3,-2,-1,0,1,2,3]
+                kern = diags(k,offset).toarray()
+            elif convolution_type == "mixed_3_bands":
+                # Sum of both previous kernels
+                k = np.array([np.ones(p-3),np.ones(p-2),np.ones(p-1),np.zeros(p),np.ones(p-1),np.ones(p-2),np.ones(p-3)],dtype=object)
+                offset = [-3,-2,-1,0,1,2,3]
+                kern = np.ones((p,p)) - np.identity(p) + diags(k,offset).toarray()
+            else:
+                raise err.InvalidArgumentValueException(f"Convolution type not understood: {convolution_type}.")
+        kernels.append(kern)
+    return kernels
```

### Comparing `as_seg-0.1.5/as_seg/autosimilarity_computation.py` & `as_seg-0.1.6/as_seg/autosimilarity_computation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,246 +1,254 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Mar 14 16:30:31 2022
-
-@author: amarmore
-
-Module used to compute autosimilarity matrices.
-"""
-import as_seg.model.errors as err
-
-import numpy as np
-import sklearn.metrics.pairwise as pairwise_distances
-import warnings
-
-def switch_autosimilarity(an_array, similarity_type, gamma = None, normalise = True):
-    """
-    High-level function to compute the autosimilarity of this matrix.
-    
-    Expects a matrix of shape (Bars, Feature representation).
-    
-    Computes it with different possible similarity function s_{x_i,x_j} (given two bars denoted as x_i and x_j):
-        - "cosine" for the cosine similarity, i.e. the normalised dot product:
-        .. math::
-            s_{x_i,x_j} = \\frac{\langle x_i, x_j \rangle}{||x_i|| ||x_j||}
-        -"covariance" for a covariance similarity, 
-        i.e. the dot product of centered features:
-        .. math::
-            s_{x_i,x_j} = \langle x_i - \hat{x}, x_j - \hat{x} \rangle
-        -"rbf" for the Radial Basis Function similarity, 
-        i.e. the exponent of the opposite of the euclidean distance between features:
-        .. math::
-            s_{x_i,x_j} = \\exp^{-\\gamma ||x_i - x_j||_2}
-        The euclidean distance can be the distance between the normalised features.
-        Gamma is a parameter.
-        See rbf_kernel from scikit-learn for more details.
-    
-    Parameters
-    ----------
-    an_array : numpy array
-        The array/matrix seen as array which autosimilarity will be computed.
-        Expected to be of shape (Bars, Feature representation).
-    similarity_type : string
-        Either "cosine", "covariance" or "rbf".
-        It represents the similarity function used for computing the autosimilarity.
-    gamma : positive float, optional
-        The gamma parameter in the rbf function, only used for the "rbf" similarity.
-        The default is None, meaning that it is computed as function of the standard deviation,
-        see get_gamma_std() for more details.
-    normalise : boolean, optional
-        Whether features should be normalised or not. 
-        Normalisation depends on the similarity function.
-        The default is True.
-
-    Returns
-    -------
-    numpy array
-        Autosimilarity matrix of the input an_array.
-
-    """
-    if similarity_type.lower() == "cosine":
-        return get_cosine_autosimilarity(an_array)#, normalise = normalise)
-    elif similarity_type.lower() == "covariance":
-        return get_covariance_autosimilarity(an_array, normalise = normalise)
-    elif similarity_type.lower() == "rbf":
-        return get_rbf_autosimilarity(an_array, gamma, normalise = normalise)
-    elif similarity_type.lower() == "centered_rbf":
-        return get_centered_rbf_autosimilarity(an_array, gamma, normalise = normalise)
-    else:
-        raise err.InvalidArgumentValueException(f"Incorrect similarity type: {similarity_type}. Should be cosine, covariance or rbf.")
-        
-def l2_normalise_barwise(an_array):
-    """
-    Normalises the array barwise (i.e., in its first dimension) by the l_2 norm.
-    
-    Null values are replaced by the small positive value of 10^{-10}.
-
-    Parameters
-    ----------
-    an_array : numpy array
-        The array which needs to be normalised.
-
-    Returns
-    -------
-    numpy array
-        The normalised array.
-
-    """
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", message="invalid value encountered in true_divide") # Avoiding to show the warning, as it's handled, not te confuse the user.
-        an_array_T = an_array.T/np.linalg.norm(an_array, axis = 1)
-        an_array_T = np.where(np.isnan(an_array_T), 1e-10, an_array_T) # Replace null lines, avoiding future errors in handling values.
-    return an_array_T.T
-
-def get_cosine_autosimilarity(an_array):#, normalise = True):
-    """
-    Computes the autosimilarity matrix with the cosine similarity function.
-    
-    The cosine similarity function is the normalised dot product between two bars, i.e.:
-    .. math::
-        s_{x_i,x_j} = \\frac{\langle x_i, x_j \rangle}{||x_i|| ||x_j||}
-    
-    Parameters
-    ----------
-    an_array : numpy array
-        The array/matrix seen as array which autosimilarity os to compute.
-        Expected to be of shape (Bars, Feature representation).
-
-    Returns
-    -------
-    numpy array
-        The autosimilarity of this array, with the cosine similarity function.
-
-    """
-    if type(an_array) is list:
-        this_array = np.array(an_array)
-    else:
-        this_array = an_array
-    #if normalise:
-    this_array = l2_normalise_barwise(this_array)
-    return this_array@this_array.T
-
-def get_covariance_autosimilarity(an_array, normalise = True):
-    """
-    Computes the autosimilarity matrix, where the similarity function is the covariance.
-    
-    The covariance similarity function corresponds to the dot product of centered features:
-    .. math::
-        s_{x_i,x_j} = \langle x_i - \hat{x}, x_j - \hat{x} \rangle
-
-    Parameters
-    ----------
-    an_array : numpy array
-        The array/matrix seen as array which autosimilarity will be computed.
-    normalise : boolean, optional
-        Whether features should be normalised or not. 
-        Normalisation here means that each centered feature is normalised by its norm.
-        The default is True.
-        
-    Returns
-    -------
-    numpy array
-        The covariance autosimilarity of this array.
-
-    """
-    if type(an_array) is list:
-        this_array = np.array(an_array)
-    else:
-        this_array = an_array
-    this_array = this_array - this_array.mean(axis=0) # centering, i.e. subtracting the average value row-wise
-    if normalise:
-        this_array = l2_normalise_barwise(this_array)
-    return this_array@this_array.T
-
-def get_rbf_autosimilarity(an_array, gamma = None, normalise = True):
-    """
-    Computes the autosimilarity matrix, where the similarity function is the Radial Basis Function (RBF).
-    
-    The RBF corresponds to the exponent of the opposite of the euclidean distance between features:
-    .. math::
-        s_{x_i,x_j} = \\exp^{-\\gamma ||x_i - x_j||_2}
-        
-    The RBF is computed via scikit-learn.
-    The default gamma value is computed in function get_gamma_std(), refer to that function for further details.
-
-    Parameters
-    ----------
-    an_array : numpy array
-        The array/matrix seen as array which autosimilarity will be computed.
-    gamma : positive float, optional
-        The gamma parameter in the rbf function.
-        The default is None, meaning that it is computed as function of the standard deviation,
-        see get_gamma_std() for more details.
-    normalise : boolean, optional
-        Whether features should be normalised or not. 
-        Normalisation here means that the euclidean norm is computed between normalised vectors.
-        The default is True.
-
-    Returns
-    -------
-    numpy array
-        The RBF autosimilarity of this array.
-
-    """
-    if type(an_array) is list:
-        this_array = np.array(an_array)
-    else:
-        this_array = an_array
-    if gamma == None:
-        gamma = get_gamma_std(this_array, scaling_factor = 1, no_diag = True, normalise = normalise)
-    if normalise:
-        this_array = l2_normalise_barwise(this_array)
-    return pairwise_distances.rbf_kernel(this_array, gamma = gamma)
-    
-def get_centered_rbf_autosimilarity(an_array, gamma = None, normalise = True):
-    """
-    TODO
-    """
-    if type(an_array) is list:
-        this_array = np.array(an_array)
-    else:
-        this_array = an_array
-    this_array = this_array - this_array.mean(axis=0) # centering, i.e. subtracting the average value row-wise
-    if gamma == None:
-        gamma = get_gamma_std(this_array, scaling_factor = 1, no_diag = True, normalise = normalise)
-    if normalise:
-        this_array = l2_normalise_barwise(this_array)
-    return pairwise_distances.rbf_kernel(this_array, gamma = gamma)
-
-
-def get_gamma_std(an_array, scaling_factor = 1, no_diag = True, normalise = True):
-    """
-    Default value for the gamma in the RBF similarity function.
-    
-    This default value is proportional to the inverse of the standard deviation of the values, more experiments should be made to fit it.
-    For now, it has been set quite empirically.
-
-    Parameters
-    ----------
-    an_array : numpy array
-        The array/matrix seen as array which autosimilarity will be computed.
-    scaling_factor : positive float, optional
-        Weigthing parameter, relating to the inverse of the standard deviation. 
-        The default is 1.
-    no_diag : boolen, optional
-        Whether the diagonal values (self similarity values) should be discarded (True) or taken into account (False). 
-        The default is True.
-    normalise : boolean, optional
-        Whether features should be normalised or not. 
-        Normalisation here means that the euclidean norm is computed between normalised vectors.
-        The default is True.
-
-    Returns
-    -------
-    gamma : float
-        The gamma parameter in the RBF similarity function.
-
-    """
-    if normalise:
-        an_array = l2_normalise_barwise(an_array)
-    euc_dist = pairwise_distances.euclidean_distances(an_array)
-    if not no_diag:
-        return scaling_factor/(2*np.std(euc_dist))
-    else:
-        for i in range(len(euc_dist)):
-            euc_dist[i,i] = float('NaN')
+# -*- coding: utf-8 -*-
+"""
+Created on Mon Mar 14 16:30:31 2022
+
+@author: amarmore
+
+Module used to compute autosimilarity matrices.
+"""
+import as_seg.model.errors as err
+
+import numpy as np
+import sklearn.metrics.pairwise as pairwise_distances
+import warnings
+eps = 1e-10
+
+def switch_autosimilarity(an_array, similarity_type, gamma = None, normalise = True):
+    """
+    High-level function to compute the autosimilarity of this matrix.
+    
+    Expects a matrix of shape (Bars, Feature representation).
+    
+    Computes it with different possible similarity function s_{x_i,x_j} (given two bars denoted as x_i and x_j):
+        - "cosine" for the cosine similarity, i.e. the normalised dot product:
+        .. math::
+            s_{x_i,x_j} = \\frac{\langle x_i, x_j \rangle}{||x_i|| ||x_j||}
+        -"covariance" for a covariance similarity, 
+        i.e. the dot product of centered features:
+        .. math::
+            s_{x_i,x_j} = \langle x_i - \hat{x}, x_j - \hat{x} \rangle
+        -"rbf" for the Radial Basis Function similarity, 
+        i.e. the exponent of the opposite of the euclidean distance between features:
+        .. math::
+            s_{x_i,x_j} = \\exp^{-\\gamma ||x_i - x_j||_2}
+        The euclidean distance can be the distance between the normalised features.
+        Gamma is a parameter.
+        See rbf_kernel from scikit-learn for more details.
+    
+    Parameters
+    ----------
+    an_array : numpy array
+        The array/matrix seen as array which autosimilarity will be computed.
+        Expected to be of shape (Bars, Feature representation).
+    similarity_type : string
+        Either "cosine", "covariance" or "rbf".
+        It represents the similarity function used for computing the autosimilarity.
+    gamma : positive float, optional
+        The gamma parameter in the rbf function, only used for the "rbf" similarity.
+        The default is None, meaning that it is computed as function of the standard deviation,
+        see get_gamma_std() for more details.
+    normalise : boolean, optional
+        Whether features should be normalised or not. 
+        Normalisation depends on the similarity function.
+        The default is True.
+
+    Returns
+    -------
+    numpy array
+        Autosimilarity matrix of the input an_array.
+
+    """
+    if similarity_type.lower() == "cosine":
+        return get_cosine_autosimilarity(an_array)#, normalise = normalise)
+    elif similarity_type.lower() == "autocorrelation" or similarity_type.lower() == "covariance":
+        return get_autocorrelation_autosimilarity(an_array, normalise = normalise)
+    elif similarity_type.lower() == "rbf":
+        return get_rbf_autosimilarity(an_array, gamma, normalise = normalise)
+    elif similarity_type.lower() == "centered_rbf":
+        return get_centered_rbf_autosimilarity(an_array, gamma, normalise = normalise)
+    else:
+        raise err.InvalidArgumentValueException(f"Incorrect similarity type: {similarity_type}. Should be cosine, covariance or rbf.")
+        
+def l2_normalise_barwise(an_array):
+    """
+    Normalises the array barwise (i.e., in its first dimension) by the l_2 norm.
+    
+    Null values are replaced by the small positive value of 10^{-10}.
+
+    Parameters
+    ----------
+    an_array : numpy array
+        The array which needs to be normalised.
+
+    Returns
+    -------
+    numpy array
+        The normalised array.
+
+    """
+    norm = np.linalg.norm(an_array, axis = 1)
+    an_array_T = np.transpose(an_array)
+    out = np.inf * np.ones_like(an_array_T)
+    np.divide(an_array_T, norm, out = out, where=norm!=0)
+    an_array_T = np.where(np.isinf(out), eps, out)
+    return np.transpose(an_array_T)
+
+def get_cosine_autosimilarity(an_array):#, normalise = True):
+    """
+    Computes the autosimilarity matrix with the cosine similarity function.
+    
+    The cosine similarity function is the normalised dot product between two bars, i.e.:
+    .. math::
+        s_{x_i,x_j} = \\frac{\langle x_i, x_j \rangle}{||x_i|| ||x_j||}
+    
+    Parameters
+    ----------
+    an_array : numpy array
+        The array/matrix seen as array which autosimilarity os to compute.
+        Expected to be of shape (Bars, Feature representation).
+
+    Returns
+    -------
+    numpy array
+        The autosimilarity of this array, with the cosine similarity function.
+
+    """
+    if type(an_array) is list:
+        this_array = np.array(an_array)
+    else:
+        this_array = an_array
+    #if normalise:
+    this_array = l2_normalise_barwise(this_array)
+    return this_array@this_array.T
+
+def get_covariance_autosimilarity(an_array, normalise = True):
+    """
+    Note: deprecated. The name of the matrix became "Autocorrelation" in the TISMIR version of the paper.
+    """
+    return get_autocorrelation_autosimilarity(an_array, normalise = normalise)
+
+def get_autocorrelation_autosimilarity(an_array, normalise = True):
+    """
+    Computes the autosimilarity matrix, where the similarity function is the autocorrelation.
+    
+    The autocorrelation similarity function corresponds to the dot product of centered features:
+    .. math::
+        s_{x_i,x_j} = \langle x_i - \hat{x}, x_j - \hat{x} \rangle
+
+    Parameters
+    ----------
+    an_array : numpy array
+        The array/matrix seen as array which autosimilarity will be computed.
+    normalise : boolean, optional
+        Whether features should be normalised or not. 
+        Normalisation here means that each centered feature is normalised by its norm.
+        The default is True.
+        
+    Returns
+    -------
+    numpy array
+        The autocorrelation autosimilarity of this array.
+
+    """
+    if type(an_array) is list:
+        this_array = np.array(an_array)
+    else:
+        this_array = an_array
+    this_array = this_array - this_array.mean(axis=0) # centering, i.e. subtracting the average value row-wise
+    if normalise:
+        this_array = l2_normalise_barwise(this_array)
+    return this_array@this_array.T
+
+def get_rbf_autosimilarity(an_array, gamma = None, normalise = True):
+    """
+    Computes the autosimilarity matrix, where the similarity function is the Radial Basis Function (RBF).
+    
+    The RBF corresponds to the exponent of the opposite of the euclidean distance between features:
+    .. math::
+        s_{x_i,x_j} = \\exp^{-\\gamma ||x_i - x_j||_2}
+        
+    The RBF is computed via scikit-learn.
+    The default gamma value is computed in function get_gamma_std(), refer to that function for further details.
+
+    Parameters
+    ----------
+    an_array : numpy array
+        The array/matrix seen as array which autosimilarity will be computed.
+    gamma : positive float, optional
+        The gamma parameter in the rbf function.
+        The default is None, meaning that it is computed as function of the standard deviation,
+        see get_gamma_std() for more details.
+    normalise : boolean, optional
+        Whether features should be normalised or not. 
+        Normalisation here means that the euclidean norm is computed between normalised vectors.
+        The default is True.
+
+    Returns
+    -------
+    numpy array
+        The RBF autosimilarity of this array.
+
+    """
+    if type(an_array) is list:
+        this_array = np.array(an_array)
+    else:
+        this_array = an_array
+    if gamma == None:
+        gamma = get_gamma_std(this_array, scaling_factor = 1, no_diag = True, normalise = normalise)
+    if normalise:
+        this_array = l2_normalise_barwise(this_array)
+    return pairwise_distances.rbf_kernel(this_array, gamma = gamma)
+    
+def get_centered_rbf_autosimilarity(an_array, gamma = None, normalise = True):
+    """
+    TODO
+    """
+    if type(an_array) is list:
+        this_array = np.array(an_array)
+    else:
+        this_array = an_array
+    this_array = this_array - this_array.mean(axis=0) # centering, i.e. subtracting the average value row-wise
+    if gamma == None:
+        gamma = get_gamma_std(this_array, scaling_factor = 1, no_diag = True, normalise = normalise)
+    if normalise:
+        this_array = l2_normalise_barwise(this_array)
+    return pairwise_distances.rbf_kernel(this_array, gamma = gamma)
+
+
+def get_gamma_std(an_array, scaling_factor = 1, no_diag = True, normalise = True):
+    """
+    Default value for the gamma in the RBF similarity function.
+    
+    This default value is proportional to the inverse of the standard deviation of the values, more experiments should be made to fit it.
+    For now, it has been set quite empirically.
+
+    Parameters
+    ----------
+    an_array : numpy array
+        The array/matrix seen as array which autosimilarity will be computed.
+    scaling_factor : positive float, optional
+        Weigthing parameter, relating to the inverse of the standard deviation. 
+        The default is 1.
+    no_diag : boolen, optional
+        Whether the diagonal values (self similarity values) should be discarded (True) or taken into account (False). 
+        The default is True.
+    normalise : boolean, optional
+        Whether features should be normalised or not. 
+        Normalisation here means that the euclidean norm is computed between normalised vectors.
+        The default is True.
+
+    Returns
+    -------
+    gamma : float
+        The gamma parameter in the RBF similarity function.
+
+    """
+    if normalise:
+        an_array = l2_normalise_barwise(an_array)
+    euc_dist = pairwise_distances.euclidean_distances(an_array)
+    if not no_diag:
+        return scaling_factor/(2*np.std(euc_dist))
+    else:
+        for i in range(len(euc_dist)):
+            euc_dist[i,i] = float('NaN')
         return scaling_factor/(2*np.nanstd(euc_dist))
```

### Comparing `as_seg-0.1.5/as_seg/data_manipulation.py` & `as_seg-0.1.6/as_seg/data_manipulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,30 +45,22 @@
     Madmom: A new python audio and music signal processing library. 
     In Proceedings of the 24th ACM international conference on Multimedia (pp. 1174-1178).
 
     """
     act = dbt.RNNDownBeatProcessor()(song_path)
     proc = dbt.DBNDownBeatTrackingProcessor(beats_per_bar=[3,4], fps=100)
     song_beats = proc(act)
-    downbeats_times = []
+    downbeats_times = [song_beats[0][0]]
     
-    if song_beats[0][1] != 1: # Adding a first downbeat at the start of the song
-        downbeats_times.append(0.1)
-    for beat in song_beats:
+    for beat in song_beats[1:]: # The first beat is already added
         if beat[1] == 1: # If the beat is a downbeat
             downbeats_times.append(beat[0])
             
-    # The following block of code artificially adds bars to the end of the song, in order to span the total song length.
-    # It seems like a good idea initially but may be detrimental, and should be debated anyway.
-    average_bar_length = np.mean([downbeats_times[i + 1] - downbeats_times[i] for i in range(len(downbeats_times) - 1)]) # average bar length in the song
     song_length = act.shape[0]/100 # Total length of the song
-    while downbeats_times[-1] + 1.1*average_bar_length < song_length: # As long as the bar estimation does not cover the entire song
-        downbeats_times.append(round(downbeats_times[-1] + average_bar_length, 2)) # artifically adds bars of the length of the average bar length in the song
     downbeats_times.append(song_length) # adding the last downbeat
-    
     return frontiers_to_segments(downbeats_times)
     
 def get_beats_from_audio_msaf(signal, sr, hop_length):
     _, audio_percussive = librosa.effects.hpss(signal)
     
     # Compute beats
     _, beat_frames = librosa.beat.beat_track(y=audio_percussive, sr=sr, hop_length=hop_length)
@@ -87,16 +79,16 @@
 def get_beats_from_audio_madmom(song_path):
     """
     TODO
     """
     act = bt.TCNBeatProcessor()(song_path)
     proc = bt.BeatTrackingProcessor(fps=100)
     song_beats = proc(act)
-    beats_times = []
     
+    # beats_times = []    
     # if song_beats[0][1] != 1: # Adding a first downbeat at the start of the song
         # beats_times.append(0.1)
     # for beat in song_beats:
         # if beat[1] == 1: # If the beat is a downbeat
             # downbeats_times.append(beat[0])
             
     return frontiers_to_segments(list(song_beats))
@@ -431,15 +423,47 @@
             frontiers_on_bars.append(frontier)
         else:
             if bars[i][1] - frontier < frontier - bars[i][0]:
                 frontiers_on_bars.append(bars[i][1])
             else:
                 frontiers_on_bars.append(bars[i][0])
     return frontiers_on_bars
-            
+
+def get_median_hop(bars, subdivision = 96, sampling_rate = 44100):
+    """
+    Returns the median hop length in the song, used for audio reconstruction.
+    The rationale is that all bars are sampled with 'subdivision' number of frames, 
+    but they can be of different lengths in absolute time.
+    Hence, the time gap between two consecutive frames (the hop length) can differ between bars.
+    For reconstruction, we use the median hop length among all bars.
+
+    Parameters
+    ----------
+    bars : list of tuples of float
+        The bars, as (start time, end time) tuples.
+    subdivision : integer, optional
+        The number of subdivision of the bar to be contained in each slice of the tensor.
+        The default is 96.
+    sampling_rate : integer, optional
+        The sampling rate of the signal, in Hz.
+        The default is 44100.
+
+    Returns
+    -------
+    integer
+        The median hop length in these bars.
+
+    """
+    hops = []
+    for bar_idx in range(1, len(bars)):
+        len_sig = bars[bar_idx][1] - bars[bar_idx][0]
+        hop = int(len_sig/subdivision * sampling_rate)
+        hops.append(hop)
+    return int(np.median(hops)) # Generally used for audio reconstruction
+
 # %% Sonification of the segmentation
 def sonify_frontiers_path(audio_file_path, frontiers_in_seconds, output_path):
     """
     Takes the path of the song and frontiers, and write a song with the frontiers sonified ("bip" in the song).
     Function inspired from MSAF.
 
     Parameters
@@ -555,22 +579,22 @@
         F measure of these frontiers,
         ie the geometric mean of both precedent scores.
 
     """
     ref_intervals, useless = mir_eval.util.adjust_intervals(reference,t_min=0)
     est_intervals, useless = mir_eval.util.adjust_intervals(np.array(segments_in_time), t_min=0, t_max=ref_intervals[-1, 1])
     try:
-        return mir_eval.segment.detection(ref_intervals, est_intervals, window = window_length, trim = False)
+        return mir_eval.segment.detection(ref_intervals, est_intervals, window = window_length, trim = True)
     except ValueError:
         cleaned_intervals = []
         #print("A segment is (probably) composed of the same start and end. Can happen with time -> bar -> time conversion, but should'nt happen for data originally segmented in bars.")
         for idx in range(len(est_intervals)):
             if est_intervals[idx][0] != est_intervals[idx][1]:
                 cleaned_intervals.append(est_intervals[idx])
-        return mir_eval.segment.detection(ref_intervals, np.array(cleaned_intervals), window = window_length, trim = False)
+        return mir_eval.segment.detection(ref_intervals, np.array(cleaned_intervals), window = window_length, trim = True)
 
 def compute_median_deviation_of_segmentation(reference, segments_in_time):
     """
     TODO
 
     Parameters
     ----------
```

### Comparing `as_seg-0.1.5/as_seg/example.py` & `as_seg-0.1.6/as_seg/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Module for reading signals
 import librosa
 
 # Module to handle annotations for MIR files
 import mirdata
 
 # Module encapsulating the computation of features from the signal
-import as_seg.model.features as features
+import as_seg.model.signal_to_spectrogram as signal_to_spectrogram
 
 # General module for manipulating data: conversion between time, bars, frame indexes, loading of data, ...
 import as_seg.data_manipulation as dm
 
 # Module to process the input in barwise features
 import as_seg.barwise_input as bi
 
@@ -32,15 +32,15 @@
 # Module containing the CBM algorithm
 import as_seg.CBM_algorithm as cbm
 
 # Plotting module
 from as_seg.model.current_plot import *
 
 # %% Loading annotations and defining the audio path
-path_to_beatles_dataset = 'C:/Users/amarmore/this_folder/Beatles dataset/' # To change
+path_to_beatles_dataset = '/home/a23marmo/datasets/beatles' # To change
 beatles = mirdata.initialize('beatles', path_to_beatles_dataset)
 beatles.download()
 
 # NB: you have to place the file "01_-_Come_Together.wav" manually in the folder "audio/11_-_Abbey_Road/"
 come_together = beatles.track('1101')
 
 references_segments = beatles.load_sections(come_together.sections_path).intervals
@@ -52,15 +52,15 @@
 bars = dm.get_bars_from_audio(song_path)
 
 # %% Computing the features
 hop_length = 32 # Oversampling the spectrogram, to select frames which will be equally-spaced barwise.
 hop_length_seconds = hop_length/sampling_rate # As bars are in seconds, we convert this hop length in seconds.
 subdivision_bars = 96 # The number of time samples to consider in each bar.
 
-log_mel = features.get_spectrogram(the_signal, sampling_rate, "log_mel_grill", hop_length = hop_length) # Log_mel spectrogram
+log_mel = signal_to_spectrogram.get_spectrogram(the_signal, sampling_rate, "log_mel", hop_length = hop_length) # Log_mel spectrogram
 
 # %% Cosine autosimilarity
 barwise_TF_cosine = bi.barwise_TF_matrix(log_mel, bars, hop_length_seconds, subdivision_bars)
 barwise_TF_cosine_autosimilarity = as_computation.switch_autosimilarity(barwise_TF_cosine, "cosine")
 #Alternatively, one could use: as_computation.get_cosine_autosimilarity(barwise_TF_cosine)
 plot_me_this_spectrogram(barwise_TF_cosine_autosimilarity, title = "Cosine autosimilarity of the Barwise TF matrix")
```

### Comparing `as_seg-0.1.5/as_seg/foote_novelty.py` & `as_seg-0.1.6/as_seg/foote_novelty.py`

 * *Files identical despite different names*

### Comparing `as_seg-0.1.5/as_seg/model/current_plot.py` & `as_seg-0.1.6/as_seg/model/current_plot.py`

 * *Files identical despite different names*

### Comparing `as_seg-0.1.5/as_seg/model/display_results.py` & `as_seg-0.1.6/as_seg/model/display_results.py`

 * *Files identical despite different names*

### Comparing `as_seg-0.1.5/as_seg/model/errors.py` & `as_seg-0.1.6/as_seg/model/errors.py`

 * *Files identical despite different names*

### Comparing `as_seg-0.1.5/as_seg/scripts/default_path.py` & `as_seg-0.1.6/as_seg/scripts/default_path.py`

 * *Files identical despite different names*

### Comparing `as_seg-0.1.5/as_seg/scripts/overall_scripts.py` & `as_seg-0.1.6/as_seg/scripts/overall_scripts.py`

 * *Files identical despite different names*

### Comparing `as_seg-0.1.5/as_seg.egg-info/PKG-INFO` & `as_seg-0.1.6/as_seg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: as-seg
-Version: 0.1.5
+Version: 0.1.6
 Summary: Package for the segmentation of autosimilarity matrices. This version is related to a stable vesion on PyPi, for installation in MSAF.
 Home-page: https://gitlab.inria.fr/amarmore/autosimilarity_segmentation
 Author: Marmoret Axel
 Author-email: axel.marmoret@imt-atlantique.fr
 License: BSD
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `as_seg-0.1.5/as_seg.egg-info/SOURCES.txt` & `as_seg-0.1.6/as_seg.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 as_seg.egg-info/PKG-INFO
 as_seg.egg-info/SOURCES.txt
 as_seg.egg-info/dependency_links.txt
 as_seg.egg-info/requires.txt
 as_seg.egg-info/top_level.txt
 as_seg/model/__init__.py
 as_seg/model/current_plot.py
+as_seg/model/dataloaders.py
 as_seg/model/display_results.py
 as_seg/model/errors.py
-as_seg/model/features.py
+as_seg/model/signal_to_spectrogram.py
 as_seg/scripts/__init__.py
 as_seg/scripts/default_path.py
 as_seg/scripts/overall_scripts.py
```

### Comparing `as_seg-0.1.5/setup.py` & `as_seg-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="as_seg",
-    version="0.1.5",
+    version="0.1.6",
     author="Marmoret Axel",
     author_email="axel.marmoret@imt-atlantique.fr",
     description="Package for the segmentation of autosimilarity matrices. This version is related to a stable vesion on PyPi, for installation in MSAF.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.inria.fr/amarmore/autosimilarity_segmentation",
     packages=setuptools.find_packages(),
```

