# Comparing `tmp/cloudquery-plugin-pb-0.0.25.tar.gz` & `tmp/cloudquery_plugin_pb-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudquery-plugin-pb-0.0.25.tar", last modified: Mon Apr  1 08:59:17 2024, max compression
+gzip compressed data, was "cloudquery_plugin_pb-0.0.26.tar", last modified: Mon May  6 10:24:25 2024, max compression
```

## Comparing `cloudquery-plugin-pb-0.0.25.tar` & `cloudquery_plugin_pb-0.0.26.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:59:17.012545 cloudquery-plugin-pb-0.0.25/
--rw-r--r--   0 runner    (1001) docker     (127)    16012 2024-04-01 08:59:07.000000 cloudquery-plugin-pb-0.0.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-01 08:59:17.012545 cloudquery-plugin-pb-0.0.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-01 08:59:07.000000 cloudquery-plugin-pb-0.0.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:59:17.008545 cloudquery-plugin-pb-0.0.25/cloudquery/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:59:17.008545 cloudquery-plugin-pb-0.0.25/cloudquery/discovery_v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 08:59:07.000000 cloudquery-plugin-pb-0.0.25/cloudquery/discovery_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-01 08:59:07.000000 cloudquery-plugin-pb-0.0.25/cloudquery/discovery_v1/discovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-01 08:59:07.000000 cloudquery-plugin-pb-0.0.25/cloudquery/discovery_v1/discovery_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-01 08:59:07.000000 cloudquery-plugin-pb-0.0.25/cloudquery/discovery_v1/discovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 08:59:07.000000 cloudquery-plugin-pb-0.0.25/cloudquery/discovery_v1/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:59:17.012545 cloudquery-plugin-pb-0.0.25/cloudquery/plugin_v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 08:59:07.000000 cloudquery-plugin-pb-0.0.25/cloudquery/plugin_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-01 08:59:07.000000 cloudquery-plugin-pb-0.0.25/cloudquery/plugin_v3/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-04-01 08:59:07.000000 cloudquery-plugin-pb-0.0.25/cloudquery/plugin_v3/plugin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-04-01 08:59:07.000000 cloudquery-plugin-pb-0.0.25/cloudquery/plugin_v3/plugin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16337 2024-04-01 08:59:07.000000 cloudquery-plugin-pb-0.0.25/cloudquery/plugin_v3/plugin_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 08:59:07.000000 cloudquery-plugin-pb-0.0.25/cloudquery/plugin_v3/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:59:17.012545 cloudquery-plugin-pb-0.0.25/cloudquery_plugin_pb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-01 08:59:17.000000 cloudquery-plugin-pb-0.0.25/cloudquery_plugin_pb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-01 08:59:17.000000 cloudquery-plugin-pb-0.0.25/cloudquery_plugin_pb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 08:59:17.000000 cloudquery-plugin-pb-0.0.25/cloudquery_plugin_pb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 08:59:17.000000 cloudquery-plugin-pb-0.0.25/cloudquery_plugin_pb.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 08:59:16.000000 cloudquery-plugin-pb-0.0.25/cloudquery_plugin_pb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 08:59:17.000000 cloudquery-plugin-pb-0.0.25/cloudquery_plugin_pb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 08:59:17.000000 cloudquery-plugin-pb-0.0.25/cloudquery_plugin_pb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-01 08:59:17.012545 cloudquery-plugin-pb-0.0.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-01 08:59:07.000000 cloudquery-plugin-pb-0.0.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:24:25.128982 cloudquery_plugin_pb-0.0.26/
+-rw-r--r--   0 runner    (1001) docker     (127)    16012 2024-05-06 10:24:14.000000 cloudquery_plugin_pb-0.0.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-06 10:24:25.128982 cloudquery_plugin_pb-0.0.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-06 10:24:14.000000 cloudquery_plugin_pb-0.0.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:24:25.124982 cloudquery_plugin_pb-0.0.26/cloudquery/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:24:25.124982 cloudquery_plugin_pb-0.0.26/cloudquery/discovery_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:24:14.000000 cloudquery_plugin_pb-0.0.26/cloudquery/discovery_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-06 10:24:14.000000 cloudquery_plugin_pb-0.0.26/cloudquery/discovery_v1/discovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-06 10:24:14.000000 cloudquery_plugin_pb-0.0.26/cloudquery/discovery_v1/discovery_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-06 10:24:14.000000 cloudquery_plugin_pb-0.0.26/cloudquery/discovery_v1/discovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:24:14.000000 cloudquery_plugin_pb-0.0.26/cloudquery/discovery_v1/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:24:25.124982 cloudquery_plugin_pb-0.0.26/cloudquery/plugin_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:24:14.000000 cloudquery_plugin_pb-0.0.26/cloudquery/plugin_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-06 10:24:14.000000 cloudquery_plugin_pb-0.0.26/cloudquery/plugin_v3/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-05-06 10:24:14.000000 cloudquery_plugin_pb-0.0.26/cloudquery/plugin_v3/plugin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-05-06 10:24:14.000000 cloudquery_plugin_pb-0.0.26/cloudquery/plugin_v3/plugin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16337 2024-05-06 10:24:14.000000 cloudquery_plugin_pb-0.0.26/cloudquery/plugin_v3/plugin_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:24:14.000000 cloudquery_plugin_pb-0.0.26/cloudquery/plugin_v3/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:24:25.128982 cloudquery_plugin_pb-0.0.26/cloudquery_plugin_pb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-06 10:24:25.000000 cloudquery_plugin_pb-0.0.26/cloudquery_plugin_pb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-06 10:24:25.000000 cloudquery_plugin_pb-0.0.26/cloudquery_plugin_pb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:24:25.000000 cloudquery_plugin_pb-0.0.26/cloudquery_plugin_pb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 10:24:25.000000 cloudquery_plugin_pb-0.0.26/cloudquery_plugin_pb.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:24:24.000000 cloudquery_plugin_pb-0.0.26/cloudquery_plugin_pb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 10:24:25.000000 cloudquery_plugin_pb-0.0.26/cloudquery_plugin_pb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 10:24:25.000000 cloudquery_plugin_pb-0.0.26/cloudquery_plugin_pb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-06 10:24:25.128982 cloudquery_plugin_pb-0.0.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-06 10:24:14.000000 cloudquery_plugin_pb-0.0.26/setup.py
```

### Comparing `cloudquery-plugin-pb-0.0.25/LICENSE` & `cloudquery_plugin_pb-0.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-pb-0.0.25/PKG-INFO` & `cloudquery_plugin_pb-0.0.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudquery-plugin-pb
-Version: 0.0.25
+Version: 0.0.26
 Summary: CloudQuery Plugin client and server library
 Home-page: https://github.com/cloudquery/plugin-pb-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudquery-plugin-pb-0.0.25/README.md` & `cloudquery_plugin_pb-0.0.26/README.md`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-pb-0.0.25/cloudquery/discovery_v1/discovery_pb2.py` & `cloudquery_plugin_pb-0.0.26/cloudquery/discovery_v1/discovery_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-pb-0.0.25/cloudquery/discovery_v1/discovery_pb2.pyi` & `cloudquery_plugin_pb-0.0.26/cloudquery/discovery_v1/discovery_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-pb-0.0.25/cloudquery/discovery_v1/discovery_pb2_grpc.py` & `cloudquery_plugin_pb-0.0.26/cloudquery/discovery_v1/discovery_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-pb-0.0.25/cloudquery/plugin_v3/arrow.py` & `cloudquery_plugin_pb-0.0.26/cloudquery/plugin_v3/arrow.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-pb-0.0.25/cloudquery/plugin_v3/plugin_pb2.py` & `cloudquery_plugin_pb-0.0.26/cloudquery/plugin_v3/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-pb-0.0.25/cloudquery/plugin_v3/plugin_pb2.pyi` & `cloudquery_plugin_pb-0.0.26/cloudquery/plugin_v3/plugin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-pb-0.0.25/cloudquery/plugin_v3/plugin_pb2_grpc.py` & `cloudquery_plugin_pb-0.0.26/cloudquery/plugin_v3/plugin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-pb-0.0.25/cloudquery_plugin_pb.egg-info/PKG-INFO` & `cloudquery_plugin_pb-0.0.26/cloudquery_plugin_pb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudquery-plugin-pb
-Version: 0.0.25
+Version: 0.0.26
 Summary: CloudQuery Plugin client and server library
 Home-page: https://github.com/cloudquery/plugin-pb-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudquery-plugin-pb-0.0.25/cloudquery_plugin_pb.egg-info/SOURCES.txt` & `cloudquery_plugin_pb-0.0.26/cloudquery_plugin_pb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-pb-0.0.25/setup.py` & `cloudquery_plugin_pb-0.0.26/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("cloudquery")
 ]
 setuptools.setup(
     name=name,
-    version="0.0.25",
+    version="0.0.26",
     description=description,
     long_description=long_description,
     author="CloudQuery LTD",
     author_email="pypi-packages@cloudquery.io",
     license="MPL-2.0",
     url=url,
     classifiers=[
```

