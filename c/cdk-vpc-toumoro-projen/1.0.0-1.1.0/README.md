# Comparing `tmp/cdk-vpc-toumoro-projen-1.0.0.tar.gz` & `tmp/cdk-vpc-toumoro-projen-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-vpc-toumoro-projen-1.0.0.tar", last modified: Mon May  6 17:01:53 2024, max compression
+gzip compressed data, was "cdk-vpc-toumoro-projen-1.1.0.tar", last modified: Mon May  6 18:09:00 2024, max compression
```

## Comparing `cdk-vpc-toumoro-projen-1.0.0.tar` & `cdk-vpc-toumoro-projen-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:01:53.400961 cdk-vpc-toumoro-projen-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-06 17:01:53.400961 cdk-vpc-toumoro-projen-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 17:01:53.400961 cdk-vpc-toumoro-projen-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:01:53.400961 cdk-vpc-toumoro-projen-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:01:53.400961 cdk-vpc-toumoro-projen-1.0.0/src/cdk-vpc-toumoro-projen/
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk-vpc-toumoro-projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:01:53.400961 cdk-vpc-toumoro-projen-1.0.0/src/cdk-vpc-toumoro-projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk-vpc-toumoro-projen/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28899 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk-vpc-toumoro-projen/_jsii/cdk-vpc-toumoro-projen@1.0.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:01:42.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk-vpc-toumoro-projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:01:53.400961 cdk-vpc-toumoro-projen-1.0.0/src/cdk_vpc_toumoro_projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-06 17:01:53.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-06 17:01:53.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk_vpc_toumoro_projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:01:53.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk_vpc_toumoro_projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-06 17:01:53.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk_vpc_toumoro_projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 17:01:53.000000 cdk-vpc-toumoro-projen-1.0.0/src/cdk_vpc_toumoro_projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:09:00.217244 cdk-vpc-toumoro-projen-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-06 18:08:50.000000 cdk-vpc-toumoro-projen-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 18:08:50.000000 cdk-vpc-toumoro-projen-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-06 18:09:00.217244 cdk-vpc-toumoro-projen-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 18:08:50.000000 cdk-vpc-toumoro-projen-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 18:08:50.000000 cdk-vpc-toumoro-projen-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 18:09:00.217244 cdk-vpc-toumoro-projen-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-06 18:08:50.000000 cdk-vpc-toumoro-projen-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:09:00.213244 cdk-vpc-toumoro-projen-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:09:00.213244 cdk-vpc-toumoro-projen-1.1.0/src/cdk-vpc-toumoro-projen/
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-06 18:08:50.000000 cdk-vpc-toumoro-projen-1.1.0/src/cdk-vpc-toumoro-projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:09:00.213244 cdk-vpc-toumoro-projen-1.1.0/src/cdk-vpc-toumoro-projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-06 18:08:50.000000 cdk-vpc-toumoro-projen-1.1.0/src/cdk-vpc-toumoro-projen/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29072 2024-05-06 18:08:50.000000 cdk-vpc-toumoro-projen-1.1.0/src/cdk-vpc-toumoro-projen/_jsii/cdk-vpc-toumoro-projen@1.1.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:08:50.000000 cdk-vpc-toumoro-projen-1.1.0/src/cdk-vpc-toumoro-projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:09:00.217244 cdk-vpc-toumoro-projen-1.1.0/src/cdk_vpc_toumoro_projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-06 18:09:00.000000 cdk-vpc-toumoro-projen-1.1.0/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-06 18:09:00.000000 cdk-vpc-toumoro-projen-1.1.0/src/cdk_vpc_toumoro_projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:09:00.000000 cdk-vpc-toumoro-projen-1.1.0/src/cdk_vpc_toumoro_projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-06 18:09:00.000000 cdk-vpc-toumoro-projen-1.1.0/src/cdk_vpc_toumoro_projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 18:09:00.000000 cdk-vpc-toumoro-projen-1.1.0/src/cdk_vpc_toumoro_projen.egg-info/top_level.txt
```

### Comparing `cdk-vpc-toumoro-projen-1.0.0/LICENSE` & `cdk-vpc-toumoro-projen-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-vpc-toumoro-projen-1.0.0/PKG-INFO` & `cdk-vpc-toumoro-projen-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-vpc-toumoro-projen
-Version: 1.0.0
+Version: 1.1.0
 Summary: A CDK construct library to create a VPC with public and private subnets.
 Home-page: https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-vpc-toumoro-projen-1.0.0/setup.py` & `cdk-vpc-toumoro-projen-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-vpc-toumoro-projen",
-    "version": "1.0.0",
+    "version": "1.1.0",
     "description": "A CDK construct library to create a VPC with public and private subnets.",
     "license": "GPL-3.0-or-later",
     "url": "https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git",
     "long_description_content_type": "text/markdown",
     "author": "tm-lcarvalho<lucio.carvalho@toumoro.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk-vpc-toumoro-projen",
         "cdk-vpc-toumoro-projen._jsii"
     ],
     "package_data": {
         "cdk-vpc-toumoro-projen._jsii": [
-            "cdk-vpc-toumoro-projen@1.0.0.jsii.tgz"
+            "cdk-vpc-toumoro-projen@1.1.0.jsii.tgz"
         ],
         "cdk-vpc-toumoro-projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-vpc-toumoro-projen-1.0.0/src/cdk-vpc-toumoro-projen/__init__.py` & `cdk-vpc-toumoro-projen-1.1.0/src/cdk-vpc-toumoro-projen/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,28 +34,38 @@
         ...
 
     @builtins.property
     @jsii.member(jsii_name="maxAzs")
     def max_azs(self) -> typing.Optional[jsii.Number]:
         ...
 
+    @builtins.property
+    @jsii.member(jsii_name="natGateways")
+    def nat_gateways(self) -> typing.Optional[jsii.Number]:
+        ...
+
 
 class _IVpcBaseProxy:
     __jsii_type__: typing.ClassVar[str] = "cdk-vpc-toumoro-projen.IVpcBase"
 
     @builtins.property
     @jsii.member(jsii_name="cidr")
     def cidr(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "cidr"))
 
     @builtins.property
     @jsii.member(jsii_name="maxAzs")
     def max_azs(self) -> typing.Optional[jsii.Number]:
         return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "maxAzs"))
 
+    @builtins.property
+    @jsii.member(jsii_name="natGateways")
+    def nat_gateways(self) -> typing.Optional[jsii.Number]:
+        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "natGateways"))
+
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IVpcBase).__jsii_proxy_class__ = lambda : _IVpcBaseProxy
 
 
 class VpcBase(
     _aws_cdk_aws_ec2_ceddda9d.Vpc,
     metaclass=jsii.JSIIMeta,
```

### Comparing `cdk-vpc-toumoro-projen-1.0.0/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO` & `cdk-vpc-toumoro-projen-1.1.0/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-vpc-toumoro-projen
-Version: 1.0.0
+Version: 1.1.0
 Summary: A CDK construct library to create a VPC with public and private subnets.
 Home-page: https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

