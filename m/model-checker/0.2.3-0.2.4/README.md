# Comparing `tmp/model_checker-0.2.3.tar.gz` & `tmp/model_checker-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_checker-0.2.3.tar", last modified: Mon May  6 19:26:42 2024, max compression
+gzip compressed data, was "model_checker-0.2.4.tar", last modified: Mon May  6 19:45:49 2024, max compression
```

## Comparing `model_checker-0.2.3.tar` & `model_checker-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 19:26:42.130903 model_checker-0.2.3/
--rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-04-26 19:58:45.000000 model_checker-0.2.3/LICENCE
--rw-r--r--   0 benjamin  (1000) users      (100)      673 2024-05-06 19:26:42.130903 model_checker-0.2.3/PKG-INFO
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 19:26:42.130903 model_checker-0.2.3/model_checker.egg-info/
--rw-r--r--   0 benjamin  (1000) users      (100)      673 2024-05-06 19:26:42.000000 model_checker-0.2.3/model_checker.egg-info/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      402 2024-05-06 19:26:42.000000 model_checker-0.2.3/model_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-06 19:26:42.000000 model_checker-0.2.3/model_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-06 19:26:42.000000 model_checker-0.2.3/model_checker.egg-info/requires.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        8 2024-05-06 19:26:42.000000 model_checker-0.2.3/model_checker.egg-info/top_level.txt
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 19:26:42.130903 model_checker-0.2.3/package/
--rw-r--r--   0 benjamin  (1000) users      (100)      647 2024-04-28 01:38:31.000000 model_checker-0.2.3/package/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)     5918 2024-05-06 18:32:01.000000 model_checker-0.2.3/package/examples.py
--rw-r--r--   0 benjamin  (1000) users      (100)    16022 2024-05-06 17:49:27.000000 model_checker-0.2.3/package/model_definitions.py
--rw-r--r--   0 benjamin  (1000) users      (100)    34588 2024-05-06 18:33:23.000000 model_checker-0.2.3/package/model_structure.py
--rw-r--r--   0 benjamin  (1000) users      (100)    19659 2024-05-04 18:05:09.000000 model_checker-0.2.3/package/semantics.py
--rw-r--r--   0 benjamin  (1000) users      (100)     7265 2024-05-03 14:48:57.000000 model_checker-0.2.3/package/syntax.py
--rw-r--r--   0 benjamin  (1000) users      (100)     5338 2024-05-06 18:33:30.000000 model_checker-0.2.3/package/test.py
--rw-r--r--   0 benjamin  (1000) users      (100)     5838 2024-05-02 19:11:05.000000 model_checker-0.2.3/package/test_complete.py
--rw-r--r--   0 benjamin  (1000) users      (100)     2070 2024-05-03 17:30:50.000000 model_checker-0.2.3/package/top_test.py
--rw-r--r--   0 benjamin  (1000) users      (100)      887 2024-05-06 19:26:05.000000 model_checker-0.2.3/pyproject.toml
--rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-06 19:26:42.130903 model_checker-0.2.3/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 19:45:49.674518 model_checker-0.2.4/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-04-26 19:58:45.000000 model_checker-0.2.4/LICENCE
+-rw-r--r--   0 benjamin  (1000) users      (100)     1357 2024-05-06 19:45:49.673518 model_checker-0.2.4/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      683 2024-05-06 19:44:36.000000 model_checker-0.2.4/README.md
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 19:45:49.673518 model_checker-0.2.4/model_checker.egg-info/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1357 2024-05-06 19:45:49.000000 model_checker-0.2.4/model_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      376 2024-05-06 19:45:49.000000 model_checker-0.2.4/model_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-06 19:45:49.000000 model_checker-0.2.4/model_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-06 19:45:49.000000 model_checker-0.2.4/model_checker.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        8 2024-05-06 19:45:49.000000 model_checker-0.2.4/model_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 19:45:49.673518 model_checker-0.2.4/package/
+-rw-r--r--   0 benjamin  (1000) users      (100)      647 2024-04-28 01:38:31.000000 model_checker-0.2.4/package/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     4335 2024-05-06 19:43:01.000000 model_checker-0.2.4/package/examples.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    16022 2024-05-06 17:49:27.000000 model_checker-0.2.4/package/model_definitions.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    34588 2024-05-06 18:33:23.000000 model_checker-0.2.4/package/model_structure.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    19659 2024-05-04 18:05:09.000000 model_checker-0.2.4/package/semantics.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     7265 2024-05-03 14:48:57.000000 model_checker-0.2.4/package/syntax.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     5838 2024-05-02 19:11:05.000000 model_checker-0.2.4/package/test_complete.py
+-rw-r--r--   0 benjamin  (1000) users      (100)      887 2024-05-06 19:45:26.000000 model_checker-0.2.4/pyproject.toml
+-rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-06 19:45:49.674518 model_checker-0.2.4/setup.cfg
```

### Comparing `model_checker-0.2.3/LICENCE` & `model_checker-0.2.4/LICENCE`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.3/package/__init__.py` & `model_checker-0.2.4/package/__init__.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.3/package/examples.py` & `model_checker-0.2.4/package/examples.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,46 @@
 """
-module for user inputs.
+Example module for user inputs.
+Premises are conjoined and conclusions are disjoined.
+To save the output, change 'save_bool' to 'True' below.
+The examples below can be turned on and off by (un)commenting the premises an conclusions.
+The final pair of premises and conclusions to be defined will be run when the file is tested.
 """
 import os
 parent_directory = os.path.dirname(__file__)
 
 ################################
 ########## SETTINGS ############
 ################################
 
-# length of bitvectors
+# number of atomic states included in the models
 N = 3
 
 # print all Z3 constraints if a model is found
 print_cons_bool = False
 
 # print core unsatisfiable Z3 constraints if no model exists
 print_unsat_core_bool = True
 
 # present option to append output to file
-save_bool = True
+save_bool = False
 
 
 ################################
-########### WORKING ############
+######## COUNTER MODELS ########
 ################################
 
-
 ### INVALID ###
 
-# premises = []
-# conclusions = []
-
-# premises = ['A']
-# conclusions = []
+premises = ['\\neg A','(A \\boxright (B \\vee C))']
+conclusions = ['(A \\boxright B)','(A \\boxright C)']
 
-# premises = ['\\neg A','(A \\boxright (B \\vee C))']
-# conclusions = ['(A \\boxright B)','(A \\boxright C)']
-
-# # NOTE: if null verifiers are permitted, then null state verifies A
-# # but possible state c does not?
 # premises = ['A','B']
 # conclusions = ['(A \\boxright B)']
 
-# premises = ['A',]
-# conclusions = ['\\neg A']
-
 # premises = ['\\neg A']
 # conclusions = ['(A \\boxright B)','(A \\boxright \\neg B)']
 
 # premises = ['(A \\boxright B)','(B \\boxright C)']
 # conclusions = ['(A \\boxright C)']
 
 # premises = ['\\neg A']
@@ -65,48 +57,31 @@
 
 # premises = ['\\Diamond (A \\wedge B)','((A \\wedge B) \\boxright C)']
 # conclusions = ['(A \\boxright (B \\boxright C))']
 
 # premises = ['\\neg (\\top \\boxright \\neg (A \\wedge B))','((A \\wedge B) \\boxright C)']
 # conclusions = ['(A \\boxright (B \\boxright C))']
 
-# premises = ['A','(A \\boxright (B \\boxright (C \\boxright D)))']
-# conclusions = []
-
 # premises = ['(\\Box A \\vee \\Box B)']
 # conclusions = ['(A \\wedge B)']
 
-# # NOTE: slow
-# premises = ['(A \\boxright B)', '\\neg ((A \\wedge C) \\boxright B)', '(((A \\wedge C) \\wedge D) \\boxright B)']
-# conclusions = []
-
-premises = ['\\Diamond A', '\\Diamond B']
-conclusions = ['\\Diamond (A \\wedge B)']
+# premises = ['\\Diamond A', '\\Diamond B']
+# conclusions = ['\\Diamond (A \\wedge B)']
 
-# # NOTE: ssh finds a model
 # premises = ['(A \\boxright B)']
 # conclusions = ['\\Box (A \\rightarrow B)']
 
 
+################################
+############ LOGIC #############
+################################
 
-
-
-
-
-
-
-
-
-### VALID ###
-
-# # NOTE: unsat_core seems satisfiable
 # premises = []
 # conclusions = ['(A \\vee \\neg A)']
 
-# # NOTE: unsat_core seems satisfiable
 # premises = []
 # conclusions = ['\\neg (A \\wedge \\neg A)']
 
 # premises = ['A','(A \\rightarrow B)']
 # conclusions = ['B']
 
 # premises = ['(A \\boxright B)']
@@ -178,69 +153,7 @@
 # conclusions = ['(\\top \\boxright A)']
 
 # premises = ['\\Box A', '\\Diamond B']
 # conclusions = ['\\Diamond (A \\wedge B)']
 
 # premises = ['\\Box (A \\rightarrow B)']
 # conclusions = ['(A \\boxright B)']
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-################################
-######### NOT WORKING ##########
-################################
-
-
-### HIGH PRIORITY: NEGATION PROBLEM ###
-
-# # NOTE: only works without \neg B
-# premises = ['\\neg B','(A \\boxright B)']
-# conclusions = ['(\\neg B \\boxright \\neg A)']
-
-# # NOTE: only works without \neg A
-# premises = ['\\neg A','(A \\boxright C)']
-# conclusions = ['((A \\wedge B) \\boxright C)']
-
-# # NOTE: only works without \neg A and \neg B
-# premises = ['\\neg A','\\neg B','(A \\boxright B)','(B \\boxright C)']
-# conclusions = ['(A \\boxright C)']
-
-# # NOTE: only works without \neg A
-# premises = ['\\neg A', '(A \\boxright B)', '\\neg ((A \\wedge C) \\boxright B)']
-# conclusions = []
-
-### MEDIUM PRIORITY: NESTED COUNTERFACTUALS ###
-
-# # NOTE: this does not find models for N = 3
-# # NOTE: N = 4 ran for minutes on ssh
-# premises = ['(A \\boxright (B \\boxright C))']
-# conclusions = ['((A \\wedge B) \\boxright C)']
-
-# # NOTE: ssh killed process
-# premises = ['(A \\boxright C)','(B \\boxright C)']
-# conclusions = ['((A \\wedge B) \\boxright C)']
-
-### LOW PRIORITY: MODAL EQUIVALENCE ###
-
-# # NOTE: killed in ssh
-# # K axiom (top)
-# premises = ['(\\top \\boxright (A \\rightarrow B))']
-# conclusions = ['((\\top \\boxright A) \\rightarrow (\\top \\boxright B))']
-
-# # NOTE: killed in ssh
-# # top-to-box equivalence
-# premises = ['(\\top \\boxright A)']
-# conclusions = ['\\Box A']
```

### Comparing `model_checker-0.2.3/package/model_definitions.py` & `model_checker-0.2.4/package/model_definitions.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.3/package/model_structure.py` & `model_checker-0.2.4/package/model_structure.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.3/package/semantics.py` & `model_checker-0.2.4/package/semantics.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.3/package/syntax.py` & `model_checker-0.2.4/package/syntax.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.3/package/test_complete.py` & `model_checker-0.2.4/package/test_complete.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.3/pyproject.toml` & `model_checker-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-checker"
-version = "0.2.3"
+version = "0.2.4"
 description = "A hyperintensional model checker for counterfactual conditionals"
 authors = [
     { name = "Benjamin Brast-McKie", email = "benbrastmckie@gmail.com" },
     { name = "Miguel Buitrago", email = "mbuit82@gmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
```

