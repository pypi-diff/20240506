# Comparing `tmp/projen-0.81.5.tar.gz` & `tmp/projen-0.81.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projen-0.81.5.tar", last modified: Mon Apr 29 16:37:35 2024, max compression
+gzip compressed data, was "projen-0.81.6.tar", last modified: Mon May  6 09:46:16 2024, max compression
```

## Comparing `projen-0.81.5.tar` & `projen-0.81.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.029273 projen-0.81.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-29 16:37:22.000000 projen-0.81.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 16:37:22.000000 projen-0.81.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-04-29 16:37:35.029273 projen-0.81.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    78674 2024-04-29 16:37:22.000000 projen-0.81.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 16:37:22.000000 projen-0.81.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:37:35.029273 projen-0.81.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-29 16:37:22.000000 projen-0.81.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.013273 projen-0.81.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.013273 projen-0.81.5/src/projen/
--rw-r--r--   0 runner    (1001) docker     (127)   651984 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.017273 projen-0.81.5/src/projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.021273 projen-0.81.5/src/projen/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/_jsii/bin/projen
--rw-r--r--   0 runner    (1001) docker     (127)  2650821 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/_jsii/projen@0.81.5.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.021273 projen-0.81.5/src/projen/awscdk/
--rw-r--r--   0 runner    (1001) docker     (127)  1079302 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/awscdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.021273 projen-0.81.5/src/projen/build/
--rw-r--r--   0 runner    (1001) docker     (127)    52320 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.021273 projen-0.81.5/src/projen/cdk/
--rw-r--r--   0 runner    (1001) docker     (127)   510147 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.021273 projen-0.81.5/src/projen/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (127)   597384 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.021273 projen-0.81.5/src/projen/cdktf/
--rw-r--r--   0 runner    (1001) docker     (127)   224466 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/cdktf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.021273 projen-0.81.5/src/projen/circleci/
--rw-r--r--   0 runner    (1001) docker     (127)    75913 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/circleci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.025273 projen-0.81.5/src/projen/github/
--rw-r--r--   0 runner    (1001) docker     (127)   409613 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.025273 projen-0.81.5/src/projen/github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)   250737 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/github/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.025273 projen-0.81.5/src/projen/gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)   202810 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/gitlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.025273 projen-0.81.5/src/projen/java/
--rw-r--r--   0 runner    (1001) docker     (127)   183709 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.025273 projen-0.81.5/src/projen/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)   844523 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/javascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.025273 projen-0.81.5/src/projen/python/
--rw-r--r--   0 runner    (1001) docker     (127)   213158 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.025273 projen-0.81.5/src/projen/release/
--rw-r--r--   0 runner    (1001) docker     (127)   285447 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.025273 projen-0.81.5/src/projen/typescript/
--rw-r--r--   0 runner    (1001) docker     (127)   474506 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/typescript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.029273 projen-0.81.5/src/projen/vscode/
--rw-r--r--   0 runner    (1001) docker     (127)    69040 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/vscode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.029273 projen-0.81.5/src/projen/web/
--rw-r--r--   0 runner    (1001) docker     (127)   797444 2024-04-29 16:37:22.000000 projen-0.81.5/src/projen/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:37:35.017273 projen-0.81.5/src/projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-04-29 16:37:34.000000 projen-0.81.5/src/projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-29 16:37:34.000000 projen-0.81.5/src/projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:37:34.000000 projen-0.81.5/src/projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-29 16:37:34.000000 projen-0.81.5/src/projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 16:37:34.000000 projen-0.81.5/src/projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.518275 projen-0.81.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-06 09:46:06.000000 projen-0.81.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 09:46:06.000000 projen-0.81.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-05-06 09:46:16.518275 projen-0.81.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    78674 2024-05-06 09:46:06.000000 projen-0.81.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 09:46:06.000000 projen-0.81.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:46:16.518275 projen-0.81.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-06 09:46:06.000000 projen-0.81.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.498274 projen-0.81.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.502274 projen-0.81.6/src/projen/
+-rw-r--r--   0 runner    (1001) docker     (127)   651984 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.502274 projen-0.81.6/src/projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.506274 projen-0.81.6/src/projen/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/_jsii/bin/projen
+-rw-r--r--   0 runner    (1001) docker     (127)  2650836 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/_jsii/projen@0.81.6.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.506274 projen-0.81.6/src/projen/awscdk/
+-rw-r--r--   0 runner    (1001) docker     (127)  1079302 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/awscdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.506274 projen-0.81.6/src/projen/build/
+-rw-r--r--   0 runner    (1001) docker     (127)    52320 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.510275 projen-0.81.6/src/projen/cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)   510147 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.510275 projen-0.81.6/src/projen/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (127)   597384 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.510275 projen-0.81.6/src/projen/cdktf/
+-rw-r--r--   0 runner    (1001) docker     (127)   224466 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/cdktf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.510275 projen-0.81.6/src/projen/circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)    75913 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/circleci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.510275 projen-0.81.6/src/projen/github/
+-rw-r--r--   0 runner    (1001) docker     (127)   409613 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.510275 projen-0.81.6/src/projen/github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)   250737 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/github/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.510275 projen-0.81.6/src/projen/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)   202810 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/gitlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.510275 projen-0.81.6/src/projen/java/
+-rw-r--r--   0 runner    (1001) docker     (127)   183709 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.510275 projen-0.81.6/src/projen/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)   844523 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/javascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.514274 projen-0.81.6/src/projen/python/
+-rw-r--r--   0 runner    (1001) docker     (127)   213158 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.514274 projen-0.81.6/src/projen/release/
+-rw-r--r--   0 runner    (1001) docker     (127)   285447 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.514274 projen-0.81.6/src/projen/typescript/
+-rw-r--r--   0 runner    (1001) docker     (127)   474506 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/typescript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.514274 projen-0.81.6/src/projen/vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)    69040 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/vscode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.514274 projen-0.81.6/src/projen/web/
+-rw-r--r--   0 runner    (1001) docker     (127)   797444 2024-05-06 09:46:06.000000 projen-0.81.6/src/projen/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:46:16.502274 projen-0.81.6/src/projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-05-06 09:46:16.000000 projen-0.81.6/src/projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-06 09:46:16.000000 projen-0.81.6/src/projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:46:16.000000 projen-0.81.6/src/projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-06 09:46:16.000000 projen-0.81.6/src/projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 09:46:16.000000 projen-0.81.6/src/projen.egg-info/top_level.txt
```

### Comparing `projen-0.81.5/LICENSE` & `projen-0.81.6/LICENSE`

 * *Files identical despite different names*

### Comparing `projen-0.81.5/PKG-INFO` & `projen-0.81.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.81.5
+Version: 0.81.6
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.81.5/README.md` & `projen-0.81.6/README.md`

 * *Files identical despite different names*

### Comparing `projen-0.81.5/setup.py` & `projen-0.81.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "projen",
-    "version": "0.81.5",
+    "version": "0.81.6",
     "description": "CDK for software projects",
     "license": "Apache-2.0",
     "url": "https://github.com/projen/projen.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -38,24 +38,24 @@
         "projen.release",
         "projen.typescript",
         "projen.vscode",
         "projen.web"
     ],
     "package_data": {
         "projen._jsii": [
-            "projen@0.81.5.jsii.tgz"
+            "projen@0.81.6.jsii.tgz"
         ],
         "projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "constructs>=10.0.0, <11.0.0",
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

### Comparing `projen-0.81.5/src/projen/__init__.py` & `projen-0.81.6/src/projen/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.5/src/projen/awscdk/__init__.py` & `projen-0.81.6/src/projen/awscdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8893,15 +8893,15 @@
         NOTE: The jsii compiler releases since 5.0.0 are not semantically versioned
         and should remain on the same minor, so we recommend using a ``~`` dependency
         (e.g. ``~5.0.0``).
 
         :default: "1.x"
 
         :stability: experimental
-        :pjnew: "~5.0.0"
+        :pjnew: "~5.4.0"
         '''
         result = self._values.get("jsii_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def publish_to_go(self) -> typing.Optional[_JsiiGoTarget_921d41d5]:
         '''(experimental) Publish Go bindings to a git repository.
@@ -18008,15 +18008,15 @@
         NOTE: The jsii compiler releases since 5.0.0 are not semantically versioned
         and should remain on the same minor, so we recommend using a ``~`` dependency
         (e.g. ``~5.0.0``).
 
         :default: "1.x"
 
         :stability: experimental
-        :pjnew: "~5.0.0"
+        :pjnew: "~5.4.0"
         '''
         result = self._values.get("jsii_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def publish_to_go(self) -> typing.Optional[_JsiiGoTarget_921d41d5]:
         '''(experimental) Publish Go bindings to a git repository.
```

### Comparing `projen-0.81.5/src/projen/build/__init__.py` & `projen-0.81.6/src/projen/build/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.5/src/projen/cdk/__init__.py` & `projen-0.81.6/src/projen/cdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4741,15 +4741,15 @@
         NOTE: The jsii compiler releases since 5.0.0 are not semantically versioned
         and should remain on the same minor, so we recommend using a ``~`` dependency
         (e.g. ``~5.0.0``).
 
         :default: "1.x"
 
         :stability: experimental
-        :pjnew: "~5.0.0"
+        :pjnew: "~5.4.0"
         '''
         result = self._values.get("jsii_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def publish_to_go(self) -> typing.Optional[JsiiGoTarget]:
         '''(experimental) Publish Go bindings to a git repository.
@@ -8497,15 +8497,15 @@
         NOTE: The jsii compiler releases since 5.0.0 are not semantically versioned
         and should remain on the same minor, so we recommend using a ``~`` dependency
         (e.g. ``~5.0.0``).
 
         :default: "1.x"
 
         :stability: experimental
-        :pjnew: "~5.0.0"
+        :pjnew: "~5.4.0"
         '''
         result = self._values.get("jsii_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def publish_to_go(self) -> typing.Optional[JsiiGoTarget]:
         '''(experimental) Publish Go bindings to a git repository.
```

### Comparing `projen-0.81.5/src/projen/cdk8s/__init__.py` & `projen-0.81.6/src/projen/cdk8s/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9476,15 +9476,15 @@
         NOTE: The jsii compiler releases since 5.0.0 are not semantically versioned
         and should remain on the same minor, so we recommend using a ``~`` dependency
         (e.g. ``~5.0.0``).
 
         :default: "1.x"
 
         :stability: experimental
-        :pjnew: "~5.0.0"
+        :pjnew: "~5.4.0"
         '''
         result = self._values.get("jsii_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def publish_to_go(self) -> typing.Optional[_JsiiGoTarget_921d41d5]:
         '''(experimental) Publish Go bindings to a git repository.
```

### Comparing `projen-0.81.5/src/projen/cdktf/__init__.py` & `projen-0.81.6/src/projen/cdktf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3553,15 +3553,15 @@
         NOTE: The jsii compiler releases since 5.0.0 are not semantically versioned
         and should remain on the same minor, so we recommend using a ``~`` dependency
         (e.g. ``~5.0.0``).
 
         :default: "1.x"
 
         :stability: experimental
-        :pjnew: "~5.0.0"
+        :pjnew: "~5.4.0"
         '''
         result = self._values.get("jsii_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def publish_to_go(self) -> typing.Optional[_JsiiGoTarget_921d41d5]:
         '''(experimental) Publish Go bindings to a git repository.
```

### Comparing `projen-0.81.5/src/projen/circleci/__init__.py` & `projen-0.81.6/src/projen/circleci/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.5/src/projen/github/__init__.py` & `projen-0.81.6/src/projen/github/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.5/src/projen/github/workflows/__init__.py` & `projen-0.81.6/src/projen/github/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.5/src/projen/gitlab/__init__.py` & `projen-0.81.6/src/projen/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.5/src/projen/java/__init__.py` & `projen-0.81.6/src/projen/java/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.5/src/projen/javascript/__init__.py` & `projen-0.81.6/src/projen/javascript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.5/src/projen/python/__init__.py` & `projen-0.81.6/src/projen/python/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.5/src/projen/release/__init__.py` & `projen-0.81.6/src/projen/release/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.5/src/projen/typescript/__init__.py` & `projen-0.81.6/src/projen/typescript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.5/src/projen/vscode/__init__.py` & `projen-0.81.6/src/projen/vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.5/src/projen/web/__init__.py` & `projen-0.81.6/src/projen/web/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.5/src/projen.egg-info/PKG-INFO` & `projen-0.81.6/src/projen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.81.5
+Version: 0.81.6
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.81.5/src/projen.egg-info/SOURCES.txt` & `projen-0.81.6/src/projen.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/projen/py.typed
 src/projen.egg-info/PKG-INFO
 src/projen.egg-info/SOURCES.txt
 src/projen.egg-info/dependency_links.txt
 src/projen.egg-info/requires.txt
 src/projen.egg-info/top_level.txt
 src/projen/_jsii/__init__.py
-src/projen/_jsii/projen@0.81.5.jsii.tgz
+src/projen/_jsii/projen@0.81.6.jsii.tgz
 src/projen/_jsii/bin/projen
 src/projen/awscdk/__init__.py
 src/projen/build/__init__.py
 src/projen/cdk/__init__.py
 src/projen/cdk8s/__init__.py
 src/projen/cdktf/__init__.py
 src/projen/circleci/__init__.py
```

