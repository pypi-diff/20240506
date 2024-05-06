# Comparing `tmp/mlora-0.3.0.post1.tar.gz` & `tmp/mlora-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlora-0.3.0.post1.tar", last modified: Tue Apr 23 06:58:50 2024, max compression
+gzip compressed data, was "mlora-0.3.1.tar", last modified: Mon May  6 09:25:43 2024, max compression
```

## Comparing `mlora-0.3.0.post1.tar` & `mlora-0.3.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-23 06:58:50.768962 mlora-0.3.0.post1/
--rw-r--r--   0 mikecovlee   (501) staff       (20)    11357 2024-01-06 04:20:01.000000 mlora-0.3.0.post1/LICENSE
--rw-r--r--   0 mikecovlee   (501) staff       (20)    11721 2024-04-23 06:58:50.768699 mlora-0.3.0.post1/PKG-INFO
--rw-r--r--   0 mikecovlee   (501) staff       (20)    10954 2024-04-10 06:30:53.000000 mlora-0.3.0.post1/README.md
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-23 06:58:50.759861 mlora-0.3.0.post1/mlora/
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1195 2024-04-23 06:58:34.000000 mlora-0.3.0.post1/mlora/__init__.py
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-23 06:58:50.762415 mlora-0.3.0.post1/mlora/backends/
--rw-r--r--   0 mikecovlee   (501) staff       (20)      987 2024-04-09 13:04:56.000000 mlora-0.3.0.post1/mlora/backends/__init__.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1324 2024-04-09 13:09:12.000000 mlora-0.3.0.post1/mlora/backends/common.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1571 2024-04-09 13:03:52.000000 mlora-0.3.0.post1/mlora/backends/cpu.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1343 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/backends/cuda.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     2044 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/backends/mps.py
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-23 06:58:50.764952 mlora-0.3.0.post1/mlora/common/
--rw-r--r--   0 mikecovlee   (501) staff       (20)     2171 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/common/__init__.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     5197 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/common/attention.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     5040 2024-04-09 12:44:14.000000 mlora-0.3.0.post1/mlora/common/checkpoint.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     2859 2024-04-16 13:15:44.000000 mlora-0.3.0.post1/mlora/common/feed_forward.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    14330 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/common/lora_linear.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    11145 2024-04-16 13:15:44.000000 mlora-0.3.0.post1/mlora/common/mix_lora.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     2266 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/common/model.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     9628 2024-04-16 13:15:44.000000 mlora-0.3.0.post1/mlora/common/modelargs.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    13118 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/dispatcher.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     9770 2024-04-11 14:44:51.000000 mlora-0.3.0.post1/mlora/evaluator.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     7872 2024-04-11 14:44:51.000000 mlora-0.3.0.post1/mlora/generator.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    18206 2024-04-16 13:15:44.000000 mlora-0.3.0.post1/mlora/model.py
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-23 06:58:50.766665 mlora-0.3.0.post1/mlora/models/
--rw-r--r--   0 mikecovlee   (501) staff       (20)      872 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/models/__init__.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     6308 2024-04-09 13:56:23.000000 mlora-0.3.0.post1/mlora/models/modeling_gemma.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    20566 2024-04-09 13:56:23.000000 mlora-0.3.0.post1/mlora/models/modeling_llama.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    12070 2024-04-09 13:56:23.000000 mlora-0.3.0.post1/mlora/models/modeling_mistral.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    22465 2024-04-09 13:56:23.000000 mlora-0.3.0.post1/mlora/models/modeling_phi.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1764 2024-04-03 07:55:06.000000 mlora-0.3.0.post1/mlora/prompter.py
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-23 06:58:50.767847 mlora-0.3.0.post1/mlora/tasks/
--rw-r--r--   0 mikecovlee   (501) staff       (20)      528 2024-04-16 13:15:44.000000 mlora-0.3.0.post1/mlora/tasks/__init__.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     6439 2024-04-11 14:44:51.000000 mlora-0.3.0.post1/mlora/tasks/common.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     3182 2024-04-11 14:44:51.000000 mlora-0.3.0.post1/mlora/tasks/glue_tasks.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     5850 2024-04-11 14:44:51.000000 mlora-0.3.0.post1/mlora/tasks/qa_tasks.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1679 2024-04-23 06:58:34.000000 mlora-0.3.0.post1/mlora/tokenizer.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     7862 2024-04-09 12:41:19.000000 mlora-0.3.0.post1/mlora/trainer.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     2125 2024-04-09 15:43:44.000000 mlora-0.3.0.post1/mlora/utils.py
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-23 06:58:50.768414 mlora-0.3.0.post1/mlora.egg-info/
--rw-r--r--   0 mikecovlee   (501) staff       (20)    11721 2024-04-23 06:58:50.000000 mlora-0.3.0.post1/mlora.egg-info/PKG-INFO
--rw-r--r--   0 mikecovlee   (501) staff       (20)      927 2024-04-23 06:58:50.000000 mlora-0.3.0.post1/mlora.egg-info/SOURCES.txt
--rw-r--r--   0 mikecovlee   (501) staff       (20)        1 2024-04-23 06:58:50.000000 mlora-0.3.0.post1/mlora.egg-info/dependency_links.txt
--rw-r--r--   0 mikecovlee   (501) staff       (20)      106 2024-04-23 06:58:50.000000 mlora-0.3.0.post1/mlora.egg-info/requires.txt
--rw-r--r--   0 mikecovlee   (501) staff       (20)        6 2024-04-23 06:58:50.000000 mlora-0.3.0.post1/mlora.egg-info/top_level.txt
--rw-r--r--   0 mikecovlee   (501) staff       (20)      823 2024-04-23 06:58:34.000000 mlora-0.3.0.post1/pyproject.toml
--rw-r--r--   0 mikecovlee   (501) staff       (20)       38 2024-04-23 06:58:50.769047 mlora-0.3.0.post1/setup.cfg
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-23 06:58:50.768069 mlora-0.3.0.post1/tests/
--rw-r--r--   0 mikecovlee   (501) staff       (20)      166 2024-04-03 07:54:48.000000 mlora-0.3.0.post1/tests/test_demo.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-05-06 09:25:43.593445 mlora-0.3.1/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    11357 2024-01-06 04:20:01.000000 mlora-0.3.1/LICENSE
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    11715 2024-05-06 09:25:43.593120 mlora-0.3.1/PKG-INFO
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    10954 2024-04-10 06:30:53.000000 mlora-0.3.1/README.md
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-05-06 09:25:43.587666 mlora-0.3.1/mlora/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1195 2024-04-23 06:58:34.000000 mlora-0.3.1/mlora/__init__.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-05-06 09:25:43.589389 mlora-0.3.1/mlora/backends/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      987 2024-04-09 13:04:56.000000 mlora-0.3.1/mlora/backends/__init__.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1324 2024-04-09 13:09:12.000000 mlora-0.3.1/mlora/backends/common.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1571 2024-04-09 13:03:52.000000 mlora-0.3.1/mlora/backends/cpu.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1343 2024-04-09 12:41:19.000000 mlora-0.3.1/mlora/backends/cuda.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     2044 2024-04-09 12:41:19.000000 mlora-0.3.1/mlora/backends/mps.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-05-06 09:25:43.590860 mlora-0.3.1/mlora/common/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     2221 2024-05-06 07:49:28.000000 mlora-0.3.1/mlora/common/__init__.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     5197 2024-04-09 12:41:19.000000 mlora-0.3.1/mlora/common/attention.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      932 2024-05-06 07:49:28.000000 mlora-0.3.1/mlora/common/checkpoint.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     2839 2024-05-06 07:49:28.000000 mlora-0.3.1/mlora/common/feed_forward.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    15638 2024-05-06 07:49:28.000000 mlora-0.3.1/mlora/common/lora_linear.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    13938 2024-05-06 07:49:28.000000 mlora-0.3.1/mlora/common/mix_lora.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     2266 2024-04-09 12:41:19.000000 mlora-0.3.1/mlora/common/model.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     9834 2024-05-06 07:49:28.000000 mlora-0.3.1/mlora/common/modelargs.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    13206 2024-05-06 07:49:28.000000 mlora-0.3.1/mlora/dispatcher.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     9764 2024-05-06 07:49:28.000000 mlora-0.3.1/mlora/evaluator.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     7905 2024-05-06 07:49:28.000000 mlora-0.3.1/mlora/generator.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    18789 2024-05-06 07:49:28.000000 mlora-0.3.1/mlora/model.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-05-06 09:25:43.591718 mlora-0.3.1/mlora/models/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      872 2024-04-09 12:41:19.000000 mlora-0.3.1/mlora/models/__init__.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     6296 2024-05-06 07:49:28.000000 mlora-0.3.1/mlora/models/modeling_gemma.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    20357 2024-05-06 07:49:28.000000 mlora-0.3.1/mlora/models/modeling_llama.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    12028 2024-05-06 07:49:28.000000 mlora-0.3.1/mlora/models/modeling_mistral.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    22290 2024-05-06 07:49:28.000000 mlora-0.3.1/mlora/models/modeling_phi.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1764 2024-04-03 07:55:06.000000 mlora-0.3.1/mlora/prompter.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-05-06 09:25:43.592375 mlora-0.3.1/mlora/tasks/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      528 2024-04-16 13:15:44.000000 mlora-0.3.1/mlora/tasks/__init__.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     6439 2024-04-11 14:44:51.000000 mlora-0.3.1/mlora/tasks/common.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     3182 2024-04-11 14:44:51.000000 mlora-0.3.1/mlora/tasks/glue_tasks.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     9752 2024-05-06 07:49:28.000000 mlora-0.3.1/mlora/tasks/qa_tasks.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1895 2024-05-06 07:49:28.000000 mlora-0.3.1/mlora/tokenizer.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     7856 2024-05-06 07:49:28.000000 mlora-0.3.1/mlora/trainer.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     2125 2024-04-09 15:43:44.000000 mlora-0.3.1/mlora/utils.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-05-06 09:25:43.592805 mlora-0.3.1/mlora.egg-info/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    11715 2024-05-06 09:25:43.000000 mlora-0.3.1/mlora.egg-info/PKG-INFO
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      927 2024-05-06 09:25:43.000000 mlora-0.3.1/mlora.egg-info/SOURCES.txt
+-rw-r--r--   0 mikecovlee   (501) staff       (20)        1 2024-05-06 09:25:43.000000 mlora-0.3.1/mlora.egg-info/dependency_links.txt
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      106 2024-05-06 09:25:43.000000 mlora-0.3.1/mlora.egg-info/requires.txt
+-rw-r--r--   0 mikecovlee   (501) staff       (20)        6 2024-05-06 09:25:43.000000 mlora-0.3.1/mlora.egg-info/top_level.txt
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      817 2024-05-06 07:49:28.000000 mlora-0.3.1/pyproject.toml
+-rw-r--r--   0 mikecovlee   (501) staff       (20)       38 2024-05-06 09:25:43.593496 mlora-0.3.1/setup.cfg
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-05-06 09:25:43.592560 mlora-0.3.1/tests/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      166 2024-04-03 07:54:48.000000 mlora-0.3.1/tests/test_demo.py
```

### Comparing `mlora-0.3.0.post1/LICENSE` & `mlora-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0.post1/PKG-INFO` & `mlora-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlora
-Version: 0.3.0.post1
+Version: 0.3.1
 Summary: A tool for fine-tuning large language models (LLMs) using the LoRA or QLoRA methods more efficiently.
 Project-URL: Homepage, https://github.com/scukdde-llm/mlora
 Project-URL: Bug Tracker, https://github.com/scukdde-llm/mlora/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `mlora-0.3.0.post1/README.md` & `mlora-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0.post1/mlora/__init__.py` & `mlora-0.3.1/mlora/__init__.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0.post1/mlora/backends/__init__.py` & `mlora-0.3.1/mlora/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0.post1/mlora/backends/common.py` & `mlora-0.3.1/mlora/backends/common.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0.post1/mlora/backends/cpu.py` & `mlora-0.3.1/mlora/backends/cpu.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0.post1/mlora/backends/cuda.py` & `mlora-0.3.1/mlora/backends/cuda.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0.post1/mlora/backends/mps.py` & `mlora-0.3.1/mlora/backends/mps.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0.post1/mlora/common/__init__.py` & `mlora-0.3.1/mlora/common/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     get_unpad_data,
     scaled_dot_product_attention,
     xformers_attention,
 )
 from .checkpoint import (
     CheckpointOffloadFunction,
     CheckpointRecomputeFunction,
+    CHECKPOINT_CLASSES,
 )
 from .feed_forward import FeedForward
 # LoRA
 from .lora_linear import (
     is_quantized,
     get_range_tensor,
     dequantize_bnb_weight,
@@ -69,14 +70,15 @@
     "repeat_kv",
     "apply_rotary_emb",
     "get_unpad_data",
     "scaled_dot_product_attention",
     "xformers_attention",
     "CheckpointOffloadFunction",
     "CheckpointRecomputeFunction",
+    "CHECKPOINT_CLASSES",
     "FeedForward",
     "is_quantized",
     "get_range_tensor",
     "dequantize_bnb_weight",
     "Lora",
     "Linear",
     "MixtralRouterLoss",
```

### Comparing `mlora-0.3.0.post1/mlora/common/attention.py` & `mlora-0.3.1/mlora/common/attention.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0.post1/mlora/common/feed_forward.py` & `mlora-0.3.1/mlora/common/feed_forward.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from .modelargs import MixConfig, LLMModelArgs, MultiLoraBatchData
 from .lora_linear import get_range_tensor, Linear
 from .mix_lora import moe_layer_factory
 from .model import LLMFeedForward
 
-from typing import Dict, List, Optional
+from typing import Tuple, Dict, List, Optional
 import torch
 
 
 class FeedForward(torch.nn.Module):
     def __init__(self, mlp: LLMFeedForward) -> None:
         super().__init__()
         self.mlp_: LLMFeedForward = mlp
         # mix of experts
         self.moes_: torch.ModuleDict = {}
 
     def state_dict(self) -> Dict[str, Linear]:
         return self.mlp_.state_dict()
 
-    def forward(self, data: torch.Tensor, input_args: MultiLoraBatchData,
-                router_logits: List[List] = None) -> torch.Tensor:
+    def forward(self, data: torch.Tensor, input_args: MultiLoraBatchData) -> Tuple[torch.Tensor, List]:
         if len(self.moes_) == 0:
-            return self.mlp_._batch_forward(data, input_args)
+            return self.mlp_._batch_forward(data, input_args), []
         else:
-            return self._mixlora_forward(data, input_args, router_logits)
+            return self._mixlora_forward(data, input_args)
 
     # MixLoRA
     def init_moe_weight(self, args: LLMModelArgs, config: MixConfig, gate: Optional[torch.Tensor] = None):
         self.moes_[config.adapter_name] = moe_layer_factory(args, config)
         if gate is None:
             torch.nn.init.normal_(
                 self.moes_[config.adapter_name].gate_.weight, mean=0.0, std=config.router_init_range_)
@@ -34,31 +33,36 @@
             with torch.no_grad():
                 self.moes_[config.adapter_name].gate_.weight.copy_(gate)
 
     def _expert_forward_callback(self, moe_name, act_fn, expert_idx, data):
         lora_name = f"moe.{moe_name}.experts.{expert_idx}"
         return self.mlp_._lora_forward(lora_name, act_fn, data)
 
-    def _mixlora_forward(self, data: torch.Tensor, input_args: MultiLoraBatchData,
-                         router_logits: List[List] = None):
-        batch_size, sequence_length, hidden_dim = data.shape
-        final_hidden_states = torch.zeros(
-            (batch_size, sequence_length, hidden_dim), dtype=data.dtype, device=data.device)
+    def _mixlora_forward(self, data: torch.Tensor, input_args: MultiLoraBatchData):
+        final_hidden_states = torch.zeros_like(data)
+
+        if input_args.output_router_logits_:
+            router_logits = [None for _ in range(
+                len(input_args.lora_batch_data_config_))]
+        else:
+            router_logits = []
+
+        lora_range = get_range_tensor(data.device, data.shape[0])
         for idx, lora_config in enumerate(input_args.lora_batch_data_config_):
             moe_name = lora_config.adapter_name_
             start_idx = lora_config.batch_start_idx_
             end_idx = lora_config.batch_end_idx_
 
             if moe_name in self.moes_:
                 current_hidden_states, current_router_outputs = self.moes_[
                     moe_name].forward(self._expert_forward_callback, data[start_idx:end_idx])
 
-                if router_logits is not None and current_router_outputs is not None:
-                    router_logits[idx].append(current_router_outputs)
+                if input_args.output_router_logits_ and current_router_outputs is not None:
+                    router_logits[idx] = current_router_outputs
             else:
                 current_hidden_states = self.mlp_._lora_forward(
                     moe_name, self.act_, data[start_idx:end_idx])
 
-            final_hidden_states.index_add_(0, get_range_tensor(data.device, batch_size)[
-                                           start_idx:end_idx], current_hidden_states)
+            final_hidden_states.index_add_(
+                0, lora_range[start_idx:end_idx], current_hidden_states)
 
-        return final_hidden_states
+        return final_hidden_states, router_logits
```

### Comparing `mlora-0.3.0.post1/mlora/common/lora_linear.py` & `mlora-0.3.1/mlora/common/lora_linear.py`

 * *Files 9% similar despite different names*

```diff
@@ -89,16 +89,15 @@
             drop_data = F.dropout(
                 data[start_idx:end_idx], p=dropout)
             drop_data.mul_(scaling)
             drop_data = drop_data @ lora_a.transpose(0, 1)
 
             lora_data = drop_data @ lora_b.transpose(0, 1)
 
-            result.index_add_(
-                dim=0, index=lora_range[start_idx:end_idx], source=lora_data)
+            result.index_add_(0, lora_range[start_idx:end_idx], lora_data)
 
             save_inputs += (lora_a, lora_b, drop_data)
 
         ctx.input_args = input_args
         ctx.dropouts = dropouts
         ctx.scalings = scalings
         ctx.save_for_backward(*save_inputs)
@@ -110,37 +109,34 @@
         grad_result = None
         grad_data = None
         grad_input_args = None
         grad_dropouts = None
         grad_scalings = None
         grad_loras = ()
 
-        data = ctx.saved_tensors[0]
-        loras = ctx.saved_tensors[1:]
+        data, *loras = ctx.saved_tensors
 
         if ctx.needs_input_grad[0]:
             grad_result = grad_output
         if ctx.needs_input_grad[1]:
-            grad_data = torch.empty_like(data)
+            grad_data = torch.zeros_like(data)
 
         lora_range = get_range_tensor(
             grad_output.device, batch_size=grad_output.shape[0])
         for lora_a, lora_b, drop_data, dropout, scaling, lora_config in zip(loras[::3],
                                                                             loras[1::3],
                                                                             loras[2::3],
                                                                             ctx.dropouts,
                                                                             ctx.scalings,
                                                                             ctx.input_args.lora_batch_data_config_):
             start_idx = lora_config.batch_start_idx_
             end_idx = lora_config.batch_end_idx_
             assert not ((lora_a is None) ^ (lora_b is None))
             if lora_a is None and lora_b is None:
                 grad_loras += (None, None)
-                grad_data.index_fill_(
-                    dim=0, index=lora_range[start_idx:end_idx], value=0)
                 continue
 
             # lora_data shape is batch_size * seq_len * in_dim
             lora_data = data[start_idx:end_idx]
             # grad_y shape is batch_size * seq_len * out_dim
             grad_y = grad_output[start_idx:end_idx]
 
@@ -152,15 +148,16 @@
 
             grad_a = torch.sum(bstage.transpose(1, 2) @ lora_data, dim=0)
             grad_b = torch.sum(grad_y.transpose(1, 2) @ drop_data, dim=0)
             grad_loras += (grad_a, grad_b)
 
             # grad_data shape is batch_size * seq_len * in_dim
             if grad_data is not None:
-                grad_data[start_idx:end_idx] = bstage @ lora_a
+                grad_data.index_add_(
+                    0, lora_range[start_idx:end_idx], bstage @ lora_a)
 
         return grad_result, grad_data, grad_input_args, grad_dropouts, grad_scalings, *grad_loras
 
 
 class Lora(nn.Module):
     def __init__(self,
                  base_layer: nn.Module,
@@ -240,21 +237,21 @@
             residual = torch.nn.functional.linear(
                 hidden_states.to(torch.float32), weight)
         else:
             # for full precision or half precision
             weight = weight.to(torch.float32)
         weight_norm = self._get_weight_norm(weight).detach()
         mag_norm_scale = (self.magnitude_vector_ / weight_norm).view(1, -1)
-        return (mag_norm_scale - 1) * residual + mag_norm_scale * result_lora
+        return mag_norm_scale * residual + mag_norm_scale * result_lora
 
     def forward(self, residual: torch.Tensor, hidden_states: torch.Tensor) -> torch.Tensor:
         result_lora = self.lora_b_(self.lora_a_(self.dropout_(
             hidden_states.to(torch.float32)))) * self.scaling_
         if self.use_dora_:
-            return self.apply_dora(residual, result_lora, hidden_states)
+            return self.apply_dora(residual, result_lora, hidden_states).to(hidden_states.dtype)
         else:
             return residual + result_lora.to(residual.dtype)
 
 
 class Linear(nn.Module):
     def __init__(self, base_layer: nn.Module, device: str):
         super().__init__()
@@ -288,35 +285,35 @@
         self.loras_[adapter_name].reset_parameters(lora_tensor)
 
     def _appy_dora(self,
                    residual: torch.Tensor,
                    lora_delta: torch.Tensor,
                    hidden_states: torch.Tensor,
                    input_args: MultiLoraBatchData):
-        next_states = residual.clone()
+        next_states = torch.zeros_like(residual)
+        lora_range = get_range_tensor(
+            next_states.device, batch_size=next_states.shape[0])
         for lora_config in input_args.lora_batch_data_config_:
             adapter_name = lora_config.adapter_name_
             start_idx = lora_config.batch_start_idx_
             end_idx = lora_config.batch_end_idx_
 
             if adapter_name == "" or adapter_name not in self.loras_:
                 continue
 
-            lora_range = get_range_tensor(
-                next_states.device, batch_size=next_states.shape[0])[start_idx:end_idx]
             if self.loras_[adapter_name].use_dora_:
-                next_states.index_add_(0, lora_range, self.loras_[adapter_name].apply_dora(
+                next_states.index_add_(0, lora_range[start_idx:end_idx], self.loras_[adapter_name].apply_dora(
                     residual[start_idx:end_idx], lora_delta[start_idx:end_idx], hidden_states[start_idx:end_idx]))
             else:
                 next_states.index_add_(
-                    0, lora_range, lora_delta[start_idx:end_idx])
+                    0, lora_range[start_idx:end_idx], residual[start_idx:end_idx] + lora_delta[start_idx:end_idx])
 
         return next_states
 
-    def forward(self, hidden_states: torch.Tensor, input_args: MultiLoraBatchData) -> torch.Tensor:
+    def _efficient_impl(self, hidden_states: torch.Tensor, input_args: MultiLoraBatchData) -> torch.Tensor:
         # hidden_states shape is: batch_size * max_seq_len * dim
         # result = hidden_states @ self.weight_.transpose(0, 1)
         residual = self.base_layer_.forward(hidden_states)
 
         if len(self.loras_) == 0:
             return residual
 
@@ -347,7 +344,39 @@
             next_states = self._appy_dora(residual.to(
                 torch.float32), lora_delta, hidden_states, input_args)
         else:
             next_states = LoraFunction.apply(
                 residual.to(torch.float32), hidden_states.to(torch.float32), input_args, dropouts, scalings, *loras)
 
         return next_states.to(hidden_states.dtype)
+
+    def _compatible_impl(self, hidden_states: torch.Tensor, input_args: MultiLoraBatchData) -> torch.Tensor:
+        # hidden_states shape is: batch_size * max_seq_len * dim
+        # result = hidden_states @ self.weight_.transpose(0, 1)
+        residual = self.base_layer_.forward(hidden_states)
+
+        if len(self.loras_) == 0:
+            return residual
+
+        next_states = torch.zeros_like(residual)
+        lora_range = get_range_tensor(
+            hidden_states.device, hidden_states.shape[0])
+
+        for lora_config in input_args.lora_batch_data_config_:
+            adapter_name = lora_config.adapter_name_
+            start_idx = lora_config.batch_start_idx_
+            end_idx = lora_config.batch_end_idx_
+
+            if adapter_name == "" or adapter_name not in self.loras_:
+                continue
+
+            lora_data = self.loras_[adapter_name].forward(
+                residual[start_idx: end_idx], hidden_states[start_idx:end_idx])
+            next_states.index_add_(0, lora_range[start_idx:end_idx], lora_data)
+
+        return next_states
+
+    def forward(self, hidden_states: torch.Tensor, input_args: MultiLoraBatchData) -> torch.Tensor:
+        if input_args.efficient_operator_:
+            return self._efficient_impl(hidden_states, input_args)
+        else:
+            return self._compatible_impl(hidden_states, input_args)
```

### Comparing `mlora-0.3.0.post1/mlora/common/mix_lora.py` & `mlora-0.3.1/mlora/common/mix_lora.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,115 @@
 from .modelargs import LLMModelArgs, MixConfig
 
 import torch
 import torch.nn.functional as F
 
-from typing import List, Tuple
+from typing import List, Tuple, Optional
 from transformers.activations import ACT2FN
 
 
-def _mixtral_load_balancing_loss_func(gate_logits: List[torch.Tensor], num_experts: int, top_k: int) -> float:
-    concatenated_gate_logits = torch.cat(gate_logits, dim=0)
+def _mixtral_load_balancing_loss_func(
+    gate_logits: List[torch.Tensor], num_experts: int, top_k: int, attention_mask: Optional[torch.Tensor] = None
+) -> float:
+    r"""
+    Computes auxiliary load balancing loss as in Switch Transformer - implemented in Pytorch.
+
+    See Switch Transformer (https://arxiv.org/abs/2101.03961) for more details. This function implements the loss
+    function presented in equations (4) - (6) of the paper. It aims at penalizing cases where the routing between
+    experts is too unbalanced.
+
+    Args:
+        gate_logits (Union[`torch.Tensor`, Tuple[torch.Tensor]):
+            Logits from the `gate`, should be a tuple of model.config.num_hidden_layers tensors of
+            shape [batch_size X sequence_length, num_experts].
+        attention_mask (`torch.Tensor`, None):
+            The attention_mask used in forward function
+            shape [batch_size X sequence_length] if not None.
+        num_experts (`int`, *optional*):
+            Number of experts
+
+    Returns:
+        The auxiliary loss.
+    """
+    compute_device = gate_logits[0].device
+    concatenated_gate_logits = torch.cat(
+        [layer_gate.to(compute_device) for layer_gate in gate_logits], dim=0)
 
     routing_weights = torch.nn.functional.softmax(
         concatenated_gate_logits, dim=-1)
 
     _, selected_experts = torch.topk(routing_weights, top_k, dim=-1)
 
-    expert_mask = torch.nn.functional.one_hot(
-        selected_experts, num_experts)
+    expert_mask = torch.nn.functional.one_hot(selected_experts, num_experts)
 
-    tokens_per_expert = torch.mean(expert_mask.float(), dim=0)
+    if attention_mask is None:
+        # Compute the percentage of tokens routed to each experts
+        tokens_per_expert = torch.mean(expert_mask.float(), dim=0)
+
+        # Compute the average probability of routing to these experts
+        router_prob_per_expert = torch.mean(routing_weights, dim=0)
+    else:
+        batch_size, sequence_length = attention_mask.shape
+        num_hidden_layers = concatenated_gate_logits.shape[0] // (
+            batch_size * sequence_length)
+
+        # Compute the mask that masks all padding tokens as 0 with the same shape of expert_mask
+        expert_attention_mask = (
+            attention_mask[None, :, :, None, None]
+            .expand((num_hidden_layers, batch_size, sequence_length, top_k, num_experts))
+            .reshape(-1, top_k, num_experts)
+            .to(compute_device)
+        )
+
+        # Compute the percentage of tokens routed to each experts
+        tokens_per_expert = torch.sum(expert_mask.float() * expert_attention_mask, dim=0) / torch.sum(
+            expert_attention_mask, dim=0
+        )
+
+        # Compute the mask that masks all padding tokens as 0 with the same shape of tokens_per_expert
+        router_per_expert_attention_mask = (
+            attention_mask[None, :, :, None]
+            .expand((num_hidden_layers, batch_size, sequence_length, num_experts))
+            .reshape(-1, num_experts)
+            .to(compute_device)
+        )
 
-    router_prob_per_expert = torch.mean(routing_weights, dim=0)
+        # Compute the average probability of routing to these experts
+        router_prob_per_expert = torch.sum(routing_weights * router_per_expert_attention_mask, dim=0) / torch.sum(
+            router_per_expert_attention_mask, dim=0
+        )
 
     overall_loss = torch.sum(
         tokens_per_expert * router_prob_per_expert.unsqueeze(0))
     return overall_loss * num_experts
 
 
 class MixtralRouterLoss(torch.nn.Module):
     def __init__(self, config: MixConfig) -> None:
         super().__init__()
         self.aux_loss_coef = config.router_aux_loss_coef_
         self.experts = config.num_experts_
         self.topk = config.top_k_
 
-    def forward(self, gate_logits) -> torch.Tensor:
-        return self.aux_loss_coef * _mixtral_load_balancing_loss_func(gate_logits, self.experts, self.topk)
+    def forward(self, gate_logits, attention_mask) -> torch.Tensor:
+        return self.aux_loss_coef * _mixtral_load_balancing_loss_func(gate_logits, self.experts, self.topk, attention_mask)
 
 
 class MixtralSparseMoe(torch.nn.Module):
     def __init__(self, args: LLMModelArgs, config: MixConfig) -> None:
         super().__init__()
 
         self.adapter_name_: str = config.adapter_name
         self.dtype_: torch.dtype = torch.float32
         self.gate_ = torch.nn.Linear(
             args.dim_, config.num_experts_, bias=False, device=config.device, dtype=self.dtype_)
         self.act_ = ACT2FN[args.hidden_act_ if config.act_fn_ is None else config.act_fn_]
-        self.experts_ = config.num_experts_
-        self.topk_ = config.top_k_
+        self.experts_: int = config.num_experts_
+        self.topk_: int = config.top_k_
+        self.jitter_noise_: float = config.jitter_noise_
         self.router_profile_: bool = False
         self.profiler_: List[int] = None
 
     def _profiling(self,
                    batch_size: int,
                    sequence_length: int,
                    selected_experts: torch.Tensor) -> None:
@@ -73,14 +130,20 @@
             for idx in range(self.experts_):
                 pressure = (
                     router_statistic_[idx] / batch_size) / sequence_length
                 self.profiler_[idx] = (self.profiler_[idx] + pressure) / 2
 
     def forward(self, expert_fn, hidden_states: torch.Tensor) -> Tuple:
         batch_size, sequence_length, hidden_dim = hidden_states.shape
+
+        if self.jitter_noise_ > 0:
+            # Multiply the token inputs by the uniform distribution - adding some noise
+            hidden_states *= torch.empty_like(hidden_states).uniform_(
+                1.0 - self.jitter_noise_, 1.0 + self.jitter_noise_)
+
         input_dtype = hidden_states.dtype
         hidden_states = hidden_states.view(-1, hidden_dim).to(self.dtype_)
         # router_logits: (batch * sequence_length, n_experts)
         router_logits = self.gate_(hidden_states)
 
         routing_weights = F.softmax(router_logits, dim=1, dtype=self.dtype_)
         routing_weights, selected_experts = torch.topk(
@@ -99,28 +162,21 @@
         expert_mask = torch.nn.functional.one_hot(
             selected_experts, num_classes=self.experts_).permute(2, 1, 0)
 
         # Loop over all available experts in the model and perform the computation on each expert
         for expert_idx in range(self.experts_):
             idx, top_x = torch.where(expert_mask[expert_idx])
 
-            if top_x.shape[0] == 0:
-                continue
-
-            # in torch it is faster to index using lists than torch tensors
-            top_x_list = top_x.tolist()
-            idx_list = idx.tolist()
-
             # Index the correct hidden states and compute the expert hidden state for
             # the current expert. We need to make sure to multiply the output hidden
             # states by `routing_weights` on the corresponding tokens (top-1 and top-2)
             current_state = hidden_states[None,
-                                          top_x_list].reshape(-1, hidden_dim).to(input_dtype)
+                                          top_x].reshape(-1, hidden_dim).to(input_dtype)
             current_hidden_states = expert_fn(
-                self.adapter_name_, self.act_, expert_idx, current_state) * routing_weights[top_x_list, idx_list, None]
+                self.adapter_name_, self.act_, expert_idx, current_state) * routing_weights[top_x, idx, None]
 
             # However `index_add_` only support torch tensors for indexing so we'll use
             # the `top_x` tensor here.
             final_hidden_states.index_add_(
                 0, top_x, current_hidden_states.to(self.dtype_))
 
         final_hidden_states = final_hidden_states.reshape(
@@ -172,15 +228,15 @@
 
 class SwitchRouterLoss(torch.nn.Module):
     def __init__(self, config: MixConfig) -> None:
         super().__init__()
         self.z_loss_coef = config.router_z_loss_coef_
         self.aux_loss_coef = config.router_aux_loss_coef_
 
-    def forward(self, router_outputs) -> torch.Tensor:
+    def forward(self, router_outputs, attention_mask) -> torch.Tensor:
         router_logits, expert_indexes = _switch_unpack_router_logits(
             router_outputs)
         z_loss = _switch_router_z_loss_func(router_logits)
         router_probs = F.softmax(router_logits, dim=-1)
         aux_loss = _switch_load_balancing_loss_func(
             router_probs, expert_indexes)
         return self.z_loss_coef * z_loss + self.aux_loss_coef * aux_loss
@@ -250,15 +306,18 @@
 }
 
 
 def router_loss_factory(config: MixConfig) -> torch.nn.Module:
     if config.routing_strategy_ not in router_loss_dict:
         raise ValueError(
             f"Unknown routing strategy {config.routing_strategy_}")
-    return router_loss_dict[config.routing_strategy_](config)
+    if config.router_loss_:
+        return router_loss_dict[config.routing_strategy_](config)
+    else:
+        return None
 
 
 moe_layer_dict = {
     "mixtral": MixtralSparseMoe,
     "switch": SwitchSparseMoe
 }
```

### Comparing `mlora-0.3.0.post1/mlora/common/model.py` & `mlora-0.3.1/mlora/common/model.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0.post1/mlora/common/modelargs.py` & `mlora-0.3.1/mlora/common/modelargs.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 @dataclass
 class LLMModelArgs:
     name_or_path_: str = ""
     device_: str = ""
     dim_: int = 4096
     multiple_of_: int = 256
+    intermediate_: int = 11008
     n_heads_: int = 32
     n_kv_heads_: int = 32
     n_layers_: int = 32
     hidden_act_: str = "silu"
     hidden_dropout_: float = 0.0
     vocab_size_: int = -1
     pad_token_id_: int = -1
@@ -68,22 +69,23 @@
 
 
 @dataclass
 class MultiLoraBatchData:
     lora_batch_data_config_: List[LoraBatchDataConfig] = None
 
     batch_tokens_: List[Tokens] = None
-    attention_masks_: List[Tokens] = None
+    batch_labels_: List[Labels] = None
+    attention_masks_: List[Masks] = None
 
-    gradient_checkpoint_: bool = True
-    inference_seq_pos_: int = -1
+    output_router_logits_: bool = True
 
-    @property
-    def inference_mode_(self) -> bool:
-        return self.inference_seq_pos_ >= 0
+    gradient_checkpoint_: str = "none"
+    efficient_operator_: bool = True
+    inference_mode_: bool = False
+    diagonal_pos_: int = 1
 
 
 @dataclass
 class LoraConfig:
     adapter_name: str = ""
     task_name: str = "casual"
     device: str = f"{get_backend().device_name()}:0"
@@ -176,46 +178,48 @@
 class MixConfig(LoraConfig):
     # expert lora
     expert_config_: LoraConfig = None
     # router config
     router_aux_loss_coef_: float = None
     router_init_range_: float = None
     routing_strategy_: str = None
+    jitter_noise_: float = None
+    router_loss_: bool = True
     num_experts_: int = None
     act_fn_: str = None
     # mixtral config
     top_k_: int = None
     # switch transformers config
     router_z_loss_coef_: float = None
     expert_capacity_: int = None
-    jitter_noise_: float = None
     ffn_dropout_: float = None
 
     def check(self) -> "MixConfig":
         super().check()
         if self.expert_config_ is not None:
             self.expert_config_.check()
         assert isinstance(self.router_aux_loss_coef_,
                           float) and self.router_aux_loss_coef_ >= 0
         assert isinstance(self.router_init_range_,
                           float) and self.router_init_range_ >= 0
         assert isinstance(self.routing_strategy_,
                           str) and self.routing_strategy_ in available_routing_strategies
+        assert isinstance(self.jitter_noise_,
+                          float) and self.jitter_noise_ >= 0
+        assert isinstance(self.router_loss_, bool)
         assert isinstance(self.num_experts_, int) and self.num_experts_ > 0
         assert self.act_fn_ is None or (isinstance(
             self.act_fn_, str) and self.act_fn_ in ACT2FN)
         if self.routing_strategy_ == "mixtral":
             assert isinstance(self.top_k_, int) and self.top_k_ > 0
         elif self.routing_strategy_ == "switch":
             assert isinstance(self.router_z_loss_coef_,
                               float) and self.router_z_loss_coef_ >= 0
             assert isinstance(self.expert_capacity_,
                               int) and self.expert_capacity_ > 0
-            assert isinstance(self.jitter_noise_,
-                              float) and self.jitter_noise_ >= 0
             assert isinstance(self.ffn_dropout_,
                               float) and self.ffn_dropout_ >= 0
 
         return self
 
     def from_config(self, config: Dict[str, any]) -> "MixConfig":
         super().from_config(config)
@@ -223,27 +227,28 @@
             expert_config = copy.deepcopy(config)
             expert_config.update(config["expert_lora"])
             self.expert_config_ = LoraConfig().from_config(expert_config)
         self.router_aux_loss_coef_ = config.get(
             "router_aux_loss_coef", 0.001)  # for training
         self.router_init_range_ = config.get("router_init_range", 0.02)
         self.routing_strategy_ = config["routing_strategy"]
+        self.jitter_noise_ = config.get("jitter_noise", 0.0)
+        self.router_loss_ = config.get("router_loss", True)
         self.num_experts_ = config["num_experts"]
         # silu for mixtral or gelu_new for switch transformers
         # left blank to automatically use the original act_fn of FFN
         self.act_fn_ = config.get("act_fn", None)
         if self.routing_strategy_ == "mixtral":
             self.top_k_ = config.get("top_k", 2)
         elif self.routing_strategy_ == "switch":
             self.router_z_loss_coef_ = config.get(
                 "router_z_loss_coef", 0.001)  # for training
             # expert_capacity = (max_sequence_length / num_experts) * capacity_factor
             # common values of capacity_factor: 1.0, 1.25, 2.0
             self.expert_capacity_ = config.get("expert_capacity", 64)
-            self.jitter_noise_ = config.get("jitter_noise", 0.0)
             self.ffn_dropout_ = config.get("ffn_dropout", 0.0)
 
         return self
 
     def export(self) -> Dict[str, any]:
         config = super().export()
         config["peft_type"] = "MIXLORA"
```

### Comparing `mlora-0.3.0.post1/mlora/dispatcher.py` & `mlora-0.3.1/mlora/dispatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,10 +346,12 @@
             lora_batch_data_config.append(LoraBatchDataConfig(adapter_name_=adapter,
                                                               batch_start_idx_=adapter_start_idx,
                                                               batch_end_idx_=adapter_end_idx))
             adapter_start_idx = adapter_end_idx
 
         self.__dispatch_task_out()
 
-        return batch_labels, MultiLoraBatchData(lora_batch_data_config_=lora_batch_data_config,
-                                                batch_tokens_=batch_tokens,
-                                                attention_masks_=attention_masks)
+        return MultiLoraBatchData(lora_batch_data_config_=lora_batch_data_config,
+                                  batch_tokens_=batch_tokens,
+                                  batch_labels_=batch_labels,
+                                  attention_masks_=attention_masks,
+                                  gradient_checkpoint_="recompute")
```

### Comparing `mlora-0.3.0.post1/mlora/evaluator.py` & `mlora-0.3.1/mlora/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     return (current_configs,
             sequence_lengths,
             batch_labels,
             MultiLoraBatchData(
                 lora_batch_data_config_=batch_data_config,
                 batch_tokens_=batch_tokens,
                 attention_masks_=atten_masks,
-                gradient_checkpoint_=False))
+                inference_mode_=True))
 
 
 def _compute_metrcis(model, current_configs, sequence_lengths, batch_labels, outputs):
     for idx, output in enumerate(outputs):
         config: EvaluateConfig = current_configs[idx]
         task: BasicTask = config.task_
         metric: BasicMetric = config.metric_
