# Comparing `tmp/barmuscomp-0.1.4.tar.gz` & `tmp/barmuscomp-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barmuscomp-0.1.4.tar", last modified: Thu May  2 15:59:36 2024, max compression
+gzip compressed data, was "barmuscomp-0.1.5.tar", last modified: Mon May  6 15:44:49 2024, max compression
```

## Comparing `barmuscomp-0.1.4.tar` & `barmuscomp-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-02 15:59:36.619294 barmuscomp-0.1.4/
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       88 2023-10-26 01:08:08.000000 barmuscomp-0.1.4/AUTHORS
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     1503 2024-01-10 11:57:04.000000 barmuscomp-0.1.4/LICENSE.md
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     3689 2024-05-02 15:59:36.619294 barmuscomp-0.1.4/PKG-INFO
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     2985 2023-10-26 01:08:08.000000 barmuscomp-0.1.4/README.md
-drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-02 15:59:36.619294 barmuscomp-0.1.4/barmuscomp/
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      305 2024-01-10 11:57:01.000000 barmuscomp-0.1.4/barmuscomp/__init__.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    36646 2024-01-10 11:57:01.000000 barmuscomp-0.1.4/barmuscomp/ae.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    19648 2024-01-10 11:57:02.000000 barmuscomp-0.1.4/barmuscomp/ae_ntd.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    13589 2024-01-10 11:57:02.000000 barmuscomp-0.1.4/barmuscomp/ae_utils.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    13546 2024-01-10 11:57:02.000000 barmuscomp-0.1.4/barmuscomp/lra.py
-drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-02 15:59:36.619294 barmuscomp-0.1.4/barmuscomp/model/
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        0 2023-10-26 01:08:08.000000 barmuscomp-0.1.4/barmuscomp/model/__init__.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     7339 2024-01-31 09:55:24.000000 barmuscomp-0.1.4/barmuscomp/model/current_plot.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     3039 2023-10-26 01:08:08.000000 barmuscomp-0.1.4/barmuscomp/model/early_stopping.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      201 2024-01-10 11:57:03.000000 barmuscomp-0.1.4/barmuscomp/model/errors.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     4388 2024-01-10 11:57:03.000000 barmuscomp-0.1.4/barmuscomp/model/features.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    19983 2024-01-10 11:57:03.000000 barmuscomp-0.1.4/barmuscomp/model/pattern_study.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     4910 2024-01-10 11:57:03.000000 barmuscomp-0.1.4/barmuscomp/model/plot_comparison_ae_ntd.py
-drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-02 15:59:36.619294 barmuscomp-0.1.4/barmuscomp/scripts/
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        0 2023-10-26 01:08:08.000000 barmuscomp-0.1.4/barmuscomp/scripts/__init__.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     1790 2024-01-10 11:57:03.000000 barmuscomp-0.1.4/barmuscomp/scripts/default_path.py
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     7444 2024-01-10 11:57:04.000000 barmuscomp-0.1.4/barmuscomp/scripts/overall_scripts.py
-drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-02 15:59:36.619294 barmuscomp-0.1.4/barmuscomp.egg-info/
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     3689 2024-05-02 15:59:36.000000 barmuscomp-0.1.4/barmuscomp.egg-info/PKG-INFO
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      642 2024-05-02 15:59:36.000000 barmuscomp-0.1.4/barmuscomp.egg-info/SOURCES.txt
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        1 2024-05-02 15:59:36.000000 barmuscomp-0.1.4/barmuscomp.egg-info/dependency_links.txt
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      177 2024-05-02 15:59:36.000000 barmuscomp-0.1.4/barmuscomp.egg-info/requires.txt
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       11 2024-05-02 15:59:36.000000 barmuscomp-0.1.4/barmuscomp.egg-info/top_level.txt
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       38 2024-05-02 15:59:36.619294 barmuscomp-0.1.4/setup.cfg
--rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     1305 2024-05-02 15:57:42.000000 barmuscomp-0.1.4/setup.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-06 15:44:49.330005 barmuscomp-0.1.5/
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       88 2023-10-26 01:08:08.000000 barmuscomp-0.1.5/AUTHORS
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     1503 2024-01-10 11:57:04.000000 barmuscomp-0.1.5/LICENSE.md
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     3689 2024-05-06 15:44:49.330005 barmuscomp-0.1.5/PKG-INFO
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     2985 2023-10-26 01:08:08.000000 barmuscomp-0.1.5/README.md
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-06 15:44:49.326005 barmuscomp-0.1.5/barmuscomp/
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)      416 2024-05-06 15:35:28.000000 barmuscomp-0.1.5/barmuscomp/__init__.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    36646 2024-01-10 11:57:01.000000 barmuscomp-0.1.5/barmuscomp/ae.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    19648 2024-01-10 11:57:02.000000 barmuscomp-0.1.5/barmuscomp/ae_ntd.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    13589 2024-01-10 11:57:02.000000 barmuscomp-0.1.5/barmuscomp/ae_utils.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    13546 2024-01-10 11:57:02.000000 barmuscomp-0.1.5/barmuscomp/lra.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-06 15:44:49.330005 barmuscomp-0.1.5/barmuscomp/model/
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)        0 2022-12-23 14:40:38.000000 barmuscomp-0.1.5/barmuscomp/model/__init__.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     1554 2024-05-06 15:36:49.000000 barmuscomp-0.1.5/barmuscomp/model/audio_helper.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     7448 2024-05-06 15:38:12.000000 barmuscomp-0.1.5/barmuscomp/model/current_plot.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     3039 2021-09-22 13:36:36.000000 barmuscomp-0.1.5/barmuscomp/model/early_stopping.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)      460 2024-05-06 14:46:57.000000 barmuscomp-0.1.5/barmuscomp/model/errors.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)    15967 2024-05-06 15:33:34.000000 barmuscomp-0.1.5/barmuscomp/model/factorisation_to_signal.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     5093 2024-05-06 15:36:00.000000 barmuscomp-0.1.5/barmuscomp/model/plot_comparison_ae_ntd.py
+-rwxrwxrwx   0 a23marmo  (1000) a23marmo  (1000)     4548 2024-05-06 15:30:35.000000 barmuscomp-0.1.5/barmuscomp/model/signal_to_spectrogram.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     1718 2024-05-06 15:32:10.000000 barmuscomp-0.1.5/barmuscomp/model/spectrogram_to_signal.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-06 15:44:49.330005 barmuscomp-0.1.5/barmuscomp/scripts/
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        0 2023-10-26 01:08:08.000000 barmuscomp-0.1.5/barmuscomp/scripts/__init__.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     1790 2024-01-10 11:57:03.000000 barmuscomp-0.1.5/barmuscomp/scripts/default_path.py
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     7444 2024-01-10 11:57:04.000000 barmuscomp-0.1.5/barmuscomp/scripts/overall_scripts.py
+drwxrwxr-x   0 a23marmo  (1000) a23marmo  (1000)        0 2024-05-06 15:44:49.330005 barmuscomp-0.1.5/barmuscomp.egg-info/
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     3689 2024-05-06 15:44:49.000000 barmuscomp-0.1.5/barmuscomp.egg-info/PKG-INFO
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      740 2024-05-06 15:44:49.000000 barmuscomp-0.1.5/barmuscomp.egg-info/SOURCES.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)        1 2024-05-06 15:44:49.000000 barmuscomp-0.1.5/barmuscomp.egg-info/dependency_links.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)      177 2024-05-06 15:44:49.000000 barmuscomp-0.1.5/barmuscomp.egg-info/requires.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       11 2024-05-06 15:44:49.000000 barmuscomp-0.1.5/barmuscomp.egg-info/top_level.txt
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)       38 2024-05-06 15:44:49.330005 barmuscomp-0.1.5/setup.cfg
+-rw-rw-r--   0 a23marmo  (1000) a23marmo  (1000)     1305 2024-05-06 15:43:27.000000 barmuscomp-0.1.5/setup.py
```

### Comparing `barmuscomp-0.1.4/LICENSE.md` & `barmuscomp-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.4/PKG-INFO` & `barmuscomp-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barmuscomp
-Version: 0.1.4
+Version: 0.1.5
 Summary: Package for barwise compression applied on musical segmentation.
 Home-page: https://gitlab.inria.fr/amarmore/barmuscomp
 Author: Marmoret Axel
 Author-email: axel.marmoret@irisa.fr
 License: BSD
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `barmuscomp-0.1.4/README.md` & `barmuscomp-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.4/barmuscomp/ae.py` & `barmuscomp-0.1.5/barmuscomp/ae.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.4/barmuscomp/ae_ntd.py` & `barmuscomp-0.1.5/barmuscomp/ae_ntd.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.4/barmuscomp/ae_utils.py` & `barmuscomp-0.1.5/barmuscomp/ae_utils.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.4/barmuscomp/lra.py` & `barmuscomp-0.1.5/barmuscomp/lra.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.4/barmuscomp/model/current_plot.py` & `barmuscomp-0.1.5/barmuscomp/model/current_plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,163 +1,160 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Fri Feb 22 16:29:17 2019
-
-@author: amarmore
-
-Defining common plotting functions.
-
-NB: This module's name actually comes from an incorrect translation
-from the french "courant" into "current", instead of "common".
-Please excuse me for this translation.
-"""
-
-import as_seg.autosimilarity_computation as as_comp
-
-from sklearn.decomposition import PCA
-import numpy as np
-import matplotlib.pyplot as plt
-import matplotlib.cm as cm
-import pandas as pd
-import IPython.display as ipd
-
-# %% Load everything from as_seg
-from as_seg.model.current_plot import *
-
-# %% NTD specific
-def plot_me_this_tucker(factors, core, cmap = cm.Greys):
-    """
-    Plot all factors, and each slice of the core (as musical pattern) from the NTD.
-    """
-    plot_me_this_spectrogram(factors[0], title = "Midi factor", x_axis = "Atoms", y_axis = "Midi value", invert_y_axis = False, cmap = cmap)
-    plot_me_this_spectrogram(factors[1].T, title = "Rythmic patterns factor", x_axis = "Position in bar", y_axis = "Atoms", cmap = cmap)
-    plot_me_this_spectrogram(factors[2].T, title = "Structural patterns factor", x_axis = "Bar index", y_axis = "Atoms", cmap = cmap)
-    print("Core:")
-    for i in range(len(core[0,0,:])):
-        plot_me_this_spectrogram(core[:,:,i], title = "Core, slice " + str(i), x_axis = "Time atoms", y_axis = "Freq Atoms", cmap = cmap)
-
-def permutate_factor(factor):
-    """
-    Computes the permutation of columns of the factors for them to be visually more comprehensible.
-    """
-    permutations = []
-    for i in factor:
-        idx_max = np.argmax(i)
-        if idx_max not in permutations:
-            permutations.append(idx_max)
-    for i in range(factor.shape[1]):
-        if i not in permutations:
-            permutations.append(i)
-    return permutations
-
-def plot_permuted_factor(factor, title = None,x_axis = None, y_axis = None, cmap = cm.Greys):
-    """
-    Plots this factor, but permuted to be easier to understand visually.
-    """
-    permut = permutate_factor(factor)
-    plot_me_this_spectrogram(factor.T[permut], title = title,x_axis = x_axis, y_axis = y_axis,
-                             figsize=(factor.shape[0]/10,factor.shape[1]/10), cmap = cmap)
-
-def plot_permuted_tucker(factors, core, cmap = cm.Greys, plot_core = True):
-    """
-    Plots every factor and slice of the core from the NTD, but permuted to be easier to understand visually.
-    """
-    plot_me_this_spectrogram(factors[0], title = "W matrix (muscial content)",
-                         x_axis = "Atoms", y_axis = "Pitch-class Index", cmap = cmap)
-    h_permut = permutate_factor(factors[1])
-    plot_me_this_spectrogram(factors[1].T[h_permut], title = "H matrix: time at barscale (rythmic content)",
-                             x_axis = "Position in the bar\n(in frame indexes)", y_axis = "Atoms\n(permuted for\nvisualization purpose)", 
-                             figsize=(factors[1].shape[0]/10,factors[1].shape[1]/10), cmap = cmap)
-    q_permut = permutate_factor(factors[2])
-    plot_me_this_spectrogram(factors[2].T[q_permut], title = "Q matrix: Bar content feature",
-                             x_axis = "Index of the bar", y_axis = "Musical pattern index\n(permuted for\nvisualization purpose)", 
-                             figsize=(factors[2].shape[0]/10,factors[2].shape[1]/10), cmap = cmap)
-    if plot_core:
-        for i, idx in enumerate(q_permut):
-            plot_me_this_spectrogram(core[:,h_permut,idx], title = "Core, slice {} (slice {} in original decomposition order)".format(i, idx), x_axis = "Time atoms", y_axis = "Freq Atoms", cmap = cm.Greys)
-  
-
-# %% Plotting audio files, in order to listen to them
-def plot_audio_list_in_dataframe(audios_list):
-    """
-    Print this list of audio signals in a list.
-    """
-    #Never tested, tocheck
-    df = pd.DataFrame(np.array(audios_list), columns = ["All patterns"]).T
-    #df[0] = df[0].apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
-    for i in range(df.shape[1]):
-        df[i] = df[i].T.apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
-    df_html = df.T.to_html(escape=False, index=False)
-    ipd.display(ipd.HTML(df_html))
-    
-# %% Single-Song AutoEncoders specific
-def plot_latent_space(latent_vectors, labels = None):
-    """
-    Visualization of the latent projection, as the matrix of representation, and as both autosimilarity and PCA of latent vectors.
-
-    Parameters
-    ----------
-    latent_vectors : array
-        Concatenation of the latent vectors, or matrix of latent representations. 
-        (same mathematical meaning but can be of different computation types.)
-    labels : None or array, optional
-        If labels are set, they will be used to color the output of PCA projection.
-        If they are set to None, no label is used. The default is None.
-
-    Returns
-    -------
-    None, but plots latent visualizations.
-
-    """
-    np_lv = np.array(latent_vectors)
-    plot_me_this_spectrogram(np_lv.T, figsize=(np_lv.shape[0]/5,np_lv.shape[1]/5), title = "z matrix", x_axis = "Bar index", y_axis = "Latent space")
-    
-    fig, axs = plt.subplots(1, 2, figsize=(15,7))
-
-    autosimil = as_comp.switch_autosimilarity(latent_vectors, similarity_type = "cosine", normalise = True)
-    padded_autosimil = pad_factor(autosimil)
-    axs[0].pcolormesh(np.arange(padded_autosimil.shape[1]), np.arange(padded_autosimil.shape[0]), padded_autosimil, cmap = cm.Greys)
-    axs[0].set_title('Autosimilarity of the z (projection in latent space)')
-    axs[0].invert_yaxis()
-    axs[0].set_xlabel("Bar index")
-    axs[0].set_ylabel("Bar index")
-    
-    if np_lv.shape[1] == 2:
-        if not isinstance(labels,np.ndarray) and labels == None:
-            axs[1].scatter(np_lv[:,0],np_lv[:,1])
-        else:
-            axs[1].scatter(np_lv[:,0],np_lv[:,1], c=labels)
-    else:
-        pca = PCA(n_components=2)
-        principalComponents = pca.fit_transform(np_lv)
-        if not isinstance(labels,np.ndarray) and labels == None:
-            axs[1].scatter(principalComponents[:,0],principalComponents[:,1])
-        else:
-            axs[1].scatter(principalComponents[:,0],principalComponents[:,1], c=labels)
-
-    axs[1].set_title('PCA of the z (projection in the latent space)')
-    plt.show()
-
-# %% AE-NTD
-def plot_audio_diff_ntd_ae_in_dataframe(signal_ntd, signal_ae):
-    df = pd.DataFrame(np.array([signal_ntd, signal_ae]), index = ["Audio NTD", "Audio AE"])
-    for i in range(df.shape[1]):
-        df[i] = df[i].T.apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
-    df_html = df.T.to_html(escape=False, index=False)
-    ipd.display(ipd.HTML(df_html))
-    
-import pandas as pd
-import IPython.display as ipd
-
-def plot_audio_diff_beta_in_dataframe(signal_beta2, signal_beta1, signal_beta0):
-    """
-    Plots the different reconstruction with different beta values in a dataframe.
-    Hardcoded for Beta = 2, 1 and 0.
-    """
-    df = pd.DataFrame(np.array([signal_beta2, signal_beta1, signal_beta0]), index = ["beta = 2", "beta = 1", "beta = 0"])
-    #df[0] = df[0].apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
-    for i in range(df.shape[1]):
-        df[i] = df[i].T.apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
-    df_html = df.T.to_html(escape=False, index=False)
-    ipd.display(ipd.HTML(df_html))
-
-
+# -*- coding: utf-8 -*-
+"""
+Created on Fri Feb 22 16:29:17 2019
+
+@author: amarmore
+
+Defining common plotting functions.
+
+NB: This module's name actually comes from an incorrect translation
+from the french "courant" into "current", instead of "common".
+Please excuse me for this translation.
+"""
+
+import as_seg.autosimilarity_computation as as_comp
+
+from sklearn.decomposition import PCA
+import numpy as np
+import matplotlib.pyplot as plt
+import matplotlib.cm as cm
+import pandas as pd
+import IPython.display as ipd
+
+# %% Load everything from as_seg
+from as_seg.model.current_plot import *
+
+# %% NTD specific
+def plot_me_this_tucker(factors, core, cmap = cm.Greys):
+    """
+    Plot all factors, and each slice of the core (as musical pattern) from the NTD.
+    """
+    plot_me_this_spectrogram(factors[0], title = "Midi factor", x_axis = "Atoms", y_axis = "Midi value", invert_y_axis = False, cmap = cmap)
+    plot_me_this_spectrogram(factors[1].T, title = "Rythmic patterns factor", x_axis = "Position in bar", y_axis = "Atoms", cmap = cmap)
+    plot_me_this_spectrogram(factors[2].T, title = "Structural patterns factor", x_axis = "Bar index", y_axis = "Atoms", cmap = cmap)
+    print("Core:")
+    for i in range(len(core[0,0,:])):
+        plot_me_this_spectrogram(core[:,:,i], title = "Core, slice " + str(i), x_axis = "Time atoms", y_axis = "Freq Atoms", cmap = cmap)
+
+def permutate_factor(factor):
+    """
+    Computes the permutation of columns of the factors for them to be visually more comprehensible.
+    """
+    permutations = []
+    for i in factor:
+        idx_max = np.argmax(i)
+        if idx_max not in permutations:
+            permutations.append(idx_max)
+    for i in range(factor.shape[1]):
+        if i not in permutations:
+            permutations.append(i)
+    return permutations
+
+def plot_permuted_factor(factor, title = None,x_axis = None, y_axis = None, cmap = cm.Greys):
+    """
+    Plots this factor, but permuted to be easier to understand visually.
+    """
+    permut = permutate_factor(factor)
+    plot_me_this_spectrogram(factor.T[permut], title = title,x_axis = x_axis, y_axis = y_axis,
+                             figsize=(factor.shape[0]/10,factor.shape[1]/10), cmap = cmap)
+
+def plot_permuted_tucker(factors, core, cmap = cm.Greys, plot_core = True):
+    """
+    Plots every factor and slice of the core from the NTD, but permuted to be easier to understand visually.
+    """
+    plot_me_this_spectrogram(factors[0], title = "W matrix (muscial content)",
+                         x_axis = "Atoms", y_axis = "Pitch-class Index", cmap = cmap)
+    h_permut = permutate_factor(factors[1])
+    plot_me_this_spectrogram(factors[1].T[h_permut], title = "H matrix: time at barscale (rythmic content)",
+                             x_axis = "Position in the bar\n(in frame indexes)", y_axis = "Atoms\n(permuted for\nvisualization purpose)", 
+                             figsize=(factors[1].shape[0]/10,factors[1].shape[1]/10), cmap = cmap)
+    q_permut = permutate_factor(factors[2])
+    plot_me_this_spectrogram(factors[2].T[q_permut], title = "Q matrix: Bar content feature",
+                             x_axis = "Index of the bar", y_axis = "Musical pattern index\n(permuted for\nvisualization purpose)", 
+                             figsize=(factors[2].shape[0]/10,factors[2].shape[1]/10), cmap = cmap)
+    if plot_core:
+        for i, idx in enumerate(q_permut):
+            plot_me_this_spectrogram(core[:,h_permut,idx], title = "Core, slice {} (slice {} in original decomposition order)".format(i, idx), x_axis = "Time atoms", y_axis = "Freq Atoms", cmap = cm.Greys)
+  
+
+# %% Plotting audio files, in order to listen to them
+def plot_audio_list_in_dataframe(audios_list):
+    """
+    Print this list of audio signals in a list.
+    """
+    #Never tested, tocheck
+    df = pd.DataFrame(np.array(audios_list), columns = ["All patterns"]).T
+    #df[0] = df[0].apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
+    for i in range(df.shape[1]):
+        df[i] = df[i].T.apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
+    df_html = df.T.to_html(escape=False, index=False)
+    ipd.display(ipd.HTML(df_html))
+    
+# %% Single-Song AutoEncoders specific
+def plot_latent_space(latent_vectors, labels = None):
+    """
+    Visualization of the latent projection, as the matrix of representation, and as both autosimilarity and PCA of latent vectors.
+
+    Parameters
+    ----------
+    latent_vectors : array
+        Concatenation of the latent vectors, or matrix of latent representations. 
+        (same mathematical meaning but can be of different computation types.)
+    labels : None or array, optional
+        If labels are set, they will be used to color the output of PCA projection.
+        If they are set to None, no label is used. The default is None.
+
+    Returns
+    -------
+    None, but plots latent visualizations.
+
+    """
+    np_lv = np.array(latent_vectors)
+    plot_me_this_spectrogram(np_lv.T, figsize=(np_lv.shape[0]/5,np_lv.shape[1]/5), title = "z matrix", x_axis = "Bar index", y_axis = "Latent space")
+    
+    fig, axs = plt.subplots(1, 2, figsize=(15,7))
+
+    autosimil = as_comp.switch_autosimilarity(latent_vectors, similarity_type = "cosine", normalise = True)
+    padded_autosimil = pad_factor(autosimil)
+    axs[0].pcolormesh(np.arange(padded_autosimil.shape[1]), np.arange(padded_autosimil.shape[0]), padded_autosimil, cmap = cm.Greys)
+    axs[0].set_title('Autosimilarity of the z (projection in latent space)')
+    axs[0].invert_yaxis()
+    axs[0].set_xlabel("Bar index")
+    axs[0].set_ylabel("Bar index")
+    
+    if np_lv.shape[1] == 2:
+        if not isinstance(labels,np.ndarray) and labels == None:
+            axs[1].scatter(np_lv[:,0],np_lv[:,1])
+        else:
+            axs[1].scatter(np_lv[:,0],np_lv[:,1], c=labels)
+    else:
+        pca = PCA(n_components=2)
+        principalComponents = pca.fit_transform(np_lv)
+        if not isinstance(labels,np.ndarray) and labels == None:
+            axs[1].scatter(principalComponents[:,0],principalComponents[:,1])
+        else:
+            axs[1].scatter(principalComponents[:,0],principalComponents[:,1], c=labels)
+
+    axs[1].set_title('PCA of the z (projection in the latent space)')
+    plt.show()
+
+# %% AE-NTD
+def plot_audio_diff_ntd_ae_in_dataframe(signal_ntd, signal_ae):
+    df = pd.DataFrame(np.array([signal_ntd, signal_ae]), index = ["Audio NTD", "Audio AE"])
+    for i in range(df.shape[1]):
+        df[i] = df[i].T.apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
+    df_html = df.T.to_html(escape=False, index=False)
+    ipd.display(ipd.HTML(df_html))
+    
+def plot_audio_diff_beta_in_dataframe(signal_beta2, signal_beta1, signal_beta0):
+    """
+    Plots the different reconstruction with different beta values in a dataframe.
+    Hardcoded for Beta = 2, 1 and 0.
+    """
+    df = pd.DataFrame(np.array([signal_beta2, signal_beta1, signal_beta0]), index = ["beta = 2", "beta = 1", "beta = 0"])
+    #df[0] = df[0].apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
+    for i in range(df.shape[1]):
+        df[i] = df[i].T.apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
+    df_html = df.T.to_html(escape=False, index=False)
+    ipd.display(ipd.HTML(df_html))
+
+
```

