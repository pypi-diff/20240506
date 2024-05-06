# Comparing `tmp/supersullytools-2.2.0.tar.gz` & `tmp/supersullytools-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supersullytools-2.2.0.tar", last modified: Thu Mar 21 19:41:42 2024, max compression
+gzip compressed data, was "supersullytools-2.3.0.tar", last modified: Mon May  6 20:19:23 2024, max compression
```

## Comparing `supersullytools-2.2.0.tar` & `supersullytools-2.3.0.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-21 19:41:42.106006 supersullytools-2.2.0/
--rw-r--r--   0 msull      (501) staff       (20)     1092 2023-11-08 05:22:30.000000 supersullytools-2.2.0/LICENSE
--rw-r--r--   0 msull      (501) staff       (20)     3169 2024-03-21 19:41:42.105542 supersullytools-2.2.0/PKG-INFO
--rw-r--r--   0 msull      (501) staff       (20)      297 2024-03-21 19:41:35.000000 supersullytools-2.2.0/README.md
--rw-r--r--   0 msull      (501) staff       (20)     2048 2024-03-21 19:41:35.000000 supersullytools-2.2.0/pyproject.toml
--rw-r--r--   0 msull      (501) staff       (20)       38 2024-03-21 19:41:42.106093 supersullytools-2.2.0/setup.cfg
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-21 19:41:42.095392 supersullytools-2.2.0/src/
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-21 19:41:42.096680 supersullytools-2.2.0/src/streamlit_app/
--rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-30 16:56:26.000000 supersullytools-2.2.0/src/streamlit_app/Home.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-21 19:41:42.097299 supersullytools-2.2.0/src/streamlit_app/pages/
--rw-r--r--   0 msull      (501) staff       (20)     3497 2024-02-16 00:42:29.000000 supersullytools-2.2.0/src/streamlit_app/pages/AI Chat.py
--rw-r--r--   0 msull      (501) staff       (20)     1328 2024-02-15 00:27:25.000000 supersullytools-2.2.0/src/streamlit_app/pages/Item Paginator.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-21 19:41:42.097707 supersullytools-2.2.0/src/supersullytools/
--rw-r--r--   0 msull      (501) staff       (20)       26 2024-03-21 19:41:35.000000 supersullytools-2.2.0/src/supersullytools/__init__.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-21 19:41:42.099725 supersullytools-2.2.0/src/supersullytools/openai/
--rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 06:06:46.000000 supersullytools-2.2.0/src/supersullytools/openai/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)     4220 2024-02-16 00:42:29.000000 supersullytools-2.2.0/src/supersullytools/openai/chat_session.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-21 19:41:42.100848 supersullytools-2.2.0/src/supersullytools/streamlit/
--rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 06:06:34.000000 supersullytools-2.2.0/src/supersullytools/streamlit/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)      571 2024-03-21 19:38:09.000000 supersullytools-2.2.0/src/supersullytools/streamlit/misc.py
--rw-r--r--   0 msull      (501) staff       (20)     6115 2023-11-30 16:44:47.000000 supersullytools-2.2.0/src/supersullytools/streamlit/paginator.py
--rw-r--r--   0 msull      (501) staff       (20)    11506 2024-02-16 00:45:03.000000 supersullytools-2.2.0/src/supersullytools/streamlit/sessions.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-21 19:41:42.101374 supersullytools-2.2.0/src/supersullytools/utils/
--rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 18:02:43.000000 supersullytools-2.2.0/src/supersullytools/utils/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)     1396 2024-02-15 22:47:53.000000 supersullytools-2.2.0/src/supersullytools/utils/misc.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-21 19:41:42.102391 supersullytools-2.2.0/src/supersullytools.egg-info/
--rw-r--r--   0 msull      (501) staff       (20)     3169 2024-03-21 19:41:42.000000 supersullytools-2.2.0/src/supersullytools.egg-info/PKG-INFO
--rw-r--r--   0 msull      (501) staff       (20)      758 2024-03-21 19:41:42.000000 supersullytools-2.2.0/src/supersullytools.egg-info/SOURCES.txt
--rw-r--r--   0 msull      (501) staff       (20)        1 2024-03-21 19:41:42.000000 supersullytools-2.2.0/src/supersullytools.egg-info/dependency_links.txt
--rw-r--r--   0 msull      (501) staff       (20)      273 2024-03-21 19:41:42.000000 supersullytools-2.2.0/src/supersullytools.egg-info/requires.txt
--rw-r--r--   0 msull      (501) staff       (20)       36 2024-03-21 19:41:42.000000 supersullytools-2.2.0/src/supersullytools.egg-info/top_level.txt
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-03-21 19:41:42.101988 supersullytools-2.2.0/src/tests/
--rw-r--r--   0 msull      (501) staff       (20)     5073 2024-02-14 23:46:43.000000 supersullytools-2.2.0/src/tests/conftest.py
--rw-r--r--   0 msull      (501) staff       (20)      795 2024-02-16 00:44:38.000000 supersullytools-2.2.0/src/tests/test_streamlit_session.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-06 20:19:23.948541 supersullytools-2.3.0/
+-rw-r--r--   0 msull      (501) staff       (20)     1092 2023-11-08 05:22:30.000000 supersullytools-2.3.0/LICENSE
+-rw-r--r--   0 msull      (501) staff       (20)     3185 2024-05-06 20:19:23.947977 supersullytools-2.3.0/PKG-INFO
+-rw-r--r--   0 msull      (501) staff       (20)      297 2024-05-06 20:19:21.000000 supersullytools-2.3.0/README.md
+-rw-r--r--   0 msull      (501) staff       (20)     2064 2024-05-06 20:19:21.000000 supersullytools-2.3.0/pyproject.toml
+-rw-r--r--   0 msull      (501) staff       (20)       38 2024-05-06 20:19:23.948659 supersullytools-2.3.0/setup.cfg
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-06 20:19:23.934477 supersullytools-2.3.0/src/
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-06 20:19:23.935769 supersullytools-2.3.0/src/streamlit_app/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-30 16:56:26.000000 supersullytools-2.3.0/src/streamlit_app/Home.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-06 20:19:23.936555 supersullytools-2.3.0/src/streamlit_app/pages/
+-rw-r--r--   0 msull      (501) staff       (20)     3497 2024-02-16 00:42:29.000000 supersullytools-2.3.0/src/streamlit_app/pages/AI Chat.py
+-rw-r--r--   0 msull      (501) staff       (20)     1328 2024-02-15 00:27:25.000000 supersullytools-2.3.0/src/streamlit_app/pages/Item Paginator.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-06 20:19:23.937160 supersullytools-2.3.0/src/supersullytools/
+-rw-r--r--   0 msull      (501) staff       (20)       26 2024-05-06 20:19:21.000000 supersullytools-2.3.0/src/supersullytools/__init__.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-06 20:19:23.940025 supersullytools-2.3.0/src/supersullytools/llm/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2024-05-06 20:11:38.000000 supersullytools-2.3.0/src/supersullytools/llm/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)    15063 2024-05-06 20:17:43.000000 supersullytools-2.3.0/src/supersullytools/llm/completions.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-06 20:19:23.940646 supersullytools-2.3.0/src/supersullytools/openai/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 06:06:46.000000 supersullytools-2.3.0/src/supersullytools/openai/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)     4329 2024-05-06 20:17:43.000000 supersullytools-2.3.0/src/supersullytools/openai/chat_session.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-06 20:19:23.941961 supersullytools-2.3.0/src/supersullytools/streamlit/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 06:06:34.000000 supersullytools-2.3.0/src/supersullytools/streamlit/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)      571 2024-03-21 19:38:09.000000 supersullytools-2.3.0/src/supersullytools/streamlit/misc.py
+-rw-r--r--   0 msull      (501) staff       (20)     6115 2023-11-30 16:44:47.000000 supersullytools-2.3.0/src/supersullytools/streamlit/paginator.py
+-rw-r--r--   0 msull      (501) staff       (20)    11506 2024-02-16 00:45:03.000000 supersullytools-2.3.0/src/supersullytools/streamlit/sessions.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-06 20:19:23.942633 supersullytools-2.3.0/src/supersullytools/utils/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 18:02:43.000000 supersullytools-2.3.0/src/supersullytools/utils/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)     1396 2024-02-15 22:47:53.000000 supersullytools-2.3.0/src/supersullytools/utils/misc.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-06 20:19:23.943800 supersullytools-2.3.0/src/supersullytools.egg-info/
+-rw-r--r--   0 msull      (501) staff       (20)     3185 2024-05-06 20:19:23.000000 supersullytools-2.3.0/src/supersullytools.egg-info/PKG-INFO
+-rw-r--r--   0 msull      (501) staff       (20)      833 2024-05-06 20:19:23.000000 supersullytools-2.3.0/src/supersullytools.egg-info/SOURCES.txt
+-rw-r--r--   0 msull      (501) staff       (20)        1 2024-05-06 20:19:23.000000 supersullytools-2.3.0/src/supersullytools.egg-info/dependency_links.txt
+-rw-r--r--   0 msull      (501) staff       (20)      289 2024-05-06 20:19:23.000000 supersullytools-2.3.0/src/supersullytools.egg-info/requires.txt
+-rw-r--r--   0 msull      (501) staff       (20)       36 2024-05-06 20:19:23.000000 supersullytools-2.3.0/src/supersullytools.egg-info/top_level.txt
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-06 20:19:23.943378 supersullytools-2.3.0/src/tests/
+-rw-r--r--   0 msull      (501) staff       (20)     5073 2024-05-06 20:18:38.000000 supersullytools-2.3.0/src/tests/conftest.py
+-rw-r--r--   0 msull      (501) staff       (20)      795 2024-02-16 00:44:38.000000 supersullytools-2.3.0/src/tests/test_streamlit_session.py
```

### Comparing `supersullytools-2.2.0/LICENSE` & `supersullytools-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `supersullytools-2.2.0/PKG-INFO` & `supersullytools-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supersullytools
-Version: 2.2.0
+Version: 2.3.0
 Summary: This is a Python package that brings together a suite of utilities and helpers across several domains of software development.
 Author-email: Sully <sully@sadburger.com>
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: boto3; extra == "dev"
 Requires-Dist: black; extra == "dev"
-Requires-Dist: boto3-stubs[dynamodb]; extra == "dev"
+Requires-Dist: boto3-stubs[bedrock-runtime,dynamodb]; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: diskcache; extra == "dev"
 Requires-Dist: humanize; extra == "dev"
 Requires-Dist: invoke; extra == "dev"
 Requires-Dist: invoke; extra == "dev"
 Requires-Dist: logzero; extra == "dev"
 Requires-Dist: numpy; extra == "dev"
@@ -49,11 +49,11 @@
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
 
 SuperSully Tools
 ================
 
-**Latest Version:** 2.2.0
+**Latest Version:** 2.3.0
 
 **SupersullyTools** is a Python package that brings together a suite of utilities and helpers across several domains of
 software development. My personal toolkit of things I want in every package I'm working on, compiled in one place.
```

