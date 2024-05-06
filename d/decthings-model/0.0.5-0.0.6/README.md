# Comparing `tmp/decthings_model-0.0.5.tar.gz` & `tmp/decthings_model-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decthings_model-0.0.5.tar", last modified: Wed Apr 24 11:50:33 2024, max compression
+gzip compressed data, was "decthings_model-0.0.6.tar", last modified: Mon May  6 13:05:40 2024, max compression
```

## Comparing `decthings_model-0.0.5.tar` & `decthings_model-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-24 11:50:33.063412 decthings_model-0.0.5/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1066 2024-04-16 09:05:15.000000 decthings_model-0.0.5/LICENSE
--rw-r--r--   0 viktor    (1000) viktor    (1000)     1464 2024-04-24 11:50:33.063412 decthings_model-0.0.5/PKG-INFO
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1029 2024-04-18 15:37:50.000000 decthings_model-0.0.5/README.md
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      421 2024-04-24 11:50:09.000000 decthings_model-0.0.5/pyproject.toml
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       38 2024-04-24 11:50:33.063412 decthings_model-0.0.5/setup.cfg
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-24 11:50:33.063412 decthings_model-0.0.5/src/
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-24 11:50:33.063412 decthings_model-0.0.5/src/decthings_model/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      133 2024-04-24 11:43:09.000000 decthings_model-0.0.5/src/decthings_model/__init__.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       34 2024-04-16 09:05:15.000000 decthings_model-0.0.5/src/decthings_model/__main__.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    11287 2024-04-24 11:49:25.000000 decthings_model-0.0.5/src/decthings_model/model.py
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-24 11:50:33.063412 decthings_model-0.0.5/src/decthings_model/run/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     6642 2024-04-16 09:05:15.000000 decthings_model-0.0.5/src/decthings_model/run/dataloader.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    14621 2024-04-16 09:05:15.000000 decthings_model-0.0.5/src/decthings_model/run/run.py
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-04-24 11:50:33.063412 decthings_model-0.0.5/src/decthings_model.egg-info/
--rw-r--r--   0 viktor    (1000) viktor    (1000)     1464 2024-04-24 11:50:33.000000 decthings_model-0.0.5/src/decthings_model.egg-info/PKG-INFO
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      408 2024-04-24 11:50:33.000000 decthings_model-0.0.5/src/decthings_model.egg-info/SOURCES.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2024-04-24 11:50:33.000000 decthings_model-0.0.5/src/decthings_model.egg-info/dependency_links.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       21 2024-04-24 11:50:33.000000 decthings_model-0.0.5/src/decthings_model.egg-info/requires.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       16 2024-04-24 11:50:33.000000 decthings_model-0.0.5/src/decthings_model.egg-info/top_level.txt
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-05-06 13:05:40.977512 decthings_model-0.0.6/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1066 2024-04-16 09:05:15.000000 decthings_model-0.0.6/LICENSE
+-rw-r--r--   0 viktor    (1000) viktor    (1000)     1464 2024-05-06 13:05:40.977512 decthings_model-0.0.6/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1029 2024-04-18 15:37:50.000000 decthings_model-0.0.6/README.md
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      421 2024-05-06 13:05:12.000000 decthings_model-0.0.6/pyproject.toml
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       38 2024-05-06 13:05:40.977512 decthings_model-0.0.6/setup.cfg
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-05-06 13:05:40.973511 decthings_model-0.0.6/src/
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-05-06 13:05:40.973511 decthings_model-0.0.6/src/decthings_model/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      133 2024-04-24 11:43:09.000000 decthings_model-0.0.6/src/decthings_model/__init__.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       34 2024-04-16 09:05:15.000000 decthings_model-0.0.6/src/decthings_model/__main__.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    11618 2024-05-06 12:33:51.000000 decthings_model-0.0.6/src/decthings_model/model.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-05-06 13:05:40.977512 decthings_model-0.0.6/src/decthings_model/run/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     6642 2024-04-16 09:05:15.000000 decthings_model-0.0.6/src/decthings_model/run/dataloader.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    15606 2024-05-06 12:33:42.000000 decthings_model-0.0.6/src/decthings_model/run/run.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-05-06 13:05:40.977512 decthings_model-0.0.6/src/decthings_model.egg-info/
+-rw-r--r--   0 viktor    (1000) viktor    (1000)     1464 2024-05-06 13:05:40.000000 decthings_model-0.0.6/src/decthings_model.egg-info/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      408 2024-05-06 13:05:40.000000 decthings_model-0.0.6/src/decthings_model.egg-info/SOURCES.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2024-05-06 13:05:40.000000 decthings_model-0.0.6/src/decthings_model.egg-info/dependency_links.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       21 2024-05-06 13:05:40.000000 decthings_model-0.0.6/src/decthings_model.egg-info/requires.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       16 2024-05-06 13:05:40.000000 decthings_model-0.0.6/src/decthings_model.egg-info/top_level.txt
```

### Comparing `decthings_model-0.0.5/LICENSE` & `decthings_model-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `decthings_model-0.0.5/PKG-INFO` & `decthings_model-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decthings-model
-Version: 0.0.5
+Version: 0.0.6
 Summary: Create a Decthings model using Python
 Project-URL: Homepage, https://github.com/decthings/model-py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `decthings_model-0.0.5/README.md` & `decthings_model-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `decthings_model-0.0.5/src/decthings_model/model.py` & `decthings_model-0.0.6/src/decthings_model/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -110,74 +110,82 @@
     def _create_data_loader_map(params: dict[str, DataLoaderBinary]) -> DataLoaderMap:
         new_params = {}
         for k in params.keys():
             new_params[k] = DataLoader(params[k])
         return new_params
 
     @staticmethod
-    def createModelState(executor, params, provider):
-        dataloader = _Model._create_data_loader_map(params)
+    def createModelState(executor, options):
+        class CreateModelStateOptions:
+            def __init__(self):
+                self.params = _Model._create_data_loader_map(options.params)
+                self.state_provider = options.state_provider
+                self.other_models = options.other_models
+
         if isinstance(executor, dict):
             if "createModelState" not in executor:
                 raise ValueError('The function "createModelState" was missing from the executor.')
             if not callable(executor["createModelState"]):
                 raise ValueError(f'The property "createModelState" on the executor was not a function - got {str(type(executor["createModelState"]))}.')
-            return executor["createModelState"](dataloader, provider)
+            return executor["createModelState"](CreateModelStateOptions())
         else:
             fn = getattr(executor, "createModelState", None)
             if fn is None:
                 raise ValueError('The function "createModelState" was missing from the executor.')
             if not callable(fn):
                 raise ValueError(f'The property "createModelState" on the executor was not a function - got {str(type(fn))}.')
-            return executor.createModelState(dataloader, provider)
+            return executor.createModelState(CreateModelStateOptions())
 
     @staticmethod
-    async def instantiateModel(executor, model_state: bytes):
+    async def instantiateModel(executor, options):
         if isinstance(executor, dict):
             if "instantiateModel" not in executor:
                 raise ValueError('The function "instantiateModel" was missing from the executor.')
             if not callable(executor["instantiateModel"]):
                 raise ValueError(f'The property "instantiateModel" on the executor was not a function - got {str(type(executor["instantiateModel"]))}.')
-            instantiated = executor["instantiateModel"](model_state)
+            instantiated = executor["instantiateModel"](options)
         else:
             fn = getattr(executor, "instantiateModel", None)
             if fn is None:
                 raise ValueError('The function "instantiateModel" was missing from the executor.')
             if not callable(fn):
                 raise ValueError(f'The property "instantiateModel" on the executor was not a function - got {str(type(fn))}.')
-            instantiated = executor.instantiateModel(model_state)
+            instantiated = executor.instantiateModel(options)
 
         if inspect.isawaitable(instantiated):
             awaitedinstantiated = await instantiated
         else:
             awaitedinstantiated = instantiated
 
         return {
-            "evaluate": lambda params: _Model.evaluate(awaitedinstantiated, params),
+            "evaluate": lambda options: _Model.evaluate(awaitedinstantiated, options),
             "dispose": lambda: _Model.dispose(awaitedinstantiated),
-            "getModelState": lambda provider: _Model.getModelState(awaitedinstantiated, provider),
-            "train": lambda tracker, params: _Model.train(awaitedinstantiated, tracker, params)
+            "getModelState": lambda options: _Model.getModelState(awaitedinstantiated, options),
+            "train": lambda options: _Model.train(awaitedinstantiated, options)
         }
 
     @staticmethod
-    async def evaluate(awaitedinstantiated, params):
-        dataloader = _Model._create_data_loader_map(params)
+    async def evaluate(awaitedinstantiated, options):
+        class EvaluateOptions:
+            def __init__(self):
+                self.params = _Model._create_data_loader_map(options.params)
+
         if isinstance(awaitedinstantiated, dict):
             if "evaluate" not in awaitedinstantiated:
                 raise ValueError('The function "evaluate" was missing from the instantiated model.')
             if not callable(awaitedinstantiated["evaluate"]):
                 raise ValueError(f'The property "evaluate" on the instantiated model was not a function - got {str(type(awaitedinstantiated["evaluate"]))}.')
-            res = awaitedinstantiated['evaluate'](dataloader)
+            res = awaitedinstantiated['evaluate'](EvaluateOptions())
         else:
             fn = getattr(awaitedinstantiated, "evaluate", None)
             if fn is None:
                 raise ValueError('The function "evaluate" was missing from the model.')
             if not callable(fn):
                 raise ValueError(f'The property "evaluate" on the model was not a function - got {str(type(fn))}.')
-            res = awaitedinstantiated.evaluate(dataloader)
+            res = awaitedinstantiated.evaluate(EvaluateOptions())
 
         if inspect.isawaitable(res):
             awaitedres = await res
         else:
             awaitedres = res
 
         if not isinstance(awaitedres, list):
@@ -214,45 +222,49 @@
             if fn is None:
                 return
             if not callable(fn):
                 raise ValueError(f'The property "dispose" on the instantiated model was not a function - got {str(type(fn))}.')
             return awaitedinstantiated.dispose()
 
     @staticmethod
-    def getModelState(awaitedinstantiated, provider):
+    def getModelState(awaitedinstantiated, options):
         if isinstance(awaitedinstantiated, dict):
             if "getModelState" not in awaitedinstantiated:
                 raise ValueError('The function "getModelState" was missing from the instantiated model.')
             if not callable(awaitedinstantiated["getModelState"]):
                 raise ValueError(f'The property "getModelState" on the instantiated model was not a function - got {str(type(awaitedinstantiated["getModelState"]))}.')
-            return awaitedinstantiated["getModelState"](provider)
+            return awaitedinstantiated["getModelState"](options)
         else:
             fn = getattr(awaitedinstantiated, "getModelState", None)
             if fn is None:
                 raise ValueError('The function "getModelState" was missing from the instantiated model.')
             if not callable(fn):
                 raise ValueError(f'The property "getModelState" on the model was not a function - got {str(type(fn))}.')
-            return awaitedinstantiated.getModelState(provider)
+            return awaitedinstantiated.getModelState(options)
 
     @staticmethod
-    def train(awaitedinstantiated, params, tracker):
-        dataloader = _Model._create_data_loader_map(params)
+    def train(awaitedinstantiated, options):
+        class TrainOptions:
+            def __init__(self):
+                self.params = _Model._create_data_loader_map(options.params)
+                self.tracker = TrainTracker(options.tracker)
+
         if isinstance(awaitedinstantiated, dict):
             if "train" not in awaitedinstantiated:
                 raise ValueError('The function "train" was missing from the instantiated model.')
             if not callable(awaitedinstantiated["train"]):
                 raise ValueError(f'The property "train" on the instantiated model was not a function - got {str(type(awaitedinstantiated["train"]))}.')
-            return awaitedinstantiated["train"](dataloader, TrainTracker(tracker))
+            return awaitedinstantiated["train"](TrainOptions())
         else:
             fn = getattr(awaitedinstantiated, "train", None)
             if fn is None:
                 raise ValueError('The function "train" was missing from the instantiated model.')
             if not callable(fn):
                 raise ValueError(f'The property "train" on the instantiated model was not a function - got {str(type(fn))}.')
-            return awaitedinstantiated.train(dataloader, TrainTracker(tracker))
+            return awaitedinstantiated.train(TrainOptions)
 
 
 def make_model(executor) -> dict:
     return {
-        "createModelState": lambda params, provider: _Model.createModelState(executor, params, provider),
-        "instantiateModel": lambda model_state: _Model.instantiateModel(executor, model_state)
+        "createModelState": lambda options: _Model.createModelState(executor, options),
+        "instantiateModel": lambda options: _Model.instantiateModel(executor, options)
     }
```

