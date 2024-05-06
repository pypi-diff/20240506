# Comparing `tmp/girona_donostia-0.1.8.tar.gz` & `tmp/girona_donostia-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girona_donostia-0.1.8.tar", last modified: Mon Aug 28 19:42:58 2023, max compression
+gzip compressed data, was "girona_donostia-0.1.9.tar", last modified: Mon May  6 14:02:18 2024, max compression
```

## Comparing `girona_donostia-0.1.8.tar` & `girona_donostia-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 petrumilev   (501) staff       (20)        0 2023-08-28 19:42:58.708046 girona_donostia-0.1.8/
--rw-r--r--   0 petrumilev   (501) staff       (20)     1067 2023-08-17 14:38:39.000000 girona_donostia-0.1.8/LICENSE
--rw-r--r--   0 petrumilev   (501) staff       (20)     2093 2023-08-28 19:42:58.707913 girona_donostia-0.1.8/PKG-INFO
--rw-r--r--   0 petrumilev   (501) staff       (20)      300 2023-08-17 13:09:34.000000 girona_donostia-0.1.8/README.md
-drwxr-xr-x   0 petrumilev   (501) staff       (20)        0 2023-08-28 19:42:58.706964 girona_donostia-0.1.8/girona_donostia/
--rw-r--r--   0 petrumilev   (501) staff       (20)      601 2023-08-28 19:42:00.000000 girona_donostia-0.1.8/girona_donostia/__init__.py
--rw-r--r--   0 petrumilev   (501) staff       (20)     2219 2023-08-28 08:53:47.000000 girona_donostia-0.1.8/girona_donostia/curve_fit.py
--rw-r--r--   0 petrumilev   (501) staff       (20)   117499 2023-08-28 14:20:07.000000 girona_donostia-0.1.8/girona_donostia/functions_for_library.py
--rw-r--r--   0 petrumilev   (501) staff       (20)     6295 2023-08-28 08:50:57.000000 girona_donostia-0.1.8/girona_donostia/objects_for_library.py
--rw-r--r--   0 petrumilev   (501) staff       (20)     7156 2023-08-28 19:36:52.000000 girona_donostia-0.1.8/girona_donostia/romberg.py
--rw-r--r--   0 petrumilev   (501) staff       (20)      869 2023-08-28 09:28:27.000000 girona_donostia-0.1.8/girona_donostia/statistic.py
-drwxr-xr-x   0 petrumilev   (501) staff       (20)        0 2023-08-28 19:42:58.707719 girona_donostia-0.1.8/girona_donostia.egg-info/
--rw-r--r--   0 petrumilev   (501) staff       (20)     2093 2023-08-28 19:42:58.000000 girona_donostia-0.1.8/girona_donostia.egg-info/PKG-INFO
--rw-r--r--   0 petrumilev   (501) staff       (20)      428 2023-08-28 19:42:58.000000 girona_donostia-0.1.8/girona_donostia.egg-info/SOURCES.txt
--rw-r--r--   0 petrumilev   (501) staff       (20)        1 2023-08-28 19:42:58.000000 girona_donostia-0.1.8/girona_donostia.egg-info/dependency_links.txt
--rw-r--r--   0 petrumilev   (501) staff       (20)       12 2023-08-28 19:42:58.000000 girona_donostia-0.1.8/girona_donostia.egg-info/requires.txt
--rw-r--r--   0 petrumilev   (501) staff       (20)       16 2023-08-28 19:42:58.000000 girona_donostia-0.1.8/girona_donostia.egg-info/top_level.txt
--rw-r--r--   0 petrumilev   (501) staff       (20)      628 2023-08-28 19:41:56.000000 girona_donostia-0.1.8/pyproject.toml
--rw-r--r--   0 petrumilev   (501) staff       (20)       38 2023-08-28 19:42:58.708096 girona_donostia-0.1.8/setup.cfg
--rw-r--r--   0 petrumilev   (501) staff       (20)      793 2023-08-28 19:41:58.000000 girona_donostia-0.1.8/setup.py
+drwxr-xr-x   0 petrumilev   (501) staff       (20)        0 2024-05-06 14:02:18.328653 girona_donostia-0.1.9/
+-rw-r--r--   0 petrumilev   (501) staff       (20)     1068 2024-05-06 13:57:09.000000 girona_donostia-0.1.9/LICENSE
+-rw-r--r--   0 petrumilev   (501) staff       (20)     2198 2024-05-06 14:02:18.328435 girona_donostia-0.1.9/PKG-INFO
+-rw-r--r--   0 petrumilev   (501) staff       (20)      355 2023-09-20 21:10:21.000000 girona_donostia-0.1.9/README.md
+drwxr-xr-x   0 petrumilev   (501) staff       (20)        0 2024-05-06 14:02:18.327128 girona_donostia-0.1.9/girona_donostia/
+-rw-r--r--   0 petrumilev   (501) staff       (20)      601 2023-08-28 19:50:43.000000 girona_donostia-0.1.9/girona_donostia/__init__.py
+-rw-r--r--   0 petrumilev   (501) staff       (20)     2219 2023-08-28 08:53:47.000000 girona_donostia-0.1.9/girona_donostia/curve_fit.py
+-rw-r--r--   0 petrumilev   (501) staff       (20)   117499 2023-08-28 14:20:07.000000 girona_donostia-0.1.9/girona_donostia/functions_for_library.py
+-rw-r--r--   0 petrumilev   (501) staff       (20)     6295 2023-08-28 08:50:57.000000 girona_donostia-0.1.9/girona_donostia/objects_for_library.py
+-rw-r--r--   0 petrumilev   (501) staff       (20)     7156 2023-08-28 19:36:52.000000 girona_donostia-0.1.9/girona_donostia/romberg.py
+-rw-r--r--   0 petrumilev   (501) staff       (20)      869 2023-08-28 09:28:27.000000 girona_donostia-0.1.9/girona_donostia/statistic.py
+drwxr-xr-x   0 petrumilev   (501) staff       (20)        0 2024-05-06 14:02:18.328180 girona_donostia-0.1.9/girona_donostia.egg-info/
+-rw-r--r--   0 petrumilev   (501) staff       (20)     2198 2024-05-06 14:02:18.000000 girona_donostia-0.1.9/girona_donostia.egg-info/PKG-INFO
+-rw-r--r--   0 petrumilev   (501) staff       (20)      428 2024-05-06 14:02:18.000000 girona_donostia-0.1.9/girona_donostia.egg-info/SOURCES.txt
+-rw-r--r--   0 petrumilev   (501) staff       (20)        1 2024-05-06 14:02:18.000000 girona_donostia-0.1.9/girona_donostia.egg-info/dependency_links.txt
+-rw-r--r--   0 petrumilev   (501) staff       (20)       12 2024-05-06 14:02:18.000000 girona_donostia-0.1.9/girona_donostia.egg-info/requires.txt
+-rw-r--r--   0 petrumilev   (501) staff       (20)       16 2024-05-06 14:02:18.000000 girona_donostia-0.1.9/girona_donostia.egg-info/top_level.txt
+-rw-r--r--   0 petrumilev   (501) staff       (20)      628 2024-05-06 14:00:03.000000 girona_donostia-0.1.9/pyproject.toml
+-rw-r--r--   0 petrumilev   (501) staff       (20)       38 2024-05-06 14:02:18.328765 girona_donostia-0.1.9/setup.cfg
+-rw-r--r--   0 petrumilev   (501) staff       (20)      794 2024-05-06 13:59:57.000000 girona_donostia-0.1.9/setup.py
```

### Comparing `girona_donostia-0.1.8/LICENSE` & `girona_donostia-0.1.9/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Petru Milev
+Copyright (c) 2024 Petru Milev
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `girona_donostia-0.1.8/PKG-INFO` & `girona_donostia-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: girona_donostia
-Version: 0.1.8
+Version: 0.1.9
 Summary: A small package to work with nonlinear optical propreties
 Home-page: https://github.com/Petru-Milev/Girona_Donostia
 Author: Petru Milev
 Author-email: Petru Milev <petia.md36@gmail.com>
 License: MIT License
         
-        Copyright (c) 2023 Petru Milev
+        Copyright (c) 2024 Petru Milev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -22,23 +22,27 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+        
 Project-URL: Homepage, https://github.com/Petru-Milev/Girona_Donostia
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
 
 # Girona_Donostia
 
 This is a source for a Python Library to study nonlinear optical propreties using Gaussian. 
 So far, this library can create a variety of Gaussian Input Files, and analize the output files (.log and .fchk files)
 
-Main Functionality is described in the Manual. 
+Main Functionality is described on the wiki page.
+https://github.com/Petru-Milev/Girona_Donostia/wiki
 
 Author: Petru Milev
```

