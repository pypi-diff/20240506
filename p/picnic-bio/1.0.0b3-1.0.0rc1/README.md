# Comparing `tmp/picnic_bio-1.0.0b3.tar.gz` & `tmp/picnic_bio-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picnic_bio-1.0.0b3.tar", last modified: Tue Apr 16 07:06:22 2024, max compression
+gzip compressed data, was "picnic_bio-1.0.0rc1.tar", last modified: Mon May  6 12:55:35 2024, max compression
```

## Comparing `picnic_bio-1.0.0b3.tar` & `picnic_bio-1.0.0rc1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-04-16 07:06:22.212587 picnic_bio-1.0.0b3/
--rw-r--r--   0 maxim      (502) staff       (20)     1514 2023-10-11 14:32:47.000000 picnic_bio-1.0.0b3/LICENSE
--rw-r--r--   0 maxim      (502) staff       (20)     9662 2024-04-16 07:06:22.212250 picnic_bio-1.0.0b3/PKG-INFO
--rw-r--r--   0 maxim      (502) staff       (20)    11501 2024-04-16 07:05:26.000000 picnic_bio-1.0.0b3/README.md
-drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-04-16 07:06:22.211485 picnic_bio-1.0.0b3/picnic_bio.egg-info/
--rw-r--r--   0 maxim      (502) staff       (20)     9662 2024-04-16 07:06:22.000000 picnic_bio-1.0.0b3/picnic_bio.egg-info/PKG-INFO
--rw-r--r--   0 maxim      (502) staff       (20)     1132 2024-04-16 07:06:22.000000 picnic_bio-1.0.0b3/picnic_bio.egg-info/SOURCES.txt
--rw-r--r--   0 maxim      (502) staff       (20)        1 2024-04-16 07:06:22.000000 picnic_bio-1.0.0b3/picnic_bio.egg-info/dependency_links.txt
--rw-r--r--   0 maxim      (502) staff       (20)       48 2024-04-16 07:06:22.000000 picnic_bio-1.0.0b3/picnic_bio.egg-info/entry_points.txt
--rw-r--r--   0 maxim      (502) staff       (20)      103 2024-04-16 07:06:22.000000 picnic_bio-1.0.0b3/picnic_bio.egg-info/requires.txt
--rw-r--r--   0 maxim      (502) staff       (20)       11 2024-04-16 07:06:22.000000 picnic_bio-1.0.0b3/picnic_bio.egg-info/top_level.txt
--rw-r--r--   0 maxim      (502) staff       (20)      182 2023-10-11 14:32:47.000000 picnic_bio-1.0.0b3/pyproject.toml
--rw-r--r--   0 maxim      (502) staff       (20)      528 2024-04-16 07:06:22.213392 picnic_bio-1.0.0b3/setup.cfg
--rw-r--r--   0 maxim      (502) staff       (20)     2228 2024-04-16 06:01:58.000000 picnic_bio-1.0.0b3/setup.py
-drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-04-16 07:06:22.158036 picnic_bio-1.0.0b3/src/
--rw-r--r--   0 maxim      (502) staff       (20)        0 2023-10-11 14:32:47.000000 picnic_bio-1.0.0b3/src/__init__.py
--rw-r--r--   0 maxim      (502) staff       (20)     2607 2024-04-16 05:56:10.000000 picnic_bio-1.0.0b3/src/exceptions.py
-drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-04-16 07:06:22.163647 picnic_bio-1.0.0b3/src/features/
--rw-r--r--   0 maxim      (502) staff       (20)        0 2023-10-11 14:32:47.000000 picnic_bio-1.0.0b3/src/features/__init__.py
--rw-r--r--   0 maxim      (502) staff       (20)     1470 2024-01-24 08:48:42.000000 picnic_bio-1.0.0b3/src/features/calculation_disorder.py
--rw-r--r--   0 maxim      (502) staff       (20)     2339 2024-01-17 16:35:26.000000 picnic_bio-1.0.0b3/src/features/goterms.py
--rw-r--r--   0 maxim      (502) staff       (20)      918 2023-10-11 14:32:47.000000 picnic_bio-1.0.0b3/src/features/sequence_complexity.py
--rw-r--r--   0 maxim      (502) staff       (20)     2571 2023-10-11 14:32:47.000000 picnic_bio-1.0.0b3/src/features/sequence_distance.py
--rw-r--r--   0 maxim      (502) staff       (20)     8898 2024-04-16 06:01:58.000000 picnic_bio-1.0.0b3/src/features/sequence_structure_AF2.py
-drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-04-16 07:06:22.164604 picnic_bio-1.0.0b3/src/files/
--rw-r--r--   0 maxim      (502) staff       (20)      285 2024-01-17 16:35:26.000000 picnic_bio-1.0.0b3/src/files/__init__.py
-drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-04-16 07:06:22.186647 picnic_bio-1.0.0b3/src/files/go/
--rw-r--r--   0 maxim      (502) staff       (20)   628505 2023-08-14 14:33:27.000000 picnic_bio-1.0.0b3/src/files/go/bp_2500_freq.txt
--rw-r--r--   0 maxim      (502) staff       (20)  3146152 2023-08-14 14:33:27.000000 picnic_bio-1.0.0b3/src/files/go/bp_2500_freq_all.json
--rw-r--r--   0 maxim      (502) staff       (20)    91947 2023-08-14 14:33:27.000000 picnic_bio-1.0.0b3/src/files/go/cc_2000_freq.txt
--rw-r--r--   0 maxim      (502) staff       (20)   263088 2023-08-14 14:33:27.000000 picnic_bio-1.0.0b3/src/files/go/cc_2000_freq_all.json
--rw-r--r--   0 maxim      (502) staff       (20)   245749 2023-08-14 14:33:27.000000 picnic_bio-1.0.0b3/src/files/go/mf_2500_freq.txt
--rw-r--r--   0 maxim      (502) staff       (20)   869522 2023-08-14 14:33:28.000000 picnic_bio-1.0.0b3/src/files/go/mf_2500_freq_all.json
-drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-04-16 07:06:22.200686 picnic_bio-1.0.0b3/src/files/models_llps/
--rw-r--r--   0 maxim      (502) staff       (20)      157 2023-08-14 14:33:28.000000 picnic_bio-1.0.0b3/src/files/models_llps/keys_llps_withgonocc_retrained_newgo_18.txt
--rw-r--r--   0 maxim      (502) staff       (20)      674 2023-08-14 14:33:28.000000 picnic_bio-1.0.0b3/src/files/models_llps/keys_llps_withoutgocattrue_92.txt
--rw-r--r--   0 maxim      (502) staff       (20)   968164 2023-08-14 14:33:28.000000 picnic_bio-1.0.0b3/src/files/models_llps/modelpipe_depth6class1_id_2_llps_withgonocc_retrained_newgo18.sav
--rw-r--r--   0 maxim      (502) staff       (20)  2346792 2023-08-14 14:33:28.000000 picnic_bio-1.0.0b3/src/files/models_llps/modelpipe_depth7class1_id_92_llps_withoutgo_24-02.sav
--rw-r--r--   0 maxim      (502) staff       (20)     4517 2024-04-16 05:59:31.000000 picnic_bio-1.0.0b3/src/main.py
-drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-04-16 07:06:22.210725 picnic_bio-1.0.0b3/src/prediction/
--rw-r--r--   0 maxim      (502) staff       (20)        0 2023-10-11 14:32:47.000000 picnic_bio-1.0.0b3/src/prediction/__init__.py
--rw-r--r--   0 maxim      (502) staff       (20)     2508 2024-04-16 05:59:31.000000 picnic_bio-1.0.0b3/src/prediction/calculation_pipeline.py
--rw-r--r--   0 maxim      (502) staff       (20)     3294 2023-10-11 14:32:47.000000 picnic_bio-1.0.0b3/src/prediction/create_model.py
--rw-r--r--   0 maxim      (502) staff       (20)     8295 2024-04-16 05:59:31.000000 picnic_bio-1.0.0b3/src/prediction/inference_model.py
+drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-05-06 12:55:35.504559 picnic_bio-1.0.0rc1/
+-rw-r--r--   0 maxim      (502) staff       (20)     1514 2023-10-11 14:32:47.000000 picnic_bio-1.0.0rc1/LICENSE
+-rw-r--r--   0 maxim      (502) staff       (20)     9883 2024-05-06 12:55:35.504286 picnic_bio-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 maxim      (502) staff       (20)    11833 2024-05-06 12:51:45.000000 picnic_bio-1.0.0rc1/README.md
+drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-05-06 12:55:35.503491 picnic_bio-1.0.0rc1/picnic_bio.egg-info/
+-rw-r--r--   0 maxim      (502) staff       (20)     9883 2024-05-06 12:55:35.000000 picnic_bio-1.0.0rc1/picnic_bio.egg-info/PKG-INFO
+-rw-r--r--   0 maxim      (502) staff       (20)     1146 2024-05-06 12:55:35.000000 picnic_bio-1.0.0rc1/picnic_bio.egg-info/SOURCES.txt
+-rw-r--r--   0 maxim      (502) staff       (20)        1 2024-05-06 12:55:35.000000 picnic_bio-1.0.0rc1/picnic_bio.egg-info/dependency_links.txt
+-rw-r--r--   0 maxim      (502) staff       (20)       48 2024-05-06 12:55:35.000000 picnic_bio-1.0.0rc1/picnic_bio.egg-info/entry_points.txt
+-rw-r--r--   0 maxim      (502) staff       (20)       90 2024-05-06 12:55:35.000000 picnic_bio-1.0.0rc1/picnic_bio.egg-info/requires.txt
+-rw-r--r--   0 maxim      (502) staff       (20)       11 2024-05-06 12:55:35.000000 picnic_bio-1.0.0rc1/picnic_bio.egg-info/top_level.txt
+-rw-r--r--   0 maxim      (502) staff       (20)      182 2023-10-11 14:32:47.000000 picnic_bio-1.0.0rc1/pyproject.toml
+-rw-r--r--   0 maxim      (502) staff       (20)      503 2024-05-06 12:55:35.505349 picnic_bio-1.0.0rc1/setup.cfg
+-rw-r--r--   0 maxim      (502) staff       (20)     2251 2024-05-06 12:51:45.000000 picnic_bio-1.0.0rc1/setup.py
+drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-05-06 12:55:35.474575 picnic_bio-1.0.0rc1/src/
+-rw-r--r--   0 maxim      (502) staff       (20)        0 2023-10-11 14:32:47.000000 picnic_bio-1.0.0rc1/src/__init__.py
+-rw-r--r--   0 maxim      (502) staff       (20)     2607 2024-04-16 05:56:10.000000 picnic_bio-1.0.0rc1/src/exceptions.py
+drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-05-06 12:55:35.477108 picnic_bio-1.0.0rc1/src/features/
+-rw-r--r--   0 maxim      (502) staff       (20)        0 2023-10-11 14:32:47.000000 picnic_bio-1.0.0rc1/src/features/__init__.py
+-rw-r--r--   0 maxim      (502) staff       (20)     1470 2024-01-24 08:48:42.000000 picnic_bio-1.0.0rc1/src/features/calculation_disorder.py
+-rw-r--r--   0 maxim      (502) staff       (20)     2339 2024-01-17 16:35:26.000000 picnic_bio-1.0.0rc1/src/features/goterms.py
+-rw-r--r--   0 maxim      (502) staff       (20)      918 2023-10-11 14:32:47.000000 picnic_bio-1.0.0rc1/src/features/sequence_complexity.py
+-rw-r--r--   0 maxim      (502) staff       (20)     2571 2023-10-11 14:32:47.000000 picnic_bio-1.0.0rc1/src/features/sequence_distance.py
+-rw-r--r--   0 maxim      (502) staff       (20)     8845 2024-05-03 08:21:54.000000 picnic_bio-1.0.0rc1/src/features/sequence_structure_AF2.py
+drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-05-06 12:55:35.477511 picnic_bio-1.0.0rc1/src/files/
+-rw-r--r--   0 maxim      (502) staff       (20)      285 2024-01-17 16:35:26.000000 picnic_bio-1.0.0rc1/src/files/__init__.py
+drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-05-06 12:55:35.491279 picnic_bio-1.0.0rc1/src/files/go/
+-rw-r--r--   0 maxim      (502) staff       (20)   628505 2023-08-14 14:33:27.000000 picnic_bio-1.0.0rc1/src/files/go/bp_2500_freq.txt
+-rw-r--r--   0 maxim      (502) staff       (20)  3146152 2023-08-14 14:33:27.000000 picnic_bio-1.0.0rc1/src/files/go/bp_2500_freq_all.json
+-rw-r--r--   0 maxim      (502) staff       (20)    91947 2023-08-14 14:33:27.000000 picnic_bio-1.0.0rc1/src/files/go/cc_2000_freq.txt
+-rw-r--r--   0 maxim      (502) staff       (20)   263088 2023-08-14 14:33:27.000000 picnic_bio-1.0.0rc1/src/files/go/cc_2000_freq_all.json
+-rw-r--r--   0 maxim      (502) staff       (20)   245749 2023-08-14 14:33:27.000000 picnic_bio-1.0.0rc1/src/files/go/mf_2500_freq.txt
+-rw-r--r--   0 maxim      (502) staff       (20)   869522 2023-08-14 14:33:28.000000 picnic_bio-1.0.0rc1/src/files/go/mf_2500_freq_all.json
+drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-05-06 12:55:35.497191 picnic_bio-1.0.0rc1/src/files/models_llps/
+-rw-r--r--   0 maxim      (502) staff       (20)      157 2023-08-14 14:33:28.000000 picnic_bio-1.0.0rc1/src/files/models_llps/keys_llps_withgonocc_retrained_newgo_18.txt
+-rw-r--r--   0 maxim      (502) staff       (20)      674 2023-08-14 14:33:28.000000 picnic_bio-1.0.0rc1/src/files/models_llps/keys_llps_withoutgocattrue_92.txt
+-rw-r--r--   0 maxim      (502) staff       (20)   968164 2023-08-14 14:33:28.000000 picnic_bio-1.0.0rc1/src/files/models_llps/modelpipe_depth6class1_id_2_llps_withgonocc_retrained_newgo18.sav
+-rw-r--r--   0 maxim      (502) staff       (20)  2346792 2023-08-14 14:33:28.000000 picnic_bio-1.0.0rc1/src/files/models_llps/modelpipe_depth7class1_id_92_llps_withoutgo_24-02.sav
+-rw-r--r--   0 maxim      (502) staff       (20)     4517 2024-04-16 05:59:31.000000 picnic_bio-1.0.0rc1/src/main.py
+drwxr-xr-x   0 maxim      (502) staff       (20)        0 2024-05-06 12:55:35.502960 picnic_bio-1.0.0rc1/src/prediction/
+-rw-r--r--   0 maxim      (502) staff       (20)        0 2023-10-11 14:32:47.000000 picnic_bio-1.0.0rc1/src/prediction/__init__.py
+-rw-r--r--   0 maxim      (502) staff       (20)     2508 2024-04-16 05:59:31.000000 picnic_bio-1.0.0rc1/src/prediction/calculation_pipeline.py
+-rw-r--r--   0 maxim      (502) staff       (20)     3294 2023-10-11 14:32:47.000000 picnic_bio-1.0.0rc1/src/prediction/create_model.py
+-rw-r--r--   0 maxim      (502) staff       (20)     8295 2024-04-16 05:59:31.000000 picnic_bio-1.0.0rc1/src/prediction/inference_model.py
+-rw-r--r--   0 maxim      (502) staff       (20)     2936 2024-05-03 08:21:54.000000 picnic_bio-1.0.0rc1/src/stride.py
```

### Comparing `picnic_bio-1.0.0b3/LICENSE` & `picnic_bio-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/PKG-INFO` & `picnic_bio-1.0.0rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picnic-bio
-Version: 1.0.0b3
+Version: 1.0.0rc1
 Summary: PICNIC (Proteins Involved in CoNdensates In Cells) is a machine learning-based model that predicts proteins involved in biomolecular condensates.
 Home-page: https://picnic.cd-code.org/
 Author: Anna Hadarovich <hadarovi@mpi-cbg.de>, Maxim Scheremetjew <schereme@mpi-cbg.de>
 Author-email: picnic@cd-code.org
 Project-URL: Documentation, https://git.mpi-cbg.de/tothpetroczylab/picnic/-/blob/main/README.md
 Project-URL: Funding, https://picnic.cd-code.org/about-us
 Project-URL: Source, https://git.mpi-cbg.de/tothpetroczylab/picnic
