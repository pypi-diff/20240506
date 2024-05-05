# Comparing `tmp/trame-vtklocal-0.3.0.tar.gz` & `tmp/trame-vtklocal-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-vtklocal-0.3.0.tar", last modified: Sun May  5 18:26:10 2024, max compression
+gzip compressed data, was "trame-vtklocal-0.3.1.tar", last modified: Sun May  5 19:09:32 2024, max compression
```

## Comparing `trame-vtklocal-0.3.0.tar` & `trame-vtklocal-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 18:26:10.137674 trame-vtklocal-0.3.0/
--rw-r--r--   0 root         (0) root         (0)      583 2024-05-05 18:25:46.000000 trame-vtklocal-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2024-05-05 18:25:46.000000 trame-vtklocal-0.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2433 2024-05-05 18:26:10.137674 trame-vtklocal-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1673 2024-05-05 18:25:46.000000 trame-vtklocal-0.3.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      896 2024-05-05 18:26:10.137674 trame-vtklocal-0.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 18:25:46.000000 trame-vtklocal-0.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 18:26:10.133674 trame-vtklocal-0.3.0/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-05 18:25:46.000000 trame-vtklocal-0.3.0/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 18:26:10.133674 trame-vtklocal-0.3.0/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-05 18:25:46.000000 trame-vtklocal-0.3.0/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       36 2024-05-05 18:25:46.000000 trame-vtklocal-0.3.0/trame/modules/vtklocal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 18:26:10.133674 trame-vtklocal-0.3.0/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-05 18:25:46.000000 trame-vtklocal-0.3.0/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      144 2024-05-05 18:25:46.000000 trame-vtklocal-0.3.0/trame/widgets/vtklocal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 18:26:10.133674 trame-vtklocal-0.3.0/trame_vtklocal/
--rw-r--r--   0 root         (0) root         (0)       96 2024-05-05 18:25:46.000000 trame-vtklocal-0.3.0/trame_vtklocal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 18:26:10.137674 trame-vtklocal-0.3.0/trame_vtklocal/module/
--rw-r--r--   0 root         (0) root         (0)      873 2024-05-05 18:25:46.000000 trame-vtklocal-0.3.0/trame_vtklocal/module/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4331 2024-05-05 18:25:46.000000 trame-vtklocal-0.3.0/trame_vtklocal/module/protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 18:26:10.133674 trame-vtklocal-0.3.0/trame_vtklocal/module/serve/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 18:26:10.137674 trame-vtklocal-0.3.0/trame_vtklocal/module/serve/js/
--rw-r--r--   0 root         (0) root         (0)     4135 2024-05-05 18:26:07.000000 trame-vtklocal-0.3.0/trame_vtklocal/module/serve/js/trame_vtklocal.umd.js
--rw-r--r--   0 root         (0) root         (0)     2109 2024-05-05 18:25:46.000000 trame-vtklocal-0.3.0/trame_vtklocal/module/wasm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 18:26:10.137674 trame-vtklocal-0.3.0/trame_vtklocal/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 18:25:46.000000 trame-vtklocal-0.3.0/trame_vtklocal/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4260 2024-05-05 18:25:46.000000 trame-vtklocal-0.3.0/trame_vtklocal/widgets/vtklocal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 18:26:10.137674 trame-vtklocal-0.3.0/trame_vtklocal.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2433 2024-05-05 18:26:10.000000 trame-vtklocal-0.3.0/trame_vtklocal.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      608 2024-05-05 18:26:10.000000 trame-vtklocal-0.3.0/trame_vtklocal.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 18:26:10.000000 trame-vtklocal-0.3.0/trame_vtklocal.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-05 18:26:10.000000 trame-vtklocal-0.3.0/trame_vtklocal.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-05 18:26:10.000000 trame-vtklocal-0.3.0/trame_vtklocal.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:09:32.802143 trame-vtklocal-0.3.1/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-05-05 19:09:09.000000 trame-vtklocal-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-05 19:09:09.000000 trame-vtklocal-0.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2433 2024-05-05 19:09:32.802143 trame-vtklocal-0.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-05-05 19:09:09.000000 trame-vtklocal-0.3.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)      896 2024-05-05 19:09:32.802143 trame-vtklocal-0.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 19:09:09.000000 trame-vtklocal-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:09:32.798143 trame-vtklocal-0.3.1/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-05 19:09:09.000000 trame-vtklocal-0.3.1/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:09:32.802143 trame-vtklocal-0.3.1/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-05 19:09:09.000000 trame-vtklocal-0.3.1/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       36 2024-05-05 19:09:09.000000 trame-vtklocal-0.3.1/trame/modules/vtklocal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:09:32.802143 trame-vtklocal-0.3.1/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-05 19:09:09.000000 trame-vtklocal-0.3.1/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      144 2024-05-05 19:09:09.000000 trame-vtklocal-0.3.1/trame/widgets/vtklocal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:09:32.802143 trame-vtklocal-0.3.1/trame_vtklocal/
+-rw-r--r--   0 root         (0) root         (0)       96 2024-05-05 19:09:09.000000 trame-vtklocal-0.3.1/trame_vtklocal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:09:32.802143 trame-vtklocal-0.3.1/trame_vtklocal/module/
+-rw-r--r--   0 root         (0) root         (0)      873 2024-05-05 19:09:09.000000 trame-vtklocal-0.3.1/trame_vtklocal/module/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4331 2024-05-05 19:09:09.000000 trame-vtklocal-0.3.1/trame_vtklocal/module/protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:09:32.798143 trame-vtklocal-0.3.1/trame_vtklocal/module/serve/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:09:32.802143 trame-vtklocal-0.3.1/trame_vtklocal/module/serve/js/
+-rw-r--r--   0 root         (0) root         (0)     4135 2024-05-05 19:09:29.000000 trame-vtklocal-0.3.1/trame_vtklocal/module/serve/js/trame_vtklocal.umd.js
+-rw-r--r--   0 root         (0) root         (0)     2148 2024-05-05 19:09:09.000000 trame-vtklocal-0.3.1/trame_vtklocal/module/wasm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:09:32.802143 trame-vtklocal-0.3.1/trame_vtklocal/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-05 19:09:09.000000 trame-vtklocal-0.3.1/trame_vtklocal/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4260 2024-05-05 19:09:09.000000 trame-vtklocal-0.3.1/trame_vtklocal/widgets/vtklocal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:09:32.802143 trame-vtklocal-0.3.1/trame_vtklocal.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2433 2024-05-05 19:09:32.000000 trame-vtklocal-0.3.1/trame_vtklocal.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      608 2024-05-05 19:09:32.000000 trame-vtklocal-0.3.1/trame_vtklocal.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 19:09:32.000000 trame-vtklocal-0.3.1/trame_vtklocal.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-05 19:09:32.000000 trame-vtklocal-0.3.1/trame_vtklocal.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-05 19:09:32.000000 trame-vtklocal-0.3.1/trame_vtklocal.egg-info/top_level.txt
```

### Comparing `trame-vtklocal-0.3.0/LICENSE` & `trame-vtklocal-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-vtklocal-0.3.0/PKG-INFO` & `trame-vtklocal-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtklocal
-Version: 0.3.0
+Version: 0.3.1
 Summary: VTK Local Rendering using WASM
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-vtklocal-0.3.0/README.rst` & `trame-vtklocal-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `trame-vtklocal-0.3.0/setup.cfg` & `trame-vtklocal-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-vtklocal
-version = 0.3.0
+version = 0.3.1
 description = VTK Local Rendering using WASM
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache Software License
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `trame-vtklocal-0.3.0/trame_vtklocal/module/__init__.py` & `trame-vtklocal-0.3.1/trame_vtklocal/module/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtklocal-0.3.0/trame_vtklocal/module/protocol.py` & `trame-vtklocal-0.3.1/trame_vtklocal/module/protocol.py`

 * *Files identical despite different names*

### Comparing `trame-vtklocal-0.3.0/trame_vtklocal/module/serve/js/trame_vtklocal.umd.js` & `trame-vtklocal-0.3.1/trame_vtklocal/module/serve/js/trame_vtklocal.umd.js`

 * *Files identical despite different names*

### Comparing `trame-vtklocal-0.3.0/trame_vtklocal/module/wasm.py` & `trame-vtklocal-0.3.1/trame_vtklocal/module/wasm.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
             async with session.get(url) as response:
                 data = await response.read()
                 if response.status == 404:
                     success = False
                 else:
                     with open(filename, "wb") as f:
                         f.write(data)
+                        success = True
                     break
         if not success:
             raise Exception("Invalid URLs " + ",".join(urls) + ". Got 404 response.")
 
 
 async def setup_wasm_directory(target_directory, wasm_urls):
     # Need to install wasm
```

### Comparing `trame-vtklocal-0.3.0/trame_vtklocal/widgets/vtklocal.py` & `trame-vtklocal-0.3.1/trame_vtklocal/widgets/vtklocal.py`

 * *Files identical despite different names*

### Comparing `trame-vtklocal-0.3.0/trame_vtklocal.egg-info/PKG-INFO` & `trame-vtklocal-0.3.1/trame_vtklocal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtklocal
-Version: 0.3.0
+Version: 0.3.1
 Summary: VTK Local Rendering using WASM
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-vtklocal-0.3.0/trame_vtklocal.egg-info/SOURCES.txt` & `trame-vtklocal-0.3.1/trame_vtklocal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

