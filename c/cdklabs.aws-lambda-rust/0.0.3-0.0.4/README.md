# Comparing `tmp/cdklabs.aws-lambda-rust-0.0.3.tar.gz` & `tmp/cdklabs.aws-lambda-rust-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.aws-lambda-rust-0.0.3.tar", last modified: Wed Jan 31 16:12:03 2024, max compression
+gzip compressed data, was "cdklabs.aws-lambda-rust-0.0.4.tar", last modified: Mon May  6 06:07:38 2024, max compression
```

## Comparing `cdklabs.aws-lambda-rust-0.0.3.tar` & `cdklabs.aws-lambda-rust-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:12:03.377767 cdklabs.aws-lambda-rust-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-01-31 16:11:50.000000 cdklabs.aws-lambda-rust-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-31 16:11:50.000000 cdklabs.aws-lambda-rust-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-01-31 16:12:03.377767 cdklabs.aws-lambda-rust-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-01-31 16:11:50.000000 cdklabs.aws-lambda-rust-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-31 16:11:50.000000 cdklabs.aws-lambda-rust-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 16:12:03.377767 cdklabs.aws-lambda-rust-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-01-31 16:11:50.000000 cdklabs.aws-lambda-rust-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:12:03.373767 cdklabs.aws-lambda-rust-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:12:03.373767 cdklabs.aws-lambda-rust-0.0.3/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:12:03.373767 cdklabs.aws-lambda-rust-0.0.3/src/cdklabs/aws_lambda_rust/
--rw-r--r--   0 runner    (1001) docker     (127)   112390 2024-01-31 16:11:50.000000 cdklabs.aws-lambda-rust-0.0.3/src/cdklabs/aws_lambda_rust/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:12:03.373767 cdklabs.aws-lambda-rust-0.0.3/src/cdklabs/aws_lambda_rust/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-01-31 16:11:50.000000 cdklabs.aws-lambda-rust-0.0.3/src/cdklabs/aws_lambda_rust/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    88453 2024-01-31 16:11:50.000000 cdklabs.aws-lambda-rust-0.0.3/src/cdklabs/aws_lambda_rust/_jsii/aws-lambda-rust@0.0.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 16:11:50.000000 cdklabs.aws-lambda-rust-0.0.3/src/cdklabs/aws_lambda_rust/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:12:03.373767 cdklabs.aws-lambda-rust-0.0.3/src/cdklabs.aws_lambda_rust.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-01-31 16:12:03.000000 cdklabs.aws-lambda-rust-0.0.3/src/cdklabs.aws_lambda_rust.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-01-31 16:12:03.000000 cdklabs.aws-lambda-rust-0.0.3/src/cdklabs.aws_lambda_rust.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 16:12:03.000000 cdklabs.aws-lambda-rust-0.0.3/src/cdklabs.aws_lambda_rust.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-31 16:12:03.000000 cdklabs.aws-lambda-rust-0.0.3/src/cdklabs.aws_lambda_rust.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-31 16:12:03.000000 cdklabs.aws-lambda-rust-0.0.3/src/cdklabs.aws_lambda_rust.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:07:38.569787 cdklabs.aws-lambda-rust-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-06 06:07:26.000000 cdklabs.aws-lambda-rust-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 06:07:26.000000 cdklabs.aws-lambda-rust-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-05-06 06:07:38.569787 cdklabs.aws-lambda-rust-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-05-06 06:07:26.000000 cdklabs.aws-lambda-rust-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 06:07:26.000000 cdklabs.aws-lambda-rust-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:07:38.569787 cdklabs.aws-lambda-rust-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-06 06:07:26.000000 cdklabs.aws-lambda-rust-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:07:38.565787 cdklabs.aws-lambda-rust-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:07:38.565787 cdklabs.aws-lambda-rust-0.0.4/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:07:38.569787 cdklabs.aws-lambda-rust-0.0.4/src/cdklabs/aws_lambda_rust/
+-rw-r--r--   0 runner    (1001) docker     (127)   112466 2024-05-06 06:07:26.000000 cdklabs.aws-lambda-rust-0.0.4/src/cdklabs/aws_lambda_rust/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:07:38.569787 cdklabs.aws-lambda-rust-0.0.4/src/cdklabs/aws_lambda_rust/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-06 06:07:26.000000 cdklabs.aws-lambda-rust-0.0.4/src/cdklabs/aws_lambda_rust/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88454 2024-05-06 06:07:26.000000 cdklabs.aws-lambda-rust-0.0.4/src/cdklabs/aws_lambda_rust/_jsii/aws-lambda-rust@0.0.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:07:26.000000 cdklabs.aws-lambda-rust-0.0.4/src/cdklabs/aws_lambda_rust/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:07:38.569787 cdklabs.aws-lambda-rust-0.0.4/src/cdklabs.aws_lambda_rust.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-05-06 06:07:38.000000 cdklabs.aws-lambda-rust-0.0.4/src/cdklabs.aws_lambda_rust.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-06 06:07:38.000000 cdklabs.aws-lambda-rust-0.0.4/src/cdklabs.aws_lambda_rust.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:07:38.000000 cdklabs.aws-lambda-rust-0.0.4/src/cdklabs.aws_lambda_rust.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-06 06:07:38.000000 cdklabs.aws-lambda-rust-0.0.4/src/cdklabs.aws_lambda_rust.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 06:07:38.000000 cdklabs.aws-lambda-rust-0.0.4/src/cdklabs.aws_lambda_rust.egg-info/top_level.txt
```

### Comparing `cdklabs.aws-lambda-rust-0.0.3/LICENSE` & `cdklabs.aws-lambda-rust-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.aws-lambda-rust-0.0.3/PKG-INFO` & `cdklabs.aws-lambda-rust-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.aws-lambda-rust
-Version: 0.0.3
+Version: 0.0.4
 Summary: @cdklabs/aws-lambda-rust
 Home-page: https://github.com/cdklabs/aws-lambda-rust.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/aws-lambda-rust.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.aws-lambda-rust-0.0.3/README.md` & `cdklabs.aws-lambda-rust-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cdklabs.aws-lambda-rust-0.0.3/setup.py` & `cdklabs.aws-lambda-rust-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.aws-lambda-rust",