### Comparing `decthings_model-0.0.5/src/decthings_model/run/dataloader.py` & `decthings_model-0.0.6/src/decthings_model/run/dataloader.py`

 * *Files identical despite different names*

### Comparing `decthings_model-0.0.5/src/decthings_model/run/run.py` & `decthings_model-0.0.6/src/decthings_model/run/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,36 +70,48 @@
         global runningProgram
         runningProgram = _module.model
     except:
         sendEventToParent("modelSessionInitialized", { "error": getErrorFromException() }, [])
         return
     sendEventToParent("modelSessionInitialized", {}, [])
 
+class OtherModelWithState:
+    def __init__(self, mount_path, state):
+        self.mount_path = mount_path
+        self.state = state
+
 async def callCreateModelState(args):
     complete = { "complete": False }
-    map = createDataLoaderMap(complete, args["params"], sendDataEventToParent)
-    provider = createStateProvider(complete, args["id"], sendEventToParent)
-    other_model_states = {}
-    for other_model_state in args["otherModelStates"]:
-        other_model_states[other_model_state["id"]] = createStateLoaderMap(complete, other_model_state["state"], sendDataEventToParent)
+    class CreateModelStateOptions:
+        def __init__(self):
+            self.params = createDataLoaderMap(complete, args["params"], sendDataEventToParent)
+            self.state_provider = createStateProvider(complete, args["id"], sendEventToParent)
+            self.other_models = {}
+            for other_model in args["otherModels"]:
+                self.other_models[other_model["id"]] = OtherModelWithState(other_model["mountPath"], createStateLoaderMap(complete, other_model["state"], sendDataEventToParent))
+
     try:
         if isinstance(runningProgram, dict):