```

### Comparing `mlora-0.3.0.post1/mlora/generator.py` & `mlora-0.3.1/mlora/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,16 @@
     prev_pos = 0
     stop_reached = torch.tensor([False] * batch_size, device=device)
     input_text_mask = tokens != tokenizer.pad_id_
     for cur_pos in range(min_tokens_len, total_len):
         input_data = MultiLoraBatchData(
             lora_batch_data_config_=batch_data_config,
             batch_tokens_=tokens[:, prev_pos:cur_pos].tolist(),
-            inference_seq_pos_=prev_pos)
+            diagonal_pos_=prev_pos + 1,
+            inference_mode_=True)
         outputs = model.forward(input_data)
         for output in outputs:
             config = config_dict[output.adapter_name]
             start_idx = output.batch_start_idx_
             end_idx = output.batch_end_idx_
 
             next_token = logits_process(output.logits[:, -1],
```

### Comparing `mlora-0.3.0.post1/mlora/model.py` & `mlora-0.3.1/mlora/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -178,24 +178,24 @@
                     lora_a = weight[lora_a_name]
                     lora_b = weight[lora_b_name]
 
                 linear_layer_list[idx].init_lora_weight(
                     config, (lora_a, lora_b))
 
 
-class LLMSequentialWrapper(torch.nn.Module):
+class OutputSequentialWrapper(torch.nn.Module):
     def __init__(self, module: torch.nn.Module):
         super().__init__()
         self.wrapper_module_ = module
 
     def name(self) -> str:
         return type(self.wrapper_module_).__name__
 
     def forward(self, input: Tuple) -> Tuple:
-        output = self.wrapper_module_.forward(*input[:2])
+        output = self.wrapper_module_.forward(input[0], input[2])
         return (output, ) + input[1:]
 
 
 class LLMModel(torch.nn.Module):
     def __init__(self, model: LLMForCausalLM):
         super().__init__()
         args: LLMModelArgs = model.config_
@@ -208,75 +208,89 @@
         self.name_or_path_ = args.name_or_path_
         self.vocab_size_ = args.vocab_size_
         self.device_ = args.device_
         self.dtype_ = args.dtype_
 
         self.output_ = OutputLayer()
         seq_module = model.sequential_module()
-        seq_module.update({"output": LLMSequentialWrapper(self.output_)})
+        seq_module.update({"output": OutputSequentialWrapper(self.output_)})
         seq_module.move_to_end("output")
         self.seq_module_ = torch.nn.Sequential(seq_module)
         # adapter configs
         self.adapter_configs_: Dict[str, LoraConfig] = {}
 
-    # train model or inference model: output is probs
-    def forward(self, input: MultiLoraBatchData,
-                labels: List[List[int]] = None) -> List[LLMModelOutput]:
-        tokens = torch.tensor(input.batch_tokens_,
+    # compute the model: output probs
+    def forward(self, input_args: MultiLoraBatchData) -> List[LLMModelOutput]:
+        assert input_args.batch_tokens_ is not None
+        assert input_args.gradient_checkpoint_ != "none" or input_args.inference_mode_
+
+        labels = input_args.batch_labels_
+
+        # prepare inputs
+        tokens = torch.tensor(input_args.batch_tokens_,
                               dtype=torch.int64, device=self.device_)
 
         # prepare mask
-        if self.config_.attn_implementation_ == "flash_attn":
-            if input.attention_masks_ is not None and 0 in input.attention_masks_:
-                # 2d mask is passed through the layers
-                mask = torch.tensor(input.attention_masks_,
-                                    dtype=torch.int64, device=self.device_)
-            else:
-                mask = None
+        if input_args.attention_masks_ is not None and 0 in input_args.attention_masks_:
+            # 2d mask is passed through the layers
+            attn_mask = torch.tensor(input_args.attention_masks_,
+                                     dtype=torch.int64, device=self.device_)
         else:
-            mask = self.model_.causal_mask(
+            attn_mask = None
+
+        if self.config_.attn_implementation_ != "flash_attn":
+            causal_mask = self.model_.causal_mask(
                 input_tokens=tokens,
-                additional_mask=input.attention_masks_,
+                additional_mask=input_args.attention_masks_,
                 multi_head=(self.config_.attn_implementation_ == "xformers"),
-                diagonal=input.inference_seq_pos_ + 1 if input.inference_mode_ else 1)
-
-        # routing data
-        router_logits: List[List] = list(
-            [] for _ in range(len(input.lora_batch_data_config_)))
+                diagonal=input_args.diagonal_pos_)
+        else:
+            causal_mask = attn_mask
 
-        if input.inference_mode_:
-            input.gradient_checkpoint_ = False
+        input_args.batch_labels_ = None
+        input_args.batch_tokens_ = None
+        input_args.attention_masks_ = None
 
-        data = (tokens, input, mask,
-                router_logits, input.gradient_checkpoint_)
+        data = (tokens, causal_mask, input_args)
 
         for seq_layer in self.seq_module_:
             data = seq_layer.forward(data)
 
+        # collecting router logits
+        router_logits = [[]
+                         for _ in range(len(input_args.lora_batch_data_config_))]
+        for seq_layer in self.seq_module_:
+            if not hasattr(seq_layer, "router_probs_"):
+                continue
+            for idx in range(len(input_args.lora_batch_data_config_)):
+                router_logits[idx].append(seq_layer.router_probs_[idx])
+
+        # calculate loss
         output = data[0]
         assert isinstance(output, List)
-        for idx, lora_config in enumerate(input.lora_batch_data_config_):
+        for idx, lora_config in enumerate(input_args.lora_batch_data_config_):
             output_data = output[idx]
             assert isinstance(output_data, LLMModelOutput)
             start_idx = lora_config.batch_start_idx_
             end_idx = lora_config.batch_end_idx_
             output_data.batch_start_idx_ = start_idx
             output_data.batch_end_idx_ = end_idx
             if labels is None:
                 continue
             # compute loss when labels provided
             output_data.loss = output_data.loss_fn_(
                 tokens[start_idx:end_idx], output_data.logits, labels[start_idx:end_idx])
             output_data.loss_fn_ = None
-            if len(router_logits[idx]) == 0:
+            if not input_args.output_router_logits_ or len(router_logits[idx]) == 0:
                 continue
             # compute router loss when router logits is available
             loss_fn = router_loss_factory(
                 self.adapter_configs_[output_data.adapter_name])
-            output_data.aux_loss = loss_fn(router_logits[idx])
+            if loss_fn is not None:
+                output_data.aux_loss = loss_fn(router_logits[idx], attn_mask)
 
         return output
 
     def init_lora_layer_weight(self, config: LoraConfig, weight: Optional[Dict[str, torch.Tensor]]):
         self.adapter_configs_[config.adapter_name] = config
         # init output layer
         if config.task_name in task_dict and isinstance(task_dict[config.task_name], SequenceClassificationTask):
```

### Comparing `mlora-0.3.0.post1/mlora/models/__init__.py` & `mlora-0.3.1/mlora/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0.post1/mlora/models/modeling_gemma.py` & `mlora-0.3.1/mlora/models/modeling_gemma.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from mlora.common import (
-    CheckpointRecomputeFunction as CheckpointFunction,
+    CHECKPOINT_CLASSES,
     FeedForward,
 )
 from mlora.models.modeling_llama import (
     LlamaConfig,
     LLAMA_ATTENTION_CLASSES as GEMMA_ATTENTION_CLASSES,
     LlamaMLP,
     LlamaDecoderLayer,
@@ -64,27 +64,26 @@
         return type(self.wrapper_module_).__name__
 
     def forward(self, input: Tuple) -> Tuple:
         module_name = self.name()
 
         if module_name == "GemmaEmbedding":
             output = self.wrapper_module_.forward(input[0])
-            if input[-1]:
+            if input[-1].gradient_checkpoint_ != "none":
                 output = output.requires_grad_(True)
-            return (output, ) + input[1:]
+            return (output,) + input[1:]
         elif module_name == "GemmaRMSNorm":
             output = self.wrapper_module_.forward(input[0])
-            return (output, ) + input[1:]
+            return (output,) + input[1:]
         elif module_name == "LlamaDecoderLayer":
-            if input[-1]:
-                output = CheckpointFunction.apply(
-                    self.wrapper_module_.forward, *input[:-1])
-            else:
-                output = self.wrapper_module_.forward(*input[:-1])
-            return (output, ) + input[1:]
+            outputs = CHECKPOINT_CLASSES[input[-1].gradient_checkpoint_](
+                self.wrapper_module_.forward, *input)
+            if len(outputs) > 1:
+                self.router_probs_ = outputs[1:]
+            return (outputs[0],) + input[1:]
         else:
             raise f"module invalid: {module_name}"
 
 
 class GemmaForCausalLM(LlamaForCausalLM):
     def __init__(self, config: LlamaConfig) -> None:
         super().__init__(config)
@@ -114,14 +113,15 @@
                         device: str = get_backend().device_name() + ":0"):
         assert not use_sliding_window, "Gemma model does not support SWA."
         llm_config: modeling_gemma.GemmaConfig = llm_model.config
         llm_args = LlamaConfig(
             name_or_path_=llm_config.name_or_path,
             vocab_size_=llm_config.vocab_size,
             dim_=llm_config.hidden_size,
+            intermediate_=llm_config.intermediate_size,
             n_layers_=llm_config.num_hidden_layers,
             n_heads_=llm_config.num_attention_heads,
             n_kv_heads_=llm_config.num_key_value_heads,
             hidden_act_=llm_config.hidden_act,
             rms_norm_eps_=llm_config.rms_norm_eps,
             max_seq_len_=llm_config.max_position_embeddings,
             rope_theta_=llm_config.rope_theta,
@@ -139,22 +139,20 @@
         model.embed_tokens_ = GemmaEmbedding(
             llm_model.model.embed_tokens.weight, llm_args.pad_token_id_, llm_args.dim_**0.5)
         model.norm_ = GemmaRMSNorm(
             llm_model.model.norm.weight, llm_args.rms_norm_eps_)
         copy_parameters(llm_model.lm_head, model.lm_head_)
 
         for idx, layer in enumerate(llm_model.model.layers):
-            decoder = LlamaDecoderLayer()
-            decoder.layer_id_ = idx
+            decoder = LlamaDecoderLayer(idx)
             decoder.self_attn_ = GEMMA_ATTENTION_CLASSES[llm_args.attn_implementation_](
                 layer.self_attn.q_proj,
                 layer.self_attn.k_proj,
                 layer.self_attn.v_proj,
                 layer.self_attn.o_proj,
-                idx,
                 llm_args,
             )
             decoder.mlp_ = FeedForward(LlamaMLP(
                 layer.mlp.gate_proj,
                 layer.mlp.down_proj,
                 layer.mlp.up_proj,
                 llm_args,
```

### Comparing `mlora-0.3.0.post1/mlora/models/modeling_llama.py` & `mlora-0.3.1/mlora/models/modeling_llama.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     apply_rotary_emb,
     get_unpad_data,
     repeat_kv,
     Masks,
     Linear,
     FeedForward,
     MultiLoraBatchData,
-    CheckpointRecomputeFunction as CheckpointFunction,
+    CHECKPOINT_CLASSES,
     LLMModelArgs,
     LLMAttention,
     LLMFeedForward,
     LLMDecoder,
     LLMForCausalLM,
 )
 from mlora.backends import _backend, get_backend
@@ -40,27 +40,25 @@
 @dataclass
 class LlamaConfig(LLMModelArgs):
     rms_norm_eps_: float = 1e-6
 
 
 # Multi-headed attention from 'Attention Is All You Need' paper.
 class LlamaAttention(LLMAttention):
-    def __init__(self, wq: nn.Module, wk: nn.Module, wv: nn.Module, wo: nn.Module,
-                 layer_idx: int, args: LlamaConfig):
+    def __init__(self, wq: nn.Module, wk: nn.Module, wv: nn.Module, wo: nn.Module, args: LlamaConfig):
         super().__init__()
         # attention
         self.wq_: Linear = Linear(wq, args.device_)  # dim * dim
         self.wk_: Linear = Linear(wk, args.device_)  # dim * dim
         self.wv_: Linear = Linear(wv, args.device_)  # dim * dim
         self.wo_: Linear = Linear(wo, args.device_)  # dim * dim
         # cos and sin
         self.cos_, self.sin_ = precompute_rope_angle(
             args.dim_ // args.n_heads_, args.max_seq_len_, args.rope_theta_, args.device_)
         # config
-        self.layer_id_ = layer_idx
         self.dim_ = args.dim_
         self.n_heads_ = args.n_heads_
         self.n_kv_heads_ = args.n_kv_heads_
         self.n_rep_ = self.n_heads_ // self.n_kv_heads_
         self.head_dim_ = args.dim_ // args.n_heads_
         self.dtype_ = args.dtype_
         self.is_causal_ = True
@@ -107,18 +105,17 @@
         attention_score = attention_score.reshape(batch_size, max_seq_len, -1)
 
         # get output attention score
         return self.wo_.forward(attention_score, input_args)
 
 
 class LlamaXformersAttention(LlamaAttention):
-    def __init__(self, wq: nn.Module, wk: nn.Module, wv: nn.Module, wo: nn.Module,
-                 layer_idx: int, args: LlamaConfig):
+    def __init__(self, wq: nn.Module, wk: nn.Module, wv: nn.Module, wo: nn.Module, args: LlamaConfig):
         assert _xformers_available, "xFormers Attention is not available"
-        super().__init__(wq, wk, wv, wo, layer_idx, args)
+        super().__init__(wq, wk, wv, wo, args)
 
     def forward(self,
                 hidden_states: torch.Tensor,
                 input_args: MultiLoraBatchData,
                 attention_mask: Optional[torch.Tensor] = None):
         batch_size, max_seq_len, _ = hidden_states.shape
 
@@ -150,18 +147,17 @@
         attention_score = attention_score.reshape(batch_size, max_seq_len, -1)
 
         # get output attention score
         return self.wo_.forward(attention_score, input_args)
 
 
 class LlamaFlashAttention(LlamaAttention):
-    def __init__(self, wq: nn.Module, wk: nn.Module, wv: nn.Module, wo: nn.Module,
-                 layer_idx: int, args: LlamaConfig):
+    def __init__(self, wq: nn.Module, wk: nn.Module, wv: nn.Module, wo: nn.Module, args: LlamaConfig):
         assert _flash_attn_available, "Flash Attention is not available"
-        super().__init__(wq, wk, wv, wo, layer_idx, args)
+        super().__init__(wq, wk, wv, wo, args)
 
     def _flash_attention_forward(
         self, query_states, key_states, value_states, attention_mask, query_length, dropout=0.0, softmax_scale=None
     ):
 
         # Contains at least one padding token in the sequence
         if attention_mask is not None:
@@ -351,46 +347,46 @@
         v = data.to(torch.float32).pow(2).mean(-1, keepdim=True)
         data = data * torch.rsqrt(v + self.norm_eps_)
 
         return (self.weight_ * data).to(input_dtype)
 
 
 class LlamaDecoderLayer(LLMDecoder):
-    def __init__(self) -> None:
+    def __init__(self, layer_id: int) -> None:
         super().__init__()
-        self.layer_id_: int = None
+        self.layer_id_: int = layer_id
         self.self_attn_: LlamaAttention = None
         self.mlp_: FeedForward = None
         self.input_layernorm_: LlamaRMSNorm = None
         self.post_attention_layernorm_: LlamaRMSNorm = None
 
     def state_dict(self) -> Dict[str, nn.Module]:
         linear_layers = self.self_attn_.state_dict()
         linear_layers.update(self.mlp_.state_dict())
         return linear_layers
 
     def forward(self,
                 hidden_states: torch.Tensor,
-                input_args: MultiLoraBatchData,
-                attention_mask: Optional[torch.Tensor] = None,
-                router_logits: Optional[List[List]] = None):
+                attention_mask: torch.Tensor,
+                input_args: MultiLoraBatchData):
+
         residual = hidden_states
         hidden_states = self.input_layernorm_(hidden_states)
         # Self Attention
         hidden_states = self.self_attn_.forward(
             hidden_states, input_args, attention_mask)
         hidden_states = residual + hidden_states
         # Fully Connected
         residual = hidden_states
         hidden_states = self.post_attention_layernorm_(hidden_states)
-        hidden_states = self.mlp_.forward(
-            hidden_states, input_args, router_logits)
+        hidden_states, router_logits = self.mlp_.forward(
+            hidden_states, input_args)
         hidden_states = residual + hidden_states
 
-        return hidden_states
+        return hidden_states, *router_logits
 
 
 class LlamaEmbedding(nn.Module):
     def __init__(self, embedding: torch.Tensor, pad_token: int):
         super().__init__()
         self.token_embedding_: torch.Tensor = embedding
         self.padding_idx_: int = pad_token
@@ -410,27 +406,26 @@
         return type(self.wrapper_module_).__name__
 
     def forward(self, input: Tuple) -> Tuple:
         module_name = self.name()
 
         if module_name == "LlamaEmbedding":
             output = self.wrapper_module_.forward(input[0])
-            if input[-1]:
+            if input[-1].gradient_checkpoint_ != "none":
                 output = output.requires_grad_(True)
-            return (output, ) + input[1:]
+            return (output,) + input[1:]
         elif module_name == "LlamaRMSNorm":
             output = self.wrapper_module_.forward(input[0])
-            return (output, ) + input[1:]
+            return (output,) + input[1:]
         elif module_name == "LlamaDecoderLayer":
-            if input[-1]:
-                output = CheckpointFunction.apply(
-                    self.wrapper_module_.forward, *input[:-1])
-            else:
-                output = self.wrapper_module_.forward(*input[:-1])
-            return (output, ) + input[1:]
+            outputs = CHECKPOINT_CLASSES[input[-1].gradient_checkpoint_](
+                self.wrapper_module_.forward, *input)
+            if len(outputs) > 1:
+                self.router_probs_ = outputs[1:]
+            return (outputs[0],) + input[1:]
         else:
             raise f"module invalid: {module_name}"
 
 
 class LlamaForCausalLM(LLMForCausalLM):
     def __init__(self, config: LlamaConfig) -> None:
         self.config_ = config
@@ -485,14 +480,15 @@
                         device: str = get_backend().device_name() + ":0"):
         assert not use_sliding_window, "Llama model does not support SWA."
         llm_config: modeling_llama.LlamaConfig = llm_model.config
         llm_args = LlamaConfig(
             name_or_path_=llm_config.name_or_path,
             vocab_size_=llm_config.vocab_size,
             dim_=llm_config.hidden_size,
+            intermediate_=llm_config.intermediate_size,
             n_layers_=llm_config.num_hidden_layers,
             n_heads_=llm_config.num_attention_heads,
             n_kv_heads_=llm_config.num_key_value_heads,
             hidden_act_=llm_config.hidden_act,
             rms_norm_eps_=llm_config.rms_norm_eps,
             max_seq_len_=llm_config.max_position_embeddings,
             rope_theta_=llm_config.rope_theta,
@@ -510,22 +506,20 @@
         model.embed_tokens_ = LlamaEmbedding(
             llm_model.model.embed_tokens.weight, llm_args.pad_token_id_)
         model.norm_ = LlamaRMSNorm(
             llm_model.model.norm.weight, llm_args.rms_norm_eps_)
         copy_parameters(llm_model.lm_head, model.lm_head_)
 
         for idx, layer in enumerate(llm_model.model.layers):
-            decoder = LlamaDecoderLayer()
-            decoder.layer_id_ = idx
+            decoder = LlamaDecoderLayer(idx)
             decoder.self_attn_ = LLAMA_ATTENTION_CLASSES[llm_args.attn_implementation_](
                 layer.self_attn.q_proj,
                 layer.self_attn.k_proj,
                 layer.self_attn.v_proj,
                 layer.self_attn.o_proj,
-                idx,
                 llm_args,
             )
             decoder.mlp_ = FeedForward(LlamaMLP(
                 layer.mlp.gate_proj,
                 layer.mlp.down_proj,
                 layer.mlp.up_proj,
                 llm_args,
```

### Comparing `mlora-0.3.0.post1/mlora/models/modeling_mistral.py` & `mlora-0.3.1/mlora/models/modeling_mistral.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,18 +36,17 @@
 class MistralConfig(LlamaConfig):
     use_sliding_window_: bool = False
     max_window_layers_: int = None
     sliding_window_: int = None
 
 
 class MistralFlashAttention(LlamaAttention):
-    def __init__(self, wq: nn.Module, wk: nn.Module, wv: nn.Module, wo: nn.Module,
-                 layer_idx: int, args: MistralConfig):
+    def __init__(self, wq: nn.Module, wk: nn.Module, wv: nn.Module, wo: nn.Module, args: MistralConfig):
         assert _flash_attn_available, "Flash Attention is not available"
-        super().__init__(wq, wk, wv, wo, layer_idx, args)
+        super().__init__(wq, wk, wv, wo, args)
         # Qwen2
         self.use_sliding_window_ = args.use_sliding_window_
         self.max_window_layers_ = args.max_window_layers_
         # Mistral and Qwen2
         self.sliding_window_ = args.sliding_window_
 
     def _flash_attention_forward(
@@ -257,14 +256,15 @@
                         use_sliding_window: bool = False,
                         device: str = get_backend().device_name() + ":0"):
         llm_config: modeling_mistral.MistralConfig = llm_model.config
         llm_args = MistralConfig(
             name_or_path_=llm_config.name_or_path,
             vocab_size_=llm_config.vocab_size,
             dim_=llm_config.hidden_size,
+            intermediate_=llm_config.intermediate_size,
             n_layers_=llm_config.num_hidden_layers,
             n_heads_=llm_config.num_attention_heads,
             n_kv_heads_=llm_config.num_key_value_heads,
             hidden_act_=llm_config.hidden_act,
             rms_norm_eps_=llm_config.rms_norm_eps,
             max_seq_len_=llm_config.max_position_embeddings,
             rope_theta_=llm_config.rope_theta,
@@ -292,22 +292,20 @@
         model.embed_tokens_ = LlamaEmbedding(
             llm_model.model.embed_tokens.weight, llm_args.pad_token_id_)
         model.norm_ = LlamaRMSNorm(
             llm_model.model.norm.weight, llm_args.rms_norm_eps_)
         copy_parameters(llm_model.lm_head, model.lm_head_)
 
         for idx, layer in enumerate(llm_model.model.layers):
-            decoder = LlamaDecoderLayer()
-            decoder.layer_id_ = idx
+            decoder = LlamaDecoderLayer(idx)
             decoder.self_attn_ = MISTRAL_ATTENTION_CLASSES[llm_args.attn_implementation_](
                 layer.self_attn.q_proj,
                 layer.self_attn.k_proj,
                 layer.self_attn.v_proj,
                 layer.self_attn.o_proj,
-                idx,
                 llm_args,
             )
             decoder.mlp_ = FeedForward(LlamaMLP(
                 layer.mlp.gate_proj,
                 layer.mlp.down_proj,
                 layer.mlp.up_proj,
                 llm_args,
```

### Comparing `mlora-0.3.0.post1/mlora/models/modeling_phi.py` & `mlora-0.3.1/mlora/models/modeling_phi.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     apply_rotary_emb,
     get_unpad_data,
     repeat_kv,
     Masks,
     Linear,
     FeedForward,
     MultiLoraBatchData,
-    CheckpointRecomputeFunction as CheckpointFunction,
+    CHECKPOINT_CLASSES,
     LLMModelArgs,
     LLMAttention,
     LLMFeedForward,
     LLMDecoder,
     LLMForCausalLM,
 )
 from mlora.backends import _backend, get_backend
@@ -65,24 +65,22 @@
     xk = torch.cat((k_rot, k_pass), dim=-1)
 
     return xq, xk
 
 
 # Multi-headed attention from 'Attention Is All You Need' paper.
 class PhiAttention(LLMAttention):
-    def __init__(self, q_proj: nn.Module, k_proj: nn.Module, v_proj: nn.Module, dense: nn.Module,
-                 layer_idx: int, args: PhiConfig):
+    def __init__(self, q_proj: nn.Module, k_proj: nn.Module, v_proj: nn.Module, dense: nn.Module, args: PhiConfig):
         super().__init__()
         # attention
         self.wq_: Linear = Linear(q_proj, args.device_)
         self.wk_: Linear = Linear(k_proj, args.device_)
         self.wv_: Linear = Linear(v_proj, args.device_)
         self.dense_: Linear = Linear(dense, args.device_)
         # config
-        self.layer_id_ = layer_idx
         self.dim_ = args.dim_
         self.n_heads_ = args.n_heads_
         self.n_kv_heads_ = args.n_kv_heads_
         self.n_rep_ = self.n_heads_ // self.n_kv_heads_
         self.head_dim_ = args.dim_ // args.n_heads_
         self.dtype_ = args.dtype_
         self.is_causal_ = True
@@ -149,18 +147,17 @@
         attention_score = attention_score.reshape(batch_size, max_seq_len, -1)
         attention_score = self.dense_.forward(attention_score, input_args)
 
         return attention_score
 
 
 class PhiXformersAttention(PhiAttention):
-    def __init__(self, q_proj: nn.Module, k_proj: nn.Module, v_proj: nn.Module, dense: nn.Module,
-                 layer_idx: int, args: PhiConfig):
+    def __init__(self, q_proj: nn.Module, k_proj: nn.Module, v_proj: nn.Module, dense: nn.Module, args: PhiConfig):
         assert _xformers_available, "xFormers Attention is not available"
-        super().__init__(q_proj, k_proj, v_proj, dense, layer_idx, args)
+        super().__init__(q_proj, k_proj, v_proj, dense, args)
 
     def forward(self,
                 hidden_states: torch.Tensor,
                 input_args: MultiLoraBatchData,
                 attention_mask: Optional[torch.Tensor] = None):
         batch_size, max_seq_len, _ = hidden_states.shape
 
@@ -195,18 +192,17 @@
         attention_score = attention_score.reshape(batch_size, max_seq_len, -1)
         attention_score = self.dense_.forward(attention_score, input_args)
 
         return attention_score
 
 
 class PhiFlashAttention2(PhiAttention):
-    def __init__(self, q_proj: nn.Module, k_proj: nn.Module, v_proj: nn.Module, dense: nn.Module,
-                 layer_idx: int, args: PhiConfig):
+    def __init__(self, q_proj: nn.Module, k_proj: nn.Module, v_proj: nn.Module, dense: nn.Module, args: PhiConfig):
         assert _flash_attn_available, "Flash Attention is not available"
-        super().__init__(q_proj, k_proj, v_proj, dense, layer_idx, args)
+        super().__init__(q_proj, k_proj, v_proj, dense, args)
 
     def _flash_attention_forward(
         self, query_states, key_states, value_states, attention_mask, query_length, dropout=0.0, softmax_scale=None
     ):
 
         # Contains at least one padding token in the sequence
         if attention_mask is not None:
@@ -381,48 +377,47 @@
         else:
             hidden_states = self.fc2_.base_layer_.forward(hidden_states)
 
         return hidden_states
 
 
 class PhiDecoderLayer(LLMDecoder):
-    def __init__(self, self_attn: LLMAttention, mlp: FeedForward, args: PhiConfig) -> None:
+    def __init__(self, layer_id: int, self_attn: LLMAttention, mlp: FeedForward, args: PhiConfig) -> None:
         super().__init__()
-        self.layer_id_: int = self_attn.layer_id_
+        self.layer_id_: int = layer_id
         self.self_attn_ = self_attn
         self.mlp_ = mlp
         self.input_layernorm_ = nn.LayerNorm(
             args.dim_, eps=args.layer_norm_eps_, dtype=args.dtype_, device=args.device_)
         self.resid_pdrop_ = args.resid_pdrop_
 
     def state_dict(self) -> Dict[str, nn.Module]:
         linear_layers = self.self_attn_.state_dict()
         linear_layers.update(self.mlp_.state_dict())
         return linear_layers
 
     def forward(self,
                 hidden_states: torch.Tensor,
-                input_args: MultiLoraBatchData,
-                attention_mask: Optional[torch.Tensor] = None,
-                router_logits: Optional[List[List]] = None):
+                attention_mask: torch.Tensor,
+                input_args: MultiLoraBatchData):
         residual = hidden_states
         hidden_states = self.input_layernorm_(hidden_states)
         # Self Attention
         attn_outputs = self.self_attn_.forward(
             hidden_states, input_args, attention_mask)
         attn_outputs = F.dropout(
             attn_outputs, self.resid_pdrop_, not input_args.inference_mode_)
         # Fully Connected
-        feed_forward_outputs = self.mlp_.forward(
-            hidden_states, input_args, router_logits)
+        feed_forward_outputs, router_logits = self.mlp_.forward(
+            hidden_states, input_args)
         feed_forward_outputs = F.dropout(
             feed_forward_outputs, self.resid_pdrop_, not input_args.inference_mode_)
         hidden_states = attn_outputs + feed_forward_outputs + residual
 
-        return hidden_states
+        return hidden_states, *router_logits
 
 
 class PhiEmbedding(nn.Module):
     def __init__(self, config: PhiConfig):
         super().__init__()
         self.embed_tokens = nn.Embedding(config.vocab_size_, config.dim_, config.pad_token_id_,
                                          dtype=config.dtype_, device=config.device_)
@@ -452,27 +447,26 @@
         return type(self.wrapper_module_).__name__
 
     def forward(self, input: Tuple) -> Tuple:
         module_name = self.name()
 
         if module_name == "PhiEmbedding":
             output = self.wrapper_module_.forward(input[0])
-            if input[-1]:
+            if input[-1].gradient_checkpoint_ != "none":
                 output = output.requires_grad_(True)
-            return (output, ) + input[1:]
+            return (output,) + input[1:]
         elif module_name == "PhiLayerNorm":
             output = self.wrapper_module_.forward(input[0])
-            return (output, ) + input[1:]
+            return (output,) + input[1:]
         elif module_name == "PhiDecoderLayer":
-            if input[-1]:
-                output = CheckpointFunction.apply(
-                    self.wrapper_module_.forward, *input[:-1])
-            else:
-                output = self.wrapper_module_.forward(*input[:-1])
-            return (output, ) + input[1:]
+            outputs = CHECKPOINT_CLASSES[input[-1].gradient_checkpoint_](
+                self.wrapper_module_.forward, *input)
+            if len(outputs) > 1:
+                self.router_probs_ = outputs[1:]
+            return (outputs[0],) + input[1:]
         else:
             raise f"module invalid: {module_name}"
 
 
 class PhiForCausalLM(LLMForCausalLM):
     def __init__(self, config: PhiConfig) -> None:
         self.config_ = config
@@ -527,14 +521,15 @@
                         device: str = get_backend().device_name() + ":0"):
         assert not use_sliding_window, "Phi model does not support SWA."
         llm_config: modeling_phi.PhiConfig = llm_model.config
         llm_args = PhiConfig(
             name_or_path_=llm_config.name_or_path,
             vocab_size_=llm_config.vocab_size,
             dim_=llm_config.hidden_size,
+            intermediate_=llm_config.intermediate_size,
             n_layers_=llm_config.num_hidden_layers,
             n_heads_=llm_config.num_attention_heads,
             n_kv_heads_=llm_config.num_key_value_heads,
             hidden_act_=llm_config.hidden_act,
             resid_pdrop_=llm_config.resid_pdrop,
             embd_pdrop_=llm_config.embd_pdrop,
             max_seq_len_=llm_config.max_position_embeddings,
@@ -558,20 +553,20 @@
         copy_parameters(llm_model.model.final_layernorm,
                         model.final_layernorm_.layernorm_)
         copy_parameters(llm_model.lm_head,
                         model.lm_head_)
 
         for idx, layer in enumerate(llm_model.model.layers):
             decoder = PhiDecoderLayer(
+                idx,
                 PHI_ATTENTION_CLASSES[llm_args.attn_implementation_](
                     layer.self_attn.q_proj,
                     layer.self_attn.k_proj,
                     layer.self_attn.v_proj,
                     layer.self_attn.dense,
-                    idx,
                     llm_args,
                 ),
                 FeedForward(PhiMLP(
                     layer.mlp.fc1,
                     layer.mlp.fc2,
                     llm_args,
                 )),
```

### Comparing `mlora-0.3.0.post1/mlora/prompter.py` & `mlora-0.3.1/mlora/prompter.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0.post1/mlora/tasks/__init__.py` & `mlora-0.3.1/mlora/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0.post1/mlora/tasks/common.py` & `mlora-0.3.1/mlora/tasks/common.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0.post1/mlora/tasks/glue_tasks.py` & `mlora-0.3.1/mlora/tasks/glue_tasks.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0.post1/mlora/tokenizer.py` & `mlora-0.3.1/mlora/tokenizer.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,22 +11,28 @@
         self.tokenizer = AutoTokenizer.from_pretrained(model_path)
         self.vocab_size_ = self.tokenizer.vocab_size
         self.bos_id_ = self.tokenizer.bos_token_id
         self.eos_id_ = self.tokenizer.eos_token_id
         self.pad_id_ = self.tokenizer.pad_token_id
         self.unk_id_ = self.tokenizer.unk_token_id
         # maybe pad id is unk
-        if self.pad_id_ is None and self.unk_id_ is not None:
+        if self.pad_id_ is not None:
+            return
+        if self.unk_id_ is None and self.eos_id_ is None:
+            logging.warn(
+                "Detecting <eos> and <unk> are None, setting <pad> to 0 by default.")
+            self.pad_id_ = 0
+        elif self.unk_id_ is not None:
+            logging.warn(
+                "Detecting <pad> is None, setting to <unk> by default.")
             self.pad_id_ = self.unk_id_
-        if self.pad_id_ is None and self.eos_id_ is not None:
+        elif self.eos_id_ is not None:
+            logging.warn(
+                "Detecting <pad> is None, setting to <eos> by default.")
             self.pad_id_ = self.eos_id_
-            logging.warn("Padding token ID is None, setting to <eos>.")
-        else:
-            raise ValueError(
-                "Can not set padding token id. <eos> and <unk> are None.")
 
     def encode(self, data: Union[str, List[str]], add_special_tokens: bool = True) -> Tokens:
         if isinstance(data, str):
             data = [data]
         tokens = []
         ret = self.tokenizer(
             data, add_special_tokens=add_special_tokens, return_attention_mask=False).input_ids
```

### Comparing `mlora-0.3.0.post1/mlora/trainer.py` & `mlora-0.3.1/mlora/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,19 +152,19 @@
         config.prepare_lr_scheduler(
             task.total_epoch_num_, len(task.train_token_data_))
 
     dispatcher.train_task_in_event_.register(task_in_callback)
 
     step_cnt = 0
     while not dispatcher.check_task_done():
-        labels, input = dispatcher.get_train_data()
+        input_args = dispatcher.get_train_data()
 
         step_cnt += 1
 
-        outputs = model.forward(input, labels)
+        outputs = model.forward(input_args)
 
         total_loss = None
         for output in outputs:
             adapter_name = output.adapter_name
             loss = output.loss / config_dict[adapter_name].accumulation_step_
             logging.info(
                 f"    adapter: {adapter_name} loss: {loss}")
```

### Comparing `mlora-0.3.0.post1/mlora/utils.py` & `mlora-0.3.1/mlora/utils.py`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0.post1/mlora.egg-info/PKG-INFO` & `mlora-0.3.1/mlora.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlora
-Version: 0.3.0.post1
+Version: 0.3.1
 Summary: A tool for fine-tuning large language models (LLMs) using the LoRA or QLoRA methods more efficiently.
 Project-URL: Homepage, https://github.com/scukdde-llm/mlora
 Project-URL: Bug Tracker, https://github.com/scukdde-llm/mlora/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `mlora-0.3.0.post1/mlora.egg-info/SOURCES.txt` & `mlora-0.3.1/mlora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlora-0.3.0.post1/pyproject.toml` & `mlora-0.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlora"
-version = "0.3.0.post1"
+version = "0.3.1"
 description = "A tool for fine-tuning large language models (LLMs) using the LoRA or QLoRA methods more efficiently."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
```

