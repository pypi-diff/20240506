# Comparing `tmp/ScholarCodeCollective-0.1.7.1.tar.gz` & `tmp/ScholarCodeCollective-0.1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScholarCodeCollective-0.1.7.1.tar", last modified: Mon May  6 18:10:43 2024, max compression
+gzip compressed data, was "ScholarCodeCollective-0.1.7.2.tar", last modified: Mon May  6 18:14:26 2024, max compression
```

## Comparing `ScholarCodeCollective-0.1.7.1.tar` & `ScholarCodeCollective-0.1.7.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.230826 ScholarCodeCollective-0.1.7.1/
--rw-rw-rw-   0        0        0     2034 2024-05-06 18:10:43.229814 ScholarCodeCollective-0.1.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     1333 2024-05-06 18:10:11.000000 ScholarCodeCollective-0.1.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.178503 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/
-drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.209347 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/Community_Representatives_main/
--rw-rw-rw-   0        0        0       26 2024-05-06 17:39:11.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/Community_Representatives_main/__init__.py
--rw-rw-rw-   0        0        0  1889833 2024-05-06 17:54:05.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/Community_Representatives_main/functions.cpp
-drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.214035 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/MDL_network_population_clustering_main/
--rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
--rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.217556 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/MDL_regionalization_main/
--rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/MDL_regionalization_main/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 11:59:09.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/MDL_regionalization_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.221645 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/Network_hubs_main/
--rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/Network_hubs_main/__init__.py
--rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/Network_hubs_main/functions.py
--rw-rw-rw-   0        0        0      129 2024-04-23 12:14:08.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.226237 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/hypergraph_binning_main/
--rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/hypergraph_binning_main/__init__.py
--rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/hypergraph_binning_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.197777 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective.egg-info/
--rw-rw-rw-   0        0        0     2034 2024-05-06 18:10:42.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1014 2024-05-06 18:10:43.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 18:10:42.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-06 18:10:42.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-05-06 18:10:42.000000 ScholarCodeCollective-0.1.7.1/ScholarCodeCollective.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 18:10:43.230826 ScholarCodeCollective-0.1.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1927 2024-05-06 18:10:34.000000 ScholarCodeCollective-0.1.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:10:43.227698 ScholarCodeCollective-0.1.7.1/tests/
--rw-rw-rw-   0        0        0     1010 2024-04-22 17:16:16.000000 ScholarCodeCollective-0.1.7.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:14:26.564484 ScholarCodeCollective-0.1.7.2/
+-rw-rw-rw-   0        0        0     2038 2024-05-06 18:14:26.564484 ScholarCodeCollective-0.1.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1388 2024-05-06 18:14:09.000000 ScholarCodeCollective-0.1.7.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 18:14:26.508232 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/
+drwxrwxrwx   0        0        0        0 2024-05-06 18:14:26.541937 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/Community_Representatives_main/
+-rw-rw-rw-   0        0        0       26 2024-05-06 17:39:11.000000 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/Community_Representatives_main/__init__.py
+-rw-rw-rw-   0        0        0  1889833 2024-05-06 17:54:05.000000 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/Community_Representatives_main/functions.cpp
+drwxrwxrwx   0        0        0        0 2024-05-06 18:14:26.547124 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/MDL_network_population_clustering_main/
+-rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
+-rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:14:26.551756 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/MDL_regionalization_main/
+-rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/MDL_regionalization_main/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 11:59:09.000000 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/MDL_regionalization_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:14:26.555767 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/Network_hubs_main/
+-rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/Network_hubs_main/__init__.py
+-rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/Network_hubs_main/functions.py
+-rw-rw-rw-   0        0        0      129 2024-04-23 12:14:08.000000 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:14:26.559608 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/hypergraph_binning_main/
+-rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/hypergraph_binning_main/__init__.py
+-rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/hypergraph_binning_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:14:26.530642 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective.egg-info/
+-rw-rw-rw-   0        0        0     2038 2024-05-06 18:14:26.000000 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1014 2024-05-06 18:14:26.000000 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 18:14:26.000000 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-06 18:14:26.000000 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-05-06 18:14:26.000000 ScholarCodeCollective-0.1.7.2/ScholarCodeCollective.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 18:14:26.564484 ScholarCodeCollective-0.1.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1927 2024-05-06 18:14:20.000000 ScholarCodeCollective-0.1.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:14:26.561098 ScholarCodeCollective-0.1.7.2/tests/
+-rw-rw-rw-   0        0        0     1010 2024-04-22 17:16:16.000000 ScholarCodeCollective-0.1.7.2/tests/__init__.py
```

### Comparing `ScholarCodeCollective-0.1.7.1/PKG-INFO` & `ScholarCodeCollective-0.1.7.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.7.1
+Version: 0.1.7.2
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
@@ -14,40 +14,41 @@
 
 ## In order to create a Python project with a similar structure you need to do the following: 
 ### The structure of the project should be as follows: 
 ```
 project
 â”œâ”€â”€ README.md
 â”œâ”€â”€ example
-â”‚Â Â  â”œâ”€â”€ __init__.py
-â”‚Â Â  â”œâ”€â”€ package_1
-â”‚Â Â  â”‚Â Â  â”œâ”€â”€ __init__.py
-â”‚Â Â  â”‚Â Â  â”œâ”€â”€ awesome_module.py
-â”‚Â Â  â”‚Â Â  â”œâ”€â”€ ...
-â”‚Â Â  â”‚Â Â  â””â”€â”€ awesome_module_n.py
-â”‚Â Â  â””â”€â”€ package_2
-â”‚Â Â      â”œâ”€â”€ __init__.py
-â”‚Â Â      â””â”€â”€ module.py
+â”‚ â”œâ”€â”€ init.py
+â”‚ â”œâ”€â”€ package_1
+â”‚ â”‚ â”œâ”€â”€ init.py
+â”‚ â”‚ â”œâ”€â”€ awesome_module.py
+â”‚ â”‚ â”œâ”€â”€ ...
+â”‚ â”‚ â””â”€â”€ awesome_module_n.py
+â”‚ â””â”€â”€ package_2
+â”‚ â”œâ”€â”€ init.py
+â”‚ â””â”€â”€ module.py
 â”œâ”€â”€ setup.py
 â””â”€â”€ tests
-    â””â”€â”€ __init__.py
+â””â”€â”€ init.py
 ```
 ### Command for wheel creation and upload 
 * For Python3 users: 
   * `python setup.py sdist`
   * `del dist\*`
   * `stwine upload --verbose dist/*    `
 
 # ScholarCodeCollective Package
 
 Welcome to the ScholarCodeCollective package. Below you will find links to various resources including our local documentation.
 
 ## Documentation
 