@@ -16,26 +16,26 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests~=2.31.0
-Requires-Dist: catboost==1.2.2
+Requires-Dist: catboost~=1.2.3
 Requires-Dist: matplotlib~=3.7.2
-Requires-Dist: pandas~=2.1.0
+Requires-Dist: pandas~=2.2.1
 Requires-Dist: Bio~=1.5.2
-Requires-Dist: numpy~=1.23.5
-Requires-Dist: prody~=2.4.0
+Requires-Dist: numpy~=1.26.4
 
 <h1 align="center">
 <img src="https://git.mpi-cbg.de/tothpetroczylab/picnic/-/raw/main/branding/logo/logo_picnic_v1.96113169.png" width="300">
 </h1><br>
 
 # PICNIC
 
@@ -55,15 +55,15 @@
 
 # Installation instructions
 
 A binary installer for the latest released version is available at the Python Package Index (PyPI).
 
 ## Requirements
 
-* Python versions >=3.9,<3.12
+* Python versions >=3.9,<3.13
 * Download and unpack IUPred2A
   * Add IUPred2A to PYTHONPATH
 * Download and unpack STRIDE
   * Add STRIDE binary to your system PATH
 
 
 ## Install external requirements
@@ -92,51 +92,58 @@
 $ tar -zxf iupred2a.tar.gz
 $ cd iupred2a
 $ export PYTHONPATH="$PWD"
 ```
 
 ## PICNIC is available on PyPI
 
-PICNIC officially supports Python versions >=3.9,<3.12.
+PICNIC officially supports Python versions >=3.9,<3.13.
 
 ```shell
 $ python3 --version
 Python 3.11.5
