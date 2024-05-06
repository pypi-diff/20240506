# Comparing `tmp/truefoundry-0.2.0rc8.tar.gz` & `tmp/truefoundry-0.2.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truefoundry-0.2.0rc8.tar", max compression
+gzip compressed data, was "truefoundry-0.2.0rc9.tar", max compression
```

## Comparing `truefoundry-0.2.0rc8.tar` & `truefoundry-0.2.0rc9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      871 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/README.md
--rw-r--r--   0        0        0     1170 2024-04-26 13:38:45.073514 truefoundry-0.2.0rc8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/truefoundry/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/truefoundry/autodeploy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/__init__.py
--rw-r--r--   0        0        0     6405 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/base.py
--rw-r--r--   0        0        0     4126 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/developer.py
--rw-r--r--   0        0        0     4438 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/project_identifier.py
--rw-r--r--   0        0        0     2352 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/tester.py
--rw-r--r--   0        0        0    12317 2024-04-26 13:38:33.433473 truefoundry-0.2.0rc8/truefoundry/autodeploy/cli.py
--rw-r--r--   0        0        0     1111 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/constants.py
--rw-r--r--   0        0        0       54 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/exception.py
--rw-r--r--   0        0        0      325 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/logger.py
--rw-r--r--   0        0        0      875 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/__init__.py
--rw-r--r--   0        0        0      856 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/ask.py
--rw-r--r--   0        0        0      665 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/base.py
--rw-r--r--   0        0        0     5892 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/commit.py
--rw-r--r--   0        0        0     3931 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/docker_build.py
--rw-r--r--   0        0        0     5078 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/docker_run.py
--rw-r--r--   0        0        0     2288 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/file_type_counts.py
--rw-r--r--   0        0        0     2577 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/list_files.py
--rw-r--r--   0        0        0     1751 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/read_file.py
--rw-r--r--   0        0        0     1614 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/send_request.py
--rw-r--r--   0        0        0     3130 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/write_file.py
--rw-r--r--   0        0        0     5358 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/utils/diff.py
--rw-r--r--   0        0        0      412 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/autodeploy/utils/pydantic_compat.py
--rw-r--r--   0        0        0        0 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/cli/__init__.py
--rw-r--r--   0        0        0      916 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/cli/__main__.py
--rw-r--r--   0        0        0       43 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/deploy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/deploy/cli/__init__.py
--rw-r--r--   0        0        0     2994 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/deploy/cli/cli.py
--rw-r--r--   0        0        0     5524 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/deploy/cli/deploy.py
--rw-r--r--   0        0        0       53 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/langchain/__init__.py
--rw-r--r--   0        0        0      179 2024-04-26 13:38:33.437473 truefoundry-0.2.0rc8/truefoundry/ml/__init__.py
--rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 truefoundry-0.2.0rc8/PKG-INFO
+-rw-r--r--   0        0        0      871 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/README.md
+-rw-r--r--   0        0        0     1169 2024-05-06 20:41:40.627005 truefoundry-0.2.0rc9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/agents/__init__.py
+-rw-r--r--   0        0        0     6405 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/agents/base.py
+-rw-r--r--   0        0        0     4126 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/agents/developer.py
+-rw-r--r--   0        0        0     4438 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/agents/project_identifier.py
+-rw-r--r--   0        0        0     2352 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/agents/tester.py
+-rw-r--r--   0        0        0    12317 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/cli.py
+-rw-r--r--   0        0        0     1111 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/constants.py
+-rw-r--r--   0        0        0       54 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/exception.py
+-rw-r--r--   0        0        0      325 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/logger.py
+-rw-r--r--   0        0        0      875 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/__init__.py
+-rw-r--r--   0        0        0      856 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/ask.py
+-rw-r--r--   0        0        0      665 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/base.py
+-rw-r--r--   0        0        0     5892 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/commit.py
+-rw-r--r--   0        0        0     3931 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/docker_build.py
+-rw-r--r--   0        0        0     5078 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/docker_run.py
+-rw-r--r--   0        0        0     2288 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/file_type_counts.py
+-rw-r--r--   0        0        0     2577 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/list_files.py
+-rw-r--r--   0        0        0     1751 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/read_file.py
+-rw-r--r--   0        0        0     1614 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/send_request.py
+-rw-r--r--   0        0        0     3130 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/write_file.py
+-rw-r--r--   0        0        0     5358 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/utils/diff.py
+-rw-r--r--   0        0        0      412 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/autodeploy/utils/pydantic_compat.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      916 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/cli/__main__.py
+-rw-r--r--   0        0        0       43 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/deploy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:41:28.486720 truefoundry-0.2.0rc9/truefoundry/deploy/cli/__init__.py
+-rw-r--r--   0        0        0     2994 2024-05-06 20:41:28.490720 truefoundry-0.2.0rc9/truefoundry/deploy/cli/cli.py
+-rw-r--r--   0        0        0     5524 2024-05-06 20:41:28.490720 truefoundry-0.2.0rc9/truefoundry/deploy/cli/deploy.py
+-rw-r--r--   0        0        0       53 2024-05-06 20:41:28.490720 truefoundry-0.2.0rc9/truefoundry/langchain/__init__.py
+-rw-r--r--   0        0        0      179 2024-05-06 20:41:28.490720 truefoundry-0.2.0rc9/truefoundry/ml/__init__.py
+-rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 truefoundry-0.2.0rc9/PKG-INFO
```

### Comparing `truefoundry-0.2.0rc8/README.md` & `truefoundry-0.2.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/pyproject.toml` & `truefoundry-0.2.0rc9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "truefoundry"
-version = "0.2.0rc8"
+version = "0.2.0rc9"
 description = "Truefoundry CLI"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.13"
