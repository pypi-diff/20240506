# Comparing `tmp/aiidalab_widgets_base-2.2.0a1.tar.gz` & `tmp/aiidalab_widgets_base-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiidalab_widgets_base-2.2.0a1.tar", last modified: Wed Apr 10 20:18:52 2024, max compression
+gzip compressed data, was "aiidalab_widgets_base-2.2.1.tar", last modified: Mon May  6 09:16:49 2024, max compression
```

## Comparing `aiidalab_widgets_base-2.2.0a1.tar` & `aiidalab_widgets_base-2.2.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:18:52.520245 aiidalab_widgets_base-2.2.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-10 20:18:52.520245 aiidalab_widgets_base-2.2.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:18:52.512245 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    70960 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/computational_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:18:52.516245 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15852 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     8796 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11302 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/elns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    29520 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/process.py
--rw-r--r--   0 runner    (1001) docker     (127)    59993 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:18:52.516245 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    59471 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/viewers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:18:52.516245 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-10 20:18:52.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-10 20:18:52.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:18:52.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:18:52.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-10 20:18:52.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 20:18:52.000000 aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-10 20:18:52.520245 aiidalab_widgets_base-2.2.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:18:52.516245 aiidalab_widgets_base-2.2.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_bug_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    30474 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_computational_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_elns.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)    10807 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_viewers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-10 20:18:48.000000 aiidalab_widgets_base-2.2.0a1/tests/test_wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:16:49.167941 aiidalab_widgets_base-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-06 09:16:49.167941 aiidalab_widgets_base-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:16:49.159941 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70960 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/computational_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:16:49.159941 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15852 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8796 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11302 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/elns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14254 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29520 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60005 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:16:49.159941 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60452 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:16:49.163941 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-06 09:16:49.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-06 09:16:49.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:16:49.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:16:48.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-06 09:16:49.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 09:16:49.000000 aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-06 09:16:49.167941 aiidalab_widgets_base-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:16:49.163941 aiidalab_widgets_base-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30474 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_computational_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_elns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11633 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_viewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-06 09:16:45.000000 aiidalab_widgets_base-2.2.1/tests/test_wizard.py
```

### Comparing `aiidalab_widgets_base-2.2.0a1/LICENSE.txt` & `aiidalab_widgets_base-2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/PKG-INFO` & `aiidalab_widgets_base-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiidalab_widgets_base
-Version: 2.2.0a1
+Version: 2.2.1
 Summary: Reusable widgets for AiiDAlab applications.
 Home-page: https://github.com/aiidalab/aiidalab-widgets-base
 Author: The AiiDAlab team
 Author-email: aiidalab@materialscloud.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
@@ -27,14 +27,15 @@
 Requires-Dist: ipywidgets~=7.7
 Requires-Dist: widgetsnbextension<3.6.3
 Requires-Dist: more-itertools~=8.0
 Requires-Dist: pymysql~=0.9
 Requires-Dist: nglview~=3.0
 Requires-Dist: spglib<3,>=1.14
 Requires-Dist: vapory~=0.1.2
+Requires-Dist: pandas~=2.1
 Provides-Extra: dev
 Requires-Dist: bumpver~=2023.1129; extra == "dev"
 Requires-Dist: pgtest~=1.3; extra == "dev"
 Requires-Dist: pre-commit~=3.5; extra == "dev"
 Requires-Dist: pytest~=7.1.0; extra == "dev"
 Requires-Dist: pytest-cov~=4.0; extra == "dev"
 Requires-Dist: pytest-docker~=2.0; extra == "dev"