-$ python3 -m pip install picnic_bio
+
+$ python3 -m venv picnic-env
+$ source picnic-env/bin/activate
+$ (picnic-env) % python -m pip install --upgrade pip
+$ (picnic-env) % python -m pip install picnic_bio
 ```
 
 ## PICNIC is also installable from source
 
 ```shell
 $ git clone git@git.mpi-cbg.de:atplab/picnic.git
 ```
 
 Once you have a copy of the source, you can embed it in your own Python package, or install it into your site-packages easily
 
 ```shell
 $ cd picnic
 $ python3 -m venv picnic-env
 $ source picnic-env/bin/activate
-(picnic-env) $ python -m pip install .
+$ (picnic-env) % python -m pip install --upgrade pip
+$ (picnic-env) $ python -m pip install .
 ```
 
 ## How to install PICNIC using Conda?
 
 There isn't any binary installer available on Conda yet. Though it is possible to install PICNIC within a virtual Conda environment.
 
 Please note that in a conda environment you have to pre-install catboost, before installing picnic-bio itself, otherwise the installation will fail when compiling the catboost package from source code. Also it is recommended to use and set up [conda-forge](https://conda-forge.org/docs/user/introduction.html) to fetch pre-compiled versions of catboost.
 
-Please also note that catboost=1.2.2 is incompatible with Python 3.12. The maintainers of catboost are working towards a fix right now.
-
 We have documented how to get around the catboost installation issue.
 
 ```shell
 $ conda config --add channels conda-forge
 $ conda config --set channel_priority strict
