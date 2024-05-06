# Comparing `tmp/ophyd_registry-1.2.0.tar.gz` & `tmp/ophyd_registry-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ophyd_registry-1.2.0.tar", last modified: Thu May  2 22:56:28 2024, max compression
+gzip compressed data, was "ophyd_registry-1.2.1.tar", last modified: Mon May  6 15:18:57 2024, max compression
```

## Comparing `ophyd_registry-1.2.0.tar` & `ophyd_registry-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-02 22:56:28.841963 ophyd_registry-1.2.0/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     9085 2024-05-02 22:56:28.840963 ophyd_registry-1.2.0/PKG-INFO
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     8066 2024-05-02 20:05:45.000000 ophyd_registry-1.2.0/README.md
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      921 2024-05-02 22:53:46.000000 ophyd_registry-1.2.0/pyproject.toml
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       38 2024-05-02 22:56:28.841963 ophyd_registry-1.2.0/setup.cfg
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-02 22:56:28.838963 ophyd_registry-1.2.0/src/
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-02 22:56:28.840963 ophyd_registry-1.2.0/src/ophyd_registry.egg-info/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     9085 2024-05-02 22:56:28.000000 ophyd_registry-1.2.0/src/ophyd_registry.egg-info/PKG-INFO
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      377 2024-05-02 22:56:28.000000 ophyd_registry-1.2.0/src/ophyd_registry.egg-info/SOURCES.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)        1 2024-05-02 22:56:28.000000 ophyd_registry-1.2.0/src/ophyd_registry.egg-info/dependency_links.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       76 2024-05-02 22:56:28.000000 ophyd_registry-1.2.0/src/ophyd_registry.egg-info/requires.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       14 2024-05-02 22:56:28.000000 ophyd_registry-1.2.0/src/ophyd_registry.egg-info/top_level.txt
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-02 22:56:28.839963 ophyd_registry-1.2.0/src/ophydregistry/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      126 2024-03-24 15:55:03.000000 ophyd_registry-1.2.0/src/ophydregistry/__init__.py
--rw-------   0 b268176   (2319) xsdspc    (1117)      371 2023-12-22 00:11:16.000000 ophyd_registry-1.2.0/src/ophydregistry/exceptions.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)    19461 2024-05-02 21:23:07.000000 ophyd_registry-1.2.0/src/ophydregistry/registry.py
-drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-02 22:56:28.839963 ophyd_registry-1.2.0/src/ophydregistry/tests/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)    14037 2024-05-02 22:54:12.000000 ophyd_registry-1.2.0/src/ophydregistry/tests/test_instrument_registry.py
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-06 15:18:57.503021 ophyd_registry-1.2.1/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     9085 2024-05-06 15:18:57.499025 ophyd_registry-1.2.1/PKG-INFO
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     8066 2024-05-02 23:03:27.000000 ophyd_registry-1.2.1/README.md
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      921 2024-05-06 15:17:59.000000 ophyd_registry-1.2.1/pyproject.toml
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       38 2024-05-06 15:18:57.503030 ophyd_registry-1.2.1/setup.cfg
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-06 15:18:57.222050 ophyd_registry-1.2.1/src/
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-06 15:18:57.494026 ophyd_registry-1.2.1/src/ophyd_registry.egg-info/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     9085 2024-05-06 15:18:57.000000 ophyd_registry-1.2.1/src/ophyd_registry.egg-info/PKG-INFO
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      377 2024-05-06 15:18:57.000000 ophyd_registry-1.2.1/src/ophyd_registry.egg-info/SOURCES.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)        1 2024-05-06 15:18:57.000000 ophyd_registry-1.2.1/src/ophyd_registry.egg-info/dependency_links.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       76 2024-05-06 15:18:57.000000 ophyd_registry-1.2.1/src/ophyd_registry.egg-info/requires.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       14 2024-05-06 15:18:57.000000 ophyd_registry-1.2.1/src/ophyd_registry.egg-info/top_level.txt
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-06 15:18:57.484029 ophyd_registry-1.2.1/src/ophydregistry/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      126 2024-03-24 15:55:03.000000 ophyd_registry-1.2.1/src/ophydregistry/__init__.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      371 2023-12-22 00:11:16.000000 ophyd_registry-1.2.1/src/ophydregistry/exceptions.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)    19662 2024-05-06 15:17:59.000000 ophyd_registry-1.2.1/src/ophydregistry/registry.py
+drwxr-xr-x   0 b268176   (2319) xsdspc    (1117)        0 2024-05-06 15:18:57.489024 ophyd_registry-1.2.1/src/ophydregistry/tests/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)    14037 2024-05-06 15:17:59.000000 ophyd_registry-1.2.1/src/ophydregistry/tests/test_instrument_registry.py
```

### Comparing `ophyd_registry-1.2.0/PKG-INFO` & `ophyd_registry-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd-registry
-Version: 1.2.0
+Version: 1.2.1
 Summary: A registry to keep track of, and retrieve, Ophyd objects.
 Author-email: Mark Wolfman <wolfman@anl.gov>
 Project-URL: Homepage, https://github.com/spc-group/ophyd-registry
 Project-URL: Bug Tracker, https://github.com/spc-group/ophyd-registry/issues
 Keywords: synchrotron,xray,bluesky
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `ophyd_registry-1.2.0/README.md` & `ophyd_registry-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ophyd_registry-1.2.0/pyproject.toml` & `ophyd_registry-1.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ophyd-registry"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Mark Wolfman", email="wolfman@anl.gov" },
 ]
 description = "A registry to keep track of, and retrieve, Ophyd objects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ophyd_registry-1.2.0/src/ophyd_registry.egg-info/PKG-INFO` & `ophyd_registry-1.2.1/src/ophyd_registry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ophyd-registry
-Version: 1.2.0
+Version: 1.2.1
 Summary: A registry to keep track of, and retrieve, Ophyd objects.
 Author-email: Mark Wolfman <wolfman@anl.gov>
 Project-URL: Homepage, https://github.com/spc-group/ophyd-registry
 Project-URL: Bug Tracker, https://github.com/spc-group/ophyd-registry/issues
 Keywords: synchrotron,xray,bluesky
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `ophyd_registry-1.2.0/src/ophydregistry/registry.py` & `ophyd_registry-1.2.1/src/ophydregistry/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import logging
 import time
 import warnings
 from collections import OrderedDict
 from itertools import chain
