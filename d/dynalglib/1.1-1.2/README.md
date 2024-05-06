# Comparing `tmp/dynalglib-1.1.tar.gz` & `tmp/dynalglib-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynalglib-1.1.tar", last modified: Mon May  6 10:18:53 2024, max compression
+gzip compressed data, was "dynalglib-1.2.tar", last modified: Mon May  6 10:34:50 2024, max compression
```

## Comparing `dynalglib-1.1.tar` & `dynalglib-1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yslsml     (501) staff       (20)        0 2024-05-06 10:18:53.408185 dynalglib-1.1/
--rw-r--r--   0 yslsml     (501) staff       (20)     1072 2024-04-29 14:04:56.000000 dynalglib-1.1/LICENSE
--rw-r--r--   0 yslsml     (501) staff       (20)     2132 2024-05-06 10:18:53.408057 dynalglib-1.1/PKG-INFO
--rw-r--r--   0 yslsml     (501) staff       (20)     1164 2024-05-06 08:58:06.000000 dynalglib-1.1/README.md
-drwxr-xr-x   0 yslsml     (501) staff       (20)        0 2024-05-06 10:18:53.405644 dynalglib-1.1/dynalglib/
--rw-r--r--   0 yslsml     (501) staff       (20)     1098 2024-05-06 08:13:56.000000 dynalglib-1.1/dynalglib/__init__.py
--rw-r--r--   0 yslsml     (501) staff       (20)     3104 2024-05-06 08:13:57.000000 dynalglib-1.1/dynalglib/coin_change.py
--rw-r--r--   0 yslsml     (501) staff       (20)     1958 2024-05-06 08:13:57.000000 dynalglib-1.1/dynalglib/fibonacci.py
--rw-r--r--   0 yslsml     (501) staff       (20)     1339 2024-05-06 08:13:57.000000 dynalglib-1.1/dynalglib/item.py
--rw-r--r--   0 yslsml     (501) staff       (20)     6130 2024-05-06 08:13:57.000000 dynalglib-1.1/dynalglib/knapsack.py
--rw-r--r--   0 yslsml     (501) staff       (20)     5222 2024-05-06 08:13:57.000000 dynalglib-1.1/dynalglib/resource_allocation.py
--rw-r--r--   0 yslsml     (501) staff       (20)     4496 2024-05-06 08:13:57.000000 dynalglib-1.1/dynalglib/tsp.py
--rw-r--r--   0 yslsml     (501) staff       (20)      543 2024-05-06 07:19:07.000000 dynalglib-1.1/dynalglib/utils.py
-drwxr-xr-x   0 yslsml     (501) staff       (20)        0 2024-05-06 10:18:53.407856 dynalglib-1.1/dynalglib.egg-info/
--rw-r--r--   0 yslsml     (501) staff       (20)     2132 2024-05-06 10:18:53.000000 dynalglib-1.1/dynalglib.egg-info/PKG-INFO
--rw-r--r--   0 yslsml     (501) staff       (20)      337 2024-05-06 10:18:53.000000 dynalglib-1.1/dynalglib.egg-info/SOURCES.txt
--rw-r--r--   0 yslsml     (501) staff       (20)        1 2024-05-06 10:18:53.000000 dynalglib-1.1/dynalglib.egg-info/dependency_links.txt
--rw-r--r--   0 yslsml     (501) staff       (20)       10 2024-05-06 10:18:53.000000 dynalglib-1.1/dynalglib.egg-info/top_level.txt
--rw-r--r--   0 yslsml     (501) staff       (20)       38 2024-05-06 10:18:53.408243 dynalglib-1.1/setup.cfg
--rw-r--r--   0 yslsml     (501) staff       (20)     1856 2024-05-06 10:18:36.000000 dynalglib-1.1/setup.py
+drwxr-xr-x   0 yslsml     (501) staff       (20)        0 2024-05-06 10:34:50.995671 dynalglib-1.2/
+-rw-r--r--   0 yslsml     (501) staff       (20)     1072 2024-04-29 14:04:56.000000 dynalglib-1.2/LICENSE
+-rw-r--r--   0 yslsml     (501) staff       (20)     2214 2024-05-06 10:34:50.995552 dynalglib-1.2/PKG-INFO
+-rw-r--r--   0 yslsml     (501) staff       (20)     1164 2024-05-06 08:58:06.000000 dynalglib-1.2/README.md
+drwxr-xr-x   0 yslsml     (501) staff       (20)        0 2024-05-06 10:34:50.992382 dynalglib-1.2/dynalglib/
+-rw-r--r--   0 yslsml     (501) staff       (20)     1098 2024-05-06 08:13:56.000000 dynalglib-1.2/dynalglib/__init__.py
+-rw-r--r--   0 yslsml     (501) staff       (20)     3104 2024-05-06 08:13:57.000000 dynalglib-1.2/dynalglib/coin_change.py
+-rw-r--r--   0 yslsml     (501) staff       (20)     1958 2024-05-06 08:13:57.000000 dynalglib-1.2/dynalglib/fibonacci.py
+-rw-r--r--   0 yslsml     (501) staff       (20)     1339 2024-05-06 08:13:57.000000 dynalglib-1.2/dynalglib/item.py
+-rw-r--r--   0 yslsml     (501) staff       (20)     6130 2024-05-06 08:13:57.000000 dynalglib-1.2/dynalglib/knapsack.py
+-rw-r--r--   0 yslsml     (501) staff       (20)     5222 2024-05-06 08:13:57.000000 dynalglib-1.2/dynalglib/resource_allocation.py
+-rw-r--r--   0 yslsml     (501) staff       (20)     4496 2024-05-06 08:13:57.000000 dynalglib-1.2/dynalglib/tsp.py
+-rw-r--r--   0 yslsml     (501) staff       (20)      543 2024-05-06 07:19:07.000000 dynalglib-1.2/dynalglib/utils.py
+drwxr-xr-x   0 yslsml     (501) staff       (20)        0 2024-05-06 10:34:50.995360 dynalglib-1.2/dynalglib.egg-info/
+-rw-r--r--   0 yslsml     (501) staff       (20)     2214 2024-05-06 10:34:50.000000 dynalglib-1.2/dynalglib.egg-info/PKG-INFO
+-rw-r--r--   0 yslsml     (501) staff       (20)      337 2024-05-06 10:34:50.000000 dynalglib-1.2/dynalglib.egg-info/SOURCES.txt
+-rw-r--r--   0 yslsml     (501) staff       (20)        1 2024-05-06 10:34:50.000000 dynalglib-1.2/dynalglib.egg-info/dependency_links.txt
+-rw-r--r--   0 yslsml     (501) staff       (20)       10 2024-05-06 10:34:50.000000 dynalglib-1.2/dynalglib.egg-info/top_level.txt
+-rw-r--r--   0 yslsml     (501) staff       (20)       38 2024-05-06 10:34:50.995714 dynalglib-1.2/setup.cfg
+-rw-r--r--   0 yslsml     (501) staff       (20)     2004 2024-05-06 10:34:44.000000 dynalglib-1.2/setup.py
```

### Comparing `dynalglib-1.1/LICENSE` & `dynalglib-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dynalglib-1.1/PKG-INFO` & `dynalglib-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dynalglib
-Version: 1.1
+Version: 1.2
 Summary: Dynalglib is a library which is designed to solve some of dynamic programming algorithms in Python.
 Home-page: https://github.com/yslsml/dynalglib
 Author: Milana Antonova
 Author-email: mmf.antonovam@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/yslsml/dynalglib/wiki/Documentation
 Project-URL: Source, https://github.com/yslsml/dynalglib