-$ conda create -n myenv python=[3.9, 3.10, 3.11] catboost=1.2.2
+
+# Choose one of the supported Python versions, when creating the Conda environment: >=3.9,<3.13
+# conda create -n myenv python=[3.9, 3.10, 3.11, 3.12] catboost
+# e.g.
+$ conda create -n myenv python=3.11 catboost
 $ conda activate myenv
 (myenv) $ python -m pip install picnic_bio
 ```
 
 # How to use?
 
 ## Usage - Using PICNIC from command line
```

### Comparing `picnic_bio-1.0.0b3/README.md` & `picnic_bio-1.0.0rc1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 # Installation instructions
 
 A binary installer for the latest released version is available at the Python Package Index (PyPI).
 
 ## Requirements
 
-* Python versions >=3.9,<3.12
+* Python versions >=3.9,<3.13
 * Download and unpack IUPred2A
   * Add IUPred2A to PYTHONPATH
 * Download and unpack STRIDE
   * Add STRIDE binary to your system PATH
 
 
 ## Install external requirements
@@ -57,51 +57,58 @@
 $ tar -zxf iupred2a.tar.gz
 $ cd iupred2a
 $ export PYTHONPATH="$PWD"
 ```
 
 ## PICNIC is available on PyPI
 
-PICNIC officially supports Python versions >=3.9,<3.12.
+PICNIC officially supports Python versions >=3.9,<3.13.
 
 ```shell
 $ python3 --version
 Python 3.11.5
