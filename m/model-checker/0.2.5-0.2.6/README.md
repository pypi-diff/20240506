# Comparing `tmp/model_checker-0.2.5.tar.gz` & `tmp/model_checker-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_checker-0.2.5.tar", last modified: Mon May  6 20:00:14 2024, max compression
+gzip compressed data, was "model_checker-0.2.6.tar", last modified: Mon May  6 20:48:40 2024, max compression
```

## Comparing `model_checker-0.2.5.tar` & `model_checker-0.2.6.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 20:00:14.897194 model_checker-0.2.5/
--rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-04-26 19:58:45.000000 model_checker-0.2.5/LICENCE
--rw-r--r--   0 benjamin  (1000) users      (100)     1357 2024-05-06 20:00:14.897194 model_checker-0.2.5/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      683 2024-05-06 19:44:36.000000 model_checker-0.2.5/README.md
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 20:00:14.897194 model_checker-0.2.5/model_checker.egg-info/
--rw-r--r--   0 benjamin  (1000) users      (100)     1357 2024-05-06 20:00:14.000000 model_checker-0.2.5/model_checker.egg-info/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      416 2024-05-06 20:00:14.000000 model_checker-0.2.5/model_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-06 20:00:14.000000 model_checker-0.2.5/model_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       61 2024-05-06 20:00:14.000000 model_checker-0.2.5/model_checker.egg-info/entry_points.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-06 20:00:14.000000 model_checker-0.2.5/model_checker.egg-info/requires.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        8 2024-05-06 20:00:14.000000 model_checker-0.2.5/model_checker.egg-info/top_level.txt
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 20:00:14.897194 model_checker-0.2.5/package/
--rw-r--r--   0 benjamin  (1000) users      (100)      647 2024-04-28 01:38:31.000000 model_checker-0.2.5/package/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)     4335 2024-05-06 19:43:01.000000 model_checker-0.2.5/package/examples.py
--rw-r--r--   0 benjamin  (1000) users      (100)    16022 2024-05-06 17:49:27.000000 model_checker-0.2.5/package/model_definitions.py
--rw-r--r--   0 benjamin  (1000) users      (100)    34588 2024-05-06 18:33:23.000000 model_checker-0.2.5/package/model_structure.py
--rw-r--r--   0 benjamin  (1000) users      (100)    19659 2024-05-04 18:05:09.000000 model_checker-0.2.5/package/semantics.py
--rw-r--r--   0 benjamin  (1000) users      (100)     7265 2024-05-03 14:48:57.000000 model_checker-0.2.5/package/syntax.py
--rw-r--r--   0 benjamin  (1000) users      (100)     5838 2024-05-02 19:11:05.000000 model_checker-0.2.5/package/test_complete.py
--rw-r--r--   0 benjamin  (1000) users      (100)      883 2024-05-06 19:59:56.000000 model_checker-0.2.5/pyproject.toml
--rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-06 20:00:14.897194 model_checker-0.2.5/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 20:48:40.571088 model_checker-0.2.6/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-04-26 19:58:45.000000 model_checker-0.2.6/LICENCE
+-rw-r--r--   0 benjamin  (1000) users      (100)     1372 2024-05-06 20:48:40.570088 model_checker-0.2.6/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      683 2024-05-06 19:44:36.000000 model_checker-0.2.6/README.md
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 20:48:40.570088 model_checker-0.2.6/model_checker.egg-info/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1372 2024-05-06 20:48:40.000000 model_checker-0.2.6/model_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      456 2024-05-06 20:48:40.000000 model_checker-0.2.6/model_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-06 20:48:40.000000 model_checker-0.2.6/model_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       61 2024-05-06 20:48:40.000000 model_checker-0.2.6/model_checker.egg-info/entry_points.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-06 20:48:40.000000 model_checker-0.2.6/model_checker.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        8 2024-05-06 20:48:40.000000 model_checker-0.2.6/model_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 20:48:40.570088 model_checker-0.2.6/package/
+-rw-r--r--   0 benjamin  (1000) users      (100)        0 2024-05-06 20:40:08.000000 model_checker-0.2.6/package/__init__.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 20:48:40.570088 model_checker-0.2.6/package/modules/
+-rw-r--r--   0 benjamin  (1000) users      (100)        0 2024-05-06 20:40:02.000000 model_checker-0.2.6/package/modules/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    16023 2024-05-06 20:40:50.000000 model_checker-0.2.6/package/modules/model_definitions.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    34591 2024-05-06 20:40:50.000000 model_checker-0.2.6/package/modules/model_structure.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    19660 2024-05-06 20:40:50.000000 model_checker-0.2.6/package/modules/semantics.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     7265 2024-05-06 20:40:50.000000 model_checker-0.2.6/package/modules/syntax.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     5846 2024-05-06 20:44:05.000000 model_checker-0.2.6/package/test_complete.py
+-rw-r--r--   0 benjamin  (1000) users      (100)      901 2024-05-06 20:38:48.000000 model_checker-0.2.6/pyproject.toml
+-rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-06 20:48:40.571088 model_checker-0.2.6/setup.cfg
```

### Comparing `model_checker-0.2.5/LICENCE` & `model_checker-0.2.6/LICENCE`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.5/PKG-INFO` & `model_checker-0.2.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.2.5
+Version: 0.2.6
 Summary: A hyperintensional model checker for counterfactual conditionals
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
-Keywords: semantics,Z3,counterfactuals,model checker
+Keywords: semantics,Z3,counterfactuals,model checker,theorem prover
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: z3-solver
```

