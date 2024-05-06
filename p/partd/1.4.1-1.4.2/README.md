# Comparing `tmp/partd-1.4.1.tar.gz` & `tmp/partd-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partd-1.4.1.tar", last modified: Mon Sep 25 18:27:33 2023, max compression
+gzip compressed data, was "partd-1.4.2.tar", last modified: Mon May  6 19:50:58 2024, max compression
```

## Comparing `partd-1.4.1.tar` & `partd-1.4.2.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-09-25 18:27:33.096125 partd-1.4.1/
--rw-r--r--   0 james      (501) staff       (20)     1505 2023-07-17 20:01:26.000000 partd-1.4.1/LICENSE.txt
--rw-r--r--   0 james      (501) staff       (20)      179 2023-07-17 20:03:10.000000 partd-1.4.1/MANIFEST.in
--rw-r--r--   0 james      (501) staff       (20)     4405 2023-09-25 18:27:33.096185 partd-1.4.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     3824 2023-07-17 20:03:10.000000 partd-1.4.1/README.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-09-25 18:27:33.096574 partd-1.4.1/partd/
--rw-r--r--   0 james      (501) staff       (20)      507 2023-07-17 20:03:10.000000 partd-1.4.1/partd/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      497 2023-09-25 18:27:33.096609 partd-1.4.1/partd/_version.py
--rw-r--r--   0 james      (501) staff       (20)     3628 2023-07-17 20:03:10.000000 partd-1.4.1/partd/buffer.py
--rw-r--r--   0 james      (501) staff       (20)     1174 2023-07-17 20:03:10.000000 partd-1.4.1/partd/compressed.py
--rw-r--r--   0 james      (501) staff       (20)     2259 2023-07-17 20:03:10.000000 partd-1.4.1/partd/core.py
--rw-r--r--   0 james      (501) staff       (20)     1701 2023-07-17 20:01:26.000000 partd-1.4.1/partd/dict.py
--rw-r--r--   0 james      (501) staff       (20)     1287 2023-07-17 20:01:26.000000 partd-1.4.1/partd/encode.py
--rw-r--r--   0 james      (501) staff       (20)     3954 2023-07-17 20:03:10.000000 partd-1.4.1/partd/file.py
--rw-r--r--   0 james      (501) staff       (20)     4181 2023-07-17 20:03:10.000000 partd-1.4.1/partd/numpy.py
--rw-r--r--   0 james      (501) staff       (20)     6931 2023-07-17 20:03:10.000000 partd-1.4.1/partd/pandas.py
--rw-r--r--   0 james      (501) staff       (20)      360 2023-07-17 20:03:10.000000 partd-1.4.1/partd/pickle.py
--rw-r--r--   0 james      (501) staff       (20)      902 2023-07-17 20:03:10.000000 partd-1.4.1/partd/python.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-09-25 18:27:33.095981 partd-1.4.1/partd/tests/
--rw-r--r--   0 james      (501) staff       (20)     1560 2023-07-17 20:01:26.000000 partd-1.4.1/partd/tests/test_buffer.py
--rw-r--r--   0 james      (501) staff       (20)      734 2023-07-17 20:01:26.000000 partd-1.4.1/partd/tests/test_compressed.py
--rw-r--r--   0 james      (501) staff       (20)      940 2023-07-17 20:01:26.000000 partd-1.4.1/partd/tests/test_dict.py
--rw-r--r--   0 james      (501) staff       (20)      700 2023-07-17 20:01:26.000000 partd-1.4.1/partd/tests/test_encode.py
--rw-r--r--   0 james      (501) staff       (20)     1800 2023-07-17 20:01:26.000000 partd-1.4.1/partd/tests/test_file.py
--rw-r--r--   0 james      (501) staff       (20)     2307 2023-07-17 20:03:10.000000 partd-1.4.1/partd/tests/test_numpy.py
--rw-r--r--   0 james      (501) staff       (20)     4849 2023-07-17 20:03:10.000000 partd-1.4.1/partd/tests/test_pandas.py
--rw-r--r--   0 james      (501) staff       (20)     1281 2023-07-17 20:01:26.000000 partd-1.4.1/partd/tests/test_partd.py
--rw-r--r--   0 james      (501) staff       (20)      762 2023-07-17 20:01:26.000000 partd-1.4.1/partd/tests/test_pickle.py
--rw-r--r--   0 james      (501) staff       (20)      248 2023-07-17 20:01:26.000000 partd-1.4.1/partd/tests/test_python.py
--rw-r--r--   0 james      (501) staff       (20)      258 2023-07-17 20:01:26.000000 partd-1.4.1/partd/tests/test_utils.py
--rw-r--r--   0 james      (501) staff       (20)     3335 2023-07-17 20:03:10.000000 partd-1.4.1/partd/tests/test_zmq.py
--rw-r--r--   0 james      (501) staff       (20)     3603 2023-07-17 20:03:10.000000 partd-1.4.1/partd/utils.py
--rw-r--r--   0 james      (501) staff       (20)     9578 2023-07-17 20:03:10.000000 partd-1.4.1/partd/zmq.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-09-25 18:27:33.093924 partd-1.4.1/partd.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     4405 2023-09-25 18:27:33.000000 partd-1.4.1/partd.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      795 2023-09-25 18:27:33.000000 partd-1.4.1/partd.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-09-25 18:27:33.000000 partd-1.4.1/partd.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-09-25 18:27:33.000000 partd-1.4.1/partd.egg-info/not-zip-safe
--rw-r--r--   0 james      (501) staff       (20)       65 2023-09-25 18:27:33.000000 partd-1.4.1/partd.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)        6 2023-09-25 18:27:33.000000 partd-1.4.1/partd.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       13 2023-07-17 20:01:26.000000 partd-1.4.1/requirements.txt
--rw-r--r--   0 james      (501) staff       (20)      194 2023-09-25 18:27:33.096427 partd-1.4.1/setup.cfg
--rwxr-xr-x   0 james      (501) staff       (20)     1159 2023-09-25 18:24:29.000000 partd-1.4.1/setup.py
--rw-r--r--   0 james      (501) staff       (20)    68607 2023-09-25 17:19:27.000000 partd-1.4.1/versioneer.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-06 19:50:58.921352 partd-1.4.2/
+-rw-r--r--   0 james      (501) staff       (20)     1505 2023-07-17 20:01:26.000000 partd-1.4.2/LICENSE.txt
+-rw-r--r--   0 james      (501) staff       (20)      154 2024-05-06 19:16:04.000000 partd-1.4.2/MANIFEST.in
+-rw-r--r--   0 james      (501) staff       (20)     4620 2024-05-06 19:50:58.921076 partd-1.4.2/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     3824 2023-07-17 20:03:10.000000 partd-1.4.2/README.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-06 19:50:58.917140 partd-1.4.2/partd/
+-rw-r--r--   0 james      (501) staff       (20)      487 2024-05-06 19:16:04.000000 partd-1.4.2/partd/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      497 2024-05-06 19:50:58.921528 partd-1.4.2/partd/_version.py
+-rw-r--r--   0 james      (501) staff       (20)     3628 2023-07-17 20:03:10.000000 partd-1.4.2/partd/buffer.py
+-rw-r--r--   0 james      (501) staff       (20)     1174 2023-07-17 20:03:10.000000 partd-1.4.2/partd/compressed.py
+-rw-r--r--   0 james      (501) staff       (20)     2259 2023-07-17 20:03:10.000000 partd-1.4.2/partd/core.py
+-rw-r--r--   0 james      (501) staff       (20)     1701 2023-07-17 20:01:26.000000 partd-1.4.2/partd/dict.py
+-rw-r--r--   0 james      (501) staff       (20)     1287 2023-07-17 20:01:26.000000 partd-1.4.2/partd/encode.py
+-rw-r--r--   0 james      (501) staff       (20)     3954 2023-07-17 20:03:10.000000 partd-1.4.2/partd/file.py
+-rw-r--r--   0 james      (501) staff       (20)     4181 2023-07-17 20:03:10.000000 partd-1.4.2/partd/numpy.py
+-rw-r--r--   0 james      (501) staff       (20)     7319 2024-05-06 19:38:30.000000 partd-1.4.2/partd/pandas.py
+-rw-r--r--   0 james      (501) staff       (20)      360 2023-07-17 20:03:10.000000 partd-1.4.2/partd/pickle.py
+-rw-r--r--   0 james      (501) staff       (20)      902 2023-07-17 20:03:10.000000 partd-1.4.2/partd/python.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-06 19:50:58.920280 partd-1.4.2/partd/tests/
+-rw-r--r--   0 james      (501) staff       (20)     1560 2023-07-17 20:01:26.000000 partd-1.4.2/partd/tests/test_buffer.py
+-rw-r--r--   0 james      (501) staff       (20)      734 2023-07-17 20:01:26.000000 partd-1.4.2/partd/tests/test_compressed.py
+-rw-r--r--   0 james      (501) staff       (20)      940 2023-07-17 20:01:26.000000 partd-1.4.2/partd/tests/test_dict.py
+-rw-r--r--   0 james      (501) staff       (20)      700 2023-07-17 20:01:26.000000 partd-1.4.2/partd/tests/test_encode.py
+-rw-r--r--   0 james      (501) staff       (20)     1800 2023-07-17 20:01:26.000000 partd-1.4.2/partd/tests/test_file.py
+-rw-r--r--   0 james      (501) staff       (20)     2307 2023-07-17 20:03:10.000000 partd-1.4.2/partd/tests/test_numpy.py
+-rw-r--r--   0 james      (501) staff       (20)     4849 2023-07-17 20:03:10.000000 partd-1.4.2/partd/tests/test_pandas.py
+-rw-r--r--   0 james      (501) staff       (20)     1281 2023-07-17 20:01:26.000000 partd-1.4.2/partd/tests/test_partd.py
+-rw-r--r--   0 james      (501) staff       (20)      762 2023-07-17 20:01:26.000000 partd-1.4.2/partd/tests/test_pickle.py
+-rw-r--r--   0 james      (501) staff       (20)      248 2023-07-17 20:01:26.000000 partd-1.4.2/partd/tests/test_python.py
+-rw-r--r--   0 james      (501) staff       (20)      258 2023-07-17 20:01:26.000000 partd-1.4.2/partd/tests/test_utils.py
+-rw-r--r--   0 james      (501) staff       (20)     3335 2023-07-17 20:03:10.000000 partd-1.4.2/partd/tests/test_zmq.py
+-rw-r--r--   0 james      (501) staff       (20)     3603 2023-07-17 20:03:10.000000 partd-1.4.2/partd/utils.py
+-rw-r--r--   0 james      (501) staff       (20)     9578 2023-07-17 20:03:10.000000 partd-1.4.2/partd/zmq.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-06 19:50:58.920489 partd-1.4.2/partd.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     4620 2024-05-06 19:50:58.000000 partd-1.4.2/partd.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      769 2024-05-06 19:50:58.000000 partd-1.4.2/partd.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2024-05-06 19:50:58.000000 partd-1.4.2/partd.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2024-05-06 19:50:58.000000 partd-1.4.2/partd.egg-info/not-zip-safe
+-rw-r--r--   0 james      (501) staff       (20)       63 2024-05-06 19:50:58.000000 partd-1.4.2/partd.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)        6 2024-05-06 19:50:58.000000 partd-1.4.2/partd.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)     1183 2024-05-06 19:38:30.000000 partd-1.4.2/pyproject.toml
+-rw-r--r--   0 james      (501) staff       (20)       38 2024-05-06 19:50:58.921416 partd-1.4.2/setup.cfg
+-rwxr-xr-x   0 james      (501) staff       (20)      194 2024-05-06 19:16:04.000000 partd-1.4.2/setup.py
```

### Comparing `partd-1.4.1/LICENSE.txt` & `partd-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/PKG-INFO` & `partd-1.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: partd
-Version: 1.4.1
+Version: 1.4.2
 Summary: Appendable key-value storage