```

### Comparing `aiidalab_widgets_base-2.2.0a1/README.md` & `aiidalab_widgets_base-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/__init__.py` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,8 +113,8 @@
     "SubmitButtonWidget",
     "WizardAppWidget",
     "WizardAppWidgetStep",
     "register_viewer_widget",
     "viewer",
 ]
 
-__version__ = "2.2.0a1"
+__version__ = "2.2.1"
```

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/bug_report.py` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/bug_report.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/computational_resources.py` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/computational_resources.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/data/__init__.py` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/databases.py` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/databases.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/dicts.py` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/dicts.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/elns.py` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/elns.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/export.py` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/export.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/misc.py` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/misc.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/nodes.py` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 class AiidaNodeTreeNode(ipytree.Node):
     def __init__(self, pk, name, **kwargs):
         self.pk = pk
         self.nodes_registry = {}
         super().__init__(name=name, **kwargs)
 
     @tl.default("opened")
-    def _default_openend(self):
-        return False
+    def _default_opened(self):
+        return True
 
 
 class AiidaProcessNodeTreeNode(AiidaNodeTreeNode):
     def __init__(self, pk, **kwargs):
         self.outputs_node = AiidaOutputsTreeNode(name="outputs", parent_pk=pk)
         super().__init__(pk=pk, **kwargs)
 
@@ -87,15 +87,15 @@
 
 class CalcFunctionTreeNode(AiidaProcessNodeTreeNode):
     icon = tl.Unicode("gear").tag(sync=True)
 
 
 class AiidaOutputsTreeNode(ipytree.Node):
     icon = tl.Unicode("folder").tag(sync=True)
-    disabled = tl.Bool(True).tag(sync=True)
+    disabled = tl.Bool(False).tag(sync=True)
 
     def __init__(self, name, parent_pk, namespaces: tuple[str, ...] = (), **kwargs):
         self.parent_pk = parent_pk
         self.nodes_registry = {}
         self.namespaces = namespaces
         super().__init__(name=name, **kwargs)
 
@@ -137,14 +137,23 @@
         # causes the output to not be properly cleared. We therefore refresh the
         # displayed tree upon change of the process trait.
         with self:
             clear_output()
             display(self._tree)
 
     def _observe_tree_selected_nodes(self, change):
+        for node in change["new"]:
+            # find the selected node and build the tree from it, so that users can expand and explore the tree
+            node_pk = (
+                node.parent_pk
+                if isinstance(node, AiidaOutputsTreeNode)
+                else getattr(node, "pk", None)
+            )
+
+            self._build_tree(self.find_node(node_pk, getattr(node, "namespaces", None)))
         return self.set_trait(
             "selected_nodes",
             tuple(
                 orm.load_node(pk=node.pk)
                 for node in change["new"]
                 if hasattr(node, "pk")
             ),
@@ -176,17 +185,27 @@
     def _to_tree_node(cls, node, name=None, **kwargs):
         """Convert an AiiDA node to a tree node."""
         if name is None:
             if isinstance(node, orm.ProcessNode):
                 name = calc_info(node)
             else:
                 name = str(node)
-        return cls.NODE_TYPE.get(type(node), UnknownTypeTreeNode)(
+        tree_node = cls.NODE_TYPE.get(type(node), UnknownTypeTreeNode)(
             pk=node.pk, name=name, **kwargs
         )
+        # Set the style based on the process state of the node
+        if isinstance(node, orm.ProcessNode):
+            process_state = (
+                engine.ProcessState.EXCEPTED if node.is_failed else node.process_state
+            )
+            tree_node.icon_style = cls.PROCESS_STATE_STYLE.get(
+                process_state, cls.PROCESS_STATE_STYLE_DEFAULT
+            )
+
+        return tree_node
 
     @classmethod
     def _find_called(cls, root):
         assert isinstance(root, AiidaProcessNodeTreeNode)
         process_node = orm.load_node(root.pk)
         called = process_node.called
         called.sort(key=lambda p: p.ctime)
@@ -247,16 +266,16 @@
             yield root.outputs_node
             yield from cls._find_called(root)
         elif isinstance(root, AiidaOutputsTreeNode):
             yield from cls._find_outputs(root)
 
     @classmethod
     def _build_tree(cls, root):
-        """Recursively build a tree nodes graph for a given tree node."""
-        root.nodes = [cls._build_tree(child) for child in cls._find_children(root)]
+        """Build a tree nodes graph for a given tree node."""
+        root.nodes = list(cls._find_children(root))
         return root
 
     @classmethod
     def _walk_tree(cls, root):
         """Breadth-first search of the node tree."""
         yield root
         for node in root.nodes:
@@ -280,17 +299,24 @@
     def update(self, _=None):
         """Refresh nodes based on the latest state of the root process and its children."""
         for root_node in self._tree.nodes:
             self._build_tree(root_node)
             for tree_node in self._walk_tree(root_node):
                 self._update_tree_node(tree_node)
 
-    def find_node(self, pk):
+    def find_node(self, pk, namespaces=None):
+        """Find a node by its pk and namespaces.
+        If node is an output node, it is identified by the parent pk and namespaces, otherwise by the pk."""
         for node in self._walk_tree(self._tree):
-            if getattr(node, "pk", None) == pk:
+            node_pk = (
+                node.parent_pk
+                if isinstance(node, AiidaOutputsTreeNode)
+                else getattr(node, "pk", None)
+            )
+            if node_pk == pk and getattr(node, "namespaces", None) == namespaces:
                 return node
         raise KeyError(pk)
 
 
 class _AppIcon:
     def __init__(self, app, path_to_root, node):
         name = app["name"]
```

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/process.py` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/process.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/structures.py` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
 
         if (
             isinstance(self.input_structure, orm.Data)
             and self.input_structure.is_stored
         ):
             # Make a link between self.input_structure and self.structure_node
             @engine.calcfunction
