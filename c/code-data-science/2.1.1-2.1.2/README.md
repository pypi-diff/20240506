# Comparing `tmp/code_data_science-2.1.1.tar.gz` & `tmp/code_data_science-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_data_science-2.1.1.tar", last modified: Thu Apr 25 16:13:34 2024, max compression
+gzip compressed data, was "code_data_science-2.1.2.tar", last modified: Mon May  6 21:38:31 2024, max compression
```

## Comparing `code_data_science-2.1.1.tar` & `code_data_science-2.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:13:34.280465 code_data_science-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-25 16:13:34.280465 code_data_science-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-25 16:13:22.000000 code_data_science-2.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:13:34.276465 code_data_science-2.1.1/code_data_science/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:13:34.280465 code_data_science-2.1.1/code_data_science/clustering_src/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/clustering_src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/clustering_src/datasets_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/clustering_src/distributed_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/clustering_src/hf_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/clustering_src/logging_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/clustering_src/preprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/clustering_src/training_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/clustering_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/data_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/data_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/palette.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/scm_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/tree_data_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:13:34.280465 code_data_science-2.1.1/code_data_science/types/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/types/notebook_parameter_types.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/types/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/unique_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-25 16:13:22.000000 code_data_science-2.1.1/code_data_science/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:13:34.280465 code_data_science-2.1.1/code_data_science.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-25 16:13:34.000000 code_data_science-2.1.1/code_data_science.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-25 16:13:34.000000 code_data_science-2.1.1/code_data_science.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:13:34.000000 code_data_science-2.1.1/code_data_science.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-25 16:13:34.000000 code_data_science-2.1.1/code_data_science.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 16:13:34.000000 code_data_science-2.1.1/code_data_science.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-25 16:13:22.000000 code_data_science-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:13:34.280465 code_data_science-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:38:31.289487 code_data_science-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-06 21:38:31.289487 code_data_science-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-06 21:38:20.000000 code_data_science-2.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:38:31.285488 code_data_science-2.1.2/code_data_science/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:38:31.289487 code_data_science-2.1.2/code_data_science/clustering_src/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/clustering_src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/clustering_src/datasets_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/clustering_src/distributed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/clustering_src/hf_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/clustering_src/logging_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/clustering_src/preprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/clustering_src/training_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/clustering_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/data_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/data_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/palette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/scm_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/tree_data_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:38:31.289487 code_data_science-2.1.2/code_data_science/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/types/notebook_parameter_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/types/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/unique_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-06 21:38:20.000000 code_data_science-2.1.2/code_data_science/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:38:31.289487 code_data_science-2.1.2/code_data_science.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-06 21:38:31.000000 code_data_science-2.1.2/code_data_science.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-06 21:38:31.000000 code_data_science-2.1.2/code_data_science.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:38:31.000000 code_data_science-2.1.2/code_data_science.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-06 21:38:31.000000 code_data_science-2.1.2/code_data_science.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 21:38:31.000000 code_data_science-2.1.2/code_data_science.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-06 21:38:20.000000 code_data_science-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:38:31.289487 code_data_science-2.1.2/setup.cfg
```

### Comparing `code_data_science-2.1.1/code_data_science/clustering_src/datasets_loader.py` & `code_data_science-2.1.2/code_data_science/clustering_src/datasets_loader.py`

 * *Files identical despite different names*

### Comparing `code_data_science-2.1.1/code_data_science/clustering_src/distributed_utils.py` & `code_data_science-2.1.2/code_data_science/clustering_src/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `code_data_science-2.1.1/code_data_science/clustering_src/hf_trainer.py` & `code_data_science-2.1.2/code_data_science/clustering_src/hf_trainer.py`

 * *Files identical despite different names*

### Comparing `code_data_science-2.1.1/code_data_science/clustering_src/logging_callback.py` & `code_data_science-2.1.2/code_data_science/clustering_src/logging_callback.py`

 * *Files identical despite different names*

### Comparing `code_data_science-2.1.1/code_data_science/clustering_src/preprocessing_utils.py` & `code_data_science-2.1.2/code_data_science/clustering_src/preprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `code_data_science-2.1.1/code_data_science/clustering_src/training_args.py` & `code_data_science-2.1.2/code_data_science/clustering_src/training_args.py`

 * *Files identical despite different names*

### Comparing `code_data_science-2.1.1/code_data_science/clustering_src/utils.py` & `code_data_science-2.1.2/code_data_science/clustering_src/utils.py`

 * *Files identical despite different names*

### Comparing `code_data_science-2.1.1/code_data_science/data_grid.py` & `code_data_science-2.1.2/code_data_science/data_grid.py`

 * *Files identical despite different names*

### Comparing `code_data_science-2.1.1/code_data_science/palette.py` & `code_data_science-2.1.2/code_data_science/palette.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -155,18 +155,18 @@
 def colors_by_weight(weight):
     """
     Generate a list of moderne colors with the specified weight.
     Weights are 100, 300, 500, 700
     """
     return [
         __moderne_color_map["digital_blue"][weight],
-        __moderne_color_map["periwinkle"][weight],
+        __moderne_color_map["midnight"][weight],
         __moderne_color_map["activity_green"][weight],
         __moderne_color_map["sage"][weight],
-        __moderne_color_map["midnight"][weight],
+        __moderne_color_map["periwinkle"][weight],
     ]
 
 
 def color_gradient(color):
     """
     Generate a color weights for a specific color.
     Colors are 'blue', 'red', 'yellow', 'green', 'indigo'
```

### Comparing `code_data_science-2.1.1/code_data_science/scm_link.py` & `code_data_science-2.1.2/code_data_science/scm_link.py`

 * *Files identical despite different names*

### Comparing `code_data_science-2.1.1/code_data_science/tree_data_grid.py` & `code_data_science-2.1.2/code_data_science/tree_data_grid.py`

 * *Files identical despite different names*

### Comparing `code_data_science-2.1.1/code_data_science/unique_dictionaries.py` & `code_data_science-2.1.2/code_data_science/unique_dictionaries.py`

 * *Files identical despite different names*

### Comparing `code_data_science-2.1.1/code_data_science/versions.py` & `code_data_science-2.1.2/code_data_science/versions.py`

 * *Files identical despite different names*

### Comparing `code_data_science-2.1.1/code_data_science.egg-info/SOURCES.txt` & `code_data_science-2.1.2/code_data_science.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `code_data_science-2.1.1/pyproject.toml` & `code_data_science-2.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # @see https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 [project]
 name = "code_data_science"
-version = "2.1.1"
+version = "2.1.2"
 description = "A python implementation of various tools used in code data science."
 authors = [
     { name = "Jonathan Schneider", email = "jonathan@moderne.io" },
     { name = "Kyle Scully", email = "kyle@moderne.io" }
 ]
 license = { text = "Apache-2.0" }
 dependencies = ["pandas==2.0.3", "ipython==8.13.0"]
```

