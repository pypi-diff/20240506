# Comparing `tmp/mojo_interfaces-1.3.2.tar.gz` & `tmp/mojo_interfaces-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_interfaces-1.3.2.tar", max compression
+gzip compressed data, was "mojo_interfaces-1.3.3.tar", max compression
```

## Comparing `mojo_interfaces-1.3.2.tar` & `mojo_interfaces-1.3.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:53:59.487475 mojo_interfaces-1.3.2/LICENSE.txt
--rw-r--r--   0        0        0      850 2024-01-26 02:53:59.487659 mojo_interfaces-1.3.2/README.rst
--rw-r--r--   0        0        0      688 2024-04-24 04:02:16.107538 mojo_interfaces-1.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-26 02:53:59.488973 mojo_interfaces-1.3.2/source/packages/mojo/interfaces/__init__.py
--rw-r--r--   0        0        0     1551 2024-01-26 02:53:59.489064 mojo_interfaces-1.3.2/source/packages/mojo/interfaces/iexcludefilter.py
--rw-r--r--   0        0        0     1544 2024-01-26 02:53:59.489143 mojo_interfaces-1.3.2/source/packages/mojo/interfaces/iincludefilter.py
--rw-r--r--   0        0        0      762 2024-02-21 07:24:58.082138 mojo_interfaces-1.3.2/source/packages/mojo/interfaces/iserializable.py
--rw-r--r--   0        0        0     6271 2024-01-26 02:53:59.489239 mojo_interfaces-1.3.2/source/packages/mojo/interfaces/isystemcontext.py
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 mojo_interfaces-1.3.2/setup.py
--rw-r--r--   0        0        0     1517 1970-01-01 00:00:00.000000 mojo_interfaces-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1556 2024-05-02 06:19:49.820698 mojo_interfaces-1.3.3/LICENSE.txt
+-rw-r--r--   0        0        0      850 2024-01-26 02:53:59.487659 mojo_interfaces-1.3.3/README.rst
+-rw-r--r--   0        0        0      688 2024-05-06 01:44:54.396917 mojo_interfaces-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-26 02:53:59.488973 mojo_interfaces-1.3.3/source/packages/mojo/interfaces/__init__.py
+-rw-r--r--   0        0        0     1375 2024-05-02 06:18:52.315984 mojo_interfaces-1.3.3/source/packages/mojo/interfaces/iexcludefilter.py
+-rw-r--r--   0        0        0     1368 2024-05-02 06:18:57.168205 mojo_interfaces-1.3.3/source/packages/mojo/interfaces/iincludefilter.py
+-rw-r--r--   0        0        0      586 2024-05-02 06:19:01.979269 mojo_interfaces-1.3.3/source/packages/mojo/interfaces/iserializable.py
+-rw-r--r--   0        0        0     6094 2024-05-02 06:19:10.706809 mojo_interfaces-1.3.3/source/packages/mojo/interfaces/isystemcontext.py
+-rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 mojo_interfaces-1.3.3/setup.py
+-rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 mojo_interfaces-1.3.3/PKG-INFO
```

### Comparing `mojo_interfaces-1.3.2/README.rst` & `mojo_interfaces-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `mojo_interfaces-1.3.2/pyproject.toml` & `mojo_interfaces-1.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "mojo-interfaces"
 description = "Automation Mojo Interfaces Package"
-version = "1.3.2"
+version = "1.3.3"
 authors = ["Myron W Walker"]
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

### Comparing `mojo_interfaces-1.3.2/source/packages/mojo/interfaces/iexcludefilter.py` & `mojo_interfaces-1.3.3/source/packages/mojo/interfaces/iexcludefilter.py`

 * *Files 13% similar despite different names*

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
 
 from typing import Any, List, Protocol
 
 class IExcludeFilter(Protocol):
     """
         The IExcludeFilter interface is used to provide a common interface for performing an
         exclude filter on objects.
```

### Comparing `mojo_interfaces-1.3.2/source/packages/mojo/interfaces/iincludefilter.py` & `mojo_interfaces-1.3.3/source/packages/mojo/interfaces/iincludefilter.py`

 * *Files 12% similar despite different names*

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
 
 from typing import Any, List, Protocol
 
 class IIncludeFilter(Protocol):
     """
         The IIncludeFilter interface is used to provide a common interface for performing an
         include filter on objects.
```

### Comparing `mojo_interfaces-1.3.2/source/packages/mojo/interfaces/iserializable.py` & `mojo_interfaces-1.3.3/source/packages/mojo/interfaces/iserializable.py`

 * *Files 22% similar despite different names*

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
 
 
 from typing import Any, Dict, Protocol
 
 class ISerializable(Protocol):
 
     @classmethod
```

### Comparing `mojo_interfaces-1.3.2/source/packages/mojo/interfaces/isystemcontext.py` & `mojo_interfaces-1.3.3/source/packages/mojo/interfaces/isystemcontext.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,14 @@
 
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
 
 
 from typing import Optional, Protocol, Sequence, Tuple, Union
 
 from mojo.errors.exceptions import NotOverloadedError
 
 from mojo.xmods.aspects import AspectsCmd
```

### Comparing `mojo_interfaces-1.3.2/setup.py` & `mojo_interfaces-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 ['mojo', 'mojo.interfaces']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'mojo-interfaces',
-    'version': '1.3.2',
+    'version': '1.3.3',
     'description': 'Automation Mojo Interfaces Package',
     'long_description': "=======================\nmojo-interfaces\n=======================\nThis is a package that contains a collection or library of interfaces that can be shared by other packages.\n\n=================\nCode Organization\n=================\n* .vscode - Common tasks\n* development - This is where the runtime environment scripts are located\n* repository-setup - Scripts for homing your repository and to your checkout and machine setup\n* userguide - Where you put your user guide\n* source/packages - Put your root folder here 'source/packages/(root-module-folder)'\n* source/sphinx - This is the Sphinx documentation folder\n* workspaces - This is where you add VSCode workspaces templates and where workspaces show up when homed.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n",
     'author': 'Myron W Walker',
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

### Comparing `mojo_interfaces-1.3.2/PKG-INFO` & `mojo_interfaces-1.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: mojo-interfaces
-Version: 1.3.2
+Version: 1.3.3
 Summary: Automation Mojo Interfaces Package
 License: LICENSE.txt
 Keywords: python
 Author: Myron W Walker
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
 
 =======================
```

