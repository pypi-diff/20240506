# Comparing `tmp/literalai-0.0.509.tar.gz` & `tmp/literalai-0.0.600.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "literalai-0.0.509.tar", last modified: Tue Apr 30 07:46:34 2024, max compression
+gzip compressed data, was "literalai-0.0.600.tar", last modified: Mon May  6 12:55:47 2024, max compression
```

## Comparing `literalai-0.0.509.tar` & `literalai-0.0.600.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:46:34.222523 literalai-0.0.509/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 07:46:26.000000 literalai-0.0.509/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-30 07:46:34.222523 literalai-0.0.509/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-30 07:46:26.000000 literalai-0.0.509/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:46:34.218523 literalai-0.0.509/literalai/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:46:34.222523 literalai-0.0.509/literalai/api/
--rw-r--r--   0 runner    (1001) docker     (127)    82368 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/api/attachment_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/api/dataset_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/api/generation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20230 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/api/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/api/prompt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/api/score_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/api/step_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/api/thread_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/api/user_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:46:34.222523 literalai-0.0.509/literalai/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17193 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/callback/langchain_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/callback/llama_index_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/dataset_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/event_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:46:34.222523 literalai-0.0.509/literalai/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18450 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/instrumentation/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12197 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/my_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-30 07:46:26.000000 literalai-0.0.509/literalai/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:46:34.218523 literalai-0.0.509/literalai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-30 07:46:33.000000 literalai-0.0.509/literalai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-30 07:46:34.000000 literalai-0.0.509/literalai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:46:33.000000 literalai-0.0.509/literalai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-30 07:46:33.000000 literalai-0.0.509/literalai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 07:46:33.000000 literalai-0.0.509/literalai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 07:46:34.222523 literalai-0.0.509/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-30 07:46:26.000000 literalai-0.0.509/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:46:34.222523 literalai-0.0.509/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:46:26.000000 literalai-0.0.509/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:47.387939 literalai-0.0.600/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 12:55:36.000000 literalai-0.0.600/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-06 12:55:47.387939 literalai-0.0.600/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-06 12:55:36.000000 literalai-0.0.600/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:47.383939 literalai-0.0.600/literalai/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:47.387939 literalai-0.0.600/literalai/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    81961 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/attachment_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/dataset_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/generation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20229 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/prompt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/score_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/step_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/thread_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/user_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:47.387939 literalai-0.0.600/literalai/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17193 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/callback/langchain_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/callback/llama_index_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/dataset_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:47.387939 literalai-0.0.600/literalai/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18454 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/instrumentation/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/my_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:47.387939 literalai-0.0.600/literalai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-06 12:55:47.000000 literalai-0.0.600/literalai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-06 12:55:47.000000 literalai-0.0.600/literalai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 12:55:47.000000 literalai-0.0.600/literalai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-06 12:55:47.000000 literalai-0.0.600/literalai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 12:55:47.000000 literalai-0.0.600/literalai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 12:55:47.387939 literalai-0.0.600/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-06 12:55:36.000000 literalai-0.0.600/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:47.387939 literalai-0.0.600/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:36.000000 literalai-0.0.600/tests/__init__.py
```

### Comparing `literalai-0.0.509/LICENSE` & `literalai-0.0.600/LICENSE`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/README.md` & `literalai-0.0.600/README.md`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/api/__init__.py` & `literalai-0.0.600/literalai/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2167,31 +2167,21 @@
     async def create_experiment(
         self,
         dataset_id: str,
         name: str,
         prompt_id: Optional[str] = None,
         params: Optional[Dict] = None,
     ) -> "DatasetExperiment":
-        """
-        Asynchronously creates an experiment within a dataset.
-
-        Args:
-            dataset_id (str): The unique identifier of the dataset.
-            name (str): The name of the experiment.
-            prompt_id (Optional[str]): The identifier of the prompt associated with the experiment.
-            params (Optional[Dict]): Additional parameters for the experiment.
-
-        Returns:
-            DatasetExperiment: The created experiment object.
-        """
         sync_api = LiteralAPI(self.api_key, self.url)
 
         return await self.gql_helper(
             *create_experiment_helper(sync_api, dataset_id, name, prompt_id, params)
         )