-            res = runningProgram["createModelState"](map, provider)
+            res = runningProgram["createModelState"](CreateModelStateOptions())
         else:
-            res = runningProgram.createModelState(map, provider)
+            res = runningProgram.createModelState(CreateModelStateOptions())
 
         if inspect.isawaitable(res):
             await res
         
         complete["complete"] = True
         return { "result": {} }
     except:
         complete["complete"] = True
         return { "result": { "error": getErrorFromException() } }
 
+class OtherModel:
+    def __init__(self, mount_path):
+        self.mount_path = mount_path
+
 async def callInstantiateModel(args):
     disposed = False
 
     modelFuture = asyncio.get_event_loop().create_future()
 
     def dispose():
         nonlocal disposed
@@ -111,21 +123,26 @@
         "model": modelFuture,
         "dispose": dispose
     }
 
     instantiatedModels[args["instantiatedModelId"]] = stored
 
     complete = { "complete": False }
-    stateLoaders = createStateLoaderMap(complete, args["state"], sendDataEventToParent)
+    class InstantiateModelOptions:
+        def __init__(self):
+            self.state = createStateLoaderMap(complete, args["state"], sendDataEventToParent)
+            self.other_models = {}
+            for other_model in args["otherModels"]:
+                self.other_models[other_model["id"]] = OtherModel(other_model["mountPath"])
 
     try:
         if isinstance(runningProgram, dict):
