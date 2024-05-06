# Comparing `tmp/ScholarCodeCollective-0.1.4.tar.gz` & `tmp/ScholarCodeCollective-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScholarCodeCollective-0.1.4.tar", last modified: Tue Apr 23 12:14:22 2024, max compression
+gzip compressed data, was "ScholarCodeCollective-0.1.5.tar", last modified: Mon May  6 17:57:16 2024, max compression
```

## Comparing `ScholarCodeCollective-0.1.4.tar` & `ScholarCodeCollective-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 12:14:22.640023 ScholarCodeCollective-0.1.4/
--rw-rw-rw-   0        0        0     3782 2024-04-23 12:14:22.640023 ScholarCodeCollective-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2644 2024-04-21 08:44:00.000000 ScholarCodeCollective-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 12:14:22.595245 ScholarCodeCollective-0.1.4/ScholarCodeCollective/
-drwxrwxrwx   0        0        0        0 2024-04-23 12:14:22.623794 ScholarCodeCollective-0.1.4/ScholarCodeCollective/MDL_network_population_clustering_main/
--rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.4/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
--rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.4/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-23 12:14:22.627956 ScholarCodeCollective-0.1.4/ScholarCodeCollective/MDL_regionalization_main/
--rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.4/ScholarCodeCollective/MDL_regionalization_main/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 11:59:09.000000 ScholarCodeCollective-0.1.4/ScholarCodeCollective/MDL_regionalization_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-23 12:14:22.631480 ScholarCodeCollective-0.1.4/ScholarCodeCollective/Network_hubs_main/
--rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.4/ScholarCodeCollective/Network_hubs_main/__init__.py
--rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.4/ScholarCodeCollective/Network_hubs_main/functions.py
--rw-rw-rw-   0        0        0      129 2024-04-23 12:14:08.000000 ScholarCodeCollective-0.1.4/ScholarCodeCollective/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.4/ScholarCodeCollective/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-23 12:14:22.636019 ScholarCodeCollective-0.1.4/ScholarCodeCollective/hypergraph_binning_main/
--rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.4/ScholarCodeCollective/hypergraph_binning_main/__init__.py
--rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.4/ScholarCodeCollective/hypergraph_binning_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-23 12:14:22.620042 ScholarCodeCollective-0.1.4/ScholarCodeCollective.egg-info/
--rw-rw-rw-   0        0        0     3782 2024-04-23 12:14:22.000000 ScholarCodeCollective-0.1.4/ScholarCodeCollective.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      815 2024-04-23 12:14:22.000000 ScholarCodeCollective-0.1.4/ScholarCodeCollective.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 12:14:22.000000 ScholarCodeCollective-0.1.4/ScholarCodeCollective.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-23 12:14:22.000000 ScholarCodeCollective-0.1.4/ScholarCodeCollective.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-04-23 12:14:22.000000 ScholarCodeCollective-0.1.4/ScholarCodeCollective.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 12:14:22.641530 ScholarCodeCollective-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      721 2024-04-23 12:14:16.000000 ScholarCodeCollective-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 12:14:22.638026 ScholarCodeCollective-0.1.4/tests/
--rw-rw-rw-   0        0        0     1010 2024-04-22 17:16:16.000000 ScholarCodeCollective-0.1.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.862033 ScholarCodeCollective-0.1.5/
+-rw-rw-rw-   0        0        0     3784 2024-05-06 17:57:16.860524 ScholarCodeCollective-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2644 2024-04-21 08:44:00.000000 ScholarCodeCollective-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.810822 ScholarCodeCollective-0.1.5/ScholarCodeCollective/
+drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.840338 ScholarCodeCollective-0.1.5/ScholarCodeCollective/Community_Representatives_main/
+-rw-rw-rw-   0        0        0       26 2024-05-06 17:39:11.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/Community_Representatives_main/__init__.py
+-rw-rw-rw-   0        0        0  1889833 2024-05-06 17:54:05.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/Community_Representatives_main/functions.cpp
+drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.845351 ScholarCodeCollective-0.1.5/ScholarCodeCollective/MDL_network_population_clustering_main/
+-rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
+-rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.849223 ScholarCodeCollective-0.1.5/ScholarCodeCollective/MDL_regionalization_main/
+-rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/MDL_regionalization_main/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 11:59:09.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/MDL_regionalization_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.852755 ScholarCodeCollective-0.1.5/ScholarCodeCollective/Network_hubs_main/
+-rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/Network_hubs_main/__init__.py
+-rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/Network_hubs_main/functions.py
+-rw-rw-rw-   0        0        0      129 2024-04-23 12:14:08.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.857101 ScholarCodeCollective-0.1.5/ScholarCodeCollective/hypergraph_binning_main/
+-rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/hypergraph_binning_main/__init__.py
+-rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective/hypergraph_binning_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.835235 ScholarCodeCollective-0.1.5/ScholarCodeCollective.egg-info/
+-rw-rw-rw-   0        0        0     3784 2024-05-06 17:57:16.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1014 2024-05-06 17:57:16.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 17:57:16.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-06 17:57:16.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-05-06 17:57:16.000000 ScholarCodeCollective-0.1.5/ScholarCodeCollective.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 17:57:16.862033 ScholarCodeCollective-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1872 2024-05-06 17:57:07.000000 ScholarCodeCollective-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:57:16.858099 ScholarCodeCollective-0.1.5/tests/
+-rw-rw-rw-   0        0        0     1010 2024-04-22 17:16:16.000000 ScholarCodeCollective-0.1.5/tests/__init__.py
```

### Comparing `ScholarCodeCollective-0.1.4/PKG-INFO` & `ScholarCodeCollective-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
-Requires-Python: >3.9,<3.12
+Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
 
 # A template to structure your Python application
 A python project to use as a template when developing a Python application.
 
 ## In order to create a Python project with a similar structure you need to do the following: 
 ### The structure of the project should be as follows:
