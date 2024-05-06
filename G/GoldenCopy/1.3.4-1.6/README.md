# Comparing `tmp/GoldenCopy-1.3.4.tar.gz` & `tmp/goldencopy-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoldenCopy-1.3.4.tar", last modified: Tue Sep  6 09:20:15 2022, max compression
+gzip compressed data, was "goldencopy-1.6.tar", last modified: Mon May  6 09:46:59 2024, max compression
```

## Comparing `GoldenCopy-1.3.4.tar` & `goldencopy-1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-09-06 09:20:15.476068 GoldenCopy-1.3.4/
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-09-06 09:20:15.476068 GoldenCopy-1.3.4/GoldenCopy.egg-info/
--rw-------   0 dramelac  (1000) dramelac  (1000)     3619 2022-09-06 09:20:15.000000 GoldenCopy-1.3.4/GoldenCopy.egg-info/PKG-INFO
--rw-------   0 dramelac  (1000) dramelac  (1000)      260 2022-09-06 09:20:15.000000 GoldenCopy-1.3.4/GoldenCopy.egg-info/SOURCES.txt
--rw-------   0 dramelac  (1000) dramelac  (1000)        1 2022-09-06 09:20:15.000000 GoldenCopy-1.3.4/GoldenCopy.egg-info/dependency_links.txt
--rw-------   0 dramelac  (1000) dramelac  (1000)       47 2022-09-06 09:20:15.000000 GoldenCopy-1.3.4/GoldenCopy.egg-info/entry_points.txt
--rw-------   0 dramelac  (1000) dramelac  (1000)       17 2022-09-06 09:20:15.000000 GoldenCopy-1.3.4/GoldenCopy.egg-info/requires.txt
--rw-------   0 dramelac  (1000) dramelac  (1000)       11 2022-09-06 09:20:15.000000 GoldenCopy-1.3.4/GoldenCopy.egg-info/top_level.txt
--rw-r-----   0 dramelac  (1000) dramelac  (1000)    35149 2022-02-22 13:33:58.000000 GoldenCopy-1.3.4/LICENSE.txt
--rw-------   0 dramelac  (1000) dramelac  (1000)     3619 2022-09-06 09:20:15.476068 GoldenCopy-1.3.4/PKG-INFO
--rw-r-----   0 dramelac  (1000) dramelac  (1000)     2680 2022-08-23 12:24:14.000000 GoldenCopy-1.3.4/README.md
--rwxr-----   0 dramelac  (1000) dramelac  (1000)     9696 2022-09-06 09:20:04.000000 GoldenCopy-1.3.4/goldencopy.py
--rw-r-----   0 dramelac  (1000) dramelac  (1000)      107 2022-09-06 09:20:15.476068 GoldenCopy-1.3.4/setup.cfg
--rw-r-----   0 dramelac  (1000) dramelac  (1000)     1439 2022-09-05 13:53:26.000000 GoldenCopy-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:59.236503 goldencopy-1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:59.236503 goldencopy-1.6/GoldenCopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-06 09:46:59.000000 goldencopy-1.6/GoldenCopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-06 09:46:59.000000 goldencopy-1.6/GoldenCopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:46:59.000000 goldencopy-1.6/GoldenCopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 09:46:59.000000 goldencopy-1.6/GoldenCopy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 09:46:59.000000 goldencopy-1.6/GoldenCopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 09:46:59.000000 goldencopy-1.6/GoldenCopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 09:46:48.000000 goldencopy-1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-06 09:46:59.236503 goldencopy-1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-06 09:46:48.000000 goldencopy-1.6/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9613 2024-05-06 09:46:48.000000 goldencopy-1.6/goldencopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-06 09:46:59.236503 goldencopy-1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-06 09:46:48.000000 goldencopy-1.6/setup.py
```

### Comparing `GoldenCopy-1.3.4/GoldenCopy.egg-info/PKG-INFO` & `goldencopy-1.6/GoldenCopy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: GoldenCopy
-Version: 1.3.4
+Version: 1.6
 Summary: Copy the properties and groups of a user or computer from neo4j (bloodhound) to create an identical golden ticket.
 Home-page: https://github.com/Dramelac/GoldenCopy
 Author: Dramelac
 Author-email: dramelac@pm.me
 License: GNU
 Project-URL: Bug Reports, https://github.com/Dramelac/GoldenCopy/issues
 Project-URL: Source, https://github.com/Dramelac/GoldenCopy
 Keywords: pentest redteam goldenticket goldencopy
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: py2neo>=2021.2.4
 
 # GoldenCopy
 
 You encounter limitations with your golden tickets (DACLs, detection)? 
 GoldenCopy retrieves all the information (ID, groups, etc) of a specific user in a neo4j database (bloodhound) and prepares the mimikatz/ticketer command to impersonate his permissions.
 
 ## Installation