-Home-page: http://github.com/dask/partd/
-Maintainer: Matthew Rocklin
-Maintainer-email: mrocklin@gmail.com
+Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD
+Project-URL: Homepage, http://github.com/dask/partd/
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Provides-Extra: complete
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: locket
+Requires-Dist: toolz
+Provides-Extra: complete
+Requires-Dist: numpy>=1.20.0; extra == "complete"
+Requires-Dist: pandas>=1.3; extra == "complete"
+Requires-Dist: pyzmq; extra == "complete"
+Requires-Dist: blosc; extra == "complete"
 
 PartD
 =====
 
 |Build Status| |Version Status|
 
 Key-value byte store with appendable values
```

### Comparing `partd-1.4.1/README.rst` & `partd-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/buffer.py` & `partd-1.4.2/partd/buffer.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/compressed.py` & `partd-1.4.2/partd/compressed.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/core.py` & `partd-1.4.2/partd/core.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/dict.py` & `partd-1.4.2/partd/dict.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/encode.py` & `partd-1.4.2/partd/encode.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/file.py` & `partd-1.4.2/partd/file.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/numpy.py` & `partd-1.4.2/partd/numpy.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/pandas.py` & `partd-1.4.2/partd/pandas.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 from functools import partial
 import pickle
 
-import numpy as np
 import pandas as pd
