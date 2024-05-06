# Comparing `tmp/gammarers.aws-waf-ip-restriction-rule-group-1.4.0.tar.gz` & `tmp/gammarers.aws-waf-ip-restriction-rule-group-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarers.aws-waf-ip-restriction-rule-group-1.4.0.tar", last modified: Fri Apr 26 09:31:40 2024, max compression
+gzip compressed data, was "gammarers.aws-waf-ip-restriction-rule-group-1.4.1.tar", last modified: Mon May  6 19:20:50 2024, max compression
```

## Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.0.tar` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:31:40.015387 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-26 09:31:30.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-26 09:31:30.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-26 09:31:40.015387 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-26 09:31:30.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-26 09:31:30.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 09:31:40.015387 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-26 09:31:30.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:31:40.015387 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:31:40.015387 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/gammarers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:31:40.015387 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/gammarers/aws_waf_ip_restriction_rule_group/
--rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-26 09:31:30.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/gammarers/aws_waf_ip_restriction_rule_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:31:40.015387 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-26 09:31:30.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23962 2024-04-26 09:31:30.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/aws-waf-ip-restriction-rule-group@1.4.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:31:30.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/gammarers/aws_waf_ip_restriction_rule_group/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:31:40.015387 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-26 09:31:39.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-26 09:31:39.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:31:39.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-26 09:31:39.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 09:31:39.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:20:50.932695 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-06 19:20:40.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 19:20:40.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-06 19:20:50.932695 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-06 19:20:40.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 19:20:40.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:20:50.932695 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-06 19:20:40.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:20:50.932695 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:20:50.932695 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/gammarers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:20:50.932695 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/gammarers/aws_waf_ip_restriction_rule_group/
+-rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-05-06 19:20:40.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/gammarers/aws_waf_ip_restriction_rule_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:20:50.932695 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-06 19:20:40.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23966 2024-05-06 19:20:40.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/aws-waf-ip-restriction-rule-group@1.4.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:20:40.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/gammarers/aws_waf_ip_restriction_rule_group/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:20:50.932695 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-06 19:20:50.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-06 19:20:50.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:20:50.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-06 19:20:50.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 19:20:50.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/top_level.txt
```

### Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.0/LICENSE` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.0/PKG-INFO` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-waf-ip-restriction-rule-group
-Version: 1.4.0
+Version: 1.4.1
 Summary: This is an AWS CDK Construct for IP Restriction Rule Group on WAF V2
 Home-page: https://github.com/gammarers/aws-waf-ip-restriction-rule-group.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-waf-ip-restriction-rule-group.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.0/README.md` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.0/setup.py` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarers.aws-waf-ip-restriction-rule-group",
-    "version": "1.4.0",
+    "version": "1.4.1",
     "description": "This is an AWS CDK Construct for IP Restriction Rule Group on WAF V2",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarers/aws-waf-ip-restriction-rule-group.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "gammarers.aws_waf_ip_restriction_rule_group",
         "gammarers.aws_waf_ip_restriction_rule_group._jsii"
     ],
     "package_data": {
         "gammarers.aws_waf_ip_restriction_rule_group._jsii": [
-            "aws-waf-ip-restriction-rule-group@1.4.0.jsii.tgz"
+            "aws-waf-ip-restriction-rule-group@1.4.1.jsii.tgz"
         ],
         "gammarers.aws_waf_ip_restriction_rule_group": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.80.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.97.0, <2.0.0",
+        "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/gammarers/aws_waf_ip_restriction_rule_group/__init__.py` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/gammarers/aws_waf_ip_restriction_rule_group/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/__init__.py` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarers/aws-waf-ip-restriction-rule-group",
-    "1.4.0",
+    "1.4.1",
     __name__[0:-6],
-    "aws-waf-ip-restriction-rule-group@1.4.0.jsii.tgz",
+    "aws-waf-ip-restriction-rule-group@1.4.1.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/PKG-INFO` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-waf-ip-restriction-rule-group
-Version: 1.4.0
+Version: 1.4.1
 Summary: This is an AWS CDK Construct for IP Restriction Rule Group on WAF V2
 Home-page: https://github.com/gammarers/aws-waf-ip-restriction-rule-group.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-waf-ip-restriction-rule-group.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.0/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/SOURCES.txt` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.1/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/SOURCES.txt
 src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/dependency_links.txt
 src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/requires.txt
 src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/top_level.txt
 src/gammarers/aws_waf_ip_restriction_rule_group/__init__.py
 src/gammarers/aws_waf_ip_restriction_rule_group/py.typed
 src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/__init__.py
-src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/aws-waf-ip-restriction-rule-group@1.4.0.jsii.tgz
+src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/aws-waf-ip-restriction-rule-group@1.4.1.jsii.tgz
```
