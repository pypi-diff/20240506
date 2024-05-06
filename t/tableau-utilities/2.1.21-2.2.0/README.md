# Comparing `tmp/tableau_utilities-2.1.21.tar.gz` & `tmp/tableau_utilities-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableau_utilities-2.1.21.tar", last modified: Tue Mar 19 20:39:16 2024, max compression
+gzip compressed data, was "tableau_utilities-2.2.0.tar", last modified: Mon May  6 16:59:27 2024, max compression
```

## Comparing `tableau_utilities-2.1.21.tar` & `tableau_utilities-2.2.0.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-03-19 20:39:16.094287 tableau_utilities-2.1.21/
--rw-r--r--   0 justin     (502) staff       (20)     1062 2022-05-25 18:48:01.000000 tableau_utilities-2.1.21/LICENSE
--rw-r--r--   0 justin     (502) staff       (20)     8650 2024-03-19 20:39:16.092597 tableau_utilities-2.1.21/PKG-INFO
--rw-r--r--   0 justin     (502) staff       (20)     8116 2024-02-29 16:48:52.000000 tableau_utilities-2.1.21/README.md
--rw-r--r--   0 justin     (502) staff       (20)       38 2024-03-19 20:39:16.094781 tableau_utilities-2.1.21/setup.cfg
--rw-r--r--   0 justin     (502) staff       (20)     1160 2024-03-19 20:32:05.000000 tableau_utilities-2.1.21/setup.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-03-19 20:39:16.030841 tableau_utilities-2.1.21/tableau_utilities/
--rw-r--r--   0 justin     (502) staff       (20)      306 2024-02-29 16:48:52.000000 tableau_utilities-2.1.21/tableau_utilities/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)     2441 2024-02-29 16:48:52.000000 tableau_utilities-2.1.21/tableau_utilities/fetch_all_cols.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-03-19 20:39:16.046707 tableau_utilities-2.1.21/tableau_utilities/general/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.1.21/tableau_utilities/general/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)     2235 2023-06-28 16:57:49.000000 tableau_utilities-2.1.21/tableau_utilities/general/cli_styling.py
--rw-r--r--   0 justin     (502) staff       (20)     3497 2023-06-28 16:57:49.000000 tableau_utilities-2.1.21/tableau_utilities/general/config_column_persona.py
--rw-r--r--   0 justin     (502) staff       (20)     2278 2023-06-28 16:57:49.000000 tableau_utilities-2.1.21/tableau_utilities/general/funcs.py
--rw-r--r--   0 justin     (502) staff       (20)     3030 2024-03-19 15:11:11.000000 tableau_utilities-2.1.21/tableau_utilities/scripted_testing.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-03-19 20:39:16.061151 tableau_utilities-2.1.21/tableau_utilities/scripts/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.1.21/tableau_utilities/scripts/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    23657 2024-03-19 19:20:15.000000 tableau_utilities-2.1.21/tableau_utilities/scripts/cli.py
--rw-r--r--   0 justin     (502) staff       (20)     1772 2023-06-28 16:57:49.000000 tableau_utilities-2.1.21/tableau_utilities/scripts/csv_config.py
--rw-r--r--   0 justin     (502) staff       (20)     9011 2024-03-19 19:20:15.000000 tableau_utilities-2.1.21/tableau_utilities/scripts/datasource.py
--rw-r--r--   0 justin     (502) staff       (20)    13151 2024-02-29 16:48:52.000000 tableau_utilities-2.1.21/tableau_utilities/scripts/gen_config.py
--rw-r--r--   0 justin     (502) staff       (20)     8539 2023-06-28 16:57:49.000000 tableau_utilities-2.1.21/tableau_utilities/scripts/merge_config.py
--rw-r--r--   0 justin     (502) staff       (20)     1867 2024-02-29 16:48:52.000000 tableau_utilities-2.1.21/tableau_utilities/scripts/server_info.py
--rw-r--r--   0 justin     (502) staff       (20)     4511 2024-02-29 16:48:52.000000 tableau_utilities-2.1.21/tableau_utilities/scripts/server_operate.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-03-19 20:39:16.065921 tableau_utilities-2.1.21/tableau_utilities/tableau_file/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.1.21/tableau_utilities/tableau_file/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)    20871 2024-03-19 20:37:51.000000 tableau_utilities-2.1.21/tableau_utilities/tableau_file/tableau_file.py
--rw-r--r--   0 justin     (502) staff       (20)    38102 2023-10-24 17:53:15.000000 tableau_utilities-2.1.21/tableau_utilities/tableau_file/tableau_file_objects.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-03-19 20:39:16.087388 tableau_utilities-2.1.21/tableau_utilities/tableau_server/
--rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.1.21/tableau_utilities/tableau_server/__init__.py
--rw-r--r--   0 justin     (502) staff       (20)     2450 2024-03-01 20:30:48.000000 tableau_utilities-2.1.21/tableau_utilities/tableau_server/base.py
--rw-r--r--   0 justin     (502) staff       (20)     1330 2024-03-01 20:30:48.000000 tableau_utilities-2.1.21/tableau_utilities/tableau_server/create.py
--rw-r--r--   0 justin     (502) staff       (20)     2193 2024-03-01 20:30:48.000000 tableau_utilities-2.1.21/tableau_utilities/tableau_server/download.py
--rw-r--r--   0 justin     (502) staff       (20)     9893 2024-03-01 20:30:48.000000 tableau_utilities-2.1.21/tableau_utilities/tableau_server/get.py
--rw-r--r--   0 justin     (502) staff       (20)    12043 2024-03-04 16:14:39.000000 tableau_utilities-2.1.21/tableau_utilities/tableau_server/publish.py
--rw-r--r--   0 justin     (502) staff       (20)      891 2024-03-01 20:30:48.000000 tableau_utilities-2.1.21/tableau_utilities/tableau_server/refresh.py
--rw-r--r--   0 justin     (502) staff       (20)     1484 2024-03-01 20:30:48.000000 tableau_utilities-2.1.21/tableau_utilities/tableau_server/static.py
--rw-r--r--   0 justin     (502) staff       (20)     5309 2024-02-29 16:48:52.000000 tableau_utilities-2.1.21/tableau_utilities/tableau_server/tableau_server.py
--rw-r--r--   0 justin     (502) staff       (20)    13195 2023-06-28 16:57:49.000000 tableau_utilities-2.1.21/tableau_utilities/tableau_server/tableau_server_objects.py
--rw-r--r--   0 justin     (502) staff       (20)     1393 2024-03-01 20:30:48.000000 tableau_utilities-2.1.21/tableau_utilities/tableau_server/update.py
--rw-r--r--   0 justin     (502) staff       (20)    11595 2023-10-24 17:53:15.000000 tableau_utilities-2.1.21/tableau_utilities/test_tableau_utilities.py
-drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-03-19 20:39:16.090200 tableau_utilities-2.1.21/tableau_utilities.egg-info/
--rw-r--r--   0 justin     (502) staff       (20)     8650 2024-03-19 20:39:15.000000 tableau_utilities-2.1.21/tableau_utilities.egg-info/PKG-INFO
--rw-r--r--   0 justin     (502) staff       (20)     1548 2024-03-19 20:39:15.000000 tableau_utilities-2.1.21/tableau_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 justin     (502) staff       (20)        1 2024-03-19 20:39:15.000000 tableau_utilities-2.1.21/tableau_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 justin     (502) staff       (20)       73 2024-03-19 20:39:15.000000 tableau_utilities-2.1.21/tableau_utilities.egg-info/entry_points.txt
--rw-r--r--   0 justin     (502) staff       (20)      139 2024-03-19 20:39:15.000000 tableau_utilities-2.1.21/tableau_utilities.egg-info/requires.txt
--rw-r--r--   0 justin     (502) staff       (20)       18 2024-03-19 20:39:15.000000 tableau_utilities-2.1.21/tableau_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-06 16:59:27.521078 tableau_utilities-2.2.0/
+-rw-r--r--   0 justin     (502) staff       (20)     1062 2022-05-25 18:48:01.000000 tableau_utilities-2.2.0/LICENSE
+-rw-r--r--   0 justin     (502) staff       (20)     9118 2024-05-06 16:59:27.520434 tableau_utilities-2.2.0/PKG-INFO
+-rw-r--r--   0 justin     (502) staff       (20)     8544 2024-05-06 16:48:53.000000 tableau_utilities-2.2.0/README.md
+-rw-r--r--   0 justin     (502) staff       (20)       38 2024-05-06 16:59:27.521216 tableau_utilities-2.2.0/setup.cfg
+-rw-r--r--   0 justin     (502) staff       (20)     1257 2024-05-06 16:48:53.000000 tableau_utilities-2.2.0/setup.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-06 16:59:27.495027 tableau_utilities-2.2.0/tableau_utilities/
+-rw-r--r--   0 justin     (502) staff       (20)      306 2024-02-29 16:48:52.000000 tableau_utilities-2.2.0/tableau_utilities/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     2441 2024-02-29 16:48:52.000000 tableau_utilities-2.2.0/tableau_utilities/fetch_all_cols.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-06 16:59:27.500756 tableau_utilities-2.2.0/tableau_utilities/general/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/general/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     2235 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/general/cli_styling.py
+-rw-r--r--   0 justin     (502) staff       (20)     3497 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/general/config_column_persona.py
+-rw-r--r--   0 justin     (502) staff       (20)     2278 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/general/funcs.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-06 16:59:27.501752 tableau_utilities-2.2.0/tableau_utilities/hyper/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2024-05-06 16:48:53.000000 tableau_utilities-2.2.0/tableau_utilities/hyper/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     5929 2024-05-06 16:48:53.000000 tableau_utilities-2.2.0/tableau_utilities/hyper/hyper.py
+-rw-r--r--   0 justin     (502) staff       (20)     3030 2024-03-20 15:25:53.000000 tableau_utilities-2.2.0/tableau_utilities/scripted_testing.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-06 16:59:27.507853 tableau_utilities-2.2.0/tableau_utilities/scripts/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/scripts/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    24339 2024-05-06 16:48:53.000000 tableau_utilities-2.2.0/tableau_utilities/scripts/cli.py
+-rw-r--r--   0 justin     (502) staff       (20)     1772 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/scripts/csv_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     9121 2024-05-06 16:58:26.000000 tableau_utilities-2.2.0/tableau_utilities/scripts/datasource.py
+-rw-r--r--   0 justin     (502) staff       (20)    13151 2024-02-29 16:48:52.000000 tableau_utilities-2.2.0/tableau_utilities/scripts/gen_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     8539 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/scripts/merge_config.py
+-rw-r--r--   0 justin     (502) staff       (20)     1867 2024-02-29 16:48:52.000000 tableau_utilities-2.2.0/tableau_utilities/scripts/server_info.py
+-rw-r--r--   0 justin     (502) staff       (20)     4511 2024-05-03 15:27:55.000000 tableau_utilities-2.2.0/tableau_utilities/scripts/server_operate.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-06 16:59:27.509921 tableau_utilities-2.2.0/tableau_utilities/tableau_file/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_file/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)    15040 2024-05-06 16:48:53.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_file/tableau_file.py
+-rw-r--r--   0 justin     (502) staff       (20)    38250 2024-05-06 16:48:53.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_file/tableau_file_objects.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-06 16:59:27.518511 tableau_utilities-2.2.0/tableau_utilities/tableau_server/
+-rw-r--r--   0 justin     (502) staff       (20)        0 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/__init__.py
+-rw-r--r--   0 justin     (502) staff       (20)     2450 2024-03-01 20:30:48.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/base.py
+-rw-r--r--   0 justin     (502) staff       (20)     1330 2024-03-01 20:30:48.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/create.py
+-rw-r--r--   0 justin     (502) staff       (20)     2193 2024-03-01 20:30:48.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/download.py
+-rw-r--r--   0 justin     (502) staff       (20)     9893 2024-03-01 20:30:48.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/get.py
+-rw-r--r--   0 justin     (502) staff       (20)    12043 2024-03-04 16:14:39.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/publish.py
+-rw-r--r--   0 justin     (502) staff       (20)      891 2024-03-01 20:30:48.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/refresh.py
+-rw-r--r--   0 justin     (502) staff       (20)     1484 2024-03-01 20:30:48.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/static.py
+-rw-r--r--   0 justin     (502) staff       (20)     5309 2024-02-29 16:48:52.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/tableau_server.py
+-rw-r--r--   0 justin     (502) staff       (20)    13195 2023-06-28 16:57:49.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/tableau_server_objects.py
+-rw-r--r--   0 justin     (502) staff       (20)     1393 2024-03-01 20:30:48.000000 tableau_utilities-2.2.0/tableau_utilities/tableau_server/update.py
+-rw-r--r--   0 justin     (502) staff       (20)    11595 2023-10-24 17:53:15.000000 tableau_utilities-2.2.0/tableau_utilities/test_tableau_utilities.py
+drwxr-xr-x   0 justin     (502) staff       (20)        0 2024-05-06 16:59:27.519436 tableau_utilities-2.2.0/tableau_utilities.egg-info/
+-rw-r--r--   0 justin     (502) staff       (20)     9118 2024-05-06 16:59:27.000000 tableau_utilities-2.2.0/tableau_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 justin     (502) staff       (20)     1617 2024-05-06 16:59:27.000000 tableau_utilities-2.2.0/tableau_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 justin     (502) staff       (20)        1 2024-05-06 16:59:27.000000 tableau_utilities-2.2.0/tableau_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 justin     (502) staff       (20)       73 2024-05-06 16:59:27.000000 tableau_utilities-2.2.0/tableau_utilities.egg-info/entry_points.txt
+-rw-r--r--   0 justin     (502) staff       (20)      148 2024-05-06 16:59:27.000000 tableau_utilities-2.2.0/tableau_utilities.egg-info/requires.txt
+-rw-r--r--   0 justin     (502) staff       (20)       18 2024-05-06 16:59:27.000000 tableau_utilities-2.2.0/tableau_utilities.egg-info/top_level.txt
```

### Comparing `tableau_utilities-2.1.21/LICENSE` & `tableau_utilities-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/PKG-INFO` & `tableau_utilities-2.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 Metadata-Version: 2.1
 Name: tableau_utilities
