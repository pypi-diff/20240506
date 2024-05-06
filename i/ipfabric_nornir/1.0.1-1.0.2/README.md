# Comparing `tmp/ipfabric_nornir-1.0.1.tar.gz` & `tmp/ipfabric_nornir-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric_nornir-1.0.1.tar", max compression
+gzip compressed data, was "ipfabric_nornir-1.0.2.tar", max compression
```

## Comparing `ipfabric_nornir-1.0.1.tar` & `ipfabric_nornir-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-11-15 18:38:57.011501 ipfabric_nornir-1.0.1/ipfabric_nornir/__init__.py
--rw-r--r--   0        0        0        0 2023-11-15 18:38:57.011501 ipfabric_nornir-1.0.1/ipfabric_nornir/plugins/__init__.py
--rw-r--r--   0        0        0      143 2023-11-15 22:17:21.821744 ipfabric_nornir-1.0.1/ipfabric_nornir/plugins/inventory/__init__.py
--rw-r--r--   0        0        0     5178 2023-11-29 16:27:50.587944 ipfabric_nornir-1.0.1/ipfabric_nornir/plugins/inventory/ipfabric.py
--rw-r--r--   0        0        0    11558 2023-11-15 18:38:57.010499 ipfabric_nornir-1.0.1/LICENSE
--rw-r--r--   0        0        0     2014 2023-11-29 16:23:05.930402 ipfabric_nornir-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3085 2023-11-16 16:03:46.357208 ipfabric_nornir-1.0.1/README.md
--rw-r--r--   0        0        0     4221 1970-01-01 00:00:00.000000 ipfabric_nornir-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-11-29 16:36:11.215522 ipfabric_nornir-1.0.2/ipfabric_nornir/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-29 16:36:11.215522 ipfabric_nornir-1.0.2/ipfabric_nornir/plugins/__init__.py
+-rw-r--r--   0        0        0      143 2023-11-29 16:36:11.215522 ipfabric_nornir-1.0.2/ipfabric_nornir/plugins/inventory/__init__.py
+-rw-r--r--   0        0        0     5178 2024-05-06 15:20:40.061866 ipfabric_nornir-1.0.2/ipfabric_nornir/plugins/inventory/ipfabric.py
+-rw-r--r--   0        0        0    11558 2023-11-15 18:38:57.010499 ipfabric_nornir-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2043 2024-05-06 15:18:07.351270 ipfabric_nornir-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3085 2023-11-29 16:36:11.215522 ipfabric_nornir-1.0.2/README.md
+-rw-r--r--   0        0        0     4262 1970-01-01 00:00:00.000000 ipfabric_nornir-1.0.2/PKG-INFO
```

### Comparing `ipfabric_nornir-1.0.1/ipfabric_nornir/plugins/inventory/ipfabric.py` & `ipfabric_nornir-1.0.2/ipfabric_nornir/plugins/inventory/ipfabric.py`

 * *Files identical despite different names*

### Comparing `ipfabric_nornir-1.0.1/LICENSE` & `ipfabric_nornir-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfabric_nornir-1.0.1/pyproject.toml` & `ipfabric_nornir-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipfabric_nornir"
-version = "1.0.1"
+version = "1.0.2"
 description = "IP Fabric Offical Plugin for nornir"
 authors = [
     "IP Fabric Solution Architecture <solution.architecture@ipfabric.io>"
 ]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://gitlab.com/ip-fabric/integrations/ipfabric_nornir"
@@ -15,19 +15,20 @@
 [tool.poetry.urls]
 "IP Fabric" = "https://ipfabric.io/"
 "Changelog" = "https://gitlab.com/ip-fabric/integrations/ipfabric_nornir/-/blob/main/CHANGELOG.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-ipfabric = "^6.3.0"
+ipfabric = ">=6.7.0,<6.9.0"
 nornir = "^3.4.1"
 nornir-netmiko = {version = "^1.0.0", optional = true}
 nornir-utils = {version = "^0.2.0", optional = true}
 nornir-napalm = {version = "^0.4.0", optional = true}
+tenacity = "^8.2.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 flake8 = "^5.0.4"
 black = "^22.12"
 setuptools = "^68.2.2"
```

### Comparing `ipfabric_nornir-1.0.1/README.md` & `ipfabric_nornir-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ipfabric_nornir-1.0.1/PKG-INFO` & `ipfabric_nornir-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: ipfabric_nornir
-Version: 1.0.1
+Version: 1.0.2
 Summary: IP Fabric Offical Plugin for nornir
 Home-page: https://gitlab.com/ip-fabric/integrations/ipfabric_nornir
 License: Apache-2.0
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: IP Fabric Solution Architecture
 Author-email: solution.architecture@ipfabric.io
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: examples
-Requires-Dist: ipfabric (>=6.3.0,<7.0.0)
+Requires-Dist: ipfabric (>=6.7.0,<6.9.0)
 Requires-Dist: nornir (>=3.4.1,<4.0.0)
 Requires-Dist: nornir-napalm (>=0.4.0,<0.5.0) ; extra == "examples"
 Requires-Dist: nornir-netmiko (>=1.0.0,<2.0.0) ; extra == "examples"
 Requires-Dist: nornir-utils (>=0.2.0,<0.3.0) ; extra == "examples"
+Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Project-URL: Changelog, https://gitlab.com/ip-fabric/integrations/ipfabric_nornir/-/blob/main/CHANGELOG.md
 Project-URL: IP Fabric, https://ipfabric.io/
 Project-URL: Repository, https://gitlab.com/ip-fabric/integrations/ipfabric_nornir
 Description-Content-Type: text/markdown
 
 ipfabric_nornir
 ==============
```