### Comparing `supersullytools-2.2.0/pyproject.toml` & `supersullytools-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "supersullytools"
-version = "2.2.0"
+version = "2.3.0"
 description = "This is a Python package that brings together a suite of utilities and helpers across several domains of software development."
 readme = "README.md"
 authors = [{ name = "Sully", email = "sully@sadburger.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -18,15 +18,15 @@
 requires-python = ">=3.10"
 dependencies = []
 
 [project.optional-dependencies]
 dev = [
     "boto3",
     "black",
-    "boto3-stubs[dynamodb]",
+    "boto3-stubs[dynamodb,bedrock-runtime]",
     "bumpver",
     "diskcache",
     "humanize",
     "invoke",
     "invoke",
     "logzero",
     "numpy",
@@ -62,15 +62,15 @@
 line-length = 120
 
 [tool.ruff]
 line-length = 120
 target-version = "py310"
 
 [tool.bumpver]
-current_version = "2.2.0"
+current_version = "2.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `supersullytools-2.2.0/src/streamlit_app/pages/AI Chat.py` & `supersullytools-2.3.0/src/streamlit_app/pages/AI Chat.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.2.0/src/streamlit_app/pages/Item Paginator.py` & `supersullytools-2.3.0/src/streamlit_app/pages/Item Paginator.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.2.0/src/supersullytools/openai/chat_session.py` & `supersullytools-2.3.0/src/supersullytools/openai/chat_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     def to_chat_function(cls) -> Function:
         return Function(name=cls.__name__, description=cls.__doc__, parameters=cls.model_json_schema())
 
 
 _T = TypeVar("_T", bound=ChatTool)
 
 
+# NOTE: this is now "legacy" and I'm using the supersullytools.llm.completions CompletionHandler class now
+
+
 @dataclass
 class ChatSession:
     initial_system_message: Optional[str] = None
     reinforcement_system_msg: Optional[str] = None
     default_tools: list[Type[_T]] = None
     history: list = field(default_factory=list)
     log: Logger = None
```

### Comparing `supersullytools-2.2.0/src/supersullytools/streamlit/misc.py` & `supersullytools-2.3.0/src/supersullytools/streamlit/misc.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.2.0/src/supersullytools/streamlit/paginator.py` & `supersullytools-2.3.0/src/supersullytools/streamlit/paginator.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.2.0/src/supersullytools/streamlit/sessions.py` & `supersullytools-2.3.0/src/supersullytools/streamlit/sessions.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.2.0/src/supersullytools/utils/misc.py` & `supersullytools-2.3.0/src/supersullytools/utils/misc.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.2.0/src/supersullytools.egg-info/PKG-INFO` & `supersullytools-2.3.0/src/supersullytools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supersullytools
-Version: 2.2.0
+Version: 2.3.0
 Summary: This is a Python package that brings together a suite of utilities and helpers across several domains of software development.
 Author-email: Sully <sully@sadburger.com>
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: boto3; extra == "dev"
 Requires-Dist: black; extra == "dev"
-Requires-Dist: boto3-stubs[dynamodb]; extra == "dev"
+Requires-Dist: boto3-stubs[bedrock-runtime,dynamodb]; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: diskcache; extra == "dev"
 Requires-Dist: humanize; extra == "dev"
 Requires-Dist: invoke; extra == "dev"
 Requires-Dist: invoke; extra == "dev"
 Requires-Dist: logzero; extra == "dev"
 Requires-Dist: numpy; extra == "dev"
@@ -49,11 +49,11 @@
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
 
 SuperSully Tools
 ================
 
-**Latest Version:** 2.2.0
+**Latest Version:** 2.3.0
 
 **SupersullyTools** is a Python package that brings together a suite of utilities and helpers across several domains of
 software development. My personal toolkit of things I want in every package I'm working on, compiled in one place.
```

### Comparing `supersullytools-2.2.0/src/supersullytools.egg-info/SOURCES.txt` & `supersullytools-2.3.0/src/supersullytools.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 src/streamlit_app/pages/Item Paginator.py
 src/supersullytools/__init__.py
 src/supersullytools.egg-info/PKG-INFO
 src/supersullytools.egg-info/SOURCES.txt
 src/supersullytools.egg-info/dependency_links.txt
 src/supersullytools.egg-info/requires.txt
 src/supersullytools.egg-info/top_level.txt
+src/supersullytools/llm/__init__.py
+src/supersullytools/llm/completions.py
 src/supersullytools/openai/__init__.py
 src/supersullytools/openai/chat_session.py
 src/supersullytools/streamlit/__init__.py
 src/supersullytools/streamlit/misc.py
 src/supersullytools/streamlit/paginator.py
 src/supersullytools/streamlit/sessions.py
 src/supersullytools/utils/__init__.py
```

### Comparing `supersullytools-2.2.0/src/tests/conftest.py` & `supersullytools-2.3.0/src/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from typing import TYPE_CHECKING
 from uuid import uuid4
 
 import boto3
 import pytest
 import requests
 from logzero import logger
-from simplesingletable import DynamoDBMemory
+from simplesingletable import DynamoDbMemory
 from simplesingletable.utils import truncate_dynamo_table
 
 if TYPE_CHECKING:
     from mypy_boto3_dynamodb.service_resource import Table
 
 
 @pytest.fixture()
-def dynamodb_memory(local_dynamodb_test_table, dynamodb_via_docker) -> DynamoDBMemory:
+def dynamodb_memory(local_dynamodb_test_table, dynamodb_via_docker) -> DynamoDbMemory:
     reset_local_dynamodb_test_table(local_dynamodb_test_table)
-    yield DynamoDBMemory(
+    yield DynamoDbMemory(
         logger=logger,
         table_name=local_dynamodb_test_table.table_name,
         endpoint_url=dynamodb_via_docker,
         connection_params={
             "aws_access_key_id": "unused",
             "aws_secret_access_key": "unused",
             "region_name": "us-west-2",
```

### Comparing `supersullytools-2.2.0/src/tests/test_streamlit_session.py` & `supersullytools-2.3.0/src/tests/test_streamlit_session.py`

 * *Files identical despite different names*

