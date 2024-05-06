# Comparing `tmp/ScholarCodeCollective-0.1.6.tar.gz` & `tmp/ScholarCodeCollective-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScholarCodeCollective-0.1.6.tar", last modified: Mon May  6 18:00:28 2024, max compression
+gzip compressed data, was "ScholarCodeCollective-0.1.7.tar", last modified: Mon May  6 18:08:45 2024, max compression
```

## Comparing `ScholarCodeCollective-0.1.6.tar` & `ScholarCodeCollective-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.170947 ScholarCodeCollective-0.1.6/
--rw-rw-rw-   0        0        0     3784 2024-05-06 18:00:28.169946 ScholarCodeCollective-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2644 2024-04-21 08:44:00.000000 ScholarCodeCollective-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.118906 ScholarCodeCollective-0.1.6/ScholarCodeCollective/
-drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.148470 ScholarCodeCollective-0.1.6/ScholarCodeCollective/Community_Representatives_main/
--rw-rw-rw-   0        0        0       26 2024-05-06 17:39:11.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/Community_Representatives_main/__init__.py
--rw-rw-rw-   0        0        0  1889833 2024-05-06 17:54:05.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/Community_Representatives_main/functions.cpp
-drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.153983 ScholarCodeCollective-0.1.6/ScholarCodeCollective/MDL_network_population_clustering_main/
--rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
--rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.157988 ScholarCodeCollective-0.1.6/ScholarCodeCollective/MDL_regionalization_main/
--rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/MDL_regionalization_main/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 11:59:09.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/MDL_regionalization_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.162504 ScholarCodeCollective-0.1.6/ScholarCodeCollective/Network_hubs_main/
--rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/Network_hubs_main/__init__.py
--rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/Network_hubs_main/functions.py
--rw-rw-rw-   0        0        0      129 2024-04-23 12:14:08.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.165939 ScholarCodeCollective-0.1.6/ScholarCodeCollective/hypergraph_binning_main/
--rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/hypergraph_binning_main/__init__.py
--rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective/hypergraph_binning_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.138335 ScholarCodeCollective-0.1.6/ScholarCodeCollective.egg-info/
--rw-rw-rw-   0        0        0     3784 2024-05-06 18:00:27.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1014 2024-05-06 18:00:28.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 18:00:27.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-06 18:00:27.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-05-06 18:00:27.000000 ScholarCodeCollective-0.1.6/ScholarCodeCollective.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 18:00:28.170947 ScholarCodeCollective-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1925 2024-05-06 18:00:19.000000 ScholarCodeCollective-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:00:28.167953 ScholarCodeCollective-0.1.6/tests/
--rw-rw-rw-   0        0        0     1010 2024-04-22 17:16:16.000000 ScholarCodeCollective-0.1.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.722256 ScholarCodeCollective-0.1.7/
+-rw-rw-rw-   0        0        0     2093 2024-05-06 18:08:45.720252 ScholarCodeCollective-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1394 2024-05-06 18:08:29.000000 ScholarCodeCollective-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.661272 ScholarCodeCollective-0.1.7/ScholarCodeCollective/
+drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.696332 ScholarCodeCollective-0.1.7/ScholarCodeCollective/Community_Representatives_main/
+-rw-rw-rw-   0        0        0       26 2024-05-06 17:39:11.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/Community_Representatives_main/__init__.py
+-rw-rw-rw-   0        0        0  1889833 2024-05-06 17:54:05.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/Community_Representatives_main/functions.cpp
+drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.701283 ScholarCodeCollective-0.1.7/ScholarCodeCollective/MDL_network_population_clustering_main/
+-rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
+-rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.706306 ScholarCodeCollective-0.1.7/ScholarCodeCollective/MDL_regionalization_main/
+-rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/MDL_regionalization_main/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 11:59:09.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/MDL_regionalization_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.710735 ScholarCodeCollective-0.1.7/ScholarCodeCollective/Network_hubs_main/
+-rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/Network_hubs_main/__init__.py
+-rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/Network_hubs_main/functions.py
+-rw-rw-rw-   0        0        0      129 2024-04-23 12:14:08.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.715802 ScholarCodeCollective-0.1.7/ScholarCodeCollective/hypergraph_binning_main/
+-rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/hypergraph_binning_main/__init__.py
+-rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective/hypergraph_binning_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.688212 ScholarCodeCollective-0.1.7/ScholarCodeCollective.egg-info/
+-rw-rw-rw-   0        0        0     2093 2024-05-06 18:08:45.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1014 2024-05-06 18:08:45.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 18:08:45.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-06 18:08:45.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-05-06 18:08:45.000000 ScholarCodeCollective-0.1.7/ScholarCodeCollective.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 18:08:45.722256 ScholarCodeCollective-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1925 2024-05-06 18:08:36.000000 ScholarCodeCollective-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:08:45.718255 ScholarCodeCollective-0.1.7/tests/
+-rw-rw-rw-   0        0        0     1010 2024-04-22 17:16:16.000000 ScholarCodeCollective-0.1.7/tests/__init__.py
```

### Comparing `ScholarCodeCollective-0.1.6/PKG-INFO` & `ScholarCodeCollective-0.1.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.6
+Version: 0.1.7
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
@@ -27,68 +27,36 @@
 â”‚Â Â  â””â”€â”€ package_2
 â”‚Â Â      â”œâ”€â”€ __init__.py
 â”‚Â Â      â””â”€â”€ module.py
 â”œâ”€â”€ setup.py
 â””â”€â”€ tests
     â””â”€â”€ __init__.py
 ```
-### (Optional) Create a Python environment: 
+### Command for wheel creation and upload 
 * For Python3 users: 
-  * `pip install virtualenv`
-  * `virtualenv venv_name`
-  * `source path/to/venv_name activate`
-* For Anaconda users: 
-  * `conda create --name conda_env`
-  * `conda activate conda_env`
-  * `conda install pip`
+  * `python setup.py sdist`
+  * `del dist\*`
+  * `stwine upload --verbose dist/*    `
 
-### Next you need to create a `setup.py`  file in the root folder. It should be similar to the one presented below: 
-```
-from distutils.core import setup
-from setuptools import setup, find_packages
+# ScholarCodeCollective Package
 
-setup(
-    name='example',
-    version='0.1dev0',
-    author='Author Name', 
-    author_email='author_email@mail.com',
-    packages=find_packages(),
-    long_description=open('README.md').read()
-)
-```
-### You need to create an **`__init__.py`** file in the `/example` directory where you should **import the packages** (i.e. `package_1`, and `package_2`): 
-```
-# example/__init__.py
-from . import package_1, package_2 
-```
+Welcome to the ScholarCodeCollective package. Below you will find links to various resources including our local documentation.
 
-### After that, you need to run the `setup.py` as follows: 
-#### While being in the root of the folder run the following command: `pip install -e .`
-An `example.egg-info` directory should now be created in the root directory: 
-```
-project
-â”œâ”€â”€ README.md
-â”œâ”€â”€ example
-â”‚Â Â  â”œâ”€â”€ __init__.py
-â”‚Â Â  â”œâ”€â”€ package_1
-â”‚Â Â  â”‚Â Â  â”œâ”€â”€ __init__.py
-â”‚Â Â  â”‚Â Â  â”œâ”€â”€ awesome_module.py
-â”‚Â Â  â”‚Â Â  â”œâ”€â”€ ...
-â”‚Â Â  â”‚Â Â  â””â”€â”€ awesome_module_n.py
-â”‚Â Â  â””â”€â”€ package_2
-â”‚Â Â      â”œâ”€â”€ __init__.py
-â”‚Â Â      â””â”€â”€ module.py
-â”œâ”€â”€ example.egg-info
-â”‚   â”œâ”€â”€ dependency_links.txt
-â”‚   â”œâ”€â”€ PKG_INFO
-â”‚   â”œâ”€â”€ SOURCES.txt
-â”‚   â””â”€â”€ top_level.txt
-â”œâ”€â”€ setup.py
-â””â”€â”€ tests
-    â””â”€â”€ __init__.py
-```
-If everything when according to plan, you should be able to use the modules you developed in the `package_1` from the `package_2` directory likewise: 
+## Documentation
 
-```
-# example/package_2/module.py
-from example.package_1.awesome_module import hello
-```
+For detailed documentation, please refer to our [local documentation](file:///D:/Research%20HKU/PYPI_lib/Documentation/_build/html/index.html).
+
+## Installation
+
+Provide installation instructions here.
+
+## Usage
+
+Provide usage instructions here.
+
+## Contributing
+
+Guidelines for how to contribute to the project.
+
+## License
+
+Information about the licensing.
```

### Comparing `ScholarCodeCollective-0.1.6/ScholarCodeCollective/Community_Representatives_main/functions.cpp` & `ScholarCodeCollective-0.1.7/ScholarCodeCollective/Community_Representatives_main/functions.cpp`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.6/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py` & `ScholarCodeCollective-0.1.7/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.6/ScholarCodeCollective/MDL_regionalization_main/functions.py` & `ScholarCodeCollective-0.1.7/ScholarCodeCollective/MDL_regionalization_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.6/ScholarCodeCollective/Network_hubs_main/functions.py` & `ScholarCodeCollective-0.1.7/ScholarCodeCollective/Network_hubs_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.6/ScholarCodeCollective/hypergraph_binning_main/functions.py` & `ScholarCodeCollective-0.1.7/ScholarCodeCollective/hypergraph_binning_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.6/ScholarCodeCollective.egg-info/PKG-INFO` & `ScholarCodeCollective-0.1.7/ScholarCodeCollective.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.6
+Version: 0.1.7
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
@@ -27,68 +27,36 @@
 â”‚Â Â  â””â”€â”€ package_2
 â”‚Â Â      â”œâ”€â”€ __init__.py
 â”‚Â Â      â””â”€â”€ module.py
 â”œâ”€â”€ setup.py
 â””â”€â”€ tests
     â””â”€â”€ __init__.py
 ```
-### (Optional) Create a Python environment: 
+### Command for wheel creation and upload 
 * For Python3 users: 
-  * `pip install virtualenv`
-  * `virtualenv venv_name`
-  * `source path/to/venv_name activate`
-* For Anaconda users: 
-  * `conda create --name conda_env`
-  * `conda activate conda_env`
-  * `conda install pip`
+  * `python setup.py sdist`
+  * `del dist\*`
+  * `stwine upload --verbose dist/*    `
 
-### Next you need to create a `setup.py`  file in the root folder. It should be similar to the one presented below: 
-```
-from distutils.core import setup
-from setuptools import setup, find_packages
+# ScholarCodeCollective Package
 
-setup(
-    name='example',
-    version='0.1dev0',
-    author='Author Name', 
-    author_email='author_email@mail.com',
-    packages=find_packages(),
-    long_description=open('README.md').read()
-)
-```
-### You need to create an **`__init__.py`** file in the `/example` directory where you should **import the packages** (i.e. `package_1`, and `package_2`): 
-```
-# example/__init__.py
-from . import package_1, package_2 
-```
+Welcome to the ScholarCodeCollective package. Below you will find links to various resources including our local documentation.
 
-### After that, you need to run the `setup.py` as follows: 
-#### While being in the root of the folder run the following command: `pip install -e .`
-An `example.egg-info` directory should now be created in the root directory: 
-```
-project
-â”œâ”€â”€ README.md
-â”œâ”€â”€ example
-â”‚Â Â  â”œâ”€â”€ __init__.py
-â”‚Â Â  â”œâ”€â”€ package_1
-â”‚Â Â  â”‚Â Â  â”œâ”€â”€ __init__.py
-â”‚Â Â  â”‚Â Â  â”œâ”€â”€ awesome_module.py
-â”‚Â Â  â”‚Â Â  â”œâ”€â”€ ...
-â”‚Â Â  â”‚Â Â  â””â”€â”€ awesome_module_n.py
-â”‚Â Â  â””â”€â”€ package_2
-â”‚Â Â      â”œâ”€â”€ __init__.py
-â”‚Â Â      â””â”€â”€ module.py
-â”œâ”€â”€ example.egg-info
-â”‚   â”œâ”€â”€ dependency_links.txt
-â”‚   â”œâ”€â”€ PKG_INFO
-â”‚   â”œâ”€â”€ SOURCES.txt
-â”‚   â””â”€â”€ top_level.txt
-â”œâ”€â”€ setup.py
-â””â”€â”€ tests
-    â””â”€â”€ __init__.py
-```
-If everything when according to plan, you should be able to use the modules you developed in the `package_1` from the `package_2` directory likewise: 
+## Documentation
 
-```
-# example/package_2/module.py
-from example.package_1.awesome_module import hello
-```
+For detailed documentation, please refer to our [local documentation](file:///D:/Research%20HKU/PYPI_lib/Documentation/_build/html/index.html).
+
+## Installation
+
+Provide installation instructions here.
+
+## Usage
+
+Provide usage instructions here.
+
+## Contributing
+
+Guidelines for how to contribute to the project.
+
+## License
+
+Information about the licensing.
```

### Comparing `ScholarCodeCollective-0.1.6/ScholarCodeCollective.egg-info/SOURCES.txt` & `ScholarCodeCollective-0.1.7/ScholarCodeCollective.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.6/setup.py` & `ScholarCodeCollective-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     Extension("ScholarCodeCollective.Community_Representatives_main.functions",
               ["ScholarCodeCollective/Community_Representatives_main/functions.pyx"],
               language='c++')  # use 'c' if not using C++ features
 ]
 
 setup(
     name='ScholarCodeCollective',
-    version='0.1.6',
+    version='0.1.7',
     description='A collective library for the code behind several academic papers',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://google.com',
     author='Author Name',
     author_email='author_email@mail.com',
     license='The Unlicense',
```

### Comparing `ScholarCodeCollective-0.1.6/tests/__init__.py` & `ScholarCodeCollective-0.1.7/tests/__init__.py`

 * *Files identical despite different names*