### Comparing `girona_donostia-0.1.8/girona_donostia/__init__.py` & `girona_donostia-0.1.9/girona_donostia/__init__.py`

 * *Files identical despite different names*

### Comparing `girona_donostia-0.1.8/girona_donostia/curve_fit.py` & `girona_donostia-0.1.9/girona_donostia/curve_fit.py`

 * *Files identical despite different names*

### Comparing `girona_donostia-0.1.8/girona_donostia/functions_for_library.py` & `girona_donostia-0.1.9/girona_donostia/functions_for_library.py`

 * *Files identical despite different names*

### Comparing `girona_donostia-0.1.8/girona_donostia/objects_for_library.py` & `girona_donostia-0.1.9/girona_donostia/objects_for_library.py`

 * *Files identical despite different names*

### Comparing `girona_donostia-0.1.8/girona_donostia/romberg.py` & `girona_donostia-0.1.9/girona_donostia/romberg.py`

 * *Files identical despite different names*

### Comparing `girona_donostia-0.1.8/girona_donostia/statistic.py` & `girona_donostia-0.1.9/girona_donostia/statistic.py`

 * *Files identical despite different names*

### Comparing `girona_donostia-0.1.8/girona_donostia.egg-info/PKG-INFO` & `girona_donostia-0.1.9/girona_donostia.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: girona-donostia
-Version: 0.1.8
+Name: girona_donostia
+Version: 0.1.9
 Summary: A small package to work with nonlinear optical propreties
 Home-page: https://github.com/Petru-Milev/Girona_Donostia
 Author: Petru Milev
 Author-email: Petru Milev <petia.md36@gmail.com>
 License: MIT License
         