-from typing import List, Mapping, Optional, Set
+from typing import Hashable, List, Mapping, Optional, Tuple
 from weakref import WeakSet, WeakValueDictionary
 
 from ophyd import ophydobj
 
+try:
+    from pcdsdevices.signal import _AggregateSignalState
+except ImportError:
+    _AggregateSignalState = ophydobj.OphydObject
+
 # Sentinal value for default parameters
 UNSET = object()
 
 
 try:
     import typhos
 except ImportError:
@@ -111,15 +116,15 @@
       collector, so to force cleanup use ``gc.collect()``.
 
     """
 
     use_typhos: bool
     keep_references: bool
     _auto_register: bool
-    _valid_classes: Set[type] = {ophydobj.OphydObject}
+    _valid_classes: Tuple[type] = (ophydobj.OphydObject, _AggregateSignalState)
 
     # components: Sequence
     _objects_by_name: Mapping
     _objects_by_label: Mapping
 
     def __init__(
         self,
@@ -191,19 +196,20 @@
             if default is not UNSET:
                 return default
             else:
                 raise
         # Remove from the list by name
         try:
             del self._objects_by_name[obj.name]
-        except KeyError:
+        except (KeyError, AttributeError):
             pass
         # Remove from the list by label
-        for objects in self._objects_by_label.values():
-            objects.discard(obj)
+        if isinstance(obj, Hashable):
+            for objects in self._objects_by_label.values():
+                objects.discard(obj)
         # Remove children from the lists as well
         sub_signals = getattr(obj, "_signals", {})
         for cpt_name, cpt in sub_signals.items():
             self.pop(cpt)
         return obj
 
     def clear(self, clear_typhos: bool = True):
@@ -342,17 +348,16 @@
         """Is the object already resolved into an ophyd device, etc.
 
         This method checks the type of the object. To extend this to
         other types of objects, override this objects
         ``_valid_classes`` attribute with a new set.
 
         """
-        for cls in self._valid_classes:
-            if isinstance(obj, cls):
-                return True
+        if isinstance(obj, self._valid_classes):
+            return True
         return False
 
     def _findall_by_label(self, label, allow_none):
         # Check for already created ophyd objects (return as is)
         if self._is_resolved(label):
             yield label
             return
```

### Comparing `ophyd_registry-1.2.0/src/ophydregistry/tests/test_instrument_registry.py` & `ophyd_registry-1.2.1/src/ophydregistry/tests/test_instrument_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from ophydregistry import ComponentNotFound, MultipleComponentsFound, Registry
 
 
 @pytest.fixture()
 def registry():
     reg = Registry(auto_register=False, use_typhos=False)
-    reg._valid_classes = {mock.MagicMock, *reg._valid_classes}
+    reg._valid_classes = (mock.MagicMock, *reg._valid_classes)
     try:
         yield reg
     finally:
         del reg
 
 
 def test_register_component(registry):
```

