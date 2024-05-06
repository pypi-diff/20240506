# Comparing `tmp/ecs_files_composer-2.1.2.tar.gz` & `tmp/ecs_files_composer-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecs_files_composer-2.1.2.tar", max compression
+gzip compressed data, was "ecs_files_composer-2.1.3.tar", max compression
```

## Comparing `ecs_files_composer-2.1.2.tar` & `ecs_files_composer-2.1.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    16725 2022-03-23 11:16:37.079578 ecs_files_composer-2.1.2/LICENSE
--rw-r--r--   0        0        0     3280 2022-03-23 11:16:37.079578 ecs_files_composer-2.1.2/README.rst
--rw-r--r--   0        0        0      223 2024-03-23 07:58:51.458140 ecs_files_composer-2.1.2/ecs_files_composer/__init__.py
--rw-r--r--   0        0        0     7758 2023-10-19 08:22:36.088481 ecs_files_composer-2.1.2/ecs_files_composer/aws_mgmt.py
--rw-r--r--   0        0        0     4182 2023-10-19 08:22:36.089481 ecs_files_composer-2.1.2/ecs_files_composer/certificates_mgmt.py
--rw-r--r--   0        0        0     4804 2023-10-19 08:22:36.089481 ecs_files_composer-2.1.2/ecs_files_composer/cli.py
--rw-r--r--   0        0        0     1605 2023-08-20 14:53:24.555417 ecs_files_composer-2.1.2/ecs_files_composer/common.py
--rw-r--r--   0        0        0     5025 2023-10-19 08:22:36.089481 ecs_files_composer-2.1.2/ecs_files_composer/ecs_files_composer.py
--rw-r--r--   0        0        0     1669 2022-07-27 07:35:08.374630 ecs_files_composer-2.1.2/ecs_files_composer/envsubst.py
--rw-r--r--   0        0        0    13688 2023-10-19 08:22:36.090481 ecs_files_composer-2.1.2/ecs_files_composer/files_mgmt.py
--rw-r--r--   0        0        0     3550 2023-10-19 08:22:36.090481 ecs_files_composer-2.1.2/ecs_files_composer/input.py
--rw-r--r--   0        0        0     3300 2024-02-02 10:43:08.348929 ecs_files_composer-2.1.2/ecs_files_composer/jinja2_filters/__init__.py
--rw-r--r--   0        0        0     1340 2024-02-02 11:02:22.316616 ecs_files_composer-2.1.2/ecs_files_composer/jinja2_functions/__init__.py
--rw-r--r--   0        0        0     6077 2024-02-02 11:02:22.316616 ecs_files_composer-2.1.2/ecs_files_composer/jinja2_functions/aws.py
--rw-r--r--   0        0        0     3055 2024-03-23 07:58:51.458140 ecs_files_composer-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     4648 1970-01-01 00:00:00.000000 ecs_files_composer-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0       95 2022-03-23 11:16:37.079578 ecs_files_composer-2.1.3/AUTHORS.rst
+-rw-r--r--   0        0        0    16725 2022-03-23 11:16:37.079578 ecs_files_composer-2.1.3/LICENSE
+-rw-r--r--   0        0        0     3280 2022-03-23 11:16:37.079578 ecs_files_composer-2.1.3/README.rst
+-rw-r--r--   0        0        0      223 2024-05-06 07:04:37.394686 ecs_files_composer-2.1.3/ecs_files_composer/__init__.py
+-rw-r--r--   0        0        0     7798 2024-05-06 06:14:50.630407 ecs_files_composer-2.1.3/ecs_files_composer/aws_mgmt.py
+-rw-r--r--   0        0        0     4182 2023-10-19 08:22:36.089481 ecs_files_composer-2.1.3/ecs_files_composer/certificates_mgmt.py
+-rw-r--r--   0        0        0     4804 2023-10-19 08:22:36.089481 ecs_files_composer-2.1.3/ecs_files_composer/cli.py
+-rw-r--r--   0        0        0     1605 2023-08-20 14:53:24.555417 ecs_files_composer-2.1.3/ecs_files_composer/common.py
+-rw-r--r--   0        0        0     5025 2023-10-19 08:22:36.089481 ecs_files_composer-2.1.3/ecs_files_composer/ecs_files_composer.py
+-rw-r--r--   0        0        0     1669 2022-07-27 07:35:08.374630 ecs_files_composer-2.1.3/ecs_files_composer/envsubst.py
+-rw-r--r--   0        0        0    13688 2023-10-19 08:22:36.090481 ecs_files_composer-2.1.3/ecs_files_composer/files_mgmt.py
+-rw-r--r--   0        0        0     3550 2023-10-19 08:22:36.090481 ecs_files_composer-2.1.3/ecs_files_composer/input.py
+-rw-r--r--   0        0        0     3300 2024-02-02 10:43:08.348929 ecs_files_composer-2.1.3/ecs_files_composer/jinja2_filters/__init__.py
+-rw-r--r--   0        0        0     1340 2024-02-02 11:02:22.316616 ecs_files_composer-2.1.3/ecs_files_composer/jinja2_functions/__init__.py
+-rw-r--r--   0        0        0     6077 2024-02-02 11:02:22.316616 ecs_files_composer-2.1.3/ecs_files_composer/jinja2_functions/aws.py
+-rw-r--r--   0        0        0     3062 2024-05-06 07:04:37.394686 ecs_files_composer-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4699 1970-01-01 00:00:00.000000 ecs_files_composer-2.1.3/PKG-INFO
```

### Comparing `ecs_files_composer-2.1.2/LICENSE` & `ecs_files_composer-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.2/README.rst` & `ecs_files_composer-2.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.2/ecs_files_composer/aws_mgmt.py` & `ecs_files_composer-2.1.3/ecs_files_composer/aws_mgmt.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,17 +54,19 @@
         client_session = create_session_from_creds(
             tmp_creds, region=iam_config_object.RegionName
         )
     else:
         client_session = boto3.session.Session(
             aws_access_key_id=iam_config_object.AccessKeyId,
             aws_secret_access_key=iam_config_object.SecretAccessKey,
-            aws_session_token=iam_config_object.SessionToken
-            if iam_config_object.SessionToken
-            else None,
+            aws_session_token=(
+                iam_config_object.SessionToken
+                if iam_config_object.SessionToken
+                else None
+            ),
         )
     return client_session
 
 
 class AwsResourceHandler:
     """
     Class to handle all AWS related credentials init.
```

### Comparing `ecs_files_composer-2.1.2/ecs_files_composer/certificates_mgmt.py` & `ecs_files_composer-2.1.3/ecs_files_composer/certificates_mgmt.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.2/ecs_files_composer/cli.py` & `ecs_files_composer-2.1.3/ecs_files_composer/cli.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.2/ecs_files_composer/common.py` & `ecs_files_composer-2.1.3/ecs_files_composer/common.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.2/ecs_files_composer/ecs_files_composer.py` & `ecs_files_composer-2.1.3/ecs_files_composer/ecs_files_composer.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.2/ecs_files_composer/envsubst.py` & `ecs_files_composer-2.1.3/ecs_files_composer/envsubst.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.2/ecs_files_composer/files_mgmt.py` & `ecs_files_composer-2.1.3/ecs_files_composer/files_mgmt.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.2/ecs_files_composer/input.py` & `ecs_files_composer-2.1.3/ecs_files_composer/input.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.2/ecs_files_composer/jinja2_filters/__init__.py` & `ecs_files_composer-2.1.3/ecs_files_composer/jinja2_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.2/ecs_files_composer/jinja2_functions/__init__.py` & `ecs_files_composer-2.1.3/ecs_files_composer/jinja2_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.2/ecs_files_composer/jinja2_functions/aws.py` & `ecs_files_composer-2.1.3/ecs_files_composer/jinja2_functions/aws.py`

 * *Files identical despite different names*

### Comparing `ecs_files_composer-2.1.2/pyproject.toml` & `ecs_files_composer-2.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecs_files_composer"
-version = "2.1.2"
+version = "2.1.3"
 description = "Files and configuration handler to inject configuration files into volumes for ECS containers"
 authors = ["John Preston <john@compose-x.io>"]
 license = "MPL-2.0"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
@@ -31,15 +31,15 @@
 flatdict = "^4.0.1"
 aws-cfn-custom-resource-resolve-parser = "^0.3.0"
 dacite = "^1.8.1"
 
 [tool.poetry.group.dev.dependencies]
 placebo = "^0.10"
 datamodel-code-generator = {extras = ["http"], version = "^0.21"}
-black = "^23.1"
+black = ">=23.1,<25.0"
 isort = "^5.10.1"
 coverage = "^7.1"
 behave = "^1.2.6"
 pytest = "^7"
 watchdog = "^3.0"
 pre-commit = "^3.3"
 tbump = "^6.9.0"
@@ -94,15 +94,15 @@
 
 omit = ["ecs_files_composer/cli.py"]
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/ecs-files-composer"
 
 [tool.tbump.version]
-current = "2.1.2"
+current = "2.1.3"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `ecs_files_composer-2.1.2/PKG-INFO` & `ecs_files_composer-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecs_files_composer
-Version: 2.1.2
+Version: 2.1.3
 Summary: Files and configuration handler to inject configuration files into volumes for ECS containers
 License: MPL-2.0
 Keywords: aws,ecs,k8s,secrets
 Author: John Preston
 Author-email: john@compose-x.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,14 +15,15 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: aws-cfn-custom-resource-resolve-parser (>=0.3.0,<0.4.0)
 Requires-Dist: boto3 (>=1.28,<2.0)
 Requires-Dist: compose-x-common (>=1.3,<2.0)
 Requires-Dist: dacite (>=1.8.1,<2.0.0)
 Requires-Dist: flatdict (>=4.0.1,<5.0.0)
```

