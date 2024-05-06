# Comparing `tmp/metatensor-core-0.1.5.tar.gz` & `tmp/metatensor_core-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metatensor-core-0.1.5.tar", last modified: Tue Apr  9 14:00:51 2024, max compression
+gzip compressed data, was "metatensor_core-0.1.6.tar", last modified: Mon May  6 09:29:45 2024, max compression
```

## Comparing `metatensor-core-0.1.5.tar` & `metatensor_core-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:00:51.744420 metatensor-core-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-09 14:00:37.000000 metatensor-core-0.1.5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-09 14:00:37.000000 metatensor-core-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-09 14:00:51.744420 metatensor-core-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:00:51.740420 metatensor-core-0.1.5/metatensor/
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/_c_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/_c_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18074 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:00:51.740420 metatensor-core-0.1.5/metatensor/data/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/data/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/data/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    17374 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    38710 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/status.py
--rw-r--r--   0 runner    (1001) docker     (127)    28174 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/metatensor/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    86573 2024-04-09 14:00:51.000000 metatensor-core-0.1.5/metatensor-core-cxx-0.1.5.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:00:51.744420 metatensor-core-0.1.5/metatensor_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-09 14:00:51.000000 metatensor-core-0.1.5/metatensor_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-09 14:00:51.000000 metatensor-core-0.1.5/metatensor_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:00:51.000000 metatensor-core-0.1.5/metatensor_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:00:50.000000 metatensor-core-0.1.5/metatensor_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 14:00:51.000000 metatensor-core-0.1.5/metatensor_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 14:00:51.000000 metatensor-core-0.1.5/metatensor_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:00:50.000000 metatensor-core-0.1.5/n_commits_since_last_tag
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:00:51.744420 metatensor-core-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-09 14:00:38.000000 metatensor-core-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:29:45.843831 metatensor_core-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-06 09:29:45.843831 metatensor_core-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:29:45.843831 metatensor_core-0.1.6/metatensor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/metatensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/metatensor/_c_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/metatensor/_c_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18074 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/metatensor/block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:29:45.843831 metatensor_core-0.1.6/metatensor/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/metatensor/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9869 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/metatensor/data/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/metatensor/data/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17374 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/metatensor/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38710 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/metatensor/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/metatensor/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28174 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/metatensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/metatensor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/metatensor/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85281 2024-05-06 09:29:45.000000 metatensor_core-0.1.6/metatensor-core-cxx-0.1.6.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:29:45.843831 metatensor_core-0.1.6/metatensor_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-06 09:29:45.000000 metatensor_core-0.1.6/metatensor_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-06 09:29:45.000000 metatensor_core-0.1.6/metatensor_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:29:45.000000 metatensor_core-0.1.6/metatensor_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:29:44.000000 metatensor_core-0.1.6/metatensor_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 09:29:45.000000 metatensor_core-0.1.6/metatensor_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 09:29:45.000000 metatensor_core-0.1.6/metatensor_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:29:44.000000 metatensor_core-0.1.6/n_commits_since_last_tag
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:29:45.843831 metatensor_core-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-05-06 09:29:32.000000 metatensor_core-0.1.6/setup.py
```

### Comparing `metatensor-core-0.1.5/LICENSE` & `metatensor_core-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.5/PKG-INFO` & `metatensor_core-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metatensor-core
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python bindings for metatensor
 Author: Guillaume Fraux, Davide Tisi, Philip Loche, Joseph W. Abbott, Jigyasa Nigam, Chiheb Ben Mahmoud
 License: BSD-3-Clause
 Project-URL: homepage, https://lab-cosmo.github.io/metatensor/latest/
 Project-URL: documentation, https://lab-cosmo.github.io/metatensor/latest/
 Project-URL: repository, https://github.com/lab-cosmo/metatensor
 Project-URL: changelog, https://lab-cosmo.github.io/metatensor/latest/core/CHANGELOG.html