-Version: 2.1.21
+Version: 2.2.0
 Summary: Utility for maintaining Tableau objects
 Home-page: http://pypi.python.org/pypi/tableau-utilities/
 Author: Justin Grilli
 Author-email: justin.grilli@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: xmltodict<1.0.0,>=0.12.0
 Requires-Dist: pyyaml<7.0.0,>=6.0
 Requires-Dist: requests<3.0.0,>=2.27.1
 Requires-Dist: pandas<2.0.0,>=1.4.1
 Requires-Dist: tabulate<1.0.0,>=0.8.9
-Requires-Dist: tableauhyperapi==0.0.18825
+Provides-Extra: hyper
+Requires-Dist: tableauhyperapi==0.0.18825; extra == "hyper"
 
 # tableau-utilities
 
 A module and CLI Utility for managing Tableau objects, locally, and in Tableau Online.
 
 ## Quick start
 
 ### Installation
 
 #### From pypi
+
+##### Core Package
 - `pip install tableau-utilities`
 
+##### Hyper Subpackage
+This extra package depends on the tableauhyperapi which is incompatible with Apple Silicon computers.  See the [tableauhyperapi installation docs](https://tableau.github.io/hyper-db/docs/installation) for workarounds to use the package on Applie Silicon.
+
+- `pip install tableau-utilities[hyper]`
+- `pip install 'tableau-utilities[hyper]'`  if you're using zsh make sure to add quotes
+
 #### Locally using pip
 - `cd tableau-utilities`
 - `pip install ./`
 
 #### Confirm installation
 - `which tableau_utilities`
   - _Describes where tableau-utilities has been installed_
```

### Comparing `tableau_utilities-2.1.21/README.md` & `tableau_utilities-2.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,24 @@
 A module and CLI Utility for managing Tableau objects, locally, and in Tableau Online.
 
 ## Quick start
 
 ### Installation
 
 #### From pypi
+
+##### Core Package
 - `pip install tableau-utilities`
 
+##### Hyper Subpackage
+This extra package depends on the tableauhyperapi which is incompatible with Apple Silicon computers.  See the [tableauhyperapi installation docs](https://tableau.github.io/hyper-db/docs/installation) for workarounds to use the package on Applie Silicon.
+
+- `pip install tableau-utilities[hyper]`
+- `pip install 'tableau-utilities[hyper]'`  if you're using zsh make sure to add quotes
+
 #### Locally using pip
 - `cd tableau-utilities`
 - `pip install ./`
 
 #### Confirm installation
 - `which tableau_utilities`
   - _Describes where tableau-utilities has been installed_
@@ -203,8 +211,8 @@
   - Add tests as needed
   - Run when making changes
 
 ## Maintenance
 
 This project is actively maintained by the Data Platform team at [@hoverinc][hover-github-link].
 
-[hover-github-link]: https://github.com/hoverinc
+[hover-github-link]: https://github.com/hoverinc
```

### Comparing `tableau_utilities-2.1.21/setup.py` & `tableau_utilities-2.2.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,29 +8,32 @@
     author_email="justin.grilli@gmail.com",
     license='MIT',
     url='http://pypi.python.org/pypi/tableau-utilities/',
     description='Utility for maintaining Tableau objects',
     long_description=readme,
     long_description_content_type='text/markdown',
     name="tableau_utilities",
-    version="2.1.21",
+    version="2.2.0",
+    requires_python=">=3.8",
     packages=[
         'tableau_utilities',
         'tableau_utilities.general',
         'tableau_utilities.tableau_file',
         'tableau_utilities.tableau_server',
-        'tableau_utilities.scripts'
+        'tableau_utilities.hyper',
+        'tableau_utilities.scripts',
     ],
     package_data={'tableau_utilities': ['tableau_file/*.yml']},
     include_package_data=True,
     install_requires=['xmltodict>=0.12.0,<1.0.0',
                       'pyyaml>=6.0,<7.0.0',
                       'requests>=2.27.1,<3.0.0',
                       'pandas>=1.4.1,<2.0.0',
                       'tabulate>=0.8.9,<1.0.0',
-                      'tableauhyperapi==0.0.18825'],
+                      ],
+    extras_require={"hyper": ['tableauhyperapi==0.0.18825']},
     entry_points={
         'console_scripts': [
             'tableau_utilities = tableau_utilities.scripts.cli:main',
         ]
     }
-)
+)
```

### Comparing `tableau_utilities-2.1.21/tableau_utilities/fetch_all_cols.py` & `tableau_utilities-2.2.0/tableau_utilities/fetch_all_cols.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/general/cli_styling.py` & `tableau_utilities-2.2.0/tableau_utilities/general/cli_styling.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/general/config_column_persona.py` & `tableau_utilities-2.2.0/tableau_utilities/general/config_column_persona.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/general/funcs.py` & `tableau_utilities-2.2.0/tableau_utilities/general/funcs.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/scripted_testing.py` & `tableau_utilities-2.2.0/tableau_utilities/scripted_testing.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/scripts/cli.py` & `tableau_utilities-2.2.0/tableau_utilities/scripts/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import argparse
 import os
 import shutil
 from argparse import RawTextHelpFormatter
 import yaml
 import pkg_resources