-from pandas.core.internals import create_block_manager_from_blocks, make_block
+from packaging.version import Version
+
+PANDAS_GE_210 = Version(pd.__version__).release >= (2, 1, 0)
+PANDAS_GE_300 =  Version(pd.__version__).major >= 3
+
+if PANDAS_GE_300:
+    from pandas.api.internals import create_dataframe_from_blocks
+    create_block_manager_from_blocks = None
+    make_block = None
+else:
+    create_dataframe_from_blocks = None
+    try:
+        from pandas.core.internals.managers import create_block_manager_from_blocks
+    except ImportError:
+        from pandas.core.internals import create_block_manager_from_blocks
+
+    from pandas.core.internals import make_block
 
 from . import numpy as pnp
 from .core import Interface
 from .encode import Encode
 from .utils import extend, framesplit, frame
+from pandas.api.types import is_extension_array_dtype
+from pandas.api.extensions import ExtensionArray
 
-try:
-    # pandas >= 0.24.0
-    from pandas.api.types import is_extension_array_dtype
-except ImportError:
-    def is_extension_array_dtype(dtype):
-        return False
-
-try:
-    # Some `ExtensionArray`s can have a `.dtype` which is not a `ExtensionDtype`
-    # (e.g. they can be backed by a NumPy dtype). For these cases we check
-    # whether the instance is a `ExtensionArray`.
-    # https://github.com/dask/partd/issues/48
-    from pandas.api.extensions import ExtensionArray
-    def is_extension_array(x):
-        return isinstance(x, ExtensionArray)
-except ImportError:
-    def is_extension_array(x):
-        return False
+def is_extension_array(x):
+    return isinstance(x, ExtensionArray)
 
 
 dumps = partial(pickle.dumps, protocol=pickle.HIGHEST_PROTOCOL)
 
 