### Comparing `model_checker-0.2.5/README.md` & `model_checker-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.5/model_checker.egg-info/PKG-INFO` & `model_checker-0.2.6/model_checker.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.2.5
+Version: 0.2.6
 Summary: A hyperintensional model checker for counterfactual conditionals
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
-Keywords: semantics,Z3,counterfactuals,model checker
+Keywords: semantics,Z3,counterfactuals,model checker,theorem prover
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: z3-solver
```

### Comparing `model_checker-0.2.5/package/model_definitions.py` & `model_checker-0.2.6/package/modules/model_definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 '''
 
 import sys
 from z3 import (
     BitVecVal, simplify,
 )
 
-from syntax import Infix
+from .syntax import Infix
 
 def summation(n, func, start = 0):
     '''summation of i ranging from start to n of func(i)
     used in find_all_bits'''
     if start == n:
         return func(start)
     return func(start) + summation(n,func,start+1)
```

### Comparing `model_checker-0.2.5/package/model_structure.py` & `model_checker-0.2.6/package/modules/model_structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 import sys
 from z3 import (
     Function,
     BitVecSort,
     BoolSort,
     BitVec,
 )
-from semantics import (
+from .semantics import (
     make_constraints,
     solve_constraints,
 )
-from model_definitions import (
+from .model_definitions import (
     find_compatible_parts,
     atomic_propositions_dict,
     coproduct,
     find_all_bits,
     find_max_comp_ver_parts,
     find_null_bit,
     find_poss_bits,
@@ -32,15 +32,15 @@
     int_to_binary,
     infix_combine,
     find_subsentences_of_kind,
     is_counterfactual,
     is_modal,
 
 )
-from syntax import (
+from .syntax import (
     AtomSort,
     Infix,
 )
 
 # TODO: the three types of objects that it would be good to store as classes
 # include: (1) premises, conclusions, input_sentences, prefix_sentences,
 # prefix_sub_sentences, infix_sub_sentences, sentence_letters, constraints;
```

### Comparing `model_checker-0.2.5/package/semantics.py` & `model_checker-0.2.6/package/modules/semantics.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Implies,
     Or,
     Not,
     Solver,
     And,
     BitVec,
 )
-from syntax import Prefix
+from .syntax import Prefix
 
 # from sympy import symbols, Or, And, Implies, Not, to_cnf
 
 # def bit_vec_length():
 #     from test_complete import N
 #     return N
 # N = bit_vec_length()
```

### Comparing `model_checker-0.2.5/package/syntax.py` & `model_checker-0.2.6/package/modules/syntax.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.5/package/test_complete.py` & `model_checker-0.2.6/package/test_complete.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 '''
 
 import argparse
 import os
 import importlib.util
 import sys
 from string import Template
-from model_structure import make_model_for
+from modules.model_structure import make_model_for
 
 script_template = Template("""
 '''
 Model Checker: ${name}
 '''
 import os
 parent_directory = os.path.dirname(__file__)
```

### Comparing `model_checker-0.2.5/pyproject.toml` & `model_checker-0.2.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-checker"
-version = "0.2.5"
+version = "0.2.6"
 description = "A hyperintensional model checker for counterfactual conditionals"
 authors = [
     { name = "Benjamin Brast-McKie", email = "benbrastmckie@gmail.com" },
     { name = "Miguel Buitrago", email = "mbuit82@gmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-keywords = ["semantics", "Z3", "counterfactuals", "model checker"]
+keywords = ["semantics", "Z3", "counterfactuals", "model checker", "theorem prover"]
 dependencies = [
     "z3-solver",
 ]
 
 [project.urls]
 Homepage = "https://github.com/benbrastmckie/ModelChecker"
 Issues = "https://github.com/benbrastmckie/ModelChecker/issues"
```

