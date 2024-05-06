# Comparing `tmp/model_checker-0.2.4.tar.gz` & `tmp/model_checker-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_checker-0.2.4.tar", last modified: Mon May  6 19:45:49 2024, max compression
+gzip compressed data, was "model_checker-0.2.5.tar", last modified: Mon May  6 20:00:14 2024, max compression
```

## Comparing `model_checker-0.2.4.tar` & `model_checker-0.2.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 19:45:49.674518 model_checker-0.2.4/
--rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-04-26 19:58:45.000000 model_checker-0.2.4/LICENCE
--rw-r--r--   0 benjamin  (1000) users      (100)     1357 2024-05-06 19:45:49.673518 model_checker-0.2.4/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      683 2024-05-06 19:44:36.000000 model_checker-0.2.4/README.md
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 19:45:49.673518 model_checker-0.2.4/model_checker.egg-info/
--rw-r--r--   0 benjamin  (1000) users      (100)     1357 2024-05-06 19:45:49.000000 model_checker-0.2.4/model_checker.egg-info/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      376 2024-05-06 19:45:49.000000 model_checker-0.2.4/model_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-06 19:45:49.000000 model_checker-0.2.4/model_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-06 19:45:49.000000 model_checker-0.2.4/model_checker.egg-info/requires.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        8 2024-05-06 19:45:49.000000 model_checker-0.2.4/model_checker.egg-info/top_level.txt
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 19:45:49.673518 model_checker-0.2.4/package/
--rw-r--r--   0 benjamin  (1000) users      (100)      647 2024-04-28 01:38:31.000000 model_checker-0.2.4/package/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)     4335 2024-05-06 19:43:01.000000 model_checker-0.2.4/package/examples.py
--rw-r--r--   0 benjamin  (1000) users      (100)    16022 2024-05-06 17:49:27.000000 model_checker-0.2.4/package/model_definitions.py
--rw-r--r--   0 benjamin  (1000) users      (100)    34588 2024-05-06 18:33:23.000000 model_checker-0.2.4/package/model_structure.py
--rw-r--r--   0 benjamin  (1000) users      (100)    19659 2024-05-04 18:05:09.000000 model_checker-0.2.4/package/semantics.py
--rw-r--r--   0 benjamin  (1000) users      (100)     7265 2024-05-03 14:48:57.000000 model_checker-0.2.4/package/syntax.py
--rw-r--r--   0 benjamin  (1000) users      (100)     5838 2024-05-02 19:11:05.000000 model_checker-0.2.4/package/test_complete.py
--rw-r--r--   0 benjamin  (1000) users      (100)      887 2024-05-06 19:45:26.000000 model_checker-0.2.4/pyproject.toml
--rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-06 19:45:49.674518 model_checker-0.2.4/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 20:00:14.897194 model_checker-0.2.5/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-04-26 19:58:45.000000 model_checker-0.2.5/LICENCE
+-rw-r--r--   0 benjamin  (1000) users      (100)     1357 2024-05-06 20:00:14.897194 model_checker-0.2.5/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      683 2024-05-06 19:44:36.000000 model_checker-0.2.5/README.md
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 20:00:14.897194 model_checker-0.2.5/model_checker.egg-info/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1357 2024-05-06 20:00:14.000000 model_checker-0.2.5/model_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      416 2024-05-06 20:00:14.000000 model_checker-0.2.5/model_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-06 20:00:14.000000 model_checker-0.2.5/model_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       61 2024-05-06 20:00:14.000000 model_checker-0.2.5/model_checker.egg-info/entry_points.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-06 20:00:14.000000 model_checker-0.2.5/model_checker.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        8 2024-05-06 20:00:14.000000 model_checker-0.2.5/model_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 20:00:14.897194 model_checker-0.2.5/package/
+-rw-r--r--   0 benjamin  (1000) users      (100)      647 2024-04-28 01:38:31.000000 model_checker-0.2.5/package/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     4335 2024-05-06 19:43:01.000000 model_checker-0.2.5/package/examples.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    16022 2024-05-06 17:49:27.000000 model_checker-0.2.5/package/model_definitions.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    34588 2024-05-06 18:33:23.000000 model_checker-0.2.5/package/model_structure.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    19659 2024-05-04 18:05:09.000000 model_checker-0.2.5/package/semantics.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     7265 2024-05-03 14:48:57.000000 model_checker-0.2.5/package/syntax.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     5838 2024-05-02 19:11:05.000000 model_checker-0.2.5/package/test_complete.py
+-rw-r--r--   0 benjamin  (1000) users      (100)      883 2024-05-06 19:59:56.000000 model_checker-0.2.5/pyproject.toml
+-rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-06 20:00:14.897194 model_checker-0.2.5/setup.cfg
```

### Comparing `model_checker-0.2.4/LICENCE` & `model_checker-0.2.5/LICENCE`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.4/PKG-INFO` & `model_checker-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.2.4
+Version: 0.2.5
 Summary: A hyperintensional model checker for counterfactual conditionals
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `model_checker-0.2.4/README.md` & `model_checker-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.4/model_checker.egg-info/PKG-INFO` & `model_checker-0.2.5/model_checker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.2.4
+Version: 0.2.5
 Summary: A hyperintensional model checker for counterfactual conditionals
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `model_checker-0.2.4/package/__init__.py` & `model_checker-0.2.5/package/__init__.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.4/package/examples.py` & `model_checker-0.2.5/package/examples.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.4/package/model_definitions.py` & `model_checker-0.2.5/package/model_definitions.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.4/package/model_structure.py` & `model_checker-0.2.5/package/model_structure.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.4/package/semantics.py` & `model_checker-0.2.5/package/semantics.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.4/package/syntax.py` & `model_checker-0.2.5/package/syntax.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.4/package/test_complete.py` & `model_checker-0.2.5/package/test_complete.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.4/pyproject.toml` & `model_checker-0.2.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-checker"
-version = "0.2.4"
+version = "0.2.5"
 description = "A hyperintensional model checker for counterfactual conditionals"
 authors = [
     { name = "Benjamin Brast-McKie", email = "benbrastmckie@gmail.com" },
     { name = "Miguel Buitrago", email = "mbuit82@gmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
@@ -22,9 +22,9 @@
     "z3-solver",
 ]
 
 [project.urls]
 Homepage = "https://github.com/benbrastmckie/ModelChecker"
 Issues = "https://github.com/benbrastmckie/ModelChecker/issues"
 
-[tool.poetry.scripts]
+[project.scripts]
 model-checker = "package.test_complete:main"
```