-servicefoundry = "0.10.10"
+servicefoundry = "0.10.9"
 mlfoundry = { version = "0.10.9", optional = true }
 openai = "^1.16.2"
 docker = "^7.0.0"
 pydantic = ">=1.10.0,<3"
 rich = "^13.7.1"
 requests = "^2.31.0"
 python-dotenv = "^1.0.1"
```

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/base.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/agents/base.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/developer.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/agents/developer.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/project_identifier.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/agents/project_identifier.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/agents/tester.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/agents/tester.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/cli.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/cli.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/constants.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/constants.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/__init__.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/ask.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/ask.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/base.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/base.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/commit.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/commit.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/docker_build.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/docker_build.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/docker_run.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/docker_run.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/file_type_counts.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/file_type_counts.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/list_files.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/list_files.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/read_file.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/read_file.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/send_request.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/send_request.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/tools/write_file.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/tools/write_file.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/autodeploy/utils/diff.py` & `truefoundry-0.2.0rc9/truefoundry/autodeploy/utils/diff.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/cli/__main__.py` & `truefoundry-0.2.0rc9/truefoundry/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/deploy/cli/cli.py` & `truefoundry-0.2.0rc9/truefoundry/deploy/cli/cli.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/truefoundry/deploy/cli/deploy.py` & `truefoundry-0.2.0rc9/truefoundry/deploy/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.0rc8/PKG-INFO` & `truefoundry-0.2.0rc9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truefoundry
-Version: 0.2.0rc8
+Version: 0.2.0rc9
 Summary: Truefoundry CLI
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,15 +17,15 @@
 Requires-Dist: inquirer (>=3.2.4,<4.0.0)
 Requires-Dist: mlfoundry (==0.10.9) ; extra == "ml"
 Requires-Dist: openai (>=1.16.2,<2.0.0)
 Requires-Dist: pydantic (>=1.10.0,<3)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
-Requires-Dist: servicefoundry (==0.10.10)
+Requires-Dist: servicefoundry (==0.10.9)
 Description-Content-Type: text/markdown
 
 # Truefoundry
 
 TrueFoundry library to help you interact with the platform programmatically by
 
 - Interacting with the deployments side of TrueFoundry, enabling you to manage workspaces, deployments, applications, and view logs.
```

