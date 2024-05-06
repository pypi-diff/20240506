# Comparing `tmp/ScholarCodeCollective-0.1.5.tar.gz` & `tmp/ScholarCodeCollective-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScholarCodeCollective-0.1.5.tar", last modified: Mon May  6 17:57:16 2024, max compression
+gzip compressed data, was "ScholarCodeCollective-0.1.6.tar", last modified: Mon May  6 18:00:28 2024, max compression
```

## Comparing `ScholarCodeCollective-0.1.5.tar` & `ScholarCodeCollective-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.862033 ScholarCodeCollective-0.1.5/
--rw-rw-rw-   0        0        0     3784 2024-05-06 17:57:16.860524 ScholarCodeCollective-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2644 2024-04-21 08:44:00.000000 ScholarCodeCollective-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.810822 ScholarCodeCollective-0.1.5/ScholarCodeCollective/
-drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.840338 ScholarCodeCollective-0.1.5/ScholarCodeCollective/Community_Representatives_main/
--rw-rw-rw-   0        0        0       26 2024-05-06 17:39:11.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/Community_Representatives_main/__init__.py
--rw-rw-rw-   0        0        0  1889833 2024-05-06 17:54:05.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/Community_Representatives_main/functions.cpp
-drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.845351 ScholarCodeCollective-0.1.5/ScholarCodeCollective/MDL_network_population_clustering_main/
--rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
--rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.849223 ScholarCodeCollective-0.1.5/ScholarCodeCollective/MDL_regionalization_main/
--rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/MDL_regionalization_main/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 11:59:09.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/MDL_regionalization_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.852755 ScholarCodeCollective-0.1.5/ScholarCodeCollective/Network_hubs_main/
--rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/Network_hubs_main/__init__.py
--rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/Network_hubs_main/functions.py
--rw-rw-rw-   0        0        0      129 2024-04-23 12:14:08.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.857101 ScholarCodeCollective-0.1.5/ScholarCodeCollective/hypergraph_binning_main/
--rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/hypergraph_binning_main/__init__.py
--rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/hypergraph_binning_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.835235 ScholarCodeCollective-0.1.5/ScholarCodeCollective.egg-info/
--rw-rw-rw-   0        0        0     3784 2024-05-06 17:57:16.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1014 2024-05-06 17:57:16.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 17:57:16.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-06 17:57:16.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-05-06 17:57:16.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 17:57:16.862033 ScholarCodeCollective-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1872 2024-05-06 17:57:07.000000 ScholarCodeCollective-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.858099 ScholarCodeCollective-0.1.5/tests/
--rw-rw-rw-   0        0        0     1010 2024-04-22 17:16:16.000000 ScholarCodeCollective-0.1.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.170947 ScholarCodeCollective-0.1.6/
+-rw-rw-rw-   0        0        0     3784 2024-05-06 18:00:28.169946 ScholarCodeCollective-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2644 2024-04-21 08:44:00.000000 ScholarCodeCollective-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.118906 ScholarCodeCollective-0.1.6/ScholarCodeCollective/
+drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.148470 ScholarCodeCollective-0.1.6/ScholarCodeCollective/Community_Representatives_main/
+-rw-rw-rw-   0        0        0       26 2024-05-06 17:39:11.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/Community_Representatives_main/__init__.py
+-rw-rw-rw-   0        0        0  1889833 2024-05-06 17:54:05.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/Community_Representatives_main/functions.cpp
+drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.153983 ScholarCodeCollective-0.1.6/ScholarCodeCollective/MDL_network_population_clustering_main/
+-rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
+-rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.157988 ScholarCodeCollective-0.1.6/ScholarCodeCollective/MDL_regionalization_main/
+-rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/MDL_regionalization_main/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 11:59:09.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/MDL_regionalization_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.162504 ScholarCodeCollective-0.1.6/ScholarCodeCollective/Network_hubs_main/
+-rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/Network_hubs_main/__init__.py
+-rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/Network_hubs_main/functions.py
+-rw-rw-rw-   0        0        0      129 2024-04-23 12:14:08.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.165939 ScholarCodeCollective-0.1.6/ScholarCodeCollective/hypergraph_binning_main/
+-rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/hypergraph_binning_main/__init__.py
+-rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/hypergraph_binning_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.138335 ScholarCodeCollective-0.1.6/ScholarCodeCollective.egg-info/
+-rw-rw-rw-   0        0        0     3784 2024-05-06 18:00:27.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1014 2024-05-06 18:00:28.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 18:00:27.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-06 18:00:27.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-05-06 18:00:27.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 18:00:28.170947 ScholarCodeCollective-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1925 2024-05-06 18:00:19.000000 ScholarCodeCollective-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.167953 ScholarCodeCollective-0.1.6/tests/
+-rw-rw-rw-   0        0        0     1010 2024-04-22 17:16:16.000000 ScholarCodeCollective-0.1.6/tests/__init__.py
```

### Comparing `ScholarCodeCollective-0.1.5/PKG-INFO` & `ScholarCodeCollective-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.5
+Version: 0.1.6
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
```

### Comparing `ScholarCodeCollective-0.1.5/README.md` & `ScholarCodeCollective-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.5/ScholarCodeCollective/Community_Representatives_main/functions.cpp` & `ScholarCodeCollective-0.1.6/ScholarCodeCollective/Community_Representatives_main/functions.cpp`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.5/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py` & `ScholarCodeCollective-0.1.6/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.5/ScholarCodeCollective/MDL_regionalization_main/functions.py` & `ScholarCodeCollective-0.1.6/ScholarCodeCollective/MDL_regionalization_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.5/ScholarCodeCollective/Network_hubs_main/functions.py` & `ScholarCodeCollective-0.1.6/ScholarCodeCollective/Network_hubs_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.5/ScholarCodeCollective/hypergraph_binning_main/functions.py` & `ScholarCodeCollective-0.1.6/ScholarCodeCollective/hypergraph_binning_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.5/ScholarCodeCollective.egg-info/PKG-INFO` & `ScholarCodeCollective-0.1.6/ScholarCodeCollective.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.5
+Version: 0.1.6
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
```

### Comparing `ScholarCodeCollective-0.1.5/ScholarCodeCollective.egg-info/SOURCES.txt` & `ScholarCodeCollective-0.1.6/ScholarCodeCollective.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.5/setup.py` & `ScholarCodeCollective-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,25 +31,25 @@
     Extension("ScholarCodeCollective.Community_Representatives_main.functions",
               ["ScholarCodeCollective/Community_Representatives_main/functions.pyx"],
               language='c++')  # use 'c' if not using C++ features
 ]
 
 setup(
     name='ScholarCodeCollective',
-    version='0.1.5',
+    version='0.1.6',
     description='A collective library for the code behind several academic papers',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://google.com',
     author='Author Name',
     author_email='author_email@mail.com',
     license='The Unlicense',
     projects_urls={
         "Documentation": "x",
-        "Source": "https://github.com"
+        "Source": "file:///D:/Research%20HKU/PYPI_lib/Documentation/_build/html/index.html"
     },
     python_requires=">=3.9, <3.12",
     packages=find_packages(),
     include_package_data=True,
     entry_points={"console_scripts": ["paper = paper.cli:main"]},
     ext_modules=cythonize(extensions, compiler_directives={'language_level': "3"})
 )
```

### Comparing `ScholarCodeCollective-0.1.5/tests/__init__.py` & `ScholarCodeCollective-0.1.6/tests/__init__.py`

 * *Files identical despite different names*