-            res = runningProgram["instantiateModel"](stateLoaders)
+            res = runningProgram["instantiateModel"](InstantiateModelOptions())
         else:
-            res = runningProgram.instantiateModel(stateLoaders)
+            res = runningProgram.instantiateModel(InstantiateModelOptions())
 
         if inspect.isawaitable(res):
             awaitedres = await res
         else:
             awaitedres = res
         complete["complete"] = True
     except:
@@ -152,35 +169,39 @@
 def callDisposeInstantiatedModel(args):
     if args["instantiatedModelId"] in instantiatedModels:
         instantiatedModel = instantiatedModels[args["instantiatedModelId"]]
         del instantiatedModels[args["instantiatedModelId"]]
         instantiatedModel["dispose"]
 
 async def callTrain(args):
-    tracker = TrainTracker(args["trainingSessionId"])
-    trainingSessions[args["trainingSessionId"]] = tracker
-
     if not args["instantiatedModelId"] in instantiatedModels:
         return { "result": { "error": "instantiated_model_not_found" } }
 
+    tracker = TrainTracker(args["trainingSessionId"])
+    trainingSessions[args["trainingSessionId"]] = tracker
+
     instantiatedModel = instantiatedModels[args["instantiatedModelId"]]
     if inspect.isawaitable(instantiatedModel["model"]):
         model = await instantiatedModel["model"]
         if model == None:
             return { "result": { "error": "instantiated_model_not_found" } }
     else:
         model = instantiatedModel["model"]
 
     complete = { "complete": False }
