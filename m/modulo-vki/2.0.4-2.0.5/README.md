# Comparing `tmp/modulo_vki-2.0.4.tar.gz` & `tmp/modulo_vki-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modulo_vki-2.0.4.tar", last modified: Wed Apr 17 14:33:57 2024, max compression
+gzip compressed data, was "modulo_vki-2.0.5.tar", last modified: Mon May  6 15:43:48 2024, max compression
```

## Comparing `modulo_vki-2.0.4.tar` & `modulo_vki-2.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 lorenzoschena   (501) staff       (20)        0 2024-04-17 14:33:57.143076 modulo_vki-2.0.4/
--rw-r--r--   0 lorenzoschena   (501) staff       (20)     1070 2024-04-17 11:38:06.000000 modulo_vki-2.0.4/LICENSE
--rw-r--r--   0 lorenzoschena   (501) staff       (20)    10527 2024-04-17 14:33:57.142702 modulo_vki-2.0.4/PKG-INFO
--rwxr-xr-x   0 lorenzoschena   (501) staff       (20)     9669 2024-04-17 11:38:06.000000 modulo_vki-2.0.4/README.md
-drwxr-xr-x   0 lorenzoschena   (501) staff       (20)        0 2024-04-17 14:33:57.136461 modulo_vki-2.0.4/modulo_vki/
--rw-r--r--   0 lorenzoschena   (501) staff       (20)      572 2024-04-17 13:31:46.000000 modulo_vki-2.0.4/modulo_vki/__init__.py
-drwxr-xr-x   0 lorenzoschena   (501) staff       (20)        0 2024-04-17 14:33:57.139579 modulo_vki-2.0.4/modulo_vki/core/
--rw-r--r--   0 lorenzoschena   (501) staff       (20)      217 2024-04-17 13:29:28.000000 modulo_vki-2.0.4/modulo_vki/core/__init__.py
--rw-r--r--   0 lorenzoschena   (501) staff       (20)     2224 2024-04-17 13:29:28.000000 modulo_vki-2.0.4/modulo_vki/core/_dft.py
--rw-r--r--   0 lorenzoschena   (501) staff       (20)     2606 2024-04-17 13:29:28.000000 modulo_vki-2.0.4/modulo_vki/core/_dmd_s.py
--rw-r--r--   0 lorenzoschena   (501) staff       (20)     3606 2024-04-17 14:07:44.000000 modulo_vki-2.0.4/modulo_vki/core/_k_matrix.py
--rw-r--r--   0 lorenzoschena   (501) staff       (20)     7147 2024-04-17 13:29:28.000000 modulo_vki-2.0.4/modulo_vki/core/_mpod_space.py
--rw-r--r--   0 lorenzoschena   (501) staff       (20)     8344 2024-04-17 13:31:45.000000 modulo_vki-2.0.4/modulo_vki/core/_mpod_time.py
--rw-r--r--   0 lorenzoschena   (501) staff       (20)     6769 2024-04-17 13:29:28.000000 modulo_vki-2.0.4/modulo_vki/core/_pod_space.py
--rw-r--r--   0 lorenzoschena   (501) staff       (20)     2096 2024-04-17 13:29:28.000000 modulo_vki-2.0.4/modulo_vki/core/_pod_time.py
--rw-r--r--   0 lorenzoschena   (501) staff       (20)     4048 2024-04-17 13:29:28.000000 modulo_vki-2.0.4/modulo_vki/core/_spod_s.py
--rw-r--r--   0 lorenzoschena   (501) staff       (20)     3762 2024-04-17 13:31:48.000000 modulo_vki-2.0.4/modulo_vki/core/_spod_t.py
--rw-r--r--   0 lorenzoschena   (501) staff       (20)    36893 2024-04-17 14:07:44.000000 modulo_vki-2.0.4/modulo_vki/modulo.py
-drwxr-xr-x   0 lorenzoschena   (501) staff       (20)        0 2024-04-17 14:33:57.141859 modulo_vki-2.0.4/modulo_vki/utils/
--rw-r--r--   0 lorenzoschena   (501) staff       (20)       90 2024-04-17 13:29:28.000000 modulo_vki-2.0.4/modulo_vki/utils/__init__.py
--rw-r--r--   0 lorenzoschena   (501) staff       (20)     1402 2024-04-17 13:29:28.000000 modulo_vki-2.0.4/modulo_vki/utils/_plots.py
--rw-r--r--   0 lorenzoschena   (501) staff       (20)    13499 2024-04-17 13:29:28.000000 modulo_vki-2.0.4/modulo_vki/utils/_utils.py
--rw-r--r--   0 lorenzoschena   (501) staff       (20)    16513 2024-04-17 13:29:28.000000 modulo_vki-2.0.4/modulo_vki/utils/others.py
--rw-r--r--   0 lorenzoschena   (501) staff       (20)    14778 2024-04-17 13:29:28.000000 modulo_vki-2.0.4/modulo_vki/utils/read_db.py
-drwxr-xr-x   0 lorenzoschena   (501) staff       (20)        0 2024-04-17 14:33:57.142161 modulo_vki-2.0.4/modulo_vki.egg-info/
--rw-r--r--   0 lorenzoschena   (501) staff       (20)    10527 2024-04-17 14:33:57.000000 modulo_vki-2.0.4/modulo_vki.egg-info/PKG-INFO
--rw-r--r--   0 lorenzoschena   (501) staff       (20)      658 2024-04-17 14:33:57.000000 modulo_vki-2.0.4/modulo_vki.egg-info/SOURCES.txt
--rw-r--r--   0 lorenzoschena   (501) staff       (20)        1 2024-04-17 14:33:57.000000 modulo_vki-2.0.4/modulo_vki.egg-info/dependency_links.txt
--rw-r--r--   0 lorenzoschena   (501) staff       (20)       87 2024-04-17 14:33:57.000000 modulo_vki-2.0.4/modulo_vki.egg-info/requires.txt
--rw-r--r--   0 lorenzoschena   (501) staff       (20)       11 2024-04-17 14:33:57.000000 modulo_vki-2.0.4/modulo_vki.egg-info/top_level.txt
--rw-r--r--   0 lorenzoschena   (501) staff       (20)       38 2024-04-17 14:33:57.143149 modulo_vki-2.0.4/setup.cfg
--rw-r--r--   0 lorenzoschena   (501) staff       (20)     2605 2024-04-17 14:18:37.000000 modulo_vki-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:43:48.425689 modulo_vki-2.0.5/
+-rw-rw-rw-   0        0        0     1091 2024-05-06 15:37:25.000000 modulo_vki-2.0.5/LICENSE
+-rw-rw-rw-   0        0        0    10623 2024-05-06 15:43:48.423988 modulo_vki-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9741 2024-05-06 15:37:25.000000 modulo_vki-2.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 15:43:48.366328 modulo_vki-2.0.5/modulo_vki/
+-rw-rw-rw-   0        0        0      594 2024-05-06 15:37:26.000000 modulo_vki-2.0.5/modulo_vki/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:43:48.406223 modulo_vki-2.0.5/modulo_vki/core/
+-rw-rw-rw-   0        0        0      226 2024-05-06 15:37:26.000000 modulo_vki-2.0.5/modulo_vki/core/__init__.py
+-rw-rw-rw-   0        0        0     2285 2024-05-06 15:37:26.000000 modulo_vki-2.0.5/modulo_vki/core/_dft.py
+-rw-rw-rw-   0        0        0     2678 2024-05-06 15:37:26.000000 modulo_vki-2.0.5/modulo_vki/core/_dmd_s.py
+-rw-rw-rw-   0        0        0     3687 2024-05-06 15:37:26.000000 modulo_vki-2.0.5/modulo_vki/core/_k_matrix.py
+-rw-rw-rw-   0        0        0     7327 2024-05-06 15:37:26.000000 modulo_vki-2.0.5/modulo_vki/core/_mpod_space.py
+-rw-rw-rw-   0        0        0     8498 2024-05-06 15:37:26.000000 modulo_vki-2.0.5/modulo_vki/core/_mpod_time.py
+-rw-rw-rw-   0        0        0     6933 2024-05-06 15:37:26.000000 modulo_vki-2.0.5/modulo_vki/core/_pod_space.py
+-rw-rw-rw-   0        0        0     2144 2024-05-06 15:37:26.000000 modulo_vki-2.0.5/modulo_vki/core/_pod_time.py
+-rw-rw-rw-   0        0        0     4149 2024-05-06 15:37:26.000000 modulo_vki-2.0.5/modulo_vki/core/_spod_s.py
+-rw-rw-rw-   0        0        0     3866 2024-05-06 15:37:26.000000 modulo_vki-2.0.5/modulo_vki/core/_spod_t.py
+-rw-rw-rw-   0        0        0    37654 2024-05-06 15:37:26.000000 modulo_vki-2.0.5/modulo_vki/modulo.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:43:48.421019 modulo_vki-2.0.5/modulo_vki/utils/
+-rw-rw-rw-   0        0        0       94 2024-05-06 15:37:26.000000 modulo_vki-2.0.5/modulo_vki/utils/__init__.py
+-rw-rw-rw-   0        0        0     1453 2024-05-06 15:37:26.000000 modulo_vki-2.0.5/modulo_vki/utils/_plots.py
+-rw-rw-rw-   0        0        0    13838 2024-05-06 15:37:26.000000 modulo_vki-2.0.5/modulo_vki/utils/_utils.py
+-rw-rw-rw-   0        0        0    16962 2024-05-06 15:37:26.000000 modulo_vki-2.0.5/modulo_vki/utils/others.py
+-rw-rw-rw-   0        0        0    15117 2024-05-06 15:37:26.000000 modulo_vki-2.0.5/modulo_vki/utils/read_db.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:43:48.423016 modulo_vki-2.0.5/modulo_vki.egg-info/
+-rw-rw-rw-   0        0        0    10623 2024-05-06 15:43:48.000000 modulo_vki-2.0.5/modulo_vki.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      658 2024-05-06 15:43:48.000000 modulo_vki-2.0.5/modulo_vki.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 15:43:48.000000 modulo_vki-2.0.5/modulo_vki.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2024-05-06 15:43:48.000000 modulo_vki-2.0.5/modulo_vki.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-06 15:43:48.000000 modulo_vki-2.0.5/modulo_vki.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 15:43:48.425689 modulo_vki-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2687 2024-05-06 15:43:18.000000 modulo_vki-2.0.5/setup.py
```

### Comparing `modulo_vki-2.0.4/PKG-INFO` & `modulo_vki-2.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-Metadata-Version: 2.1
-Name: modulo_vki
-Version: 2.0.4
-Summary: MODULO (MODal mULtiscale pOd) is a software developed at the von Karman Institute to perform Multiscale Modal Analysis of numerical and experimental data.
-Home-page: https://github.com/mendezVKI/MODULO/tree/master/modulo_python_package/
-Author: ['R. Poletti', 'L. Schena', 'D. Ninni', 'M. A. Mendez']
-Author-email: mendez@vki.ac.be
-License: BSD (3-clause)
-Classifier: Development Status :: 4 - Beta
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: tqdm
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: scikit-learn
-Requires-Dist: ipykernel
-Requires-Dist: ipython
-Requires-Dist: ipython-genutils
-Requires-Dist: ipywidgets
-Requires-Dist: matplotlib
-
-
-
-MODULO - latest update 2.0
-===================
-
-This repository contains version 2.0 of MODULO (MODal mULtiscale pOd), a software developed at the von Karman Institute to perform data-driven modal decompositions and, in particular, the Multiscale Proper Orthogonal Decomposition (mPOD).
-
-The old version based on MATLAB implementation and related GUI is no longer maintained but will remain available on the branch "Old_Matlab_Implementation". We also keep the first Python implementation in the branch "Old_Python_Implementation". See the Readme file in these branches for more information.
-
-#### Documentation
-
-The full documentation is available at https://modulo.readthedocs.io/en/latest/intro.html.
-This documentation is stored alongside the source code and linked to a specific version of MODULO.
-
-## What is MODULO, and what are data-driven decompositions?
-
-MODULO allows to compute data-driven decompositions of experimental and numerical data. To have a concise overview of the context, we refer to: 
-
-- Ninni, D., Mendez, M. A. (2020), "MODULO: A Software for Multiscale Proper Orthogonal Decomposition of data", Software X, Vol 12, 100622, https://doi.org/10.1016/j.softx.2020.100622.
-
-- Poletti, R., Schena, L., Ninni, D., Mendez, M.A (2024) "MODULO: a python toolbox for data-driven modal decomposition", Submitted to Journal of Open Source Software. Preprint available [here](https://www.researchgate.net/publication/376885484_MODULO_a_python_toolbox_for_data-driven_modal_decomposition)
-
-The first article also presents the first version of MODULO (available in the OLD_Matlab_Implementation branch) and its GUI developed by D. Ninni. The second introduces MODULO v2 in this branch and alternative open source projects. While many projects allows for computing common decompositions such as POD, DMD and the SPODs, MODULO is currently the only opensource project allowing to compute the mPOD.
-
-For a more comprehensive overview on the theory of data-driven decompositions, we refer to the chapter:
-
-- Mendez, M. A. (2023) "Generalized and Multiscale Modal Analysis". In : Mendez M.A., Ianiro, A., Noack, B.R., Brunton, S. L. (Eds), "Data-Driven Fluid Mechanics: Combining First Principles and Machine Learning". Cambridge University Press, 2023:153-181. https://doi.org/10.1017/9781108896214.013. The pre-print is available at https://arxiv.org/abs/2208.12630. 
-
-and the article that first presented the complete treatment of the mPOD :
-
-- Mendez, M. A., Balabane, M., Buchlin, J.-M. (2019) "Multi-Scale Proper Orthogonal Decomposition of Complex Fluid Flows" Journal of Fluid Mechanics 870:988-1036, https://doi.org/10.1017/9781108896214.013. The pre-print is available at https://arxiv.org/abs/2208.12630. 
-
-Ongoing works on nonlinear methods are discussed here:
-
-- Mendez, M. A. (2023) "Linear and Nonlinear Dimensionality Reduction from Fluid Mechanics to Machine Learning", Meas. Sci. Technol. 34(042001), https://doi.org/10.1088/1361-6501/acaffe. The pre-print is available at https://arxiv.org/abs/2208.07746.   
-
-## What is new in this V 2.0? 
-
-This version expands considerably the version v1 in "Old_Python_Implementation", for which a first tutorial was provided by L. Schena in https://www.youtube.com/watch?v=y2uSvdxAwHk. 
-The major updates are the following :
-
-1. Faster EIG/SVD algorithms, using powerful randomized svd solvers from scikit_learn (see [this](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.TruncatedSVD.html) and [this](https://scikit-learn.org/stable/modules/generated/sklearn.utils.extmath.randomized_svd.html) ). It is now possible to select various options as "eig_solver" and "svd_solver", offering different trade-offs in terms of accuracy vs computational time.
-
-2. In addition to the traditional POD computation using the K matrix (Sirovinch's method), it is now possible to compute the POD directly via SVD using any of the four "svd_solver" options.
-This is generally faster but requires more memory.
-
-3. Faster subscale estimators for the mPOD: the previous version used the rank of the correlation matrix in each scale to define the number of modes to be computed in each portion of the splitting vector before assembling the full basis. This is computationally very demanding. This estimation has been replaced by a frequency-based threshold (i.e. based on the frequency bins within each portion) since one can show that the frequency-based estimator is always more "conservative" than the rank-based estimator.
-
-4. Major improvement on the memory saving option: the previous version of modulo always required in input the matrix D. Then, if the memory saving option was active, the matrix was partitioned and stored locally to free the RAM before computing the correlation matrix (see [this tutorial by D. Ninni](https://www.youtube.com/watch?v=LclxO1WTuao)). In the new version, it is possible to initialize a modulo object *without* the matrix D (see exercise 5 in the examples). Instead, one can create the partitions without loading the matrix D.
-
-5. Implementation of Dynamic Mode Decomposition (DMD) from [Schmid, P.J 2010](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/dynamic-mode-decomposition-of-numerical-and-experimental-data/AA4C763B525515AD4521A6CC5E10DBD4).
-
-6. Implementation of the two Spectral POD formulations, namely the one from [Sieber et al 2016](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/abs/spectral-proper-orthogonal-decomposition/DCD8A6EDEFD56F5A9715DBAD38BD461A), and the one from [Towne et al 2018](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/abs/spectral-proper-orthogonal-decomposition-and-its-relationship-to-dynamic-mode-decomposition-and-resolvent-analysis/EC2A6DF76490A0B9EB208CC2CA037717)
-
-7. Implementation of a kernel version of the POD, in which the correlation matrix is replaced by a kernel matrix. This is described in Lecture 15 of the course [Hands on Machine Learning for Fluid dynamics 2023](https://www.vki.ac.be/index.php/events-ls/events/eventdetail/552/-/online-on-site-hands-on-machine-learning-for-fluid-dynamics-2023). See also [this](https://arxiv.org/abs/2208.07746).
-
-8. Implementation of a formulation for non-uniform meshes, using a weighted matrix for all the relevant inner products. This is currently available only for POD and mPOD but allows for handling data produced from CFD simulation without resampling on a uniform grid (see exercise 4). It can be used both with and without the memory-saving option.
-
-## New Tutorials 
-
-The installation provides five exercises to explore MODULO's features while familiarizing with data-driven decompositions. These are available in the /exercise/ folder in plain Python format and jupyter notebooks. 
-
-- Exercise 1. In this exercise, we consider the flow past a cylinder. The dataset was created via Large Eddy Simulations (LES) by Denis Dumoulin during his STP at VKI in 2016 (Report available on request). For convenience, the data was first mapped to a Cartesian grid. This test case is by far the most popular because it's well-known to have a simple low-order representation with modes that have nearly harmonic temporal structures. We compute the POD and the DMD and compare the results... the difference between DMD and POD modes is hardly distinguishable!
-
-- Exercise 2. We consider the flow of an impinging gas jet, taken from [this](https://arxiv.org/abs/1804.09646) paper. This dataset was collected via Time-Resolved Particle Image Velocimetry (TR-PIV). Only the first 200 POD modes were stored. This dataset has much richer dynamics than the previous one and cannot be easily approximated using a few modes. We use it to explore the differences between the DFT, the SPODs and the mPOD. These have different purposes and look for different features.
-
-- Exercise 3. We take back the cylinder test case to explore the differences between the POD and the generalized Karhunen–Loève (KL) expansion in which a kernel matrix replaces the correlation matrix. The POD is a particular case of KL where the kernel function generating the kernel matrix is the plain inner product. Here, we also consider a Gaussian kernel. Different kernel functions define similarity in different ways and thus produce widely different modes. Different modal structures tell different stories about the dataset, but... what can you say about efficiency in data compression? 
-
-- Exercise 4. We consider the flow past a cylinder again, but this time in transient conditions and on an experimental test case taken from [this](https://arxiv.org/abs/2001.01971) paper. In this exercise, you can reproduce the same results from the article to see how the mPOD allows to achieve both time and frequency localization without compromising much of the convergence of the POD. The dataset is quite large, so you might have difficulties handling it if you have less than 32 GB of RAM. But fear not: the memory saving feature allows to compute POD and mPOD without loading the data into memory!
-
-- Exercise 5. We consider the flow of an impinging gas jet again, but this time on a numerical test case. This dataset was produced by Yannic Lowenstein during his STP at VKI at the end of 2023, with the help of Dr. Maria Faruoli. The Reynolds number is two orders of magnitude higher than in exercise 2, yet the flow features you will observe are pretty similar, at least qualitatively. From a learning perspective, the key feature of this test case is that the data is not available on a uniform grid. But fear not: with the new features, it is possible to compute the decompositions using appropriate weights!
- 
+Metadata-Version: 2.1
+Name: modulo_vki
+Version: 2.0.5
+Summary: MODULO (MODal mULtiscale pOd) is a software developed at the von Karman Institute to perform Multiscale Modal Analysis of numerical and experimental data.
+Home-page: https://github.com/mendezVKI/MODULO/tree/master/modulo_python_package/
+Author: ['R. Poletti', 'L. Schena', 'D. Ninni', 'M. A. Mendez']
+Author-email: mendez@vki.ac.be
+License: BSD (3-clause)
+Classifier: Development Status :: 4 - Beta
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: tqdm
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+Requires-Dist: ipykernel
+Requires-Dist: ipython
+Requires-Dist: ipython-genutils
+Requires-Dist: ipywidgets
+Requires-Dist: matplotlib
+
+
+
+MODULO - latest update 2.0
+===================
+
+This repository contains version 2.0 of MODULO (MODal mULtiscale pOd), a software developed at the von Karman Institute to perform data-driven modal decompositions and, in particular, the Multiscale Proper Orthogonal Decomposition (mPOD).
+
+The old version based on MATLAB implementation and related GUI is no longer maintained but will remain available on the branch "Old_Matlab_Implementation". We also keep the first Python implementation in the branch "Old_Python_Implementation". See the Readme file in these branches for more information.
+
+#### Documentation
+
+The full documentation is available at https://modulo.readthedocs.io/en/latest/intro.html.
+This documentation is stored alongside the source code and linked to a specific version of MODULO.
+
+## What is MODULO, and what are data-driven decompositions?
+
+MODULO allows to compute data-driven decompositions of experimental and numerical data. To have a concise overview of the context, we refer to: 
+
+- Ninni, D., Mendez, M. A. (2020), "MODULO: A Software for Multiscale Proper Orthogonal Decomposition of data", Software X, Vol 12, 100622, https://doi.org/10.1016/j.softx.2020.100622.
+
+- Poletti, R., Schena, L., Ninni, D., Mendez, M.A (2024) "MODULO: a python toolbox for data-driven modal decomposition", Submitted to Journal of Open Source Software. Preprint available [here](https://www.researchgate.net/publication/376885484_MODULO_a_python_toolbox_for_data-driven_modal_decomposition)
+
+The first article also presents the first version of MODULO (available in the OLD_Matlab_Implementation branch) and its GUI developed by D. Ninni. The second introduces MODULO v2 in this branch and alternative open source projects. While many projects allows for computing common decompositions such as POD, DMD and the SPODs, MODULO is currently the only opensource project allowing to compute the mPOD.
+
+For a more comprehensive overview on the theory of data-driven decompositions, we refer to the chapter:
+
+- Mendez, M. A. (2023) "Generalized and Multiscale Modal Analysis". In : Mendez M.A., Ianiro, A., Noack, B.R., Brunton, S. L. (Eds), "Data-Driven Fluid Mechanics: Combining First Principles and Machine Learning". Cambridge University Press, 2023:153-181. https://doi.org/10.1017/9781108896214.013. The pre-print is available at https://arxiv.org/abs/2208.12630. 
+
+and the article that first presented the complete treatment of the mPOD :
+
+- Mendez, M. A., Balabane, M., Buchlin, J.-M. (2019) "Multi-Scale Proper Orthogonal Decomposition of Complex Fluid Flows" Journal of Fluid Mechanics 870:988-1036, https://doi.org/10.1017/9781108896214.013. The pre-print is available at https://arxiv.org/abs/2208.12630. 
+
+Ongoing works on nonlinear methods are discussed here:
+
+- Mendez, M. A. (2023) "Linear and Nonlinear Dimensionality Reduction from Fluid Mechanics to Machine Learning", Meas. Sci. Technol. 34(042001), https://doi.org/10.1088/1361-6501/acaffe. The pre-print is available at https://arxiv.org/abs/2208.07746.   
+
+## What is new in this V 2.0? 
+
+This version expands considerably the version v1 in "Old_Python_Implementation", for which a first tutorial was provided by L. Schena in https://www.youtube.com/watch?v=y2uSvdxAwHk. 
+The major updates are the following :
+
+1. Faster EIG/SVD algorithms, using powerful randomized svd solvers from scikit_learn (see [this](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.TruncatedSVD.html) and [this](https://scikit-learn.org/stable/modules/generated/sklearn.utils.extmath.randomized_svd.html) ). It is now possible to select various options as "eig_solver" and "svd_solver", offering different trade-offs in terms of accuracy vs computational time.
+
+2. In addition to the traditional POD computation using the K matrix (Sirovinch's method), it is now possible to compute the POD directly via SVD using any of the four "svd_solver" options.
+This is generally faster but requires more memory.
+
+3. Faster subscale estimators for the mPOD: the previous version used the rank of the correlation matrix in each scale to define the number of modes to be computed in each portion of the splitting vector before assembling the full basis. This is computationally very demanding. This estimation has been replaced by a frequency-based threshold (i.e. based on the frequency bins within each portion) since one can show that the frequency-based estimator is always more "conservative" than the rank-based estimator.
+
+4. Major improvement on the memory saving option: the previous version of modulo always required in input the matrix D. Then, if the memory saving option was active, the matrix was partitioned and stored locally to free the RAM before computing the correlation matrix (see [this tutorial by D. Ninni](https://www.youtube.com/watch?v=LclxO1WTuao)). In the new version, it is possible to initialize a modulo object *without* the matrix D (see exercise 5 in the examples). Instead, one can create the partitions without loading the matrix D.
+
+5. Implementation of Dynamic Mode Decomposition (DMD) from [Schmid, P.J 2010](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/dynamic-mode-decomposition-of-numerical-and-experimental-data/AA4C763B525515AD4521A6CC5E10DBD4).
+
+6. Implementation of the two Spectral POD formulations, namely the one from [Sieber et al 2016](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/abs/spectral-proper-orthogonal-decomposition/DCD8A6EDEFD56F5A9715DBAD38BD461A), and the one from [Towne et al 2018](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/abs/spectral-proper-orthogonal-decomposition-and-its-relationship-to-dynamic-mode-decomposition-and-resolvent-analysis/EC2A6DF76490A0B9EB208CC2CA037717)
+
+7. Implementation of a kernel version of the POD, in which the correlation matrix is replaced by a kernel matrix. This is described in Lecture 15 of the course [Hands on Machine Learning for Fluid dynamics 2023](https://www.vki.ac.be/index.php/events-ls/events/eventdetail/552/-/online-on-site-hands-on-machine-learning-for-fluid-dynamics-2023). See also [this](https://arxiv.org/abs/2208.07746).
+
+8. Implementation of a formulation for non-uniform meshes, using a weighted matrix for all the relevant inner products. This is currently available only for POD and mPOD but allows for handling data produced from CFD simulation without resampling on a uniform grid (see exercise 4). It can be used both with and without the memory-saving option.
+
+## New Tutorials 
+
+The installation provides five exercises to explore MODULO's features while familiarizing with data-driven decompositions. These are available in the /exercise/ folder in plain Python format and jupyter notebooks. 
+
+- Exercise 1. In this exercise, we consider the flow past a cylinder. The dataset was created via Large Eddy Simulations (LES) by Denis Dumoulin during his STP at VKI in 2016 (Report available on request). For convenience, the data was first mapped to a Cartesian grid. This test case is by far the most popular because it's well-known to have a simple low-order representation with modes that have nearly harmonic temporal structures. We compute the POD and the DMD and compare the results... the difference between DMD and POD modes is hardly distinguishable!
+
+- Exercise 2. We consider the flow of an impinging gas jet, taken from [this](https://arxiv.org/abs/1804.09646) paper. This dataset was collected via Time-Resolved Particle Image Velocimetry (TR-PIV). Only the first 200 POD modes were stored. This dataset has much richer dynamics than the previous one and cannot be easily approximated using a few modes. We use it to explore the differences between the DFT, the SPODs and the mPOD. These have different purposes and look for different features.
+
+- Exercise 3. We take back the cylinder test case to explore the differences between the POD and the generalized Karhunen–Loève (KL) expansion in which a kernel matrix replaces the correlation matrix. The POD is a particular case of KL where the kernel function generating the kernel matrix is the plain inner product. Here, we also consider a Gaussian kernel. Different kernel functions define similarity in different ways and thus produce widely different modes. Different modal structures tell different stories about the dataset, but... what can you say about efficiency in data compression? 
+
+- Exercise 4. We consider the flow past a cylinder again, but this time in transient conditions and on an experimental test case taken from [this](https://arxiv.org/abs/2001.01971) paper. In this exercise, you can reproduce the same results from the article to see how the mPOD allows to achieve both time and frequency localization without compromising much of the convergence of the POD. The dataset is quite large, so you might have difficulties handling it if you have less than 32 GB of RAM. But fear not: the memory saving feature allows to compute POD and mPOD without loading the data into memory!
+
+- Exercise 5. We consider the flow of an impinging gas jet again, but this time on a numerical test case. This dataset was produced by Yannic Lowenstein during his STP at VKI at the end of 2023, with the help of Dr. Maria Faruoli. The Reynolds number is two orders of magnitude higher than in exercise 2, yet the flow features you will observe are pretty similar, at least qualitatively. From a learning perspective, the key feature of this test case is that the data is not available on a uniform grid. But fear not: with the new features, it is possible to compute the decompositions using appropriate weights!
+
```

### Comparing `modulo_vki-2.0.4/README.md` & `modulo_vki-2.0.5/README.md`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-
-
-MODULO - latest update 2.0
-===================
-
-This repository contains version 2.0 of MODULO (MODal mULtiscale pOd), a software developed at the von Karman Institute to perform data-driven modal decompositions and, in particular, the Multiscale Proper Orthogonal Decomposition (mPOD).
-
-The old version based on MATLAB implementation and related GUI is no longer maintained but will remain available on the branch "Old_Matlab_Implementation". We also keep the first Python implementation in the branch "Old_Python_Implementation". See the Readme file in these branches for more information.
-
-#### Documentation
-
-The full documentation is available at https://modulo.readthedocs.io/en/latest/intro.html.
-This documentation is stored alongside the source code and linked to a specific version of MODULO.
-
-## What is MODULO, and what are data-driven decompositions?
-
-MODULO allows to compute data-driven decompositions of experimental and numerical data. To have a concise overview of the context, we refer to: 
-
-- Ninni, D., Mendez, M. A. (2020), "MODULO: A Software for Multiscale Proper Orthogonal Decomposition of data", Software X, Vol 12, 100622, https://doi.org/10.1016/j.softx.2020.100622.
-
-- Poletti, R., Schena, L., Ninni, D., Mendez, M.A (2024) "MODULO: a python toolbox for data-driven modal decomposition", Submitted to Journal of Open Source Software. Preprint available [here](https://www.researchgate.net/publication/376885484_MODULO_a_python_toolbox_for_data-driven_modal_decomposition)
-
-The first article also presents the first version of MODULO (available in the OLD_Matlab_Implementation branch) and its GUI developed by D. Ninni. The second introduces MODULO v2 in this branch and alternative open source projects. While many projects allows for computing common decompositions such as POD, DMD and the SPODs, MODULO is currently the only opensource project allowing to compute the mPOD.
-
-For a more comprehensive overview on the theory of data-driven decompositions, we refer to the chapter:
-
-- Mendez, M. A. (2023) "Generalized and Multiscale Modal Analysis". In : Mendez M.A., Ianiro, A., Noack, B.R., Brunton, S. L. (Eds), "Data-Driven Fluid Mechanics: Combining First Principles and Machine Learning". Cambridge University Press, 2023:153-181. https://doi.org/10.1017/9781108896214.013. The pre-print is available at https://arxiv.org/abs/2208.12630. 
-
-and the article that first presented the complete treatment of the mPOD :
-
-- Mendez, M. A., Balabane, M., Buchlin, J.-M. (2019) "Multi-Scale Proper Orthogonal Decomposition of Complex Fluid Flows" Journal of Fluid Mechanics 870:988-1036, https://doi.org/10.1017/9781108896214.013. The pre-print is available at https://arxiv.org/abs/2208.12630. 
-
-Ongoing works on nonlinear methods are discussed here:
-
-- Mendez, M. A. (2023) "Linear and Nonlinear Dimensionality Reduction from Fluid Mechanics to Machine Learning", Meas. Sci. Technol. 34(042001), https://doi.org/10.1088/1361-6501/acaffe. The pre-print is available at https://arxiv.org/abs/2208.07746.   
-
-## What is new in this V 2.0? 
-
-This version expands considerably the version v1 in "Old_Python_Implementation", for which a first tutorial was provided by L. Schena in https://www.youtube.com/watch?v=y2uSvdxAwHk. 
-The major updates are the following :
-
-1. Faster EIG/SVD algorithms, using powerful randomized svd solvers from scikit_learn (see [this](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.TruncatedSVD.html) and [this](https://scikit-learn.org/stable/modules/generated/sklearn.utils.extmath.randomized_svd.html) ). It is now possible to select various options as "eig_solver" and "svd_solver", offering different trade-offs in terms of accuracy vs computational time.
-
-2. In addition to the traditional POD computation using the K matrix (Sirovinch's method), it is now possible to compute the POD directly via SVD using any of the four "svd_solver" options.
-This is generally faster but requires more memory.
-
-3. Faster subscale estimators for the mPOD: the previous version used the rank of the correlation matrix in each scale to define the number of modes to be computed in each portion of the splitting vector before assembling the full basis. This is computationally very demanding. This estimation has been replaced by a frequency-based threshold (i.e. based on the frequency bins within each portion) since one can show that the frequency-based estimator is always more "conservative" than the rank-based estimator.
-
-4. Major improvement on the memory saving option: the previous version of modulo always required in input the matrix D. Then, if the memory saving option was active, the matrix was partitioned and stored locally to free the RAM before computing the correlation matrix (see [this tutorial by D. Ninni](https://www.youtube.com/watch?v=LclxO1WTuao)). In the new version, it is possible to initialize a modulo object *without* the matrix D (see exercise 5 in the examples). Instead, one can create the partitions without loading the matrix D.
-
-5. Implementation of Dynamic Mode Decomposition (DMD) from [Schmid, P.J 2010](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/dynamic-mode-decomposition-of-numerical-and-experimental-data/AA4C763B525515AD4521A6CC5E10DBD4).
-
-6. Implementation of the two Spectral POD formulations, namely the one from [Sieber et al 2016](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/abs/spectral-proper-orthogonal-decomposition/DCD8A6EDEFD56F5A9715DBAD38BD461A), and the one from [Towne et al 2018](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/abs/spectral-proper-orthogonal-decomposition-and-its-relationship-to-dynamic-mode-decomposition-and-resolvent-analysis/EC2A6DF76490A0B9EB208CC2CA037717)
-
-7. Implementation of a kernel version of the POD, in which the correlation matrix is replaced by a kernel matrix. This is described in Lecture 15 of the course [Hands on Machine Learning for Fluid dynamics 2023](https://www.vki.ac.be/index.php/events-ls/events/eventdetail/552/-/online-on-site-hands-on-machine-learning-for-fluid-dynamics-2023). See also [this](https://arxiv.org/abs/2208.07746).
-
-8. Implementation of a formulation for non-uniform meshes, using a weighted matrix for all the relevant inner products. This is currently available only for POD and mPOD but allows for handling data produced from CFD simulation without resampling on a uniform grid (see exercise 4). It can be used both with and without the memory-saving option.
-
-## New Tutorials 
-
-The installation provides five exercises to explore MODULO's features while familiarizing with data-driven decompositions. These are available in the /exercise/ folder in plain Python format and jupyter notebooks. 
-
-- Exercise 1. In this exercise, we consider the flow past a cylinder. The dataset was created via Large Eddy Simulations (LES) by Denis Dumoulin during his STP at VKI in 2016 (Report available on request). For convenience, the data was first mapped to a Cartesian grid. This test case is by far the most popular because it's well-known to have a simple low-order representation with modes that have nearly harmonic temporal structures. We compute the POD and the DMD and compare the results... the difference between DMD and POD modes is hardly distinguishable!
-
-- Exercise 2. We consider the flow of an impinging gas jet, taken from [this](https://arxiv.org/abs/1804.09646) paper. This dataset was collected via Time-Resolved Particle Image Velocimetry (TR-PIV). Only the first 200 POD modes were stored. This dataset has much richer dynamics than the previous one and cannot be easily approximated using a few modes. We use it to explore the differences between the DFT, the SPODs and the mPOD. These have different purposes and look for different features.
-
-- Exercise 3. We take back the cylinder test case to explore the differences between the POD and the generalized Karhunen–Loève (KL) expansion in which a kernel matrix replaces the correlation matrix. The POD is a particular case of KL where the kernel function generating the kernel matrix is the plain inner product. Here, we also consider a Gaussian kernel. Different kernel functions define similarity in different ways and thus produce widely different modes. Different modal structures tell different stories about the dataset, but... what can you say about efficiency in data compression? 
-
-- Exercise 4. We consider the flow past a cylinder again, but this time in transient conditions and on an experimental test case taken from [this](https://arxiv.org/abs/2001.01971) paper. In this exercise, you can reproduce the same results from the article to see how the mPOD allows to achieve both time and frequency localization without compromising much of the convergence of the POD. The dataset is quite large, so you might have difficulties handling it if you have less than 32 GB of RAM. But fear not: the memory saving feature allows to compute POD and mPOD without loading the data into memory!
-
-- Exercise 5. We consider the flow of an impinging gas jet again, but this time on a numerical test case. This dataset was produced by Yannic Lowenstein during his STP at VKI at the end of 2023, with the help of Dr. Maria Faruoli. The Reynolds number is two orders of magnitude higher than in exercise 2, yet the flow features you will observe are pretty similar, at least qualitatively. From a learning perspective, the key feature of this test case is that the data is not available on a uniform grid. But fear not: with the new features, it is possible to compute the decompositions using appropriate weights!
- 
+
+
+MODULO - latest update 2.0
+===================
+
+This repository contains version 2.0 of MODULO (MODal mULtiscale pOd), a software developed at the von Karman Institute to perform data-driven modal decompositions and, in particular, the Multiscale Proper Orthogonal Decomposition (mPOD).
+
+The old version based on MATLAB implementation and related GUI is no longer maintained but will remain available on the branch "Old_Matlab_Implementation". We also keep the first Python implementation in the branch "Old_Python_Implementation". See the Readme file in these branches for more information.
+
+#### Documentation
+
+The full documentation is available at https://modulo.readthedocs.io/en/latest/intro.html.
+This documentation is stored alongside the source code and linked to a specific version of MODULO.
+
+## What is MODULO, and what are data-driven decompositions?
+
+MODULO allows to compute data-driven decompositions of experimental and numerical data. To have a concise overview of the context, we refer to: 
+
+- Ninni, D., Mendez, M. A. (2020), "MODULO: A Software for Multiscale Proper Orthogonal Decomposition of data", Software X, Vol 12, 100622, https://doi.org/10.1016/j.softx.2020.100622.
+
+- Poletti, R., Schena, L., Ninni, D., Mendez, M.A (2024) "MODULO: a python toolbox for data-driven modal decomposition", Submitted to Journal of Open Source Software. Preprint available [here](https://www.researchgate.net/publication/376885484_MODULO_a_python_toolbox_for_data-driven_modal_decomposition)
+
+The first article also presents the first version of MODULO (available in the OLD_Matlab_Implementation branch) and its GUI developed by D. Ninni. The second introduces MODULO v2 in this branch and alternative open source projects. While many projects allows for computing common decompositions such as POD, DMD and the SPODs, MODULO is currently the only opensource project allowing to compute the mPOD.
+
+For a more comprehensive overview on the theory of data-driven decompositions, we refer to the chapter:
+
+- Mendez, M. A. (2023) "Generalized and Multiscale Modal Analysis". In : Mendez M.A., Ianiro, A., Noack, B.R., Brunton, S. L. (Eds), "Data-Driven Fluid Mechanics: Combining First Principles and Machine Learning". Cambridge University Press, 2023:153-181. https://doi.org/10.1017/9781108896214.013. The pre-print is available at https://arxiv.org/abs/2208.12630. 
+
+and the article that first presented the complete treatment of the mPOD :
+
+- Mendez, M. A., Balabane, M., Buchlin, J.-M. (2019) "Multi-Scale Proper Orthogonal Decomposition of Complex Fluid Flows" Journal of Fluid Mechanics 870:988-1036, https://doi.org/10.1017/9781108896214.013. The pre-print is available at https://arxiv.org/abs/2208.12630. 
+
+Ongoing works on nonlinear methods are discussed here:
+
+- Mendez, M. A. (2023) "Linear and Nonlinear Dimensionality Reduction from Fluid Mechanics to Machine Learning", Meas. Sci. Technol. 34(042001), https://doi.org/10.1088/1361-6501/acaffe. The pre-print is available at https://arxiv.org/abs/2208.07746.   
+
+## What is new in this V 2.0? 
+
+This version expands considerably the version v1 in "Old_Python_Implementation", for which a first tutorial was provided by L. Schena in https://www.youtube.com/watch?v=y2uSvdxAwHk. 
+The major updates are the following :
+
+1. Faster EIG/SVD algorithms, using powerful randomized svd solvers from scikit_learn (see [this](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.TruncatedSVD.html) and [this](https://scikit-learn.org/stable/modules/generated/sklearn.utils.extmath.randomized_svd.html) ). It is now possible to select various options as "eig_solver" and "svd_solver", offering different trade-offs in terms of accuracy vs computational time.
+
+2. In addition to the traditional POD computation using the K matrix (Sirovinch's method), it is now possible to compute the POD directly via SVD using any of the four "svd_solver" options.
+This is generally faster but requires more memory.
+
+3. Faster subscale estimators for the mPOD: the previous version used the rank of the correlation matrix in each scale to define the number of modes to be computed in each portion of the splitting vector before assembling the full basis. This is computationally very demanding. This estimation has been replaced by a frequency-based threshold (i.e. based on the frequency bins within each portion) since one can show that the frequency-based estimator is always more "conservative" than the rank-based estimator.
+
+4. Major improvement on the memory saving option: the previous version of modulo always required in input the matrix D. Then, if the memory saving option was active, the matrix was partitioned and stored locally to free the RAM before computing the correlation matrix (see [this tutorial by D. Ninni](https://www.youtube.com/watch?v=LclxO1WTuao)). In the new version, it is possible to initialize a modulo object *without* the matrix D (see exercise 5 in the examples). Instead, one can create the partitions without loading the matrix D.
+
+5. Implementation of Dynamic Mode Decomposition (DMD) from [Schmid, P.J 2010](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/dynamic-mode-decomposition-of-numerical-and-experimental-data/AA4C763B525515AD4521A6CC5E10DBD4).
+
+6. Implementation of the two Spectral POD formulations, namely the one from [Sieber et al 2016](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/abs/spectral-proper-orthogonal-decomposition/DCD8A6EDEFD56F5A9715DBAD38BD461A), and the one from [Towne et al 2018](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/abs/spectral-proper-orthogonal-decomposition-and-its-relationship-to-dynamic-mode-decomposition-and-resolvent-analysis/EC2A6DF76490A0B9EB208CC2CA037717)
+
+7. Implementation of a kernel version of the POD, in which the correlation matrix is replaced by a kernel matrix. This is described in Lecture 15 of the course [Hands on Machine Learning for Fluid dynamics 2023](https://www.vki.ac.be/index.php/events-ls/events/eventdetail/552/-/online-on-site-hands-on-machine-learning-for-fluid-dynamics-2023). See also [this](https://arxiv.org/abs/2208.07746).
+
+8. Implementation of a formulation for non-uniform meshes, using a weighted matrix for all the relevant inner products. This is currently available only for POD and mPOD but allows for handling data produced from CFD simulation without resampling on a uniform grid (see exercise 4). It can be used both with and without the memory-saving option.
+
+## New Tutorials 
+
+The installation provides five exercises to explore MODULO's features while familiarizing with data-driven decompositions. These are available in the /exercise/ folder in plain Python format and jupyter notebooks. 
+
+- Exercise 1. In this exercise, we consider the flow past a cylinder. The dataset was created via Large Eddy Simulations (LES) by Denis Dumoulin during his STP at VKI in 2016 (Report available on request). For convenience, the data was first mapped to a Cartesian grid. This test case is by far the most popular because it's well-known to have a simple low-order representation with modes that have nearly harmonic temporal structures. We compute the POD and the DMD and compare the results... the difference between DMD and POD modes is hardly distinguishable!
+
+- Exercise 2. We consider the flow of an impinging gas jet, taken from [this](https://arxiv.org/abs/1804.09646) paper. This dataset was collected via Time-Resolved Particle Image Velocimetry (TR-PIV). Only the first 200 POD modes were stored. This dataset has much richer dynamics than the previous one and cannot be easily approximated using a few modes. We use it to explore the differences between the DFT, the SPODs and the mPOD. These have different purposes and look for different features.
+
+- Exercise 3. We take back the cylinder test case to explore the differences between the POD and the generalized Karhunen–Loève (KL) expansion in which a kernel matrix replaces the correlation matrix. The POD is a particular case of KL where the kernel function generating the kernel matrix is the plain inner product. Here, we also consider a Gaussian kernel. Different kernel functions define similarity in different ways and thus produce widely different modes. Different modal structures tell different stories about the dataset, but... what can you say about efficiency in data compression? 
+
+- Exercise 4. We consider the flow past a cylinder again, but this time in transient conditions and on an experimental test case taken from [this](https://arxiv.org/abs/2001.01971) paper. In this exercise, you can reproduce the same results from the article to see how the mPOD allows to achieve both time and frequency localization without compromising much of the convergence of the POD. The dataset is quite large, so you might have difficulties handling it if you have less than 32 GB of RAM. But fear not: the memory saving feature allows to compute POD and mPOD without loading the data into memory!
+
+- Exercise 5. We consider the flow of an impinging gas jet again, but this time on a numerical test case. This dataset was produced by Yannic Lowenstein during his STP at VKI at the end of 2023, with the help of Dr. Maria Faruoli. The Reynolds number is two orders of magnitude higher than in exercise 2, yet the flow features you will observe are pretty similar, at least qualitatively. From a learning perspective, the key feature of this test case is that the data is not available on a uniform grid. But fear not: with the new features, it is possible to compute the decompositions using appropriate weights!
+
```

### Comparing `modulo_vki-2.0.4/modulo_vki/__init__.py` & `modulo_vki-2.0.5/modulo_vki/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-
-#from ._version import get_versions
-#__version__ = get_versions()['version']
-#del get_versions
-
-
-# from .utils.read_db import *
-# from .utils._utils import *
-# from .utils._plots import *
-# from .utils.others import *
-
-# from .core._k_matrix import *
-# from .core._dft import *
-# from .core._dmd_s import *
-# from .core._k_matrix import *
-# from .core._mpod_time import *
-# from .core._mpod_space import *
-# from .core._pod_time import *
-# from .core._pod_space import *
-# from .core._spod_s import *
-# from .core._spod_t import *
-
+
+#from ._version import get_versions
+#__version__ = get_versions()['version']
+#del get_versions
+
+
+# from .utils.read_db import *
+# from .utils._utils import *
+# from .utils._plots import *
+# from .utils.others import *
+
+# from .core._k_matrix import *
+# from .core._dft import *
+# from .core._dmd_s import *
+# from .core._k_matrix import *
+# from .core._mpod_time import *
+# from .core._mpod_space import *
+# from .core._pod_time import *
+# from .core._pod_space import *
+# from .core._spod_s import *
+# from .core._spod_t import *
+
 from modulo_vki.modulo import ModuloVKI
```

### Comparing `modulo_vki-2.0.4/modulo_vki/core/_dft.py` & `modulo_vki-2.0.5/modulo_vki/core/_dft.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import os
-
-import numpy as np
-from tqdm import tqdm
-
-
-def dft_fit(N_T, F_S, D, FOLDER_OUT, SAVE_DFT=False):
-    """
-    This function computes the DFT form the dataset D.
-    Currently, this does not handle the memory saving feature.
-    
-    :param N_T: int.
-        number of snapshots 
-    :param F_S:
-        Sampling frequency (in Hz)
-    :param D:
-        Snapshot matrix
-    :param FOLDER_OUT:
-        Folder in which the results are saved if SAVE_SPATIAL_POD = True
-    :param SAVE_DFT:
-        If True, results are saved on disk and released from memory
-        
-    :return: Sorted_Freqs, np.array
-        Frequency bins, in Hz. 
-    :return: Phi_F, np.array
-        (Complex) Spatial structures for each mode
-    :return: SIGMA_F, np.array
-         (real) amplitude of each modes
-    
-    """
-    n_t = int(N_T)
-    Freqs = np.fft.fftfreq(n_t) * F_S  # Compute the frequency bins
-    # PSI_F = np.conj(np.fft.fft(np.eye(n_t)) / np.sqrt(n_t))  # Prepare the Fourier Matrix.
-
-    # Method 1 (didactic!)
-    # PHI_SIGMA = np.dot(D, np.conj(PSI_F))  # This is PHI * SIGMA
-
-    # Method 2
-    PHI_SIGMA = (np.fft.fft(D, n_t, 1)) / (n_t ** 0.5)
-
-    PHI_F = np.zeros((D.shape[0], n_t), dtype=complex)  # Initialize the PHI_F MATRIX
-    SIGMA_F = np.zeros(n_t)  # Initialize the SIGMA_F MATRIX
-
-    # Now we proceed with the normalization. This is also intense so we time it
-    for r in tqdm(range(0, n_t)):  # Loop over the PHI_SIGMA to normalize
-        # MEX = 'Proj ' + str(r + 1) + ' /' + str(n_t)
-        # print(MEX)
-        SIGMA_F[r] = abs(np.vdot(PHI_SIGMA[:, r], PHI_SIGMA[:, r])) ** 0.5
-        PHI_F[:, r] = PHI_SIGMA[:, r] / SIGMA_F[r]
-
-    Indices = np.flipud(np.argsort(SIGMA_F))  # find indices for sorting in decreasing order
-    Sorted_Sigmas = SIGMA_F[Indices]  # Sort all the sigmas
-    Sorted_Freqs = Freqs[Indices]  # Sort all the frequencies accordingly.
-    Phi_F = PHI_F[:, Indices]  # Sorted Spatial Structures Matrix
-    SIGMA_F = Sorted_Sigmas  # Sorted Amplitude Matrix (vector)
-
-    if SAVE_DFT:
-        os.makedirs(FOLDER_OUT + 'DFT', exist_ok=True)
-        np.savez(FOLDER_OUT + 'DFT/dft_fitted', Freqs=Sorted_Freqs, Phis=Phi_F, Sigmas=SIGMA_F)
-
-    return Sorted_Freqs, Phi_F, SIGMA_F
+import os
+
+import numpy as np
+from tqdm import tqdm
+
+
+def dft_fit(N_T, F_S, D, FOLDER_OUT, SAVE_DFT=False):
+    """
+    This function computes the DFT form the dataset D.
+    Currently, this does not handle the memory saving feature.
+    
+    :param N_T: int.
+        number of snapshots 
+    :param F_S:
+        Sampling frequency (in Hz)
+    :param D:
+        Snapshot matrix
+    :param FOLDER_OUT:
+        Folder in which the results are saved if SAVE_SPATIAL_POD = True
+    :param SAVE_DFT:
+        If True, results are saved on disk and released from memory
+        
+    :return: Sorted_Freqs, np.array
+        Frequency bins, in Hz. 
+    :return: Phi_F, np.array
+        (Complex) Spatial structures for each mode
+    :return: SIGMA_F, np.array
+         (real) amplitude of each modes
+    
+    """
+    n_t = int(N_T)
+    Freqs = np.fft.fftfreq(n_t) * F_S  # Compute the frequency bins
+    # PSI_F = np.conj(np.fft.fft(np.eye(n_t)) / np.sqrt(n_t))  # Prepare the Fourier Matrix.
+
+    # Method 1 (didactic!)
+    # PHI_SIGMA = np.dot(D, np.conj(PSI_F))  # This is PHI * SIGMA
+
+    # Method 2
+    PHI_SIGMA = (np.fft.fft(D, n_t, 1)) / (n_t ** 0.5)
+
+    PHI_F = np.zeros((D.shape[0], n_t), dtype=complex)  # Initialize the PHI_F MATRIX
+    SIGMA_F = np.zeros(n_t)  # Initialize the SIGMA_F MATRIX
+
+    # Now we proceed with the normalization. This is also intense so we time it
+    for r in tqdm(range(0, n_t)):  # Loop over the PHI_SIGMA to normalize
+        # MEX = 'Proj ' + str(r + 1) + ' /' + str(n_t)
+        # print(MEX)
+        SIGMA_F[r] = abs(np.vdot(PHI_SIGMA[:, r], PHI_SIGMA[:, r])) ** 0.5
+        PHI_F[:, r] = PHI_SIGMA[:, r] / SIGMA_F[r]
+
+    Indices = np.flipud(np.argsort(SIGMA_F))  # find indices for sorting in decreasing order
+    Sorted_Sigmas = SIGMA_F[Indices]  # Sort all the sigmas
+    Sorted_Freqs = Freqs[Indices]  # Sort all the frequencies accordingly.
+    Phi_F = PHI_F[:, Indices]  # Sorted Spatial Structures Matrix
+    SIGMA_F = Sorted_Sigmas  # Sorted Amplitude Matrix (vector)
+
+    if SAVE_DFT:
+        os.makedirs(FOLDER_OUT + 'DFT', exist_ok=True)
+        np.savez(FOLDER_OUT + 'DFT/dft_fitted', Freqs=Sorted_Freqs, Phis=Phi_F, Sigmas=SIGMA_F)
+
+    return Sorted_Freqs, Phi_F, SIGMA_F
```

### Comparing `modulo_vki-2.0.4/modulo_vki/core/_dmd_s.py` & `modulo_vki-2.0.5/modulo_vki/core/_dmd_s.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-import os
-import numpy as np
-from numpy import linalg as LA
-from ..utils._utils import switch_svds
-
-
-def dmd_s(D_1, D_2, n_Modes, F_S,
-          SAVE_T_DMD=False,
-          FOLDER_OUT='./',
-          svd_solver: str = 'svd_sklearn_truncated'):
-    """
-    This method computes the Dynamic Mode Decomposition (DMD) using hte PIP algorithm from Penland.    
-    
-    :param D_1: np.array 
-           First portion of the data, i.e. D[:,0:n_t-1]            
-    :param D_2: np.array
-           Second portion of the data, i.e. D[:,1:n_t]
-    :param Phi_P, Psi_P, Sigma_P: np.arrays
-           POD decomposition of D1
-    :param F_S: float
-           Sampling frequency in Hz
-    :param FOLDER_OUT: str
-           Folder in which the results will be saved (if SAVE_T_DMD=True)
-    :param K: np.array
-           Temporal correlation matrix
-    :param SAVE_T_POD: bool
-           A flag deciding whether the results are saved on disk or not. If the MEMORY_SAVING feature is active, it is switched True by default.
-    :param n_Modes: int
-           number of modes that will be computed
-    :param svd_solver: str,
-           svd solver to be used 
-          
-     
-    :return1 Phi_D: np.array. 
-          DMD's complex spatial structures
-    :return2 Lambda_D: np.array. 
-          DMD Eigenvalues (of the reduced propagator)
-    :return3 freqs: np.array. 
-          Frequencies (in Hz, associated to the DMD modes)
-    :return4 a0s: np.array. 
-          Initial Coefficients of the Modes
-    """   
-    
-    Phi_P, Psi_P, Sigma_P = switch_svds(D_1, n_Modes, svd_solver)
-    print('SVD of D1 rdy')
-    Sigma_inv = np.diag(1 / Sigma_P)
-    dt = 1 / F_S
-    # %% Step 3: Compute approximated propagator
-    P_A = LA.multi_dot([np.transpose(Phi_P), D_2, Psi_P, Sigma_inv])
-    print('reduced propagator rdy')
-
-    # %% Step 4: Compute eigenvalues of the system
-    Lambda, Q = LA.eig(P_A) # not necessarily symmetric def pos! Avoid eigsh, eigh
-    freqs = np.imag(np.log(Lambda)) / (2 * np.pi * dt)
-    print(' lambdas and freqs rdy')
-
-    # %% Step 5: Spatial structures of the DMD in the PIP style
-    Phi_D = LA.multi_dot([D_2, Psi_P, Sigma_inv, Q])
-    print('Phi_D rdy')
-
-    # %% Step 6: Compute the initial coefficients
-    # a0s=LA.lstsq(Phi_D, D_1[:,0],rcond=None)
-    a0s = LA.pinv(Phi_D).dot(D_1[:, 0])
-    print('Sigma_D rdy')
-
-    if SAVE_T_DMD:
-        os.makedirs(FOLDER_OUT + "/DMD/", exist_ok=True)
-        print("Saving DMD results")
-        np.savez(FOLDER_OUT + '/DMD/dmd_decomposition',
-                 Phi_D=Phi_D, Lambda=Lambda, freqs=freqs, a0s=a0s)
-
-    return Phi_D, Lambda, freqs, a0s
+import os
+import numpy as np
+from numpy import linalg as LA
+from ..utils._utils import switch_svds
+
+
+def dmd_s(D_1, D_2, n_Modes, F_S,
+          SAVE_T_DMD=False,
+          FOLDER_OUT='./',
+          svd_solver: str = 'svd_sklearn_truncated'):
+    """
+    This method computes the Dynamic Mode Decomposition (DMD) using hte PIP algorithm from Penland.    
+    
+    :param D_1: np.array 
+           First portion of the data, i.e. D[:,0:n_t-1]            
+    :param D_2: np.array
+           Second portion of the data, i.e. D[:,1:n_t]
+    :param Phi_P, Psi_P, Sigma_P: np.arrays
+           POD decomposition of D1
+    :param F_S: float
+           Sampling frequency in Hz
+    :param FOLDER_OUT: str
+           Folder in which the results will be saved (if SAVE_T_DMD=True)
+    :param K: np.array
+           Temporal correlation matrix
+    :param SAVE_T_POD: bool
+           A flag deciding whether the results are saved on disk or not. If the MEMORY_SAVING feature is active, it is switched True by default.
+    :param n_Modes: int
+           number of modes that will be computed
+    :param svd_solver: str,
+           svd solver to be used 
+          
+     
+    :return1 Phi_D: np.array. 
+          DMD's complex spatial structures
+    :return2 Lambda_D: np.array. 
+          DMD Eigenvalues (of the reduced propagator)
+    :return3 freqs: np.array. 
+          Frequencies (in Hz, associated to the DMD modes)
+    :return4 a0s: np.array. 
+          Initial Coefficients of the Modes
+    """   
+    
+    Phi_P, Psi_P, Sigma_P = switch_svds(D_1, n_Modes, svd_solver)
+    print('SVD of D1 rdy')
+    Sigma_inv = np.diag(1 / Sigma_P)
+    dt = 1 / F_S
+    # %% Step 3: Compute approximated propagator
+    P_A = LA.multi_dot([np.transpose(Phi_P), D_2, Psi_P, Sigma_inv])
+    print('reduced propagator rdy')
+
+    # %% Step 4: Compute eigenvalues of the system
+    Lambda, Q = LA.eig(P_A) # not necessarily symmetric def pos! Avoid eigsh, eigh
+    freqs = np.imag(np.log(Lambda)) / (2 * np.pi * dt)
+    print(' lambdas and freqs rdy')
+
+    # %% Step 5: Spatial structures of the DMD in the PIP style
+    Phi_D = LA.multi_dot([D_2, Psi_P, Sigma_inv, Q])
+    print('Phi_D rdy')
+
+    # %% Step 6: Compute the initial coefficients
+    # a0s=LA.lstsq(Phi_D, D_1[:,0],rcond=None)
+    a0s = LA.pinv(Phi_D).dot(D_1[:, 0])
+    print('Sigma_D rdy')
+
+    if SAVE_T_DMD:
+        os.makedirs(FOLDER_OUT + "/DMD/", exist_ok=True)
+        print("Saving DMD results")
+        np.savez(FOLDER_OUT + '/DMD/dmd_decomposition',
+                 Phi_D=Phi_D, Lambda=Lambda, freqs=freqs, a0s=a0s)
+
+    return Phi_D, Lambda, freqs, a0s
```

### Comparing `modulo_vki-2.0.4/modulo_vki/core/_mpod_space.py` & `modulo_vki-2.0.5/modulo_vki/core/_mpod_space.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-import numpy as np
-import os
-from tqdm import tqdm
-import math
-
-
-def spatial_basis_mPOD(D, PSI_M, N_T, N_PARTITIONS, N_S, MEMORY_SAVING, FOLDER_OUT, SAVE: bool = False,weights: np.array = np.array([])):
-    """
-    Given the temporal basis of the mPOD now the spatial ones are computed
-    
-    :param D: 
-        Snapshot matrix D: if memory savig is active, this is ignored.    
-    :param PSI_M: np.array.: 
-        The mPOD temporal basis Psi tentatively assembled from all scales
-    :param N_T: int. 
-        Number of snapshots
-    :param N_PARTITIONS: int. 
-        Number of partitions in the memory saving
-    :param N_S: int. 
-        Number of grid points in space
-    :param MEMORY_SAVING: bool. 
-        Inherited from main class, if True turns on the MEMORY_SAVING feature, loading the partitions and starting the proper algorithm  
-    :param FOLDER_OUT: str. 
-        Folder in which the results are saved if SAVE_SPATIAL_POD = True
-    :param SAVE_SPATIAL_POD: bool.
-        If True, results are saved on disk and released from memory
-    :param weights:  np.array
-        weight vector [w_i,....,w_{N_s}] where w_i = area_cell_i/area_grid. Only needed if grid is non-uniform & MEMORY_SAVING== True
-    :return: Phi_M, Psi_M, Sigma_M: np.arrays. The final (sorted) mPOD decomposition
-    """
-    
-    R1 = 0; R2 = 0
-    if MEMORY_SAVING:
-        SAVE = True
-        os.makedirs(FOLDER_OUT + '/mPOD/', exist_ok=True)
-        dim_col = math.floor(N_T / N_PARTITIONS)
-        dim_row = math.floor(N_S / N_PARTITIONS)
-        dr = np.zeros((dim_row, N_T))
-
-        # 1 --- Converting partitions dC to dR
-        if N_S % N_PARTITIONS != 0:
-            tot_blocks_row = N_PARTITIONS + 1
-        else:
-            tot_blocks_row = N_PARTITIONS
-
-        if N_T % N_PARTITIONS != 0:
-            tot_blocks_col = N_PARTITIONS + 1
-        else:
-            tot_blocks_col = N_PARTITIONS
-
-        fixed = 0
-
-        for i in range(1, tot_blocks_row + 1):
-            # --- Check if dim_row has to be fixed:
-            if i == tot_blocks_row and (N_S - dim_row * N_PARTITIONS > 0):
-                dim_row_fix = N_S - dim_row * N_PARTITIONS
-                dr = np.zeros((dim_row_fix, N_T))
-
-            for cont in range(1, tot_blocks_col + 1):
-                di = np.load(FOLDER_OUT + f"/data_partitions/di_{cont}.npz")['di']
-
-                if i == tot_blocks_row and (N_S - dim_row * N_PARTITIONS > 0) and fixed == 0:
-                    R1 = R2
-                    R2 = R1 + (N_S - dim_row * N_PARTITIONS)
-                    fixed = 1
-                elif fixed == 0:
-                    R1 = (i - 1) * dim_row
-                    R2 = i * dim_row
-
-                # Same as before, but we don't need the variable fixed because if
-                #         % the code runs this loop, it will be the last time
-
-                if cont == tot_blocks_col and (N_T - dim_col * N_PARTITIONS > 0):
-                    C1 = C2
-                    C2 = C1 + (N_T - dim_col * N_PARTITIONS)
-                else:
-                    C1 = (cont - 1) * dim_col
-                    C2 = cont * dim_col
-
-                dr[:, C1:C2] = di[R1:R2, :]
-
-            # 2 --- Computing partitions R of PHI_SIGMA
-            PHI_SIGMA_BLOCK = dr @ PSI_M
-            np.savez(FOLDER_OUT + f'/mPOD/phi_sigma_{i}', PHI_SIGMA_BLOCK)
-
-        # 3 --- Convert partitions R to partitions C and get SIGMA
-        R = PSI_M.shape[1]
-        dim_col = math.floor(R / N_PARTITIONS)
-        dim_row = math.floor(N_S / N_PARTITIONS)
-        dps = np.zeros((N_S, dim_col))
-        SIGMA_M = []
-        PHI_M = []
-
-        if R % N_PARTITIONS != 0:
-            tot_blocks_col = N_PARTITIONS + 1
-        else:
-            tot_blocks_col = N_PARTITIONS
-
-        fixed = 0
-
-        # Here we apply the same logic of the loop before
-
-        for j in range(1, tot_blocks_col + 1):
-
-            if j == tot_blocks_col and (R - dim_col * N_PARTITIONS > 0):
-                dim_col_fix = R - dim_col * N_PARTITIONS
-                dps = np.zeros((N_S, dim_col_fix))
-
-            for k in range(1, tot_blocks_row + 1):
-                PHI_SIGMA_BLOCK = np.load(FOLDER_OUT + f"/mPOD/phi_sigma_{k}.npz")['arr_0']
-
-                if j == tot_blocks_col and (R - dim_col * N_PARTITIONS > 0) and fixed == 0:
-                    R1 = R2
-                    R2 = R1 + (R - dim_col * N_PARTITIONS)
-                    fixed = 1
-                elif fixed == 0:
-                    R1 = (j - 1) * dim_col
-                    R2 = j * dim_col
-
-                if k == tot_blocks_row and (N_S - dim_row * N_PARTITIONS > 0):
-                    C1 = C2
-                    C2 = C1 + (N_S - dim_row * N_PARTITIONS)
-                else:
-                    C1 = (k - 1) * dim_row
-                    C2 = k * dim_row
-
-                dps[C1:C2, :] = PHI_SIGMA_BLOCK[:, R1:R2]
-
-            # Getting sigmas and phis
-            for z in range(R1, R2):
-                zz = z - R1
-                if weights.size == 0:
-                    SIGMA_M.append(np.linalg.norm(dps[:, zz]))
-                else:
-                    SIGMA_M.append(np.linalg.norm(dps[:, zz]*np.sqrt(weights)))
-                tmp = dps[:, zz] / SIGMA_M[z]
-                #print(f'Shape tmp = {np.shape(tmp)}')
-                PHI_M.append(tmp)
-                np.savez(FOLDER_OUT + f'/mPOD/phi_{z + 1}', tmp)
-
-        Indices = np.argsort(SIGMA_M)[::-1]  # find indices for sorting in decreasing order
-        SIGMA_M = np.asarray(SIGMA_M)
-        PHI_M = np.asarray(PHI_M).T
-        PSI_M = np.asarray(PSI_M)
-        Sorted_Sigmas = SIGMA_M[Indices]  # Sort all the sigmas
-        Phi_M = PHI_M[:, Indices]  # Sorted Spatial Structures Matrix
-        Psi_M = PSI_M[:, Indices]  # Sorted Temporal Structures Matrix
-        Sigma_M = Sorted_Sigmas  # Sorted Amplitude Matrix
-
-    else:
-        R = PSI_M.shape[1]
-        PHI_M_SIGMA_M = np.dot(D, (PSI_M))
-        # Initialize the output
-        PHI_M = np.zeros((N_S, R))
-        SIGMA_M = np.zeros((R))
-
-        for i in tqdm(range(0, R)):
-            # print('Completing mPOD Mode ' + str(i))
-            # Assign the norm as amplitude
-            if weights.size == 0:
-                SIGMA_M[i] = np.linalg.norm(PHI_M_SIGMA_M[:, i])
-            else:
-                SIGMA_M[i] = np.linalg.norm(PHI_M_SIGMA_M[:, i]*np.sqrt(weights))
-            # Normalize the columns of C to get spatial modes
-            PHI_M[:, i] = PHI_M_SIGMA_M[:, i] / SIGMA_M[i]
-
-        Indices = np.flipud(np.argsort(SIGMA_M))  # find indices for sorting in decreasing order
-        Sorted_Sigmas = SIGMA_M[Indices]  # Sort all the sigmas
-        Phi_M = PHI_M[:, Indices]  # Sorted Spatial Structures Matrix
-        Psi_M = PSI_M[:, Indices]  # Sorted Temporal Structures Matrix
-        Sigma_M = Sorted_Sigmas  # Sorted Amplitude Matrix
-
-    if SAVE:
-        '''Saving results in MODULO tmp proper folder'''
-        os.makedirs(FOLDER_OUT + '/mPOD/', exist_ok=True)
-        np.savez(FOLDER_OUT + "/mPOD/sorted_phis", Phi_M)
-        np.savez(FOLDER_OUT + "/mPOD/sorted_psis", Psi_M)
-        np.savez(FOLDER_OUT + "/mPOD/sorted_sigma", Sorted_Sigmas)
-
-    return Phi_M, Psi_M, Sigma_M
+import numpy as np
+import os
+from tqdm import tqdm
+import math
+
+
+def spatial_basis_mPOD(D, PSI_M, N_T, N_PARTITIONS, N_S, MEMORY_SAVING, FOLDER_OUT, SAVE: bool = False,weights: np.array = np.array([])):
+    """
+    Given the temporal basis of the mPOD now the spatial ones are computed
+    
+    :param D: 
+        Snapshot matrix D: if memory savig is active, this is ignored.    
+    :param PSI_M: np.array.: 
+        The mPOD temporal basis Psi tentatively assembled from all scales
+    :param N_T: int. 
+        Number of snapshots
+    :param N_PARTITIONS: int. 
+        Number of partitions in the memory saving
+    :param N_S: int. 
+        Number of grid points in space
+    :param MEMORY_SAVING: bool. 
+        Inherited from main class, if True turns on the MEMORY_SAVING feature, loading the partitions and starting the proper algorithm  
+    :param FOLDER_OUT: str. 
+        Folder in which the results are saved if SAVE_SPATIAL_POD = True
+    :param SAVE_SPATIAL_POD: bool.
+        If True, results are saved on disk and released from memory
+    :param weights:  np.array
+        weight vector [w_i,....,w_{N_s}] where w_i = area_cell_i/area_grid. Only needed if grid is non-uniform & MEMORY_SAVING== True
+    :return: Phi_M, Psi_M, Sigma_M: np.arrays. The final (sorted) mPOD decomposition
+    """
+    
+    R1 = 0; R2 = 0
+    if MEMORY_SAVING:
+        SAVE = True
+        os.makedirs(FOLDER_OUT + '/mPOD/', exist_ok=True)
+        dim_col = math.floor(N_T / N_PARTITIONS)
+        dim_row = math.floor(N_S / N_PARTITIONS)
+        dr = np.zeros((dim_row, N_T))
+
+        # 1 --- Converting partitions dC to dR
+        if N_S % N_PARTITIONS != 0:
+            tot_blocks_row = N_PARTITIONS + 1
+        else:
+            tot_blocks_row = N_PARTITIONS
+
+        if N_T % N_PARTITIONS != 0:
+            tot_blocks_col = N_PARTITIONS + 1
+        else:
+            tot_blocks_col = N_PARTITIONS
+
+        fixed = 0
+
+        for i in range(1, tot_blocks_row + 1):
+            # --- Check if dim_row has to be fixed:
+            if i == tot_blocks_row and (N_S - dim_row * N_PARTITIONS > 0):
+                dim_row_fix = N_S - dim_row * N_PARTITIONS
+                dr = np.zeros((dim_row_fix, N_T))
+
+            for cont in range(1, tot_blocks_col + 1):
+                di = np.load(FOLDER_OUT + f"/data_partitions/di_{cont}.npz")['di']
+
+                if i == tot_blocks_row and (N_S - dim_row * N_PARTITIONS > 0) and fixed == 0:
+                    R1 = R2
+                    R2 = R1 + (N_S - dim_row * N_PARTITIONS)
+                    fixed = 1
+                elif fixed == 0:
+                    R1 = (i - 1) * dim_row
+                    R2 = i * dim_row
+
+                # Same as before, but we don't need the variable fixed because if
+                #         % the code runs this loop, it will be the last time
+
+                if cont == tot_blocks_col and (N_T - dim_col * N_PARTITIONS > 0):
+                    C1 = C2
+                    C2 = C1 + (N_T - dim_col * N_PARTITIONS)
+                else:
+                    C1 = (cont - 1) * dim_col
+                    C2 = cont * dim_col
+
+                dr[:, C1:C2] = di[R1:R2, :]
+
+            # 2 --- Computing partitions R of PHI_SIGMA
+            PHI_SIGMA_BLOCK = dr @ PSI_M
+            np.savez(FOLDER_OUT + f'/mPOD/phi_sigma_{i}', PHI_SIGMA_BLOCK)
+
+        # 3 --- Convert partitions R to partitions C and get SIGMA
+        R = PSI_M.shape[1]
+        dim_col = math.floor(R / N_PARTITIONS)
+        dim_row = math.floor(N_S / N_PARTITIONS)
+        dps = np.zeros((N_S, dim_col))
+        SIGMA_M = []
+        PHI_M = []
+
+        if R % N_PARTITIONS != 0:
+            tot_blocks_col = N_PARTITIONS + 1
+        else:
+            tot_blocks_col = N_PARTITIONS
+
+        fixed = 0
+
+        # Here we apply the same logic of the loop before
+
+        for j in range(1, tot_blocks_col + 1):
+
+            if j == tot_blocks_col and (R - dim_col * N_PARTITIONS > 0):
+                dim_col_fix = R - dim_col * N_PARTITIONS
+                dps = np.zeros((N_S, dim_col_fix))
+
+            for k in range(1, tot_blocks_row + 1):
+                PHI_SIGMA_BLOCK = np.load(FOLDER_OUT + f"/mPOD/phi_sigma_{k}.npz")['arr_0']
+
+                if j == tot_blocks_col and (R - dim_col * N_PARTITIONS > 0) and fixed == 0:
+                    R1 = R2
+                    R2 = R1 + (R - dim_col * N_PARTITIONS)
+                    fixed = 1
+                elif fixed == 0:
+                    R1 = (j - 1) * dim_col
+                    R2 = j * dim_col
+
+                if k == tot_blocks_row and (N_S - dim_row * N_PARTITIONS > 0):
+                    C1 = C2
+                    C2 = C1 + (N_S - dim_row * N_PARTITIONS)
+                else:
+                    C1 = (k - 1) * dim_row
+                    C2 = k * dim_row
+
+                dps[C1:C2, :] = PHI_SIGMA_BLOCK[:, R1:R2]
+
+            # Getting sigmas and phis
+            for z in range(R1, R2):
+                zz = z - R1
+                if weights.size == 0:
+                    SIGMA_M.append(np.linalg.norm(dps[:, zz]))
+                else:
+                    SIGMA_M.append(np.linalg.norm(dps[:, zz]*np.sqrt(weights)))
+                tmp = dps[:, zz] / SIGMA_M[z]
+                #print(f'Shape tmp = {np.shape(tmp)}')
+                PHI_M.append(tmp)
+                np.savez(FOLDER_OUT + f'/mPOD/phi_{z + 1}', tmp)
+
+        Indices = np.argsort(SIGMA_M)[::-1]  # find indices for sorting in decreasing order
+        SIGMA_M = np.asarray(SIGMA_M)
+        PHI_M = np.asarray(PHI_M).T
+        PSI_M = np.asarray(PSI_M)
+        Sorted_Sigmas = SIGMA_M[Indices]  # Sort all the sigmas
+        Phi_M = PHI_M[:, Indices]  # Sorted Spatial Structures Matrix
+        Psi_M = PSI_M[:, Indices]  # Sorted Temporal Structures Matrix
+        Sigma_M = Sorted_Sigmas  # Sorted Amplitude Matrix
+
+    else:
+        R = PSI_M.shape[1]
+        PHI_M_SIGMA_M = np.dot(D, (PSI_M))
+        # Initialize the output
+        PHI_M = np.zeros((N_S, R))
+        SIGMA_M = np.zeros((R))
+
+        for i in tqdm(range(0, R)):
+            # print('Completing mPOD Mode ' + str(i))
+            # Assign the norm as amplitude
+            if weights.size == 0:
+                SIGMA_M[i] = np.linalg.norm(PHI_M_SIGMA_M[:, i])
+            else:
+                SIGMA_M[i] = np.linalg.norm(PHI_M_SIGMA_M[:, i]*np.sqrt(weights))
+            # Normalize the columns of C to get spatial modes
+            PHI_M[:, i] = PHI_M_SIGMA_M[:, i] / SIGMA_M[i]
+
+        Indices = np.flipud(np.argsort(SIGMA_M))  # find indices for sorting in decreasing order
+        Sorted_Sigmas = SIGMA_M[Indices]  # Sort all the sigmas
+        Phi_M = PHI_M[:, Indices]  # Sorted Spatial Structures Matrix
+        Psi_M = PSI_M[:, Indices]  # Sorted Temporal Structures Matrix
+        Sigma_M = Sorted_Sigmas  # Sorted Amplitude Matrix
+
+    if SAVE:
+        '''Saving results in MODULO tmp proper folder'''
+        os.makedirs(FOLDER_OUT + '/mPOD/', exist_ok=True)
+        np.savez(FOLDER_OUT + "/mPOD/sorted_phis", Phi_M)
+        np.savez(FOLDER_OUT + "/mPOD/sorted_psis", Psi_M)
+        np.savez(FOLDER_OUT + "/mPOD/sorted_sigma", Sorted_Sigmas)
+
+    return Phi_M, Psi_M, Sigma_M
```

### Comparing `modulo_vki-2.0.4/modulo_vki/core/_mpod_time.py` & `modulo_vki-2.0.5/modulo_vki/core/_mpod_time.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-import os
-import numpy as np
-from scipy.signal import firwin  # To create FIR kernels
-from tqdm import tqdm
-from modulo_vki.utils._utils import conv_m, switch_eigs
-
-
-def temporal_basis_mPOD(K, Nf, Ex, F_V, Keep, boundaries, MODE='reduced', dt=1,FOLDER_OUT: str = "./", MEMORY_SAVING: bool = False,SAT: int = 100,n_Modes=10, eig_solver: str = 'svd_sklearn_randomized'):
-    '''
-    This function computes the PSIs for the mPOD. In this implementation, a "dft-trick" is proposed, in order to avoid
-    expansive SVDs. Randomized SVD is used by default for the diagonalization.
-    
-    :param K: 
-        np.array  Temporal correlation matrix
-    :param dt: float.   
-        1/fs, the dt between snapshots. Units in seconds.
-    :param Nf: 
-        np.array. Vector collecting the order of the FIR filters used in each scale.
-    :param Ex: int.
-        Extension at the boundaries of K to impose the boundary conditions (see boundaries). It must be at least as Nf.
-    :param F_V: np.array. 
-        Frequency splitting vector, containing the frequencies of each scale (see article). If the time axis is in seconds, these frequencies are in Hz.
-    :param Keep: np.array. 
-        Vector defining which scale to keep.
-    :param boundaries: str -> {'nearest', 'reflect', 'wrap' or 'extrap'}. 
-        In order to avoid 'edge effects' if the time correlation matrix is not periodic, several boundary conditions can be used. Options are (from scipy.ndimage.convolve):
-        ‘reflect’ (d c b a | a b c d | d c b a)    The input is extended by reflecting about the edge of the last pixel.
-        ‘nearest’ (a a a a | a b c d | d d d d)    The input is extended by replicating the last pixel.
-        ‘wrap’ (a b c d | a b c d | a b c d)       The input is extended by wrapping around to the opposite edge.
-    :param MODE: tr -> {‘reduced’, ‘complete’, ‘r’, ‘raw’}
-        As a final step of this algorithm, the orthogonality is imposed via a QR-factorization. This parameterd define how to perform such factorization, according to numpy.
-        Options: this is a wrapper to np.linalg.qr(_, mode=MODE). Check numpy's documentation.
-        if ‘reduced’ The final basis will not necessarely be full. If ‘complete’ The final basis will always be full
-    :param FOLDER_OUT: str. 
-        This is the directory where intermediate results will be stored if the memory saving is active.It will be ignored if MEMORY_SAVING=False.              
-    :param MEMORY_SAVING: Bool. 
-        If memory saving is active, the results will be saved locally.  Nevertheless, since Psi_M is usually not expensive, it will be returned.        
-    :param SAT: int.
-        Maximum number of modes per scale. The user can decide how many modes to compute; otherwise, modulo set the default SAT=100.
-    :param n_Modes: int. 
-        Total number of modes that will be finally exported   
-    :param eig_solver: str. 
-        This is the eigenvalue solver that will be used. Refer to eigs_swith for the options.      
-    :return PSI_M: np.array. 
-        The mPOD PSIs. Yet to be sorted ! 
-    '''
-
-    if Ex < np.max(Nf):
-        raise RuntimeError("For the mPOD temporal basis computation Ex must be larger than or equal to Nf")
-
-    #Converting F_V in radiants and initialise number of scales M
-    Fs = 1 / dt
-    F_Bank_r = F_V * 2 / Fs
-    M = len(F_Bank_r)
-
-    # Loop over the scales to show the transfer functions
-    Psi_M = np.array([])
-    Lambda_M = np.array([])
-    n_t = K.shape[1]
-    
-   # if K_S:
-   #     Ks = np.zeros((n_t, n_t, M + 1))
-
-    #DFT-trick below: computing frequency bins.
-    Freqs = np.fft.fftfreq(n_t) * Fs
-
-    print("Filtering and Diagonalizing H scale: \n")
-
-    #Filtering and computing eigenvectors
-
-    for m in tqdm(range(0, M)):
-        # Generate the 1d filter for this
-        if m < 1:
-            if Keep[m] == 1:
-             # Low Pass Filter
-             h_A = firwin(Nf[m], F_Bank_r[m], window='hamming')
-             # Filter K_LP
-             print('\n Filtering Largest Scale')
-             K_L = conv_m(K=K, h=h_A, Ex=Ex, boundaries=boundaries)
-             # R_K = np.linalg.matrix_rank(K_L, tol=None, hermitian=True)
-             '''We replace it with an estimation based on the non-zero freqs the cut off frequency of the scale is '''
-             F_CUT = F_Bank_r[m] * Fs / 2
-             Indices = np.argwhere(np.abs(Freqs) < F_CUT)
-             R_K = np.min([len(Indices), SAT])
-             print(str(len(Indices)) + ' Modes Estimated')
-             print('\n Diagonalizing Largest Scale')
-             Psi_P, Lambda_P = switch_eigs(K_L, R_K, eig_solver) #svds_RND(K_L, R_K)
-             Psi_M=Psi_P; Lambda_M=Lambda_P
-            else:
-             print('\n Scale '+str(m)+' jumped (keep['+str(m)+']=0)')  
-            # if K_S:
-            #     Ks[:, :, m] = K_L  # First large scale
-                         
-            # method = signal.choose_conv_method(K, h2d, mode='same')
-        elif m > 0 and m < M - 1:
-            if Keep[m] == 1:
-                # print(m)
-                print('\n Working on Scale '+str(m)+'/'+str(M))
-                # This is the 1d Kernel for Band pass
-                h1d_H = firwin(Nf[m], [F_Bank_r[m], F_Bank_r[m + 1]], pass_zero=False)  # Band-pass
-                F_CUT1 = F_Bank_r[m] * Fs / 2
-                F_CUT2 = F_Bank_r[m + 1] * Fs / 2
-                Indices = np.argwhere((np.abs(Freqs) > F_CUT1) & (np.abs(Freqs) < F_CUT2))
-                R_K = np.min([len(Indices), SAT])  # number of frequencies here
-                print(str(len(Indices)) + ' Modes Estimated')
-                # print('Filtering H Scale ' + str(m + 1) + '/' + str(M))
-                K_H = conv_m(K, h1d_H, Ex, boundaries)
-                # Ks[:, :, m + 1] = K_H  # Intermediate band-pass
-                print('Diagonalizing H Scale ' + str(m + 1) + '/' + str(M))
-                # R_K = np.linalg.matrix_rank(K_H, tol=None, hermitian=True)
-                Psi_P, Lambda_P = switch_eigs(K_H, R_K, eig_solver) #svds_RND(K_H, R_K)  # Diagonalize scale
-                if np.shape(Psi_M)[0]==0: # if this is the first contribute to the basis
-                 Psi_M=Psi_P; Lambda_M=Lambda_P
-                else:                    
-                 Psi_M = np.concatenate((Psi_M, Psi_P), axis=1)  # append to the previous
-                 Lambda_M = np.concatenate((Lambda_M, Lambda_P), axis=0)
-            else:
-                print('\n Scale '+str(m)+' jumped (keep['+str(m)+']=0)')  
-      
-        else: # this is the case m=M: this is a high pass
-            if Keep[m] == 1:
-                print('Working on Scale '+str(m)+'/'+str(M))
-                # This is the 1d Kernel for High Pass (last scale)
-                h1d_H = firwin(Nf[m], F_Bank_r[m], pass_zero=False)
-                F_CUT1 = F_Bank_r[m] * Fs / 2
-                Indices = np.argwhere((np.abs(Freqs) > F_CUT1))
-                R_K = len(Indices)
-                R_K = np.min([len(Indices), SAT])  # number of frequencies here
-                print(str(len(Indices)) + ' Modes Estimated')
-                print('Filtering H Scale ' + str(m + 1) + '/ ' + str(M))
-                K_H = conv_m(K, h1d_H, Ex, boundaries)
-                # Ks[:, :, m + 1] = K_H  # Last (high pass) scale
-                print('Diagonalizing H Scale ' + str(m + 1) + '/ ' + str(M))
-                # R_K = np.linalg.matrix_rank(K_H, tol=None, hermitian=True)
-                Psi_P, Lambda_P = switch_eigs(K_H, R_K, eig_solver) #svds_RND(K_H, R_K)  # Diagonalize scale
-                Psi_M = np.concatenate((Psi_M, Psi_P), axis=1)  # append to the previous
-                Lambda_M = np.concatenate((Lambda_M, Lambda_P), axis=0)
-            else:
-                print('\n Scale '+str(m)+' jumped (keep['+str(m)+']=0)')  
-
-    # Now Order the Scales
-    Indices = np.flip(np.argsort(Lambda_M))  # find indices for sorting in decreasing order
-    Psi_M = Psi_M[:, Indices]  # Sort the temporal structures
-    #print(f"Size psis in mpodtime = {np.shape(Psi_M)}")
-    # Now we complete the basis via re-orghotonalization
-    print('\n QR Polishing...')
-    PSI_M, R = np.linalg.qr(Psi_M, mode=MODE)
-    print('Done!')
-
-    if MEMORY_SAVING:
-        os.makedirs(FOLDER_OUT + '/mPOD', exist_ok=True)
-        np.savez(FOLDER_OUT + '/mPOD/Psis', Psis=PSI_M)
-    
-    return PSI_M[:,0:n_Modes]
+import os
+import numpy as np
+from scipy.signal import firwin  # To create FIR kernels
+from tqdm import tqdm
+from modulo_vki.utils._utils import conv_m, switch_eigs
+
+
+def temporal_basis_mPOD(K, Nf, Ex, F_V, Keep, boundaries, MODE='reduced', dt=1,FOLDER_OUT: str = "./", MEMORY_SAVING: bool = False,SAT: int = 100,n_Modes=10, eig_solver: str = 'svd_sklearn_randomized'):
+    '''
+    This function computes the PSIs for the mPOD. In this implementation, a "dft-trick" is proposed, in order to avoid
+    expansive SVDs. Randomized SVD is used by default for the diagonalization.
+    
+    :param K: 
+        np.array  Temporal correlation matrix
+    :param dt: float.   
+        1/fs, the dt between snapshots. Units in seconds.
+    :param Nf: 
+        np.array. Vector collecting the order of the FIR filters used in each scale.
+    :param Ex: int.
+        Extension at the boundaries of K to impose the boundary conditions (see boundaries). It must be at least as Nf.
+    :param F_V: np.array. 
+        Frequency splitting vector, containing the frequencies of each scale (see article). If the time axis is in seconds, these frequencies are in Hz.
+    :param Keep: np.array. 
+        Vector defining which scale to keep.
+    :param boundaries: str -> {'nearest', 'reflect', 'wrap' or 'extrap'}. 
+        In order to avoid 'edge effects' if the time correlation matrix is not periodic, several boundary conditions can be used. Options are (from scipy.ndimage.convolve):
+        ‘reflect’ (d c b a | a b c d | d c b a)    The input is extended by reflecting about the edge of the last pixel.
+        ‘nearest’ (a a a a | a b c d | d d d d)    The input is extended by replicating the last pixel.
+        ‘wrap’ (a b c d | a b c d | a b c d)       The input is extended by wrapping around to the opposite edge.
+    :param MODE: tr -> {‘reduced’, ‘complete’, ‘r’, ‘raw’}
+        As a final step of this algorithm, the orthogonality is imposed via a QR-factorization. This parameterd define how to perform such factorization, according to numpy.
+        Options: this is a wrapper to np.linalg.qr(_, mode=MODE). Check numpy's documentation.
+        if ‘reduced’ The final basis will not necessarely be full. If ‘complete’ The final basis will always be full
+    :param FOLDER_OUT: str. 
+        This is the directory where intermediate results will be stored if the memory saving is active.It will be ignored if MEMORY_SAVING=False.              
+    :param MEMORY_SAVING: Bool. 
+        If memory saving is active, the results will be saved locally.  Nevertheless, since Psi_M is usually not expensive, it will be returned.        
+    :param SAT: int.
+        Maximum number of modes per scale. The user can decide how many modes to compute; otherwise, modulo set the default SAT=100.
+    :param n_Modes: int. 
+        Total number of modes that will be finally exported   
+    :param eig_solver: str. 
+        This is the eigenvalue solver that will be used. Refer to eigs_swith for the options.      
+    :return PSI_M: np.array. 
+        The mPOD PSIs. Yet to be sorted ! 
+    '''
+
+    if Ex < np.max(Nf):
+        raise RuntimeError("For the mPOD temporal basis computation Ex must be larger than or equal to Nf")
+
+    #Converting F_V in radiants and initialise number of scales M
+    Fs = 1 / dt
+    F_Bank_r = F_V * 2 / Fs
+    M = len(F_Bank_r)
+
+    # Loop over the scales to show the transfer functions
+    Psi_M = np.array([])
+    Lambda_M = np.array([])
+    n_t = K.shape[1]
+    
+   # if K_S:
+   #     Ks = np.zeros((n_t, n_t, M + 1))
+
+    #DFT-trick below: computing frequency bins.
+    Freqs = np.fft.fftfreq(n_t) * Fs
+
+    print("Filtering and Diagonalizing H scale: \n")
+
+    #Filtering and computing eigenvectors
+
+    for m in tqdm(range(0, M)):
+        # Generate the 1d filter for this
+        if m < 1:
+            if Keep[m] == 1:
+             # Low Pass Filter
+             h_A = firwin(Nf[m], F_Bank_r[m], window='hamming')
+             # Filter K_LP
+             print('\n Filtering Largest Scale')
+             K_L = conv_m(K=K, h=h_A, Ex=Ex, boundaries=boundaries)
+             # R_K = np.linalg.matrix_rank(K_L, tol=None, hermitian=True)
+             '''We replace it with an estimation based on the non-zero freqs the cut off frequency of the scale is '''
+             F_CUT = F_Bank_r[m] * Fs / 2
+             Indices = np.argwhere(np.abs(Freqs) < F_CUT)
+             R_K = np.min([len(Indices), SAT])
+             print(str(len(Indices)) + ' Modes Estimated')
+             print('\n Diagonalizing Largest Scale')
+             Psi_P, Lambda_P = switch_eigs(K_L, R_K, eig_solver) #svds_RND(K_L, R_K)
+             Psi_M=Psi_P; Lambda_M=Lambda_P
+            else:
+             print('\n Scale '+str(m)+' jumped (keep['+str(m)+']=0)')  
+            # if K_S:
+            #     Ks[:, :, m] = K_L  # First large scale
+                         
+            # method = signal.choose_conv_method(K, h2d, mode='same')
+        elif m > 0 and m < M - 1:
+            if Keep[m] == 1:
+                # print(m)
+                print('\n Working on Scale '+str(m)+'/'+str(M))
+                # This is the 1d Kernel for Band pass
+                h1d_H = firwin(Nf[m], [F_Bank_r[m], F_Bank_r[m + 1]], pass_zero=False)  # Band-pass
+                F_CUT1 = F_Bank_r[m] * Fs / 2
+                F_CUT2 = F_Bank_r[m + 1] * Fs / 2
+                Indices = np.argwhere((np.abs(Freqs) > F_CUT1) & (np.abs(Freqs) < F_CUT2))
+                R_K = np.min([len(Indices), SAT])  # number of frequencies here
+                print(str(len(Indices)) + ' Modes Estimated')
+                # print('Filtering H Scale ' + str(m + 1) + '/' + str(M))
+                K_H = conv_m(K, h1d_H, Ex, boundaries)
+                # Ks[:, :, m + 1] = K_H  # Intermediate band-pass
+                print('Diagonalizing H Scale ' + str(m + 1) + '/' + str(M))
+                # R_K = np.linalg.matrix_rank(K_H, tol=None, hermitian=True)
+                Psi_P, Lambda_P = switch_eigs(K_H, R_K, eig_solver) #svds_RND(K_H, R_K)  # Diagonalize scale
+                if np.shape(Psi_M)[0]==0: # if this is the first contribute to the basis
+                 Psi_M=Psi_P; Lambda_M=Lambda_P
+                else:                    
+                 Psi_M = np.concatenate((Psi_M, Psi_P), axis=1)  # append to the previous
+                 Lambda_M = np.concatenate((Lambda_M, Lambda_P), axis=0)
+            else:
+                print('\n Scale '+str(m)+' jumped (keep['+str(m)+']=0)')  
+      
+        else: # this is the case m=M: this is a high pass
+            if Keep[m] == 1:
+                print('Working on Scale '+str(m)+'/'+str(M))
+                # This is the 1d Kernel for High Pass (last scale)
+                h1d_H = firwin(Nf[m], F_Bank_r[m], pass_zero=False)
+                F_CUT1 = F_Bank_r[m] * Fs / 2
+                Indices = np.argwhere((np.abs(Freqs) > F_CUT1))
+                R_K = len(Indices)
+                R_K = np.min([len(Indices), SAT])  # number of frequencies here
+                print(str(len(Indices)) + ' Modes Estimated')
+                print('Filtering H Scale ' + str(m + 1) + '/ ' + str(M))
+                K_H = conv_m(K, h1d_H, Ex, boundaries)
+                # Ks[:, :, m + 1] = K_H  # Last (high pass) scale
+                print('Diagonalizing H Scale ' + str(m + 1) + '/ ' + str(M))
+                # R_K = np.linalg.matrix_rank(K_H, tol=None, hermitian=True)
+                Psi_P, Lambda_P = switch_eigs(K_H, R_K, eig_solver) #svds_RND(K_H, R_K)  # Diagonalize scale
+                Psi_M = np.concatenate((Psi_M, Psi_P), axis=1)  # append to the previous
+                Lambda_M = np.concatenate((Lambda_M, Lambda_P), axis=0)
+            else:
+                print('\n Scale '+str(m)+' jumped (keep['+str(m)+']=0)')  
+
+    # Now Order the Scales
+    Indices = np.flip(np.argsort(Lambda_M))  # find indices for sorting in decreasing order
+    Psi_M = Psi_M[:, Indices]  # Sort the temporal structures
+    #print(f"Size psis in mpodtime = {np.shape(Psi_M)}")
+    # Now we complete the basis via re-orghotonalization
+    print('\n QR Polishing...')
+    PSI_M, R = np.linalg.qr(Psi_M, mode=MODE)
+    print('Done!')
+
+    if MEMORY_SAVING:
+        os.makedirs(FOLDER_OUT + '/mPOD', exist_ok=True)
+        np.savez(FOLDER_OUT + '/mPOD/Psis', Psis=PSI_M)
+    
+    return PSI_M[:,0:n_Modes]
```

### Comparing `modulo_vki-2.0.4/modulo_vki/core/_pod_space.py` & `modulo_vki-2.0.5/modulo_vki/core/_pod_space.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-import math
-import numpy as np
-from tqdm import tqdm
-import os
-
-
-def Spatial_basis_POD(D, PSI_P, Sigma_P, MEMORY_SAVING, N_T, FOLDER_OUT='./', N_PARTITIONS=1, SAVE_SPATIAL_POD=False,
-                      rescale=False):
-    """
-    This function computs the POD spatial basis from the temporal basis,
-
-    :param D: np.array. 
-         matrix on which to project the temporal basis
-    :param PSI_P: np.array. 
-          POD's Psis
-    :param Sigma_P: np.array. 
-          POD's Sigmas
-    :param MEMORY_SAVING: bool. 
-         Inherited from main class, if True turns on the MEMORY_SAVING feature, loading the partitions and starting the proper algorithm          
-    :param N_T: int. 
-         Number of temporal snapshots
-    :param FOLDER_OUT: str. 
-         Folder in which the results are saved if SAVE_SPATIAL_POD = True
-    :param N_PARTITIONS: int. 
-         Number of partitions to be loaded. If D has been partitioned using MODULO, this parameter is automatically inherited from the main class. To be specified otherwise.
-
-    :param SAVE_SPATIAL_POD: bool. 
-         If True, results are saved on disk and released from memory
-
-    :param rescale: bool. 
-          If False, the Sigmas are used for the normalization. If True, these are ignored and the normalization is carried out.
-          For the standard POD, False is the way to go. 
-          However, for other decompositions (eg. the SPOD_s) you must use rescale=True                        
-
-    :return Phi_P: np.array. 
-          POD's Phis
-    """
-
-    R = PSI_P.shape[1]
-
-    if not MEMORY_SAVING:
-        N_S = D.shape[0]
-
-        if rescale:
-            # The following is the general normalization approach.
-            # not needed for POD for required for SPOD
-            Phi_P = np.zeros((N_S, R))
-            # N_S = D.shape[0] unused variable
-            PHI_P_SIGMA_P = np.dot(D, PSI_P)
-            print("Completing Spatial Structures Modes: \n")
-
-            for i in tqdm(range(0, R)):
-                # Normalize the columns of C to get spatial modes
-                Phi_P[:, i] = PHI_P_SIGMA_P[:, i] / Sigma_P[i]
-
-        else:
-            # We take only the first R modes.
-            Sigma_P_t = Sigma_P[0:R];
-            Sigma_P_Inv_V = 1 / Sigma_P_t
-            # So we have the inverse
-            Sigma_P_Inv = np.diag(Sigma_P_Inv_V)
-            # Here is the one shot projection:
-            Phi_P = np.linalg.multi_dot([D, PSI_P[:, 0:R], Sigma_P_Inv])
-
-            if SAVE_SPATIAL_POD:
-                os.makedirs(FOLDER_OUT + 'POD', exist_ok=True)
-                np.savez(FOLDER_OUT + '/POD/pod_spatial_basis', phis=Phi_P)
-                # removed PHI_P_SIGMA_P=PHI_P_SIGMA_P, not present if not rescale and not needed (?)
-
-        return Phi_P
-
-    else:
-
-        N_S = np.shape(np.load(FOLDER_OUT + "/data_partitions/di_1.npz")['di'])[0]
-        dim_col = math.floor(N_T / N_PARTITIONS)
-        dim_row = math.floor(N_S / N_PARTITIONS)
-        dr = np.zeros((dim_row, N_T))
-
-        # 1 -- Converting partitions dC to dR
-        if N_S % N_PARTITIONS != 0:
-            tot_blocks_row = N_PARTITIONS + 1
-        else:
-            tot_blocks_row = N_PARTITIONS
-
-        if N_T % N_PARTITIONS != 0:
-            tot_blocks_col = N_PARTITIONS + 1
-        else:
-            tot_blocks_col = N_PARTITIONS
-
-        # --- Loading Psi_P
-        fixed = 0
-        R1 = 0
-        R2 = 0
-        C1 = 0
-        C2 = 0
-
-        for i in range(1, tot_blocks_row + 1):
-
-            if (i == tot_blocks_row) and (N_S - dim_row * N_PARTITIONS > 0):
-                dim_row_fix = N_S - dim_row * N_PARTITIONS
-                dr = np.zeros((dim_row_fix, N_T))
-
-            for b in range(1, tot_blocks_col + 1):
-                di = np.load(FOLDER_OUT + f"/data_partitions/di_{b}.npz")['di']
-                if (i == tot_blocks_row) and (N_S - dim_row * N_PARTITIONS > 0) and fixed == 0:
-                    R1 = R2
-                    R2 = R1 + (N_S - dim_row * N_PARTITIONS)
-                    fixed = 1
-                elif fixed == 0:
-                    R1 = (i - 1) * dim_row
-                    R2 = i * dim_row
-
-                if (b == tot_blocks_col) and (N_T - dim_col * N_PARTITIONS > 0):
-                    C1 = C2
-                    C2 = C1 + (N_T - dim_col * N_PARTITIONS)
-                else:
-                    C1 = (b - 1) * dim_col
-                    C2 = b * dim_col
-
-                np.copyto(dr[:, C1:C2], di[R1:R2, :])
-
-            PHI_SIGMA_BLOCK = np.dot(dr, PSI_P)
-            np.savez(FOLDER_OUT + f"/POD/PHI_SIGMA_{i}",
-                     phi_sigma=PHI_SIGMA_BLOCK)
-
-        # 3 - Converting partitions R to partitions C and get Sigmas
-        dim_col = math.floor(R / N_PARTITIONS)
-        dim_row = math.floor(N_S / N_PARTITIONS)
-        dps = np.zeros((N_S, dim_col))
-        Phi_P = np.zeros((N_S, R))
-
-        if R % N_PARTITIONS != 0:
-            tot_blocks_col = N_PARTITIONS + 1
-        else:
-            tot_blocks_col = N_PARTITIONS
-
-        fixed = 0
-
-        for i in range(1, tot_blocks_col + 1):
-
-            if (i == tot_blocks_col) and (R - dim_col * N_PARTITIONS > 0):
-                dim_col_fix = R - dim_col * N_PARTITIONS
-                dps = np.zeros((N_S, dim_col_fix))
-
-            for b in range(1, tot_blocks_row + 1):
-
-                PHI_SIGMA_BLOCK = np.load(FOLDER_OUT + f"/POD/PHI_SIGMA_{b}.npz")['phi_sigma']
-
-                if (i == tot_blocks_col) and (R - dim_col * N_PARTITIONS > 0) and fixed == 0:
-                    R1 = R2
-                    R2 = R1 + (R - dim_col * N_PARTITIONS)
-                    fixed = 1
-                elif fixed == 0:
-                    R1 = (i - 1) * dim_col
-                    R2 = i * dim_col
-
-                if (b == tot_blocks_col) and (N_S - dim_row * N_PARTITIONS > 0):
-                    C1 = C2
-                    C2 = C1 + (N_S - dim_row * N_PARTITIONS)
-                else:
-                    C1 = (b - 1) * dim_row
-                    C2 = b * dim_row
-
-                dps[C1:C2, :] = PHI_SIGMA_BLOCK[:, R1:R2]
-
-            # Computing Sigmas and Phis
-            if rescale:
-                for j in range(R1, R2):
-                    jj = j - R1
-                    Sigma_P[jj] = np.linalg.norm(dps[:, jj])
-                    Phi_P = dps[:, jj] / Sigma_P[jj]
-                    np.savez(FOLDER_OUT + f"/POD/phi_{j + 1}", phi_p=Phi_P)
-            else:
-                for j in range(R1, R2):
-                    jj = j - R1
-                    Phi_P = dps[:, jj] / Sigma_P[jj]
-                    np.savez(FOLDER_OUT + f"/POD/phi_{j + 1}", phi_p=Phi_P)
-
-        Phi_P_M = np.zeros((N_S, R))
-        for j in range(R):
-            Phi_P_V = np.load(FOLDER_OUT + f"/POD/phi_{j + 1}.npz")['phi_p']
-            Phi_P_M[:, j] = Phi_P_V
-
-        return Phi_P_M
+import math
+import numpy as np
+from tqdm import tqdm
+import os
+
+
+def Spatial_basis_POD(D, PSI_P, Sigma_P, MEMORY_SAVING, N_T, FOLDER_OUT='./', N_PARTITIONS=1, SAVE_SPATIAL_POD=False,
+                      rescale=False):
+    """
+    This function computs the POD spatial basis from the temporal basis,
+
+    :param D: np.array. 
+         matrix on which to project the temporal basis
+    :param PSI_P: np.array. 
+          POD's Psis
+    :param Sigma_P: np.array. 
+          POD's Sigmas
+    :param MEMORY_SAVING: bool. 
+         Inherited from main class, if True turns on the MEMORY_SAVING feature, loading the partitions and starting the proper algorithm          
+    :param N_T: int. 
+         Number of temporal snapshots
+    :param FOLDER_OUT: str. 
+         Folder in which the results are saved if SAVE_SPATIAL_POD = True
+    :param N_PARTITIONS: int. 
+         Number of partitions to be loaded. If D has been partitioned using MODULO, this parameter is automatically inherited from the main class. To be specified otherwise.
+
+    :param SAVE_SPATIAL_POD: bool. 
+         If True, results are saved on disk and released from memory
+
+    :param rescale: bool. 
+          If False, the Sigmas are used for the normalization. If True, these are ignored and the normalization is carried out.
+          For the standard POD, False is the way to go. 
+          However, for other decompositions (eg. the SPOD_s) you must use rescale=True                        
+
+    :return Phi_P: np.array. 
+          POD's Phis
+    """
+
+    R = PSI_P.shape[1]
+
+    if not MEMORY_SAVING:
+        N_S = D.shape[0]
+
+        if rescale:
+            # The following is the general normalization approach.
+            # not needed for POD for required for SPOD
+            Phi_P = np.zeros((N_S, R))
+            # N_S = D.shape[0] unused variable
+            PHI_P_SIGMA_P = np.dot(D, PSI_P)
+            print("Completing Spatial Structures Modes: \n")
+
+            for i in tqdm(range(0, R)):
+                # Normalize the columns of C to get spatial modes
+                Phi_P[:, i] = PHI_P_SIGMA_P[:, i] / Sigma_P[i]
+
+        else:
+            # We take only the first R modes.
+            Sigma_P_t = Sigma_P[0:R];
+            Sigma_P_Inv_V = 1 / Sigma_P_t
+            # So we have the inverse
+            Sigma_P_Inv = np.diag(Sigma_P_Inv_V)
+            # Here is the one shot projection:
+            Phi_P = np.linalg.multi_dot([D, PSI_P[:, 0:R], Sigma_P_Inv])
+
+            if SAVE_SPATIAL_POD:
+                os.makedirs(FOLDER_OUT + 'POD', exist_ok=True)
+                np.savez(FOLDER_OUT + '/POD/pod_spatial_basis', phis=Phi_P)
+                # removed PHI_P_SIGMA_P=PHI_P_SIGMA_P, not present if not rescale and not needed (?)
+
+        return Phi_P
+
+    else:
+
+        N_S = np.shape(np.load(FOLDER_OUT + "/data_partitions/di_1.npz")['di'])[0]
+        dim_col = math.floor(N_T / N_PARTITIONS)
+        dim_row = math.floor(N_S / N_PARTITIONS)
+        dr = np.zeros((dim_row, N_T))
+
+        # 1 -- Converting partitions dC to dR
+        if N_S % N_PARTITIONS != 0:
+            tot_blocks_row = N_PARTITIONS + 1
+        else:
+            tot_blocks_row = N_PARTITIONS
+
+        if N_T % N_PARTITIONS != 0:
+            tot_blocks_col = N_PARTITIONS + 1
+        else:
+            tot_blocks_col = N_PARTITIONS
+
+        # --- Loading Psi_P
+        fixed = 0
+        R1 = 0
+        R2 = 0
+        C1 = 0
+        C2 = 0
+
+        for i in range(1, tot_blocks_row + 1):
+
+            if (i == tot_blocks_row) and (N_S - dim_row * N_PARTITIONS > 0):
+                dim_row_fix = N_S - dim_row * N_PARTITIONS
+                dr = np.zeros((dim_row_fix, N_T))
+
+            for b in range(1, tot_blocks_col + 1):
+                di = np.load(FOLDER_OUT + f"/data_partitions/di_{b}.npz")['di']
+                if (i == tot_blocks_row) and (N_S - dim_row * N_PARTITIONS > 0) and fixed == 0:
+                    R1 = R2
+                    R2 = R1 + (N_S - dim_row * N_PARTITIONS)
+                    fixed = 1
+                elif fixed == 0:
+                    R1 = (i - 1) * dim_row
+                    R2 = i * dim_row
+
+                if (b == tot_blocks_col) and (N_T - dim_col * N_PARTITIONS > 0):
+                    C1 = C2
+                    C2 = C1 + (N_T - dim_col * N_PARTITIONS)
+                else:
+                    C1 = (b - 1) * dim_col
+                    C2 = b * dim_col
+
+                np.copyto(dr[:, C1:C2], di[R1:R2, :])
+
+            PHI_SIGMA_BLOCK = np.dot(dr, PSI_P)
+            np.savez(FOLDER_OUT + f"/PHI_SIGMA_{i}",
+                     phi_sigma=PHI_SIGMA_BLOCK)
+
+        # 3 - Converting partitions R to partitions C and get Sigmas
+        dim_col = math.floor(R / N_PARTITIONS)
+        dim_row = math.floor(N_S / N_PARTITIONS)
+        dps = np.zeros((N_S, dim_col))
+        Phi_P = np.zeros((N_S, R))
+
+        if R % N_PARTITIONS != 0:
+            tot_blocks_col = N_PARTITIONS + 1
+        else:
+            tot_blocks_col = N_PARTITIONS
+
+        fixed = 0
+
+        for i in range(1, tot_blocks_col + 1):
+
+            if (i == tot_blocks_col) and (R - dim_col * N_PARTITIONS > 0):
+                dim_col_fix = R - dim_col * N_PARTITIONS
+                dps = np.zeros((N_S, dim_col_fix))
+
+            for b in range(1, tot_blocks_row + 1):
+
+                PHI_SIGMA_BLOCK = np.load(FOLDER_OUT + f"/PHI_SIGMA_{b}.npz")['phi_sigma']
+
+                if (i == tot_blocks_col) and (R - dim_col * N_PARTITIONS > 0) and fixed == 0:
+                    R1 = R2
+                    R2 = R1 + (R - dim_col * N_PARTITIONS)
+                    fixed = 1
+                elif fixed == 0:
+                    R1 = (i - 1) * dim_col
+                    R2 = i * dim_col
+
+                if (b == tot_blocks_col) and (N_S - dim_row * N_PARTITIONS > 0):
+                    C1 = C2
+                    C2 = C1 + (N_S - dim_row * N_PARTITIONS)
+                else:
+                    C1 = (b - 1) * dim_row
+                    C2 = b * dim_row
+
+                dps[C1:C2, :] = PHI_SIGMA_BLOCK[:, R1:R2]
+
+            # Computing Sigmas and Phis
+            if rescale:
+                for j in range(R1, R2):
+                    jj = j - R1
+                    Sigma_P[jj] = np.linalg.norm(dps[:, jj])
+                    Phi_P = dps[:, jj] / Sigma_P[jj]
+                    np.savez(FOLDER_OUT + f"/phi_{j + 1}", phi_p=Phi_P)
+            else:
+                for j in range(R1, R2):
+                    jj = j - R1
+                    Phi_P = dps[:, jj] / Sigma_P[jj]
+                    np.savez(FOLDER_OUT + f"/phi_{j + 1}", phi_p=Phi_P)
+
+        Phi_P_M = np.zeros((N_S, R))
+        for j in range(R):
+            Phi_P_V = np.load(FOLDER_OUT + f"/phi_{j + 1}.npz")['phi_p']
+            Phi_P_M[:, j] = Phi_P_V
+
+        return Phi_P_M
```

### Comparing `modulo_vki-2.0.4/modulo_vki/core/_pod_time.py` & `modulo_vki-2.0.5/modulo_vki/core/_pod_time.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import os
-import numpy as np
-from ..utils._utils import switch_eigs
-
-
-def Temporal_basis_POD(K, SAVE_T_POD=False, FOLDER_OUT='./', n_Modes=10,eig_solver: str = 'eigh'):
-    """
-    This method computes the POD basis. For some theoretical insights, you can find the theoretical background of the proper orthogonal decomposition in a nutshell here: https://youtu.be/8fhupzhAR_M
-
-    :param FOLDER_OUT: str. Folder in which the results will be saved (if SAVE_T_POD=True)
-    :param K: np.array. Temporal correlation matrix
-    :param SAVE_T_POD: bool. A flag deciding whether the results are saved on disk or not. If the MEMORY_SAVING feature is active, it is switched True by default.
-    :param n_Modes: int. Number of modes that will be computed
-    :param svd_solver: str. Svd solver to be used throughout the computation
-    :return: Psi_P: np.array. POD's Psis
-    :return: Sigma_P: np.array. POD's Sigmas
-    """
-    # Solver 1: Use the standard SVD
-    # Psi_P, Lambda_P, _ = np.linalg.svd(K)
-    # Sigma_P = np.sqrt(Lambda_P)
-
-    # Solver 2: Use randomized SVD ############## WARNING #################
-    # if svd_solver.lower() == 'svd_sklearn_truncated':
-    #     svd = TruncatedSVD(n_Modes)
-    #     svd.fit_transform(K)
-    #     Psi_P = svd.components_.T
-    #     Lambda_P = svd.singular_values_
-    #     Sigma_P = np.sqrt(Lambda_P)
-    # elif svd_solver.lower() == 'svd_numpy':
-    #     Psi_P, Lambda_P, _ = np.linalg.svd(K)
-    #     Sigma_P = np.sqrt(Lambda_P)
-    # elif svd_solver.lower() == 'svd_sklearn_randomized':
-    #     Psi_P, Lambda_P, _ = svds_RND(K, n_Modes)
-    #     Sigma_P = np.sqrt(Lambda_P)
-    # elif svd_solver.lower() == 'svd_scipy_sparse':
-    #     Psi_P, Lambda_P, _ = svds(K, k=n_Modes)
-    #     Sigma_P = np.sqrt(Lambda_P)
-
-    print("diagonalizing K....")
-    Psi_P, Sigma_P = switch_eigs(K, n_Modes, eig_solver)
-    
-
-    if SAVE_T_POD:
-        os.makedirs(FOLDER_OUT + "/POD/", exist_ok=True)
-        print("Saving POD temporal basis")
-        np.savez(FOLDER_OUT + '/POD/temporal_basis', Psis=Psi_P, Sigmas=Sigma_P)
-
-    return Psi_P, Sigma_P
+import os
+import numpy as np
+from ..utils._utils import switch_eigs
+
+
+def Temporal_basis_POD(K, SAVE_T_POD=False, FOLDER_OUT='./', n_Modes=10,eig_solver: str = 'eigh'):
+    """
+    This method computes the POD basis. For some theoretical insights, you can find the theoretical background of the proper orthogonal decomposition in a nutshell here: https://youtu.be/8fhupzhAR_M
+
+    :param FOLDER_OUT: str. Folder in which the results will be saved (if SAVE_T_POD=True)
+    :param K: np.array. Temporal correlation matrix
+    :param SAVE_T_POD: bool. A flag deciding whether the results are saved on disk or not. If the MEMORY_SAVING feature is active, it is switched True by default.
+    :param n_Modes: int. Number of modes that will be computed
+    :param svd_solver: str. Svd solver to be used throughout the computation
+    :return: Psi_P: np.array. POD's Psis
+    :return: Sigma_P: np.array. POD's Sigmas
+    """
+    # Solver 1: Use the standard SVD
+    # Psi_P, Lambda_P, _ = np.linalg.svd(K)
+    # Sigma_P = np.sqrt(Lambda_P)
+
+    # Solver 2: Use randomized SVD ############## WARNING #################
+    # if svd_solver.lower() == 'svd_sklearn_truncated':
+    #     svd = TruncatedSVD(n_Modes)
+    #     svd.fit_transform(K)
+    #     Psi_P = svd.components_.T
+    #     Lambda_P = svd.singular_values_
+    #     Sigma_P = np.sqrt(Lambda_P)
+    # elif svd_solver.lower() == 'svd_numpy':
+    #     Psi_P, Lambda_P, _ = np.linalg.svd(K)
+    #     Sigma_P = np.sqrt(Lambda_P)
+    # elif svd_solver.lower() == 'svd_sklearn_randomized':
+    #     Psi_P, Lambda_P, _ = svds_RND(K, n_Modes)
+    #     Sigma_P = np.sqrt(Lambda_P)
+    # elif svd_solver.lower() == 'svd_scipy_sparse':
+    #     Psi_P, Lambda_P, _ = svds(K, k=n_Modes)
+    #     Sigma_P = np.sqrt(Lambda_P)
+
+    print("diagonalizing K....")
+    Psi_P, Sigma_P = switch_eigs(K, n_Modes, eig_solver)
+    
+
+    if SAVE_T_POD:
+        os.makedirs(FOLDER_OUT + "/POD/", exist_ok=True)
+        print("Saving POD temporal basis")
+        np.savez(FOLDER_OUT + '/POD/temporal_basis', Psis=Psi_P, Sigmas=Sigma_P)
+
+    return Psi_P, Sigma_P
```

### Comparing `modulo_vki-2.0.4/modulo_vki/core/_spod_s.py` & `modulo_vki-2.0.5/modulo_vki/core/_spod_s.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-import numpy as np
-from scipy import signal
-from scipy.signal import firwin
-from ._pod_time import Temporal_basis_POD
-from ._pod_space import Spatial_basis_POD
-
-def compute_SPOD_s(D, K, F_S, n_s, n_t,N_o=100, f_c=0.3,n_Modes=10, SAVE_SPOD=True,
-                   FOLDER_OUT='./', MEMORY_SAVING=False, N_PARTITIONS=1):
-    """
-    This method computes the Spectral POD of your data.
-    This is the one by Sieber
-    et al (https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/abs/spectral-proper-orthogonal-decomposition/DCD8A6EDEFD56F5A9715DBAD38BD461A)
-
-    :param F_S: float,
-           Sampling Frequency [Hz]
-    :param N_o: float,
-           Semi-Order of the diagonal filter.
-           Note that the filter order will be 2 N_o +1 (to make sure it is odd)
-    :param f_c: float,
-           cut-off frequency of the diagonal filter
-    :param n_Modes: float,
-           number of modes to be computed
-    :param SAVE_SPOD: bool,
-           If True, MODULO will save the output in self.FOLDER OUT/MODULO_tmp
-    :param FOLDER_OUT: string
-           Define where the out will be stored (ignored if SAVE_POD=False)
-    :param MEMORY SAVING: bool
-           Define if memory saving is active or not (reduntant; to be improved)
-           Currently left for compatibility with the rest of MODULO.
-    :param N_PARTITIONS: int
-           number of partitions (if memory saving = False, it should be 1). 
-           (reduntant; to be improved)
-           Currently left for compatibility with the rest of MODULO.           
-    :return Psi_P: np.array
-           SPOD Psis
-    :return Sigma_P: np.array
-           SPOD Sigmas.
-    :return Phi_P: np.array
-            SPOD Phis
-    """
-    # if self.D is None:
-    #     D = np.load(self.FOLDER_OUT + '/MODULO_tmp/data_matrix/database.npz')['D']
-    #     SAVE_SPOD = True
-    #     # TODO : Lorenzo check this stuff
-    # else:
-    #     D = self.D
-    #
-    # n_s = self.N_S  # Repeat variable for debugging compatibility
-    # n_t = self.N_T
-    #
-    # print('Computing Correlation Matrix \n')
-
-    # The first step is the same as the POD: we compute the correlation matrix
-    # K = CorrelationMatrix(self.N_T, self.N_PARTITIONS, self.MEMORY_SAVING,
-    #                       self.FOLDER_OUT, D=self.D)
-
-    # 1. Initialize the extended
-    K_e = np.zeros((n_t + 2 * N_o, n_t + 2 * N_o))
-    # From which we clearly know that:
-    K_e[N_o:n_t + N_o, N_o:n_t + N_o] = K
-
-    # 2. We fill the edges ( a bit of repetition but ok.. )
-
-    # Row-wise, Upper part
-    for i in range(0, N_o):
-        K_e[i, i:i + n_t] = K[0, :]
-
-    # Row-wise, bottom part
-    for i in range(N_o + n_t, n_t + 2 * N_o):
-        K_e[i, i - n_t + 1:i + 1] = K[-1, :]
-
-        # Column-wise, left part
-    for j in range(0, N_o):
-        K_e[j:j + n_t, j] = K[:, 0]
-
-        # Column-wise, right part
-    for j in range(N_o + n_t, 2 * N_o + n_t):
-        K_e[j - n_t + 1:j + 1, j] = K[:, -1]
-
-    # Now you create the diagonal kernel in 2D
-    h_f = firwin(N_o, f_c)  # Kernel in 1D
-    # This is also something that must be put in a separate file:
-    # To cancel the phase lag we make this non-causal with a symmetric
-    # shift, hence with zero padding as equal as possible on both sides
-    n_padd_l = round((n_t - N_o) / 2);
-    n_padd_r = n_t - N_o - n_padd_l
-
-    h_f_pad = np.pad(h_f, (n_padd_l, n_padd_r))  # symmetrically padded kernel in 1D
-    h_f_2 = np.diag(h_f_pad)
-
-    # Finally the filtered K is just
-    K_F = signal.fftconvolve(K_e, h_f_2, mode='same')[N_o:n_t + N_o, N_o:n_t + N_o]
-    # plt.plot(np.diag(K),'b--'); plt.plot(np.diag(K_F_e),'r')
-
-    # From now on it's just POD:
-    Psi_P, Sigma_P = Temporal_basis_POD(K_F, SAVE_SPOD, FOLDER_OUT, n_Modes)
-    # but with a normalization aspect to be careful about!  
-    Phi_P = Spatial_basis_POD(D, N_T=n_t, PSI_P=Psi_P, Sigma_P=Sigma_P,
-                              MEMORY_SAVING=MEMORY_SAVING, FOLDER_OUT=FOLDER_OUT,
-                              N_PARTITIONS=N_PARTITIONS,rescale=True)
-
+import numpy as np
+from scipy import signal
+from scipy.signal import firwin
+from ._pod_time import Temporal_basis_POD
+from ._pod_space import Spatial_basis_POD
+
+def compute_SPOD_s(D, K, F_S, n_s, n_t,N_o=100, f_c=0.3,n_Modes=10, SAVE_SPOD=True,
+                   FOLDER_OUT='./', MEMORY_SAVING=False, N_PARTITIONS=1):
+    """
+    This method computes the Spectral POD of your data.
+    This is the one by Sieber
+    et al (https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/abs/spectral-proper-orthogonal-decomposition/DCD8A6EDEFD56F5A9715DBAD38BD461A)
+
+    :param F_S: float,
+           Sampling Frequency [Hz]
+    :param N_o: float,
+           Semi-Order of the diagonal filter.
+           Note that the filter order will be 2 N_o +1 (to make sure it is odd)
+    :param f_c: float,
+           cut-off frequency of the diagonal filter
+    :param n_Modes: float,
+           number of modes to be computed
+    :param SAVE_SPOD: bool,
+           If True, MODULO will save the output in self.FOLDER OUT/MODULO_tmp
+    :param FOLDER_OUT: string
+           Define where the out will be stored (ignored if SAVE_POD=False)
+    :param MEMORY SAVING: bool
+           Define if memory saving is active or not (reduntant; to be improved)
+           Currently left for compatibility with the rest of MODULO.
+    :param N_PARTITIONS: int
+           number of partitions (if memory saving = False, it should be 1). 
+           (reduntant; to be improved)
+           Currently left for compatibility with the rest of MODULO.           
+    :return Psi_P: np.array
+           SPOD Psis
+    :return Sigma_P: np.array
+           SPOD Sigmas.
+    :return Phi_P: np.array
+            SPOD Phis
+    """
+    # if self.D is None:
+    #     D = np.load(self.FOLDER_OUT + '/MODULO_tmp/data_matrix/database.npz')['D']
+    #     SAVE_SPOD = True
+    #     # TODO : Lorenzo check this stuff
+    # else:
+    #     D = self.D
+    #
+    # n_s = self.N_S  # Repeat variable for debugging compatibility
+    # n_t = self.N_T
+    #
+    # print('Computing Correlation Matrix \n')
+
+    # The first step is the same as the POD: we compute the correlation matrix
+    # K = CorrelationMatrix(self.N_T, self.N_PARTITIONS, self.MEMORY_SAVING,
+    #                       self.FOLDER_OUT, D=self.D)
+
+    # 1. Initialize the extended
+    K_e = np.zeros((n_t + 2 * N_o, n_t + 2 * N_o))
+    # From which we clearly know that:
+    K_e[N_o:n_t + N_o, N_o:n_t + N_o] = K
+
+    # 2. We fill the edges ( a bit of repetition but ok.. )
+
+    # Row-wise, Upper part
+    for i in range(0, N_o):
+        K_e[i, i:i + n_t] = K[0, :]
+
+    # Row-wise, bottom part
+    for i in range(N_o + n_t, n_t + 2 * N_o):
+        K_e[i, i - n_t + 1:i + 1] = K[-1, :]
+
+        # Column-wise, left part
+    for j in range(0, N_o):
+        K_e[j:j + n_t, j] = K[:, 0]
+
+        # Column-wise, right part
+    for j in range(N_o + n_t, 2 * N_o + n_t):
+        K_e[j - n_t + 1:j + 1, j] = K[:, -1]
+
+    # Now you create the diagonal kernel in 2D
+    h_f = firwin(N_o, f_c)  # Kernel in 1D
+    # This is also something that must be put in a separate file:
+    # To cancel the phase lag we make this non-causal with a symmetric
+    # shift, hence with zero padding as equal as possible on both sides
+    n_padd_l = round((n_t - N_o) / 2);
+    n_padd_r = n_t - N_o - n_padd_l
+
+    h_f_pad = np.pad(h_f, (n_padd_l, n_padd_r))  # symmetrically padded kernel in 1D
+    h_f_2 = np.diag(h_f_pad)
+
+    # Finally the filtered K is just
+    K_F = signal.fftconvolve(K_e, h_f_2, mode='same')[N_o:n_t + N_o, N_o:n_t + N_o]
+    # plt.plot(np.diag(K),'b--'); plt.plot(np.diag(K_F_e),'r')
+
+    # From now on it's just POD:
+    Psi_P, Sigma_P = Temporal_basis_POD(K_F, SAVE_SPOD, FOLDER_OUT, n_Modes)
+    # but with a normalization aspect to be careful about!  
+    Phi_P = Spatial_basis_POD(D, N_T=n_t, PSI_P=Psi_P, Sigma_P=Sigma_P,
+                              MEMORY_SAVING=MEMORY_SAVING, FOLDER_OUT=FOLDER_OUT,
+                              N_PARTITIONS=N_PARTITIONS,rescale=True)
+
     return Phi_P, Psi_P, Sigma_P
```

### Comparing `modulo_vki-2.0.4/modulo_vki/core/_spod_t.py` & `modulo_vki-2.0.5/modulo_vki/core/_spod_t.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-import numpy as np
-from modulo_vki.utils._utils import overlap
-from tqdm import tqdm
-import os
-
-from modulo_vki.utils._utils import switch_svds
-
-
-
-def compute_SPOD_t(D, F_S, L_B=500, O_B=250,n_Modes=10, SAVE_SPOD=True, FOLDER_OUT='/',
-                   possible_svds='svd_sklearn_truncated'):
-    """
-    This method computes the Spectral POD of your data.
-    This is the one by Town 
-    et al (https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/spectral-proper-orthogonal-decomposition-and-its-relationship-to-dynamic-mode-decomposition-and-resolvent-analysis/EC2A6DF76490A0B9EB208CC2CA037717)
-    
-    :param D: array.
-      snapshot matrix to decompose, of size N_S,N_T 
-    :param F_S: float,
-      Sampling Frequency [Hz]
-    :param L_B: float,
-      Lenght of the chunks
-    :param O_B: float,
-      Overlapping between blocks in the chunk
-    :param n_Modes: float,
-      Number of modes to be computed FOR EACH FREQUENCY
-    :param SAVE_SPOD: bool,
-      If True, MODULO will save the output in FOLDER OUT/MODULO_tmp
-    :param possible_svds: str,      
-      Svd solver to be used throughout the computation
-           
-    :return Psi_P_hat: np.array
-      Spectra of the SPOD Modes
-    :return Sigma_P: np.array
-      Amplitudes of the SPOD Modes.
-    :return Phi_P: np.array
-      SPOD Phis
-    :return freq: float
-      Frequency bins for the Spectral POD
-    """
-        
-    # if D is None:
-    #     D = np.load(FOLDER_OUT + '/MODULO_tmp/data_matrix/database.npz')['D']
-    #     SAVE_SPOD = True
-    # else:
-    #     D = D
-    #
-    # n_s = N_S  # Repeat variable for debugging compatibility
-    # n_t = N_T
-    #
-    # # First comput the PS in each point (this is very time consuming and should be parallelized)
-    # # Note: this can be improved a lot...! ok for the moment
-    print('Computing PSD at all points\n')
-    N_S,N_T=np.shape(D)
-
-    # Step 1 : Partition the data into blocks ( potentially overlapping)
-    Ind = np.arange(N_T)
-    Indices = overlap(Ind, len_chunk=L_B, len_sep=O_B)
-
-    N_B = np.shape(Indices)[1]
-    N_P = np.shape(Indices)[0]
-    print('Partitioned into blocks of length n_B=' + str(N_B))
-    print('Number of partitions retained is n_P=' + str(N_P))
-
-    # The frequency bins are thus defined:
-    Freqs = np.fft.fftfreq(N_B) * F_S  # Compute the frequency bins
-    Keep_IND = np.where(Freqs >= 0)
-    N_B2 = len(Keep_IND[0])  # indexes for positive frequencies
-    Freqs_Pos = Freqs[Keep_IND]  # positive frequencies
-
-    # Step 2 : Construct the D_hats in each partition
-    D_P_hat_Tens = np.zeros((N_S, N_B, N_P))
-    print('Computing DFTs in each partition')
-    for k in tqdm(range(0, N_P)):  # Loop over the partitions
-        D_p = D[:, Indices[k]]  # Take the portion of data
-        D_P_hat_Tens[:, :, k] = np.fft.fft(D_p, N_B, 1)
-
-    # This would be the mean over the frequencies
-    # D_hat_Mean=np.mean(D_P_hat_Tens,axis=1)
-
-    # Initialize the outputs
-    Sigma_SP = np.zeros((n_Modes, N_B2))
-    Phi_SP = np.zeros((N_S, n_Modes, N_B2))
-
-    # Step 3: Loop over frequencies to build the modes.
-    # Note: you only care about half of these frequencies.
-    # This is why you loop over N_B2, not N_B
-    print('Computing POD for each frequency')
-    for j in tqdm(range(0, N_B2)):
-        # Get D_hat of the chunk
-        D_hat_f = D_P_hat_Tens[:, j, :]
-        # Go for the SVD
- 
-        U,V,Sigma=switch_svds(D_hat_f,n_Modes,svd_solver=possible_svds)
-
-        Phi_SP[:, :, j] = U
-        Sigma_SP[:, j] = Sigma / (N_S * N_B)
-
-    if SAVE_SPOD:
-        folder_dir = FOLDER_OUT + '/SPOD_T'
-        os.makedirs(folder_dir, exist_ok=True)
-        np.savez(folder_dir + '/spod_t.npz', Phi=Phi_SP, Sigma=Sigma_SP, Freqs=Freqs_Pos)
-
-    return Phi_SP, Sigma_SP, Freqs_Pos
+import numpy as np
+from modulo_vki.utils._utils import overlap
+from tqdm import tqdm
+import os
+
+from modulo_vki.utils._utils import switch_svds
+
+
+
+def compute_SPOD_t(D, F_S, L_B=500, O_B=250,n_Modes=10, SAVE_SPOD=True, FOLDER_OUT='/',
+                   possible_svds='svd_sklearn_truncated'):
+    """
+    This method computes the Spectral POD of your data.
+    This is the one by Town 
+    et al (https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/spectral-proper-orthogonal-decomposition-and-its-relationship-to-dynamic-mode-decomposition-and-resolvent-analysis/EC2A6DF76490A0B9EB208CC2CA037717)
+    
+    :param D: array.
+      snapshot matrix to decompose, of size N_S,N_T 
+    :param F_S: float,
+      Sampling Frequency [Hz]
+    :param L_B: float,
+      Lenght of the chunks
+    :param O_B: float,
+      Overlapping between blocks in the chunk
+    :param n_Modes: float,
+      Number of modes to be computed FOR EACH FREQUENCY
+    :param SAVE_SPOD: bool,
+      If True, MODULO will save the output in FOLDER OUT/MODULO_tmp
+    :param possible_svds: str,      
+      Svd solver to be used throughout the computation
+           
+    :return Psi_P_hat: np.array
+      Spectra of the SPOD Modes
+    :return Sigma_P: np.array
+      Amplitudes of the SPOD Modes.
+    :return Phi_P: np.array
+      SPOD Phis
+    :return freq: float
+      Frequency bins for the Spectral POD
+    """
+        
+    # if D is None:
+    #     D = np.load(FOLDER_OUT + '/MODULO_tmp/data_matrix/database.npz')['D']
+    #     SAVE_SPOD = True
+    # else:
+    #     D = D
+    #
+    # n_s = N_S  # Repeat variable for debugging compatibility
+    # n_t = N_T
+    #
+    # # First comput the PS in each point (this is very time consuming and should be parallelized)
+    # # Note: this can be improved a lot...! ok for the moment
+    print('Computing PSD at all points\n')
+    N_S,N_T=np.shape(D)
+
+    # Step 1 : Partition the data into blocks ( potentially overlapping)
+    Ind = np.arange(N_T)
+    Indices = overlap(Ind, len_chunk=L_B, len_sep=O_B)
+
+    N_B = np.shape(Indices)[1]
+    N_P = np.shape(Indices)[0]
+    print('Partitioned into blocks of length n_B=' + str(N_B))
+    print('Number of partitions retained is n_P=' + str(N_P))
+
+    # The frequency bins are thus defined:
+    Freqs = np.fft.fftfreq(N_B) * F_S  # Compute the frequency bins
+    Keep_IND = np.where(Freqs >= 0)
+    N_B2 = len(Keep_IND[0])  # indexes for positive frequencies
+    Freqs_Pos = Freqs[Keep_IND]  # positive frequencies
+
+    # Step 2 : Construct the D_hats in each partition
+    D_P_hat_Tens = np.zeros((N_S, N_B, N_P))
+    print('Computing DFTs in each partition')
+    for k in tqdm(range(0, N_P)):  # Loop over the partitions
+        D_p = D[:, Indices[k]]  # Take the portion of data
+        D_P_hat_Tens[:, :, k] = np.fft.fft(D_p, N_B, 1)
+
+    # This would be the mean over the frequencies
+    # D_hat_Mean=np.mean(D_P_hat_Tens,axis=1)
+
+    # Initialize the outputs
+    Sigma_SP = np.zeros((n_Modes, N_B2))
+    Phi_SP = np.zeros((N_S, n_Modes, N_B2))
+
+    # Step 3: Loop over frequencies to build the modes.
+    # Note: you only care about half of these frequencies.
+    # This is why you loop over N_B2, not N_B
+    print('Computing POD for each frequency')
+    for j in tqdm(range(0, N_B2)):
+        # Get D_hat of the chunk
+        D_hat_f = D_P_hat_Tens[:, j, :]
+        # Go for the SVD
+ 
+        U,V,Sigma=switch_svds(D_hat_f,n_Modes,svd_solver=possible_svds)
+
+        Phi_SP[:, :, j] = U
+        Sigma_SP[:, j] = Sigma / (N_S * N_B)
+
+    if SAVE_SPOD:
+        folder_dir = FOLDER_OUT + '/SPOD_T'
+        os.makedirs(folder_dir, exist_ok=True)
+        np.savez(folder_dir + '/spod_t.npz', Phi=Phi_SP, Sigma=Sigma_SP, Freqs=Freqs_Pos)
+
+    return Phi_SP, Sigma_SP, Freqs_Pos
```

### Comparing `modulo_vki-2.0.4/modulo_vki/utils/_plots.py` & `modulo_vki-2.0.5/modulo_vki/utils/_plots.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import numpy as np
-import matplotlib.pyplot as plt
-from matplotlib.patches import Rectangle
-
-
-def plot_mesh(X, Y, x, y, X_mid, Y_mid):
-    """
-    Plot original mesh and rectangular mesh over original mesh
-    :param X:
-    :param Y:
-    :param x:
-    :param y:
-    :param X_mid:
-    :param Y_mid:
-    :return:
-    """
-    # Plot original mesh
-    fig, ax = plt.subplots()
-    ax.scatter(X, Y, marker='.', color='k')
-    ax.set_title('Original Mesh')
-    ax.set_xlabel('x')
-    ax.set_ylabel('y')
-
-    # Plot rectangular mesh over original mesh
-    fig, ax = plt.subplots(figsize=(10, 8))
-    im = ax.imshow(np.zeros_like(X), cmap='gray', extent=[x.min(), x.max(), y.min(), y.max()], origin='lower')
-    ax.scatter(X, Y, marker='.', color='k')
-    ax.plot(X_mid, Y_mid, '--k', lw=1)
-    ax.plot(X_mid.T, Y_mid.T, '--k', lw=1)
-    ax.set_title('Rectangular Mesh over Original Mesh')
-    ax.set_xlabel('x')
-    ax.set_ylabel('y')
-    fig.colorbar(im)
-    ax.set(xlim=(-1.2, 1.2), ylim=(0.9, 5.3))
-
-    return plt.show()
-
-
-def plot_areas(X_mid, Y_mid, areas):
-    """
-    Plot relative areas of sub-rectangles
-    :param X_mid:
-    :param Y_mid:
-    :param areas:
-    :return:
-    """
-    fig, ax = plt.subplots()
-    ax.pcolormesh(X_mid, Y_mid, areas, cmap='viridis', shading='auto')
-    ax.set_xlabel('x')
-    ax.set_ylabel('y')
-    ax.set_title('Relative areas of sub-rectangles')
+import numpy as np
+import matplotlib.pyplot as plt
+from matplotlib.patches import Rectangle
+
+
+def plot_mesh(X, Y, x, y, X_mid, Y_mid):
+    """
+    Plot original mesh and rectangular mesh over original mesh
+    :param X:
+    :param Y:
+    :param x:
+    :param y:
+    :param X_mid:
+    :param Y_mid:
+    :return:
+    """
+    # Plot original mesh
+    fig, ax = plt.subplots()
+    ax.scatter(X, Y, marker='.', color='k')
+    ax.set_title('Original Mesh')
+    ax.set_xlabel('x')
+    ax.set_ylabel('y')
+
+    # Plot rectangular mesh over original mesh
+    fig, ax = plt.subplots(figsize=(10, 8))
+    im = ax.imshow(np.zeros_like(X), cmap='gray', extent=[x.min(), x.max(), y.min(), y.max()], origin='lower')
+    ax.scatter(X, Y, marker='.', color='k')
+    ax.plot(X_mid, Y_mid, '--k', lw=1)
+    ax.plot(X_mid.T, Y_mid.T, '--k', lw=1)
+    ax.set_title('Rectangular Mesh over Original Mesh')
+    ax.set_xlabel('x')
+    ax.set_ylabel('y')
+    fig.colorbar(im)
+    ax.set(xlim=(-1.2, 1.2), ylim=(0.9, 5.3))
+
+    return plt.show()
+
+
+def plot_areas(X_mid, Y_mid, areas):
+    """
+    Plot relative areas of sub-rectangles
+    :param X_mid:
+    :param Y_mid:
+    :param areas:
+    :return:
+    """
+    fig, ax = plt.subplots()
+    ax.pcolormesh(X_mid, Y_mid, areas, cmap='viridis', shading='auto')
+    ax.set_xlabel('x')
+    ax.set_ylabel('y')
+    ax.set_title('Relative areas of sub-rectangles')
     return plt.show()
```

### Comparing `modulo_vki-2.0.4/modulo_vki/utils/_utils.py` & `modulo_vki-2.0.5/modulo_vki/utils/_utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,340 +1,340 @@
-import numpy as np
-from scipy import signal
-from scipy.sparse.linalg import svds, eigsh
-from sklearn.decomposition import TruncatedSVD
-from scipy.linalg import eigh
-from sklearn.utils.extmath import randomized_svd
-
-
-def Bound_EXT(S, Ex, boundaries):
-    """
-   This function computes the extension of a signal for
-   filtering purposes
-
-   :param S: The Input signal
-   :param Nf: The Size of the Kernel (must be an odd number!)
-   :param boundaries: The type of extension:
-           ‘reflect’ (d c b a | a b c d | d c b a)    The input is extended by reflecting about the edge of the last pixel.
-           ‘nearest’ (a a a a | a b c d | d d d d)    The input is extended by replicating the last pixel.
-           ‘wrap’ (a b c d | a b c d | a b c d)       The input is extended by wrapping around to the opposite edge.
-           ‘extrap’ Extrapolation                     The input is extended via linear extrapolation.
-
-
-   """
-    # We first perform a zero padding
-    # Ex=int((Nf-1)/2) # Extension on each size
-    size_Ext = 2 * Ex + len(S)  # Compute the size of the extended signal
-    S_extend = np.zeros((int(size_Ext)))  # Initialize extended signal
-    S_extend[Ex:int((size_Ext - Ex))] = S;  # Assign the Signal on the zeroes
-
-    if boundaries == "reflect":
-        LEFT = np.flip(S[0:Ex])  # Prepare the reflection on the left
-        RIGHT = np.flip(S[len(S) - Ex:len(S)])  # Prepare the reflectino on the right
-        S_extend[0:Ex] = LEFT
-        S_extend[len(S_extend) - Ex:len(S_extend)] = RIGHT
-    elif boundaries == "nearest":
-        LEFT = np.ones(Ex) * S[0]  # Prepare the constant on the left
-        RIGHT = np.ones(Ex) * S[len(S) - 1]  # Prepare the constant on the Right
-        S_extend[0:Ex] = LEFT
-        S_extend[len(S_extend) - Ex:len(S_extend)] = RIGHT
-    elif boundaries == "wrap":
-        LEFT = S[len(S) - Ex:len(S)]  # Wrap on the Left
-        RIGHT = S[0:Ex]  # Wrap on the Right
-        S_extend[0:Ex] = LEFT
-        S_extend[len(S_extend) - Ex:len(S_extend)] = RIGHT
-    elif boundaries == "extrap":
-        LEFT = np.ones(Ex) * S[0]  # Prepare the constant on the left
-        RIGHT = np.ones(Ex) * S[len(S) - 1]  # Prepare the constant on the Right
-        S_extend[0:Ex] = LEFT
-        S_extend[len(S_extend) - Ex:len(S_extend)] = RIGHT
-        print('Not active yet, replaced by nearest')
-    return S_extend
-
-
-def conv_m(K, h, Ex, boundaries):
-    """
-   This function computes the 2D convolution by perfoming 2 sets of 1D convolutions.
-   Moreover, we here use the fft with an appropriate extension
-   that avoids the periodicity condition.
-
-   :param K: Matrix to be filtered
-   :param h: The 1D Kernel of the filter
-   :param boundaries: The type of extension:
-           ‘reflect’ (d c b a | a b c d | d c b a)    The input is extended by reflecting about the edge of the last pixel.
-           ‘nearest’ (a a a a | a b c d | d d d d)    The input is extended by replicating the last pixel.
-           ‘wrap’ (a b c d | a b c d | a b c d)       The input is extended by wrapping around to the opposite edge.
-           ‘extrap’ Extrapolation                     The input is extended via linear extrapolation.
-   """
-    # Filter along the raws
-    n_t = np.shape(K)[0]
-    # Ex=int(n_t/2)
-    K_F1 = np.zeros(np.shape(K))
-    K_F2 = np.zeros(np.shape(K))
-    # K_F=np.zeros(np.shape(K))
-    for k in range(0, n_t):
-        S = K[:, k]
-        S_Ext = Bound_EXT(S, Ex, boundaries)
-        S_Filt = signal.fftconvolve(S_Ext, h, mode='valid')
-        # Compute where to take the signal
-        Ex1 = int((len(S_Filt) - len(S)) / 2)
-        # K_F1[k,:]=S_Filt[Ex:(len(S_Filt)-Ex)]
-        K_F1[:, k] = S_Filt[Ex1:(len(S_Filt) - Ex1)]
-    for k in range(0, n_t):
-        S = K_F1[k, :]
-        S_Ext = Bound_EXT(S, Ex, boundaries)
-        S_Filt = signal.fftconvolve(S_Ext, h, mode='valid')
-        # Compute where to take the signal
-        Ex1 = int((len(S_Filt) - len(S)) / 2)
-        # K_F2[:,k]=S_Filt[Ex:(len(S_Filt)-Ex)]
-        K_F2[k, :] = S_Filt[Ex1:(len(S_Filt) - Ex1)]
-        # K_F=K_F1+K_F2
-    return K_F2
-
-
-def _loop_gemm(a, b, c=None, chunksize=100):
-    size_i = a.shape[0]
-    size_zip = a.shape[1]
-
-    size_j = b.shape[1]
-    size_alt_zip = b.shape[0]
-
-    if size_zip != size_alt_zip:
-        ValueError("Loop GEMM zip index is not of the same size for both tensors")
-
-    if c is None:
-        c = np.zeros((size_i, size_j))
-
-    istart = 0
-    for i in range(int(np.ceil(size_i / float(chunksize)))):
-
-        left_slice = slice(istart, istart + chunksize)
-        left_view = a[left_slice]
-
-        jstart = 0
-        for j in range(int(np.ceil(size_j / float(chunksize)))):
-            right_slice = slice(jstart, jstart + chunksize)
-            right_view = b[:, right_slice]
-
-            c[left_slice, right_slice] = np.dot(left_view, right_view)
-            jstart += chunksize
-
-        istart += chunksize
-
-    return c
-
-
-def svds_RND(K, R_K):
-    """
-    Quick and dirty implementation of randomized SVD
-    for computing eigenvalues of K. We follow same input/output structure
-    as for the svds in scipy
-    """
-    svd = TruncatedSVD(R_K)
-    svd.fit_transform(K)
-    Psi_P = svd.components_.T
-    Lambda_P = svd.singular_values_
-    return Psi_P, Lambda_P
-
-
-def overlap(array, len_chunk, len_sep=1):
-    """
-    Returns a matrix of all full overlapping chunks of the input `array`, with a chunk
-    length of `len_chunk` and a separation length of `len_sep`. Begins with the first full
-    chunk in the array. 
-    This function is taken from https://stackoverflow.com/questions/38163366/split-list-into-separate-but-overlapping-chunks
-    it is designed to split an array with certain overlaps
-    
-    :param array: 
-    :param len_chunk: 
-    :param len_sep: 
-    :return array_matrix:
-    """
-
-    n_arrays = int(np.ceil((array.size - len_chunk + 1) / len_sep))
-
-    array_matrix = np.tile(array, n_arrays).reshape(n_arrays, -1)
-
-    columns = np.array(((len_sep * np.arange(0, n_arrays)).reshape(n_arrays, -1) + np.tile(
-        np.arange(0, len_chunk), n_arrays).reshape(n_arrays, -1)), dtype=np.intp)
-
-    rows = np.array((np.arange(n_arrays).reshape(n_arrays, -1) + np.tile(
-        np.zeros(len_chunk), n_arrays).reshape(n_arrays, -1)), dtype=np.intp)
-
-    return array_matrix[rows, columns]
-
-
-# def switch_svds_K(A, n_modes, svd_solver):
-#     """
-#     Utility function to switch between different svd solvers
-#     for the diagonalization of K. Being K symmetric and positive definite,
-#     Its eigenvalue decomposition is equivalent to an SVD.
-#     Thus we are using SVD solvers as eig solvers here.
-#     The options are the same used for switch_svds (which goes for the SVD of D)
-
-#     --------------------------------------------------------------------------------------------------------------------
-#     Parameters:
-#     -----------
-#     :param A: np.array,
-#         Array of which compute the SVD
-#     :param n_modes: int,
-#         Number of modes to be computed. Note that if the `svd_numpy` method is chosen, the full matrix are
-#         computed, but then only the first n_modes are returned. Thus, it is not more computationally efficient.
-#     :param svd_solver: str,
-#         can be:
-#             'svd_numpy'.
-#              This uses np.linalg.svd.
-#              It is the most accurate but the slowest and most expensive.
-#              It computes all the modes.
-
-#             'svd_sklearn_truncated'
-#             This uses the TruncatedSVD from scikitlearn. This uses either
-#             svds from scipy or randomized from sklearn depending on the size
-#             of the matrix. These are the two remaining options.
-#             To the merit of chosing this is to let sklearn take the decision as to 
-#             what to use.
-
-#             'svd_scipy_sparse'
-#             This uses the svds from scipy.
-
-#             'svd_sklearn_randomized',
-#             This uses the randomized from sklearn.
-#     Returns
-#     --------
-#     :return Psi_P, np.array (N_S x n_modes)
-#     :return Sigma_P, np.array (n_modes)
-#     """
-#     if svd_solver.lower() == 'svd_sklearn_truncated':
-#         svd = TruncatedSVD(n_modes)
-#         svd.fit_transform(A)
-#         Psi_P = svd.components_.T
-#         Lambda_P = svd.singular_values_
-#         Sigma_P = np.sqrt(Lambda_P)
-#     elif svd_solver.lower() == 'svd_numpy':
-#         Psi_P, Lambda_P, _ = np.linalg.svd(A)
-#         Sigma_P = np.sqrt(Lambda_P)
-#         Psi_P = Psi_P[:, :n_modes]
-#         Sigma_P = Sigma_P[:n_modes]
-#     elif svd_solver.lower() == 'svd_sklearn_randomized':
-#         Psi_P, Lambda_P = randomized_svd(A, n_modes)
-#         Sigma_P = np.sqrt(Lambda_P)
-#     elif svd_solver.lower() == 'svd_scipy_sparse':
-#         Psi_P, Lambda_P, _ = svds(A, k=n_modes)
-#         Sigma_P = np.sqrt(Lambda_P)
-
-#     return Psi_P, Sigma_P
-
-
-def switch_svds(A, n_modes, svd_solver='svd_sklearn_truncated'):
-    """
-    Utility function to switch between different svd solvers
-    for the SVD of the snapshot matrix. This is a true SVD solver.
-
-    --------------------------------------------------------------------------------------------------------------------
-    Parameters:
-    -----------
-    :param A: np.array,
-        Array of which compute the SVD
-    :param n_modes: int,
-        Number of modes to be computed. Note that if the `svd_numpy` method is chosen, the full matrix are
-        computed, but then only the first n_modes are returned. Thus, it is not more computationally efficient.
-    :param svd_solver: str,
-        can be:
-            'svd_numpy'.
-             This uses np.linalg.svd.
-             It is the most accurate but the slowest and most expensive.
-             It computes all the modes.
-
-            'svd_sklearn_truncated'
-            This uses the TruncatedSVD from scikitlearn. This uses either
-            svds from scipy or randomized from sklearn depending on the size
-            of the matrix. These are the two remaining options. 
-            The merit of chosing this is to let sklearn take the decision as to 
-            what to use. One prefers to force the usage of any of those with the other two
-            options
-
-            'svd_scipy_sparse'
-            This uses the svds from scipy.
-
-            'svd_sklearn_randomized',
-            This uses the randomized from sklearn.
-
-    Returns
-    --------
-    :return Psi_P, np.array (N_S x n_modes)
-    :return Sigma_P, np.array (n_modes)
-    """
-    if svd_solver.lower() == 'svd_sklearn_truncated':
-        svd = TruncatedSVD(n_modes)
-        X_transformed = svd.fit_transform(A)
-        Phi_P = X_transformed / svd.singular_values_
-        Psi_P = svd.components_.T
-        Sigma_P = svd.singular_values_
-    elif svd_solver.lower() == 'svd_numpy':
-        Phi_P, Sigma_P, Psi_P = np.linalg.svd(A)
-        Phi_P = Phi_P[:, 0:n_modes]
-        Psi_P = Psi_P.T[:, 0:n_modes]
-        Sigma_P = Sigma_P[0:n_modes]
-    elif svd_solver.lower() == 'svd_sklearn_randomized':
-        Phi_P, Sigma_P, Psi_P = randomized_svd(A, n_modes)
-        Psi_P = Psi_P.T
-    elif svd_solver.lower() == 'svd_scipy_sparse':
-        Phi_P, Sigma_P, Psi_P = svds(A, k=n_modes)
-        Psi_P = Psi_P.T
-        # It turns out that this does not rank them in decreasing order.
-        # Hence we do it manually:
-        idx = np.flip(np.argsort(Sigma_P))
-        Sigma_P = Sigma_P[idx]
-        Phi_P = Phi_P[:, idx]
-        Psi_P = Psi_P[:, idx]
-
-    return Phi_P, Psi_P, Sigma_P
-
-
-def switch_eigs(A, n_modes, eig_solver):
-    """
-    Utility function to switch between different eig solvers in a consistent way across different
-    methods of the package.
-    --------------------------------------------------------------------------------------------------------------------
-    Parameters:
-    -----------
-    :param A: np.array,
-        Array of which compute the eigenvalues
-    :param n_modes: int,
-        Number of modes to be computed. Note that if the `svd_numpy` method is chosen, the full matrix are
-        computed, but then only the first n_modes are returned. Thus, it is not more computationally efficient.
-    :param eig_solver: str,
-        can be:
-            'svd_sklearn_randomized',
-            This uses svd truncated approach, which picks either randomized svd or scipy svds.
-            By default, it should pick mostly the first.
-
-            'eigsh' from scipy sparse. This is a compromise between the previous and the following.
-
-            'eigh' from scipy lin alg. This is the most precise, although a bit more expensive
-
-    Returns
-    --------
-    :return Psi_P, np.array (N_S x n_modes)
-    :return Sigma_P, np.array (n_modes)
-    """
-    if eig_solver.lower() == 'svd_sklearn_randomized':
-        Psi_P, Lambda_P = svds_RND(A, n_modes)
-    elif eig_solver.lower() == 'eigh':
-        n = np.shape(A)[0]
-        Lambda_P, Psi_P = eigh(A, subset_by_index=[n - n_modes, n - 1])
-        # It turns out that this does not rank them in decreasing order.
-        # Hence we do it manually:
-        idx = np.flip(np.argsort(Lambda_P))
-        Lambda_P = Lambda_P[idx]
-        Psi_P = Psi_P[:, idx]
-    elif eig_solver.lower() == 'eigsh':
-        Lambda_P, Psi_P = eigsh(A, k=n_modes)
-        # It turns out that this does not rank them in decreasing order.
-        # Hence we do it manually:
-        idx = np.flip(np.argsort(Lambda_P))
-        Lambda_P = Lambda_P[idx]
-        Psi_P = Psi_P[:, idx]
-
-    Sigma_P = np.sqrt(Lambda_P)
-
+import numpy as np
+from scipy import signal
+from scipy.sparse.linalg import svds, eigsh
+from sklearn.decomposition import TruncatedSVD
+from scipy.linalg import eigh
+from sklearn.utils.extmath import randomized_svd
+
+
+def Bound_EXT(S, Ex, boundaries):
+    """
+   This function computes the extension of a signal for
+   filtering purposes
+
+   :param S: The Input signal
+   :param Nf: The Size of the Kernel (must be an odd number!)
+   :param boundaries: The type of extension:
+           ‘reflect’ (d c b a | a b c d | d c b a)    The input is extended by reflecting about the edge of the last pixel.
+           ‘nearest’ (a a a a | a b c d | d d d d)    The input is extended by replicating the last pixel.
+           ‘wrap’ (a b c d | a b c d | a b c d)       The input is extended by wrapping around to the opposite edge.
+           ‘extrap’ Extrapolation                     The input is extended via linear extrapolation.
+
+
+   """
+    # We first perform a zero padding
+    # Ex=int((Nf-1)/2) # Extension on each size
+    size_Ext = 2 * Ex + len(S)  # Compute the size of the extended signal
+    S_extend = np.zeros((int(size_Ext)))  # Initialize extended signal
+    S_extend[Ex:int((size_Ext - Ex))] = S;  # Assign the Signal on the zeroes
+
+    if boundaries == "reflect":
+        LEFT = np.flip(S[0:Ex])  # Prepare the reflection on the left
+        RIGHT = np.flip(S[len(S) - Ex:len(S)])  # Prepare the reflectino on the right
+        S_extend[0:Ex] = LEFT
+        S_extend[len(S_extend) - Ex:len(S_extend)] = RIGHT
+    elif boundaries == "nearest":
+        LEFT = np.ones(Ex) * S[0]  # Prepare the constant on the left
+        RIGHT = np.ones(Ex) * S[len(S) - 1]  # Prepare the constant on the Right
+        S_extend[0:Ex] = LEFT
+        S_extend[len(S_extend) - Ex:len(S_extend)] = RIGHT
+    elif boundaries == "wrap":
+        LEFT = S[len(S) - Ex:len(S)]  # Wrap on the Left
+        RIGHT = S[0:Ex]  # Wrap on the Right
+        S_extend[0:Ex] = LEFT
+        S_extend[len(S_extend) - Ex:len(S_extend)] = RIGHT
+    elif boundaries == "extrap":
+        LEFT = np.ones(Ex) * S[0]  # Prepare the constant on the left
+        RIGHT = np.ones(Ex) * S[len(S) - 1]  # Prepare the constant on the Right
+        S_extend[0:Ex] = LEFT
+        S_extend[len(S_extend) - Ex:len(S_extend)] = RIGHT
+        print('Not active yet, replaced by nearest')
+    return S_extend
+
+
+def conv_m(K, h, Ex, boundaries):
+    """
+   This function computes the 2D convolution by perfoming 2 sets of 1D convolutions.
+   Moreover, we here use the fft with an appropriate extension
+   that avoids the periodicity condition.
+
+   :param K: Matrix to be filtered
+   :param h: The 1D Kernel of the filter
+   :param boundaries: The type of extension:
+           ‘reflect’ (d c b a | a b c d | d c b a)    The input is extended by reflecting about the edge of the last pixel.
+           ‘nearest’ (a a a a | a b c d | d d d d)    The input is extended by replicating the last pixel.
+           ‘wrap’ (a b c d | a b c d | a b c d)       The input is extended by wrapping around to the opposite edge.
+           ‘extrap’ Extrapolation                     The input is extended via linear extrapolation.
+   """
+    # Filter along the raws
+    n_t = np.shape(K)[0]
+    # Ex=int(n_t/2)
+    K_F1 = np.zeros(np.shape(K))
+    K_F2 = np.zeros(np.shape(K))
+    # K_F=np.zeros(np.shape(K))
+    for k in range(0, n_t):
+        S = K[:, k]
+        S_Ext = Bound_EXT(S, Ex, boundaries)
+        S_Filt = signal.fftconvolve(S_Ext, h, mode='valid')
+        # Compute where to take the signal
+        Ex1 = int((len(S_Filt) - len(S)) / 2)
+        # K_F1[k,:]=S_Filt[Ex:(len(S_Filt)-Ex)]
+        K_F1[:, k] = S_Filt[Ex1:(len(S_Filt) - Ex1)]
+    for k in range(0, n_t):
+        S = K_F1[k, :]
+        S_Ext = Bound_EXT(S, Ex, boundaries)
+        S_Filt = signal.fftconvolve(S_Ext, h, mode='valid')
+        # Compute where to take the signal
+        Ex1 = int((len(S_Filt) - len(S)) / 2)
+        # K_F2[:,k]=S_Filt[Ex:(len(S_Filt)-Ex)]
+        K_F2[k, :] = S_Filt[Ex1:(len(S_Filt) - Ex1)]
+        # K_F=K_F1+K_F2
+    return K_F2
+
+
+def _loop_gemm(a, b, c=None, chunksize=100):
+    size_i = a.shape[0]
+    size_zip = a.shape[1]
+
+    size_j = b.shape[1]
+    size_alt_zip = b.shape[0]
+
+    if size_zip != size_alt_zip:
+        ValueError("Loop GEMM zip index is not of the same size for both tensors")
+
+    if c is None:
+        c = np.zeros((size_i, size_j))
+
+    istart = 0
+    for i in range(int(np.ceil(size_i / float(chunksize)))):
+
+        left_slice = slice(istart, istart + chunksize)
+        left_view = a[left_slice]
+
+        jstart = 0
+        for j in range(int(np.ceil(size_j / float(chunksize)))):
+            right_slice = slice(jstart, jstart + chunksize)
+            right_view = b[:, right_slice]
+
+            c[left_slice, right_slice] = np.dot(left_view, right_view)
+            jstart += chunksize
+
+        istart += chunksize
+
+    return c
+
+
+def svds_RND(K, R_K):
+    """
+    Quick and dirty implementation of randomized SVD
+    for computing eigenvalues of K. We follow same input/output structure
+    as for the svds in scipy
+    """
+    svd = TruncatedSVD(R_K)
+    svd.fit_transform(K)
+    Psi_P = svd.components_.T
+    Lambda_P = svd.singular_values_
+    return Psi_P, Lambda_P
+
+
+def overlap(array, len_chunk, len_sep=1):
+    """
+    Returns a matrix of all full overlapping chunks of the input `array`, with a chunk
+    length of `len_chunk` and a separation length of `len_sep`. Begins with the first full
+    chunk in the array. 
+    This function is taken from https://stackoverflow.com/questions/38163366/split-list-into-separate-but-overlapping-chunks
+    it is designed to split an array with certain overlaps
+    
+    :param array: 
+    :param len_chunk: 
+    :param len_sep: 
+    :return array_matrix:
+    """
+
+    n_arrays = int(np.ceil((array.size - len_chunk + 1) / len_sep))
+
+    array_matrix = np.tile(array, n_arrays).reshape(n_arrays, -1)
+
+    columns = np.array(((len_sep * np.arange(0, n_arrays)).reshape(n_arrays, -1) + np.tile(
+        np.arange(0, len_chunk), n_arrays).reshape(n_arrays, -1)), dtype=np.intp)
+
+    rows = np.array((np.arange(n_arrays).reshape(n_arrays, -1) + np.tile(
+        np.zeros(len_chunk), n_arrays).reshape(n_arrays, -1)), dtype=np.intp)
+
+    return array_matrix[rows, columns]
+
+
+# def switch_svds_K(A, n_modes, svd_solver):
+#     """
+#     Utility function to switch between different svd solvers
+#     for the diagonalization of K. Being K symmetric and positive definite,
+#     Its eigenvalue decomposition is equivalent to an SVD.
+#     Thus we are using SVD solvers as eig solvers here.
+#     The options are the same used for switch_svds (which goes for the SVD of D)
+
+#     --------------------------------------------------------------------------------------------------------------------
+#     Parameters:
+#     -----------
+#     :param A: np.array,
+#         Array of which compute the SVD
+#     :param n_modes: int,
+#         Number of modes to be computed. Note that if the `svd_numpy` method is chosen, the full matrix are
+#         computed, but then only the first n_modes are returned. Thus, it is not more computationally efficient.
+#     :param svd_solver: str,
+#         can be:
+#             'svd_numpy'.
+#              This uses np.linalg.svd.
+#              It is the most accurate but the slowest and most expensive.
+#              It computes all the modes.
+
+#             'svd_sklearn_truncated'
+#             This uses the TruncatedSVD from scikitlearn. This uses either
+#             svds from scipy or randomized from sklearn depending on the size
+#             of the matrix. These are the two remaining options.
+#             To the merit of chosing this is to let sklearn take the decision as to 
+#             what to use.
+
+#             'svd_scipy_sparse'
+#             This uses the svds from scipy.
+
+#             'svd_sklearn_randomized',
+#             This uses the randomized from sklearn.
+#     Returns
+#     --------
+#     :return Psi_P, np.array (N_S x n_modes)
+#     :return Sigma_P, np.array (n_modes)
+#     """
+#     if svd_solver.lower() == 'svd_sklearn_truncated':
+#         svd = TruncatedSVD(n_modes)
+#         svd.fit_transform(A)
+#         Psi_P = svd.components_.T
+#         Lambda_P = svd.singular_values_
+#         Sigma_P = np.sqrt(Lambda_P)
+#     elif svd_solver.lower() == 'svd_numpy':
+#         Psi_P, Lambda_P, _ = np.linalg.svd(A)
+#         Sigma_P = np.sqrt(Lambda_P)
+#         Psi_P = Psi_P[:, :n_modes]
+#         Sigma_P = Sigma_P[:n_modes]
+#     elif svd_solver.lower() == 'svd_sklearn_randomized':
+#         Psi_P, Lambda_P = randomized_svd(A, n_modes)
+#         Sigma_P = np.sqrt(Lambda_P)
+#     elif svd_solver.lower() == 'svd_scipy_sparse':
+#         Psi_P, Lambda_P, _ = svds(A, k=n_modes)
+#         Sigma_P = np.sqrt(Lambda_P)
+
+#     return Psi_P, Sigma_P
+
+
+def switch_svds(A, n_modes, svd_solver='svd_sklearn_truncated'):
+    """
+    Utility function to switch between different svd solvers
+    for the SVD of the snapshot matrix. This is a true SVD solver.
+
+    --------------------------------------------------------------------------------------------------------------------
+    Parameters:
+    -----------
+    :param A: np.array,
+        Array of which compute the SVD
+    :param n_modes: int,
+        Number of modes to be computed. Note that if the `svd_numpy` method is chosen, the full matrix are
+        computed, but then only the first n_modes are returned. Thus, it is not more computationally efficient.
+    :param svd_solver: str,
+        can be:
+            'svd_numpy'.
+             This uses np.linalg.svd.
+             It is the most accurate but the slowest and most expensive.
+             It computes all the modes.
+
+            'svd_sklearn_truncated'
+            This uses the TruncatedSVD from scikitlearn. This uses either
+            svds from scipy or randomized from sklearn depending on the size
+            of the matrix. These are the two remaining options. 
+            The merit of chosing this is to let sklearn take the decision as to 
+            what to use. One prefers to force the usage of any of those with the other two
+            options
+
+            'svd_scipy_sparse'
+            This uses the svds from scipy.
+
+            'svd_sklearn_randomized',
+            This uses the randomized from sklearn.
+
+    Returns
+    --------
+    :return Psi_P, np.array (N_S x n_modes)
+    :return Sigma_P, np.array (n_modes)
+    """
+    if svd_solver.lower() == 'svd_sklearn_truncated':
+        svd = TruncatedSVD(n_modes)
+        X_transformed = svd.fit_transform(A)
+        Phi_P = X_transformed / svd.singular_values_
+        Psi_P = svd.components_.T
+        Sigma_P = svd.singular_values_
+    elif svd_solver.lower() == 'svd_numpy':
+        Phi_P, Sigma_P, Psi_P = np.linalg.svd(A)
+        Phi_P = Phi_P[:, 0:n_modes]
+        Psi_P = Psi_P.T[:, 0:n_modes]
+        Sigma_P = Sigma_P[0:n_modes]
+    elif svd_solver.lower() == 'svd_sklearn_randomized':
+        Phi_P, Sigma_P, Psi_P = randomized_svd(A, n_modes)
+        Psi_P = Psi_P.T
+    elif svd_solver.lower() == 'svd_scipy_sparse':
+        Phi_P, Sigma_P, Psi_P = svds(A, k=n_modes)
+        Psi_P = Psi_P.T
+        # It turns out that this does not rank them in decreasing order.
+        # Hence we do it manually:
+        idx = np.flip(np.argsort(Sigma_P))
+        Sigma_P = Sigma_P[idx]
+        Phi_P = Phi_P[:, idx]
+        Psi_P = Psi_P[:, idx]
+
+    return Phi_P, Psi_P, Sigma_P
+
+
+def switch_eigs(A, n_modes, eig_solver):
+    """
+    Utility function to switch between different eig solvers in a consistent way across different
+    methods of the package.
+    --------------------------------------------------------------------------------------------------------------------
+    Parameters:
+    -----------
+    :param A: np.array,
+        Array of which compute the eigenvalues
+    :param n_modes: int,
+        Number of modes to be computed. Note that if the `svd_numpy` method is chosen, the full matrix are
+        computed, but then only the first n_modes are returned. Thus, it is not more computationally efficient.
+    :param eig_solver: str,
+        can be:
+            'svd_sklearn_randomized',
+            This uses svd truncated approach, which picks either randomized svd or scipy svds.
+            By default, it should pick mostly the first.
+
+            'eigsh' from scipy sparse. This is a compromise between the previous and the following.
+
+            'eigh' from scipy lin alg. This is the most precise, although a bit more expensive
+
+    Returns
+    --------
+    :return Psi_P, np.array (N_S x n_modes)
+    :return Sigma_P, np.array (n_modes)
+    """
+    if eig_solver.lower() == 'svd_sklearn_randomized':
+        Psi_P, Lambda_P = svds_RND(A, n_modes)
+    elif eig_solver.lower() == 'eigh':
+        n = np.shape(A)[0]
+        Lambda_P, Psi_P = eigh(A, subset_by_index=[n - n_modes, n - 1])
+        # It turns out that this does not rank them in decreasing order.
+        # Hence we do it manually:
+        idx = np.flip(np.argsort(Lambda_P))
+        Lambda_P = Lambda_P[idx]
+        Psi_P = Psi_P[:, idx]
+    elif eig_solver.lower() == 'eigsh':
+        Lambda_P, Psi_P = eigsh(A, k=n_modes)
+        # It turns out that this does not rank them in decreasing order.
+        # Hence we do it manually:
+        idx = np.flip(np.argsort(Lambda_P))
+        Lambda_P = Lambda_P[idx]
+        Psi_P = Psi_P[:, idx]
+
+    Sigma_P = np.sqrt(Lambda_P)
+
     return Psi_P, Sigma_P
```

### Comparing `modulo_vki-2.0.4/modulo_vki/utils/others.py` & `modulo_vki-2.0.5/modulo_vki/utils/others.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,449 +1,449 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Dec 30 20:33:42 2019
-@author: mendez
-"""
-
-import numpy as np
-import matplotlib.pyplot as plt
-
-
-def Plot_Field_TEXT_JET(File):
-    """
-    This function plots the vector field from the TR-PIV in Exercise 4.
-
-     :param File: Name of the file to load
-
-    """
-    # We first perform a zero padding
-    Name = File
-    # Read data from a file
-    DATA = np.genfromtxt(Name)  # Here we have the four colums
-    Dat = DATA[1:, :]  # Here we remove the first raw, containing the header
-    nxny = Dat.shape[0]  # is the to be doubled at the end we will have n_s=2 * n_x * n_y
-    n_s = 2 * nxny
-    ## 1. Reconstruct Mesh from file
-    X_S = Dat[:, 0];
-    Y_S = Dat[:, 1];
-    # Reshape also the velocity components
-    V_X = Dat[:, 2]  # U component
-    V_Y = Dat[:, 3]  # V component
-    # Put both components as fields in the grid
-    Xg, Yg, Vxg, Vyg, Magn = Plot_Field_JET(X_S, Y_S, V_X, V_Y, False, 2, 0.6)
-    # Show this particular step
-    fig, ax = plt.subplots(figsize=(8, 5))  # This creates the figure
-    # Or you can plot it as streamlines
-    plt.contourf(Xg, Yg, Magn)
-    # One possibility is to use quiver
-    STEPx = 2
-    STEPy = 2
-    plt.quiver(Xg[::STEPx, ::STEPy], Yg[::STEPx, ::STEPy], \
-               Vxg[::STEPx, ::STEPy], -Vyg[::STEPx, ::STEPy], color='k')  # Create a quiver (arrows) plot
-
-    plt.rc('text', usetex=True)  # This is Miguel's customization
-    plt.rc('font', family='serif')
-    plt.rc('xtick', labelsize=16)
-    plt.rc('ytick', labelsize=16)
-    ax.set_aspect('equal')  # Set equal aspect ratio
-    ax.set_xlabel('$x[mm]$', fontsize=16)
-    ax.set_ylabel('$y[mm]$', fontsize=16)
-    ax.set_title('Velocity Field via TR-PIV', fontsize=18)
-    ax.set_xticks(np.arange(0, 40, 10))
-    ax.set_yticks(np.arange(10, 30, 5))
-    ax.set_xlim([0, 35])
-    ax.set_ylim(10, 29)
-    ax.invert_yaxis()  # Invert Axis for plotting purpose
-    plt.show()
-    Name[len(Name) - 12:len(Name)] + ' Plotted'
-    return n_s, Xg, Yg, Vxg, -Vyg, X_S, Y_S
-
-
-def Plot_Field_JET(X_S, Y_S, V_X, V_Y, PLOT, Step, Scale):
-    # Number of n_X/n_Y from forward differences
-    GRAD_X = np.diff(X_S)
-    # GRAD_Y=np.diff(Y_S);
-    # Depending on the reshaping performed, one of the two will start with
-    # non-zero gradient. The other will have zero gradient only on the change.
-    IND_X = np.where(GRAD_X != 0);
-    DAT = IND_X[0];
-    n_y = DAT[0] + 1;
-    nxny = X_S.shape[0]  # is the to be doubled at the end we will have n_s=2 * n_x * n_y
-    # n_s=2*nxny
-    # Reshaping the grid from the data
-    n_x = (nxny // (n_y))  # Carefull with integer and float!
-    Xg = np.transpose(X_S.reshape((n_x, n_y)))
-    Yg = np.transpose(Y_S.reshape((n_x, n_y)))  # This is now the mesh! 60x114.
-    Mod = np.sqrt(V_X ** 2 + V_Y ** 2)
-    Vxg = np.transpose(V_X.reshape((n_x, n_y)))
-    Vyg = np.transpose(V_Y.reshape((n_x, n_y)))
-    Magn = np.transpose(Mod.reshape((n_x, n_y)))
-    if PLOT:
-        # Show this particular step
-        #    fig, ax = plt.subplots(figsize=(8, 5)) # This creates the figure
-        # Or you can plot it as streamlines
-        #fig, ax = plt.subplots(figsize=(8, 5))  # This creates the figure
-        #ax.contourf(Xg, Yg, Magn)
-        plt.contourf(Xg,Yg,Magn) 
-        # One possibility is to use quiver
-        STEPx = Step
-        STEPy = Step
-
-        plt.quiver(Xg[::STEPx, ::STEPy], Yg[::STEPx, ::STEPy], \
-                   Vxg[::STEPx, ::STEPy], -Vyg[::STEPx, ::STEPy], color='k',
-                   scale=Scale)  # Create a quiver (arrows) plot
-
-        plt.rc('text', usetex=True)  # This is Miguel's customization
-        plt.rc('font', family='serif')
-        plt.rc('xtick', labelsize=16)
-        plt.rc('ytick', labelsize=16)
-    #    ax.set_aspect('equal') # Set equal aspect ratio
-    #    ax.set_xlabel('$x[mm]$',fontsize=16)
-    #    ax.set_ylabel('$y[mm]$',fontsize=16)
-    #    ax.set_title('Velocity Field via TR-PIV',fontsize=18)
-    #    ax.set_xticks(np.arange(0,40,10))
-    #    ax.set_yticks(np.arange(10,30,5))
-    #    ax.set_xlim([0,35])
-    #    ax.set_ylim(10,29)
-    #    ax.invert_yaxis() # Invert Axis for plotting purpose
-    #    plt.show()
-
-    return Xg, Yg, Vxg, Vyg, Magn
-
-
-# Define the function to produce a gif file
-def Animation_JET(Giff_NAME,D,X_S,Y_S,In,Fin,Step):
-    """
-    The gif file is created from the provided data snapshot
-    """
-    n_t=Fin-In    
-    GRAD_X = np.diff(X_S)
-    IND_X = np.where(GRAD_X != 0);
-    DAT = IND_X[0];
-    n_y = DAT[0] + 1;
-    nxny = X_S.shape[0]  # is the to be doubled at the end we will have n_s=2 * n_x * n_y
-    # n_s=2*nxny
-    # Reshaping the grid from the data
-    n_x = (nxny // (n_y))  # Carefull with integer and float!
-    Xg = np.transpose(X_S.reshape((n_x, n_y)))
-    Yg = np.transpose(Y_S.reshape((n_x, n_y)))  # This is now the mesh! 60x114.    n_y, n_x = Yg.shape;
-    nxny = n_x * n_y
-    import os
-    # Create a temporary file to store the images in the GIF
-    Fol_Out = 'Gif_Images_temporary'
-    if not os.path.exists(Fol_Out):
-        os.mkdir(Fol_Out)
-
-    # Prepare Animation of the analytical solution
-    for k in range(1,n_t,Step):
-        Dat = D[:, k+In]
-        V_X_m = Dat[0:nxny]
-        V_Y_m = Dat[nxny::]
-        # Put both components as fields in the grid
-        Mod = np.sqrt(V_X_m ** 2 + V_Y_m ** 2)
-        Vxg = np.transpose(V_X_m.reshape((n_x, n_y)))
-        Vyg = np.transpose(V_Y_m.reshape((n_x, n_y)))
-        Magn = np.transpose(Mod.reshape((n_x, n_y)))
-        fig, ax = plt.subplots(figsize=(8, 5))  # This creates the figure
-        # Or you can plot it as streamlines
-        plt.contourf(Xg, Yg, Magn)
-        # One possibility is to use quiver
-        STEPx = 2
-        STEPy = 2
-        plt.quiver(Xg[::STEPx, ::STEPy], Yg[::STEPx, ::STEPy], \
-                   Vxg[::STEPx, ::STEPy], -Vyg[::STEPx, ::STEPy], color='k')  # Create a quiver (arrows) plot
-
-        plt.rc('text', usetex=True)  # This is Miguel's customization
-        plt.rc('font', family='serif')
-        plt.rc('xtick', labelsize=16)
-        plt.rc('ytick', labelsize=16)
-        ax.set_aspect('equal')  # Set equal aspect ratio
-        ax.set_xlabel('$x[mm]$', fontsize=16)
-        ax.set_ylabel('$y[mm]$', fontsize=16)
-        #ax.set_title('Velocity Field via TR-PIV', fontsize=18)
-        ax.set_xticks(np.arange(0, 40, 10))
-        ax.set_yticks(np.arange(10, 30, 5))
-        ax.set_xlim([0, 35])
-        ax.set_ylim(10, 29)
-        plt.clim(0, 6)
-        ax.invert_yaxis()  # Invert Axis for plotting purpose
-        #plt.show()
-
-        NameOUT = Fol_Out + os.sep + 'Im%03d' % (k) + '.png'
-        plt.savefig(NameOUT, dpi=100)
-        plt.close(fig)
-        print('Image n ' + str(k) + ' of ' + str(n_t))
-
-    # Assembly the GIF
-    import imageio  # This used for the animation
-
-    images = []
-
-    for k in range(1,n_t,Step):
-        MEX = 'Preparing Im ' + str(k)
-        print(MEX)
-        NameOUT = Fol_Out + os.sep + 'Im%03d' % (k) + '.png'
-        images.append(imageio.imread(NameOUT))
-
-    # Now we can assembly the video and clean the folder of png's (optional)
-    imageio.mimsave(Giff_NAME, images, duration=0.05)
-    import shutil  # nice and powerfull tool to delete a folder and its content
-
-    shutil.rmtree(Fol_Out)
-    return 'Gif Created'
-
-
-
-
-def Plot_2D_CFD_Cyl(Xg,Yg,U,V,k=10,CL=16,Name=''):
-    # Make a 2D plot of the 2D cylinder test case in Openfoam.
-    n_x,n_y=np.shape(Xg)
-    U_g=U[:,k].reshape(n_y,n_x).T
-    V_g=V[:,k].reshape(n_y,n_x).T
-    # Prepare the plot        
-    fig, ax = plt.subplots(figsize=(6, 3)) # This creates the figure
-    plt.contourf(Xg,Yg,np.sqrt(U_g**2+V_g**2),30)
-    # plt.quiver(Xg,Yg,U_g,V_g,scale=10000)
-    ax.set_aspect('equal') # Set equal aspect ratio
-    ax.set_xlabel('$x[mm]$',fontsize=13)
-    ax.set_ylabel('$y[mm]$',fontsize=13)
-    #ax.set_title('Tutorial 2: Cylinder Wake',fontsize=12)
-    ax.set_xticks(np.arange(-0.1,0.2,0.05))
-    ax.set_yticks(np.arange(-0.1,0.1,0.05))
-    ax.set_xlim([-0.05,0.2])
-    ax.set_ylim(-0.05,0.05)
-    
-    if CL !=0:
-     plt.clim(0, CL)
-
-    circle = plt.Circle((0,0),0.0075,fill=True,color='r',edgecolor='k',alpha=0.5)
-    plt.gcf().gca().add_artist(circle)
-    plt.tight_layout()
-              
-    if len(Name) !=0:
-        plt.savefig(Name, dpi=200)
-        plt.close(fig)
-        print('Image exported')
-    
-    return 
-
-
-def Animation_2D_CFD_Cyl(Giff_NAME,D,Xg,Yg,In,Fin,Step):
-    """
-    The gif file is created from the provided data snapshot
-    """
-    n_t=Fin-In 
-    n_x,n_y=np.shape(Xg); nxny=n_x*n_y
-    U = D[0:nxny,:]
-    V = D[nxny::,]
-    
-    import os
-    # Create a temporary file to store the images in the GIF
-    Fol_Out = 'Gif_Images_temporary'
-    if not os.path.exists(Fol_Out):
-        os.mkdir(Fol_Out)
-    # Loop to produce the Gifs    
-    for k in range(1,n_t,Step):
-     NameOUT = Fol_Out + os.sep + 'Im%03d' % (k) + '.png'
-     Plot_2D_CFD_Cyl(Xg,Yg,U,V,k=k+In,CL=16,Name=NameOUT)
-
-    import imageio  # This used for the animation
-    images = []
-
-    for k in range(1,n_t,Step):
-        MEX = 'Preparing Im ' + str(k)
-        print(MEX)
-        NameOUT = Fol_Out + os.sep + 'Im%03d' % (k) + '.png'
-        images.append(imageio.imread(NameOUT))
-
-    # Now we can assembly the video and clean the folder of png's (optional)
-    imageio.mimsave(Giff_NAME, images, duration=0.05)
-    import shutil  # nice and powerfull tool to delete a folder and its content
-
-    shutil.rmtree(Fol_Out)
-    return 'Gif Created'
-
-
-
-def Plot_Field_TEXT_Cylinder(File,Name_Mesh,Name_FIG):  
-   """
-   This function plots the vector field from the TR-PIV in Exercise 4.
-      
-    :param File: Name of the file to load          
-   
-   """
-   # We first perform a zero padding
-   Name=File
-   # Read data from a file
-   DATA = np.genfromtxt(Name) # Here we have the four colums
-   Dat=DATA[1:,:] # Here we remove the first raw, containing the header
-   nxny=Dat.shape[0] # is the to be doubled at the end we will have n_s=2 * n_x * n_y
-   n_s=2*nxny
-   ## 1. Reconstruct Mesh from file Name_Mesh
-   DATA_mesh=np.genfromtxt(Name_Mesh);
-   Dat_mesh=DATA_mesh[1:,:]
-   X_S=Dat_mesh[:,0];
-   Y_S=Dat_mesh[:,1];
-   # Reshape also the velocity components
-   V_X=Dat[:,0] # U component
-   V_Y=Dat[:,1] # V component
-   # Put both components as fields in the grid
-   Xg,Yg,Vxg,Vyg,Magn=Plot_Field_Cylinder(X_S,Y_S,V_X,V_Y,False,2,0.6)
-   # Show this particular step
-   fig, ax = plt.subplots(figsize=(5, 3)) # This creates the figure
-   # Or you can plot it as streamlines
-   CL=plt.contourf(Xg,Yg,Magn,levels=np.arange(0,18,2))
-   # One possibility is to use quiver
-   STEPx=1;  STEPy=1
-   plt.quiver(Xg[::STEPx,::STEPy],Yg[::STEPx,::STEPy],\
-               Vxg[::STEPx,::STEPy],Vyg[::STEPx,::STEPy],color='k')
-   plt.rc('text', usetex=True)      
-   plt.rc('font', family='serif')
-   plt.rc('xtick',labelsize=12)
-   plt.rc('ytick',labelsize=12)
-   fig.colorbar(CL,pad=0.05,fraction=0.025)
-   ax.set_aspect('equal') # Set equal aspect ratio
-   ax.set_xlabel('$x[mm]$',fontsize=13)
-   ax.set_ylabel('$y[mm]$',fontsize=13)
-   #ax.set_title('Tutorial 2: Cylinder Wake',fontsize=12)
-   ax.set_xticks(np.arange(0,70,10))
-   ax.set_yticks(np.arange(-10,11,10))
-   ax.set_xlim([0,50])
-   ax.set_ylim(-10,10)
-   circle = plt.Circle((0,0),2.5,fill=True,color='r',edgecolor='k',alpha=0.5)
-   plt.gcf().gca().add_artist(circle)
-   plt.tight_layout()   
-   plt.savefig(Name_FIG, dpi=200) 
-   plt.show()
-   print(Name_FIG+' printed')
-   return n_s, Xg, Yg, Vxg, Vyg, X_S, Y_S
-
-
-def Plot_Field_Cylinder(X_S,Y_S,V_X,V_Y,PLOT,Step,Scale):
-  # Number of n_X/n_Y from forward differences
-   GRAD_X=np.diff(Y_S) 
-   #GRAD_Y=np.diff(Y_S);
-   # Depending on the reshaping performed, one of the two will start with
-   # non-zero gradient. The other will have zero gradient only on the change.
-   IND_X=np.where(GRAD_X!=0); DAT=IND_X[0]; n_y=DAT[0]+1;
-   nxny=X_S.shape[0] # is the to be doubled at the end we will have n_s=2 * n_x * n_y
-   #n_s=2*nxny
-   # Reshaping the grid from the data
-   n_x=(nxny//(n_y)) # Carefull with integer and float!
-   Xg=np.transpose(X_S.reshape((n_x,n_y)))
-   Yg=np.transpose(Y_S.reshape((n_x,n_y))) # This is now the mesh! 60x114.
-   Mod=np.sqrt(V_X**2+V_Y**2)
-   Vxg=np.transpose(V_X.reshape((n_x,n_y)))
-   Vyg=np.transpose(V_Y.reshape((n_x,n_y)))
-   Magn=np.transpose(Mod.reshape((n_x,n_y)))
-  
-   if PLOT:
-    # One possibility is to use quiver
-    STEPx=Step;  STEPy=Step
-    fig, ax = plt.subplots(figsize=(5, 3)) # This creates the figure
-    # Or you can plot it as streamlines
-    CL=plt.contourf(Xg,Yg,Magn,levels=np.arange(0,18,2))
-    # One possibility is to use quiver
-    STEPx=1;  STEPy=1
-    plt.quiver(Xg[::STEPx,::STEPy],Yg[::STEPx,::STEPy],\
-               Vxg[::STEPx,::STEPy],Vyg[::STEPx,::STEPy],color='k')
-    plt.rc('text', usetex=True)      
-    plt.rc('font', family='serif')
-    plt.rc('xtick',labelsize=12)
-    plt.rc('ytick',labelsize=12)
-    fig.colorbar(CL,pad=0.05,fraction=0.025)
-    ax.set_aspect('equal') # Set equal aspect ratio
-    ax.set_xlabel('$x[mm]$',fontsize=13)
-    ax.set_ylabel('$y[mm]$',fontsize=13)
-    #ax.set_title('Tutorial 2: Cylinder Wake',fontsize=12)
-    ax.set_xticks(np.arange(0,70,10))
-    ax.set_yticks(np.arange(-10,11,10))
-    ax.set_xlim([0,50])
-    ax.set_ylim(-10,10)
-    circle = plt.Circle((0,0),2.5,fill=True,color='r',edgecolor='k',alpha=0.5)
-    plt.gcf().gca().add_artist(circle)
-    plt.tight_layout()
-    plt.show()
-       
-   return Xg,Yg,Vxg,Vyg,Magn  
-   
-def Plot_Scalar_Field_Cylinder(X_S,Y_S,V_X,V_Y,Scalar,PLOT,Step,Scale):
-  # Number of n_X/n_Y from forward differences
-   GRAD_X=np.diff(Y_S) 
-   #GRAD_Y=np.diff(Y_S);
-   # Depending on the reshaping performed, one of the two will start with
-   # non-zero gradient. The other will have zero gradient only on the change.
-   IND_X=np.where(GRAD_X!=0); DAT=IND_X[0]; n_y=DAT[0]+1;
-   nxny=X_S.shape[0] # is the to be doubled at the end we will have n_s=2 * n_x * n_y
-   #n_s=2*nxny
-   # Reshaping the grid from the data
-   n_x=(nxny//(n_y)) # Carefull with integer and float!
-   Xg=np.transpose(X_S.reshape((n_x,n_y)))
-   Yg=np.transpose(Y_S.reshape((n_x,n_y))) # This is now the mesh! 60x114.
-   Vxg=np.transpose(V_X.reshape((n_x,n_y)))
-   Vyg=np.transpose(V_Y.reshape((n_x,n_y)))
-   Magn=np.transpose(Scalar.reshape((n_x,n_y)))
-  
-   if PLOT:
-    # One possibility is to use quiver
-    STEPx=Step;  STEPy=Step
-    fig, ax = plt.subplots(figsize=(5, 3)) # This creates the figure
-    # Or you can plot it as streamlines
-    CL=plt.contourf(Xg,Yg,Magn*100,levels=np.arange(0,70,10))
-    # One possibility is to use quiver
-    STEPx=1;  STEPy=1
-    plt.quiver(Xg[::STEPx,::STEPy],Yg[::STEPx,::STEPy],\
-               Vxg[::STEPx,::STEPy],Vyg[::STEPx,::STEPy],color='k')
-    plt.rc('text', usetex=True)      
-    plt.rc('font', family='serif')
-    plt.rc('xtick',labelsize=12)
-    plt.rc('ytick',labelsize=12)
-    fig.colorbar(CL,pad=0.05,fraction=0.025)
-    ax.set_aspect('equal') # Set equal aspect ratio
-    ax.set_xlabel('$x[mm]$',fontsize=13)
-    ax.set_ylabel('$y[mm]$',fontsize=13)
-    #ax.set_title('Tutorial 2: Cylinder Wake',fontsize=12)
-    ax.set_xticks(np.arange(0,70,10))
-    ax.set_yticks(np.arange(-10,11,10))
-    ax.set_xlim([0,50])
-    ax.set_ylim(-10,10)
-    circle = plt.Circle((0,0),2.5,fill=True,color='r',edgecolor='k',alpha=0.5)
-    plt.gcf().gca().add_artist(circle)
-    plt.tight_layout()
-    plt.show()
-       
-   return Xg,Yg,Vxg,Vyg,Magn  
-
-
-
-def plot_grid_cylinder_flow(Xg,Yg,Vxg,Vyg):
- STEPx=1;  STEPy=1
- # This creates the figure
- fig, ax = plt.subplots(figsize=(6, 3)) 
- Magn=np.sqrt(Vxg**2+Vyg**2)
- # Plot Contour
- #CL=plt.contourf(Xg,Yg,Magn,levels=np.linspace(0,np.max(Magn),5))
- CL=plt.contourf(Xg,Yg,Magn,20,cmap='viridis',alpha=0.95)
- # One possibility is to use quiver
- STEPx=1;  STEPy=1
- plt.quiver(Xg[::STEPx,::STEPy],Yg[::STEPx,::STEPy],\
-            Vxg[::STEPx,::STEPy],Vyg[::STEPx,::STEPy],color='k')
- plt.rc('text', usetex=True)      
- plt.rc('font', family='serif')
- plt.rc('xtick',labelsize=12)
- plt.rc('ytick',labelsize=12)
- #fig.colorbar(CL,pad=0.05,fraction=0.025)
- ax.set_aspect('equal') # Set equal aspect ratio
- ax.set_xlabel('$x[mm]$',fontsize=13)
- ax.set_ylabel('$y[mm]$',fontsize=13)
- #ax.set_title('Tutorial 2: Cylinder Wake',fontsize=12)
- ax.set_xticks(np.arange(0,70,10))
- ax.set_yticks(np.arange(-10,11,10))
- ax.set_xlim([0,50])
- ax.set_ylim(-10,10)
- circle = plt.Circle((0,0),2.5,fill=True,color='r',edgecolor='k',alpha=0.5)
- plt.gcf().gca().add_artist(circle)
- plt.tight_layout()
- plt.show()
-
-
-
+# -*- coding: utf-8 -*-
+"""
+Created on Mon Dec 30 20:33:42 2019
+@author: mendez
+"""
+
+import numpy as np
+import matplotlib.pyplot as plt
+
+
+def Plot_Field_TEXT_JET(File):
+    """
+    This function plots the vector field from the TR-PIV in Exercise 4.
+
+     :param File: Name of the file to load
+
+    """
+    # We first perform a zero padding
+    Name = File
+    # Read data from a file
+    DATA = np.genfromtxt(Name)  # Here we have the four colums
+    Dat = DATA[1:, :]  # Here we remove the first raw, containing the header
+    nxny = Dat.shape[0]  # is the to be doubled at the end we will have n_s=2 * n_x * n_y
+    n_s = 2 * nxny
+    ## 1. Reconstruct Mesh from file
+    X_S = Dat[:, 0];
+    Y_S = Dat[:, 1];
+    # Reshape also the velocity components
+    V_X = Dat[:, 2]  # U component
+    V_Y = Dat[:, 3]  # V component
+    # Put both components as fields in the grid
+    Xg, Yg, Vxg, Vyg, Magn = Plot_Field_JET(X_S, Y_S, V_X, V_Y, False, 2, 0.6)
+    # Show this particular step
+    fig, ax = plt.subplots(figsize=(8, 5))  # This creates the figure
+    # Or you can plot it as streamlines
+    plt.contourf(Xg, Yg, Magn)
+    # One possibility is to use quiver
+    STEPx = 2
+    STEPy = 2
+    plt.quiver(Xg[::STEPx, ::STEPy], Yg[::STEPx, ::STEPy], \
+               Vxg[::STEPx, ::STEPy], -Vyg[::STEPx, ::STEPy], color='k')  # Create a quiver (arrows) plot
+
+    plt.rc('text', usetex=True)  # This is Miguel's customization
+    plt.rc('font', family='serif')
+    plt.rc('xtick', labelsize=16)
+    plt.rc('ytick', labelsize=16)
+    ax.set_aspect('equal')  # Set equal aspect ratio
+    ax.set_xlabel('$x[mm]$', fontsize=16)
+    ax.set_ylabel('$y[mm]$', fontsize=16)
+    ax.set_title('Velocity Field via TR-PIV', fontsize=18)
+    ax.set_xticks(np.arange(0, 40, 10))
+    ax.set_yticks(np.arange(10, 30, 5))
+    ax.set_xlim([0, 35])
+    ax.set_ylim(10, 29)
+    ax.invert_yaxis()  # Invert Axis for plotting purpose
+    plt.show()
+    Name[len(Name) - 12:len(Name)] + ' Plotted'
+    return n_s, Xg, Yg, Vxg, -Vyg, X_S, Y_S
+
+
+def Plot_Field_JET(X_S, Y_S, V_X, V_Y, PLOT, Step, Scale):
+    # Number of n_X/n_Y from forward differences
+    GRAD_X = np.diff(X_S)
+    # GRAD_Y=np.diff(Y_S);
+    # Depending on the reshaping performed, one of the two will start with
+    # non-zero gradient. The other will have zero gradient only on the change.
+    IND_X = np.where(GRAD_X != 0);
+    DAT = IND_X[0];
+    n_y = DAT[0] + 1;
+    nxny = X_S.shape[0]  # is the to be doubled at the end we will have n_s=2 * n_x * n_y
+    # n_s=2*nxny
+    # Reshaping the grid from the data
+    n_x = (nxny // (n_y))  # Carefull with integer and float!
+    Xg = np.transpose(X_S.reshape((n_x, n_y)))
+    Yg = np.transpose(Y_S.reshape((n_x, n_y)))  # This is now the mesh! 60x114.
+    Mod = np.sqrt(V_X ** 2 + V_Y ** 2)
+    Vxg = np.transpose(V_X.reshape((n_x, n_y)))
+    Vyg = np.transpose(V_Y.reshape((n_x, n_y)))
+    Magn = np.transpose(Mod.reshape((n_x, n_y)))
+    if PLOT:
+        # Show this particular step
+        #    fig, ax = plt.subplots(figsize=(8, 5)) # This creates the figure
+        # Or you can plot it as streamlines
+        #fig, ax = plt.subplots(figsize=(8, 5))  # This creates the figure
+        #ax.contourf(Xg, Yg, Magn)
+        plt.contourf(Xg,Yg,Magn) 
+        # One possibility is to use quiver
+        STEPx = Step
+        STEPy = Step
+
+        plt.quiver(Xg[::STEPx, ::STEPy], Yg[::STEPx, ::STEPy], \
+                   Vxg[::STEPx, ::STEPy], -Vyg[::STEPx, ::STEPy], color='k',
+                   scale=Scale)  # Create a quiver (arrows) plot
+
+        plt.rc('text', usetex=True)  # This is Miguel's customization
+        plt.rc('font', family='serif')
+        plt.rc('xtick', labelsize=16)
+        plt.rc('ytick', labelsize=16)
+    #    ax.set_aspect('equal') # Set equal aspect ratio
+    #    ax.set_xlabel('$x[mm]$',fontsize=16)
+    #    ax.set_ylabel('$y[mm]$',fontsize=16)
+    #    ax.set_title('Velocity Field via TR-PIV',fontsize=18)
+    #    ax.set_xticks(np.arange(0,40,10))
+    #    ax.set_yticks(np.arange(10,30,5))
+    #    ax.set_xlim([0,35])
+    #    ax.set_ylim(10,29)
+    #    ax.invert_yaxis() # Invert Axis for plotting purpose
+    #    plt.show()
+
+    return Xg, Yg, Vxg, Vyg, Magn
+
+
+# Define the function to produce a gif file
+def Animation_JET(Giff_NAME,D,X_S,Y_S,In,Fin,Step):
+    """
+    The gif file is created from the provided data snapshot
+    """
+    n_t=Fin-In    
+    GRAD_X = np.diff(X_S)
+    IND_X = np.where(GRAD_X != 0);
+    DAT = IND_X[0];
+    n_y = DAT[0] + 1;
+    nxny = X_S.shape[0]  # is the to be doubled at the end we will have n_s=2 * n_x * n_y
+    # n_s=2*nxny
+    # Reshaping the grid from the data
+    n_x = (nxny // (n_y))  # Carefull with integer and float!
+    Xg = np.transpose(X_S.reshape((n_x, n_y)))
+    Yg = np.transpose(Y_S.reshape((n_x, n_y)))  # This is now the mesh! 60x114.    n_y, n_x = Yg.shape;
+    nxny = n_x * n_y
+    import os
+    # Create a temporary file to store the images in the GIF
+    Fol_Out = 'Gif_Images_temporary'
+    if not os.path.exists(Fol_Out):
+        os.mkdir(Fol_Out)
+
+    # Prepare Animation of the analytical solution
+    for k in range(1,n_t,Step):
+        Dat = D[:, k+In]
+        V_X_m = Dat[0:nxny]
+        V_Y_m = Dat[nxny::]
+        # Put both components as fields in the grid
+        Mod = np.sqrt(V_X_m ** 2 + V_Y_m ** 2)
+        Vxg = np.transpose(V_X_m.reshape((n_x, n_y)))
+        Vyg = np.transpose(V_Y_m.reshape((n_x, n_y)))
+        Magn = np.transpose(Mod.reshape((n_x, n_y)))
+        fig, ax = plt.subplots(figsize=(8, 5))  # This creates the figure
+        # Or you can plot it as streamlines
+        plt.contourf(Xg, Yg, Magn)
+        # One possibility is to use quiver
+        STEPx = 2
+        STEPy = 2
+        plt.quiver(Xg[::STEPx, ::STEPy], Yg[::STEPx, ::STEPy], \
+                   Vxg[::STEPx, ::STEPy], -Vyg[::STEPx, ::STEPy], color='k')  # Create a quiver (arrows) plot
+
+        plt.rc('text', usetex=True)  # This is Miguel's customization
+        plt.rc('font', family='serif')
+        plt.rc('xtick', labelsize=16)
+        plt.rc('ytick', labelsize=16)
+        ax.set_aspect('equal')  # Set equal aspect ratio
+        ax.set_xlabel('$x[mm]$', fontsize=16)
+        ax.set_ylabel('$y[mm]$', fontsize=16)
+        #ax.set_title('Velocity Field via TR-PIV', fontsize=18)
+        ax.set_xticks(np.arange(0, 40, 10))
+        ax.set_yticks(np.arange(10, 30, 5))
+        ax.set_xlim([0, 35])
+        ax.set_ylim(10, 29)
+        plt.clim(0, 6)
+        ax.invert_yaxis()  # Invert Axis for plotting purpose
+        #plt.show()
+
+        NameOUT = Fol_Out + os.sep + 'Im%03d' % (k) + '.png'
+        plt.savefig(NameOUT, dpi=100)
+        plt.close(fig)
+        print('Image n ' + str(k) + ' of ' + str(n_t))
+
+    # Assembly the GIF
+    import imageio  # This used for the animation
+
+    images = []
+
+    for k in range(1,n_t,Step):
+        MEX = 'Preparing Im ' + str(k)
+        print(MEX)
+        NameOUT = Fol_Out + os.sep + 'Im%03d' % (k) + '.png'
+        images.append(imageio.imread(NameOUT))
+
+    # Now we can assembly the video and clean the folder of png's (optional)
+    imageio.mimsave(Giff_NAME, images, duration=0.05)
+    import shutil  # nice and powerfull tool to delete a folder and its content
+
+    shutil.rmtree(Fol_Out)
+    return 'Gif Created'
+
+
+
+
+def Plot_2D_CFD_Cyl(Xg,Yg,U,V,k=10,CL=16,Name=''):
+    # Make a 2D plot of the 2D cylinder test case in Openfoam.
+    n_x,n_y=np.shape(Xg)
+    U_g=U[:,k].reshape(n_y,n_x).T
+    V_g=V[:,k].reshape(n_y,n_x).T
+    # Prepare the plot        
+    fig, ax = plt.subplots(figsize=(6, 3)) # This creates the figure
+    plt.contourf(Xg,Yg,np.sqrt(U_g**2+V_g**2),30)
+    # plt.quiver(Xg,Yg,U_g,V_g,scale=10000)
+    ax.set_aspect('equal') # Set equal aspect ratio
+    ax.set_xlabel('$x[mm]$',fontsize=13)
+    ax.set_ylabel('$y[mm]$',fontsize=13)
+    #ax.set_title('Tutorial 2: Cylinder Wake',fontsize=12)
+    ax.set_xticks(np.arange(-0.1,0.2,0.05))
+    ax.set_yticks(np.arange(-0.1,0.1,0.05))
+    ax.set_xlim([-0.05,0.2])
+    ax.set_ylim(-0.05,0.05)
+    
+    if CL !=0:
+     plt.clim(0, CL)
+
+    circle = plt.Circle((0,0),0.0075,fill=True,color='r',edgecolor='k',alpha=0.5)
+    plt.gcf().gca().add_artist(circle)
+    plt.tight_layout()
+              
+    if len(Name) !=0:
+        plt.savefig(Name, dpi=200)
+        plt.close(fig)
+        print('Image exported')
+    
+    return 
+
+
+def Animation_2D_CFD_Cyl(Giff_NAME,D,Xg,Yg,In,Fin,Step):
+    """
+    The gif file is created from the provided data snapshot
+    """
+    n_t=Fin-In 
+    n_x,n_y=np.shape(Xg); nxny=n_x*n_y
+    U = D[0:nxny,:]
+    V = D[nxny::,]
+    
+    import os
+    # Create a temporary file to store the images in the GIF
+    Fol_Out = 'Gif_Images_temporary'
+    if not os.path.exists(Fol_Out):
+        os.mkdir(Fol_Out)
+    # Loop to produce the Gifs    
+    for k in range(1,n_t,Step):
+     NameOUT = Fol_Out + os.sep + 'Im%03d' % (k) + '.png'
+     Plot_2D_CFD_Cyl(Xg,Yg,U,V,k=k+In,CL=16,Name=NameOUT)
+
+    import imageio  # This used for the animation
+    images = []
+
+    for k in range(1,n_t,Step):
+        MEX = 'Preparing Im ' + str(k)
+        print(MEX)
+        NameOUT = Fol_Out + os.sep + 'Im%03d' % (k) + '.png'
+        images.append(imageio.imread(NameOUT))
+
+    # Now we can assembly the video and clean the folder of png's (optional)
+    imageio.mimsave(Giff_NAME, images, duration=0.05)
+    import shutil  # nice and powerfull tool to delete a folder and its content
+
+    shutil.rmtree(Fol_Out)
+    return 'Gif Created'
+
+
+
+def Plot_Field_TEXT_Cylinder(File,Name_Mesh,Name_FIG):  
+   """
+   This function plots the vector field from the TR-PIV in Exercise 4.
+      
+    :param File: Name of the file to load          
+   
+   """
+   # We first perform a zero padding
+   Name=File
+   # Read data from a file
+   DATA = np.genfromtxt(Name) # Here we have the four colums
+   Dat=DATA[1:,:] # Here we remove the first raw, containing the header
+   nxny=Dat.shape[0] # is the to be doubled at the end we will have n_s=2 * n_x * n_y
+   n_s=2*nxny
+   ## 1. Reconstruct Mesh from file Name_Mesh
+   DATA_mesh=np.genfromtxt(Name_Mesh);
+   Dat_mesh=DATA_mesh[1:,:]
+   X_S=Dat_mesh[:,0];
+   Y_S=Dat_mesh[:,1];
+   # Reshape also the velocity components
+   V_X=Dat[:,0] # U component
+   V_Y=Dat[:,1] # V component
+   # Put both components as fields in the grid
+   Xg,Yg,Vxg,Vyg,Magn=Plot_Field_Cylinder(X_S,Y_S,V_X,V_Y,False,2,0.6)
+   # Show this particular step
+   fig, ax = plt.subplots(figsize=(5, 3)) # This creates the figure
+   # Or you can plot it as streamlines
+   CL=plt.contourf(Xg,Yg,Magn,levels=np.arange(0,18,2))
+   # One possibility is to use quiver
+   STEPx=1;  STEPy=1
+   plt.quiver(Xg[::STEPx,::STEPy],Yg[::STEPx,::STEPy],\
+               Vxg[::STEPx,::STEPy],Vyg[::STEPx,::STEPy],color='k')
+   plt.rc('text', usetex=True)      
+   plt.rc('font', family='serif')
+   plt.rc('xtick',labelsize=12)
+   plt.rc('ytick',labelsize=12)
+   fig.colorbar(CL,pad=0.05,fraction=0.025)
+   ax.set_aspect('equal') # Set equal aspect ratio
+   ax.set_xlabel('$x[mm]$',fontsize=13)
+   ax.set_ylabel('$y[mm]$',fontsize=13)
+   #ax.set_title('Tutorial 2: Cylinder Wake',fontsize=12)
+   ax.set_xticks(np.arange(0,70,10))
+   ax.set_yticks(np.arange(-10,11,10))
+   ax.set_xlim([0,50])
+   ax.set_ylim(-10,10)
+   circle = plt.Circle((0,0),2.5,fill=True,color='r',edgecolor='k',alpha=0.5)
+   plt.gcf().gca().add_artist(circle)
+   plt.tight_layout()   
+   plt.savefig(Name_FIG, dpi=200) 
+   plt.show()
+   print(Name_FIG+' printed')
+   return n_s, Xg, Yg, Vxg, Vyg, X_S, Y_S
+
+
+def Plot_Field_Cylinder(X_S,Y_S,V_X,V_Y,PLOT,Step,Scale):
+  # Number of n_X/n_Y from forward differences
+   GRAD_X=np.diff(Y_S) 
+   #GRAD_Y=np.diff(Y_S);
+   # Depending on the reshaping performed, one of the two will start with
+   # non-zero gradient. The other will have zero gradient only on the change.
+   IND_X=np.where(GRAD_X!=0); DAT=IND_X[0]; n_y=DAT[0]+1;
+   nxny=X_S.shape[0] # is the to be doubled at the end we will have n_s=2 * n_x * n_y
+   #n_s=2*nxny
+   # Reshaping the grid from the data
+   n_x=(nxny//(n_y)) # Carefull with integer and float!
+   Xg=np.transpose(X_S.reshape((n_x,n_y)))
+   Yg=np.transpose(Y_S.reshape((n_x,n_y))) # This is now the mesh! 60x114.
+   Mod=np.sqrt(V_X**2+V_Y**2)
+   Vxg=np.transpose(V_X.reshape((n_x,n_y)))
+   Vyg=np.transpose(V_Y.reshape((n_x,n_y)))
+   Magn=np.transpose(Mod.reshape((n_x,n_y)))
+  
+   if PLOT:
+    # One possibility is to use quiver
+    STEPx=Step;  STEPy=Step
+    fig, ax = plt.subplots(figsize=(5, 3)) # This creates the figure
+    # Or you can plot it as streamlines
+    CL=plt.contourf(Xg,Yg,Magn,levels=np.arange(0,18,2))
+    # One possibility is to use quiver
+    STEPx=1;  STEPy=1
+    plt.quiver(Xg[::STEPx,::STEPy],Yg[::STEPx,::STEPy],\
+               Vxg[::STEPx,::STEPy],Vyg[::STEPx,::STEPy],color='k')
+    plt.rc('text', usetex=True)      
+    plt.rc('font', family='serif')
+    plt.rc('xtick',labelsize=12)
+    plt.rc('ytick',labelsize=12)
+    fig.colorbar(CL,pad=0.05,fraction=0.025)
+    ax.set_aspect('equal') # Set equal aspect ratio
+    ax.set_xlabel('$x[mm]$',fontsize=13)
+    ax.set_ylabel('$y[mm]$',fontsize=13)
+    #ax.set_title('Tutorial 2: Cylinder Wake',fontsize=12)
+    ax.set_xticks(np.arange(0,70,10))
+    ax.set_yticks(np.arange(-10,11,10))
+    ax.set_xlim([0,50])
+    ax.set_ylim(-10,10)
+    circle = plt.Circle((0,0),2.5,fill=True,color='r',edgecolor='k',alpha=0.5)
+    plt.gcf().gca().add_artist(circle)
+    plt.tight_layout()
+    plt.show()
+       
+   return Xg,Yg,Vxg,Vyg,Magn  
+   
+def Plot_Scalar_Field_Cylinder(X_S,Y_S,V_X,V_Y,Scalar,PLOT,Step,Scale):
+  # Number of n_X/n_Y from forward differences
+   GRAD_X=np.diff(Y_S) 
+   #GRAD_Y=np.diff(Y_S);
+   # Depending on the reshaping performed, one of the two will start with
+   # non-zero gradient. The other will have zero gradient only on the change.
+   IND_X=np.where(GRAD_X!=0); DAT=IND_X[0]; n_y=DAT[0]+1;
+   nxny=X_S.shape[0] # is the to be doubled at the end we will have n_s=2 * n_x * n_y
+   #n_s=2*nxny
+   # Reshaping the grid from the data
+   n_x=(nxny//(n_y)) # Carefull with integer and float!
+   Xg=np.transpose(X_S.reshape((n_x,n_y)))
+   Yg=np.transpose(Y_S.reshape((n_x,n_y))) # This is now the mesh! 60x114.
+   Vxg=np.transpose(V_X.reshape((n_x,n_y)))
+   Vyg=np.transpose(V_Y.reshape((n_x,n_y)))
+   Magn=np.transpose(Scalar.reshape((n_x,n_y)))
+  
+   if PLOT:
+    # One possibility is to use quiver
+    STEPx=Step;  STEPy=Step
+    fig, ax = plt.subplots(figsize=(5, 3)) # This creates the figure
+    # Or you can plot it as streamlines
+    CL=plt.contourf(Xg,Yg,Magn*100,levels=np.arange(0,70,10))
+    # One possibility is to use quiver
+    STEPx=1;  STEPy=1
+    plt.quiver(Xg[::STEPx,::STEPy],Yg[::STEPx,::STEPy],\
+               Vxg[::STEPx,::STEPy],Vyg[::STEPx,::STEPy],color='k')
+    plt.rc('text', usetex=True)      
+    plt.rc('font', family='serif')
+    plt.rc('xtick',labelsize=12)
+    plt.rc('ytick',labelsize=12)
+    fig.colorbar(CL,pad=0.05,fraction=0.025)
+    ax.set_aspect('equal') # Set equal aspect ratio
+    ax.set_xlabel('$x[mm]$',fontsize=13)
+    ax.set_ylabel('$y[mm]$',fontsize=13)
+    #ax.set_title('Tutorial 2: Cylinder Wake',fontsize=12)
+    ax.set_xticks(np.arange(0,70,10))
+    ax.set_yticks(np.arange(-10,11,10))
+    ax.set_xlim([0,50])
+    ax.set_ylim(-10,10)
+    circle = plt.Circle((0,0),2.5,fill=True,color='r',edgecolor='k',alpha=0.5)
+    plt.gcf().gca().add_artist(circle)
+    plt.tight_layout()
+    plt.show()
+       
+   return Xg,Yg,Vxg,Vyg,Magn  
+
+
+
+def plot_grid_cylinder_flow(Xg,Yg,Vxg,Vyg):
+ STEPx=1;  STEPy=1
+ # This creates the figure
+ fig, ax = plt.subplots(figsize=(6, 3)) 
+ Magn=np.sqrt(Vxg**2+Vyg**2)
+ # Plot Contour
+ #CL=plt.contourf(Xg,Yg,Magn,levels=np.linspace(0,np.max(Magn),5))
+ CL=plt.contourf(Xg,Yg,Magn,20,cmap='viridis',alpha=0.95)
+ # One possibility is to use quiver
+ STEPx=1;  STEPy=1
+ plt.quiver(Xg[::STEPx,::STEPy],Yg[::STEPx,::STEPy],\
+            Vxg[::STEPx,::STEPy],Vyg[::STEPx,::STEPy],color='k')
+ plt.rc('text', usetex=True)      
+ plt.rc('font', family='serif')
+ plt.rc('xtick',labelsize=12)
+ plt.rc('ytick',labelsize=12)
+ #fig.colorbar(CL,pad=0.05,fraction=0.025)
+ ax.set_aspect('equal') # Set equal aspect ratio
+ ax.set_xlabel('$x[mm]$',fontsize=13)
+ ax.set_ylabel('$y[mm]$',fontsize=13)
+ #ax.set_title('Tutorial 2: Cylinder Wake',fontsize=12)
+ ax.set_xticks(np.arange(0,70,10))
+ ax.set_yticks(np.arange(-10,11,10))
+ ax.set_xlim([0,50])
+ ax.set_ylim(-10,10)
+ circle = plt.Circle((0,0),2.5,fill=True,color='r',edgecolor='k',alpha=0.5)
+ plt.gcf().gca().add_artist(circle)
+ plt.tight_layout()
+ plt.show()
+
+
+
```

### Comparing `modulo_vki-2.0.4/modulo_vki/utils/read_db.py` & `modulo_vki-2.0.5/modulo_vki/utils/read_db.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,339 +1,339 @@
-import numpy as np
-import os
-from tqdm import tqdm
-import math
-
-
-class ReadData:
-    """
-    A MODULO helper class for input data.  ReadData allows to load the data directly before using MODULO, and
-    hence assembling the data matrix D from data.
-    """
-
-
-    def __init__(self):
-        pass
-
-
-    @classmethod
-    def _data_processing(cls,D: np.array, FOLDER_OUT: str='./',
-                   N_PARTITIONS: int = 1,
-                   MR: bool = False, SAVE_D: bool = False,
-                   FOLDER_IN: str = './', filename: str = '',
-                   h: int = 0, f: int = 0, c: int = 0,
-                   N: int = 0, N_S: int = 0, N_T: int = 0):
-        """
-        First, if the D matrix is not provided, this method attempts to load the data and assembles the D matrix.
-        Then, it performs pre-processing operations on the data matrix, D. if MR=True, the mean (per each column - i.e.: snapshot at time t_i) is removed;
-        If the MEMORY_SAVING=True the data matrix is splitted to optimize memory usage. Moreover, D is stored on disk and removed from the live memory.
-        Finally, if in this condition, also the data type of the matrix is self is changed: from float64 -> float32, with the same purpose.
-
-        :param D: np.array
-             data matrix D
-        :param FOLDER_OUT: str
-             folder in which the data (partitions and/or data matrix itself) will be eventually saved.
-        :param MEMORY_SAVING: bool, optional
-             If True, memory saving feature is activated. Passed through __init__
-        :param N_PARTITIONS: int
-             In memory saving environment, this parameter refers to the number of partitions to be applied
-             to the data matrix. If the number indicated by the user is not a multiple of the N_T
-             i.e.: if (N_T % N_PARTITIONS) !=0 - then an additional partition is introduced, that contains
-             the remaining columns
-        :param MR: bool, optional
-             If True, it removes the mean (per column) from each snapshot
-        :param SAVE_D: bool, optional
-             If True, the matrix D is saved into memory. If the Memory Saving feature is active, this is performed
-             by default.
-        :param FOLDER_IN: str, optional. Needed only if database=None
-             If the D matrix is not provided (database = None), read it from the path FOLDER_IN
-        :param filename: str, optional. Needed only if database=None
-             If the database is not provided, read it from the files filename
-             The files must be named "filenamexxxx.dat" where x is the number of the file
-             that goes from 0 to the number of time steps saved
-        :param h: int, optional. Needed only if database=None
-             Lines to be skipped from the header of filename
-        :param f: int, optional. Needed only if database=None
-             Lines to be skipped from the footer of filename
-        :param c: int, optional. Needed only if database=None
-             Columns to be skipped (for example if the first c columns contain the mesh grid.)
-        :param N: int, optional. Needed only if database=None
-             Components to be analysed.
-        :param N_S:  int, optional. Needed only if database=None
-             Number of points in space.
-        :param N_T: int, optional. Needed only if database=None
-             components to be analysed.
-
-    
-        :return:
-             There are four possible scenario:
-              1. if N_Partitions ==1 and MR = True, return is D,D_MEAN (the mean snapshot!)
-              2. if N_Partitions ==1 and MR = False, return is D.
-              3. if N_Partitions >1 and MR = True, return is D_MEAN
-              4. if N_Partitions >1 and MR=False, return is None
-        
-
-        """
-        
-        if isinstance(D, np.ndarray):  # D was already initialised
-            N_S = int(np.shape(D)[0])
-            N_T = int(np.shape(D)[1])
-            if MR:
-                '''Removing mean from data matrix'''
-
-                print("Removing the mean from D ...")
-                D_MEAN = np.mean(D, 1)  # Temporal average (along the columns)
-                D_Mr = D - np.array([D_MEAN, ] * N_T).transpose()  # Mean Removed
-                print("Computing the mean-removed D ... ")
-                np.copyto(D, D_Mr)                
-                del D_Mr
-
-            if N_PARTITIONS > 1:
-                '''Converting D into float32, applying partitions and saving all.'''
-                SAVE_D = True
-                database = D.astype('float32', casting='same_kind')
-                os.makedirs(FOLDER_OUT + "/data_partitions/", exist_ok=True)
-                print("Memory Saving feature is active. Partitioning Data Matrix...")
-                if N_T % N_PARTITIONS != 0:
-                    dim_col = math.floor(N_T / N_PARTITIONS)
-
-                    columns_to_part = dim_col * N_PARTITIONS
-                    splitted_tmp = np.hsplit(database[:, :columns_to_part], N_PARTITIONS)
-                    for ii in range(1, len(splitted_tmp) + 1):
-                        np.savez(FOLDER_OUT + f"/data_partitions/di_{ii}", di=splitted_tmp[ii - 1])
-
-                    np.savez(FOLDER_OUT + f"/data_partitions/di_{N_PARTITIONS + 1}",
-                             di=database[:, columns_to_part:])
-                else:
-                    splitted_tmp = np.hsplit(database, N_PARTITIONS)
-                    for ii in range(1, len(splitted_tmp) + 1):
-                        np.savez(FOLDER_OUT + f"/data_partitions/di_{ii}", di=splitted_tmp[ii - 1])
-
-                print("\n Data Matrix has been successfully splitted. \n")
-
-            if SAVE_D:
-                '''Saving data matrix in FOLDER_OUT'''
-                os.makedirs(FOLDER_OUT + "/data_matrix", exist_ok=True)
-                print(f"Saving the matrix D in {FOLDER_OUT}")
-                np.savez(FOLDER_OUT + '/data_matrix/database', D=database, n_t=N_T, n_s=N_S)
-        else:  # try to read the data
-            print("Data matrix was not provided, reading it from {}".format(FOLDER_IN))
-            # First check if the data were saved in the supported format
-            try:
-                Name = FOLDER_IN + os.sep + filename % (0 + 1) + '.dat'  # Name of the file to read
-                # Read data from a file
-                DATA = np.genfromtxt(Name, skip_header=h, skip_footer=f)  # Here we have the two colums
-            except:
-                raise AttributeError(
-                    "FOLDER_IN {} does not exist or filename {} has not the good format. Check the help!".format(
-                        FOLDER_IN, filename))
-
-            if N_PARTITIONS == 1:  # If you have only one partition (one matrix! )
-                D = np.zeros((N_S, N_T))
-
-                print("\n \n Importing data with no partitions... \n \n")
-
-                if MR:
-                    print("Mean removal activated")
-                    D_MEAN = np.zeros(N_S)
-
-                for k in tqdm(range(0, N_T)):
-                    Name = FOLDER_IN + os.sep + filename % (k + 1) + '.dat'  # Name of the file to read
-                    # Read data from a file
-                    DATA = np.genfromtxt(Name,  # usecols=np.arange(0, 2),
-                                         skip_header=h, skip_footer=f)  # Here we have the two colums
-                    # Dat = DATA[1:, :]  # Here we remove the first raw, containing the header
-                    for ii in range(c, N + c):
-                        tmp = DATA[:, ii]
-                        if ii == c:
-                            V = np.copy(tmp)
-                        else:
-                            V = np.concatenate([V, tmp], axis=0)
-                    if MR:
-                        D_MEAN += 1 / N_T * V  # Snapshot contribution to the mean
-
-                    D[:, k] = V  # Reshape and assign
-
-                if MR:
-                    print("Removing the mean from D ...")
-                    D_Mr = D - D_MEAN.reshape(-1, 1)  # Mean Removed
-                    print("Computing the mean-removed D ... ")
-                    np.copyto(D, D_Mr)
-                    del D_Mr
-
-            elif N_PARTITIONS > 1:  # then we enter in the memory saving loop
-                # prepare the folder to store the parittions
-                os.makedirs(FOLDER_OUT + "/data_partitions/", exist_ok=True)
-                print("Memory Saving feature is active. Partitioning Data Matrix...")
-
-                dim_col = math.floor(N_T / N_PARTITIONS)
-                columns_to_part = dim_col * N_PARTITIONS  # These are integer multiples of N_PARTITIONS
-                vec = np.arange(0, columns_to_part)
-                # This gets the blocks
-                splitted_tmp = np.hsplit(vec, N_PARTITIONS)
-                if columns_to_part != N_T:
-                    print("WARNING: the last " + str(
-                        N_T - 1 - splitted_tmp[N_PARTITIONS - 1][-1]) + ' snapshots are not considered')
-
-                if MR:
-                    print("Mean removal activated")
-                    D_MEAN = np.zeros(N_S)
-
-                for ii in range(1, len(splitted_tmp) + 1):
-                    count = 0
-                    print('Working on block ' + str(ii) + '/' + str(N_PARTITIONS))
-                    D = np.zeros((N_S, len(splitted_tmp[0])))
-                    i1 = splitted_tmp[ii - 1][0];
-                    i2 = splitted_tmp[ii - 1][-1]  # ranges
-                    for k in tqdm(range(i1, i2 + 1)):
-                        Name = FOLDER_IN + os.sep + filename % (k + 1) + '.dat'  # Name of the file to read
-                        DATA = np.genfromtxt(Name,  # usecols=np.arange(0, 2),
-                                             skip_header=h, skip_footer=f)  # Here we have the two colums
-                        for nn in range(c, N + c):
-                            tmp = DATA[:, nn]
-                            if nn == c:
-                                V = np.copy(tmp)
-                            else:
-                                V = np.concatenate([V, tmp], axis=0)
-
-                        if MR:
-                            D_MEAN += 1 / N_T * V  # Snapshot contribution to the mean
-
-                        D[:, count] = V  # Reshape and assign
-                        count += 1
-                    np.savez(FOLDER_OUT + f"/data_partitions/di_{ii}", di=D)
-                    print('Partition ' + str(ii) + '/' + str(N_PARTITIONS) + ' saved')
-
-                if MR:
-                    print('Reloading the data for removing the mean')
-                    for ii in range(1, len(splitted_tmp) + 1):
-                        print(f"Mean centering block {ii}")
-                        di = np.load(FOLDER_OUT + f"/data_partitions/di_{ii}.npz")['di']
-                        di_mr = di - D_MEAN.reshape(-1, 1)  # Mean Removed
-                        np.savez(FOLDER_OUT + f"/data_partitions/di_{ii}", di=di_mr)
-            else:
-                raise TypeError("number of partitions not valid.")
-
-        if (N_PARTITIONS ==1 and MR==True):
-         return D, D_MEAN  
-        elif (N_PARTITIONS ==1 and MR==False):
-         return D
-        elif (N_PARTITIONS >1 and MR==True):
-         return D_MEAN
-        else:
-          return None
-      
-'''
-    @classmethod
-    def from_xls(cls, filename, **kwargs):
-        """
-        This class method builds the df from an excel file.
-
-        work
-
-        """
-        ## TBD
-        return
-
-    @classmethod
-    def _from_csv(cls, folder, filename, N, N_S,
-                  h: int = 0, f: int = 0,
-                  c: int = 0):
-        """
-        This method imports data (in the specified format) and then assemblies the corresponding
-        data matrix, D.
-
-        :param folder: str 
-                Folder in which the data is stored
-        :param filename: str
-                Name of the files to be imported
-        :param N number of components: int
-                Components to be analysed
-        :param h: int 
-                Lines to be skipped from header
-        :param f: int
-                Lines to be skipped from footer
-        :param c: int
-                Columns to be skipped
-
-        :return: np.array
-                Assembled DataMarix
-
-        """
-        path, dirs, files = next(os.walk(folder))
-        files = [f for f in files if f.endswith('.csv')]
-        N_T = len(files)
-        D = np.zeros((N_S, N_T))
-
-        print("\n \n Importing data... \n \n")
-
-        for k in tqdm(range(0, N_T)):
-            Name = folder + files[k] #os.sep + filename % (k + 1) + '.csv'  # Name of the file to read
-            # Read data from a file
-            DATA = np.genfromtxt(Name,  # usecols=np.arange(0, 2),
-                                 skip_header=h, skip_footer=f)  # Here we have the two colums
-            # Dat = DATA[1:, :]  # Here we remove the first raw, containing the header
-            for ii in range(c, N + c):
-                tmp = DATA[:, ii]
-                if ii == c:
-                    V = np.copy(tmp)
-                else:
-                    V = np.concatenate([V, tmp], axis=0)
-
-            D[:, k] = V  # Reshape and assign
-
-        return D
-
-    @classmethod
-    def _from_txt(cls, folder, filename, N, N_S,
-                  h: int = 0, f: int = 0,
-                  c: int = 0):
-        """
-        This method imports data (in the specified format) and then assemblies the corresponding
-        data matrix, D.
-
-        :param folder: str 
-                Folder in which the data is stored
-        :param filename: str
-                Name of the files to be imported
-        :param N number of components: int
-                Components to be analysed
-        :param h: int 
-                Lines to be skipped from header
-        :param f: int
-                Lines to be skipped from footer
-        :param c: int
-                Columns to be skipped
-
-        :return: np.array
-                Assembled DataMarix
-
-        """
-        path, dirs, files = next(os.walk(folder))
-        N_T = len(files)
-        D = np.zeros((N_S, N_T))
-
-        print("\n \n Importing data... \n \n")
-
-        for k in tqdm(range(0, N_T)):
-            Name = folder + os.sep + filename % (k + 1) + '.txt'  # Name of the file to read
-            # Read data from a file
-            DATA = np.genfromtxt(Name,  # usecols=np.arange(0, 2),
-                                 skip_header=h, skip_footer=f)  # Here we have the two colums
-            # Dat = DATA[1:, :]  # Here we remove the first raw, containing the header
-            for ii in range(c, N + c):
-                tmp = DATA[:, ii]
-                if ii == c:
-                    V = np.copy(tmp)
-                else:
-                    V = np.concatenate([V, tmp], axis=0)
-
-            D[:, k] = V  # Reshape and assign
-
-        return D
-
-
-'''
-
-
-#%%
-
+import numpy as np
+import os
+from tqdm import tqdm
+import math
+
+
+class ReadData:
+    """
+    A MODULO helper class for input data.  ReadData allows to load the data directly before using MODULO, and
+    hence assembling the data matrix D from data.
+    """
+
+
+    def __init__(self):
+        pass
+
+
+    @classmethod
+    def _data_processing(cls,D: np.array, FOLDER_OUT: str='./',
+                   N_PARTITIONS: int = 1,
+                   MR: bool = False, SAVE_D: bool = False,
+                   FOLDER_IN: str = './', filename: str = '',
+                   h: int = 0, f: int = 0, c: int = 0,
+                   N: int = 0, N_S: int = 0, N_T: int = 0):
+        """
+        First, if the D matrix is not provided, this method attempts to load the data and assembles the D matrix.
+        Then, it performs pre-processing operations on the data matrix, D. if MR=True, the mean (per each column - i.e.: snapshot at time t_i) is removed;
+        If the MEMORY_SAVING=True the data matrix is splitted to optimize memory usage. Moreover, D is stored on disk and removed from the live memory.
+        Finally, if in this condition, also the data type of the matrix is self is changed: from float64 -> float32, with the same purpose.
+
+        :param D: np.array
+             data matrix D
+        :param FOLDER_OUT: str
+             folder in which the data (partitions and/or data matrix itself) will be eventually saved.
+        :param MEMORY_SAVING: bool, optional
+             If True, memory saving feature is activated. Passed through __init__
+        :param N_PARTITIONS: int
+             In memory saving environment, this parameter refers to the number of partitions to be applied
+             to the data matrix. If the number indicated by the user is not a multiple of the N_T
+             i.e.: if (N_T % N_PARTITIONS) !=0 - then an additional partition is introduced, that contains
+             the remaining columns
+        :param MR: bool, optional
+             If True, it removes the mean (per column) from each snapshot
+        :param SAVE_D: bool, optional
+             If True, the matrix D is saved into memory. If the Memory Saving feature is active, this is performed
+             by default.
+        :param FOLDER_IN: str, optional. Needed only if database=None
+             If the D matrix is not provided (database = None), read it from the path FOLDER_IN
+        :param filename: str, optional. Needed only if database=None
+             If the database is not provided, read it from the files filename
+             The files must be named "filenamexxxx.dat" where x is the number of the file
+             that goes from 0 to the number of time steps saved
+        :param h: int, optional. Needed only if database=None
+             Lines to be skipped from the header of filename
+        :param f: int, optional. Needed only if database=None
+             Lines to be skipped from the footer of filename
+        :param c: int, optional. Needed only if database=None
+             Columns to be skipped (for example if the first c columns contain the mesh grid.)
+        :param N: int, optional. Needed only if database=None
+             Components to be analysed.
+        :param N_S:  int, optional. Needed only if database=None
+             Number of points in space.
+        :param N_T: int, optional. Needed only if database=None
+             components to be analysed.
+
+    
+        :return:
+             There are four possible scenario:
+              1. if N_Partitions ==1 and MR = True, return is D,D_MEAN (the mean snapshot!)
+              2. if N_Partitions ==1 and MR = False, return is D.
+              3. if N_Partitions >1 and MR = True, return is D_MEAN
+              4. if N_Partitions >1 and MR=False, return is None
+        
+
+        """
+        
+        if isinstance(D, np.ndarray):  # D was already initialised
+            N_S = int(np.shape(D)[0])
+            N_T = int(np.shape(D)[1])
+            if MR:
+                '''Removing mean from data matrix'''
+
+                print("Removing the mean from D ...")
+                D_MEAN = np.mean(D, 1)  # Temporal average (along the columns)
+                D_Mr = D - np.array([D_MEAN, ] * N_T).transpose()  # Mean Removed
+                print("Computing the mean-removed D ... ")
+                np.copyto(D, D_Mr)                
+                del D_Mr
+
+            if N_PARTITIONS > 1:
+                '''Converting D into float32, applying partitions and saving all.'''
+                SAVE_D = True
+                database = D.astype('float32', casting='same_kind')
+                os.makedirs(FOLDER_OUT + "/data_partitions/", exist_ok=True)
+                print("Memory Saving feature is active. Partitioning Data Matrix...")
+                if N_T % N_PARTITIONS != 0:
+                    dim_col = math.floor(N_T / N_PARTITIONS)
+
+                    columns_to_part = dim_col * N_PARTITIONS
+                    splitted_tmp = np.hsplit(database[:, :columns_to_part], N_PARTITIONS)
+                    for ii in range(1, len(splitted_tmp) + 1):
+                        np.savez(FOLDER_OUT + f"/data_partitions/di_{ii}", di=splitted_tmp[ii - 1])
+
+                    np.savez(FOLDER_OUT + f"/data_partitions/di_{N_PARTITIONS + 1}",
+                             di=database[:, columns_to_part:])
+                else:
+                    splitted_tmp = np.hsplit(database, N_PARTITIONS)
+                    for ii in range(1, len(splitted_tmp) + 1):
+                        np.savez(FOLDER_OUT + f"/data_partitions/di_{ii}", di=splitted_tmp[ii - 1])
+
+                print("\n Data Matrix has been successfully splitted. \n")
+
+            if SAVE_D:
+                '''Saving data matrix in FOLDER_OUT'''
+                os.makedirs(FOLDER_OUT + "/data_matrix", exist_ok=True)
+                print(f"Saving the matrix D in {FOLDER_OUT}")
+                np.savez(FOLDER_OUT + '/data_matrix/database', D=database, n_t=N_T, n_s=N_S)
+        else:  # try to read the data
+            print("Data matrix was not provided, reading it from {}".format(FOLDER_IN))
+            # First check if the data were saved in the supported format
+            try:
+                Name = FOLDER_IN + os.sep + filename % (0 + 1) + '.dat'  # Name of the file to read
+                # Read data from a file
+                DATA = np.genfromtxt(Name, skip_header=h, skip_footer=f)  # Here we have the two colums
+            except:
+                raise AttributeError(
+                    "FOLDER_IN {} does not exist or filename {} has not the good format. Check the help!".format(
+                        FOLDER_IN, filename))
+
+            if N_PARTITIONS == 1:  # If you have only one partition (one matrix! )
+                D = np.zeros((N_S, N_T))
+
+                print("\n \n Importing data with no partitions... \n \n")
+
+                if MR:
+                    print("Mean removal activated")
+                    D_MEAN = np.zeros(N_S)
+
+                for k in tqdm(range(0, N_T)):
+                    Name = FOLDER_IN + os.sep + filename % (k + 1) + '.dat'  # Name of the file to read
+                    # Read data from a file
+                    DATA = np.genfromtxt(Name,  # usecols=np.arange(0, 2),
+                                         skip_header=h, skip_footer=f)  # Here we have the two colums
+                    # Dat = DATA[1:, :]  # Here we remove the first raw, containing the header
+                    for ii in range(c, N + c):
+                        tmp = DATA[:, ii]
+                        if ii == c:
+                            V = np.copy(tmp)
+                        else:
+                            V = np.concatenate([V, tmp], axis=0)
+                    if MR:
+                        D_MEAN += 1 / N_T * V  # Snapshot contribution to the mean
+
+                    D[:, k] = V  # Reshape and assign
+
+                if MR:
+                    print("Removing the mean from D ...")
+                    D_Mr = D - D_MEAN.reshape(-1, 1)  # Mean Removed
+                    print("Computing the mean-removed D ... ")
+                    np.copyto(D, D_Mr)
+                    del D_Mr
+
+            elif N_PARTITIONS > 1:  # then we enter in the memory saving loop
+                # prepare the folder to store the parittions
+                os.makedirs(FOLDER_OUT + "/data_partitions/", exist_ok=True)
+                print("Memory Saving feature is active. Partitioning Data Matrix...")
+
+                dim_col = math.floor(N_T / N_PARTITIONS)
+                columns_to_part = dim_col * N_PARTITIONS  # These are integer multiples of N_PARTITIONS
+                vec = np.arange(0, columns_to_part)
+                # This gets the blocks
+                splitted_tmp = np.hsplit(vec, N_PARTITIONS)
+                if columns_to_part != N_T:
+                    print("WARNING: the last " + str(
+                        N_T - 1 - splitted_tmp[N_PARTITIONS - 1][-1]) + ' snapshots are not considered')
+
+                if MR:
+                    print("Mean removal activated")
+                    D_MEAN = np.zeros(N_S)
+
+                for ii in range(1, len(splitted_tmp) + 1):
+                    count = 0
+                    print('Working on block ' + str(ii) + '/' + str(N_PARTITIONS))
+                    D = np.zeros((N_S, len(splitted_tmp[0])))
+                    i1 = splitted_tmp[ii - 1][0];
+                    i2 = splitted_tmp[ii - 1][-1]  # ranges
+                    for k in tqdm(range(i1, i2 + 1)):
+                        Name = FOLDER_IN + os.sep + filename % (k + 1) + '.dat'  # Name of the file to read
+                        DATA = np.genfromtxt(Name,  # usecols=np.arange(0, 2),
+                                             skip_header=h, skip_footer=f)  # Here we have the two colums
+                        for nn in range(c, N + c):
+                            tmp = DATA[:, nn]
+                            if nn == c:
+                                V = np.copy(tmp)
+                            else:
+                                V = np.concatenate([V, tmp], axis=0)
+
+                        if MR:
+                            D_MEAN += 1 / N_T * V  # Snapshot contribution to the mean
+
+                        D[:, count] = V  # Reshape and assign
+                        count += 1
+                    np.savez(FOLDER_OUT + f"/data_partitions/di_{ii}", di=D)
+                    print('Partition ' + str(ii) + '/' + str(N_PARTITIONS) + ' saved')
+
+                if MR:
+                    print('Reloading the data for removing the mean')
+                    for ii in range(1, len(splitted_tmp) + 1):
+                        print(f"Mean centering block {ii}")
+                        di = np.load(FOLDER_OUT + f"/data_partitions/di_{ii}.npz")['di']
+                        di_mr = di - D_MEAN.reshape(-1, 1)  # Mean Removed
+                        np.savez(FOLDER_OUT + f"/data_partitions/di_{ii}", di=di_mr)
+            else:
+                raise TypeError("number of partitions not valid.")
+
+        if (N_PARTITIONS ==1 and MR==True):
+         return D, D_MEAN  
+        elif (N_PARTITIONS ==1 and MR==False):
+         return D
+        elif (N_PARTITIONS >1 and MR==True):
+         return D_MEAN
+        else:
+          return None
+      
+'''
+    @classmethod
+    def from_xls(cls, filename, **kwargs):
+        """
+        This class method builds the df from an excel file.
+
+        work
+
+        """
+        ## TBD
+        return
+
+    @classmethod
+    def _from_csv(cls, folder, filename, N, N_S,
+                  h: int = 0, f: int = 0,
+                  c: int = 0):
+        """
+        This method imports data (in the specified format) and then assemblies the corresponding
+        data matrix, D.
+
+        :param folder: str 
+                Folder in which the data is stored
+        :param filename: str
+                Name of the files to be imported
+        :param N number of components: int
+                Components to be analysed
+        :param h: int 
+                Lines to be skipped from header
+        :param f: int
+                Lines to be skipped from footer
+        :param c: int
+                Columns to be skipped
+
+        :return: np.array
+                Assembled DataMarix
+
+        """
+        path, dirs, files = next(os.walk(folder))
+        files = [f for f in files if f.endswith('.csv')]
+        N_T = len(files)
+        D = np.zeros((N_S, N_T))
+
+        print("\n \n Importing data... \n \n")
+
+        for k in tqdm(range(0, N_T)):
+            Name = folder + files[k] #os.sep + filename % (k + 1) + '.csv'  # Name of the file to read
+            # Read data from a file
+            DATA = np.genfromtxt(Name,  # usecols=np.arange(0, 2),
+                                 skip_header=h, skip_footer=f)  # Here we have the two colums
+            # Dat = DATA[1:, :]  # Here we remove the first raw, containing the header
+            for ii in range(c, N + c):
+                tmp = DATA[:, ii]
+                if ii == c:
+                    V = np.copy(tmp)
+                else:
+                    V = np.concatenate([V, tmp], axis=0)
+
+            D[:, k] = V  # Reshape and assign
+
+        return D
+
+    @classmethod
+    def _from_txt(cls, folder, filename, N, N_S,
+                  h: int = 0, f: int = 0,
+                  c: int = 0):
+        """
+        This method imports data (in the specified format) and then assemblies the corresponding
+        data matrix, D.
+
+        :param folder: str 
+                Folder in which the data is stored
+        :param filename: str
+                Name of the files to be imported
+        :param N number of components: int
+                Components to be analysed
+        :param h: int 
+                Lines to be skipped from header
+        :param f: int
+                Lines to be skipped from footer
+        :param c: int
+                Columns to be skipped
+
+        :return: np.array
+                Assembled DataMarix
+
+        """
+        path, dirs, files = next(os.walk(folder))
+        N_T = len(files)
+        D = np.zeros((N_S, N_T))
+
+        print("\n \n Importing data... \n \n")
+
+        for k in tqdm(range(0, N_T)):
+            Name = folder + os.sep + filename % (k + 1) + '.txt'  # Name of the file to read
+            # Read data from a file
+            DATA = np.genfromtxt(Name,  # usecols=np.arange(0, 2),
+                                 skip_header=h, skip_footer=f)  # Here we have the two colums
+            # Dat = DATA[1:, :]  # Here we remove the first raw, containing the header
+            for ii in range(c, N + c):
+                tmp = DATA[:, ii]
+                if ii == c:
+                    V = np.copy(tmp)
+                else:
+                    V = np.concatenate([V, tmp], axis=0)
+
+            D[:, k] = V  # Reshape and assign
+
+        return D
+
+
+'''
+
+
+#%%
+
```

### Comparing `modulo_vki-2.0.4/modulo_vki.egg-info/PKG-INFO` & `modulo_vki-2.0.5/modulo_vki.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-Metadata-Version: 2.1
-Name: modulo_vki
-Version: 2.0.4
-Summary: MODULO (MODal mULtiscale pOd) is a software developed at the von Karman Institute to perform Multiscale Modal Analysis of numerical and experimental data.
-Home-page: https://github.com/mendezVKI/MODULO/tree/master/modulo_python_package/
-Author: ['R. Poletti', 'L. Schena', 'D. Ninni', 'M. A. Mendez']
-Author-email: mendez@vki.ac.be
-License: BSD (3-clause)
-Classifier: Development Status :: 4 - Beta
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: tqdm
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: scikit-learn
-Requires-Dist: ipykernel
-Requires-Dist: ipython
-Requires-Dist: ipython-genutils
-Requires-Dist: ipywidgets
-Requires-Dist: matplotlib
-
-
-
-MODULO - latest update 2.0
-===================
-
-This repository contains version 2.0 of MODULO (MODal mULtiscale pOd), a software developed at the von Karman Institute to perform data-driven modal decompositions and, in particular, the Multiscale Proper Orthogonal Decomposition (mPOD).
-
-The old version based on MATLAB implementation and related GUI is no longer maintained but will remain available on the branch "Old_Matlab_Implementation". We also keep the first Python implementation in the branch "Old_Python_Implementation". See the Readme file in these branches for more information.
-
-#### Documentation
-
-The full documentation is available at https://modulo.readthedocs.io/en/latest/intro.html.
-This documentation is stored alongside the source code and linked to a specific version of MODULO.
-
-## What is MODULO, and what are data-driven decompositions?
-
-MODULO allows to compute data-driven decompositions of experimental and numerical data. To have a concise overview of the context, we refer to: 
-
-- Ninni, D., Mendez, M. A. (2020), "MODULO: A Software for Multiscale Proper Orthogonal Decomposition of data", Software X, Vol 12, 100622, https://doi.org/10.1016/j.softx.2020.100622.
-
-- Poletti, R., Schena, L., Ninni, D., Mendez, M.A (2024) "MODULO: a python toolbox for data-driven modal decomposition", Submitted to Journal of Open Source Software. Preprint available [here](https://www.researchgate.net/publication/376885484_MODULO_a_python_toolbox_for_data-driven_modal_decomposition)
-
-The first article also presents the first version of MODULO (available in the OLD_Matlab_Implementation branch) and its GUI developed by D. Ninni. The second introduces MODULO v2 in this branch and alternative open source projects. While many projects allows for computing common decompositions such as POD, DMD and the SPODs, MODULO is currently the only opensource project allowing to compute the mPOD.
-
-For a more comprehensive overview on the theory of data-driven decompositions, we refer to the chapter:
-
-- Mendez, M. A. (2023) "Generalized and Multiscale Modal Analysis". In : Mendez M.A., Ianiro, A., Noack, B.R., Brunton, S. L. (Eds), "Data-Driven Fluid Mechanics: Combining First Principles and Machine Learning". Cambridge University Press, 2023:153-181. https://doi.org/10.1017/9781108896214.013. The pre-print is available at https://arxiv.org/abs/2208.12630. 
-
-and the article that first presented the complete treatment of the mPOD :
-
-- Mendez, M. A., Balabane, M., Buchlin, J.-M. (2019) "Multi-Scale Proper Orthogonal Decomposition of Complex Fluid Flows" Journal of Fluid Mechanics 870:988-1036, https://doi.org/10.1017/9781108896214.013. The pre-print is available at https://arxiv.org/abs/2208.12630. 
-
-Ongoing works on nonlinear methods are discussed here:
-
-- Mendez, M. A. (2023) "Linear and Nonlinear Dimensionality Reduction from Fluid Mechanics to Machine Learning", Meas. Sci. Technol. 34(042001), https://doi.org/10.1088/1361-6501/acaffe. The pre-print is available at https://arxiv.org/abs/2208.07746.   
-
-## What is new in this V 2.0? 
-
-This version expands considerably the version v1 in "Old_Python_Implementation", for which a first tutorial was provided by L. Schena in https://www.youtube.com/watch?v=y2uSvdxAwHk. 
-The major updates are the following :
-
-1. Faster EIG/SVD algorithms, using powerful randomized svd solvers from scikit_learn (see [this](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.TruncatedSVD.html) and [this](https://scikit-learn.org/stable/modules/generated/sklearn.utils.extmath.randomized_svd.html) ). It is now possible to select various options as "eig_solver" and "svd_solver", offering different trade-offs in terms of accuracy vs computational time.
-
-2. In addition to the traditional POD computation using the K matrix (Sirovinch's method), it is now possible to compute the POD directly via SVD using any of the four "svd_solver" options.
-This is generally faster but requires more memory.
-
-3. Faster subscale estimators for the mPOD: the previous version used the rank of the correlation matrix in each scale to define the number of modes to be computed in each portion of the splitting vector before assembling the full basis. This is computationally very demanding. This estimation has been replaced by a frequency-based threshold (i.e. based on the frequency bins within each portion) since one can show that the frequency-based estimator is always more "conservative" than the rank-based estimator.
-
-4. Major improvement on the memory saving option: the previous version of modulo always required in input the matrix D. Then, if the memory saving option was active, the matrix was partitioned and stored locally to free the RAM before computing the correlation matrix (see [this tutorial by D. Ninni](https://www.youtube.com/watch?v=LclxO1WTuao)). In the new version, it is possible to initialize a modulo object *without* the matrix D (see exercise 5 in the examples). Instead, one can create the partitions without loading the matrix D.
-
-5. Implementation of Dynamic Mode Decomposition (DMD) from [Schmid, P.J 2010](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/dynamic-mode-decomposition-of-numerical-and-experimental-data/AA4C763B525515AD4521A6CC5E10DBD4).
-
-6. Implementation of the two Spectral POD formulations, namely the one from [Sieber et al 2016](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/abs/spectral-proper-orthogonal-decomposition/DCD8A6EDEFD56F5A9715DBAD38BD461A), and the one from [Towne et al 2018](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/abs/spectral-proper-orthogonal-decomposition-and-its-relationship-to-dynamic-mode-decomposition-and-resolvent-analysis/EC2A6DF76490A0B9EB208CC2CA037717)
-
-7. Implementation of a kernel version of the POD, in which the correlation matrix is replaced by a kernel matrix. This is described in Lecture 15 of the course [Hands on Machine Learning for Fluid dynamics 2023](https://www.vki.ac.be/index.php/events-ls/events/eventdetail/552/-/online-on-site-hands-on-machine-learning-for-fluid-dynamics-2023). See also [this](https://arxiv.org/abs/2208.07746).
-
-8. Implementation of a formulation for non-uniform meshes, using a weighted matrix for all the relevant inner products. This is currently available only for POD and mPOD but allows for handling data produced from CFD simulation without resampling on a uniform grid (see exercise 4). It can be used both with and without the memory-saving option.
-
-## New Tutorials 
-
-The installation provides five exercises to explore MODULO's features while familiarizing with data-driven decompositions. These are available in the /exercise/ folder in plain Python format and jupyter notebooks. 
-
-- Exercise 1. In this exercise, we consider the flow past a cylinder. The dataset was created via Large Eddy Simulations (LES) by Denis Dumoulin during his STP at VKI in 2016 (Report available on request). For convenience, the data was first mapped to a Cartesian grid. This test case is by far the most popular because it's well-known to have a simple low-order representation with modes that have nearly harmonic temporal structures. We compute the POD and the DMD and compare the results... the difference between DMD and POD modes is hardly distinguishable!
-
-- Exercise 2. We consider the flow of an impinging gas jet, taken from [this](https://arxiv.org/abs/1804.09646) paper. This dataset was collected via Time-Resolved Particle Image Velocimetry (TR-PIV). Only the first 200 POD modes were stored. This dataset has much richer dynamics than the previous one and cannot be easily approximated using a few modes. We use it to explore the differences between the DFT, the SPODs and the mPOD. These have different purposes and look for different features.
-
-- Exercise 3. We take back the cylinder test case to explore the differences between the POD and the generalized Karhunen–Loève (KL) expansion in which a kernel matrix replaces the correlation matrix. The POD is a particular case of KL where the kernel function generating the kernel matrix is the plain inner product. Here, we also consider a Gaussian kernel. Different kernel functions define similarity in different ways and thus produce widely different modes. Different modal structures tell different stories about the dataset, but... what can you say about efficiency in data compression? 
-
-- Exercise 4. We consider the flow past a cylinder again, but this time in transient conditions and on an experimental test case taken from [this](https://arxiv.org/abs/2001.01971) paper. In this exercise, you can reproduce the same results from the article to see how the mPOD allows to achieve both time and frequency localization without compromising much of the convergence of the POD. The dataset is quite large, so you might have difficulties handling it if you have less than 32 GB of RAM. But fear not: the memory saving feature allows to compute POD and mPOD without loading the data into memory!
-
-- Exercise 5. We consider the flow of an impinging gas jet again, but this time on a numerical test case. This dataset was produced by Yannic Lowenstein during his STP at VKI at the end of 2023, with the help of Dr. Maria Faruoli. The Reynolds number is two orders of magnitude higher than in exercise 2, yet the flow features you will observe are pretty similar, at least qualitatively. From a learning perspective, the key feature of this test case is that the data is not available on a uniform grid. But fear not: with the new features, it is possible to compute the decompositions using appropriate weights!
- 
+Metadata-Version: 2.1
+Name: modulo_vki
+Version: 2.0.5
+Summary: MODULO (MODal mULtiscale pOd) is a software developed at the von Karman Institute to perform Multiscale Modal Analysis of numerical and experimental data.
+Home-page: https://github.com/mendezVKI/MODULO/tree/master/modulo_python_package/
+Author: ['R. Poletti', 'L. Schena', 'D. Ninni', 'M. A. Mendez']
+Author-email: mendez@vki.ac.be
+License: BSD (3-clause)
+Classifier: Development Status :: 4 - Beta
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: tqdm
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+Requires-Dist: ipykernel
+Requires-Dist: ipython
+Requires-Dist: ipython-genutils
+Requires-Dist: ipywidgets
+Requires-Dist: matplotlib
+
+
+
+MODULO - latest update 2.0
+===================
+
+This repository contains version 2.0 of MODULO (MODal mULtiscale pOd), a software developed at the von Karman Institute to perform data-driven modal decompositions and, in particular, the Multiscale Proper Orthogonal Decomposition (mPOD).
+
+The old version based on MATLAB implementation and related GUI is no longer maintained but will remain available on the branch "Old_Matlab_Implementation". We also keep the first Python implementation in the branch "Old_Python_Implementation". See the Readme file in these branches for more information.
+
+#### Documentation
+
+The full documentation is available at https://modulo.readthedocs.io/en/latest/intro.html.
+This documentation is stored alongside the source code and linked to a specific version of MODULO.
+
+## What is MODULO, and what are data-driven decompositions?
+
+MODULO allows to compute data-driven decompositions of experimental and numerical data. To have a concise overview of the context, we refer to: 
+
+- Ninni, D., Mendez, M. A. (2020), "MODULO: A Software for Multiscale Proper Orthogonal Decomposition of data", Software X, Vol 12, 100622, https://doi.org/10.1016/j.softx.2020.100622.
+
+- Poletti, R., Schena, L., Ninni, D., Mendez, M.A (2024) "MODULO: a python toolbox for data-driven modal decomposition", Submitted to Journal of Open Source Software. Preprint available [here](https://www.researchgate.net/publication/376885484_MODULO_a_python_toolbox_for_data-driven_modal_decomposition)
+
+The first article also presents the first version of MODULO (available in the OLD_Matlab_Implementation branch) and its GUI developed by D. Ninni. The second introduces MODULO v2 in this branch and alternative open source projects. While many projects allows for computing common decompositions such as POD, DMD and the SPODs, MODULO is currently the only opensource project allowing to compute the mPOD.
+
+For a more comprehensive overview on the theory of data-driven decompositions, we refer to the chapter:
+
+- Mendez, M. A. (2023) "Generalized and Multiscale Modal Analysis". In : Mendez M.A., Ianiro, A., Noack, B.R., Brunton, S. L. (Eds), "Data-Driven Fluid Mechanics: Combining First Principles and Machine Learning". Cambridge University Press, 2023:153-181. https://doi.org/10.1017/9781108896214.013. The pre-print is available at https://arxiv.org/abs/2208.12630. 
+
+and the article that first presented the complete treatment of the mPOD :
+
+- Mendez, M. A., Balabane, M., Buchlin, J.-M. (2019) "Multi-Scale Proper Orthogonal Decomposition of Complex Fluid Flows" Journal of Fluid Mechanics 870:988-1036, https://doi.org/10.1017/9781108896214.013. The pre-print is available at https://arxiv.org/abs/2208.12630. 
+
+Ongoing works on nonlinear methods are discussed here:
+
+- Mendez, M. A. (2023) "Linear and Nonlinear Dimensionality Reduction from Fluid Mechanics to Machine Learning", Meas. Sci. Technol. 34(042001), https://doi.org/10.1088/1361-6501/acaffe. The pre-print is available at https://arxiv.org/abs/2208.07746.   
+
+## What is new in this V 2.0? 
+
+This version expands considerably the version v1 in "Old_Python_Implementation", for which a first tutorial was provided by L. Schena in https://www.youtube.com/watch?v=y2uSvdxAwHk. 
+The major updates are the following :
+
+1. Faster EIG/SVD algorithms, using powerful randomized svd solvers from scikit_learn (see [this](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.TruncatedSVD.html) and [this](https://scikit-learn.org/stable/modules/generated/sklearn.utils.extmath.randomized_svd.html) ). It is now possible to select various options as "eig_solver" and "svd_solver", offering different trade-offs in terms of accuracy vs computational time.
+
+2. In addition to the traditional POD computation using the K matrix (Sirovinch's method), it is now possible to compute the POD directly via SVD using any of the four "svd_solver" options.
+This is generally faster but requires more memory.
+
+3. Faster subscale estimators for the mPOD: the previous version used the rank of the correlation matrix in each scale to define the number of modes to be computed in each portion of the splitting vector before assembling the full basis. This is computationally very demanding. This estimation has been replaced by a frequency-based threshold (i.e. based on the frequency bins within each portion) since one can show that the frequency-based estimator is always more "conservative" than the rank-based estimator.
+
+4. Major improvement on the memory saving option: the previous version of modulo always required in input the matrix D. Then, if the memory saving option was active, the matrix was partitioned and stored locally to free the RAM before computing the correlation matrix (see [this tutorial by D. Ninni](https://www.youtube.com/watch?v=LclxO1WTuao)). In the new version, it is possible to initialize a modulo object *without* the matrix D (see exercise 5 in the examples). Instead, one can create the partitions without loading the matrix D.
+
+5. Implementation of Dynamic Mode Decomposition (DMD) from [Schmid, P.J 2010](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/dynamic-mode-decomposition-of-numerical-and-experimental-data/AA4C763B525515AD4521A6CC5E10DBD4).
+
+6. Implementation of the two Spectral POD formulations, namely the one from [Sieber et al 2016](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/abs/spectral-proper-orthogonal-decomposition/DCD8A6EDEFD56F5A9715DBAD38BD461A), and the one from [Towne et al 2018](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/abs/spectral-proper-orthogonal-decomposition-and-its-relationship-to-dynamic-mode-decomposition-and-resolvent-analysis/EC2A6DF76490A0B9EB208CC2CA037717)
+
+7. Implementation of a kernel version of the POD, in which the correlation matrix is replaced by a kernel matrix. This is described in Lecture 15 of the course [Hands on Machine Learning for Fluid dynamics 2023](https://www.vki.ac.be/index.php/events-ls/events/eventdetail/552/-/online-on-site-hands-on-machine-learning-for-fluid-dynamics-2023). See also [this](https://arxiv.org/abs/2208.07746).
+
+8. Implementation of a formulation for non-uniform meshes, using a weighted matrix for all the relevant inner products. This is currently available only for POD and mPOD but allows for handling data produced from CFD simulation without resampling on a uniform grid (see exercise 4). It can be used both with and without the memory-saving option.
+
+## New Tutorials 
+
+The installation provides five exercises to explore MODULO's features while familiarizing with data-driven decompositions. These are available in the /exercise/ folder in plain Python format and jupyter notebooks. 
+
+- Exercise 1. In this exercise, we consider the flow past a cylinder. The dataset was created via Large Eddy Simulations (LES) by Denis Dumoulin during his STP at VKI in 2016 (Report available on request). For convenience, the data was first mapped to a Cartesian grid. This test case is by far the most popular because it's well-known to have a simple low-order representation with modes that have nearly harmonic temporal structures. We compute the POD and the DMD and compare the results... the difference between DMD and POD modes is hardly distinguishable!
+
+- Exercise 2. We consider the flow of an impinging gas jet, taken from [this](https://arxiv.org/abs/1804.09646) paper. This dataset was collected via Time-Resolved Particle Image Velocimetry (TR-PIV). Only the first 200 POD modes were stored. This dataset has much richer dynamics than the previous one and cannot be easily approximated using a few modes. We use it to explore the differences between the DFT, the SPODs and the mPOD. These have different purposes and look for different features.
+
+- Exercise 3. We take back the cylinder test case to explore the differences between the POD and the generalized Karhunen–Loève (KL) expansion in which a kernel matrix replaces the correlation matrix. The POD is a particular case of KL where the kernel function generating the kernel matrix is the plain inner product. Here, we also consider a Gaussian kernel. Different kernel functions define similarity in different ways and thus produce widely different modes. Different modal structures tell different stories about the dataset, but... what can you say about efficiency in data compression? 
+
+- Exercise 4. We consider the flow past a cylinder again, but this time in transient conditions and on an experimental test case taken from [this](https://arxiv.org/abs/2001.01971) paper. In this exercise, you can reproduce the same results from the article to see how the mPOD allows to achieve both time and frequency localization without compromising much of the convergence of the POD. The dataset is quite large, so you might have difficulties handling it if you have less than 32 GB of RAM. But fear not: the memory saving feature allows to compute POD and mPOD without loading the data into memory!
+
+- Exercise 5. We consider the flow of an impinging gas jet again, but this time on a numerical test case. This dataset was produced by Yannic Lowenstein during his STP at VKI at the end of 2023, with the help of Dr. Maria Faruoli. The Reynolds number is two orders of magnitude higher than in exercise 2, yet the flow features you will observe are pretty similar, at least qualitatively. From a learning perspective, the key feature of this test case is that the data is not available on a uniform grid. But fear not: with the new features, it is possible to compute the decompositions using appropriate weights!
+
```

### Comparing `modulo_vki-2.0.4/modulo_vki.egg-info/SOURCES.txt` & `modulo_vki-2.0.5/modulo_vki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modulo_vki-2.0.4/setup.py` & `modulo_vki-2.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from os import path
-from setuptools import setup, find_packages
-import sys
-
-# NOTE: This file must remain Python 2 compatible for the foreseeable future,
-# to ensure that we error out properly for people with outdated setuptools
-# and/or pip.
-min_version = (3, 6)
-if sys.version_info < min_version:
-    error = """
-modulo_vki does not support Python {0}.{1}.
-Python {2}.{3} and above is required. Check your Python version like so:
-
-python3 --version
-
-This may be due to an out-of-date pip. Make sure you have pip >= 9.0.1.
-Upgrade pip like so:
-
-pip install --upgrade pip
-""".format(*(sys.version_info[:2] + min_version))
-    sys.exit(error)
-
-here = path.abspath(path.dirname(__file__))
-
-with open(path.join(here, 'README.md'), encoding='utf-8') as readme_file:
-    readme = readme_file.read()
-
-# with open(path.join(here, 'requirements.txt')) as requirements_file:
-#     # Parse requirements.txt, ignoring any commented-out lines.
-#     requirements = [line for line in requirements_file.read().splitlines()
-#                     if not line.startswith('#')]
-
-
-setup(
-    name='modulo_vki',
-    version='2.0.4',
-    description="MODULO (MODal mULtiscale pOd) is a software developed at the von Karman Institute to perform "
-                "Multiscale Modal Analysis of numerical and experimental data.",
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    author=["R. Poletti","L. Schena", "D. Ninni", "M. A. Mendez"],
-    author_email='mendez@vki.ac.be',
-    url='https://github.com/mendezVKI/MODULO/tree/master/modulo_python_package/',
-    python_requires='>={}'.format('.'.join(str(n) for n in min_version)),
-    packages=find_packages(exclude=['docs', 'tests']),
-    entry_points={
-        'console_scripts': [
-            # 'command = some.module:some_function',
-        ],
-    },
-    include_package_data=True,
-    package_data={
-        'modulo': [
-            # When adding files here, remember to update MANIFEST.in as well,
-            # or else they will not be included in the distribution on PyPI!
-            # 'path/to/data_file',
-        ]
-    },
-    install_requires=[
-        "tqdm",
-        "numpy",
-        "scipy",
-        "scikit-learn",
-        "ipykernel",
-        "ipython",
-        "ipython-genutils",
-        "ipywidgets",
-        "matplotlib",
-    ],
-    extra_requires={
-        'tutorials': [
-            "pyvista",
-            "imageio",
-        ]
-    },
-    license='BSD (3-clause)',
-    classifiers=[
-        'Development Status :: 4 - Beta',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-    ],
-)
+from os import path
+from setuptools import setup, find_packages
+import sys
+
+# NOTE: This file must remain Python 2 compatible for the foreseeable future,
+# to ensure that we error out properly for people with outdated setuptools
+# and/or pip.
+min_version = (3, 6)
+if sys.version_info < min_version:
+    error = """
+modulo_vki does not support Python {0}.{1}.
+Python {2}.{3} and above is required. Check your Python version like so:
+
+python3 --version
+
+This may be due to an out-of-date pip. Make sure you have pip >= 9.0.1.
+Upgrade pip like so:
+
+pip install --upgrade pip
+""".format(*(sys.version_info[:2] + min_version))
+    sys.exit(error)
+
+here = path.abspath(path.dirname(__file__))
+
+with open(path.join(here, 'README.md'), encoding='utf-8') as readme_file:
+    readme = readme_file.read()
+
+# with open(path.join(here, 'requirements.txt')) as requirements_file:
+#     # Parse requirements.txt, ignoring any commented-out lines.
+#     requirements = [line for line in requirements_file.read().splitlines()
+#                     if not line.startswith('#')]
+
+
+setup(
+    name='modulo_vki',
+    version='2.0.5',
+    description="MODULO (MODal mULtiscale pOd) is a software developed at the von Karman Institute to perform "
+                "Multiscale Modal Analysis of numerical and experimental data.",
+    long_description=readme,
+    long_description_content_type='text/markdown',
+    author=["R. Poletti","L. Schena", "D. Ninni", "M. A. Mendez"],
+    author_email='mendez@vki.ac.be',
+    url='https://github.com/mendezVKI/MODULO/tree/master/modulo_python_package/',
+    python_requires='>={}'.format('.'.join(str(n) for n in min_version)),
+    packages=find_packages(exclude=['docs', 'tests']),
+    entry_points={
+        'console_scripts': [
+            # 'command = some.module:some_function',
+        ],
+    },
+    include_package_data=True,
+    package_data={
+        'modulo': [
+            # When adding files here, remember to update MANIFEST.in as well,
+            # or else they will not be included in the distribution on PyPI!
+            # 'path/to/data_file',
+        ]
+    },
+    install_requires=[
+        "tqdm",
+        "numpy",
+        "scipy",
+        "scikit-learn",
+        "ipykernel",
+        "ipython",
+        "ipython-genutils",
+        "ipywidgets",
+        "matplotlib",
+    ],
+    extra_requires={
+        'tutorials': [
+            "pyvista",
+            "imageio",
+        ]
+    },
+    license='BSD (3-clause)',
+    classifiers=[
+        'Development Status :: 4 - Beta',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3',
+    ],
+)
```