```

### Comparing `ScholarCodeCollective-0.1.4/README.md` & `ScholarCodeCollective-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.4/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py` & `ScholarCodeCollective-0.1.5/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.4/ScholarCodeCollective/MDL_regionalization_main/functions.py` & `ScholarCodeCollective-0.1.5/ScholarCodeCollective/MDL_regionalization_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.4/ScholarCodeCollective/Network_hubs_main/functions.py` & `ScholarCodeCollective-0.1.5/ScholarCodeCollective/Network_hubs_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.4/ScholarCodeCollective/hypergraph_binning_main/functions.py` & `ScholarCodeCollective-0.1.5/ScholarCodeCollective/hypergraph_binning_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.4/ScholarCodeCollective.egg-info/PKG-INFO` & `ScholarCodeCollective-0.1.5/ScholarCodeCollective.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
-Requires-Python: >3.9,<3.12
+Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
 
 # A template to structure your Python application
 A python project to use as a template when developing a Python application.
 
 ## In order to create a Python project with a similar structure you need to do the following: 
 ### The structure of the project should be as follows:
```

### Comparing `ScholarCodeCollective-0.1.4/ScholarCodeCollective.egg-info/SOURCES.txt` & `ScholarCodeCollective-0.1.5/ScholarCodeCollective.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 ScholarCodeCollective/__init__.py
 ScholarCodeCollective/cli.py
 ScholarCodeCollective.egg-info/PKG-INFO
 ScholarCodeCollective.egg-info/SOURCES.txt
 ScholarCodeCollective.egg-info/dependency_links.txt
 ScholarCodeCollective.egg-info/entry_points.txt
 ScholarCodeCollective.egg-info/top_level.txt
+ScholarCodeCollective/Community_Representatives_main/functions.cpp
+ScholarCodeCollective/Community_Representatives_main/__init__.py
+ScholarCodeCollective/Community_Representatives_main/functions.cpp
 ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
 ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
 ScholarCodeCollective/MDL_regionalization_main/__init__.py
 ScholarCodeCollective/MDL_regionalization_main/functions.py
 ScholarCodeCollective/Network_hubs_main/__init__.py
 ScholarCodeCollective/Network_hubs_main/functions.py
 ScholarCodeCollective/hypergraph_binning_main/__init__.py
```

### Comparing `ScholarCodeCollective-0.1.4/setup.py` & `ScholarCodeCollective-0.1.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,55 @@
-from distutils.core import setup
-import pathlib
-import setuptools
+# from distutils.core import setup
+# import pathlib
+# import setuptools
+from setuptools import setup, find_packages, Extension
+from Cython.Build import cythonize
+import numpy  # If your Cython modules use NumPy
 
-setuptools.setup(
+
+# setuptools.setup(
+#     name='ScholarCodeCollective',
+#     version='0.1.4',
+#     description='A collective library for the code behind several academic papers',
+#     long_description=open('README.md').read(),
+#     long_description_content_type='text/markdown',
+#     url='https://google.com',
+#     author='Author Name', 
+#     author_email='author_email@mail.com',
+#     license='The Unlicense',
+#     projects_urls={
+#         "Documentation": "x",
+#         "Source": "https://github.com"
+#     },
+#     python_requires=">3.9,<3.12",
+#     packages=setuptools.find_packages(),
+#     include_package_data=True,
+#     entry_points={"console_scripts": ["paper = paper.cli:main"]},
+
+# )
+
+extensions = [
+    Extension("ScholarCodeCollective.Community_Representatives_main.functions",
+              ["ScholarCodeCollective/Community_Representatives_main/functions.pyx"],
+              language='c++')  # use 'c' if not using C++ features
+]
+
+setup(
     name='ScholarCodeCollective',
-    version='0.1.4',
+    version='0.1.5',
     description='A collective library for the code behind several academic papers',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://google.com',
-    author='Author Name', 
+    author='Author Name',
     author_email='author_email@mail.com',
     license='The Unlicense',
     projects_urls={
         "Documentation": "x",
         "Source": "https://github.com"
     },
-    python_requires=">3.9,<3.12",
-    packages=setuptools.find_packages(),
+    python_requires=">=3.9, <3.12",
+    packages=find_packages(),
     include_package_data=True,
     entry_points={"console_scripts": ["paper = paper.cli:main"]},
-
+    ext_modules=cythonize(extensions, compiler_directives={'language_level': "3"})
 )
```

### Comparing `ScholarCodeCollective-0.1.4/tests/__init__.py` & `ScholarCodeCollective-0.1.5/tests/__init__.py`

 * *Files identical despite different names*