-$ python3 -m pip install picnic_bio
+
+$ python3 -m venv picnic-env
+$ source picnic-env/bin/activate
+$ (picnic-env) % python -m pip install --upgrade pip
+$ (picnic-env) % python -m pip install picnic_bio
 ```
 
 ## PICNIC is also installable from source
 
 ```shell
 $ git clone git@git.mpi-cbg.de:atplab/picnic.git
 ```
 
 Once you have a copy of the source, you can embed it in your own Python package, or install it into your site-packages easily
 
 ```shell
 $ cd picnic
 $ python3 -m venv picnic-env
 $ source picnic-env/bin/activate
-(picnic-env) $ python -m pip install .
+$ (picnic-env) % python -m pip install --upgrade pip
+$ (picnic-env) $ python -m pip install .
 ```
 
 ## How to install PICNIC using Conda?
 
 There isn't any binary installer available on Conda yet. Though it is possible to install PICNIC within a virtual Conda environment.
 
 Please note that in a conda environment you have to pre-install catboost, before installing picnic-bio itself, otherwise the installation will fail when compiling the catboost package from source code. Also it is recommended to use and set up [conda-forge](https://conda-forge.org/docs/user/introduction.html) to fetch pre-compiled versions of catboost.
 
-Please also note that catboost=1.2.2 is incompatible with Python 3.12. The maintainers of catboost are working towards a fix right now.
-
 We have documented how to get around the catboost installation issue.
 
 ```shell
 $ conda config --add channels conda-forge
 $ conda config --set channel_priority strict