-For detailed documentation, please refer to our [local documentation](google.com).
+For detailed documentation, please refer to our [local documentation](file:///D:/Research%20HKU/PYPI_lib/Documentation/_build/html/index.html).
+(file:///D:/Research%20HKU/PYPI_lib/Documentation/_build/html/index.html)
 
 ## Installation
 
 Provide installation instructions here.
 
 ## Usage
```

### Comparing `ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/Community_Representatives_main/functions.cpp` & `ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/Community_Representatives_main/functions.cpp`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py` & `ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/MDL_regionalization_main/functions.py` & `ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/MDL_regionalization_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/Network_hubs_main/functions.py` & `ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/Network_hubs_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.1/ScholarCodeCollective/hypergraph_binning_main/functions.py` & `ScholarCodeCollective-0.1.7.2/ScholarCodeCollective/hypergraph_binning_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.1/ScholarCodeCollective.egg-info/PKG-INFO` & `ScholarCodeCollective-0.1.7.2/ScholarCodeCollective.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.7.1
+Version: 0.1.7.2
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
@@ -14,40 +14,41 @@
 
 ## In order to create a Python project with a similar structure you need to do the following: 
 ### The structure of the project should be as follows: 
 ```
 project
 â”œâ”€â”€ README.md
 â”œâ”€â”€ example
-â”‚Â Â  â”œâ”€â”€ __init__.py
-â”‚Â Â  â”œâ”€â”€ package_1
-â”‚Â Â  â”‚Â Â  â”œâ”€â”€ __init__.py
-â”‚Â Â  â”‚Â Â  â”œâ”€â”€ awesome_module.py
-â”‚Â Â  â”‚Â Â  â”œâ”€â”€ ...
-â”‚Â Â  â”‚Â Â  â””â”€â”€ awesome_module_n.py
-â”‚Â Â  â””â”€â”€ package_2
-â”‚Â Â      â”œâ”€â”€ __init__.py
-â”‚Â Â      â””â”€â”€ module.py
+â”‚ â”œâ”€â”€ init.py
+â”‚ â”œâ”€â”€ package_1
+â”‚ â”‚ â”œâ”€â”€ init.py
+â”‚ â”‚ â”œâ”€â”€ awesome_module.py
+â”‚ â”‚ â”œâ”€â”€ ...
+â”‚ â”‚ â””â”€â”€ awesome_module_n.py
+â”‚ â””â”€â”€ package_2
+â”‚ â”œâ”€â”€ init.py
+â”‚ â””â”€â”€ module.py
 â”œâ”€â”€ setup.py
 â””â”€â”€ tests
-    â””â”€â”€ __init__.py
+â””â”€â”€ init.py
 ```
 ### Command for wheel creation and upload 
 * For Python3 users: 
   * `python setup.py sdist`
   * `del dist\*`
   * `stwine upload --verbose dist/*    `
 
 # ScholarCodeCollective Package
 
 Welcome to the ScholarCodeCollective package. Below you will find links to various resources including our local documentation.
 
 ## Documentation
 
-For detailed documentation, please refer to our [local documentation](google.com).
+For detailed documentation, please refer to our [local documentation](file:///D:/Research%20HKU/PYPI_lib/Documentation/_build/html/index.html).
+(file:///D:/Research%20HKU/PYPI_lib/Documentation/_build/html/index.html)
 
 ## Installation
 
 Provide installation instructions here.
 
 ## Usage
```

### Comparing `ScholarCodeCollective-0.1.7.1/ScholarCodeCollective.egg-info/SOURCES.txt` & `ScholarCodeCollective-0.1.7.2/ScholarCodeCollective.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.1/setup.py` & `ScholarCodeCollective-0.1.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     Extension("ScholarCodeCollective.Community_Representatives_main.functions",
               ["ScholarCodeCollective/Community_Representatives_main/functions.pyx"],
               language='c++')  # use 'c' if not using C++ features
 ]
 
 setup(
     name='ScholarCodeCollective',
-    version='0.1.7.1',
+    version='0.1.7.2',
     description='A collective library for the code behind several academic papers',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://google.com',
     author='Author Name',
     author_email='author_email@mail.com',
     license='The Unlicense',
```

### Comparing `ScholarCodeCollective-0.1.7.1/tests/__init__.py` & `ScholarCodeCollective-0.1.7.2/tests/__init__.py`

 * *Files identical despite different names*