+import pkgutil
+import importlib.metadata
 
 import tableau_utilities.tableau_server.tableau_server as ts
 
 from tableau_utilities.general.config_column_persona import personas
 from tableau_utilities.general.cli_styling import Color, Symbol, color_print
 from tableau_utilities.scripts.gen_config import generate_config
 from tableau_utilities.scripts.merge_config import merge_configs
@@ -153,17 +155,17 @@
 parser_datasource.add_argument('--caption', help='Short name/Alias for the column')
 parser_datasource.add_argument('--title_case_caption', action='store_true',
                                help='Converts caption to title case. Applied after --caption')
 parser_datasource.add_argument('--persona', choices=list(personas.keys()),
                                help='The datatype persona of the column. Required for adding a new column')
 parser_datasource.add_argument('--desc', help='A Tableau column description')
 parser_datasource.add_argument('--calculation', help='A Tableau calculation')
-parser_datasource.add_argument('-E', '--empty_extract', action='store_true',
+parser_datasource.add_argument('-ee', '--empty_extract', action='store_true',
                                help='Adds an empty extract to the Datasource if specified.')
-parser_datasource.add_argument('-F', '--filter_extract',
+parser_datasource.add_argument('-fe', '--filter_extract',
                                help='Deletes data from the extract based on the condition string provided. '
                                     """E.g. "CREATED_AT" < '1/1/2024'""")
 parser_datasource.set_defaults(func=datasource)
 
 # GENERATE CONFIG
 parser_config_gen = subparsers.add_parser(
     'generate_config', help='Generate configs to programmatically manage metadata in Tableau '
@@ -258,14 +260,24 @@
         parser.error(f'--merge_with {args.merge_with} requires --definitions_csv')
     if args.merge_with == 'config' and args.additional_config is None:
         parser.error(f'--merge_with {args.merge_with} requires --existing_config')
     if args.merge_with == 'generate_merge_all' and args.target_directory is None:
         parser.error(f'--merge_with {args.merge_with} requires --target_directory')
 
 
+def validate_subpackage_hyper():
+    """ Checks that the hyper subpackage is installed for functions that use it """
+
+    try:
+        version = importlib.metadata.version("tableauhyperapi")
+    except importlib.metadata.PackageNotFoundError:
+        parser.error(
+            '--filter_extract and --empty_extract require the tableau_utilities[hyper] subpackage.  See installation notes if you are on an Apple Silicon (Apple M1, Apple M2, ...)')
+
+
 def tableau_authentication(args):
     """ Creates the Tableau server authentication from a variety of methods for passing in credentials """
     debug = args.debugging_logs
     yaml_path = args.settings_path
     color = Color()
     symbol = Symbol()
 
@@ -449,26 +461,33 @@
     tmp_folder = args.output_dir
     if args.clean_dir:
         shutil.rmtree(tmp_folder, ignore_errors=True)
 
     os.makedirs(tmp_folder, exist_ok=True)
     os.chdir(tmp_folder)
 
+    needs_subpackage_hyper = (
+        args.command == 'datasource' and (args.empty_extract or args.filter_extract)
+    )
+
     needs_tableau_server = (
         (args.command == 'generate_config' and args.location == 'online')
         or (args.command == 'merge_config' and args.location == 'online')
         or (args.command == 'datasource' and args.location == 'online')
         or (args.command == 'connection' and args.connection_operation == 'embed_user_pass')
         or args.command == 'server_info'
         or args.command == 'server_operate'
     )
 
+    if needs_subpackage_hyper:
+        validate_subpackage_hyper()
+
     if needs_tableau_server:
         server = tableau_authentication(args)
         args.func(args, server)
     # Run functions that don't need the server
     else:
         args.func(args)
 
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `tableau_utilities-2.1.21/tableau_utilities/scripts/csv_config.py` & `tableau_utilities-2.2.0/tableau_utilities/scripts/csv_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/scripts/datasource.py` & `tableau_utilities-2.2.0/tableau_utilities/scripts/datasource.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from time import time
 from tableau_utilities.general.config_column_persona import personas, get_persona_by_attribs, \
     get_persona_by_metadata_local_type
 from tableau_utilities.general.cli_styling import Color
 from tableau_utilities.general.cli_styling import Symbol
 from tableau_utilities.tableau_file.tableau_file import Datasource
 from tableau_utilities.tableau_server.tableau_server import TableauServer
+from tableau_utilities.hyper.hyper import create_empty_hyper_extract, filter_hyper_extract
 
 
 def datasource(args, server=None):
     """ Updates a Tableau Datasource locally
 
     Args:
         args: An argparse args object
@@ -69,21 +70,21 @@
               f'Downloaded Datasource: {color.fg_yellow}{datasource_path}{color.reset}\n')
 
     datasource_file_name = os.path.basename(datasource_path)
     ds = Datasource(datasource_path)
 
     # Add an empty .hyper file to the Datasource; Useful for publishing without data
     if empty_extract:
-        ds.empty_extract()
+        create_empty_hyper_extract(ds)
         print(f'{color.fg_green}Added empty .hyper extract for {datasource_path}{color.reset}')
     # Otherwise, filter the extract if filter_extract string provided
     elif filter_extract:
         start = time()
         print(f'{color.fg_cyan}...Filtering extract data...{color.reset}')
-        ds.filter_extract(filter_extract)
+        filter_hyper_extract(ds, filter_extract)
         print(f'{color.fg_green}{symbol.success} (Done in {round(time() - start)} sec) '
               f'Filtered extract data for {datasource_path}{color.reset}')
 
     if save_tds:
         start = time()
         print(f'{color.fg_cyan}...Extracting {datasource_file_name}...{color.reset}')
         save_folder = f'{datasource_file_name} - BEFORE'
```

### Comparing `tableau_utilities-2.1.21/tableau_utilities/scripts/gen_config.py` & `tableau_utilities-2.2.0/tableau_utilities/scripts/gen_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/scripts/merge_config.py` & `tableau_utilities-2.2.0/tableau_utilities/scripts/merge_config.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/scripts/server_info.py` & `tableau_utilities-2.2.0/tableau_utilities/scripts/server_info.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/scripts/server_operate.py` & `tableau_utilities-2.2.0/tableau_utilities/scripts/server_operate.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/tableau_file/tableau_file.py` & `tableau_utilities-2.2.0/tableau_utilities/tableau_file/tableau_file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 import xml.etree.ElementTree as ET
 import os
 import shutil
 import xmltodict
-from tableauhyperapi import HyperProcess, Connection, Telemetry, CreateMode, TableDefinition, TableName, SqlType
 from zipfile import ZipFile
 
 import tableau_utilities.tableau_file.tableau_file_objects as tfo
 from tableau_utilities.general.funcs import transform_tableau_object
 
 
 class TableauFileError(Exception):
@@ -298,115 +297,14 @@
                     found = True
                     self.extract.connection.cols[col].key = extract_col.key
                     self.extract.connection.cols[col].value = extract_col.value
             # Otherwise, Add Extract MappingCol
             if not found:
                 self.extract.connection.cols.append(extract_col)
 
-    def empty_extract(self):
-        """ Creates an empty extract (.hyper file) for the Tableau file.
-            If the extract exists, it will be overwritten. """
-        # Get relevant paths, and create a temp folder and move the Tableau file into it
-        temp_folder = os.path.join(self.file_directory, f'__TEMP_{self.file_name}')
-        extract_folder = os.path.join(temp_folder, 'Data', 'Extracts')
-        hyper_rel_path = os.path.join('Data', 'Extracts', f'{self.file_name}.hyper')
-        temp_path = os.path.join(temp_folder, self.file_basename)
-        tdsx_basename = f'{self.file_name}.tdsx'
-        tdsx_path = os.path.join(temp_folder, tdsx_basename)
-        os.makedirs(extract_folder, exist_ok=True)
-        shutil.move(self.file_path, temp_path)
-        if self.extension == 'tdsx':
-            # Unzip the TDS file
-            with ZipFile(temp_path) as z:
-                for f in z.filelist:
-                    ext = f.filename.split('.')[-1]
-                    if ext in ['tds', 'twb']:
-                        tds_path = z.extract(member=f, path=temp_folder)
-        else:
-            tds_path = temp_path
-        hyper_path = os.path.join(extract_folder, f'{self.file_name}.hyper')
-        params = {"default_database_version": "2"}
-        # Get columns from the metadata
-        columns = dict()  # Use a dict to ensure no duplicate columns are referenced
-        for metadata in self.connection.metadata_records:
-            if metadata.local_type == 'integer':
-                column = TableDefinition.Column(metadata.remote_name, SqlType.int())
-            elif metadata.local_type == 'real':
-                column = TableDefinition.Column(metadata.remote_name, SqlType.double())
-            elif metadata.local_type == 'string':
-                column = TableDefinition.Column(metadata.remote_name, SqlType.varchar(metadata.width or 1020))
-            elif metadata.local_type == 'boolean':
-                column = TableDefinition.Column(metadata.remote_name, SqlType.bool())
-            elif metadata.local_type == 'datetime':
-                column = TableDefinition.Column(metadata.remote_name, SqlType.timestamp())
-            elif metadata.local_type == 'date':
-                column = TableDefinition.Column(metadata.remote_name, SqlType.date())
-            else:
-                raise TableauFileError(f'Got unexpected metadata type for hyper table: {metadata.local_type}')
-            columns[metadata.remote_name] = column
-        # Create an empty .hyper file based on the metadata of the Tableau file
-        with HyperProcess(Telemetry.SEND_USAGE_DATA_TO_TABLEAU, parameters=params) as hyper:
-            with Connection(hyper.endpoint, hyper_path, CreateMode.CREATE_AND_REPLACE) as connection:
-                # Create an `Extract` table inside an `Extract` schema
-                connection.catalog.create_schema('Extract')
-                table = TableDefinition(TableName('Extract', 'Extract'), columns.values())
-                connection.catalog.create_table(table)
-        # Archive the extract with the TDS file
-        with ZipFile(tdsx_path, 'w') as z:
-            z.write(tds_path, arcname=os.path.basename(tds_path))
-            z.write(hyper_path, arcname=hyper_rel_path)
-        # Update datasource extract to reference .hyper file
-        if self.extract:
-            self.extract.connection.class_name = 'hyper'
-            self.extract.connection.authentication = 'auth-none'
-            self.extract.connection.author_locale = 'en_US'
-            self.extract.connection.extract_engine = None
-            self.extract.connection.dbname = hyper_rel_path
-        # Move the tdsx out of the temp_folder and delete temp_folder
-        self.file_path = os.path.join(self.file_directory, tdsx_basename)
-        self.file_basename = tdsx_basename
-        self.extension = 'tdsx'
-        shutil.move(tdsx_path, self.file_path)
-        shutil.rmtree(temp_folder, ignore_errors=True)
-
-    def filter_extract(self, delete_condition: str):
-        """ Filters the data in the extract (.hyper file) for the Tableau file.
-
-        Args:
-            delete_condition (str): A condition string to add to the WHERE clause of data to delete.
-        """
-        if self.extension != 'tdsx' or not self.has_extract_data:
-            return None
-        # Get relevant paths, and create a temp folder and move the Tableau file into it
-        temp_folder = os.path.join(self.file_directory, f'__TEMP_{self.file_name}')
-        temp_path = os.path.join(temp_folder, self.file_basename)
-        os.makedirs(temp_folder, exist_ok=True)
-        shutil.move(self.file_path, temp_path)
-        # Unzip the TDS file
-        unzipped_files = list()
-        with ZipFile(temp_path) as z:
-            for f in z.filelist:
-                ext = f.filename.split('.')[-1]
-                path = z.extract(member=f, path=temp_folder)
-                unzipped_files.append(path)
-                if ext == 'hyper':
-                    hyper_path = path
-        # Update .hyper file based on the filter condition
-        with HyperProcess(Telemetry.SEND_USAGE_DATA_TO_TABLEAU) as hyper:
-            with Connection(hyper.endpoint, hyper_path, CreateMode.NONE) as connection:
-                connection.execute_command(f'DELETE FROM "Extract"."Extract" WHERE {delete_condition}')
-        # Archive the extract with the TDS file
-        with ZipFile(temp_path, 'w') as z:
-            for file in unzipped_files:
-                arcname = file.split(temp_folder)[-1]
-                z.write(file, arcname=arcname)
-        # Move the tdsx out of the temp_folder and delete temp_folder
-        shutil.move(temp_path, self.file_path)
-        shutil.rmtree(temp_folder, ignore_errors=True)
-
     def save(self):
         """ Save all changes made to each section of the Datasource """
         parent = self._root.find('.')
         ending_index = -1
         for section in self.sections():
             if not section:
                 continue
@@ -433,8 +331,8 @@
     unzip = False
     unzip_all_files = False
 
     ds = Datasource(ds_path)
     if unzip:
         ds.unzip(unzip_all=unzip_all_files)
 
-    print(ds.columns.get('[USER_ID]'))
+    print(ds.columns.get('[USER_ID]'))
```

### Comparing `tableau_utilities-2.1.21/tableau_utilities/tableau_file/tableau_file_objects.py` & `tableau_utilities-2.2.0/tableau_utilities/tableau_file/tableau_file_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -703,14 +703,15 @@
     workgroup_auth_mode: str = None
     tablename: str = None
     default_settings: str = None
     directory: str = None
     filename: str = None
     extract_engine: bool = None
     port: int = None
+    max_varchar_size: str = None
 
     def dict(self):
         output = dict()
         if self.authentication is not None:
             output['@authentication'] = self.authentication
         if self.class_name is not None:
             output['@class'] = self.class_name
@@ -752,14 +753,16 @@
             output['@directory'] = self.directory
         if self.filename is not None:
             output['@filename'] = self.filename
         if self.extract_engine is not None:
             output['@extract-engine'] = str(self.extract_engine).lower()
         if self.port is not None:
             output['@port'] = str(self.port)
+        if self.max_varchar_size is not None:
+            output['@max-varchar-size'] = str(self.max_varchar_size)
         return output
 
 
 @dataclass
 class NamedConnection(TableauFileObject):
     """ The NamedConnection Tableau file object """
     name: str
```

### Comparing `tableau_utilities-2.1.21/tableau_utilities/tableau_server/base.py` & `tableau_utilities-2.2.0/tableau_utilities/tableau_server/base.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/tableau_server/create.py` & `tableau_utilities-2.2.0/tableau_utilities/tableau_server/create.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/tableau_server/download.py` & `tableau_utilities-2.2.0/tableau_utilities/tableau_server/download.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/tableau_server/get.py` & `tableau_utilities-2.2.0/tableau_utilities/tableau_server/get.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/tableau_server/publish.py` & `tableau_utilities-2.2.0/tableau_utilities/tableau_server/publish.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/tableau_server/refresh.py` & `tableau_utilities-2.2.0/tableau_utilities/tableau_server/refresh.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/tableau_server/static.py` & `tableau_utilities-2.2.0/tableau_utilities/tableau_server/static.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/tableau_server/tableau_server.py` & `tableau_utilities-2.2.0/tableau_utilities/tableau_server/tableau_server.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/tableau_server/tableau_server_objects.py` & `tableau_utilities-2.2.0/tableau_utilities/tableau_server/tableau_server_objects.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/tableau_server/update.py` & `tableau_utilities-2.2.0/tableau_utilities/tableau_server/update.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities/test_tableau_utilities.py` & `tableau_utilities-2.2.0/tableau_utilities/test_tableau_utilities.py`

 * *Files identical despite different names*

### Comparing `tableau_utilities-2.1.21/tableau_utilities.egg-info/PKG-INFO` & `tableau_utilities-2.2.0/tableau_utilities.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 Metadata-Version: 2.1
 Name: tableau_utilities
-Version: 2.1.21
+Version: 2.2.0
 Summary: Utility for maintaining Tableau objects
 Home-page: http://pypi.python.org/pypi/tableau-utilities/
 Author: Justin Grilli
 Author-email: justin.grilli@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: xmltodict<1.0.0,>=0.12.0
 Requires-Dist: pyyaml<7.0.0,>=6.0
 Requires-Dist: requests<3.0.0,>=2.27.1
 Requires-Dist: pandas<2.0.0,>=1.4.1
 Requires-Dist: tabulate<1.0.0,>=0.8.9
-Requires-Dist: tableauhyperapi==0.0.18825
+Provides-Extra: hyper
+Requires-Dist: tableauhyperapi==0.0.18825; extra == "hyper"
 
 # tableau-utilities
 
 A module and CLI Utility for managing Tableau objects, locally, and in Tableau Online.
 
 ## Quick start
 
 ### Installation
 
 #### From pypi
+
+##### Core Package
 - `pip install tableau-utilities`
 
+##### Hyper Subpackage
+This extra package depends on the tableauhyperapi which is incompatible with Apple Silicon computers.  See the [tableauhyperapi installation docs](https://tableau.github.io/hyper-db/docs/installation) for workarounds to use the package on Applie Silicon.
+
+- `pip install tableau-utilities[hyper]`
+- `pip install 'tableau-utilities[hyper]'`  if you're using zsh make sure to add quotes
+
 #### Locally using pip
 - `cd tableau-utilities`
 - `pip install ./`
 
 #### Confirm installation
 - `which tableau_utilities`
   - _Describes where tableau-utilities has been installed_
```

### Comparing `tableau_utilities-2.1.21/tableau_utilities.egg-info/SOURCES.txt` & `tableau_utilities-2.2.0/tableau_utilities.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 tableau_utilities.egg-info/entry_points.txt
 tableau_utilities.egg-info/requires.txt
 tableau_utilities.egg-info/top_level.txt
 tableau_utilities/general/__init__.py
 tableau_utilities/general/cli_styling.py
 tableau_utilities/general/config_column_persona.py
 tableau_utilities/general/funcs.py
+tableau_utilities/hyper/__init__.py
+tableau_utilities/hyper/hyper.py
 tableau_utilities/scripts/__init__.py
 tableau_utilities/scripts/cli.py
 tableau_utilities/scripts/csv_config.py
 tableau_utilities/scripts/datasource.py
 tableau_utilities/scripts/gen_config.py
 tableau_utilities/scripts/merge_config.py
 tableau_utilities/scripts/server_info.py
```

