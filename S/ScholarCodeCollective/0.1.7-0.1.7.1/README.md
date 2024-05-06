# Comparing `tmp/ScholarCodeCollective-0.1.7.tar.gz` & `tmp/ScholarCodeCollective-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScholarCodeCollective-0.1.7.tar", last modified: Mon May  6 18:08:45 2024, max compression
+gzip compressed data, was "ScholarCodeCollective-0.1.7.1.tar", last modified: Mon May  6 18:10:43 2024, max compression
```

## Comparing `ScholarCodeCollective-0.1.7.tar` & `ScholarCodeCollective-0.1.7.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.722256 ScholarCodeCollective-0.1.7/
--rw-rw-rw-   0        0        0     2093 2024-05-06 18:08:45.720252 ScholarCodeCollective-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1394 2024-05-06 18:08:29.000000 ScholarCodeCollective-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.661272 ScholarCodeCollective-0.1.7/ScholarCodeCollective/
-drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.696332 ScholarCodeCollective-0.1.7/ScholarCodeCollective/Community_Representatives_main/
--rw-rw-rw-   0        0        0       26 2024-05-06 17:39:11.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/Community_Representatives_main/__init__.py
--rw-rw-rw-   0        0        0  1889833 2024-05-06 17:54:05.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/Community_Representatives_main/functions.cpp
-drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.701283 ScholarCodeCollective-0.1.7/ScholarCodeCollective/MDL_network_population_clustering_main/
--rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
--rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.706306 ScholarCodeCollective-0.1.7/ScholarCodeCollective/MDL_regionalization_main/
--rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/MDL_regionalization_main/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 11:59:09.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/MDL_regionalization_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.710735 ScholarCodeCollective-0.1.7/ScholarCodeCollective/Network_hubs_main/
--rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/Network_hubs_main/__init__.py
--rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/Network_hubs_main/functions.py
--rw-rw-rw-   0        0        0      129 2024-04-23 12:14:08.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.715802 ScholarCodeCollective-0.1.7/ScholarCodeCollective/hypergraph_binning_main/
--rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/hypergraph_binning_main/__init__.py
--rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/hypergraph_binning_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.688212 ScholarCodeCollective-0.1.7/ScholarCodeCollective.egg-info/
--rw-rw-rw-   0        0        0     2093 2024-05-06 18:08:45.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1014 2024-05-06 18:08:45.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 18:08:45.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-06 18:08:45.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-05-06 18:08:45.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 18:08:45.722256 ScholarCodeCollective-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1925 2024-05-06 18:08:36.000000 ScholarCodeCollective-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.718255 ScholarCodeCollective-0.1.7/tests/
--rw-rw-rw-   0        0        0     1010 2024-04-22 17:16:16.000000 ScholarCodeCollective-0.1.7/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.230826 ScholarCodeCollective-0.1.7.1/
+-rw-rw-rw-   0        0        0     2034 2024-05-06 18:10:43.229814 ScholarCodeCollective-0.1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1333 2024-05-06 18:10:11.000000 ScholarCodeCollective-0.1.7.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.178503 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/
+drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.209347 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/Community_Representatives_main/
+-rw-rw-rw-   0        0        0       26 2024-05-06 17:39:11.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/Community_Representatives_main/__init__.py
+-rw-rw-rw-   0        0        0  1889833 2024-05-06 17:54:05.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/Community_Representatives_main/functions.cpp
+drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.214035 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/MDL_network_population_clustering_main/
+-rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
+-rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.217556 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/MDL_regionalization_main/
+-rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/MDL_regionalization_main/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 11:59:09.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/MDL_regionalization_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.221645 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/Network_hubs_main/
+-rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/Network_hubs_main/__init__.py
+-rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/Network_hubs_main/functions.py
+-rw-rw-rw-   0        0        0      129 2024-04-23 12:14:08.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.226237 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/hypergraph_binning_main/
+-rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/hypergraph_binning_main/__init__.py
+-rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/hypergraph_binning_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.197777 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective.egg-info/
+-rw-rw-rw-   0        0        0     2034 2024-05-06 18:10:42.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1014 2024-05-06 18:10:43.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 18:10:42.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-06 18:10:42.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-05-06 18:10:42.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 18:10:43.230826 ScholarCodeCollective-0.1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1927 2024-05-06 18:10:34.000000 ScholarCodeCollective-0.1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.227698 ScholarCodeCollective-0.1.7.1/tests/
+-rw-rw-rw-   0        0        0     1010 2024-04-22 17:16:16.000000 ScholarCodeCollective-0.1.7.1/tests/__init__.py
```

### Comparing `ScholarCodeCollective-0.1.7/PKG-INFO` & `ScholarCodeCollective-0.1.7.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
@@ -39,15 +39,15 @@
 
 # ScholarCodeCollective Package
 
 Welcome to the ScholarCodeCollective package. Below you will find links to various resources including our local documentation.
 
 ## Documentation
 
