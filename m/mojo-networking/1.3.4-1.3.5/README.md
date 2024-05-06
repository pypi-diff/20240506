# Comparing `tmp/mojo_networking-1.3.4.tar.gz` & `tmp/mojo_networking-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_networking-1.3.4.tar", max compression
+gzip compressed data, was "mojo_networking-1.3.5.tar", max compression
```

## Comparing `mojo_networking-1.3.4.tar` & `mojo_networking-1.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:54:48.206905 mojo_networking-1.3.4/LICENSE.txt
--rw-r--r--   0        0        0      117 2024-01-26 02:54:48.207038 mojo_networking-1.3.4/README.md
--rw-r--r--   0        0        0      889 2024-04-24 04:04:12.162282 mojo_networking-1.3.4/pyproject.toml
--rw-r--r--   0        0        0      500 2024-01-26 02:54:48.208882 mojo_networking-1.3.4/source/packages/mojo/networking/__init__.py
--rw-r--r--   0        0        0      613 2024-01-26 02:54:48.208987 mojo_networking-1.3.4/source/packages/mojo/networking/broadcast.py
--rw-r--r--   0        0        0     7259 2024-04-23 18:40:08.355498 mojo_networking-1.3.4/source/packages/mojo/networking/constants.py
--rw-r--r--   0        0        0     2910 2024-01-26 02:54:48.209132 mojo_networking-1.3.4/source/packages/mojo/networking/exceptions.py
--rw-r--r--   0        0        0     9204 2024-01-26 02:54:48.209233 mojo_networking-1.3.4/source/packages/mojo/networking/interfaces.py
--rw-r--r--   0        0        0     8824 2024-01-26 02:54:48.209339 mojo_networking-1.3.4/source/packages/mojo/networking/multicast.py
--rw-r--r--   0        0        0     5795 2024-04-23 20:33:28.693413 mojo_networking-1.3.4/source/packages/mojo/networking/resolution.py
--rw-r--r--   0        0        0     1845 2024-01-26 02:54:48.209499 mojo_networking-1.3.4/source/packages/mojo/networking/trafficcapturecontext.py
--rw-r--r--   0        0        0     4543 2024-01-26 02:54:48.209575 mojo_networking-1.3.4/source/packages/mojo/networking/unicast.py
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 mojo_networking-1.3.4/setup.py
--rw-r--r--   0        0        0     1037 1970-01-01 00:00:00.000000 mojo_networking-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:54:48.206905 mojo_networking-1.3.5/LICENSE.txt
+-rw-r--r--   0        0        0      117 2024-01-26 02:54:48.207038 mojo_networking-1.3.5/README.md
+-rw-r--r--   0        0        0      889 2024-05-06 01:49:00.660753 mojo_networking-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0      500 2024-01-26 02:54:48.208882 mojo_networking-1.3.5/source/packages/mojo/networking/__init__.py
+-rw-r--r--   0        0        0      613 2024-01-26 02:54:48.208987 mojo_networking-1.3.5/source/packages/mojo/networking/broadcast.py
+-rw-r--r--   0        0        0     7259 2024-04-23 18:40:08.355498 mojo_networking-1.3.5/source/packages/mojo/networking/constants.py
+-rw-r--r--   0        0        0     2910 2024-01-26 02:54:48.209132 mojo_networking-1.3.5/source/packages/mojo/networking/exceptions.py
+-rw-r--r--   0        0        0     9204 2024-01-26 02:54:48.209233 mojo_networking-1.3.5/source/packages/mojo/networking/interfaces.py
+-rw-r--r--   0        0        0     8824 2024-01-26 02:54:48.209339 mojo_networking-1.3.5/source/packages/mojo/networking/multicast.py
+-rw-r--r--   0        0        0     5795 2024-04-23 20:33:28.693413 mojo_networking-1.3.5/source/packages/mojo/networking/resolution.py
+-rw-r--r--   0        0        0     1845 2024-01-26 02:54:48.209499 mojo_networking-1.3.5/source/packages/mojo/networking/trafficcapturecontext.py
+-rw-r--r--   0        0        0     4543 2024-01-26 02:54:48.209575 mojo_networking-1.3.5/source/packages/mojo/networking/unicast.py
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 mojo_networking-1.3.5/setup.py
+-rw-r--r--   0        0        0      987 1970-01-01 00:00:00.000000 mojo_networking-1.3.5/PKG-INFO
```

### Comparing `mojo_networking-1.3.4/LICENSE.txt` & `mojo_networking-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_networking-1.3.4/pyproject.toml` & `mojo_networking-1.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-networking"
 description = "Automation Mojo Netorking Package (mojo-networking)"
-version = "1.3.4"
+version = "1.3.5"
 authors = [
     "Myron Walker <myron.walker@gmail.com>"
 ]
 readme = "README.md"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -17,15 +17,15 @@
 ]
 packages = [{include="mojo", from="source/packages"}]
 
 homepage = "http://automationmojo.com"
 repository = "https://github.com/automationmojo/mojo-networking"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.9,<4.0"
 netifaces = "^0.11.0"
 requests = ">=2.31.0 <3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 myst-parser = "^0.18.1"
 sphinx = ">=1.6,<6"
 sphinx-rtd-theme = "^1.1.1"
```

### Comparing `mojo_networking-1.3.4/source/packages/mojo/networking/broadcast.py` & `mojo_networking-1.3.5/source/packages/mojo/networking/broadcast.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-1.3.4/source/packages/mojo/networking/constants.py` & `mojo_networking-1.3.5/source/packages/mojo/networking/constants.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-1.3.4/source/packages/mojo/networking/exceptions.py` & `mojo_networking-1.3.5/source/packages/mojo/networking/exceptions.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-1.3.4/source/packages/mojo/networking/interfaces.py` & `mojo_networking-1.3.5/source/packages/mojo/networking/interfaces.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-1.3.4/source/packages/mojo/networking/multicast.py` & `mojo_networking-1.3.5/source/packages/mojo/networking/multicast.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-1.3.4/source/packages/mojo/networking/resolution.py` & `mojo_networking-1.3.5/source/packages/mojo/networking/resolution.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-1.3.4/source/packages/mojo/networking/trafficcapturecontext.py` & `mojo_networking-1.3.5/source/packages/mojo/networking/trafficcapturecontext.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-1.3.4/source/packages/mojo/networking/unicast.py` & `mojo_networking-1.3.5/source/packages/mojo/networking/unicast.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-1.3.4/setup.py` & `mojo_networking-1.3.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 {'': ['*']}
 
 install_requires = \
 ['netifaces>=0.11.0,<0.12.0', 'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'mojo-networking',
-    'version': '1.3.4',
+    'version': '1.3.5',
     'description': 'Automation Mojo Netorking Package (mojo-networking)',
     'long_description': '# python-package-template\nThis is a template repository that can be used to quickly create a python package project.\n',
     'author': 'Myron Walker',
     'author_email': 'myron.walker@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'http://automationmojo.com',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `mojo_networking-1.3.4/PKG-INFO` & `mojo_networking-1.3.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: mojo-networking
-Version: 1.3.4
+Version: 1.3.5
 Summary: Automation Mojo Netorking Package (mojo-networking)
 Home-page: http://automationmojo.com
 License: LICENSE.txt
 Keywords: python
 Author: Myron Walker
 Author-email: myron.walker@gmail.com
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
 Requires-Dist: netifaces (>=0.11.0,<0.12.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/automationmojo/mojo-networking
```