### Comparing `barmuscomp-0.1.4/barmuscomp/model/early_stopping.py` & `barmuscomp-0.1.5/barmuscomp/model/early_stopping.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.4/barmuscomp/model/features.py` & `barmuscomp-0.1.5/barmuscomp/model/signal_to_spectrogram.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Mar 25 16:54:59 2020
-
-@author: amarmore
-"""
-
-import barmuscomp.model.errors as err
-
-# %% Load everything from as_seg
-from as_seg.model.features import *
-# See details in as_seg
-
-# %% HCQT
-def get_hcqt_params():
-    """
-    Credit to & al. [1] (comes directly from https://github.com/rabitt/ismir2017-deepsalience)
-    
-    Fixing parameters for the HCQT computation.
-
-    Returns
-    -------
-    bins_per_octave : TYPE
-        DESCRIPTION.
-    n_octaves : TYPE
-        DESCRIPTION.
-    harmonics : TYPE
-        DESCRIPTION.
-    sr : TYPE
-        DESCRIPTION.
-    fmin : TYPE
-        DESCRIPTION.
-    hop_length : TYPE
-        DESCRIPTION.
-        
-    References
-    ----------
-    [1] Bittner, R. M., McFee, B., Salamon, J., Li, P., & Bello, J. P. (2017, October). 
-    Deep Salience Representations for F0 Estimation in Polyphonic Music. In ISMIR (pp. 63-70).
-
-    """
-    bins_per_octave = 60
-    n_octaves = 6
-    harmonics = [0.5, 1, 2, 3, 4, 5]
-    sr = 22050
-    fmin = 32.7
-    hop_length = 256
-    return bins_per_octave, n_octaves, harmonics, sr, fmin, hop_length
-
-
-def compute_hcqt_bittner(signal, sr):
-    """
-    Credit to Bittner & al. [1] (comes from https://github.com/rabitt/ismir2017-deepsalience).
-    
-    Computes HCQT representation of the signal, as presented in [1] (3-rd order tensor).
-
-    Parameters
-    ----------
-    signal : numpy array
-        Signal of the song.
-    sr : int
-        the sampling_rate
-
-    Returns
-    -------
-    log_hcqt : np array
-        The tensor of logarithm HCQT.
-        
-    References
-    ----------
-    [1] Bittner, R. M., McFee, B., Salamon, J., Li, P., & Bello, J. P. (2017, October). 
-    Deep Salience Representations for F0 Estimation in Polyphonic Music. In ISMIR (pp. 63-70).
-    """
-    (bins_per_octave, n_octaves, harmonics,
-     sr, f_min, hop_length) = get_hcqt_params()
-    #y, fs = librosa.load(audio_fpath, sr=sr)
-
-    cqt_list = []
-    shapes = []
-    for h in harmonics:
-        cqt = librosa.cqt(
-            signal, sr=sr, hop_length=hop_length, fmin=f_min*float(h),
-            n_bins=bins_per_octave*n_octaves,
-            bins_per_octave=bins_per_octave
-        )
-        cqt_list.append(cqt)
-        shapes.append(cqt.shape)
-
-    shapes_equal = [s == shapes[0] for s in shapes]
-    if not all(shapes_equal):
-        min_time = np.min([s[1] for s in shapes])
-        new_cqt_list = []
-        for i in range(len(cqt_list)):
-            new_cqt_list.append(cqt_list[i][:, :min_time])
-        cqt_list = new_cqt_list
-
-    log_hcqt = ((1.0/80.0) * librosa.core.amplitude_to_db(
-        np.abs(np.array(cqt_list)), ref=np.max)) + 1.0
-
-    return log_hcqt
-
-def my_compute_hcqt(signal, sr):
-    """
-    Credit to Bittner & al. [1] (comes from https://github.com/rabitt/ismir2017-deepsalience).
-    
-    Computes HCQT representation of the signal, as presented in [1] (3-rd order tensor).
-    The order of the mode is changed though, so tht first two modes correspond to frequency and time respectively,
-    and that the third corresponds to harmonic content.
-
-    Parameters
-    ----------
-    signal : numpy array
-        Signal of the song.
-    sr : int
-        the sampling_rate
-
-    Returns
-    -------
-    log_hcqt : np array
-        The tensor of logarithm HCQT.
-        
-    References
-    ----------
-    [1] Bittner, R. M., McFee, B., Salamon, J., Li, P., & Bello, J. P. (2017, October). 
-    Deep Salience Representations for F0 Estimation in Polyphonic Music. In ISMIR (pp. 63-70).
-    """
-    (bins_per_octave, n_octaves, harmonics, sr, f_min, hop_length) = get_hcqt_params()
-
-    freq_mode_len = bins_per_octave*n_octaves
-
-    first_cqt = librosa.cqt(signal, sr=sr, hop_length=hop_length, fmin=f_min*float(harmonics[0]),
-                            n_bins=freq_mode_len, bins_per_octave=bins_per_octave)
-
-    time_mode_len = first_cqt.shape[1]
-    
-    h_cqt = np.array(first_cqt).reshape(freq_mode_len, time_mode_len, 1)
-    
-    for h in harmonics[1:]:
-        cqt = librosa.cqt(signal, sr=sr, hop_length=hop_length, fmin=f_min*float(h),
-            n_bins=bins_per_octave*n_octaves,bins_per_octave=bins_per_octave)
-        current_cqt = cqt.reshape(freq_mode_len, time_mode_len, 1)
-        h_cqt = np.append(h_cqt, current_cqt, axis = 2)
-
-    log_hcqt = ((1.0/80.0) * librosa.core.amplitude_to_db(np.abs(h_cqt), ref=np.max)) + 1.0
-
-    return log_hcqt
-
+# -*- coding: utf-8 -*-
+"""
+Created on Wed Mar 25 16:54:59 2020
+
+@author: amarmore
+"""
+
+import barmuscomp.model.errors as err
+
+# %% Load everything from as_seg
+from as_seg.model.signal_to_spectrogram import *
+# See details in as_seg
+
+# %% HCQT
+def get_hcqt_params():
+    """
+    Credit to & al. [1] (comes directly from https://github.com/rabitt/ismir2017-deepsalience)
+    
+    Fixing parameters for the HCQT computation.
+
+    Returns
+    -------
+    bins_per_octave : TYPE
+        DESCRIPTION.
+    n_octaves : TYPE
+        DESCRIPTION.
+    harmonics : TYPE
+        DESCRIPTION.
+    sr : TYPE
+        DESCRIPTION.
+    fmin : TYPE
+        DESCRIPTION.
+    hop_length : TYPE
+        DESCRIPTION.
+        
+    References
+    ----------
+    [1] Bittner, R. M., McFee, B., Salamon, J., Li, P., & Bello, J. P. (2017, October). 
+    Deep Salience Representations for F0 Estimation in Polyphonic Music. In ISMIR (pp. 63-70).
+
+    """
+    bins_per_octave = 60
+    n_octaves = 6
+    harmonics = [0.5, 1, 2, 3, 4, 5]
+    sr = 22050
+    fmin = 32.7
+    hop_length = 256
+    return bins_per_octave, n_octaves, harmonics, sr, fmin, hop_length
+
+
+def compute_hcqt_bittner(signal, sr):
+    """
+    Credit to Bittner & al. [1] (comes from https://github.com/rabitt/ismir2017-deepsalience).
+    
+    Computes HCQT representation of the signal, as presented in [1] (3-rd order tensor).
+
+    Parameters
+    ----------
+    signal : numpy array
+        Signal of the song.
+    sr : int
+        the sampling_rate
+
+    Returns
+    -------
+    log_hcqt : np array
+        The tensor of logarithm HCQT.
+        
+    References
+    ----------
+    [1] Bittner, R. M., McFee, B., Salamon, J., Li, P., & Bello, J. P. (2017, October). 
+    Deep Salience Representations for F0 Estimation in Polyphonic Music. In ISMIR (pp. 63-70).
+    """
+    (bins_per_octave, n_octaves, harmonics,
+     sr, f_min, hop_length) = get_hcqt_params()
+    #y, fs = librosa.load(audio_fpath, sr=sr)
+
+    cqt_list = []
+    shapes = []
+    for h in harmonics:
+        cqt = librosa.cqt(
+            signal, sr=sr, hop_length=hop_length, fmin=f_min*float(h),
+            n_bins=bins_per_octave*n_octaves,
+            bins_per_octave=bins_per_octave
+        )
+        cqt_list.append(cqt)
+        shapes.append(cqt.shape)
+
+    shapes_equal = [s == shapes[0] for s in shapes]
+    if not all(shapes_equal):
+        min_time = np.min([s[1] for s in shapes])
+        new_cqt_list = []
+        for i in range(len(cqt_list)):
+            new_cqt_list.append(cqt_list[i][:, :min_time])
+        cqt_list = new_cqt_list
+
+    log_hcqt = ((1.0/80.0) * librosa.core.amplitude_to_db(
+        np.abs(np.array(cqt_list)), ref=np.max)) + 1.0
+
+    return log_hcqt
+
+def my_compute_hcqt(signal, sr):
+    """
+    Credit to Bittner & al. [1] (comes from https://github.com/rabitt/ismir2017-deepsalience).
+    
+    Computes HCQT representation of the signal, as presented in [1] (3-rd order tensor).
+    The order of the mode is changed though, so tht first two modes correspond to frequency and time respectively,
+    and that the third corresponds to harmonic content.
+
+    Parameters
+    ----------
+    signal : numpy array
+        Signal of the song.
+    sr : int
+        the sampling_rate
+
+    Returns
+    -------
+    log_hcqt : np array
+        The tensor of logarithm HCQT.
+        
+    References
+    ----------
+    [1] Bittner, R. M., McFee, B., Salamon, J., Li, P., & Bello, J. P. (2017, October). 
+    Deep Salience Representations for F0 Estimation in Polyphonic Music. In ISMIR (pp. 63-70).
+    """
+    (bins_per_octave, n_octaves, harmonics, sr, f_min, hop_length) = get_hcqt_params()
+
+    freq_mode_len = bins_per_octave*n_octaves
+
+    first_cqt = librosa.cqt(signal, sr=sr, hop_length=hop_length, fmin=f_min*float(harmonics[0]),
+                            n_bins=freq_mode_len, bins_per_octave=bins_per_octave)
+
+    time_mode_len = first_cqt.shape[1]
+    
+    h_cqt = np.array(first_cqt).reshape(freq_mode_len, time_mode_len, 1)
+    
+    for h in harmonics[1:]:
+        cqt = librosa.cqt(signal, sr=sr, hop_length=hop_length, fmin=f_min*float(h),
+            n_bins=bins_per_octave*n_octaves,bins_per_octave=bins_per_octave)
+        current_cqt = cqt.reshape(freq_mode_len, time_mode_len, 1)
+        h_cqt = np.append(h_cqt, current_cqt, axis = 2)
+
+    log_hcqt = ((1.0/80.0) * librosa.core.amplitude_to_db(np.abs(h_cqt), ref=np.max)) + 1.0
+
+    return log_hcqt
+
```

### Comparing `barmuscomp-0.1.4/barmuscomp/model/plot_comparison_ae_ntd.py` & `barmuscomp-0.1.5/barmuscomp/model/plot_comparison_ae_ntd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Jul 26 15:37:15 2022
-
-@author: amarmore
-
-Plotting functions used for comparing NTD and AE-NTD outputs.
-Ugly code.
-"""
-import as_seg.autosimilarity_computation as as_comp
-from barmuscomp.model.current_plot import *
-import barmuscomp.model.pattern_study as ps
-
-import numpy as np
-import pandas as pd
-
-def plot_audio_diff_ntd_ae_in_dataframe(signal_ntd, signal_ae):
-    """
-    Listening to both audio examples (comparing NTD and AE-NTD).
-    """
-    df = pd.DataFrame(np.array([signal_ntd, signal_ae]), index = ["Audio NTD", "Audio AE"])
-    for i in range(df.shape[1]):
-        df[i] = df[i].T.apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
-    df_html = df.T.to_html(escape=False, index=False)
-    ipd.display(ipd.HTML(df_html))
-    
-def plot_spec_ntd_ae(spec_1, spec_2, title, to_permute = True, plot_diff = False):
-    """
-    Plotting both NTD and AE-NTD Q matrix.
-    """
-    if spec_1.shape[0] == spec_1.shape[1]:
-        fig, axs = plt.subplots(1, 2, figsize=(14,7))
-    else:
-        fig, axs = plt.subplots(1, 2, figsize=(15,min(5, 15*spec_1.shape[0]/spec_1.shape[1])))
-    if to_permute:
-        permut_1 = permutate_factor(spec_1.T) 
-        spec_1 = spec_1[permut_1]
-        permut_2 = permutate_factor(spec_2.T)
-        spec_2 = spec_2[permut_2]
-    diff = spec_2 - spec_1
-    axs[0].pcolormesh(np.arange(spec_1.shape[1]), np.arange(spec_1.shape[0]), spec_1, cmap=cm.Greys, shading='auto')
-    axs[0].set_title(f"{title} of NTD")
-    axs[1].pcolormesh(np.arange(spec_2.shape[1]), np.arange(spec_2.shape[0]), spec_2, cmap=cm.Greys, shading='auto')
-    axs[1].set_title(f"{title} of AE")
-    axs[0].invert_yaxis()
-    axs[1].invert_yaxis()
-    plt.show()
-    if plot_diff:
-        if spec_1.shape[0] == spec_1.shape[1]:
-            fig, axs = plt.subplots(1, 2, figsize=(14,7))
-        else:
-            fig, axs = plt.subplots(1, 2, figsize=(15,min(5, 15*spec_1.shape[0]/spec_1.shape[1])))
-        axs[0].pcolormesh(np.arange(diff.shape[1]), np.arange(diff.shape[0]), diff, cmap=cm.Greys, shading='auto')
-        axs[0].set_title(f"Diff entre les 2 spectrogrammes\n (couleurs normalisées entre min et max)\n Diff maximale: {np.amax(np.abs(diff))}")
-        the_max = max(np.amax(spec_1), np.amax(spec_2))
-        axs[1].pcolormesh(np.arange(diff.shape[1]), np.arange(diff.shape[0]), diff, cmap=cm.Greys, vmin=0, vmax=the_max, shading='auto')
-        axs[1].set_title(f"Diff entre les 2 spectrogrammes\n (couleurs normalisées entre 0 et max des 2 spectrogrammes)\n Valeur max des 2 specs{the_max}")
-        axs[0].invert_yaxis()
-        axs[1].invert_yaxis()
-        plt.show()
-
-def plot_patterns_ae_and_ntd(spec_patterns_ntd, signal_patterns_ntd, core_ae, factors_ae, signal_patterns_ae, nb_patterns_to_show):
-    """
-    Compares the patterns of both NTD and AE-NTD.
-    """
-    for i in range(nb_patterns_to_show):
-        pattern = factors_ae[0]@core_ae[:,:,i]@factors_ae[1].T
-        plot_spec_ntd_ae(spec_patterns_ntd[i], pattern, title = f"{i}-th pattern in the decoder", to_permute = False)
-        plot_audio_diff_ntd_ae_in_dataframe(signal_patterns_ntd[i], signal_patterns_ae[i])
-        
-def plot_comparison_this_ae_ntd(ssae, projection, hop_length, factors_ntd, tensor_mag_original, tensor_phase_original, nb_bars, phase_retrieval_song, phase_retrieval_patterns,
-                                autosimilarity_type = "Cosine", plot_patterns = False, nb_patterns_to_show = 4, subdivision = 96, spec_patterns_ntd = None, signal_patterns_ntd = None):
-    """
-    Compares the overall outputs of both NTD and AE-NTD.
-    """    
-    autosimil = as_comp.switch_autosimilarity(projection, similarity_type = autosimilarity_type, normalise = True)
-    autosimil_ntd = as_comp.switch_autosimilarity(factors_ntd[2], similarity_type = autosimilarity_type, normalise = True)
-    plot_spec_ntd_ae(autosimil_ntd, autosimil, "Autosimilarity", to_permute = False)
-
-    W = ssae.get_W()
-    H = ssae.get_H()
-    G = ssae.get_G()
-    proj_np = np.array(projection)
-
-    plot_spec_ntd_ae(factors_ntd[0], W, title = "W matrix")
-    plot_spec_ntd_ae(factors_ntd[1].T, H.T, title = "H matrix")
-    plot_spec_ntd_ae(factors_ntd[2].T, proj_np.T, title = "Latent representations")
-    song_sdr, patterns_sdr, audio_patterns = ps.sdr_songscale_patternscale_encpasulation(G, [W, H, proj_np], hop_length, tensor_mag_original, tensor_phase_original,
-                                                                 nb_bars, phase_retrieval_song, phase_retrieval_patterns, subdivision = subdivision)
-    
-    print(f"SDR at the song scale: {song_sdr}")
-    print(f"SDR at the pattern scale: average = {np.mean(patterns_sdr)}, std = {np.std(patterns_sdr)}")
-
-    if plot_patterns:
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Jul 26 15:37:15 2022
+
+@author: amarmore
+
+Plotting functions used for comparing NTD and AE-NTD outputs.
+Ugly code.
+"""
+import as_seg.autosimilarity_computation as as_comp
+from barmuscomp.model.current_plot import *
+import barmuscomp.model.pattern_study as ps # TODO: update with last version, i.e. factorisation to signal and spectrogram to signal
+
+import numpy as np
+import pandas as pd
+
+def plot_audio_diff_ntd_ae_in_dataframe(signal_ntd, signal_ae):
+    """
+    Listening to both audio examples (comparing NTD and AE-NTD).
+    """
+    df = pd.DataFrame(np.array([signal_ntd, signal_ae]), index = ["Audio NTD", "Audio AE"])
+    for i in range(df.shape[1]):
+        df[i] = df[i].T.apply(lambda x:x._repr_html_().replace('\n', '').strip())#, axis=1)
+    df_html = df.T.to_html(escape=False, index=False)
+    ipd.display(ipd.HTML(df_html))
+    
+def plot_spec_ntd_ae(spec_1, spec_2, title, to_permute = True, plot_diff = False):
+    """
+    Plotting both NTD and AE-NTD Q matrix.
+    """
+    if spec_1.shape[0] == spec_1.shape[1]:
+        fig, axs = plt.subplots(1, 2, figsize=(14,7))
+    else:
+        fig, axs = plt.subplots(1, 2, figsize=(15,min(5, 15*spec_1.shape[0]/spec_1.shape[1])))
+    if to_permute:
+        permut_1 = permutate_factor(spec_1.T) 
+        spec_1 = spec_1[permut_1]
+        permut_2 = permutate_factor(spec_2.T)
+        spec_2 = spec_2[permut_2]
+    diff = spec_2 - spec_1
+    axs[0].pcolormesh(np.arange(spec_1.shape[1]), np.arange(spec_1.shape[0]), spec_1, cmap=cm.Greys, shading='auto')
+    axs[0].set_title(f"{title} of NTD")
+    axs[1].pcolormesh(np.arange(spec_2.shape[1]), np.arange(spec_2.shape[0]), spec_2, cmap=cm.Greys, shading='auto')
+    axs[1].set_title(f"{title} of AE")
+    axs[0].invert_yaxis()
+    axs[1].invert_yaxis()
+    plt.show()
+    if plot_diff:
+        if spec_1.shape[0] == spec_1.shape[1]:
+            fig, axs = plt.subplots(1, 2, figsize=(14,7))
+        else:
+            fig, axs = plt.subplots(1, 2, figsize=(15,min(5, 15*spec_1.shape[0]/spec_1.shape[1])))
+        axs[0].pcolormesh(np.arange(diff.shape[1]), np.arange(diff.shape[0]), diff, cmap=cm.Greys, shading='auto')
+        axs[0].set_title(f"Diff entre les 2 spectrogrammes\n (couleurs normalisées entre min et max)\n Diff maximale: {np.amax(np.abs(diff))}")
+        the_max = max(np.amax(spec_1), np.amax(spec_2))
+        axs[1].pcolormesh(np.arange(diff.shape[1]), np.arange(diff.shape[0]), diff, cmap=cm.Greys, vmin=0, vmax=the_max, shading='auto')
+        axs[1].set_title(f"Diff entre les 2 spectrogrammes\n (couleurs normalisées entre 0 et max des 2 spectrogrammes)\n Valeur max des 2 specs{the_max}")
+        axs[0].invert_yaxis()
+        axs[1].invert_yaxis()
+        plt.show()
+
+def plot_patterns_ae_and_ntd(spec_patterns_ntd, signal_patterns_ntd, core_ae, factors_ae, signal_patterns_ae, nb_patterns_to_show):
+    """
+    Compares the patterns of both NTD and AE-NTD.
+    """
+    for i in range(nb_patterns_to_show):
+        pattern = factors_ae[0]@core_ae[:,:,i]@factors_ae[1].T
+        plot_spec_ntd_ae(spec_patterns_ntd[i], pattern, title = f"{i}-th pattern in the decoder", to_permute = False)
+        plot_audio_diff_ntd_ae_in_dataframe(signal_patterns_ntd[i], signal_patterns_ae[i])
+        
+def plot_comparison_this_ae_ntd(ssae, projection, hop_length, factors_ntd, tensor_mag_original, tensor_phase_original, nb_bars, phase_retrieval_song, phase_retrieval_patterns,
+                                autosimilarity_type = "Cosine", plot_patterns = False, nb_patterns_to_show = 4, subdivision = 96, spec_patterns_ntd = None, signal_patterns_ntd = None):
+    """
+    Compares the overall outputs of both NTD and AE-NTD.
+    """    
+    autosimil = as_comp.switch_autosimilarity(projection, similarity_type = autosimilarity_type, normalise = True)
+    autosimil_ntd = as_comp.switch_autosimilarity(factors_ntd[2], similarity_type = autosimilarity_type, normalise = True)
+    plot_spec_ntd_ae(autosimil_ntd, autosimil, "Autosimilarity", to_permute = False)
+
+    W = ssae.get_W()
+    H = ssae.get_H()
+    G = ssae.get_G()
+    proj_np = np.array(projection)
+
+    plot_spec_ntd_ae(factors_ntd[0], W, title = "W matrix")
+    plot_spec_ntd_ae(factors_ntd[1].T, H.T, title = "H matrix")
+    plot_spec_ntd_ae(factors_ntd[2].T, proj_np.T, title = "Latent representations")
+    song_sdr, patterns_sdr, audio_patterns = ps.sdr_songscale_patternscale_encpasulation(G, [W, H, proj_np], hop_length, tensor_mag_original, tensor_phase_original,
+                                                                 nb_bars, phase_retrieval_song, phase_retrieval_patterns, subdivision = subdivision)
+    
+    print(f"SDR at the song scale: {song_sdr}")
+    print(f"SDR at the pattern scale: average = {np.mean(patterns_sdr)}, std = {np.std(patterns_sdr)}")
+
+    if plot_patterns:
         plot_patterns_ae_and_ntd(spec_patterns_ntd, signal_patterns_ntd, G, [W, H, proj_np], signal_patterns_ae = audio_patterns, nb_patterns_to_show = nb_patterns_to_show)
```

### Comparing `barmuscomp-0.1.4/barmuscomp/scripts/default_path.py` & `barmuscomp-0.1.5/barmuscomp/scripts/default_path.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.4/barmuscomp/scripts/overall_scripts.py` & `barmuscomp-0.1.5/barmuscomp/scripts/overall_scripts.py`

 * *Files identical despite different names*

### Comparing `barmuscomp-0.1.4/barmuscomp.egg-info/PKG-INFO` & `barmuscomp-0.1.5/barmuscomp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barmuscomp
-Version: 0.1.4
+Version: 0.1.5
 Summary: Package for barwise compression applied on musical segmentation.
 Home-page: https://gitlab.inria.fr/amarmore/barmuscomp
 Author: Marmoret Axel
 Author-email: axel.marmoret@irisa.fr
 License: BSD
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `barmuscomp-0.1.4/barmuscomp.egg-info/SOURCES.txt` & `barmuscomp-0.1.5/barmuscomp.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 barmuscomp/lra.py
 barmuscomp.egg-info/PKG-INFO
 barmuscomp.egg-info/SOURCES.txt
 barmuscomp.egg-info/dependency_links.txt
 barmuscomp.egg-info/requires.txt
 barmuscomp.egg-info/top_level.txt
 barmuscomp/model/__init__.py
+barmuscomp/model/audio_helper.py
 barmuscomp/model/current_plot.py
 barmuscomp/model/early_stopping.py
 barmuscomp/model/errors.py
-barmuscomp/model/features.py
-barmuscomp/model/pattern_study.py
+barmuscomp/model/factorisation_to_signal.py
 barmuscomp/model/plot_comparison_ae_ntd.py
+barmuscomp/model/signal_to_spectrogram.py
+barmuscomp/model/spectrogram_to_signal.py
 barmuscomp/scripts/__init__.py
 barmuscomp/scripts/default_path.py
 barmuscomp/scripts/overall_scripts.py
```

### Comparing `barmuscomp-0.1.4/setup.py` & `barmuscomp-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="barmuscomp",
-    version="0.1.4",
+    version="0.1.5",
     author="Marmoret Axel",
     author_email="axel.marmoret@irisa.fr",
     description="Package for barwise compression applied on musical segmentation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.inria.fr/amarmore/barmuscomp",
     packages=setuptools.find_packages(),
```

