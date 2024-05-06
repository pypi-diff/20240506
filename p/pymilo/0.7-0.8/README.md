# Comparing `tmp/pymilo-0.7.tar.gz` & `tmp/pymilo-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymilo-0.7.tar", last modified: Wed Apr  3 04:56:46 2024, max compression
+gzip compressed data, was "pymilo-0.8.tar", last modified: Mon May  6 10:53:13 2024, max compression
```

## Comparing `pymilo-0.7.tar` & `pymilo-0.8.tar`

### file list

```diff
@@ -1,52 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:56:46.668030 pymilo-0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-03 04:56:38.000000 pymilo-0.7/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 04:56:38.000000 pymilo-0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14743 2024-04-03 04:56:46.668030 pymilo-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-04-03 04:56:38.000000 pymilo-0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:56:46.660030 pymilo-0.7/pymilo/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:56:46.664030 pymilo-0.7/pymilo/chains/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/chains/clustering_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/chains/decision_tree_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/chains/linear_model_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/chains/naive_bayes_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/chains/neighbours_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/chains/neural_network_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/chains/svm_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:56:46.664030 pymilo-0.7/pymilo/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/exceptions/deserialize_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/exceptions/pymilo_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/exceptions/serialize_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/pymilo_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/pymilo_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/pymilo_param.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:56:46.664030 pymilo-0.7/pymilo/transporters/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/adamoptimizer_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12751 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/baseloss_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/bisecting_tree_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/cfnode_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/function_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16633 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/general_data_structure_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/labelbinarizer_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/lossfunction_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/neighbors_tree_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/randomstate_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/sgdoptimizer_transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/transporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/transporters/tree_transporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:56:46.668030 pymilo-0.7/pymilo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/utils/data_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/utils/test_pymilo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-03 04:56:38.000000 pymilo-0.7/pymilo/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:56:46.668030 pymilo-0.7/pymilo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14743 2024-04-03 04:56:46.000000 pymilo-0.7/pymilo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-03 04:56:46.000000 pymilo-0.7/pymilo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 04:56:46.000000 pymilo-0.7/pymilo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 04:56:46.000000 pymilo-0.7/pymilo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 04:56:46.000000 pymilo-0.7/pymilo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 04:56:46.668030 pymilo-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-03 04:56:38.000000 pymilo-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:53:13.401304 pymilo-0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-06 10:53:05.000000 pymilo-0.8/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-06 10:53:05.000000 pymilo-0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15933 2024-05-06 10:53:13.401304 pymilo-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-06 10:53:05.000000 pymilo-0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:53:13.393304 pymilo-0.8/pymilo/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:53:13.397304 pymilo-0.8/pymilo/chains/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/chains/clustering_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/chains/decision_tree_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15573 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/chains/ensemble_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/chains/linear_model_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/chains/naive_bayes_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/chains/neighbours_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/chains/neural_network_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/chains/svm_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/chains/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:53:13.397304 pymilo-0.8/pymilo/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/exceptions/deserialize_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/exceptions/pymilo_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/exceptions/serialize_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/pymilo_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/pymilo_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9179 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/pymilo_param.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:53:13.401304 pymilo-0.8/pymilo/transporters/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/adamoptimizer_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12751 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/baseloss_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/binmapper_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/bisecting_tree_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/bunch_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/cfnode_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/function_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17936 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/general_data_structure_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/generator_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/lossfunction_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/neighbors_tree_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/preprocessing_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/randomstate_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/sgdoptimizer_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/tree_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/transporters/treepredictor_transporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:53:13.401304 pymilo-0.8/pymilo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/utils/data_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/utils/test_pymilo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-06 10:53:05.000000 pymilo-0.8/pymilo/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:53:13.401304 pymilo-0.8/pymilo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15933 2024-05-06 10:53:13.000000 pymilo-0.8/pymilo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-06 10:53:13.000000 pymilo-0.8/pymilo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:53:13.000000 pymilo-0.8/pymilo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-06 10:53:13.000000 pymilo-0.8/pymilo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 10:53:13.000000 pymilo-0.8/pymilo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 10:53:13.401304 pymilo-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-06 10:53:05.000000 pymilo-0.8/setup.py
```

### Comparing `pymilo-0.7/AUTHORS.md` & `pymilo-0.8/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pymilo-0.7/LICENSE` & `pymilo-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pymilo-0.7/PKG-INFO` & `pymilo-0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymilo
-Version: 0.7
+Version: 0.8
 Summary: Transportation of ML models
 Home-page: https://github.com/openscilab/pymilo
-Download-URL: https://github.com/openscilab/pymilo/tarball/v0.7
+Download-URL: https://github.com/openscilab/pymilo/tarball/v0.8
 Author: PyMilo Development Team
 Author-email: pymilo@openscilab.com
 License: MIT
 Project-URL: Source, https://github.com/openscilab/pymilo
 Keywords: python3 python machine_learning ML
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -41,44 +41,22 @@
 Requires-Dist: scikit-learn>=0.22.2
 
 
 <div align="center">
     <img src="https://github.com/openscilab/pymilo/raw/main/otherfiles/logo.png" width="500" height="300">
     <br/>
     <br/>
-    <a href="https://codecov.io/gh/openscilab/pymilo">
-        <img src="https://codecov.io/gh/openscilab/pymilo/branch/main/graph/badge.svg" alt="Codecov"/>
-    </a>
-    <a href="https://badge.fury.io/py/pymilo">
-        <img src="https://badge.fury.io/py/pymilo.svg" alt="PyPI version" height="18">
-    </a>
-    <a href="https://www.python.org/">
-        <img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3">
-    </a>
-    <a href="https://discord.gg/mtuMS8AjDS">
-        <img src="https://img.shields.io/discord/1064533716615049236.svg" alt="Discord Channel">
-    </a>
+    <a href="https://codecov.io/gh/openscilab/pymilo"><img src="https://codecov.io/gh/openscilab/pymilo/branch/main/graph/badge.svg" alt="Codecov"/></a>
+    <a href="https://badge.fury.io/py/pymilo"><img src="https://badge.fury.io/py/pymilo.svg" alt="PyPI version" height="18"></a>
+    <a href="https://www.python.org/"><img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3"></a>
+    <a href="https://discord.gg/mtuMS8AjDS"><img src="https://img.shields.io/discord/1064533716615049236.svg" alt="Discord Channel"></a>
 </div>
 
 ----------
 