-    map = createDataLoaderMap(complete, args["params"], sendDataEventToParent)
+    class TrainOptions:
+        def __init__(self):
+            self.params = createDataLoaderMap(complete, args["params"], sendDataEventToParent)
+            self.tracker = tracker
+
     try:
         if isinstance(model, dict):
-            res = model["train"](map, tracker)
+            res = model["train"](TrainOptions())
         else:
-            res = model.train(map, tracker)
+            res = model.train(TrainOptions())
 
         if inspect.isawaitable(res):
             await res
         
         tracker._complete = True
         complete["complete"] = True
     except:
@@ -206,20 +227,23 @@
     if inspect.isawaitable(instantiatedModel["model"]):
         model = await instantiatedModel["model"]
         if model == None:
             return { "result": { "error": "instantiated_model_not_found" } }
     else:
         model = instantiatedModel["model"]
     complete = { "complete": False }
-    map = createDataLoaderMap(complete, args["params"], sendDataEventToParent)
+    class EvaluateOptions:
+        def __init__(self):
+            self.params = createDataLoaderMap(complete, args["params"], sendDataEventToParent)
+
     try:
         if isinstance(model, dict):
-            res = model["evaluate"](map)
+            res = model["evaluate"](EvaluateOptions())
         else:
-            res = model.evaluate(map)
+            res = model.evaluate(EvaluateOptions())
 
         if inspect.isawaitable(res):
             awaitedres = await res
         else:
             awaitedres = res
         
         complete["complete"] = True
@@ -255,21 +279,23 @@
         model = await instantiatedModel["model"]
         if model == None:
             return { "result": { "error": "instantiated_model_not_found" } }
     else:
         model = instantiatedModel["model"]
     
     complete = { "complete": False }
-    provider = createStateProvider(complete, args["id"], sendEventToParent)
+    class GetModelStateOptions:
+        def __init__(self):
+            self.state_provider = createStateProvider(complete, args["id"], sendEventToParent)
 
     try:
         if isinstance(model, dict):
-            res = model["getModelState"](provider)
+            res = model["getModelState"](GetModelStateOptions())
         else:
-            res = model.getModelState(provider)
+            res = model.getModelState(GetModelStateOptions())
 
         if inspect.isawaitable(res):
             await res
         
         complete["complete"] = True
     except:
         complete["complete"] = True
```

### Comparing `decthings_model-0.0.5/src/decthings_model.egg-info/PKG-INFO` & `decthings_model-0.0.6/src/decthings_model.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decthings-model
-Version: 0.0.5
+Version: 0.0.6
 Summary: Create a Decthings model using Python
 Project-URL: Homepage, https://github.com/decthings/model-py
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