-Keywords: math,dynamic algo,algorithms,algorithm,dynamic programming,knapsack problem
+Keywords: math,dynamic algo,algorithms,algorithm,dynamic programming,knapsack problem,knapsack,traveling salesman problem,tsp,resource allocation,fibonacci,coin change
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dynalglib-1.1/README.md` & `dynalglib-1.2/README.md`

 * *Files identical despite different names*

### Comparing `dynalglib-1.1/dynalglib/__init__.py` & `dynalglib-1.2/dynalglib/__init__.py`

 * *Files identical despite different names*

### Comparing `dynalglib-1.1/dynalglib/coin_change.py` & `dynalglib-1.2/dynalglib/coin_change.py`

 * *Files identical despite different names*

### Comparing `dynalglib-1.1/dynalglib/fibonacci.py` & `dynalglib-1.2/dynalglib/fibonacci.py`

 * *Files identical despite different names*

### Comparing `dynalglib-1.1/dynalglib/item.py` & `dynalglib-1.2/dynalglib/item.py`

 * *Files identical despite different names*

### Comparing `dynalglib-1.1/dynalglib/knapsack.py` & `dynalglib-1.2/dynalglib/knapsack.py`

 * *Files identical despite different names*

### Comparing `dynalglib-1.1/dynalglib/resource_allocation.py` & `dynalglib-1.2/dynalglib/resource_allocation.py`

 * *Files identical despite different names*

### Comparing `dynalglib-1.1/dynalglib/tsp.py` & `dynalglib-1.2/dynalglib/tsp.py`

 * *Files identical despite different names*

### Comparing `dynalglib-1.1/dynalglib/utils.py` & `dynalglib-1.2/dynalglib/utils.py`

 * *Files identical despite different names*

### Comparing `dynalglib-1.1/dynalglib.egg-info/PKG-INFO` & `dynalglib-1.2/dynalglib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dynalglib
-Version: 1.1
+Version: 1.2
 Summary: Dynalglib is a library which is designed to solve some of dynamic programming algorithms in Python.
 Home-page: https://github.com/yslsml/dynalglib
 Author: Milana Antonova
 Author-email: mmf.antonovam@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/yslsml/dynalglib/wiki/Documentation
 Project-URL: Source, https://github.com/yslsml/dynalglib
-Keywords: math,dynamic algo,algorithms,algorithm,dynamic programming,knapsack problem
+Keywords: math,dynamic algo,algorithms,algorithm,dynamic programming,knapsack problem,knapsack,traveling salesman problem,tsp,resource allocation,fibonacci,coin change
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dynalglib-1.1/setup.py` & `dynalglib-1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from distutils.core import setup
 import pathlib
 
-VERSION = "1.1"
+VERSION = "1.2"
 
 setup(
     name="dynalglib",  # How you named your package folder (MyLib)
     packages=["dynalglib"],  # Chose the same as "name"
     version=VERSION,  # Start with a small number and increase it with every change you make
     license="MIT",  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description="Dynalglib is a library which is designed to solve some of dynamic programming algorithms in Python.",  # Give a short description about your library
@@ -21,14 +21,20 @@
     keywords=[
         "math",
         "dynamic algo",
         "algorithms",
         "algorithm",
         "dynamic programming",
         "knapsack problem",
+        "knapsack",
+        "traveling salesman problem", 
+        "tsp",
+        "resource allocation",
+        "fibonacci",
+        "coin change"
     ],  # Keywords that define your package best
     classifiers=[
         "Development Status :: 3 - Alpha",  # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         "Intended Audience :: Developers",  # Define that your audience are developers
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",  # Again, pick a license
         "Programming Language :: Python :: 3.7",
```