-For detailed documentation, please refer to our [local documentation](file:///D:/Research%20HKU/PYPI_lib/Documentation/_build/html/index.html).
+For detailed documentation, please refer to our [local documentation](google.com).
 
 ## Installation
 
 Provide installation instructions here.
 
 ## Usage
```

### Comparing `ScholarCodeCollective-0.1.7/README.md` & `ScholarCodeCollective-0.1.7.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 # ScholarCodeCollective Package
 
 Welcome to the ScholarCodeCollective package. Below you will find links to various resources including our local documentation.
 
 ## Documentation
 
-For detailed documentation, please refer to our [local documentation](file:///D:/Research%20HKU/PYPI_lib/Documentation/_build/html/index.html).
+For detailed documentation, please refer to our [local documentation](google.com).
 
 ## Installation
 
 Provide installation instructions here.
 
 ## Usage
```

### Comparing `ScholarCodeCollective-0.1.7/ScholarCodeCollective/Community_Representatives_main/functions.cpp` & `ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/Community_Representatives_main/functions.cpp`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py` & `ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7/ScholarCodeCollective/MDL_regionalization_main/functions.py` & `ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/MDL_regionalization_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7/ScholarCodeCollective/Network_hubs_main/functions.py` & `ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/Network_hubs_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7/ScholarCodeCollective/hypergraph_binning_main/functions.py` & `ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/hypergraph_binning_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7/ScholarCodeCollective.egg-info/PKG-INFO` & `ScholarCodeCollective-0.1.7.1/ScholarCodeCollective.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
@@ -39,15 +39,15 @@
 
 # ScholarCodeCollective Package
 
 Welcome to the ScholarCodeCollective package. Below you will find links to various resources including our local documentation.
 
 ## Documentation
 
-For detailed documentation, please refer to our [local documentation](file:///D:/Research%20HKU/PYPI_lib/Documentation/_build/html/index.html).
+For detailed documentation, please refer to our [local documentation](google.com).
 
 ## Installation
 
 Provide installation instructions here.
 
 ## Usage
```

### Comparing `ScholarCodeCollective-0.1.7/ScholarCodeCollective.egg-info/SOURCES.txt` & `ScholarCodeCollective-0.1.7.1/ScholarCodeCollective.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7/setup.py` & `ScholarCodeCollective-0.1.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     Extension("ScholarCodeCollective.Community_Representatives_main.functions",
               ["ScholarCodeCollective/Community_Representatives_main/functions.pyx"],
               language='c++')  # use 'c' if not using C++ features
 ]
 
 setup(
     name='ScholarCodeCollective',
-    version='0.1.7',
+    version='0.1.7.1',
     description='A collective library for the code behind several academic papers',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://google.com',
     author='Author Name',
     author_email='author_email@mail.com',
     license='The Unlicense',
```

### Comparing `ScholarCodeCollective-0.1.7/tests/__init__.py` & `ScholarCodeCollective-0.1.7.1/tests/__init__.py`

 * *Files identical despite different names*