-            def user_modifications(_source_structure):
+            def user_modifications(source_structure):  # noqa F841
                 return self.structure_node
 
             structure_node = user_modifications(self.input_structure)
 
         else:
             structure_node = self.structure_node.store()
         self.output.value = f"Stored in AiiDA [{structure_node}]"
```

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/utils/__init__.py` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/viewers.py` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/viewers.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,20 @@
     Returns the object itself if the viewer wasn't found."""
     if not isinstance(obj, orm.Node):  # only working with AiiDA nodes
         warnings.warn(
             f"This viewer works only with AiiDA objects, got {type(obj)}", stacklevel=2
         )
         return obj
 
-    if obj.node_type in AIIDA_VIEWER_MAPPING:
-        _viewer = AIIDA_VIEWER_MAPPING[obj.node_type]
+    _viewer = AIIDA_VIEWER_MAPPING.get(obj.node_type)
+    if isinstance(obj, orm.ProcessNode):
+        # Allow to register specific viewers based on obj.process_type
+        _viewer = AIIDA_VIEWER_MAPPING.get(obj.process_type, _viewer)
+
+    if _viewer:
         return _viewer(obj, **kwargs)
     else:
         # No viewer registered for this type, return object itself
         return obj
 
 
 class AiidaNodeViewWidget(ipw.VBox):
@@ -1132,15 +1136,26 @@
 
     @tl.observe("supercell")
     def _observe_supercell(self, _=None):
         if self.structure is not None:
             self.set_trait(
                 "displayed_structure", None
             )  # To make sure the structure is always updated.
-            self.set_trait("displayed_structure", self.structure.repeat(self.supercell))
+            # nglview displays structures by first saving them to a temporary "pdb" file, which necessitates
+            # converting the unit cell and atomic positions into a standard form where the a-axis aligns along the x-axis.
+            # This transformation can cause discrepancies between the atom positions and custom bonds calculated from the original structure.
+            # To mitigate this, we transform the "displayed_structure" into the standard form prior to rendering in nglview.
+            # This ensures that nglview's internal handling does not further modify the structure unexpectedly.
+            standard_structure = self.structure.copy()
+            standard_structure.set_cell(
+                self.structure.cell.standard_form()[0], scale_atoms=True
+            )
+            self.set_trait(
+                "displayed_structure", standard_structure.repeat(self.supercell)
+            )
 
     @tl.validate("structure")
     def _valid_structure(self, change):
         """Update structure."""
         structure = change["value"]
         if isinstance(structure, ase.Atoms):
             self.pk = None
```

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base/wizard.py` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base/wizard.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/PKG-INFO` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiidalab_widgets_base
-Version: 2.2.0a1
+Version: 2.2.1
 Summary: Reusable widgets for AiiDAlab applications.
 Home-page: https://github.com/aiidalab/aiidalab-widgets-base
 Author: The AiiDAlab team
 Author-email: aiidalab@materialscloud.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
@@ -27,14 +27,15 @@
 Requires-Dist: ipywidgets~=7.7
 Requires-Dist: widgetsnbextension<3.6.3
 Requires-Dist: more-itertools~=8.0
 Requires-Dist: pymysql~=0.9
 Requires-Dist: nglview~=3.0
 Requires-Dist: spglib<3,>=1.14
 Requires-Dist: vapory~=0.1.2