```

### Comparing `GoldenCopy-1.3.4/LICENSE.txt` & `goldencopy-1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GoldenCopy-1.3.4/PKG-INFO` & `goldencopy-1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: GoldenCopy
-Version: 1.3.4
+Version: 1.6
 Summary: Copy the properties and groups of a user or computer from neo4j (bloodhound) to create an identical golden ticket.
 Home-page: https://github.com/Dramelac/GoldenCopy
 Author: Dramelac
 Author-email: dramelac@pm.me
 License: GNU
 Project-URL: Bug Reports, https://github.com/Dramelac/GoldenCopy/issues
 Project-URL: Source, https://github.com/Dramelac/GoldenCopy
 Keywords: pentest redteam goldenticket goldencopy
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: py2neo>=2021.2.4
 
 # GoldenCopy
 
 You encounter limitations with your golden tickets (DACLs, detection)? 
 GoldenCopy retrieves all the information (ID, groups, etc) of a specific user in a neo4j database (bloodhound) and prepares the mimikatz/ticketer command to impersonate his permissions.
 
 ## Installation
```

### Comparing `GoldenCopy-1.3.4/README.md` & `goldencopy-1.6/README.md`

 * *Files identical despite different names*

### Comparing `GoldenCopy-1.3.4/goldencopy.py` & `goldencopy-1.6/goldencopy.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List
 
 from py2neo import Graph
 import argparse
 import logging
 import re
 
-__version__ = '1.3.4'
+__version__ = '1.6'
 
 
 def args_parser():
     parser = argparse.ArgumentParser(
         description=f"GoldenCopy v{__version__} - Copy the properties and groups of a user from neo4j to create an identical golden ticket")
     # Logging config
     parser.add_argument('-v', '--verbose', action="count", default=0, dest="verbosity", help="Enable verbose logging")
@@ -231,17 +231,16 @@
           f"-domain {user.domain} " \
           f"-domain-sid {user.domain_id} " \
           f"-groups {groupList(user)} " \
           f"-user-id {user.user_id} " \
           f"{getExtraSid(user)}" \
           f"{args.custom}"
     if args.stealth:
-        logger.warning("WARNING: default ticketer duration use days and not hours, you should fix your tools ! "
-                       "(stealth require 10 hours tickets)")
-        cmd += f"-duration 10 "
+        logger.warning("WARNING: Be sure to use the latest version of impacket!")
+        cmd += f"-duration 10 -extra-pac "
     cmd += "'"+user.username+"'"
     cmd += f" && export KRB5CCNAME=$(pwd)/'{user.username}.ccache'"
     print(cmd)
     print()
     return cmd
```

### Comparing `GoldenCopy-1.3.4/setup.py` & `goldencopy-1.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='GoldenCopy',
-    version="1.3.4",
+    version='1.6',
     license='GNU',
     author="Dramelac",
     author_email='dramelac@pm.me',
     description='Copy the properties and groups of a user or computer from neo4j (bloodhound) to create an identical golden ticket.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.6, <4',
@@ -20,26 +20,28 @@
     keywords='pentest redteam goldenticket goldencopy',
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-          'py2neo>=2021.2.3'
-      ],
+        'py2neo>=2021.2.4',
+    ],
     py_modules=["goldencopy"],
     entry_points={
-    'console_scripts': [
-        'goldencopy=goldencopy:main',
-    ],
-},
+        'console_scripts': [
+            'goldencopy=goldencopy:main',
+        ],
+    },
 
     project_urls={
         'Bug Reports': 'https://github.com/Dramelac/GoldenCopy/issues',
         'Source': 'https://github.com/Dramelac/GoldenCopy',
     },
 
-)
+)
```