+
 class PandasColumns(Interface):
     def __init__(self, partd=None):
         self.partd = pnp.Numpy(partd)
         Interface.__init__(self)
 
     def append(self, data, **kwargs):
         for k, df in data.items():
@@ -144,15 +146,15 @@
     if extension == ("other", ()):
         bytes = pickle.dumps(values)
     else:
         bytes = pnp.compress(pnp.serialize(values), values.dtype)
     return header, bytes
 
 
-def block_from_header_bytes(header, bytes):
+def block_from_header_bytes(header, bytes, create_block: bool):
     placement, dtype, shape, (extension_type, extension_values) = header
 
     if extension_type == "other":
         values = pickle.loads(bytes)
     else:
         values = pnp.deserialize(pnp.decompress(bytes, dtype), dtype,
                                  copy=True).reshape(shape)
@@ -160,15 +162,17 @@
         values = pd.Categorical.from_codes(values,
                                            extension_values[1],
                                            ordered=extension_values[0])
     elif extension_type == 'datetime64_tz_type':
         tz_info = extension_values[0]
         values = pd.DatetimeIndex(values).tz_localize('utc').tz_convert(
             tz_info)
-    return make_block(values, placement=placement)
+    if create_block:
+        return make_block(values, placement=placement)
+    return values, placement
 
 
 def serialize(df):
     """ Serialize and compress a Pandas DataFrame
 
     Uses Pandas blocks, snappy, and blosc to deconstruct an array into bytes
     """