-        Copyright (c) 2023 Petru Milev
+        Copyright (c) 2024 Petru Milev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -22,23 +22,27 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+        
 Project-URL: Homepage, https://github.com/Petru-Milev/Girona_Donostia
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
 
 # Girona_Donostia
 
 This is a source for a Python Library to study nonlinear optical propreties using Gaussian. 
 So far, this library can create a variety of Gaussian Input Files, and analize the output files (.log and .fchk files)
 
-Main Functionality is described in the Manual. 
+Main Functionality is described on the wiki page.
+https://github.com/Petru-Milev/Girona_Donostia/wiki
 
 Author: Petru Milev
```

### Comparing `girona_donostia-0.1.8/pyproject.toml` & `girona_donostia-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "girona_donostia"
-version = "0.1.8"
+version = "0.1.9"
 license ={file = "LICENSE"}
 authors = [
   { name="Petru Milev", email="petia.md36@gmail.com" },
 ]
 description = "A small package to work with nonlinear optical propreties"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `girona_donostia-0.1.8/setup.py` & `girona_donostia-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='girona_donostia',
-    version='0.1.8',    
+    version='0.1.9',    
     description='A package to help facilitate studying of Nonlinear optical propreties',
     url='https://github.com/Petru-Milev/Girona_Donostia',
     author='Petru Milev',
     author_email='petia.md36@gmail.com',
     license='MIT',
     packages = find_packages(include=['girona_donostia', 'girona_donostia.*']),
 
@@ -15,8 +15,8 @@
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',  
         'Operating System :: POSIX :: Linux',        
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
-)
+)
```