+Requires-Dist: pandas~=2.1
 Provides-Extra: dev
 Requires-Dist: bumpver~=2023.1129; extra == "dev"
 Requires-Dist: pgtest~=1.3; extra == "dev"
 Requires-Dist: pre-commit~=3.5; extra == "dev"
 Requires-Dist: pytest~=7.1.0; extra == "dev"
 Requires-Dist: pytest-cov~=4.0; extra == "dev"
 Requires-Dist: pytest-docker~=2.0; extra == "dev"
```

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/SOURCES.txt` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/aiidalab_widgets_base.egg-info/requires.txt` & `aiidalab_widgets_base-2.2.1/aiidalab_widgets_base.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ipywidgets~=7.7
 widgetsnbextension<3.6.3
 more-itertools~=8.0
 pymysql~=0.9
 nglview~=3.0
 spglib<3,>=1.14
 vapory~=0.1.2
+pandas~=2.1
 
 [dev]
 bumpver~=2023.1129
 pgtest~=1.3
 pre-commit~=3.5
 pytest~=7.1.0
 pytest-cov~=4.0
```

### Comparing `aiidalab_widgets_base-2.2.0a1/pyproject.toml` & `aiidalab_widgets_base-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/setup.cfg` & `aiidalab_widgets_base-2.2.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 	ipywidgets~=7.7
 	widgetsnbextension<3.6.3
 	more-itertools~=8.0
 	pymysql~=0.9
 	nglview~=3.0
 	spglib>=1.14,<3
 	vapory~=0.1.2
+	pandas~=2.1
 python_requires = >=3.9
 include_package_data = True
 zip_safe = False
 
 [options.extras_require]
 dev = 
 	bumpver~=2023.1129
@@ -60,15 +61,15 @@
 docs = 
 	sphinx
 	sphinx-design
 	pydata-sphinx-theme
 	myst-nb
 
 [bumpver]
-current_version = "v2.2.0a1"
+current_version = "v2.2.1"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = True
 tag = True
 push = True
 
 [bumpver:file_patterns]
```

### Comparing `aiidalab_widgets_base-2.2.0a1/tests/test_bug_report.py` & `aiidalab_widgets_base-2.2.1/tests/test_bug_report.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/tests/test_computational_resources.py` & `aiidalab_widgets_base-2.2.1/tests/test_computational_resources.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/tests/test_databases.py` & `aiidalab_widgets_base-2.2.1/tests/test_databases.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/tests/test_elns.py` & `aiidalab_widgets_base-2.2.1/tests/test_elns.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/tests/test_export.py` & `aiidalab_widgets_base-2.2.1/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/tests/test_nodes.py` & `aiidalab_widgets_base-2.2.1/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/tests/test_process.py` & `aiidalab_widgets_base-2.2.1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/tests/test_structures.py` & `aiidalab_widgets_base-2.2.1/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `aiidalab_widgets_base-2.2.0a1/tests/test_viewers.py` & `aiidalab_widgets_base-2.2.1/tests/test_viewers.py`

 * *Files 5% similar despite different names*

```diff
@@ -278,7 +278,29 @@
             (0.0, 0.763239, -0.477047),
             (0.0, -0.763239, -0.477047),
         ],
     )
     viewer = viewers.StructureDataViewer()
     bonds = viewer._compute_bonds(water)
     assert len(bonds) == 4
+
+
+@pytest.mark.usefixtures("aiida_profile_clean")
+def test_loading_viewer_using_process_type(generate_calc_job_node):
+    """Test loading a viewer widget based on the process type of the process node."""
+    from aiidalab_widgets_base import register_viewer_widget
+
+    # Define and register a viewer widget for the calculation type identified by "aiida.calculations:abc".
+    @register_viewer_widget("aiida.calculations:abc")
+    class AbcViewer:
+        def __init__(self, node=None):
+            self.node = node
+
+    # Generate a calc job node with the specific entry point "abc".
+    process = generate_calc_job_node(entry_point_name="abc")
+    # Load the viewer widget for the generated process node.
+    viewer = viewers.viewer(process)
+    # Verify that the loaded viewer is the correct type and is associated with the intended node.
+    assert isinstance(
+        viewer, AbcViewer
+    ), "Viewer is not an instance of the expected viewer class."
+    assert viewer.node == process, "Viewer's node does not match the test process node."
```

### Comparing `aiidalab_widgets_base-2.2.0a1/tests/test_wizard.py` & `aiidalab_widgets_base-2.2.1/tests/test_wizard.py`

 * *Files identical despite different names*