-    "version": "0.0.3",
+    "version": "0.0.4",
     "description": "@cdklabs/aws-lambda-rust",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/aws-lambda-rust.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cdklabs.aws_lambda_rust",
         "cdklabs.aws_lambda_rust._jsii"
     ],
     "package_data": {
         "cdklabs.aws_lambda_rust._jsii": [
-            "aws-lambda-rust@0.0.3.jsii.tgz"
+            "aws-lambda-rust@0.0.4.jsii.tgz"
         ],
         "cdklabs.aws_lambda_rust": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.121.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.94.0, <2.0.0",
+        "jsii>=1.97.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdklabs.aws-lambda-rust-0.0.3/src/cdklabs/aws_lambda_rust/__init__.py` & `cdklabs.aws-lambda-rust-0.0.4/src/cdklabs/aws_lambda_rust/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,17 @@
 * **afterBundling**: runs after all bundling commands
 
 They all receive the directory containing the lock file (inputDir) and the directory where the bundled asset will be output (outputDir).
 They must return an array of commands to run. Commands are chained with &&.
 
 The commands will run in the environment in which bundling occurs: inside the container for Docker bundling or on the host OS for local bundling.
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
```

### Comparing `cdklabs.aws-lambda-rust-0.0.3/src/cdklabs.aws_lambda_rust.egg-info/PKG-INFO` & `cdklabs.aws-lambda-rust-0.0.4/src/cdklabs.aws_lambda_rust.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.aws-lambda-rust
-Version: 0.0.3
+Version: 0.0.4
 Summary: @cdklabs/aws-lambda-rust
 Home-page: https://github.com/cdklabs/aws-lambda-rust.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/aws-lambda-rust.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

