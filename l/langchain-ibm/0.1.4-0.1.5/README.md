# Comparing `tmp/langchain_ibm-0.1.4.tar.gz` & `tmp/langchain_ibm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_ibm-0.1.4.tar", max compression
+gzip compressed data, was "langchain_ibm-0.1.5.tar", max compression
```

## Comparing `langchain_ibm-0.1.4.tar` & `langchain_ibm-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-04-23 17:42:38.235938 langchain_ibm-0.1.4/LICENSE
--rw-r--r--   0        0        0     4395 2024-04-23 17:42:38.235938 langchain_ibm-0.1.4/README.md
--rw-r--r--   0        0        0      144 2024-04-23 17:42:38.235938 langchain_ibm-0.1.4/langchain_ibm/__init__.py
--rw-r--r--   0        0        0     6888 2024-04-23 17:42:38.235938 langchain_ibm-0.1.4/langchain_ibm/embeddings.py
--rw-r--r--   0        0        0    16309 2024-04-23 17:42:38.235938 langchain_ibm-0.1.4/langchain_ibm/llms.py
--rw-r--r--   0        0        0        0 2024-04-23 17:42:38.235938 langchain_ibm-0.1.4/langchain_ibm/py.typed
--rw-r--r--   0        0        0     2559 2024-04-23 17:42:38.235938 langchain_ibm-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 langchain_ibm-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-06 16:59:02.731979 langchain_ibm-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4395 2024-05-06 16:59:02.731979 langchain_ibm-0.1.5/README.md
+-rw-r--r--   0        0        0      144 2024-05-06 16:59:02.731979 langchain_ibm-0.1.5/langchain_ibm/__init__.py
+-rw-r--r--   0        0        0     6694 2024-05-06 16:59:02.731979 langchain_ibm-0.1.5/langchain_ibm/embeddings.py
+-rw-r--r--   0        0        0    16163 2024-05-06 16:59:02.731979 langchain_ibm-0.1.5/langchain_ibm/llms.py
+-rw-r--r--   0        0        0        0 2024-05-06 16:59:02.731979 langchain_ibm-0.1.5/langchain_ibm/py.typed
+-rw-r--r--   0        0        0     2564 2024-05-06 16:59:02.731979 langchain_ibm-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 langchain_ibm-0.1.5/PKG-INFO
```

### Comparing `langchain_ibm-0.1.4/LICENSE` & `langchain_ibm-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_ibm-0.1.4/README.md` & `langchain_ibm-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `langchain_ibm-0.1.4/langchain_ibm/embeddings.py` & `langchain_ibm-0.1.5/langchain_ibm/embeddings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from typing import Dict, List, Optional, Union
 
-from ibm_watsonx_ai import APIClient  # type: ignore
+from ibm_watsonx_ai import APIClient, Credentials  # type: ignore
 from ibm_watsonx_ai.foundation_models.embeddings import Embeddings  # type: ignore
 from langchain_core.embeddings import Embeddings as LangChainEmbeddings
 from langchain_core.pydantic_v1 import (
     BaseModel,
     Extra,
     Field,
     SecretStr,
@@ -125,46 +125,41 @@
                 if not values["instance_id"] or "WATSONX_INSTANCE_ID" not in os.environ:
                     values["instance_id"] = convert_to_secret_str(
                         get_from_dict_or_env(
                             values, "instance_id", "WATSONX_INSTANCE_ID"
                         )
                     )
 
-            credentials = {
-                "url": values["url"].get_secret_value() if values["url"] else None,
-                "apikey": values["apikey"].get_secret_value()
+            credentials = Credentials(
+                url=values["url"].get_secret_value() if values["url"] else None,
+                api_key=values["apikey"].get_secret_value()
                 if values["apikey"]
                 else None,
-                "token": values["token"].get_secret_value()
-                if values["token"]
-                else None,
-                "password": values["password"].get_secret_value()
+                token=values["token"].get_secret_value() if values["token"] else None,
+                password=values["password"].get_secret_value()
                 if values["password"]
                 else None,
-                "username": values["username"].get_secret_value()
+                username=values["username"].get_secret_value()
                 if values["username"]
                 else None,
-                "instance_id": values["instance_id"].get_secret_value()
+                instance_id=values["instance_id"].get_secret_value()
                 if values["instance_id"]
                 else None,
-                "version": values["version"].get_secret_value()
+                version=values["version"].get_secret_value()
                 if values["version"]
                 else None,
-            }
-            credentials_without_none_value = {
-                key: value for key, value in credentials.items() if value is not None
-            }
+                verify=values["verify"],
+            )
 
             watsonx_embed = Embeddings(
                 model_id=values["model_id"],
                 params=values["params"],
-                credentials=credentials_without_none_value,
+                credentials=credentials,
                 project_id=values["project_id"],
                 space_id=values["space_id"],
-                verify=values["verify"],
             )
 
             values["watsonx_embed"] = watsonx_embed
 
         return values
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
```