+    
+    create_experiment.__doc__ = LiteralAPI.create_experiment.__doc__
 
     async def create_experiment_item(
         self, experiment_item: DatasetExperimentItem
     ) -> DatasetExperimentItem:
         """
         Asynchronously creates an item within an experiment.
```

### Comparing `literalai-0.0.509/literalai/api/attachment_helpers.py` & `literalai-0.0.600/literalai/api/attachment_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/api/dataset_helpers.py` & `literalai-0.0.600/literalai/api/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/api/generation_helpers.py` & `literalai-0.0.600/literalai/api/generation_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/api/gql.py` & `literalai-0.0.600/literalai/api/gql.py`

 * *Files 0% similar despite different names*

```diff
@@ -794,15 +794,15 @@
 """
 
 CREATE_EXPERIMENT = """
     mutation CreateDatasetExperiment(
         $name: String! 
         $datasetId: String!
         $promptId: String
-        $params: Json!
+        $params: Json
     ) {
         createDatasetExperiment(
             name: $name
             datasetId: $datasetId
             promptId: $promptId
             params: $params
         ) {
```

### Comparing `literalai-0.0.509/literalai/api/prompt_helpers.py` & `literalai-0.0.600/literalai/api/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/api/score_helpers.py` & `literalai-0.0.600/literalai/api/score_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/api/step_helpers.py` & `literalai-0.0.600/literalai/api/step_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/api/thread_helpers.py` & `literalai-0.0.600/literalai/api/thread_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/api/user_helpers.py` & `literalai-0.0.600/literalai/api/user_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/callback/langchain_callback.py` & `literalai-0.0.600/literalai/callback/langchain_callback.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/callback/llama_index_callback.py` & `literalai-0.0.600/literalai/callback/llama_index_callback.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/client.py` & `literalai-0.0.600/literalai/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 class BaseLiteralClient:
     api: Union[LiteralAPI, AsyncLiteralAPI]
 
     def __init__(
         self,
-        batch_size: int = 1,
+        batch_size: int = 5,
         is_async: bool = False,
         api_key: Optional[str] = None,
         url: Optional[str] = None,
         disabled: bool = False,
     ):
         if not api_key:
             api_key = os.getenv("LITERAL_API_KEY", None)
@@ -216,15 +216,15 @@
 
 
 class LiteralClient(BaseLiteralClient):
     api: LiteralAPI
 
     def __init__(
         self,
-        batch_size: int = 1,
+        batch_size: int = 5,
         api_key: Optional[str] = None,
         url: Optional[str] = None,
         disabled: bool = False,
     ):
         super().__init__(
             batch_size=batch_size,
             is_async=False,
@@ -238,15 +238,15 @@
 
 
 class AsyncLiteralClient(BaseLiteralClient):
     api: AsyncLiteralAPI
 
     def __init__(
         self,
-        batch_size: int = 1,
+        batch_size: int = 5,
         api_key: Optional[str] = None,
         url: Optional[str] = None,
         disabled: bool = False,
     ):
         super().__init__(
             batch_size=batch_size,
             is_async=True,
```

### Comparing `literalai-0.0.509/literalai/dataset.py` & `literalai-0.0.600/literalai/dataset.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/dataset_experiment.py` & `literalai-0.0.600/literalai/dataset_experiment.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/dataset_item.py` & `literalai-0.0.600/literalai/dataset_item.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/event_processor.py` & `literalai-0.0.600/literalai/event_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     func_call = functools.partial(ctx.run, func, *args, **kwargs)
     return await loop.run_in_executor(None, func_call)
 
 
 class EventProcessor:
     event_queue: queue.Queue
 
-    def __init__(self, api: "LiteralAPI", batch_size: int = 1, disabled: bool = False):
+    def __init__(self, api: "LiteralAPI", batch_size: int = 5, disabled: bool = False):
         self.batch_size = batch_size
         self.api = api
         self.event_queue = queue.Queue()
         self.processing_thread = threading.Thread(
             target=self._process_events, daemon=True
         )
         self.disabled = disabled
```

### Comparing `literalai-0.0.509/literalai/filter.py` & `literalai-0.0.600/literalai/filter.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/helper.py` & `literalai-0.0.600/literalai/helper.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/instrumentation/openai.py` & `literalai-0.0.600/literalai/instrumentation/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                 prompt_id=prompt_id,
                 variables=variables,
                 provider="openai",
                 model=model,
                 tools=tools,
                 settings=settings,
                 messages=messages,
-                tags=kwargs.get("literal_tags"),
+                tags=kwargs.get("literalai_tags"),
             )
 
         elif generation_type == GenerationType.COMPLETION:
             settings = {
                 "model": model,
                 "best_of": kwargs.get("best_of"),
                 "echo": kwargs.get("echo"),
@@ -153,15 +153,15 @@
             }
             settings = {k: v for k, v in settings.items() if v is not None}
             return CompletionGeneration(
                 provider="openai",
                 model=model,
                 settings=settings,
                 prompt=kwargs.get("prompt"),
-                tags=kwargs.get("literal_tags"),
+                tags=kwargs.get("literalai_tags"),
             )
 
     def update_step_after(
         generation: Union[ChatGeneration, CompletionGeneration], result
     ):
         if generation and isinstance(generation, ChatGeneration):
             generation.message_completion = result.choices[0].message.model_dump()
```

### Comparing `literalai-0.0.509/literalai/message.py` & `literalai-0.0.600/literalai/message.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/my_types.py` & `literalai-0.0.600/literalai/my_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 class TextContent(TypedDict, total=False):
     type: Literal["text"]
     text: str
 
 
 class ImageUrlContent(TypedDict, total=False):
     type: Literal["image_url"]
-    image_url: str
+    image_url: Dict
 
 
 class GenerationMessage(TypedDict, total=False):
     uuid: Optional[str]
     templated: Optional[bool]
     name: Optional[str]
     role: Optional[GenerationMessageRole]
```

### Comparing `literalai-0.0.509/literalai/prompt.py` & `literalai-0.0.600/literalai/prompt.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/requirements.py` & `literalai-0.0.600/literalai/requirements.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/step.py` & `literalai-0.0.600/literalai/step.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/thread.py` & `literalai-0.0.600/literalai/thread.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.509/literalai/wrappers.py` & `literalai-0.0.600/literalai/wrappers.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,53 +19,53 @@
 class AfterContext(TypedDict):
     original_func: Callable
     generation: Optional[Union["ChatGeneration", "CompletionGeneration"]]
     step: Optional["Step"]
     start: float
 
 
-def remove_literal_args(kargs):
-    '''Remove argument prefixed with "literal_" from kwargs and return them in a separate dict'''
+def remove_literalai_args(kargs):
+    '''Remove argument prefixed with "literalai_" from kwargs and return them in a separate dict'''
     largs = {}
     for key in list(kargs.keys()):
-        if key.startswith("literal_"):
+        if key.startswith("literalai_"):
             value = kargs.pop(key)
             largs[key] = value
     return largs
 
-def restore_literal_args(kargs, largs):
-    '''Reverse the effect of remove_literal_args by merging the literal arguments into kwargs'''
+def restore_literalai_args(kargs, largs):
+    '''Reverse the effect of remove_literalai_args by merging the literal arguments into kwargs'''
     for key in list(largs.keys()):
         kargs[key] = largs[key]
 
 
 def sync_wrapper(before_func=None, after_func=None):
     def decorator(original_func):
         @wraps(original_func)
         def wrapped(*args, **kwargs):
             context = {"original_func": original_func}
             # If a before_func is provided, call it with the shared context.
             if before_func:
                 before_func(context, *args, **kwargs)
             # Remove literal arguments before calling the original function
-            literal_args = remove_literal_args(kwargs)
+            literalai_args = remove_literalai_args(kwargs)
             context["start"] = time.time()
             try:
                 result = original_func(*args, **kwargs)
             except Exception as e:
                 active_steps = active_steps_var.get()
                 if active_steps and len(active_steps) > 0:
                     current_step = active_steps[-1]
                     current_step.error = str(e)
                     current_step.end()
                     current_step.processor.flush()
                 raise e
             # If an after_func is provided, call it with the result and the shared context.
             if after_func:
-                restore_literal_args(kwargs, literal_args)
+                restore_literalai_args(kwargs, literalai_args)
                 result = after_func(result, context, *args, **kwargs)
 
             return result
 
         return wrapped
 
     return decorator
@@ -77,30 +77,30 @@
         async def wrapped(*args, **kwargs):
             context = {"original_func": original_func}
             # If a before_func is provided, call it with the shared context.
             if before_func:
                 await before_func(context, *args, **kwargs)
 
             # Remove literal arguments before calling the original function
-            literal_args = remove_literal_args(kwargs)
+            literalai_args = remove_literalai_args(kwargs)
             context["start"] = time.time()
             try:
                 result = await original_func(*args, **kwargs)
             except Exception as e:
                 active_steps = active_steps_var.get()
                 if active_steps and len(active_steps) > 0:
                     current_step = active_steps[-1]
                     current_step.error = str(e)
                     current_step.end()
                     current_step.processor.flush()
                 raise e
 
             # If an after_func is provided, call it with the result and the shared context.
             if after_func:
-                restore_literal_args(kwargs, literal_args)
+                restore_literalai_args(kwargs, literalai_args)
                 result = await after_func(result, context, *args, **kwargs)
 
             return result
 
         return wrapped
 
     return decorator
```

### Comparing `literalai-0.0.509/literalai.egg-info/SOURCES.txt` & `literalai-0.0.600/literalai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