-$ conda create -n myenv python=[3.9, 3.10, 3.11] catboost=1.2.2
+
+# Choose one of the supported Python versions, when creating the Conda environment: >=3.9,<3.13
+# conda create -n myenv python=[3.9, 3.10, 3.11, 3.12] catboost
+# e.g.
+$ conda create -n myenv python=3.11 catboost
 $ conda activate myenv
 (myenv) $ python -m pip install picnic_bio
 ```
 
 # How to use?
 
 ## Usage - Using PICNIC from command line
@@ -323,14 +330,18 @@
 
 ### How to upload distribution files to PyPi?
 
 Finally, we need to upload these files to PyPi using Twine. Use the following command from the project root
 directory. Enter the PyPi credentials to complete uploading the package.
 
 ```shell
+# Perform a test upload on testPyPI
+(packaging) $ twine upload --repository testpypi dist/*
+
+# Finally upload the distribution to PyPI
 (packaging) $ twine upload dist/*
 ```
 
 
 ### How to deactivate the virtual environment?
 
 ```shell
```

### Comparing `picnic_bio-1.0.0b3/picnic_bio.egg-info/PKG-INFO` & `picnic_bio-1.0.0rc1/picnic_bio.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picnic-bio
-Version: 1.0.0b3
+Version: 1.0.0rc1
 Summary: PICNIC (Proteins Involved in CoNdensates In Cells) is a machine learning-based model that predicts proteins involved in biomolecular condensates.
 Home-page: https://picnic.cd-code.org/
 Author: Anna Hadarovich <hadarovi@mpi-cbg.de>, Maxim Scheremetjew <schereme@mpi-cbg.de>
 Author-email: picnic@cd-code.org
 Project-URL: Documentation, https://git.mpi-cbg.de/tothpetroczylab/picnic/-/blob/main/README.md
 Project-URL: Funding, https://picnic.cd-code.org/about-us
 Project-URL: Source, https://git.mpi-cbg.de/tothpetroczylab/picnic
@@ -16,26 +16,26 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests~=2.31.0
-Requires-Dist: catboost==1.2.2
+Requires-Dist: catboost~=1.2.3
 Requires-Dist: matplotlib~=3.7.2
-Requires-Dist: pandas~=2.1.0
+Requires-Dist: pandas~=2.2.1
 Requires-Dist: Bio~=1.5.2
-Requires-Dist: numpy~=1.23.5
-Requires-Dist: prody~=2.4.0
+Requires-Dist: numpy~=1.26.4
 
 <h1 align="center">
 <img src="https://git.mpi-cbg.de/tothpetroczylab/picnic/-/raw/main/branding/logo/logo_picnic_v1.96113169.png" width="300">
 </h1><br>
 
 # PICNIC
 
@@ -55,15 +55,15 @@
 
 # Installation instructions
 
 A binary installer for the latest released version is available at the Python Package Index (PyPI).
 
 ## Requirements
 
-* Python versions >=3.9,<3.12
+* Python versions >=3.9,<3.13
 * Download and unpack IUPred2A
   * Add IUPred2A to PYTHONPATH
 * Download and unpack STRIDE
   * Add STRIDE binary to your system PATH
 
 
 ## Install external requirements
@@ -92,51 +92,58 @@
 $ tar -zxf iupred2a.tar.gz
 $ cd iupred2a
 $ export PYTHONPATH="$PWD"
 ```
 
 ## PICNIC is available on PyPI
 
-PICNIC officially supports Python versions >=3.9,<3.12.
+PICNIC officially supports Python versions >=3.9,<3.13.
 
 ```shell
 $ python3 --version
 Python 3.11.5
-$ python3 -m pip install picnic_bio
+
+$ python3 -m venv picnic-env
+$ source picnic-env/bin/activate
+$ (picnic-env) % python -m pip install --upgrade pip
+$ (picnic-env) % python -m pip install picnic_bio
 ```
 
 ## PICNIC is also installable from source
 
 ```shell
 $ git clone git@git.mpi-cbg.de:atplab/picnic.git
 ```
 
 Once you have a copy of the source, you can embed it in your own Python package, or install it into your site-packages easily
 
 ```shell
 $ cd picnic
 $ python3 -m venv picnic-env
 $ source picnic-env/bin/activate
-(picnic-env) $ python -m pip install .
+$ (picnic-env) % python -m pip install --upgrade pip
+$ (picnic-env) $ python -m pip install .
 ```
 
 ## How to install PICNIC using Conda?
 
 There isn't any binary installer available on Conda yet. Though it is possible to install PICNIC within a virtual Conda environment.
 
 Please note that in a conda environment you have to pre-install catboost, before installing picnic-bio itself, otherwise the installation will fail when compiling the catboost package from source code. Also it is recommended to use and set up [conda-forge](https://conda-forge.org/docs/user/introduction.html) to fetch pre-compiled versions of catboost.
 
-Please also note that catboost=1.2.2 is incompatible with Python 3.12. The maintainers of catboost are working towards a fix right now.
-
 We have documented how to get around the catboost installation issue.
 
 ```shell
 $ conda config --add channels conda-forge
 $ conda config --set channel_priority strict
-$ conda create -n myenv python=[3.9, 3.10, 3.11] catboost=1.2.2
+
+# Choose one of the supported Python versions, when creating the Conda environment: >=3.9,<3.13
+# conda create -n myenv python=[3.9, 3.10, 3.11, 3.12] catboost
+# e.g.
+$ conda create -n myenv python=3.11 catboost
 $ conda activate myenv
 (myenv) $ python -m pip install picnic_bio
 ```
 
 # How to use?
 
 ## Usage - Using PICNIC from command line
```

### Comparing `picnic_bio-1.0.0b3/picnic_bio.egg-info/SOURCES.txt` & `picnic_bio-1.0.0rc1/picnic_bio.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 picnic_bio.egg-info/dependency_links.txt
 picnic_bio.egg-info/entry_points.txt
 picnic_bio.egg-info/requires.txt
 picnic_bio.egg-info/top_level.txt
 src/__init__.py
 src/exceptions.py
 src/main.py
+src/stride.py
 src/features/__init__.py
 src/features/calculation_disorder.py
 src/features/goterms.py
 src/features/sequence_complexity.py
 src/features/sequence_distance.py
 src/features/sequence_structure_AF2.py
 src/files/__init__.py
```

### Comparing `picnic_bio-1.0.0b3/setup.py` & `picnic_bio-1.0.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     for line in fh:
         if line.startswith("# Development"):
             break
         long_description += line
 
 setuptools.setup(
     name="picnic-bio",
-    version="1.0.0-beta3",
+    version="1.0.0-rc1",
     author="Anna Hadarovich <hadarovi@mpi-cbg.de>, Maxim Scheremetjew <schereme@mpi-cbg.de>",
     author_email="picnic@cd-code.org",
     description="PICNIC (Proteins Involved in CoNdensates In Cells) is a machine learning-based model that predicts proteins involved in biomolecular condensates.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://picnic.cd-code.org/",
     project_urls={
@@ -30,28 +30,28 @@
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Operating System :: Unix",
         "Operating System :: MacOS",
     ],
     package_dir={"picnic_bio": "src"},
     package_data={"picnic_bio": ["files/models_llps/*", "files/iupred2a/data/*", "files/go/*"]},
     python_requires=">=3.9",
     install_requires=[
         "requests ~=2.31.0",
-        "catboost ==1.2.2",
+        "catboost ~=1.2.3",
         "matplotlib ~=3.7.2",
-        "pandas ~=2.1.0",
+        "pandas ~=2.2.1",
         "Bio ~=1.5.2",
-        "numpy ~=1.23.5",
-        "prody ~=2.4.0",
+        "numpy ~=1.26.4",
     ],
     entry_points={
         "console_scripts": [
             "picnic = picnic_bio.main:main",
         ]
     },
 )
```

### Comparing `picnic_bio-1.0.0b3/src/exceptions.py` & `picnic_bio-1.0.0rc1/src/exceptions.py`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/src/features/calculation_disorder.py` & `picnic_bio-1.0.0rc1/src/features/calculation_disorder.py`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/src/features/goterms.py` & `picnic_bio-1.0.0rc1/src/features/goterms.py`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/src/features/sequence_complexity.py` & `picnic_bio-1.0.0rc1/src/features/sequence_complexity.py`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/src/features/sequence_distance.py` & `picnic_bio-1.0.0rc1/src/features/sequence_distance.py`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/src/features/sequence_structure_AF2.py` & `picnic_bio-1.0.0rc1/src/features/sequence_structure_AF2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import collections
 import os
 
-import prody as pr
 import requests
 
 from ..exceptions import (
     CouldNotDownloadAlphaFoldModelError,
     CouldNotDownloadFASTAFileError,
     NoAlphaFoldModelProvidedError,
 )
+from ..stride import exec_stride
 
 
 def get_dict():
     aadict = {
         "A": 1,
         "G": 1,
         "V": 1,
@@ -50,15 +50,15 @@
 def produce_stride_output_af(af_models_path, name, stride_out_path):
 
     forstride = os.listdir(af_models_path)
     result = [i for i in forstride if (i.startswith("AF-" + name + "-") and i.endswith(".pdb"))]
     if len(result) == 0:
         raise NoAlphaFoldModelProvidedError(af_models_path)
     for f in result:
-        pr.execSTRIDE(af_models_path + f, outputname=f, outputdir=stride_out_path)
+        exec_stride(af_models_path + f, output_name=f, output_dir=stride_out_path)
     return
 
 
 def get_ordered_dict(result):
     d = dict()
     for r in result:
         nummstr = r[:-13]
@@ -280,11 +280,7 @@
     try:
         url = f"https://rest.uniprot.org/uniprotkb/{uniprot_id}.fasta"
         file_path = f"{path_file}{uniprot_id}.fasta"
         send_request_and_write_content_to_file(url, file_path)
     except requests.exceptions.RequestException as err:
         raise CouldNotDownloadFASTAFileError(uniprot_id, err)
     return file_path
-
-
-if __name__ == "__main__":
-    print("Feature AF")  # noqa: T201
```

### Comparing `picnic_bio-1.0.0b3/src/files/go/bp_2500_freq.txt` & `picnic_bio-1.0.0rc1/src/files/go/bp_2500_freq.txt`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/src/files/go/bp_2500_freq_all.json` & `picnic_bio-1.0.0rc1/src/files/go/bp_2500_freq_all.json`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/src/files/go/cc_2000_freq.txt` & `picnic_bio-1.0.0rc1/src/files/go/cc_2000_freq.txt`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/src/files/go/cc_2000_freq_all.json` & `picnic_bio-1.0.0rc1/src/files/go/cc_2000_freq_all.json`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/src/files/go/mf_2500_freq.txt` & `picnic_bio-1.0.0rc1/src/files/go/mf_2500_freq.txt`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/src/files/go/mf_2500_freq_all.json` & `picnic_bio-1.0.0rc1/src/files/go/mf_2500_freq_all.json`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/src/files/models_llps/keys_llps_withoutgocattrue_92.txt` & `picnic_bio-1.0.0rc1/src/files/models_llps/keys_llps_withoutgocattrue_92.txt`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/src/files/models_llps/modelpipe_depth6class1_id_2_llps_withgonocc_retrained_newgo18.sav` & `picnic_bio-1.0.0rc1/src/files/models_llps/modelpipe_depth6class1_id_2_llps_withgonocc_retrained_newgo18.sav`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/src/files/models_llps/modelpipe_depth7class1_id_92_llps_withoutgo_24-02.sav` & `picnic_bio-1.0.0rc1/src/files/models_llps/modelpipe_depth7class1_id_92_llps_withoutgo_24-02.sav`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/src/main.py` & `picnic_bio-1.0.0rc1/src/main.py`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/src/prediction/calculation_pipeline.py` & `picnic_bio-1.0.0rc1/src/prediction/calculation_pipeline.py`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/src/prediction/create_model.py` & `picnic_bio-1.0.0rc1/src/prediction/create_model.py`

 * *Files identical despite different names*

### Comparing `picnic_bio-1.0.0b3/src/prediction/inference_model.py` & `picnic_bio-1.0.0rc1/src/prediction/inference_model.py`

 * *Files identical despite different names*