-## Table of contents
-
-* [Overview](https://github.com/openscilab/pymilo#overview)
-* [Installation](https://github.com/openscilab/pymilo#installation)
-* [Usage](https://github.com/openscilab/pymilo#usage)
-* [Issues & Bug Reports](https://github.com/openscilab/pymilo#issues--bug-reports)
-* [Contribution](https://github.com/openscilab/pymilo/blob/main/.github/CONTRIBUTING.md)
-* [Authors](https://github.com/openscilab/pymilo/blob/main/AUTHORS.md)
-* [License](https://github.com/openscilab/pymilo/blob/main/LICENSE)
-* [Show Your Support](https://github.com/openscilab/pymilo#show-your-support)
-* [Changelog](https://github.com/openscilab/pymilo/blob/main/CHANGELOG.md)
-* [Code of Conduct](https://github.com/openscilab/pymilo/blob/main/.github/CODE_OF_CONDUCT.md)
-
-
 ## Overview
 <p align="justify">
 PyMilo is an open source Python package that provides a simple, efficient, and safe way for users to export pre-trained machine learning models in a transparent way. By this, the exported model can be used in other environments, transferred across different platforms, and shared with others. PyMilo allows the users to export the models that are trained using popular Python libraries like scikit-learn, and then use them in deployment environments, or share them without exposing the underlying code or dependencies. The transparency of the exported models ensures reliability and safety for the end users, as it eliminates the risks of binary or pickle formats.
 </p>
 <table>
     <tr>
         <td align="center">PyPI Counter</td>
@@ -125,17 +103,17 @@
 
 
 ## Installation
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)
-- Run `pip install pymilo==0.7`
+- Run `pip install pymilo==0.8`
 ### Source code
-- Download [Version 0.7](https://github.com/openscilab/pymilo/archive/v0.7.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
+- Download [Version 0.8](https://github.com/openscilab/pymilo/archive/v0.8.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
 - Run `pip install .`
 
 ## Usage
 ### Model preparation 
 ```pycon
 >>> from sklearn import datasets
 >>> from pymilo import Export, Import
@@ -161,27 +139,30 @@
 >>> #### Import the pymilo-exported model and get a real scikit model
 >>> imported_model = Import(PATH_TO_JSON_FILE)
 ```
 ### Get the associated model
 ```pycon 
 >>> imported_sklearn_model = imported_model.to_model()
 ```
-#### Note: `imported_sklearn_model` has the **exact same** functionality as the `model` object earlier.
+* Note: `imported_sklearn_model` has the **exact same** functionality as the `model` object earlier.
 
 ## Supported ML models
 | scikit-learn | PyTorch | 
 | ---------------- | ---------------- | 
 | Linear Models &#x2705; | - | 
 | Neural networks &#x2705; | -  | 
 | Trees &#x2705; | -  | 
 | Clustering &#x2705; | -  | 
 | Naïve Bayes &#x2705; | -  | 
 | Support vector machines (SVMs) &#x2705; | -  | 
-| Nearest Neighbors &#x2705; | -  | 
-| Ensemble Models &#x274C; | - | 
+| Nearest Neighbors &#x2705; | -  |  
+| Ensemble Models &#x2705; | - | 
+| Pipeline Model &#x2705; | - |
+| Preprocessing Models ⏳ | - |
+
 Details are available in [Supported Models](https://github.com/openscilab/pymilo/blob/main/SUPPORTED_MODELS.md).
 
 ## Issues & bug reports
 
 Just fill an issue and describe it. We'll check it ASAP! or send an email to [pymilo@openscilab.com](mailto:pymilo@openscilab.com "pymilo@openscilab.com"). 
 
 - Please complete the issue template
@@ -209,14 +190,70 @@
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 ### Added
 ### Changed
+## [0.8] - 2024-05-06
+### Added
+- `StandardScaler` Transformer in `pymilo_param.py`
+- `PreprocessingTransporter` Transporter
+- ndarray shape config in `GeneralDataStructure` Transporter
+- `util.py` in chains
+- `BinMapperTransporter` Transporter
+- `BunchTransporter` Transporter
+- `GeneratorTransporter` Transporter
+- `TreePredictorTransporter` Transporter
+- `AdaboostClassifier` model
+- `AdaboostRegressor` model
+- `BaggingClassifier` model
+- `BaggingRegressor` model
+- `ExtraTreesClassifier` model
+- `ExtraTreesRegressor` model
+- `GradientBoosterClassifier` model
+- `GradientBoosterRegressor` model
+- `HistGradientBoosterClassifier` model
+- `HistGradientBoosterRegressor` model
+- `RandomForestClassifier` model
+- `RandomForestRegressor` model
+- `IsolationForest` model
+- `RandomTreesEmbedding` model
+- `StackingClassifier` model
+- `StackingRegressor` model
+- `VotingClassifier` model
+- `VotingRegressor` model
+- `Pipeline` model
+- Ensemble models test runner
+- Ensemble chain
+- `SECURITY.md`
+### Changed
+- `Pipeline` test updated
+- `LabelBinarizer`,`LabelEncoder` and `OneHotEncoder` got embedded in `PreprocessingTransporter`
+- Preprocessing support added to Ensemble chain
+- Preprocessing params initialized in `pymilo_param`
+- `util.py` in utils updated
+- `test_pymilo.py` updated
+- `pymilo_func.py` updated
+- `linear_model_chain.py` updated
+- `neural_network_chain.py` updated
+- `decision_tree_chain.py` updated
+- `clustering_chain.py` updated
+- `naive_bayes_chain.py` updated
+- `neighbours_chain.py` updated
+- `svm_chain.py` updated
+- `GeneralDataStructure` Transporter updated
+- `LossFunction` Transporter updated
+- `AbstractTransporter` updated
+- Tests config modified
+- Unequal sklearn version error added in `pymilo_param.py`
+- Ensemble params initialized in `pymilo_param`
+- Ensemble support added to `pymilo_func.py`
+- `SUPPORTED_MODELS.md` updated
+- `README.md` updated
 ## [0.7] - 2024-04-03
 ### Added
 - `pymilo_nearest_neighbor_test` function added to `test_pymilo.py`
 - `NeighborsTreeTransporter` Transporter
 - `LocalOutlierFactor` model
 - `RadiusNeighborsClassifier` model
 - `RadiusNeighborsRegressor` model
@@ -364,15 +401,16 @@
 - `linear_model_chain` refactored
 ## [0.1] - 2023-06-29
 ### Added
 - scikit-learn linear models support
 - `Export` class
 - `Import` class
 
-[Unreleased]: https://github.com/openscilab/pymilo/compare/v0.7...dev
+[Unreleased]: https://github.com/openscilab/pymilo/compare/v0.8...dev
+[0.8]: https://github.com/openscilab/pymilo/compare/v0.7...v0.8
 [0.7]: https://github.com/openscilab/pymilo/compare/v0.6...v0.7
 [0.6]: https://github.com/openscilab/pymilo/compare/v0.5...v0.6
 [0.5]: https://github.com/openscilab/pymilo/compare/v0.4...v0.5
 [0.4]: https://github.com/openscilab/pymilo/compare/v0.3...v0.4
 [0.3]: https://github.com/openscilab/pymilo/compare/v0.2...v0.3
 [0.2]: https://github.com/openscilab/pymilo/compare/v0.1...v0.2
 [0.1]: https://github.com/openscilab/pymilo/compare/e887108...v0.1
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pymilo Version: 0.7 Summary: Transportation of ML
+Metadata-Version: 2.1 Name: pymilo Version: 0.8 Summary: Transportation of ML
 models Home-page: https://github.com/openscilab/pymilo Download-URL: https://
-github.com/openscilab/pymilo/tarball/v0.7 Author: PyMilo Development Team
+github.com/openscilab/pymilo/tarball/v0.8 Author: PyMilo Development Team
 Author-email: pymilo@openscilab.com License: MIT Project-URL: Source, https://
 github.com/openscilab/pymilo Keywords: python3 python machine_learning ML
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
@@ -21,25 +21,15 @@
 Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
 Engineering :: Physics Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE License-File: AUTHORS.md Requires-Dist:
 numpy>=1.9.0 Requires-Dist: scikit-learn>=0.22.2
       [https://github.com/openscilab/pymilo/raw/main/otherfiles/logo.png]
 
          _[_C_o_d_e_c_o_v_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_b_u_i_l_t_ _w_i_t_h_ _P_y_t_h_o_n_3_]_[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]
----------- ## Table of contents * [Overview](https://github.com/openscilab/
-pymilo#overview) * [Installation](https://github.com/openscilab/
-pymilo#installation) * [Usage](https://github.com/openscilab/pymilo#usage) *
-[Issues & Bug Reports](https://github.com/openscilab/pymilo#issues--bug-
-reports) * [Contribution](https://github.com/openscilab/pymilo/blob/
-main/.github/CONTRIBUTING.md) * [Authors](https://github.com/openscilab/pymilo/
-blob/main/AUTHORS.md) * [License](https://github.com/openscilab/pymilo/blob/
-main/LICENSE) * [Show Your Support](https://github.com/openscilab/pymilo#show-
-your-support) * [Changelog](https://github.com/openscilab/pymilo/blob/main/
-CHANGELOG.md) * [Code of Conduct](https://github.com/openscilab/pymilo/blob/
-main/.github/CODE_OF_CONDUCT.md) ## Overview
+---------- ## Overview
 PyMilo is an open source Python package that provides a simple, efficient, and
 safe way for users to export pre-trained machine learning models in a
 transparent way. By this, the exported model can be used in other environments,
 transferred across different platforms, and shared with others. PyMilo allows
 the users to export the models that are trained using popular Python libraries
 like scikit-learn, and then use them in deployment environments, or share them
 without exposing the underlying code or dependencies. The transparency of the
@@ -52,50 +42,76 @@
         [https://github.com/openscilab/    [https://github.com/openscilab/
    CI  pymilo/actions/workflows/test.yml/ pymilo/actions/workflows/test.yml/
              badge.svg?branch=main]             badge.svg?branch=dev]
                           _[_h_t_t_p_s_:_/_/_a_p_p_._c_o_d_a_c_y_._c_o_m_/_p_r_o_j_e_c_t_/
 Code Quality _[_C_o_d_e_F_a_c_t_o_r_]           _b_a_d_g_e_/_G_r_a_d_e_/            _[_c_o_d_e_b_e_a_t_ _b_a_d_g_e_]
                           _9_e_e_e_c_9_9_e_d_1_1_f_4_d_9_b_8_6_a_f_3_6_d_c_9_0_f_5_f_7_5_3_]
 ## Installation ### PyPI - Check [Python Packaging User Guide](https://
-packaging.python.org/installing/) - Run `pip install pymilo==0.7` ### Source
-code - Download [Version 0.7](https://github.com/openscilab/pymilo/archive/
-v0.7.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
+packaging.python.org/installing/) - Run `pip install pymilo==0.8` ### Source
+code - Download [Version 0.8](https://github.com/openscilab/pymilo/archive/
+v0.8.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
 dev.zip) - Run `pip install .` ## Usage ### Model preparation ```pycon >>> from
 sklearn import datasets >>> from pymilo import Export, Import >>> from
 sklearn.linear_model import LinearRegression >>> import os >>> X, Y =
 datasets.load_diabetes(return_X_y=True) >>> threshold = 20 >>> X_train, X_test
 = X[:-threshold], X[-threshold:] >>> Y_train, Y_test = Y[:-threshold], Y[-
 threshold:] >>> model = LinearRegression() >>> #### Train the model using the
 training sets >>> model.fit(X_train, Y_train) ``` ### Save model ```pycon >>>
 #### Export the fitted model to a transparent json file >>> exported_model =
 Export(model) >>> PATH_TO_JSON_FILE = os.path.join(os.getcwd(),"test.json") >>>
 exported_model.save(PATH_TO_JSON_FILE) ``` ### Load model ```pycon >>> ####
 Import the pymilo-exported model and get a real scikit model >>> imported_model
 = Import(PATH_TO_JSON_FILE) ``` ### Get the associated model ```pycon >>>
-imported_sklearn_model = imported_model.to_model() ``` #### Note:
+imported_sklearn_model = imported_model.to_model() ``` * Note:
 `imported_sklearn_model` has the **exact same** functionality as the `model`
 object earlier. ## Supported ML models | scikit-learn | PyTorch | | -----------
 ----- | ---------------- | | Linear Models ✅ | - | | Neural networks ✅ | - | |
 Trees ✅ | - | | Clustering ✅ | - | | NaÃ¯ve Bayes ✅ | - | | Support vector
-machines (SVMs) ✅ | - | | Nearest Neighbors ✅ | - | | Ensemble Models ❌ | - |
-Details are available in [Supported Models](https://github.com/openscilab/
-pymilo/blob/main/SUPPORTED_MODELS.md). ## Issues & bug reports Just fill an
-issue and describe it. We'll check it ASAP! or send an email to
-[pymilo@openscilab.com](mailto:pymilo@openscilab.com "pymilo@openscilab.com").
-- Please complete the issue template You can also join our discord server
-_[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]## Show your support ### Star this repo Give a â­ï¸ if this
-project helped you! ### Donate to our project If you do like our project and we
-hope that you do, can you please support us? Our project is not and is never
-going to be working for profit. We need the money just so we can continue doing
-what we do ;-) . _[_P_y_M_i_l_o_ _D_o_n_a_t_i_o_n_]# Changelog All notable changes to this
-project will be documented in this file. The format is based on [Keep a
-Changelog](http://keepachangelog.com/en/1.0.0/) and this project adheres to
-[Semantic Versioning](http://semver.org/spec/v2.0.0.html). ## [Unreleased] ###
-Added ### Changed ## [0.7] - 2024-04-03 ### Added -
-`pymilo_nearest_neighbor_test` function added to `test_pymilo.py` -
+machines (SVMs) ✅ | - | | Nearest Neighbors ✅ | - | | Ensemble Models ✅ | - | |
+Pipeline Model ✅ | - | | Preprocessing Models â³ | - | Details are available
+in [Supported Models](https://github.com/openscilab/pymilo/blob/main/
+SUPPORTED_MODELS.md). ## Issues & bug reports Just fill an issue and describe
+it. We'll check it ASAP! or send an email to [pymilo@openscilab.com](mailto:
+pymilo@openscilab.com "pymilo@openscilab.com"). - Please complete the issue
+template You can also join our discord server _[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]## Show your
+support ### Star this repo Give a â­ï¸ if this project helped you! ### Donate
+to our project If you do like our project and we hope that you do, can you
+please support us? Our project is not and is never going to be working for
+profit. We need the money just so we can continue doing what we do ;-) .
+_[_P_y_M_i_l_o_ _D_o_n_a_t_i_o_n_]# Changelog All notable changes to this project will be
+documented in this file. The format is based on [Keep a Changelog](http://
+keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning]
+(http://semver.org/spec/v2.0.0.html). ## [Unreleased] ### Added ### Changed ##
+[0.8] - 2024-05-06 ### Added - `StandardScaler` Transformer in
+`pymilo_param.py` - `PreprocessingTransporter` Transporter - ndarray shape
+config in `GeneralDataStructure` Transporter - `util.py` in chains -
+`BinMapperTransporter` Transporter - `BunchTransporter` Transporter -
+`GeneratorTransporter` Transporter - `TreePredictorTransporter` Transporter -
+`AdaboostClassifier` model - `AdaboostRegressor` model - `BaggingClassifier`
+model - `BaggingRegressor` model - `ExtraTreesClassifier` model -
+`ExtraTreesRegressor` model - `GradientBoosterClassifier` model -
+`GradientBoosterRegressor` model - `HistGradientBoosterClassifier` model -
+`HistGradientBoosterRegressor` model - `RandomForestClassifier` model -
+`RandomForestRegressor` model - `IsolationForest` model -
+`RandomTreesEmbedding` model - `StackingClassifier` model - `StackingRegressor`
+model - `VotingClassifier` model - `VotingRegressor` model - `Pipeline` model -
+Ensemble models test runner - Ensemble chain - `SECURITY.md` ### Changed -
+`Pipeline` test updated - `LabelBinarizer`,`LabelEncoder` and `OneHotEncoder`
+got embedded in `PreprocessingTransporter` - Preprocessing support added to
+Ensemble chain - Preprocessing params initialized in `pymilo_param` - `util.py`
+in utils updated - `test_pymilo.py` updated - `pymilo_func.py` updated -
+`linear_model_chain.py` updated - `neural_network_chain.py` updated -
+`decision_tree_chain.py` updated - `clustering_chain.py` updated -
+`naive_bayes_chain.py` updated - `neighbours_chain.py` updated - `svm_chain.py`
+updated - `GeneralDataStructure` Transporter updated - `LossFunction`
+Transporter updated - `AbstractTransporter` updated - Tests config modified -
+Unequal sklearn version error added in `pymilo_param.py` - Ensemble params
+initialized in `pymilo_param` - Ensemble support added to `pymilo_func.py` -
+`SUPPORTED_MODELS.md` updated - `README.md` updated ## [0.7] - 2024-04-03 ###
+Added - `pymilo_nearest_neighbor_test` function added to `test_pymilo.py` -
 `NeighborsTreeTransporter` Transporter - `LocalOutlierFactor` model -
 `RadiusNeighborsClassifier` model - `RadiusNeighborsRegressor` model -
 `NearestCentroid` model - `NearestNeighbors` model - `KNeighborsClassifier`
 model - `KNeighborsRegressor` model - Neighbors models test runner - Neighbors
 chain ### Changed - Tests config modified - Neighbors params initialized in
 `pymilo_param` - Neighbors support added to `pymilo_func.py` -
 `SUPPORTED_MODELS.md` updated - `README.md` updated ## [0.6] - 2024-03-27 ###
@@ -159,14 +175,14 @@
 - `GeneralDataStructure` Transporter updated - `LabelBinerizer` Transporter
 updated - `linear model` chain updated - GeneralDataStructure transporter
 enhanced - LabelBinerizer transporter updated - transporters' chain router
 added to `pymilo func` - NeuralNetwork params initialized in `pymilo_param` -
 `pymilo_test` updated to support multiple models - `linear_model_chain`
 refactored ## [0.1] - 2023-06-29 ### Added - scikit-learn linear models support
 - `Export` class - `Import` class [Unreleased]: https://github.com/openscilab/
-pymilo/compare/v0.7...dev [0.7]: https://github.com/openscilab/pymilo/compare/
-v0.6...v0.7 [0.6]: https://github.com/openscilab/pymilo/compare/v0.5...v0.6
-[0.5]: https://github.com/openscilab/pymilo/compare/v0.4...v0.5 [0.4]: https://
-github.com/openscilab/pymilo/compare/v0.3...v0.4 [0.3]: https://github.com/
-openscilab/pymilo/compare/v0.2...v0.3 [0.2]: https://github.com/openscilab/
-pymilo/compare/v0.1...v0.2 [0.1]: https://github.com/openscilab/pymilo/compare/
-e887108...v0.1
+pymilo/compare/v0.8...dev [0.8]: https://github.com/openscilab/pymilo/compare/
+v0.7...v0.8 [0.7]: https://github.com/openscilab/pymilo/compare/v0.6...v0.7
+[0.6]: https://github.com/openscilab/pymilo/compare/v0.5...v0.6 [0.5]: https://
+github.com/openscilab/pymilo/compare/v0.4...v0.5 [0.4]: https://github.com/
+openscilab/pymilo/compare/v0.3...v0.4 [0.3]: https://github.com/openscilab/
+pymilo/compare/v0.2...v0.3 [0.2]: https://github.com/openscilab/pymilo/compare/
+v0.1...v0.2 [0.1]: https://github.com/openscilab/pymilo/compare/e887108...v0.1
```

### Comparing `pymilo-0.7/README.md` & `pymilo-0.8/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,19 @@
 <div align="center">
     <img src="https://github.com/openscilab/pymilo/raw/main/otherfiles/logo.png" width="500" height="300">
     <br/>
     <br/>
-    <a href="https://codecov.io/gh/openscilab/pymilo">
-        <img src="https://codecov.io/gh/openscilab/pymilo/branch/main/graph/badge.svg" alt="Codecov"/>
-    </a>
-    <a href="https://badge.fury.io/py/pymilo">
-        <img src="https://badge.fury.io/py/pymilo.svg" alt="PyPI version" height="18">
-    </a>
-    <a href="https://www.python.org/">
-        <img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3">
-    </a>
-    <a href="https://discord.gg/mtuMS8AjDS">
-        <img src="https://img.shields.io/discord/1064533716615049236.svg" alt="Discord Channel">
-    </a>
+    <a href="https://codecov.io/gh/openscilab/pymilo"><img src="https://codecov.io/gh/openscilab/pymilo/branch/main/graph/badge.svg" alt="Codecov"/></a>
+    <a href="https://badge.fury.io/py/pymilo"><img src="https://badge.fury.io/py/pymilo.svg" alt="PyPI version" height="18"></a>
+    <a href="https://www.python.org/"><img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3"></a>
+    <a href="https://discord.gg/mtuMS8AjDS"><img src="https://img.shields.io/discord/1064533716615049236.svg" alt="Discord Channel"></a>
 </div>
 
 ----------
 
-## Table of contents
-
-* [Overview](https://github.com/openscilab/pymilo#overview)
-* [Installation](https://github.com/openscilab/pymilo#installation)
-* [Usage](https://github.com/openscilab/pymilo#usage)
-* [Issues & Bug Reports](https://github.com/openscilab/pymilo#issues--bug-reports)
-* [Contribution](https://github.com/openscilab/pymilo/blob/main/.github/CONTRIBUTING.md)
-* [Authors](https://github.com/openscilab/pymilo/blob/main/AUTHORS.md)
-* [License](https://github.com/openscilab/pymilo/blob/main/LICENSE)
-* [Show Your Support](https://github.com/openscilab/pymilo#show-your-support)
-* [Changelog](https://github.com/openscilab/pymilo/blob/main/CHANGELOG.md)
-* [Code of Conduct](https://github.com/openscilab/pymilo/blob/main/.github/CODE_OF_CONDUCT.md)
-
-
 ## Overview
 <p align="justify">
 PyMilo is an open source Python package that provides a simple, efficient, and safe way for users to export pre-trained machine learning models in a transparent way. By this, the exported model can be used in other environments, transferred across different platforms, and shared with others. PyMilo allows the users to export the models that are trained using popular Python libraries like scikit-learn, and then use them in deployment environments, or share them without exposing the underlying code or dependencies. The transparency of the exported models ensures reliability and safety for the end users, as it eliminates the risks of binary or pickle formats.
 </p>
 <table>
     <tr>
         <td align="center">PyPI Counter</td>
@@ -82,17 +60,17 @@
 
 
 ## Installation
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)
-- Run `pip install pymilo==0.7`
+- Run `pip install pymilo==0.8`
 ### Source code
-- Download [Version 0.7](https://github.com/openscilab/pymilo/archive/v0.7.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
+- Download [Version 0.8](https://github.com/openscilab/pymilo/archive/v0.8.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
 - Run `pip install .`
 
 ## Usage
 ### Model preparation 
 ```pycon
 >>> from sklearn import datasets
 >>> from pymilo import Export, Import
@@ -118,27 +96,30 @@
 >>> #### Import the pymilo-exported model and get a real scikit model
 >>> imported_model = Import(PATH_TO_JSON_FILE)
 ```
 ### Get the associated model
 ```pycon 
 >>> imported_sklearn_model = imported_model.to_model()
 ```
-#### Note: `imported_sklearn_model` has the **exact same** functionality as the `model` object earlier.
+* Note: `imported_sklearn_model` has the **exact same** functionality as the `model` object earlier.
 
 ## Supported ML models
 | scikit-learn | PyTorch | 
 | ---------------- | ---------------- | 
 | Linear Models &#x2705; | - | 
 | Neural networks &#x2705; | -  | 
 | Trees &#x2705; | -  | 
 | Clustering &#x2705; | -  | 
 | Naïve Bayes &#x2705; | -  | 
 | Support vector machines (SVMs) &#x2705; | -  | 
-| Nearest Neighbors &#x2705; | -  | 
-| Ensemble Models &#x274C; | - | 
+| Nearest Neighbors &#x2705; | -  |  
+| Ensemble Models &#x2705; | - | 
+| Pipeline Model &#x2705; | - |
+| Preprocessing Models ⏳ | - |
+
 Details are available in [Supported Models](https://github.com/openscilab/pymilo/blob/main/SUPPORTED_MODELS.md).
 
 ## Issues & bug reports
 
 Just fill an issue and describe it. We'll check it ASAP! or send an email to [pymilo@openscilab.com](mailto:pymilo@openscilab.com "pymilo@openscilab.com"). 
 
 - Please complete the issue template
```

#### html2text {}

```diff
@@ -1,21 +1,11 @@
       [https://github.com/openscilab/pymilo/raw/main/otherfiles/logo.png]
 
          _[_C_o_d_e_c_o_v_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_b_u_i_l_t_ _w_i_t_h_ _P_y_t_h_o_n_3_]_[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]
----------- ## Table of contents * [Overview](https://github.com/openscilab/
-pymilo#overview) * [Installation](https://github.com/openscilab/
-pymilo#installation) * [Usage](https://github.com/openscilab/pymilo#usage) *
-[Issues & Bug Reports](https://github.com/openscilab/pymilo#issues--bug-
-reports) * [Contribution](https://github.com/openscilab/pymilo/blob/
-main/.github/CONTRIBUTING.md) * [Authors](https://github.com/openscilab/pymilo/
-blob/main/AUTHORS.md) * [License](https://github.com/openscilab/pymilo/blob/
-main/LICENSE) * [Show Your Support](https://github.com/openscilab/pymilo#show-
-your-support) * [Changelog](https://github.com/openscilab/pymilo/blob/main/
-CHANGELOG.md) * [Code of Conduct](https://github.com/openscilab/pymilo/blob/
-main/.github/CODE_OF_CONDUCT.md) ## Overview
+---------- ## Overview
 PyMilo is an open source Python package that provides a simple, efficient, and
 safe way for users to export pre-trained machine learning models in a
 transparent way. By this, the exported model can be used in other environments,
 transferred across different platforms, and shared with others. PyMilo allows
 the users to export the models that are trained using popular Python libraries
 like scikit-learn, and then use them in deployment environments, or share them
 without exposing the underlying code or dependencies. The transparency of the
@@ -28,38 +18,39 @@
         [https://github.com/openscilab/    [https://github.com/openscilab/
    CI  pymilo/actions/workflows/test.yml/ pymilo/actions/workflows/test.yml/
              badge.svg?branch=main]             badge.svg?branch=dev]
                           _[_h_t_t_p_s_:_/_/_a_p_p_._c_o_d_a_c_y_._c_o_m_/_p_r_o_j_e_c_t_/
 Code Quality _[_C_o_d_e_F_a_c_t_o_r_]           _b_a_d_g_e_/_G_r_a_d_e_/            _[_c_o_d_e_b_e_a_t_ _b_a_d_g_e_]
                           _9_e_e_e_c_9_9_e_d_1_1_f_4_d_9_b_8_6_a_f_3_6_d_c_9_0_f_5_f_7_5_3_]
 ## Installation ### PyPI - Check [Python Packaging User Guide](https://
-packaging.python.org/installing/) - Run `pip install pymilo==0.7` ### Source
-code - Download [Version 0.7](https://github.com/openscilab/pymilo/archive/
-v0.7.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
+packaging.python.org/installing/) - Run `pip install pymilo==0.8` ### Source
+code - Download [Version 0.8](https://github.com/openscilab/pymilo/archive/
+v0.8.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
 dev.zip) - Run `pip install .` ## Usage ### Model preparation ```pycon >>> from
 sklearn import datasets >>> from pymilo import Export, Import >>> from
 sklearn.linear_model import LinearRegression >>> import os >>> X, Y =
 datasets.load_diabetes(return_X_y=True) >>> threshold = 20 >>> X_train, X_test
 = X[:-threshold], X[-threshold:] >>> Y_train, Y_test = Y[:-threshold], Y[-
 threshold:] >>> model = LinearRegression() >>> #### Train the model using the
 training sets >>> model.fit(X_train, Y_train) ``` ### Save model ```pycon >>>
 #### Export the fitted model to a transparent json file >>> exported_model =
 Export(model) >>> PATH_TO_JSON_FILE = os.path.join(os.getcwd(),"test.json") >>>
 exported_model.save(PATH_TO_JSON_FILE) ``` ### Load model ```pycon >>> ####
 Import the pymilo-exported model and get a real scikit model >>> imported_model
 = Import(PATH_TO_JSON_FILE) ``` ### Get the associated model ```pycon >>>
-imported_sklearn_model = imported_model.to_model() ``` #### Note:
+imported_sklearn_model = imported_model.to_model() ``` * Note:
 `imported_sklearn_model` has the **exact same** functionality as the `model`
 object earlier. ## Supported ML models | scikit-learn | PyTorch | | -----------
 ----- | ---------------- | | Linear Models ✅ | - | | Neural networks ✅ | - | |
 Trees ✅ | - | | Clustering ✅ | - | | NaÃ¯ve Bayes ✅ | - | | Support vector
-machines (SVMs) ✅ | - | | Nearest Neighbors ✅ | - | | Ensemble Models ❌ | - |
-Details are available in [Supported Models](https://github.com/openscilab/
-pymilo/blob/main/SUPPORTED_MODELS.md). ## Issues & bug reports Just fill an
-issue and describe it. We'll check it ASAP! or send an email to
-[pymilo@openscilab.com](mailto:pymilo@openscilab.com "pymilo@openscilab.com").
-- Please complete the issue template You can also join our discord server
-_[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]## Show your support ### Star this repo Give a â­ï¸ if this
-project helped you! ### Donate to our project If you do like our project and we
-hope that you do, can you please support us? Our project is not and is never
-going to be working for profit. We need the money just so we can continue doing
-what we do ;-) ._[_P_y_M_i_l_o_ _D_o_n_a_t_i_o_n_]
+machines (SVMs) ✅ | - | | Nearest Neighbors ✅ | - | | Ensemble Models ✅ | - | |
+Pipeline Model ✅ | - | | Preprocessing Models â³ | - | Details are available
+in [Supported Models](https://github.com/openscilab/pymilo/blob/main/
+SUPPORTED_MODELS.md). ## Issues & bug reports Just fill an issue and describe
+it. We'll check it ASAP! or send an email to [pymilo@openscilab.com](mailto:
+pymilo@openscilab.com "pymilo@openscilab.com"). - Please complete the issue
+template You can also join our discord server _[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]## Show your
+support ### Star this repo Give a â­ï¸ if this project helped you! ### Donate
+to our project If you do like our project and we hope that you do, can you
+please support us? Our project is not and is never going to be working for
+profit. We need the money just so we can continue doing what we do ;-) ._[_P_y_M_i_l_o
+_D_o_n_a_t_i_o_n_]
```

### Comparing `pymilo-0.7/pymilo/chains/clustering_chain.py` & `pymilo-0.8/pymilo/chains/clustering_chain.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # -*- coding: utf-8 -*-
 """PyMilo chain for clustering models."""
 from ..transporters.transporter import Command
 
 from ..transporters.general_data_structure_transporter import GeneralDataStructureTransporter
 from ..transporters.function_transporter import FunctionTransporter
 from ..transporters.cfnode_transporter import CFNodeTransporter
+from ..transporters.preprocessing_transporter import PreprocessingTransporter
+
+from ..utils.util import get_sklearn_type
 
 from ..pymilo_param import SKLEARN_CLUSTERING_TABLE, NOT_SUPPORTED
 from ..exceptions.serialize_exception import PymiloSerializationException, SerilaizatoinErrorTypes
 from ..exceptions.deserialize_exception import PymiloDeserializationException, DeSerilaizatoinErrorTypes
 from traceback import format_exc
 
 bisecting_kmeans_support = SKLEARN_CLUSTERING_TABLE["BisectingKMeans"] != NOT_SUPPORTED
 CLUSTERING_CHAIN = {
+    "PreprocessingTransporter": PreprocessingTransporter(),
     "GeneralDataStructureTransporter": GeneralDataStructureTransporter(),
     "FunctionTransporter": FunctionTransporter(),
     "CFNodeTransporter": CFNodeTransporter(),
 }
 
 if bisecting_kmeans_support:
     from ..transporters.randomstate_transporter import RandomStateTransporter
@@ -32,28 +36,31 @@
     :param model: is a string name of a clusterer or a sklearn object of it
     :type model: any object
     :return: check result as bool
     """
     if isinstance(model, str):
         return model in SKLEARN_CLUSTERING_TABLE
     else:
-        return type(model) in SKLEARN_CLUSTERING_TABLE.values()
+        return get_sklearn_type(model) in SKLEARN_CLUSTERING_TABLE.keys()
 
 
-def transport_clusterer(request, command):
+def transport_clusterer(request, command, is_inner_model=False):
     """
     Return the transported (Serialized or Deserialized) model.
 
     :param request: given clusterer to be transported
     :type request: any object
     :param command: command to specify whether the request should be serialized or deserialized
     :type command: transporter.Command
+    :param is_inner_model: determines whether it is an inner linear model of a super ml model
+    :type is_inner_model: boolean
     :return: the transported request as a json string or sklearn clustering model
     """
-    _validate_input(request, command)
+    if not is_inner_model:
+        _validate_input(request, command)
 
     if command == Command.SERIALIZE:
         try:
             return serialize_clusterer(request)
         except Exception as e:
             raise PymiloSerializationException(
                 {
@@ -63,15 +70,15 @@
                         'Traceback': format_exc(),
                     },
                     'object': request,
                 })
 
     elif command == Command.DESERIALZIE:
         try:
-            return deserialize_clusterer(request)
+            return deserialize_clusterer(request, is_inner_model)
         except Exception as e:
             raise PymiloDeserializationException(
                 {
                     'error_type': SerilaizatoinErrorTypes.VALID_MODEL_INVALID_INTERNAL_STRUCTURE,
                     'error': {
                         'Exception': repr(e),
                         'Traceback': format_exc()},
@@ -88,28 +95,36 @@
     """
     for transporter in CLUSTERING_CHAIN:
         CLUSTERING_CHAIN[transporter].transport(
             clusterer_object, Command.SERIALIZE)
     return clusterer_object.__dict__
 
 
-def deserialize_clusterer(clusterer):
+def deserialize_clusterer(clusterer, is_inner_model=False):
     """
     Return the associated sklearn clustering model of the given clusterer.
 
     :param clusterer: given json string of a clustering model to get deserialized to associated sklearn clustering model
     :type clusterer: obj
+    :param is_inner_model: determines whether it is an inner linear model of a super ml model
+    :type is_inner_model: boolean
     :return: associated sklearn clustering model
     """
-    raw_model = SKLEARN_CLUSTERING_TABLE[clusterer.type]()
-    data = clusterer.data
+    raw_model = None
+    data = None
+    if is_inner_model:
+        raw_model = SKLEARN_CLUSTERING_TABLE[clusterer["type"]]()
+        data = clusterer["data"]
+    else:
+        raw_model = SKLEARN_CLUSTERING_TABLE[clusterer.type]()
+        data = clusterer.data
 
     for transporter in CLUSTERING_CHAIN:
         CLUSTERING_CHAIN[transporter].transport(
-            clusterer, Command.DESERIALZIE)
+            clusterer, Command.DESERIALZIE, is_inner_model)
     for item in data:
         setattr(raw_model, item, data[item])
     return raw_model
 
 
 def _validate_input(model, command):
     """
```

### Comparing `pymilo-0.7/pymilo/chains/linear_model_chain.py` & `pymilo-0.8/pymilo/chains/linear_model_chain.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,73 @@
 # -*- coding: utf-8 -*-
 """PyMilo chain for linear models."""
 from ..transporters.transporter import Command
 
 from ..transporters.general_data_structure_transporter import GeneralDataStructureTransporter
 from ..transporters.baseloss_transporter import BaseLossTransporter
 from ..transporters.lossfunction_transporter import LossFunctionTransporter
-from ..transporters.labelbinarizer_transporter import LabelBinarizerTransporter
+from ..transporters.preprocessing_transporter import PreprocessingTransporter
 
 from ..pymilo_param import SKLEARN_LINEAR_MODEL_TABLE
 from ..utils.util import get_sklearn_type, is_iterable
 
 from ..exceptions.serialize_exception import PymiloSerializationException, SerilaizatoinErrorTypes
 from ..exceptions.deserialize_exception import PymiloDeserializationException, DeSerilaizatoinErrorTypes
 from traceback import format_exc
 
 
 LINEAR_MODEL_CHAIN = {
+    "PreprocessingTransporter": PreprocessingTransporter(),
     "GeneralDataStructureTransporter": GeneralDataStructureTransporter(),
     "BaseLossTransporter": BaseLossTransporter(),
     "LossFunctionTransporter": LossFunctionTransporter(),
-    "LabelBinarizerTransporter": LabelBinarizerTransporter()}
+}
 
 
 def is_linear_model(model):
     """
     Check if the input model is a sklearn's linear model.
 
     :param model: name of a linear model or a sklearn object of it
     :type model: any object
     :return: check result as bool
     """
     if isinstance(model, str):
         return model in SKLEARN_LINEAR_MODEL_TABLE
     else:
-        return type(model) in SKLEARN_LINEAR_MODEL_TABLE.values()
+        return get_sklearn_type(model) in SKLEARN_LINEAR_MODEL_TABLE.keys()
 
 
 def is_deserialized_linear_model(content):
     """
     Check if the given content is a previously serialized model by Pymilo's Export or not.
 
     :param content: given object to be authorized as a valid pymilo exported serialized model
     :type content: any object
     :return: check result as bool
     """
     if not is_iterable(content):
         return False
-    return "inner-model-type" in content and "inner-model-data" in content
+    return "pymilo-inner-model-type" in content and "pymilo-inner-model-data" in content
 
 
 def transport_linear_model(request, command, is_inner_model=False):
     """
     Return the transported (Serialized or Deserialized) model.
 
     :param request: given model to be transported
     :type request: any object
     :param command: command to specify whether the request should be serialized or deserialized
     :type command: transporter.Command
-    :param is_inner_model: determines whether the request is an inner linear model, as a single field of a wrapper linear model
+    :param is_inner_model: determines whether it is an inner linear model of a super ml model
     :type is_inner_model: boolean
     :return: the transported request as a json string or sklearn linear model
     """
     if not is_inner_model:
-        validate_input(request, command, is_inner_model)
+        validate_input(request, command)
 
     if command == Command.SERIALIZE:
         try:
             return serialize_linear_model(request)
         except Exception as e:
             raise PymiloSerializationException(
                 {
@@ -97,32 +98,32 @@
     :type linear_model_object: any sklearn linear model
     :return: the serialized json string of the given linear model
     """
     # first serializing the inner linear models...
     for key in linear_model_object.__dict__:
         if is_linear_model(linear_model_object.__dict__[key]):
             linear_model_object.__dict__[key] = {
-                "inner-model-data": transport_linear_model(linear_model_object.__dict__[key], Command.SERIALIZE),
-                "inner-model-type": get_sklearn_type(linear_model_object.__dict__[key]),
-                "by-pass": True
+                "pymilo-inner-model-data": transport_linear_model(linear_model_object.__dict__[key], Command.SERIALIZE, True),
+                "pymilo-inner-model-type": get_sklearn_type(linear_model_object.__dict__[key]),
+                "pymilo-by-pass": True
             }
     # now serializing non-linear model fields
     for transporter in LINEAR_MODEL_CHAIN:
         LINEAR_MODEL_CHAIN[transporter].transport(
             linear_model_object, Command.SERIALIZE)
     return linear_model_object.__dict__
 
 
 def deserialize_linear_model(linear_model, is_inner_model):
     """
     Return the associated sklearn linear model of the given linear_model.
 
     :param linear_model: given json string of a linear model to get deserialized to associated sklearn linear model
     :type linear_model: obj
-    :param is_inner_model: determines whether the request is an inner linear model, as a single field of a wrapper linear model
+    :param is_inner_model: determines whether it is an inner linear model of a super ml model
     :type is_inner_model: boolean
     :return: associated sklearn linear model
     """
     raw_model = None
     data = None
     if is_inner_model:
         raw_model = SKLEARN_LINEAR_MODEL_TABLE[linear_model["type"]]()
@@ -131,50 +132,48 @@
         raw_model = SKLEARN_LINEAR_MODEL_TABLE[linear_model.type]()
         data = linear_model.data
     # first deserializing the inner linear models(one depth inner linear
     # models have been deserialized -> TODO full depth).
     for key in data:
         if is_deserialized_linear_model(data[key]):
             data[key] = transport_linear_model({
-                "data": data[key]["inner-model-data"],
-                "type": data[key]["inner-model-type"]
+                "data": data[key]["pymilo-inner-model-data"],
+                "type": data[key]["pymilo-inner-model-type"]
             }, Command.DESERIALZIE, is_inner_model=True)
     # now deserializing non-linear models fields
     for transporter in LINEAR_MODEL_CHAIN:
         LINEAR_MODEL_CHAIN[transporter].transport(
             linear_model, Command.DESERIALZIE, is_inner_model)
     for item in data:
         setattr(raw_model, item, data[item])
     return raw_model
 
 
-def validate_input(model, command, is_inner_model):
+def validate_input(model, command):
     """
     Check if the provided inputs are valid in relation to each other.
 
     :param model: a sklearn linear model or a json string of it, serialized through the pymilo export.
     :type model: obj
     :param command: command to specify whether the request should be serialized or deserialized
     :type command: transporter.Command
-    :param is_inner_model: determines whether the request is an inner linear model, as a single field of a wrapper linear model
-    :type is_inner_model: boolean
     :return: None
     """
     if command == Command.SERIALIZE:
         if is_linear_model(model):
             return
         else:
             raise PymiloSerializationException(
                 {
                     'error_type': SerilaizatoinErrorTypes.INVALID_MODEL,
                     'object': model
                 }
             )
     elif command == Command.DESERIALZIE:
-        model_type = model["type"] if is_inner_model else model.type
+        model_type = model.type
         if is_linear_model(model_type):
             return
         else:
             raise PymiloDeserializationException(
                 {
                     'error_type': DeSerilaizatoinErrorTypes.INVALID_MODEL,
                     'object': model
```

### Comparing `pymilo-0.7/pymilo/chains/naive_bayes_chain.py` & `pymilo-0.8/pymilo/chains/naive_bayes_chain.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # -*- coding: utf-8 -*-
 """PyMilo chain for naive bayes models."""
 from ..transporters.transporter import Command
 
 from ..transporters.general_data_structure_transporter import GeneralDataStructureTransporter
+from ..transporters.preprocessing_transporter import PreprocessingTransporter
 
 from ..pymilo_param import SKLEARN_NAIVE_BAYES_TABLE
 from ..exceptions.serialize_exception import PymiloSerializationException, SerilaizatoinErrorTypes
 from ..exceptions.deserialize_exception import PymiloDeserializationException, DeSerilaizatoinErrorTypes
+
+from ..utils.util import get_sklearn_type
+
 from traceback import format_exc
 
 NAIVE_BAYES_CHAIN = {
+    "PreprocessingTransporter": PreprocessingTransporter(),
     "GeneralDataStructureTransporter": GeneralDataStructureTransporter(),
 }
 
 
 def is_naive_bayes(model):
     """
     Check if the input model is a sklearn's naive bayes model.
@@ -21,28 +26,31 @@
     :param model: is a string name of a naive bayes or a sklearn object of it
     :type model: any object
     :return: check result as bool
     """
     if isinstance(model, str):
         return model in SKLEARN_NAIVE_BAYES_TABLE
     else:
-        return type(model) in SKLEARN_NAIVE_BAYES_TABLE.values()
+        return get_sklearn_type(model) in SKLEARN_NAIVE_BAYES_TABLE.keys()
 
 
-def transport_naive_bayes(request, command):
+def transport_naive_bayes(request, command, is_inner_model=False):
     """
     Return the transported (Serialized or Deserialized) model.
 
     :param request: given naive bayes to be transported
     :type request: any object
     :param command: command to specify whether the request should be serialized or deserialized
     :type command: transporter.Command
+    :param is_inner_model: determines whether it is an inner linear model of a super ml model
+    :type is_inner_model: boolean
     :return: the transported request as a json string or sklearn naive bayes model
     """
-    _validate_input(request, command)
+    if not is_inner_model:
+        _validate_input(request, command)
 
     if command == Command.SERIALIZE:
         try:
             return serialize_naive_bayes(request)
         except Exception as e:
             raise PymiloSerializationException(
                 {
@@ -52,15 +60,15 @@
                         'Traceback': format_exc(),
                     },
                     'object': request,
                 })
 
     elif command == Command.DESERIALZIE:
         try:
-            return deserialize_naive_bayes(request)
+            return deserialize_naive_bayes(request, is_inner_model)
         except Exception as e:
             raise PymiloDeserializationException(
                 {
                     'error_type': SerilaizatoinErrorTypes.VALID_MODEL_INVALID_INTERNAL_STRUCTURE,
                     'error': {
                         'Exception': repr(e),
                         'Traceback': format_exc()},
@@ -77,28 +85,36 @@
     """
     for transporter in NAIVE_BAYES_CHAIN:
         NAIVE_BAYES_CHAIN[transporter].transport(
             naive_bayes_object, Command.SERIALIZE)
     return naive_bayes_object.__dict__
 
 
-def deserialize_naive_bayes(naive_bayes):
+def deserialize_naive_bayes(naive_bayes, is_inner_model=False):
     """
     Return the associated sklearn naive bayes model of the given naive bayes.
 
     :param naive bayes: given json string of a naive bayes model to get deserialized to associated sklearn naive bayes model
     :type naive bayes: obj
+    :param is_inner_model: determines whether it is an inner linear model of a super ml model
+    :type is_inner_model: boolean
     :return: associated sklearn naive bayes model
     """
-    raw_model = SKLEARN_NAIVE_BAYES_TABLE[naive_bayes.type]()
-    data = naive_bayes.data
+    raw_model = None
+    data = None
+    if is_inner_model:
+        raw_model = SKLEARN_NAIVE_BAYES_TABLE[naive_bayes["type"]]()
+        data = naive_bayes["data"]
+    else:
+        raw_model = SKLEARN_NAIVE_BAYES_TABLE[naive_bayes.type]()
+        data = naive_bayes.data
 
     for transporter in NAIVE_BAYES_CHAIN:
         NAIVE_BAYES_CHAIN[transporter].transport(
-            naive_bayes, Command.DESERIALZIE)
+            naive_bayes, Command.DESERIALZIE, is_inner_model)
     for item in data:
         setattr(raw_model, item, data[item])
     return raw_model
 
 
 def _validate_input(model, command):
     """
```

### Comparing `pymilo-0.7/pymilo/chains/neighbours_chain.py` & `pymilo-0.8/pymilo/chains/neighbours_chain.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # -*- coding: utf-8 -*-
 """PyMilo chain for neighbors models."""
 from ..transporters.transporter import Command
 
 from ..transporters.general_data_structure_transporter import GeneralDataStructureTransporter
 from ..transporters.neighbors_tree_transporter import NeighborsTreeTransporter
+from ..transporters.preprocessing_transporter import PreprocessingTransporter
 
 from ..pymilo_param import SKLEARN_NEIGHBORS_TABLE
 from ..exceptions.serialize_exception import PymiloSerializationException, SerilaizatoinErrorTypes
 from ..exceptions.deserialize_exception import PymiloDeserializationException, DeSerilaizatoinErrorTypes
+
+from ..utils.util import get_sklearn_type
+
 from traceback import format_exc
 
 NEIGHBORS_CHAIN = {
+    "PreprocessingTransporter": PreprocessingTransporter(),
     "GeneralDataStructureTransporter": GeneralDataStructureTransporter(),
     "NeighborsTreeTransporter": NeighborsTreeTransporter(),
 }
 
 
 def is_neighbors(model):
     """
@@ -23,28 +28,31 @@
     :param model: is a string name of a neighbor or a sklearn object of it
     :type model: any object
     :return: check result as bool
     """
     if isinstance(model, str):
         return model in SKLEARN_NEIGHBORS_TABLE
     else:
-        return type(model) in SKLEARN_NEIGHBORS_TABLE.values()
+        return get_sklearn_type(model) in SKLEARN_NEIGHBORS_TABLE.keys()
 
 
-def transport_neighbor(request, command):
+def transport_neighbor(request, command, is_inner_model=False):
     """
     Return the transported (Serialized or Deserialized) model.
 
     :param request: given neighbor to be transported
     :type request: any object
     :param command: command to specify whether the request should be serialized or deserialized
     :type command: transporter.Command
+    :param is_inner_model: determines whether it is an inner linear model of a super ml model
+    :type is_inner_model: boolean
     :return: the transported request as a json string or sklearn neighbors model
     """
-    _validate_input(request, command)
+    if not is_inner_model:
+        _validate_input(request, command)
 
     if command == Command.SERIALIZE:
         try:
             return serialize_neighbor(request)
         except Exception as e:
             raise PymiloSerializationException(
                 {
@@ -54,15 +62,15 @@
                         'Traceback': format_exc(),
                     },
                     'object': request,
                 })
 
     elif command == Command.DESERIALZIE:
         try:
-            return deserialize_neighbor(request)
+            return deserialize_neighbor(request, is_inner_model)
         except Exception as e:
             raise PymiloDeserializationException(
                 {
                     'error_type': SerilaizatoinErrorTypes.VALID_MODEL_INVALID_INTERNAL_STRUCTURE,
                     'error': {
                         'Exception': repr(e),
                         'Traceback': format_exc()},
@@ -79,28 +87,36 @@
     """
     for transporter in NEIGHBORS_CHAIN:
         NEIGHBORS_CHAIN[transporter].transport(
             neighbor_object, Command.SERIALIZE)
     return neighbor_object.__dict__
 
 
-def deserialize_neighbor(neighbor):
+def deserialize_neighbor(neighbor, is_inner_model=False):
     """
     Return the associated sklearn neighbor model of the given neighbor.
 
     :param neighbor: given json string of a neighbor model to get deserialized to associated sklearn neighbors model
     :type neighbor: obj
+    :param is_inner_model: determines whether it is an inner linear model of a super ml model
+    :type is_inner_model: boolean
     :return: associated sklearn neighbor model
     """
-    raw_model = SKLEARN_NEIGHBORS_TABLE[neighbor.type]()
-    data = neighbor.data
+    raw_model = None
+    data = None
+    if is_inner_model:
+        raw_model = SKLEARN_NEIGHBORS_TABLE[neighbor["type"]]()
+        data = neighbor["data"]
+    else:
+        raw_model = SKLEARN_NEIGHBORS_TABLE[neighbor.type]()
+        data = neighbor.data
 
     for transporter in NEIGHBORS_CHAIN:
         NEIGHBORS_CHAIN[transporter].transport(
-            neighbor, Command.DESERIALZIE)
+            neighbor, Command.DESERIALZIE, is_inner_model)
     for item in data:
         setattr(raw_model, item, data[item])
     return raw_model
 
 
 def _validate_input(model, command):
     """
```

### Comparing `pymilo-0.7/pymilo/chains/neural_network_chain.py` & `pymilo-0.8/pymilo/chains/neural_network_chain.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,57 +2,63 @@
 """PyMilo chain for linear models."""
 from ..transporters.transporter import Command
 
 from ..transporters.general_data_structure_transporter import GeneralDataStructureTransporter
 from ..transporters.randomstate_transporter import RandomStateTransporter
 from ..transporters.sgdoptimizer_transporter import SGDOptimizerTransporter
 from ..transporters.adamoptimizer_transporter import AdamOptimizerTransporter
-from ..transporters.labelbinarizer_transporter import LabelBinarizerTransporter
+from ..transporters.preprocessing_transporter import PreprocessingTransporter
 
 from ..pymilo_param import SKLEARN_NEURAL_NETWORK_TABLE
 
 from ..exceptions.serialize_exception import PymiloSerializationException, SerilaizatoinErrorTypes
 from ..exceptions.deserialize_exception import PymiloDeserializationException, DeSerilaizatoinErrorTypes
+
+from ..utils.util import get_sklearn_type
+
 from traceback import format_exc
 
 
 NEURAL_NETWORK_CHAIN = {
+    "PreprocessingTransporter": PreprocessingTransporter(),
     "GeneralDataStructureTransporter": GeneralDataStructureTransporter(),
     "RandomStateTransporter": RandomStateTransporter(),
     "SGDOptimizer": SGDOptimizerTransporter(),
     "AdamOptimizerTransporter": AdamOptimizerTransporter(),
-    "LabelBinarizerTransporter": LabelBinarizerTransporter(),
 }
 
 
 def is_neural_network(model):
     """
     Check if the input model is a sklearn's neural network.
 
     :param model: is a string name of a neural network or a sklearn object of it
     :type model: any object
     :return: check result as bool
     """
     if isinstance(model, str):
         return model in SKLEARN_NEURAL_NETWORK_TABLE
     else:
-        return type(model) in SKLEARN_NEURAL_NETWORK_TABLE.values()
+        return get_sklearn_type(model) in SKLEARN_NEURAL_NETWORK_TABLE.keys()
 
 
-def transport_neural_network(request, command):
+def transport_neural_network(request, command, is_inner_model=False):
     """
     Return the transported (Serialized or Deserialized) model.
 
     :param request: given neural network model to be transported
     :type request: any object
     :param command: command to specify whether the request should be serialized or deserialized
     :type command: transporter.Command
+    :param is_inner_model: determines whether it is an inner linear model of a super ml model
+    :type is_inner_model: boolean
     :return: the transported request as a json string or sklearn neural network model
     """
-    _validate_input(request, command)
+    if not is_inner_model:
+        _validate_input(request, command)
 
     if command == Command.SERIALIZE:
         try:
             return serialize_neural_network(request)
         except Exception as e:
             raise PymiloSerializationException(
                 {
@@ -62,15 +68,15 @@
                         'Traceback': format_exc(),
                     },
                     'object': request,
                 })
 
     elif command == Command.DESERIALZIE:
         try:
-            return deserialize_neural_network(request)
+            return deserialize_neural_network(request, is_inner_model)
         except Exception as e:
             raise PymiloDeserializationException(
                 {
                     'error_type': SerilaizatoinErrorTypes.VALID_MODEL_INVALID_INTERNAL_STRUCTURE,
                     'error': {
                         'Exception': repr(e),
                         'Traceback': format_exc()},
@@ -87,28 +93,36 @@
     """
     for transporter in NEURAL_NETWORK_CHAIN:
         NEURAL_NETWORK_CHAIN[transporter].transport(
             neural_network_object, Command.SERIALIZE)
     return neural_network_object.__dict__
 
 
-def deserialize_neural_network(neural_network):
+def deserialize_neural_network(neural_network, is_inner_model=False):
     """
     Return the associated sklearn neural network model of the given neural_network.
 
     :param neural_network: given json string of a neural network model to get deserialized to associated sklearn NN model
     :type neural_network: obj
+    :param is_inner_model: determines whether it is an inner linear model of a super ml model
+    :type is_inner_model: boolean
     :return: associated sklearn NN model
     """
-    raw_model = SKLEARN_NEURAL_NETWORK_TABLE[neural_network.type]()
-    data = neural_network.data
+    raw_model = None
+    data = None
+    if is_inner_model:
+        raw_model = SKLEARN_NEURAL_NETWORK_TABLE[neural_network["type"]]()
+        data = neural_network["data"]
+    else:
+        raw_model = SKLEARN_NEURAL_NETWORK_TABLE[neural_network.type]()
+        data = neural_network.data
 
     for transporter in NEURAL_NETWORK_CHAIN:
         NEURAL_NETWORK_CHAIN[transporter].transport(
-            neural_network, Command.DESERIALZIE)
+            neural_network, Command.DESERIALZIE, is_inner_model)
     for item in data:
         setattr(raw_model, item, data[item])
     return raw_model
 
 
 def _validate_input(model, command):
     """
```

### Comparing `pymilo-0.7/pymilo/chains/svm_chain.py` & `pymilo-0.8/pymilo/chains/svm_chain.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # -*- coding: utf-8 -*-
 """PyMilo chain for svm models."""
 from ..transporters.transporter import Command
 
 from ..transporters.general_data_structure_transporter import GeneralDataStructureTransporter
 from ..transporters.randomstate_transporter import RandomStateTransporter
+from ..transporters.preprocessing_transporter import PreprocessingTransporter
 
 from ..pymilo_param import SKLEARN_SVM_TABLE
 from ..exceptions.serialize_exception import PymiloSerializationException, SerilaizatoinErrorTypes
 from ..exceptions.deserialize_exception import PymiloDeserializationException, DeSerilaizatoinErrorTypes
+
+from ..utils.util import get_sklearn_type
+
 from traceback import format_exc
 
 SVM_CHAIN = {
+    "PreprocessingTransporter": PreprocessingTransporter(),
     "GeneralDataStructureTransporter": GeneralDataStructureTransporter(),
     "RandomStateTransporter": RandomStateTransporter(),
 }
 
 
 def is_svm(model):
     """
@@ -23,28 +28,31 @@
     :param model: is a string name of a svm or a sklearn object of it
     :type model: any object
     :return: check result as bool
     """
     if isinstance(model, str):
         return model in SKLEARN_SVM_TABLE
     else:
-        return type(model) in SKLEARN_SVM_TABLE.values()
+        return get_sklearn_type(model) in SKLEARN_SVM_TABLE.keys()
 
 
-def transport_svm(request, command):
+def transport_svm(request, command, is_inner_model=False):
     """
     Return the transported (Serialized or Deserialized) model.
 
     :param request: given svm to be transported
     :type request: any object
     :param command: command to specify whether the request should be serialized or deserialized
     :type command: transporter.Command
+    :param is_inner_model: determines whether it is an inner linear model of a super ml model
+    :type is_inner_model: boolean
     :return: the transported request as a json string or sklearn svm model
     """
-    _validate_input(request, command)
+    if not is_inner_model:
+        _validate_input(request, command)
 
     if command == Command.SERIALIZE:
         try:
             return serialize_svm(request)
         except Exception as e:
             raise PymiloSerializationException(
                 {
@@ -54,15 +62,15 @@
                         'Traceback': format_exc(),
                     },
                     'object': request,
                 })
 
     elif command == Command.DESERIALZIE:
         try:
-            return deserialize_svm(request)
+            return deserialize_svm(request, is_inner_model)
         except Exception as e:
             raise PymiloDeserializationException(
                 {
                     'error_type': SerilaizatoinErrorTypes.VALID_MODEL_INVALID_INTERNAL_STRUCTURE,
                     'error': {
                         'Exception': repr(e),
                         'Traceback': format_exc()},
@@ -79,28 +87,36 @@
     """
     for transporter in SVM_CHAIN:
         SVM_CHAIN[transporter].transport(
             svm_object, Command.SERIALIZE)
     return svm_object.__dict__
 
 
-def deserialize_svm(svm):
+def deserialize_svm(svm, is_inner_model=False):
     """
     Return the associated sklearn svm model of the given svm.
 
     :param svm: given json string of a svm model to get deserialized to associated sklearn svm model
     :type svm: obj
+    :param is_inner_model: determines whether it is an inner linear model of a super ml model
+    :type is_inner_model: boolean
     :return: associated sklearn svm model
     """
-    raw_model = SKLEARN_SVM_TABLE[svm.type]()
-    data = svm.data
+    raw_model = None
+    data = None
+    if is_inner_model:
+        raw_model = SKLEARN_SVM_TABLE[svm["type"]]()
+        data = svm["data"]
+    else:
+        raw_model = SKLEARN_SVM_TABLE[svm.type]()
+        data = svm.data
 
     for transporter in SVM_CHAIN:
         SVM_CHAIN[transporter].transport(
-            svm, Command.DESERIALZIE)
+            svm, Command.DESERIALZIE, is_inner_model)
     for item in data:
         setattr(raw_model, item, data[item])
     return raw_model
 
 
 def _validate_input(model, command):
     """
```

### Comparing `pymilo-0.7/pymilo/exceptions/deserialize_exception.py` & `pymilo-0.8/pymilo/exceptions/deserialize_exception.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.7/pymilo/exceptions/pymilo_exception.py` & `pymilo-0.8/pymilo/exceptions/pymilo_exception.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.7/pymilo/exceptions/serialize_exception.py` & `pymilo-0.8/pymilo/exceptions/serialize_exception.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.7/pymilo/pymilo_obj.py` & `pymilo-0.8/pymilo/pymilo_obj.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """PyMilo modules."""
 from .pymilo_func import get_sklearn_data, get_sklearn_version, to_sklearn_model
 from .utils.util import get_sklearn_type
-from .pymilo_param import PYMILO_VERSION, PYMILO_VERSION_DOES_NOT_EXIST, UNEQUAL_PYMILO_VERSIONS
+from .pymilo_param import PYMILO_VERSION, PYMILO_VERSION_DOES_NOT_EXIST, UNEQUAL_PYMILO_VERSIONS, UNEQUAL_SKLEARN_VERSIONS
 import json
 
 from .exceptions.deserialize_exception import PymiloDeserializationException, DeSerilaizatoinErrorTypes
 from .exceptions.serialize_exception import PymiloSerializationException, SerilaizatoinErrorTypes
 from traceback import format_exc
 from warnings import warn
 
@@ -100,14 +100,16 @@
             else:
                 with open(file_adr, 'r') as fp:
                     serialized_model_obj = json.load(fp)
             if "pymilo_version" not in serialized_model_obj:
                 raise Exception(PYMILO_VERSION_DOES_NOT_EXIST)
             if not serialized_model_obj["pymilo_version"] == PYMILO_VERSION:
                 warn(UNEQUAL_PYMILO_VERSIONS, category=Warning)
+            if not serialized_model_obj["sklearn_version"] == get_sklearn_version():
+                warn(UNEQUAL_SKLEARN_VERSIONS, category=Warning)
             self.data = serialized_model_obj["data"]
             self.version = serialized_model_obj["sklearn_version"]
             self.type = serialized_model_obj["model_type"]
         except Exception as e:
             json_content = None
             if json_dump and isinstance(json_dump, str):
                 json_content = json_dump
```

### Comparing `pymilo-0.7/pymilo/pymilo_param.py` & `pymilo-0.8/pymilo/pymilo_param.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,110 +1,30 @@
 # -*- coding: utf-8 -*-
 """Parameters and constants."""
-from sklearn.neighbors import KNeighborsRegressor
-from sklearn.neighbors import KNeighborsClassifier
-from sklearn.neighbors import RadiusNeighborsRegressor
-from sklearn.neighbors import RadiusNeighborsClassifier
-from sklearn.neighbors import NearestNeighbors
-from sklearn.neighbors import NearestCentroid
-from sklearn.neighbors import LocalOutlierFactor
-
-from sklearn.svm import SVR
-from sklearn.svm import SVC
-from sklearn.svm import OneClassSVM
-from sklearn.svm import NuSVR
-from sklearn.svm import NuSVC
-from sklearn.svm import LinearSVR
-from sklearn.svm import LinearSVC
-from sklearn.naive_bayes import CategoricalNB
-from sklearn.naive_bayes import BernoulliNB
-from sklearn.naive_bayes import ComplementNB
-from sklearn.naive_bayes import MultinomialNB
-from sklearn.naive_bayes import GaussianNB
-from sklearn.preprocessing import LabelBinarizer
-from numpy import uint8
-from numpy import intc
-from numpy import inf
-from numpy import float64
-from numpy import int32
-from numpy import int64
-from sklearn.mixture import BayesianGaussianMixture
-from sklearn.mixture import GaussianMixture
-from sklearn.cluster import Birch
-from sklearn.cluster import OPTICS
-from sklearn.linear_model import HuberRegressor
-from sklearn.linear_model import TheilSenRegressor
-from sklearn.linear_model import RANSACRegressor
-from sklearn.linear_model import PassiveAggressiveRegressor
-from sklearn.linear_model import PassiveAggressiveClassifier
-from sklearn.linear_model import Perceptron
-from sklearn.linear_model import SGDClassifier
-from sklearn.linear_model import SGDRegressor
-from sklearn.linear_model import LogisticRegressionCV
-from sklearn.linear_model import LogisticRegression
-from sklearn.linear_model import ARDRegression
-from sklearn.linear_model import BayesianRidge
-from sklearn.linear_model import OrthogonalMatchingPursuitCV
-from sklearn.linear_model import OrthogonalMatchingPursuit
-from sklearn.linear_model import MultiTaskElasticNetCV
-from sklearn.linear_model import MultiTaskElasticNet
-from sklearn.linear_model import ElasticNetCV
-from sklearn.linear_model import ElasticNet
-from sklearn.linear_model import MultiTaskLassoCV
-from sklearn.linear_model import MultiTaskLasso
-from sklearn.linear_model import LassoLarsIC
-from sklearn.linear_model import LassoLarsCV
-from sklearn.linear_model import LassoLars
-from sklearn.linear_model import LassoCV
-from sklearn.linear_model import Lasso
-from sklearn.linear_model import RidgeClassifierCV
-from sklearn.linear_model import RidgeClassifier
-from sklearn.linear_model import RidgeCV
-from sklearn.linear_model import Ridge
-from sklearn.linear_model import LinearRegression
-
-from sklearn.neural_network import MLPRegressor
-from sklearn.neural_network import MLPClassifier
-from sklearn.neural_network import BernoulliRBM
-
-from sklearn.tree import DecisionTreeRegressor
-from sklearn.tree import DecisionTreeClassifier
-from sklearn.tree import ExtraTreeRegressor
-from sklearn.tree import ExtraTreeClassifier
-
-from sklearn.cluster import KMeans
-from sklearn.cluster import MiniBatchKMeans
-from sklearn.cluster import AffinityPropagation
-from sklearn.cluster import MeanShift
-from sklearn.cluster import SpectralClustering
-from sklearn.cluster import SpectralBiclustering
-from sklearn.cluster import SpectralCoclustering
-from sklearn.cluster import AgglomerativeClustering
-from sklearn.cluster import FeatureAgglomeration
-from sklearn.cluster import DBSCAN
+import numpy as np
+import sklearn.linear_model as linear_model
+import sklearn.neural_network as neural_network
+import sklearn.tree as tree
+import sklearn.cluster as cluster
+import sklearn.mixture as mixture
+import sklearn.naive_bayes as naive_bayes
+import sklearn.svm as svm
+import sklearn.neighbors as neighbors
+import sklearn.dummy as dummy
+import sklearn.ensemble as ensemble
+import sklearn.pipeline as pipeline
+import sklearn.preprocessing as preprocessing
 
-bisecting_kmeans_support = False
-try:
-    from sklearn.cluster import BisectingKMeans
-    bisecting_kmeans_support = True
-except BaseException:
-    pass
-
-hdbscan_support = False
+quantile_regressor_support = False
 try:
-    from sklearn.cluster import HDBSCAN
-    hdbscan_support = True
+    from sklearn.linear_model import QuantileRegressor
+    quantile_regressor_support = True
 except BaseException:
     pass
 
-PYMILO_VERSION = "0.7"
-NOT_SUPPORTED = "NOT_SUPPORTED"
-PYMILO_VERSION_DOES_NOT_EXIST = "Corrupted JSON file, `pymilo_version` doesn't exist in this file."
-UNEQUAL_PYMILO_VERSIONS = "warning: Installed Pymilo version differes from pymilo version used to create the JSON file."
-
 glm_support = {
     'GammaRegressor': False,
     'PoissonRegressor': False,
     'TweedieRegressor': False
 }
 try:
     from sklearn.linear_model import TweedieRegressor
@@ -112,150 +32,206 @@
     from sklearn.linear_model import PoissonRegressor
     glm_support['PoissonRegressor'] = True
     from sklearn.linear_model import GammaRegressor
     glm_support['GammaRegressor'] = True
 except BaseException:
     pass
 
-
 sgd_one_class_svm_support = False
 try:
     from sklearn.linear_model import SGDOneClassSVM
     sgd_one_class_svm_support = True
 except BaseException:
     pass
 
 
-quantile_regressor_support = False
+bisecting_kmeans_support = False
 try:
-    from sklearn.linear_model import QuantileRegressor
-    quantile_regressor_support = True
+    from sklearn.cluster import BisectingKMeans
+    bisecting_kmeans_support = True
 except BaseException:
     pass
 
+hdbscan_support = False
+try:
+    from sklearn.cluster import HDBSCAN
+    hdbscan_support = True
+except BaseException:
+    pass
+
+
+hist_gradient_boosting_support = False
+try:
+    from sklearn.ensemble import HistGradientBoostingRegressor
+    from sklearn.ensemble import HistGradientBoostingClassifier
+    hist_gradient_boosting_support = True
+except BaseException:
+    pass
+
+
+PYMILO_VERSION = "0.8"
+NOT_SUPPORTED = "NOT_SUPPORTED"
+PYMILO_VERSION_DOES_NOT_EXIST = "Corrupted JSON file, `pymilo_version` doesn't exist in this file."
+UNEQUAL_PYMILO_VERSIONS = "warning: Installed PyMilo version differes from the PyMilo version used to create the JSON file."
+UNEQUAL_SKLEARN_VERSIONS = "warning: Installed Scikit version differes from the Scikit version used to create the JSON file and it may prevent PyMilo from transporting seamlessly."
 
 SKLEARN_LINEAR_MODEL_TABLE = {
-    "LinearRegression": LinearRegression,
-    "Ridge": Ridge,
-    "RidgeCV": RidgeCV,
-    "RidgeClassifier": RidgeClassifier,
-    "RidgeClassifierCV": RidgeClassifierCV,
-    "Lasso": Lasso,
-    "LassoCV": LassoCV,
-    "LassoLars": LassoLars,
-    "LassoLarsCV": LassoLarsCV,
-    "LassoLarsIC": LassoLarsIC,
-    "MultiTaskLasso": MultiTaskLasso,
-    "MultiTaskLassoCV": MultiTaskLassoCV,
-    "ElasticNet": ElasticNet,
-    "ElasticNetCV": ElasticNetCV,
-    "MultiTaskElasticNet": MultiTaskElasticNet,
-    "MultiTaskElasticNetCV": MultiTaskElasticNetCV,
-    "OrthogonalMatchingPursuit": OrthogonalMatchingPursuit,
-    "OrthogonalMatchingPursuitCV": OrthogonalMatchingPursuitCV,
-    "BayesianRidge": BayesianRidge,
-    "ARDRegression": ARDRegression,
-    "LogisticRegression": LogisticRegression,
-    "LogisticRegressionCV": LogisticRegressionCV,
+    "DummyRegressor": dummy.DummyRegressor,
+    "DummyClassifier": dummy.DummyClassifier,
+    "LinearRegression": linear_model.LinearRegression,
+    "Ridge": linear_model.Ridge,
+    "RidgeCV": linear_model.RidgeCV,
+    "RidgeClassifier": linear_model.RidgeClassifier,
+    "RidgeClassifierCV": linear_model.RidgeClassifierCV,
+    "Lasso": linear_model.Lasso,
+    "LassoCV": linear_model.LassoCV,
+    "LassoLars": linear_model.LassoLars,
+    "LassoLarsCV": linear_model.LassoLarsCV,
+    "LassoLarsIC": linear_model.LassoLarsIC,
+    "MultiTaskLasso": linear_model.MultiTaskLasso,
+    "MultiTaskLassoCV": linear_model.MultiTaskLassoCV,
+    "ElasticNet": linear_model.ElasticNet,
+    "ElasticNetCV": linear_model.ElasticNetCV,
+    "MultiTaskElasticNet": linear_model.MultiTaskElasticNet,
+    "MultiTaskElasticNetCV": linear_model.MultiTaskElasticNetCV,
+    "OrthogonalMatchingPursuit": linear_model.OrthogonalMatchingPursuit,
+    "OrthogonalMatchingPursuitCV": linear_model.OrthogonalMatchingPursuitCV,
+    "BayesianRidge": linear_model.BayesianRidge,
+    "ARDRegression": linear_model.ARDRegression,
+    "LogisticRegression": linear_model.LogisticRegression,
+    "LogisticRegressionCV": linear_model.LogisticRegressionCV,
     "TweedieRegressor": TweedieRegressor if glm_support['TweedieRegressor'] else NOT_SUPPORTED,
     "PoissonRegressor": PoissonRegressor if glm_support['PoissonRegressor'] else NOT_SUPPORTED,
     "GammaRegressor": GammaRegressor if glm_support['GammaRegressor'] else NOT_SUPPORTED,
-    "SGDRegressor": SGDRegressor,
-    "SGDClassifier": SGDClassifier,
+    "SGDRegressor": linear_model.SGDRegressor,
+    "SGDClassifier": linear_model.SGDClassifier,
     "SGDOneClassSVM": SGDOneClassSVM if sgd_one_class_svm_support else NOT_SUPPORTED,
-    "Perceptron": Perceptron,
-    "PassiveAggressiveRegressor": PassiveAggressiveRegressor,
-    "PassiveAggressiveClassifier": PassiveAggressiveClassifier,
-    "RANSACRegressor": RANSACRegressor,
-    "TheilSenRegressor": TheilSenRegressor,
-    "HuberRegressor": HuberRegressor,
+    "Perceptron": linear_model.Perceptron,
+    "PassiveAggressiveRegressor": linear_model.PassiveAggressiveRegressor,
+    "PassiveAggressiveClassifier": linear_model.PassiveAggressiveClassifier,
+    "RANSACRegressor": linear_model.RANSACRegressor,
+    "TheilSenRegressor": linear_model.TheilSenRegressor,
+    "HuberRegressor": linear_model.HuberRegressor,
     "QuantileRegressor": QuantileRegressor if quantile_regressor_support else NOT_SUPPORTED,
 }
 
 SKLEARN_NEURAL_NETWORK_TABLE = {
-    "MLPRegressor": MLPRegressor,
-    "MLPClassifier": MLPClassifier,
-    "BernoulliRBM": BernoulliRBM,
+    "MLPRegressor": neural_network.MLPRegressor,
+    "MLPClassifier": neural_network.MLPClassifier,
+    "BernoulliRBM": neural_network.BernoulliRBM,
 }
 
 SKLEARN_DECISION_TREE_TABLE = {
-    "DecisionTreeRegressor": DecisionTreeRegressor,
-    "DecisionTreeClassifier": DecisionTreeClassifier,
-    "ExtraTreeRegressor": ExtraTreeRegressor,
-    "ExtraTreeClassifier": ExtraTreeClassifier
+    "DecisionTreeRegressor": tree.DecisionTreeRegressor,
+    "DecisionTreeClassifier": tree.DecisionTreeClassifier,
+    "ExtraTreeRegressor": tree.ExtraTreeRegressor,
+    "ExtraTreeClassifier": tree.ExtraTreeClassifier
 }
 
 SKLEARN_CLUSTERING_TABLE = {
-    "KMeans": KMeans,
-    "MiniBatchKMeans": MiniBatchKMeans,
+    "KMeans": cluster.KMeans,
+    "MiniBatchKMeans": cluster.MiniBatchKMeans,
     "BisectingKMeans": BisectingKMeans if bisecting_kmeans_support else NOT_SUPPORTED,
-    "AffinityPropagation": AffinityPropagation,
-    "MeanShift": MeanShift,
-    "SpectralClustering": SpectralClustering,
-    "SpectralBiclustering": SpectralBiclustering,
-    "SpectralCoclustering": SpectralCoclustering,
-    "AgglomerativeClustering": AgglomerativeClustering,
-    "FeatureAgglomeration": FeatureAgglomeration,
-    "DBSCAN": DBSCAN,
+    "AffinityPropagation": cluster.AffinityPropagation,
+    "MeanShift": cluster.MeanShift,
+    "SpectralClustering": cluster.SpectralClustering,
+    "SpectralBiclustering": cluster.SpectralBiclustering,
+    "SpectralCoclustering": cluster.SpectralCoclustering,
+    "AgglomerativeClustering": cluster.AgglomerativeClustering,
+    "FeatureAgglomeration": cluster.FeatureAgglomeration,
+    "DBSCAN": cluster.DBSCAN,
     "HDBSCAN": HDBSCAN if hdbscan_support else NOT_SUPPORTED,
-    "OPTICS": OPTICS,
-    "Birch": Birch,
-    "GaussianMixture": GaussianMixture,
-    "BayesianGaussianMixture": BayesianGaussianMixture,
+    "OPTICS": cluster.OPTICS,
+    "Birch": cluster.Birch,
+    "GaussianMixture": mixture.GaussianMixture,
+    "BayesianGaussianMixture": mixture.BayesianGaussianMixture,
 }
 
 SKLEARN_NAIVE_BAYES_TABLE = {
-    "GaussianNB": GaussianNB,
-    "MultinomialNB": MultinomialNB,
-    "ComplementNB": ComplementNB,
-    "BernoulliNB": BernoulliNB,
-    "CategoricalNB": CategoricalNB,
+    "GaussianNB": naive_bayes.GaussianNB,
+    "MultinomialNB": naive_bayes.MultinomialNB,
+    "ComplementNB": naive_bayes.ComplementNB,
+    "BernoulliNB": naive_bayes.BernoulliNB,
+    "CategoricalNB": naive_bayes.CategoricalNB,
 }
 
 SKLEARN_SVM_TABLE = {
-    "LinearSVC": LinearSVC,
-    "LinearSVR": LinearSVR,
-    "NuSVC": NuSVC,
-    "NuSVR": NuSVR,
-    "OneClassSVM": OneClassSVM,
-    "SVC": SVC,
-    "SVR": SVR,
+    "LinearSVC": svm.LinearSVC,
+    "LinearSVR": svm.LinearSVR,
+    "NuSVC": svm.NuSVC,
+    "NuSVR": svm.NuSVR,
+    "OneClassSVM": svm.OneClassSVM,
+    "SVC": svm.SVC,
+    "SVR": svm.SVR,
 }
 
 SKLEARN_NEIGHBORS_TABLE = {
-    "KNeighborsRegressor": KNeighborsRegressor,
-    "KNeighborsClassifier": KNeighborsClassifier,
-    "RadiusNeighborsRegressor": RadiusNeighborsRegressor,
-    "RadiusNeighborsClassifier": RadiusNeighborsClassifier,
-    "NearestNeighbors": NearestNeighbors,
-    "NearestCentroid": NearestCentroid,
-    "LocalOutlierFactor": LocalOutlierFactor,
+    "KNeighborsRegressor": neighbors.KNeighborsRegressor,
+    "KNeighborsClassifier": neighbors.KNeighborsClassifier,
+    "RadiusNeighborsRegressor": neighbors.RadiusNeighborsRegressor,
+    "RadiusNeighborsClassifier": neighbors.RadiusNeighborsClassifier,
+    "NearestNeighbors": neighbors.NearestNeighbors,
+    "NearestCentroid": neighbors.NearestCentroid,
+    "LocalOutlierFactor": neighbors.LocalOutlierFactor,
+}
+
+SKLEARN_ENSEMBLE_TABLE = {
+    "AdaBoostRegressor": ensemble.AdaBoostRegressor,
+    "AdaBoostClassifier": ensemble.AdaBoostClassifier,
+    "BaggingRegressor": ensemble.BaggingRegressor,
+    "BaggingClassifier": ensemble.BaggingClassifier,
+    "ExtraTreesClassifier": ensemble.ExtraTreesClassifier,
+    "ExtraTreesRegressor": ensemble.ExtraTreesRegressor,
+    "GradientBoostingRegressor": ensemble.GradientBoostingRegressor,
+    "GradientBoostingClassifier": ensemble.GradientBoostingClassifier,
+    "IsolationForest": ensemble.IsolationForest,
+    "RandomForestClassifier": ensemble.RandomForestClassifier,
+    "RandomForestRegressor": ensemble.RandomForestRegressor,
+    "RandomTreesEmbedding": ensemble.RandomTreesEmbedding,
+    "StackingRegressor": ensemble.StackingRegressor,
+    "StackingClassifier": ensemble.StackingClassifier,
+    "VotingRegressor": ensemble.VotingRegressor,
+    "VotingClassifier": ensemble.VotingClassifier,
+    "HistGradientBoostingRegressor": HistGradientBoostingRegressor if hist_gradient_boosting_support else NOT_SUPPORTED,
+    "HistGradientBoostingClassifier": HistGradientBoostingClassifier if hist_gradient_boosting_support else NOT_SUPPORTED,
+    ####
+    "Pipeline": pipeline.Pipeline,
+}
+
+SKLEARN_PREPROCESSING_TABLE = {
+    "StandardScaler": preprocessing.StandardScaler,
+    "OneHotEncoder": preprocessing.OneHotEncoder,
+    "LabelBinarizer": preprocessing.LabelBinarizer,
+    "LabelEncoder": preprocessing.LabelEncoder,
 }
 
 KEYS_NEED_PREPROCESSING_BEFORE_DESERIALIZATION = {
-    "_label_binarizer": LabelBinarizer,  # in Ridge Classifier
-    "active_": int32,  # in Lasso Lars
-    "n_nonzero_coefs_": int64,  # in OMP-CV
+    "_label_binarizer": preprocessing.LabelBinarizer,  # in Ridge Classifier
+    "active_": np.int32,  # in Lasso Lars
+    "n_nonzero_coefs_": np.int64,  # in OMP-CV
     "scores_": dict,  # in Logistic Regression CV,
     "_base_loss": {},  # BaseLoss in Logistic Regression,
     "loss_function_": {},  # LossFunction in SGD Classifier,
     "estimator_": {},  # LinearRegression model inside RANSAC
 }
 
 NUMPY_TYPE_DICT = {
-    "numpy.intc": intc,
-    "numpy.int32": int32,
-    "numpy.int64": int64,
-    "numpy.float64": float64,
-    "numpy.infinity": lambda _: inf,
-    "numpy.uint8": uint8,
+    "numpy.intc": np.intc,
+    "numpy.int32": np.int32,
+    "numpy.int64": np.int64,
+    "numpy.float64": np.float64,
+    "numpy.infinity": lambda _: np.inf,
+    "numpy.uint8": np.uint8,
+    "numpy.uint64": np.uint64,
+    "numpy.dtype": np.dtype,
 }
 
 EXPORTED_MODELS_PATH = {
     "LINEAR_MODEL": "exported_linear_models",
     "NEURAL_NETWORK": "exported_neural_networks",
     "DECISION_TREE": "exported_decision_trees",
     "CLUSTERING": "exported_clusterings",
     "NAIVE_BAYES": "exported_naive_bayes",
     "SVM": "exported_svms",
-    "NEIGHBORS": "exported_neighbors"
+    "NEIGHBORS": "exported_neighbors",
+    "ENSEMBLE": "exported_ensembles",
 }
```

### Comparing `pymilo-0.7/pymilo/transporters/adamoptimizer_transporter.py` & `pymilo-0.8/pymilo/transporters/adamoptimizer_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.7/pymilo/transporters/baseloss_transporter.py` & `pymilo-0.8/pymilo/transporters/baseloss_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.7/pymilo/transporters/bisecting_tree_transporter.py` & `pymilo-0.8/pymilo/transporters/bisecting_tree_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.7/pymilo/transporters/cfnode_transporter.py` & `pymilo-0.8/pymilo/transporters/cfnode_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.7/pymilo/transporters/function_transporter.py` & `pymilo-0.8/pymilo/transporters/function_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.7/pymilo/transporters/general_data_structure_transporter.py` & `pymilo-0.8/pymilo/transporters/general_data_structure_transporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,31 +89,44 @@
         :type data: dict
         :param key: the special key of the data param, which we're going to serialize its value(data[key])
         :type key: object
         :param model_type: the model type of the ML model, which its data dictionary is given as the data param.
         :type model_type: str
         :return: pymilo serialized output of data[key]
         """
+        if isinstance(data[key], type):
+            raw_type = str(data[key])
+            raw_type = "numpy" + str(raw_type).split("numpy")[-1][:-2]
+            if raw_type in NUMPY_TYPE_DICT.keys():
+                data[key] = {
+                    "np-type": "numpy.dtype",
+                    "value": raw_type
+                }
         # 1. Handling numpy infinity, ransac
-        if isinstance(data[key], type(np.inf)):
+        elif isinstance(data[key], np.float64):
             if np.inf == data[key]:
                 data[key] = {
                     "np-type": "numpy.infinity",
                     "value": "infinite"  # added for compatibility
                 }
+            else:
+                data[key] = {"value": data[key], "np-type": "numpy.float64"}
 
         elif isinstance(data[key], np.intc):
             data[key] = {"value": int(data[key]), "np-type": "numpy.intc"}
 
         elif isinstance(data[key], np.int32):
             data[key] = {"value": int(data[key]), "np-type": "numpy.int32"}
 
         elif isinstance(data[key], np.int64):
             data[key] = {"value": int(data[key]), "np-type": "numpy.int64"}
 
+        elif isinstance(data[key], np.uint64):
+            data[key] = {"value": int(data[key]), "np-type": "numpy.uint64"}
+
         elif isinstance(data[key], list):
             new_list = []
             for item in data[key]:
                 if isinstance(item, np.int32):
                     new_list.append(
                         {"value": int(item), "np-type": "numpy.int32"})
                 elif isinstance(item, np.int64):
@@ -199,14 +212,17 @@
 
         if not isinstance(content, dict):
             return content
 
         if self.is_deserialized_ndarray(content):
             return self.deep_deserialize_ndarray(content)
 
+        if check_str_in_iterable("np-type", content) and check_str_in_iterable("value", content):
+            return self.get_deserialized_regular_primary_types(content)
+
         for key in content:
 
             if isinstance(content[key], dict):
                 content[key] = self.get_deserialized_dict(content[key])
 
             elif isinstance(content[key], list):
                 new_list = []
@@ -218,14 +234,15 @@
                 content[key] = new_list
 
             if check_str_in_iterable(
                     "np-type", content[key]):
                 new_key = NUMPY_TYPE_DICT[content[key]["np-type"]](key)
                 new_value = content[key]["key-value"]
                 black_list_key_values.append([key, new_key, new_value])
+
         for black_key_value in black_list_key_values:
             prev_key, new_key, new_value = black_key_value
             del content[prev_key]
             content[new_key] = new_value
 
         return content
 
@@ -258,29 +275,29 @@
             3. handling np.infinity type
 
         :param content: given item needed to get back to its original form
         :type content: object
         :return: the associated np.int32|np.int64|np.inf
         """
         if "np-type" in content:
+            if content["np-type"] == "numpy.dtype":
+                return NUMPY_TYPE_DICT[content["np-type"]](NUMPY_TYPE_DICT[content['value']])
             return NUMPY_TYPE_DICT[content["np-type"]](content['value'])
 
     def is_numpy_primary_type(self, content):
         """
         Check whether the given object is a numpy primary type.
 
         :type content: given object to get checked whether it is a numpy primary type or not
         :return: boolean representing whether the associated content is a numpy primary type or not
         """
         if is_primitive(content):
             return False
         current_supported_primary_types = NUMPY_TYPE_DICT.values()
-        if not is_iterable(content):
-            return False
-        if "np-type" in content and content["np-type"] in current_supported_primary_types:
+        if check_str_in_iterable("np-type", content) and content["np-type"] in current_supported_primary_types:
             return True
         else:
             return False
 
     def ndarray_to_list(self, ndarray_item):
         """
         Convert the given ndarray to its fully listed format.
@@ -348,16 +365,15 @@
         :param primitive: given primitive needed to get deserialized to it's pure primitive form
         :type primitive: pure python primitive or dict
         :return: pure python primitive or numpy primitive data type
         """
         if is_primitive(primitive):
             return primitive
         elif check_str_in_iterable("np-type", primitive):
-            return NUMPY_TYPE_DICT[primitive["np-type"]
-                                   ](primitive['value'])
+            return self.get_deserialized_regular_primary_types(primitive)
         else:
             return primitive
 
     def deep_serialize_ndarray(self, ndarray):
         """
         Serialize the given ndarray.
 
@@ -377,14 +393,15 @@
                 new_list.append(self.deep_serialize_ndarray(item))
             else:
                 new_list.append(item)
 
         return {
             'pymiloed-ndarray-list': new_list,
             'pymiloed-ndarray-dtype': str(dtype),
+            'pymiloed-ndarray-shape': ndarray.shape,
             'pymiloed-data-structure': 'numpy.ndarray'
         }
 
     def is_deserialized_ndarray(self, deserialized_ndarray):
         """
         Check whether the given input is a previously pymilo-deserialized ndarray.
 
@@ -410,19 +427,27 @@
         :return: numpy.ndarray
         """
         if not self.is_deserialized_ndarray(deserialized_ndarray):
             return None  # throw error
 
         inner_list = deserialized_ndarray['pymiloed-ndarray-list']
         dtype = deserialized_ndarray['pymiloed-ndarray-dtype']
+        shape = deserialized_ndarray['pymiloed-ndarray-shape']
 
         if dtype.startswith("["):
             dtype = literal_eval(dtype)
 
         new_list = []
         for item in inner_list:
             if self.is_deserialized_ndarray(item):
                 new_list.append(self.deep_deserialize_ndarray(item))
             else:
-                new_list.append(item)
-
-        return np.asarray(new_list, dtype=dtype)
+                if len(shape) == 1:
+                    # shape in form if [int] so inner items should not be list.
+                    # convert each inner item to tuple(if it a list)
+                    if isinstance(item, list):
+                        new_list.append(tuple(item))
+                    else:
+                        new_list.append(item)
+                else:
+                    new_list.append(item)
+        return np.asarray(new_list, dtype=dtype).reshape(shape)
```

### Comparing `pymilo-0.7/pymilo/transporters/labelbinarizer_transporter.py` & `pymilo-0.8/pymilo/transporters/generator_transporter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,82 +1,65 @@
 # -*- coding: utf-8 -*-
-"""PyMilo LabelBinarizer transporter."""
-from ..pymilo_param import KEYS_NEED_PREPROCESSING_BEFORE_DESERIALIZATION
-from sklearn import preprocessing
-import numpy as np
+"""PyMilo Generator transporter."""
+from numpy.random._generator import Generator
+from ..utils.util import is_primitive, check_str_in_iterable
 from .transporter import AbstractTransporter
-from .general_data_structure_transporter import GeneralDataStructureTransporter
+from numpy.random import default_rng
 
 
-class LabelBinarizerTransporter(AbstractTransporter):
-    """Customized PyMilo Transporter developed to handle LabelBinarizer field(for Ridge Classifier(+[CV]))."""
+class GeneratorTransporter(AbstractTransporter):
+    """Customized PyMilo Transporter developed to handle Generator objects."""
 
     def serialize(self, data, key, model_type):
         """
-        Serialize the LabelBinarizer field(if there is).
+        Serialize Generator object.
 
         serialize the data[key] of the given model which type is model_type.
         basically in order to fully serialize a model, we should traverse over all the keys of its data dictionary and
         pass it through the chain of associated transporters to get fully serialized.
 
         :param data: the internal data dictionary of the given model
         :type data: dict
         :param key: the special key of the data param, which we're going to serialize its value(data[key])
         :type key: object
         :param model_type: the model type of the ML model, which data dictionary is given as the data param
         :type model_type: str
         :return: pymilo serialized output of data[key]
         """
-        if isinstance(data[key], preprocessing.LabelBinarizer):
-            data[key] = self.get_serialized_label_binarizer(data[key])
+        if isinstance(data[key], Generator):
+            generator = data[key]
+            data[key] = {
+                "pymilo-bypass": True,
+                "pymilo-generator": {
+                    "state": generator.__getstate__()
+                }
+            }
         return data[key]
 
-    def get_serialized_label_binarizer(self, label_binarizer):
-        """
-        Serialize a LabelBinarizer object.
-
-        :param label_binarizer: a label_binarizer object
-        :type label_binarizer: sklearn.preprocessing.LabelBinarizer
-        :return: pymilo serialized output of label_binarizer object
-        """
-        data = label_binarizer.__dict__
-        for key in data:
-            if isinstance(data[key], np.ndarray):
-                data[key] = GeneralDataStructureTransporter().deep_serialize_ndarray(data[key])
-        return data
-
     def deserialize(self, data, key, model_type):
         """
-        Deserialize the LabelBinarizer field(if there is).
+        Deserialize previously pymilo serialized Generator object.
 
         deserialize the data[key] of the given model which type is model_type.
         basically in order to fully deserialize a model, we should traverse over all the keys of its serialized data dictionary and
         pass it through the chain of associated transporters to get fully deserialized.
 
-        :param data: the internal data dictionary of the associated json file
-            of the ML model which is generated previously by pymilo export.
+        :param data: the internal data dictionary of the associated json file of the ML model which is generated previously by
+        pymilo export.
         :type data: dict
         :param key: the special key of the data param, which we're going to deserialize its value(data[key])
         :type key: object
         :param model_type: the model type of the ML model, which internal serialized data dictionary is given as the data param
         :type model_type: str
         :return: pymilo deserialized output of data[key]
         """
         content = data[key]
-        if key != "_label_binarizer":
+        if is_primitive(content) or content is None:
             return content
-        return self.get_deserialized_label_binarizer(content)
 
-    def get_deserialized_label_binarizer(self, content):
-        """
-        Deserialize the pymilo serialized labelBinarizer field of the associated ML model.
+        if check_str_in_iterable("pymilo-generator", content):
+            serialized_generator = content["pymilo-generator"]
+            generator = default_rng(0)
+            generator.__setstate__(serialized_generator["state"])
+            return generator
 
-        :param content: a label_binarizer object
-        :type content: sklearn.preprocessing.LabelBinarizer
-        :return: a sklearn.preprocessing.LabelBinarizer instance derived from the
-        pymilo deserialized output of the previously pymilo serialized label_binarizer field.
-        """
-        raw_lb = KEYS_NEED_PREPROCESSING_BEFORE_DESERIALIZATION["_label_binarizer"](
-        )
-        for item in content:
-            setattr(raw_lb, item, content[item])
-        return raw_lb
+        return content
```

### Comparing `pymilo-0.7/pymilo/transporters/neighbors_tree_transporter.py` & `pymilo-0.8/pymilo/transporters/neighbors_tree_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.7/pymilo/transporters/randomstate_transporter.py` & `pymilo-0.8/pymilo/transporters/randomstate_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.7/pymilo/transporters/sgdoptimizer_transporter.py` & `pymilo-0.8/pymilo/transporters/sgdoptimizer_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.7/pymilo/transporters/transporter.py` & `pymilo-0.8/pymilo/transporters/transporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,30 +102,32 @@
         :param content: either a ML model object's internal data dictionary or an object associated with the json string of a pymilo serialized ML model.
         :type content: object
         :return: boolean, whether to bypass or not
         """
         if is_primitive(content):
             return False
 
-        if check_str_in_iterable("by-pass", content):
-            return content["by-pass"]
+        if check_str_in_iterable("pymilo-bypass", content):
+            return content["pymilo-bypass"]
         else:
             return False
 
     def transport(self, request, command, is_inner_model=False):
         """
         Either serializes or deserializes the request according to the given command.
 
         basically in order to fully transport a request, we should traverse over all the keys of its internal data dictionary and
         pass it through the chain of associated transporters to get fully transported.
 
         :param request: either a ML model object itself(when command is serialize) or an object associated with the json string of a pymilo serialized ML model(when command is deserialize)
         :type request: object
         :param command: determines the type of transportation, it can be either Serialize or Deserialize
         :type command: Command class
+        :param is_inner_model: determines whether it is an inner linear model of a super ml model
+        :type is_inner_model: boolean
         :return: pymilo transported output of data[key]
         """
         if command == Command.SERIALIZE:
             # request is a sklearn model
             data = request.__dict__
             for key in data:
                 if self.bypass(data[key]):
```

### Comparing `pymilo-0.7/pymilo/transporters/tree_transporter.py` & `pymilo-0.8/pymilo/transporters/tree_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.7/pymilo/utils/data_exporter.py` & `pymilo-0.8/pymilo/utils/data_exporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.7/pymilo/utils/test_pymilo.py` & `pymilo-0.8/pymilo/utils/test_pymilo.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,56 +2,30 @@
 """pymilo test modules."""
 import os
 import copy
 from numpy import array_equal
 
 from ..pymilo_obj import Export
 from ..pymilo_obj import Import
+from ..pymilo_func import get_transporter, compare_model_outputs
+from ..pymilo_param import EXPORTED_MODELS_PATH
 
 from sklearn.metrics import mean_squared_error, r2_score
 from sklearn.metrics import accuracy_score, hinge_loss
 
-from ..pymilo_func import compare_model_outputs
-
-from ..chains.linear_model_chain import is_linear_model
-from ..chains.neural_network_chain import is_neural_network
-from ..chains.decision_tree_chain import is_decision_tree
-from ..chains.clustering_chain import is_clusterer
-from ..chains.naive_bayes_chain import is_naive_bayes
-from ..chains.svm_chain import is_svm
-from ..chains.neighbours_chain import is_neighbors
-
-from ..pymilo_param import EXPORTED_MODELS_PATH
-
 
 def pymilo_export_path(model):
     """
     Return the associated folder name to save the json file generated by pymilo Export(applied to the given model).
 
     :param model: given model
     :type model: any sklearn's model class
     :return: folder name
     """
-    model_type = None
-    if is_linear_model(model):
-        model_type = "LINEAR_MODEL"
-    elif is_neural_network(model):
-        model_type = "NEURAL_NETWORK"
-    elif is_decision_tree(model):
-        model_type = "DECISION_TREE"
-    elif is_clusterer(model):
-        model_type = "CLUSTERING"
-    elif is_naive_bayes(model):
-        model_type = "NAIVE_BAYES"
-    elif is_svm(model):
-        model_type = "SVM"
-    elif is_neighbors(model):
-        model_type = "NEIGHBORS"
-    else:
-        model_type = None
+    model_type, _ = get_transporter(model)
     return EXPORTED_MODELS_PATH[model_type]
 
 
 def pymilo_test(model, model_name):
     """
     Return the pymilo imported model's outputs for given test_data.
```

### Comparing `pymilo-0.7/pymilo/utils/util.py` & `pymilo-0.8/pymilo/utils/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     """
     Check if the given object is primitive.
 
     :param obj: given object
     :type obj: any valid type
     :return: True if object is primitive
     """
+    if isinstance(obj, dict):
+        return False
     return not hasattr(obj, '__dict__')
 
 
 def is_iterable(obj):
     """
     Check if the given object is iterable.
```

### Comparing `pymilo-0.7/pymilo.egg-info/PKG-INFO` & `pymilo-0.8/pymilo.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymilo
-Version: 0.7
+Version: 0.8
 Summary: Transportation of ML models
 Home-page: https://github.com/openscilab/pymilo
-Download-URL: https://github.com/openscilab/pymilo/tarball/v0.7
+Download-URL: https://github.com/openscilab/pymilo/tarball/v0.8
 Author: PyMilo Development Team
 Author-email: pymilo@openscilab.com
 License: MIT
 Project-URL: Source, https://github.com/openscilab/pymilo
 Keywords: python3 python machine_learning ML
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -41,44 +41,22 @@
 Requires-Dist: scikit-learn>=0.22.2
 
 
 <div align="center">
     <img src="https://github.com/openscilab/pymilo/raw/main/otherfiles/logo.png" width="500" height="300">
     <br/>
     <br/>
-    <a href="https://codecov.io/gh/openscilab/pymilo">
-        <img src="https://codecov.io/gh/openscilab/pymilo/branch/main/graph/badge.svg" alt="Codecov"/>
-    </a>
-    <a href="https://badge.fury.io/py/pymilo">
-        <img src="https://badge.fury.io/py/pymilo.svg" alt="PyPI version" height="18">
-    </a>
-    <a href="https://www.python.org/">
-        <img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3">
-    </a>
-    <a href="https://discord.gg/mtuMS8AjDS">
-        <img src="https://img.shields.io/discord/1064533716615049236.svg" alt="Discord Channel">
-    </a>
+    <a href="https://codecov.io/gh/openscilab/pymilo"><img src="https://codecov.io/gh/openscilab/pymilo/branch/main/graph/badge.svg" alt="Codecov"/></a>
+    <a href="https://badge.fury.io/py/pymilo"><img src="https://badge.fury.io/py/pymilo.svg" alt="PyPI version" height="18"></a>
+    <a href="https://www.python.org/"><img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3"></a>
+    <a href="https://discord.gg/mtuMS8AjDS"><img src="https://img.shields.io/discord/1064533716615049236.svg" alt="Discord Channel"></a>
 </div>
 
 ----------
 
-## Table of contents
-
-* [Overview](https://github.com/openscilab/pymilo#overview)
-* [Installation](https://github.com/openscilab/pymilo#installation)
-* [Usage](https://github.com/openscilab/pymilo#usage)
-* [Issues & Bug Reports](https://github.com/openscilab/pymilo#issues--bug-reports)
-* [Contribution](https://github.com/openscilab/pymilo/blob/main/.github/CONTRIBUTING.md)
-* [Authors](https://github.com/openscilab/pymilo/blob/main/AUTHORS.md)
-* [License](https://github.com/openscilab/pymilo/blob/main/LICENSE)
-* [Show Your Support](https://github.com/openscilab/pymilo#show-your-support)
-* [Changelog](https://github.com/openscilab/pymilo/blob/main/CHANGELOG.md)
-* [Code of Conduct](https://github.com/openscilab/pymilo/blob/main/.github/CODE_OF_CONDUCT.md)
-
-
 ## Overview
 <p align="justify">
 PyMilo is an open source Python package that provides a simple, efficient, and safe way for users to export pre-trained machine learning models in a transparent way. By this, the exported model can be used in other environments, transferred across different platforms, and shared with others. PyMilo allows the users to export the models that are trained using popular Python libraries like scikit-learn, and then use them in deployment environments, or share them without exposing the underlying code or dependencies. The transparency of the exported models ensures reliability and safety for the end users, as it eliminates the risks of binary or pickle formats.
 </p>
 <table>
     <tr>
         <td align="center">PyPI Counter</td>
@@ -125,17 +103,17 @@
 
 
 ## Installation
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)
-- Run `pip install pymilo==0.7`
+- Run `pip install pymilo==0.8`
 ### Source code
-- Download [Version 0.7](https://github.com/openscilab/pymilo/archive/v0.7.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
+- Download [Version 0.8](https://github.com/openscilab/pymilo/archive/v0.8.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
 - Run `pip install .`
 
 ## Usage
 ### Model preparation 
 ```pycon
 >>> from sklearn import datasets
 >>> from pymilo import Export, Import
@@ -161,27 +139,30 @@
 >>> #### Import the pymilo-exported model and get a real scikit model
 >>> imported_model = Import(PATH_TO_JSON_FILE)
 ```
 ### Get the associated model
 ```pycon 
 >>> imported_sklearn_model = imported_model.to_model()
 ```
-#### Note: `imported_sklearn_model` has the **exact same** functionality as the `model` object earlier.
+* Note: `imported_sklearn_model` has the **exact same** functionality as the `model` object earlier.
 
 ## Supported ML models
 | scikit-learn | PyTorch | 
 | ---------------- | ---------------- | 
 | Linear Models &#x2705; | - | 
 | Neural networks &#x2705; | -  | 
 | Trees &#x2705; | -  | 
 | Clustering &#x2705; | -  | 
 | Naïve Bayes &#x2705; | -  | 
 | Support vector machines (SVMs) &#x2705; | -  | 
-| Nearest Neighbors &#x2705; | -  | 
-| Ensemble Models &#x274C; | - | 
+| Nearest Neighbors &#x2705; | -  |  
+| Ensemble Models &#x2705; | - | 
+| Pipeline Model &#x2705; | - |
+| Preprocessing Models ⏳ | - |
+
 Details are available in [Supported Models](https://github.com/openscilab/pymilo/blob/main/SUPPORTED_MODELS.md).
 
 ## Issues & bug reports
 
 Just fill an issue and describe it. We'll check it ASAP! or send an email to [pymilo@openscilab.com](mailto:pymilo@openscilab.com "pymilo@openscilab.com"). 
 
 - Please complete the issue template
@@ -209,14 +190,70 @@
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 ### Added
 ### Changed
+## [0.8] - 2024-05-06
+### Added
+- `StandardScaler` Transformer in `pymilo_param.py`
+- `PreprocessingTransporter` Transporter
+- ndarray shape config in `GeneralDataStructure` Transporter
+- `util.py` in chains
+- `BinMapperTransporter` Transporter
+- `BunchTransporter` Transporter
+- `GeneratorTransporter` Transporter
+- `TreePredictorTransporter` Transporter
+- `AdaboostClassifier` model
+- `AdaboostRegressor` model
+- `BaggingClassifier` model
+- `BaggingRegressor` model
+- `ExtraTreesClassifier` model
+- `ExtraTreesRegressor` model
+- `GradientBoosterClassifier` model
+- `GradientBoosterRegressor` model
+- `HistGradientBoosterClassifier` model
+- `HistGradientBoosterRegressor` model
+- `RandomForestClassifier` model
+- `RandomForestRegressor` model
+- `IsolationForest` model
+- `RandomTreesEmbedding` model
+- `StackingClassifier` model
+- `StackingRegressor` model
+- `VotingClassifier` model
+- `VotingRegressor` model
+- `Pipeline` model
+- Ensemble models test runner
+- Ensemble chain
+- `SECURITY.md`
+### Changed
+- `Pipeline` test updated
+- `LabelBinarizer`,`LabelEncoder` and `OneHotEncoder` got embedded in `PreprocessingTransporter`
+- Preprocessing support added to Ensemble chain
+- Preprocessing params initialized in `pymilo_param`
+- `util.py` in utils updated
+- `test_pymilo.py` updated
+- `pymilo_func.py` updated
+- `linear_model_chain.py` updated
+- `neural_network_chain.py` updated
+- `decision_tree_chain.py` updated
+- `clustering_chain.py` updated
+- `naive_bayes_chain.py` updated
+- `neighbours_chain.py` updated
+- `svm_chain.py` updated
+- `GeneralDataStructure` Transporter updated
+- `LossFunction` Transporter updated
+- `AbstractTransporter` updated
+- Tests config modified
+- Unequal sklearn version error added in `pymilo_param.py`
+- Ensemble params initialized in `pymilo_param`
+- Ensemble support added to `pymilo_func.py`
+- `SUPPORTED_MODELS.md` updated
+- `README.md` updated
 ## [0.7] - 2024-04-03
 ### Added
 - `pymilo_nearest_neighbor_test` function added to `test_pymilo.py`
 - `NeighborsTreeTransporter` Transporter
 - `LocalOutlierFactor` model
 - `RadiusNeighborsClassifier` model
 - `RadiusNeighborsRegressor` model
@@ -364,15 +401,16 @@
 - `linear_model_chain` refactored
 ## [0.1] - 2023-06-29
 ### Added
 - scikit-learn linear models support
 - `Export` class
 - `Import` class
 
-[Unreleased]: https://github.com/openscilab/pymilo/compare/v0.7...dev
+[Unreleased]: https://github.com/openscilab/pymilo/compare/v0.8...dev
+[0.8]: https://github.com/openscilab/pymilo/compare/v0.7...v0.8
 [0.7]: https://github.com/openscilab/pymilo/compare/v0.6...v0.7
 [0.6]: https://github.com/openscilab/pymilo/compare/v0.5...v0.6
 [0.5]: https://github.com/openscilab/pymilo/compare/v0.4...v0.5
 [0.4]: https://github.com/openscilab/pymilo/compare/v0.3...v0.4
 [0.3]: https://github.com/openscilab/pymilo/compare/v0.2...v0.3
 [0.2]: https://github.com/openscilab/pymilo/compare/v0.1...v0.2
 [0.1]: https://github.com/openscilab/pymilo/compare/e887108...v0.1
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pymilo Version: 0.7 Summary: Transportation of ML
+Metadata-Version: 2.1 Name: pymilo Version: 0.8 Summary: Transportation of ML
 models Home-page: https://github.com/openscilab/pymilo Download-URL: https://
-github.com/openscilab/pymilo/tarball/v0.7 Author: PyMilo Development Team
+github.com/openscilab/pymilo/tarball/v0.8 Author: PyMilo Development Team
 Author-email: pymilo@openscilab.com License: MIT Project-URL: Source, https://
 github.com/openscilab/pymilo Keywords: python3 python machine_learning ML
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
@@ -21,25 +21,15 @@
 Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
 Engineering :: Physics Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE License-File: AUTHORS.md Requires-Dist:
 numpy>=1.9.0 Requires-Dist: scikit-learn>=0.22.2
       [https://github.com/openscilab/pymilo/raw/main/otherfiles/logo.png]
 
          _[_C_o_d_e_c_o_v_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_b_u_i_l_t_ _w_i_t_h_ _P_y_t_h_o_n_3_]_[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]
----------- ## Table of contents * [Overview](https://github.com/openscilab/
-pymilo#overview) * [Installation](https://github.com/openscilab/
-pymilo#installation) * [Usage](https://github.com/openscilab/pymilo#usage) *
-[Issues & Bug Reports](https://github.com/openscilab/pymilo#issues--bug-
-reports) * [Contribution](https://github.com/openscilab/pymilo/blob/
-main/.github/CONTRIBUTING.md) * [Authors](https://github.com/openscilab/pymilo/
-blob/main/AUTHORS.md) * [License](https://github.com/openscilab/pymilo/blob/
-main/LICENSE) * [Show Your Support](https://github.com/openscilab/pymilo#show-
-your-support) * [Changelog](https://github.com/openscilab/pymilo/blob/main/
-CHANGELOG.md) * [Code of Conduct](https://github.com/openscilab/pymilo/blob/
-main/.github/CODE_OF_CONDUCT.md) ## Overview
+---------- ## Overview
 PyMilo is an open source Python package that provides a simple, efficient, and
 safe way for users to export pre-trained machine learning models in a
 transparent way. By this, the exported model can be used in other environments,
 transferred across different platforms, and shared with others. PyMilo allows
 the users to export the models that are trained using popular Python libraries
 like scikit-learn, and then use them in deployment environments, or share them
 without exposing the underlying code or dependencies. The transparency of the
@@ -52,50 +42,76 @@
         [https://github.com/openscilab/    [https://github.com/openscilab/
    CI  pymilo/actions/workflows/test.yml/ pymilo/actions/workflows/test.yml/
              badge.svg?branch=main]             badge.svg?branch=dev]
                           _[_h_t_t_p_s_:_/_/_a_p_p_._c_o_d_a_c_y_._c_o_m_/_p_r_o_j_e_c_t_/
 Code Quality _[_C_o_d_e_F_a_c_t_o_r_]           _b_a_d_g_e_/_G_r_a_d_e_/            _[_c_o_d_e_b_e_a_t_ _b_a_d_g_e_]
                           _9_e_e_e_c_9_9_e_d_1_1_f_4_d_9_b_8_6_a_f_3_6_d_c_9_0_f_5_f_7_5_3_]
 ## Installation ### PyPI - Check [Python Packaging User Guide](https://
-packaging.python.org/installing/) - Run `pip install pymilo==0.7` ### Source
-code - Download [Version 0.7](https://github.com/openscilab/pymilo/archive/
-v0.7.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
+packaging.python.org/installing/) - Run `pip install pymilo==0.8` ### Source
+code - Download [Version 0.8](https://github.com/openscilab/pymilo/archive/
+v0.8.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
 dev.zip) - Run `pip install .` ## Usage ### Model preparation ```pycon >>> from
 sklearn import datasets >>> from pymilo import Export, Import >>> from
 sklearn.linear_model import LinearRegression >>> import os >>> X, Y =
 datasets.load_diabetes(return_X_y=True) >>> threshold = 20 >>> X_train, X_test
 = X[:-threshold], X[-threshold:] >>> Y_train, Y_test = Y[:-threshold], Y[-
 threshold:] >>> model = LinearRegression() >>> #### Train the model using the
 training sets >>> model.fit(X_train, Y_train) ``` ### Save model ```pycon >>>
 #### Export the fitted model to a transparent json file >>> exported_model =
 Export(model) >>> PATH_TO_JSON_FILE = os.path.join(os.getcwd(),"test.json") >>>
 exported_model.save(PATH_TO_JSON_FILE) ``` ### Load model ```pycon >>> ####
 Import the pymilo-exported model and get a real scikit model >>> imported_model
 = Import(PATH_TO_JSON_FILE) ``` ### Get the associated model ```pycon >>>
-imported_sklearn_model = imported_model.to_model() ``` #### Note:
+imported_sklearn_model = imported_model.to_model() ``` * Note:
 `imported_sklearn_model` has the **exact same** functionality as the `model`
 object earlier. ## Supported ML models | scikit-learn | PyTorch | | -----------
 ----- | ---------------- | | Linear Models ✅ | - | | Neural networks ✅ | - | |
 Trees ✅ | - | | Clustering ✅ | - | | NaÃ¯ve Bayes ✅ | - | | Support vector
-machines (SVMs) ✅ | - | | Nearest Neighbors ✅ | - | | Ensemble Models ❌ | - |
-Details are available in [Supported Models](https://github.com/openscilab/
-pymilo/blob/main/SUPPORTED_MODELS.md). ## Issues & bug reports Just fill an
-issue and describe it. We'll check it ASAP! or send an email to
-[pymilo@openscilab.com](mailto:pymilo@openscilab.com "pymilo@openscilab.com").
-- Please complete the issue template You can also join our discord server
-_[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]## Show your support ### Star this repo Give a â­ï¸ if this
-project helped you! ### Donate to our project If you do like our project and we
-hope that you do, can you please support us? Our project is not and is never
-going to be working for profit. We need the money just so we can continue doing
-what we do ;-) . _[_P_y_M_i_l_o_ _D_o_n_a_t_i_o_n_]# Changelog All notable changes to this
-project will be documented in this file. The format is based on [Keep a
-Changelog](http://keepachangelog.com/en/1.0.0/) and this project adheres to
-[Semantic Versioning](http://semver.org/spec/v2.0.0.html). ## [Unreleased] ###
-Added ### Changed ## [0.7] - 2024-04-03 ### Added -
-`pymilo_nearest_neighbor_test` function added to `test_pymilo.py` -
+machines (SVMs) ✅ | - | | Nearest Neighbors ✅ | - | | Ensemble Models ✅ | - | |
+Pipeline Model ✅ | - | | Preprocessing Models â³ | - | Details are available
+in [Supported Models](https://github.com/openscilab/pymilo/blob/main/
+SUPPORTED_MODELS.md). ## Issues & bug reports Just fill an issue and describe
+it. We'll check it ASAP! or send an email to [pymilo@openscilab.com](mailto:
+pymilo@openscilab.com "pymilo@openscilab.com"). - Please complete the issue
+template You can also join our discord server _[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]## Show your
+support ### Star this repo Give a â­ï¸ if this project helped you! ### Donate
+to our project If you do like our project and we hope that you do, can you
+please support us? Our project is not and is never going to be working for
+profit. We need the money just so we can continue doing what we do ;-) .
+_[_P_y_M_i_l_o_ _D_o_n_a_t_i_o_n_]# Changelog All notable changes to this project will be
+documented in this file. The format is based on [Keep a Changelog](http://
+keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning]
+(http://semver.org/spec/v2.0.0.html). ## [Unreleased] ### Added ### Changed ##
+[0.8] - 2024-05-06 ### Added - `StandardScaler` Transformer in
+`pymilo_param.py` - `PreprocessingTransporter` Transporter - ndarray shape
+config in `GeneralDataStructure` Transporter - `util.py` in chains -
+`BinMapperTransporter` Transporter - `BunchTransporter` Transporter -
+`GeneratorTransporter` Transporter - `TreePredictorTransporter` Transporter -
+`AdaboostClassifier` model - `AdaboostRegressor` model - `BaggingClassifier`
+model - `BaggingRegressor` model - `ExtraTreesClassifier` model -
+`ExtraTreesRegressor` model - `GradientBoosterClassifier` model -
+`GradientBoosterRegressor` model - `HistGradientBoosterClassifier` model -
+`HistGradientBoosterRegressor` model - `RandomForestClassifier` model -
+`RandomForestRegressor` model - `IsolationForest` model -
+`RandomTreesEmbedding` model - `StackingClassifier` model - `StackingRegressor`
+model - `VotingClassifier` model - `VotingRegressor` model - `Pipeline` model -
+Ensemble models test runner - Ensemble chain - `SECURITY.md` ### Changed -
+`Pipeline` test updated - `LabelBinarizer`,`LabelEncoder` and `OneHotEncoder`
+got embedded in `PreprocessingTransporter` - Preprocessing support added to
+Ensemble chain - Preprocessing params initialized in `pymilo_param` - `util.py`
+in utils updated - `test_pymilo.py` updated - `pymilo_func.py` updated -
+`linear_model_chain.py` updated - `neural_network_chain.py` updated -
+`decision_tree_chain.py` updated - `clustering_chain.py` updated -
+`naive_bayes_chain.py` updated - `neighbours_chain.py` updated - `svm_chain.py`
+updated - `GeneralDataStructure` Transporter updated - `LossFunction`
+Transporter updated - `AbstractTransporter` updated - Tests config modified -
+Unequal sklearn version error added in `pymilo_param.py` - Ensemble params
+initialized in `pymilo_param` - Ensemble support added to `pymilo_func.py` -
+`SUPPORTED_MODELS.md` updated - `README.md` updated ## [0.7] - 2024-04-03 ###
+Added - `pymilo_nearest_neighbor_test` function added to `test_pymilo.py` -
 `NeighborsTreeTransporter` Transporter - `LocalOutlierFactor` model -
 `RadiusNeighborsClassifier` model - `RadiusNeighborsRegressor` model -
 `NearestCentroid` model - `NearestNeighbors` model - `KNeighborsClassifier`
 model - `KNeighborsRegressor` model - Neighbors models test runner - Neighbors
 chain ### Changed - Tests config modified - Neighbors params initialized in
 `pymilo_param` - Neighbors support added to `pymilo_func.py` -
 `SUPPORTED_MODELS.md` updated - `README.md` updated ## [0.6] - 2024-03-27 ###
@@ -159,14 +175,14 @@
 - `GeneralDataStructure` Transporter updated - `LabelBinerizer` Transporter
 updated - `linear model` chain updated - GeneralDataStructure transporter
 enhanced - LabelBinerizer transporter updated - transporters' chain router
 added to `pymilo func` - NeuralNetwork params initialized in `pymilo_param` -
 `pymilo_test` updated to support multiple models - `linear_model_chain`
 refactored ## [0.1] - 2023-06-29 ### Added - scikit-learn linear models support
 - `Export` class - `Import` class [Unreleased]: https://github.com/openscilab/
-pymilo/compare/v0.7...dev [0.7]: https://github.com/openscilab/pymilo/compare/
-v0.6...v0.7 [0.6]: https://github.com/openscilab/pymilo/compare/v0.5...v0.6
-[0.5]: https://github.com/openscilab/pymilo/compare/v0.4...v0.5 [0.4]: https://
-github.com/openscilab/pymilo/compare/v0.3...v0.4 [0.3]: https://github.com/
-openscilab/pymilo/compare/v0.2...v0.3 [0.2]: https://github.com/openscilab/
-pymilo/compare/v0.1...v0.2 [0.1]: https://github.com/openscilab/pymilo/compare/
-e887108...v0.1
+pymilo/compare/v0.8...dev [0.8]: https://github.com/openscilab/pymilo/compare/
+v0.7...v0.8 [0.7]: https://github.com/openscilab/pymilo/compare/v0.6...v0.7
+[0.6]: https://github.com/openscilab/pymilo/compare/v0.5...v0.6 [0.5]: https://
+github.com/openscilab/pymilo/compare/v0.4...v0.5 [0.4]: https://github.com/
+openscilab/pymilo/compare/v0.3...v0.4 [0.3]: https://github.com/openscilab/
+pymilo/compare/v0.2...v0.3 [0.2]: https://github.com/openscilab/pymilo/compare/
+v0.1...v0.2 [0.1]: https://github.com/openscilab/pymilo/compare/e887108...v0.1
```

### Comparing `pymilo-0.7/pymilo.egg-info/SOURCES.txt` & `pymilo-0.8/pymilo.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,34 +10,40 @@
 pymilo.egg-info/SOURCES.txt
 pymilo.egg-info/dependency_links.txt
 pymilo.egg-info/requires.txt
 pymilo.egg-info/top_level.txt
 pymilo/chains/__init__.py
 pymilo/chains/clustering_chain.py
 pymilo/chains/decision_tree_chain.py
+pymilo/chains/ensemble_chain.py
 pymilo/chains/linear_model_chain.py
 pymilo/chains/naive_bayes_chain.py
 pymilo/chains/neighbours_chain.py
 pymilo/chains/neural_network_chain.py
 pymilo/chains/svm_chain.py
+pymilo/chains/util.py
 pymilo/exceptions/__init__.py
 pymilo/exceptions/deserialize_exception.py
 pymilo/exceptions/pymilo_exception.py
 pymilo/exceptions/serialize_exception.py
 pymilo/transporters/__init__.py
 pymilo/transporters/adamoptimizer_transporter.py
 pymilo/transporters/baseloss_transporter.py
+pymilo/transporters/binmapper_transporter.py
 pymilo/transporters/bisecting_tree_transporter.py
+pymilo/transporters/bunch_transporter.py
 pymilo/transporters/cfnode_transporter.py
 pymilo/transporters/function_transporter.py
 pymilo/transporters/general_data_structure_transporter.py
-pymilo/transporters/labelbinarizer_transporter.py
+pymilo/transporters/generator_transporter.py
 pymilo/transporters/lossfunction_transporter.py
 pymilo/transporters/neighbors_tree_transporter.py
+pymilo/transporters/preprocessing_transporter.py
 pymilo/transporters/randomstate_transporter.py
 pymilo/transporters/sgdoptimizer_transporter.py
 pymilo/transporters/transporter.py
 pymilo/transporters/tree_transporter.py
+pymilo/transporters/treepredictor_transporter.py
 pymilo/utils/__init__.py
 pymilo/utils/data_exporter.py
 pymilo/utils/test_pymilo.py
 pymilo/utils/util.py
```

### Comparing `pymilo-0.7/setup.py` & `pymilo-0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,22 +30,22 @@
     name='pymilo',
     packages=[
         'pymilo',
         'pymilo.utils',
         'pymilo.chains',
         'pymilo.transporters',
         'pymilo.exceptions'],
-    version='0.7',
+    version='0.8',
     description='Transportation of ML models',
     long_description=read_description(),
     long_description_content_type='text/markdown',
     author='PyMilo Development Team',
     author_email='pymilo@openscilab.com',
     url='https://github.com/openscilab/pymilo',
-    download_url='https://github.com/openscilab/pymilo/tarball/v0.7',
+    download_url='https://github.com/openscilab/pymilo/tarball/v0.8',
     keywords="python3 python machine_learning ML",
     project_urls={
             'Source': 'https://github.com/openscilab/pymilo',
     },
     install_requires=get_requires(),
     python_requires='>=3.6',
     classifiers=[
```

