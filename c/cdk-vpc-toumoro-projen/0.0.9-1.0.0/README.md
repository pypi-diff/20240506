# Comparing `tmp/cdk-vpc-toumoro-projen-0.0.9.tar.gz` & `tmp/cdk-vpc-toumoro-projen-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-vpc-toumoro-projen-0.0.9.tar", last modified: Thu May  2 19:20:06 2024, max compression
+gzip compressed data, was "cdk-vpc-toumoro-projen-1.0.0.tar", last modified: Mon May  6 17:01:53 2024, max compression
```

## Comparing `cdk-vpc-toumoro-projen-0.0.9.tar` & `cdk-vpc-toumoro-projen-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:20:06.002659 cdk-vpc-toumoro-projen-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-02 19:20:06.002659 cdk-vpc-toumoro-projen-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:20:06.002659 cdk-vpc-toumoro-projen-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:20:05.998659 cdk-vpc-toumoro-projen-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:20:05.998659 cdk-vpc-toumoro-projen-0.0.9/src/cdk-vpc-toumoro-projen/
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk-vpc-toumoro-projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:20:05.998659 cdk-vpc-toumoro-projen-0.0.9/src/cdk-vpc-toumoro-projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk-vpc-toumoro-projen/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23273 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk-vpc-toumoro-projen/_jsii/cdk-vpc-toumoro-projen@0.0.9.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:19:42.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk-vpc-toumoro-projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:20:06.002659 cdk-vpc-toumoro-projen-0.0.9/src/cdk_vpc_toumoro_projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-02 19:20:05.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-02 19:20:05.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk_vpc_toumoro_projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:20:05.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk_vpc_toumoro_projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-02 19:20:05.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk_vpc_toumoro_projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 19:20:05.000000 cdk-vpc-toumoro-projen-0.0.9/src/cdk_vpc_toumoro_projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:01:53.400961 cdk-vpc-toumoro-projen-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-06 17:01:53.400961 cdk-vpc-toumoro-projen-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 17:01:53.400961 cdk-vpc-toumoro-projen-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:01:53.400961 cdk-vpc-toumoro-projen-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:01:53.400961 cdk-vpc-toumoro-projen-1.0.0/src/cdk-vpc-toumoro-projen/
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk-vpc-toumoro-projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:01:53.400961 cdk-vpc-toumoro-projen-1.0.0/src/cdk-vpc-toumoro-projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk-vpc-toumoro-projen/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28899 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk-vpc-toumoro-projen/_jsii/cdk-vpc-toumoro-projen@1.0.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk-vpc-toumoro-projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:01:53.400961 cdk-vpc-toumoro-projen-1.0.0/src/cdk_vpc_toumoro_projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-06 17:01:53.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-06 17:01:53.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk_vpc_toumoro_projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:01:53.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk_vpc_toumoro_projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-06 17:01:53.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk_vpc_toumoro_projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 17:01:53.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk_vpc_toumoro_projen.egg-info/top_level.txt
```

### Comparing `cdk-vpc-toumoro-projen-0.0.9/LICENSE` & `cdk-vpc-toumoro-projen-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-vpc-toumoro-projen-0.0.9/PKG-INFO` & `cdk-vpc-toumoro-projen-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-vpc-toumoro-projen
-Version: 0.0.9
+Version: 1.0.0
 Summary: A CDK construct library to create a VPC with public and private subnets.
 Home-page: https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -18,7 +18,11 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # replace this
+
+# Documentation API
+
+[API](API.md)
```

### Comparing `cdk-vpc-toumoro-projen-0.0.9/setup.py` & `cdk-vpc-toumoro-projen-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-vpc-toumoro-projen",
-    "version": "0.0.9",
+    "version": "1.0.0",
     "description": "A CDK construct library to create a VPC with public and private subnets.",
     "license": "GPL-3.0-or-later",
     "url": "https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git",
     "long_description_content_type": "text/markdown",
     "author": "tm-lcarvalho<lucio.carvalho@toumoro.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "cdk-vpc-toumoro-projen",
         "cdk-vpc-toumoro-projen._jsii"
     ],
     "package_data": {
         "cdk-vpc-toumoro-projen._jsii": [
-            "cdk-vpc-toumoro-projen@0.0.9.jsii.tgz"
+            "cdk-vpc-toumoro-projen@1.0.0.jsii.tgz"
         ],
         "cdk-vpc-toumoro-projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib>=2.1.0, <3.0.0",
+        "aws-cdk-lib>=2.140.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.96.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `cdk-vpc-toumoro-projen-0.0.9/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO` & `cdk-vpc-toumoro-projen-1.0.0/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-vpc-toumoro-projen
-Version: 0.0.9
+Version: 1.0.0
 Summary: A CDK construct library to create a VPC with public and private subnets.
 Home-page: https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -18,7 +18,11 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # replace this
+
+# Documentation API
+
+[API](API.md)
```

