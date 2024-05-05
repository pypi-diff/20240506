# Comparing `tmp/mojo_errors-1.3.6.tar.gz` & `tmp/mojo_errors-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_errors-1.3.6.tar", max compression
+gzip compressed data, was "mojo_errors-1.3.7.tar", max compression
```

## Comparing `mojo_errors-1.3.6.tar` & `mojo_errors-1.3.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:55:15.327504 mojo_errors-1.3.6/LICENSE.txt
--rw-r--r--   0        0        0      154 2024-01-29 05:14:53.461749 mojo_errors-1.3.6/README.rst
--rw-r--r--   0        0        0      663 2024-04-24 03:49:12.060446 mojo_errors-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     5281 2024-01-26 02:55:15.328551 mojo_errors-1.3.6/source/packages/mojo/errors/exceptions.py
--rw-r--r--   0        0        0    11785 2024-03-09 19:49:42.773416 mojo_errors-1.3.6/source/packages/mojo/errors/xtraceback.py
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 mojo_errors-1.3.6/setup.py
--rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 mojo_errors-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:55:15.327504 mojo_errors-1.3.7/LICENSE.txt
+-rw-r--r--   0        0        0      154 2024-01-29 05:14:53.461749 mojo_errors-1.3.7/README.rst
+-rw-r--r--   0        0        0      663 2024-05-05 22:47:35.143495 mojo_errors-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     5105 2024-05-02 02:53:05.622002 mojo_errors-1.3.7/source/packages/mojo/errors/exceptions.py
+-rw-r--r--   0        0        0    11609 2024-05-02 02:53:23.372760 mojo_errors-1.3.7/source/packages/mojo/errors/xtraceback.py
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 mojo_errors-1.3.7/setup.py
+-rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 mojo_errors-1.3.7/PKG-INFO
```

### Comparing `mojo_errors-1.3.6/LICENSE.txt` & `mojo_errors-1.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_errors-1.3.6/pyproject.toml` & `mojo_errors-1.3.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "mojo-errors"
 description = "Automation Mojo Errors Module"
-version = "1.3.6"
+version = "1.3.7"
 authors = []
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
 ]
 keywords = [
     "python"
 ]
 packages = [{include="mojo", from="source/packages"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.9,<4.0"
 
 [tool.poetry.group.dev.dependencies]
 myst-parser = "^0.18.1"
 sphinx = ">=1.6,<6"
 sphinx-rtd-theme = "^1.1.1"
 
 [tool.poetry.group.dbio.dependencies]
```

### Comparing `mojo_errors-1.3.6/source/packages/mojo/errors/exceptions.py` & `mojo_errors-1.3.7/source/packages/mojo/errors/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,15 @@
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
 
 from http.client import HTTPException
 
 class AbstractMethodError(RuntimeError):
     """
         This error is raised when an abstract method has been called.
     """
```

### Comparing `mojo_errors-1.3.6/source/packages/mojo/errors/xtraceback.py` & `mojo_errors-1.3.7/source/packages/mojo/errors/xtraceback.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,15 @@
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
 
 from typing import Any, Dict, List, Optional
 
 from types import ModuleType, CodeType
 
 import inspect
 import os
```

### Comparing `mojo_errors-1.3.6/setup.py` & `mojo_errors-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 ['mojo', 'mojo.errors']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'mojo-errors',
-    'version': '1.3.6',
+    'version': '1.3.7',
     'description': 'Automation Mojo Errors Module',
     'long_description': '==============================\nAutomation Mojo Errors Package\n==============================\nPython package that provides a common source of error types.\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `mojo_errors-1.3.6/PKG-INFO` & `mojo_errors-1.3.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: mojo-errors
-Version: 1.3.6
+Version: 1.3.7
 Summary: Automation Mojo Errors Module
 License: LICENSE.txt
 Keywords: python
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 
 ==============================
```