@@ -189,17 +193,22 @@
 def deserialize(bytes):
     """ Deserialize and decompress bytes back to a pandas DataFrame """
     frames = list(framesplit(bytes))
     headers = pickle.loads(frames[0])
     bytes = frames[1:]
     axes = [index_from_header_bytes(headers[0], bytes[0]),
             index_from_header_bytes(headers[1], bytes[1])]
-    blocks = [block_from_header_bytes(h, b)
+    blocks = [block_from_header_bytes(h, b, create_block=not PANDAS_GE_300)
               for (h, b) in zip(headers[2:], bytes[2:])]
-    return pd.DataFrame(create_block_manager_from_blocks(blocks, axes))
+    if PANDAS_GE_300:
+        return pd.api.internals.create_dataframe_from_blocks(blocks, axes[1], axes[0])
+    elif PANDAS_GE_210:
+        return pd.DataFrame._from_mgr(create_block_manager_from_blocks(blocks, axes), axes=axes)
+    else:
+        return pd.DataFrame(create_block_manager_from_blocks(blocks, axes))
 
 
 def join(dfs):
     if not dfs:
         return pd.DataFrame()
     else:
         return pd.concat(dfs)
```

### Comparing `partd-1.4.1/partd/python.py` & `partd-1.4.2/partd/python.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/tests/test_buffer.py` & `partd-1.4.2/partd/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/tests/test_compressed.py` & `partd-1.4.2/partd/tests/test_compressed.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/tests/test_dict.py` & `partd-1.4.2/partd/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/tests/test_encode.py` & `partd-1.4.2/partd/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/tests/test_file.py` & `partd-1.4.2/partd/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/tests/test_numpy.py` & `partd-1.4.2/partd/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/tests/test_pandas.py` & `partd-1.4.2/partd/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/tests/test_partd.py` & `partd-1.4.2/partd/tests/test_partd.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/tests/test_pickle.py` & `partd-1.4.2/partd/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/tests/test_zmq.py` & `partd-1.4.2/partd/tests/test_zmq.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/utils.py` & `partd-1.4.2/partd/utils.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd/zmq.py` & `partd-1.4.2/partd/zmq.py`

 * *Files identical despite different names*

### Comparing `partd-1.4.1/partd.egg-info/PKG-INFO` & `partd-1.4.2/partd.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: partd
-Version: 1.4.1
+Version: 1.4.2
 Summary: Appendable key-value storage
-Home-page: http://github.com/dask/partd/
-Maintainer: Matthew Rocklin
-Maintainer-email: mrocklin@gmail.com
+Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD
+Project-URL: Homepage, http://github.com/dask/partd/
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Provides-Extra: complete
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: locket
+Requires-Dist: toolz
+Provides-Extra: complete
+Requires-Dist: numpy>=1.20.0; extra == "complete"
+Requires-Dist: pandas>=1.3; extra == "complete"
+Requires-Dist: pyzmq; extra == "complete"
+Requires-Dist: blosc; extra == "complete"
 
 PartD
 =====
 
 |Build Status| |Version Status|
 
 Key-value byte store with appendable values
```

### Comparing `partd-1.4.1/partd.egg-info/SOURCES.txt` & `partd-1.4.2/partd.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
-requirements.txt
-setup.cfg
+pyproject.toml
 setup.py
-versioneer.py
 partd/__init__.py
 partd/_version.py
 partd/buffer.py
 partd/compressed.py
 partd/core.py
 partd/dict.py
 partd/encode.py
```