### Comparing `langchain_ibm-0.1.4/langchain_ibm/llms.py` & `langchain_ibm-0.1.5/langchain_ibm/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import os
 from typing import Any, Dict, Iterator, List, Mapping, Optional, Union
 
+from ibm_watsonx_ai import Credentials  # type: ignore
 from ibm_watsonx_ai.foundation_models import Model, ModelInference  # type: ignore
 from langchain_core.callbacks import CallbackManagerForLLMRun
 from langchain_core.language_models.llms import BaseLLM
 from langchain_core.outputs import Generation, GenerationChunk, LLMResult
 from langchain_core.pydantic_v1 import Extra, Field, SecretStr, root_validator
 from langchain_core.utils import convert_to_secret_str, get_from_dict_or_env
 
@@ -185,48 +186,42 @@
                     )
                 if not values["instance_id"] or "WATSONX_INSTANCE_ID" not in os.environ:
                     values["instance_id"] = convert_to_secret_str(
                         get_from_dict_or_env(
                             values, "instance_id", "WATSONX_INSTANCE_ID"
                         )
                     )
-
-            credentials = {
-                "url": values["url"].get_secret_value() if values["url"] else None,
-                "apikey": values["apikey"].get_secret_value()
+            credentials = Credentials(
+                url=values["url"].get_secret_value() if values["url"] else None,
+                api_key=values["apikey"].get_secret_value()
                 if values["apikey"]
                 else None,
-                "token": values["token"].get_secret_value()
-                if values["token"]
-                else None,
-                "password": values["password"].get_secret_value()
+                token=values["token"].get_secret_value() if values["token"] else None,
+                password=values["password"].get_secret_value()
                 if values["password"]
                 else None,
-                "username": values["username"].get_secret_value()
+                username=values["username"].get_secret_value()
                 if values["username"]
                 else None,
-                "instance_id": values["instance_id"].get_secret_value()
+                instance_id=values["instance_id"].get_secret_value()
                 if values["instance_id"]
                 else None,
-                "version": values["version"].get_secret_value()
+                version=values["version"].get_secret_value()
                 if values["version"]
                 else None,
-            }
-            credentials_without_none_value = {
-                key: value for key, value in credentials.items() if value is not None
-            }
+                verify=values["verify"],
+            )
 
             watsonx_model = ModelInference(
                 model_id=values["model_id"],
                 deployment_id=values["deployment_id"],
-                credentials=credentials_without_none_value,
+                credentials=credentials,
                 params=values["params"],
                 project_id=values["project_id"],
                 space_id=values["space_id"],
-                verify=values["verify"],
             )
             values["watsonx_model"] = watsonx_model
 
         return values
 
     @property
     def _identifying_params(self) -> Mapping[str, Any]:
@@ -329,15 +324,15 @@
             stop: Optional list of stop words to use when generating.
             run_manager: Optional callback manager.
         Returns:
             The string generated by the model.
         Example:
             .. code-block:: python
 
-                response = watsonx_llm("What is a molecule")
+                response = watsonx_llm.invoke("What is a molecule")
         """
         result = self._generate(
             prompts=[prompt], stop=stop, run_manager=run_manager, **kwargs
         )
         return result.generations[0][0].text
 
     def _generate(
```

### Comparing `langchain_ibm-0.1.4/pyproject.toml` & `langchain_ibm-0.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "langchain-ibm"
-version = "0.1.4"
+version = "0.1.5"
 description = "An integration package connecting IBM watsonx.ai and LangChain"
 authors = ["IBM"]
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/ibm"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-langchain-core = "^0.1.42"
-ibm-watsonx-ai = "^0.2.6"
+langchain-core = "^0.1.50"
+ibm-watsonx-ai = "^1.0.1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
@@ -51,15 +51,15 @@
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 langchain-core = { path = "../../core", develop = true }
 
-[tool.ruff]
+[tool.ruff.lint]
 select = [
   "E", # pycodestyle
   "F", # pyflakes
   "I", # isort
 ]
 
 [tool.mypy]
```

### Comparing `langchain_ibm-0.1.4/PKG-INFO` & `langchain_ibm-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-ibm
-Version: 0.1.4
+Version: 0.1.5
 Summary: An integration package connecting IBM watsonx.ai and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Author: IBM
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ibm-watsonx-ai (>=0.2.6,<0.3.0)
-Requires-Dist: langchain-core (>=0.1.42,<0.2.0)
+Requires-Dist: ibm-watsonx-ai (>=1.0.1,<2.0.0)
+Requires-Dist: langchain-core (>=0.1.50,<0.2.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/ibm
 Description-Content-Type: text/markdown
 
 # langchain-ibm
 
 This package provides the integration between LangChain and IBM watsonx.ai through the `ibm-watsonx-ai` SDK.
```