```

### Comparing `metatensor-core-0.1.5/metatensor/__init__.py` & `metatensor_core-0.1.6/metatensor/__init__.py`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.5/metatensor/_c_api.py` & `metatensor_core-0.1.6/metatensor/_c_api.py`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.5/metatensor/_c_lib.py` & `metatensor_core-0.1.6/metatensor/_c_lib.py`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.5/metatensor/block.py` & `metatensor_core-0.1.6/metatensor/block.py`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.5/metatensor/data/array.py` & `metatensor_core-0.1.6/metatensor/data/array.py`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.5/metatensor/data/extract.py` & `metatensor_core-0.1.6/metatensor/data/extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,54 +14,54 @@
 
     HAS_TORCH = True
 except ImportError:
     HAS_TORCH = False
 
 
 if HAS_TORCH:
-    # This NewType is only used for typechecking and documentation purposes
+    # This NewType is only used for typechecking and documentation purposes. If you are
+    # trying to add support for new array types, see `data.array.ArrayWrapper` instead.
     Array = NewType("Array", Union[np.ndarray, torch.Tensor])
 else:
     Array = NewType("Array", np.ndarray)
 
 Array.__doc__ = """
-An ``Array`` contains the actual data stored in a
-:py:class:`metatensor.TensorBlock`.
+An ``Array`` contains the actual data stored in a :py:class:`metatensor.TensorBlock`.
 
-This data is manipulated by ``metatensor`` in a completely opaque way: this
-library does not know what's inside the arrays appart from a small set of
-constrains:
+This data is manipulated by ``metatensor`` in a completely opaque way: this library does
+not know what's inside the arrays appart from a small set of constrains:
 
-- the array contains numeric data (loading and saving
-  :py:class:`metatensor.TensorMap` additionally assumes arrays of 64-bit IEEE-754
+- the array contains numeric data (:py:func:`metatensor.load` and
+  :py:func:`metatensor.save` additionally requires contiguous arrays of 64-bit IEEE-754
   floating points numbers);
 - they are stored as row-major, n-dimensional arrays with at least 2 dimensions;
 - it is possible to create new arrays and move data from one array to another.
 
-The actual type of an ``Array`` depends on how the
-:py:class:`metatensor.TensorBlock` was created. Currently,
-:py:class:`numpy.ndarray` and :py:class:`torch.Tensor` are supported.
+The actual type of an ``Array`` depends on how the :py:class:`metatensor.TensorBlock`
+was created. Currently, :py:class:`numpy.ndarray` and :py:class:`torch.Tensor` are
+supported.
 """
 
 
 _ADDITIONAL_ORIGINS = {}
 
 
 def register_external_data_wrapper(origin, klass):
     """
     Register a non-Python data origin and the corresponding class wrapper.
 
-    The wrapper class constructor must take two arguments (raw ``mts_array`` and
-    python ``parent`` object) and return a subclass of either
-    :py:class:`numpy.ndarray` or :py:class:`torch.Tensor`, which keeps
-    ``parent`` alive. The :py:class:`metatensor.data.ExternalCpuArray` class
-    should provide the right behavior for data living in CPU memory, and can
-    serve as an example for more advanced custom arrays.
+    The wrapper class constructor must take two arguments (raw ``mts_array`` and python
+    ``parent`` object) and return a subclass of either :py:class:`numpy.ndarray` or
+    :py:class:`torch.Tensor`, which keeps ``parent`` alive. The
+    :py:class:`metatensor.data.ExternalCpuArray` class should provide the right behavior
+    for data living in CPU memory, and can serve as an example for more advanced custom
+    arrays.
 
-    :param origin: new origin to register as a string
+    :param origin: data origin name as a string, corresponding to the output of
+        :c:func:`mts_array_t.origin`
     :param klass: wrapper class to use for this origin
     """
 
     if not isinstance(origin, str):
         raise ValueError(f"origin must be a string, got {type(origin)}")
 
     global _ADDITIONAL_ORIGINS
```

### Comparing `metatensor-core-0.1.5/metatensor/io.py` & `metatensor_core-0.1.6/metatensor/io.py`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.5/metatensor/labels.py` & `metatensor_core-0.1.6/metatensor/labels.py`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.5/metatensor/status.py` & `metatensor_core-0.1.6/metatensor/status.py`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.5/metatensor/tensor.py` & `metatensor_core-0.1.6/metatensor/tensor.py`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.5/metatensor/utils.py` & `metatensor_core-0.1.6/metatensor/utils.py`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.5/metatensor_core.egg-info/PKG-INFO` & `metatensor_core-0.1.6/metatensor_core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metatensor-core
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python bindings for metatensor
 Author: Guillaume Fraux, Davide Tisi, Philip Loche, Joseph W. Abbott, Jigyasa Nigam, Chiheb Ben Mahmoud
 License: BSD-3-Clause
 Project-URL: homepage, https://lab-cosmo.github.io/metatensor/latest/
 Project-URL: documentation, https://lab-cosmo.github.io/metatensor/latest/
 Project-URL: repository, https://github.com/lab-cosmo/metatensor
 Project-URL: changelog, https://lab-cosmo.github.io/metatensor/latest/core/CHANGELOG.html
```

### Comparing `metatensor-core-0.1.5/metatensor_core.egg-info/SOURCES.txt` & `metatensor_core-0.1.6/metatensor_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.rst
-metatensor-core-cxx-0.1.5.tar.gz
+metatensor-core-cxx-0.1.6.tar.gz
 n_commits_since_last_tag
 pyproject.toml
 setup.py
 metatensor/__init__.py
 metatensor/_c_api.py
 metatensor/_c_lib.py
 metatensor/block.py
```

### Comparing `metatensor-core-0.1.5/pyproject.toml` & `metatensor_core-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `metatensor-core-0.1.5/setup.py` & `metatensor_core-0.1.6/setup.py`

 * *Files identical despite different names*

