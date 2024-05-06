# Comparing `tmp/short_transformers-0.2.0.tar.gz` & `tmp/short_transformers-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "short_transformers-0.2.0.tar", max compression
+gzip compressed data, was "short_transformers-0.3.0.tar", max compression
```

## Comparing `short_transformers-0.2.0.tar` & `short_transformers-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     4986 2024-05-04 22:43:54.503553 short_transformers-0.2.0/README.md
--rw-r--r--   0        0        0      379 2024-05-05 07:31:37.664285 short_transformers-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       98 2024-05-04 22:49:29.887096 short_transformers-0.2.0/short_transformers/__init__.py
--rw-r--r--   0        0        0      748 2024-05-04 09:18:55.749638 short_transformers-0.2.0/short_transformers/dist.py
--rw-r--r--   0        0        0      945 2024-05-04 22:49:29.887096 short_transformers-0.2.0/short_transformers/graph.py
--rw-r--r--   0        0        0      529 2024-05-04 22:49:29.887096 short_transformers-0.2.0/short_transformers/log.py
--rw-r--r--   0        0        0     8463 2024-05-04 22:50:54.290980 short_transformers-0.2.0/short_transformers/short_transformer.py
--rw-r--r--   0        0        0       76 2024-05-04 20:32:31.974305 short_transformers-0.2.0/short_transformers/utils.py
--rw-r--r--   0        0        0     5598 1970-01-01 00:00:00.000000 short_transformers-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4631 2024-05-05 10:50:38.907960 short_transformers-0.3.0/README.md
+-rw-r--r--   0        0        0      379 2024-05-05 11:10:11.698358 short_transformers-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       98 2024-05-04 22:49:29.887096 short_transformers-0.3.0/short_transformers/__init__.py
+-rw-r--r--   0        0        0      748 2024-05-04 09:18:55.749638 short_transformers-0.3.0/short_transformers/dist.py
+-rw-r--r--   0        0        0     7004 2024-05-05 11:08:35.650489 short_transformers-0.3.0/short_transformers/short_transformer.py
+-rw-r--r--   0        0        0      281 2024-05-05 10:42:13.996656 short_transformers-0.3.0/short_transformers/utils/__init__.py
+-rw-r--r--   0        0        0      529 2024-05-04 22:49:29.887096 short_transformers-0.3.0/short_transformers/utils/log.py
+-rw-r--r--   0        0        0      965 2024-05-05 10:54:41.243629 short_transformers-0.3.0/short_transformers/utils/plot.py
+-rw-r--r--   0        0        0     1200 2024-05-05 10:51:18.167907 short_transformers-0.3.0/short_transformers/utils/utils.py
+-rw-r--r--   0        0        0     5243 1970-01-01 00:00:00.000000 short_transformers-0.3.0/PKG-INFO
```

### Comparing `short_transformers-0.2.0/README.md` & `short_transformers-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,103 @@
 # :scissors: Short Transformers
 
-- Pytorch implementation of layer pruning proposed in [The Unreasonable Ineffectiveness of the Deeper Layers](https://arxiv.org/pdf/2403.17887.pdf).
+- [Unofficial] Pytorch implementation of layer pruning proposed in [The Unreasonable Ineffectiveness of the Deeper Layers](https://arxiv.org/pdf/2403.17887.pdf).
 - The repository reproduces and extends original methods by offering different layer pruning criteria.
 
 <p align="center">
-<img src="./docs/memory.png" align="center" width='300'/>
+<img src="./docs/merged.png" align="center" alt="Normalized angular distance from initial layer l (x-axis) with block size n (y-axis)." height='250'/>
 </p>
 
+
 [![pypi Version](https://img.shields.io/pypi/v/short-transformers.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/short-transformers/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 ## Installation:
 ```sh
 pip install short-transformers
 ```
 
 Required additional dependencies: `transformers`, `datasets`.
 
 ## Quickstart:
 ```python
 from short_transformers import ShortTransformer
+from datasets import load_dataset
 
 # load from path/hf_hub
 model = ShortTransformer.from_pretrained(model_name)
 
 # or use hf model
-model = ShortTransformer.from_model(hf_model)
+# model = ShortTransformer.from_model(hf_model)
 
-# remove n layers, use hf dataset to find the optimal cut
+# load hf dataset
+dataset = load_dataset("allenai/c4", "en", split="validation", streaming=True)
+
+# remove 5 layers, use the dataset to find the least important layers to remove
 short_model = model.remove_layers(block_size=5, dataset=dataset, limit=1000)
 
 # continue training to heal after the cut
 # ...
 
 # save as hf model
 short_mdoel.save_pretrained(output_path)
 ```
-Example log output:
-```sh
-[2024-05-04 18:39:03] [short-transformers] Running inference on 1000 samples.
-1000it [00:06, ?it/s]
-[2024-05-04 18:39:09] [short-transformers] Inference results saved to `model.memory`.
-[2024-05-04 18:39:09] [short-transformers] Choosing optimal 5-layers block to prune.
-[2024-05-04 18:39:09] [short-transformers] Best 5-layers block to prune starts at layer: 23.
-[2024-05-04 18:39:09] [short-transformers] Removing layers: [23, 24, 25, 26, 27]
-[2024-05-04 18:39:09] [short-transformers] Changing model config to reflect changes:
-        config.num_hidden_layers: 32 -> 27
-        config._name_or_path: meta-llama/Meta-Llama-3-8B -> meta-llama/Meta-Llama-3-8B-27L
-[2024-05-04 18:39:09] [short-transformers] Cleaning `model.memory`.
-```
 
 Both `short_model` and the saved model are fully compatible with transformers. See `examples/basic.py` for a complete working example.
 
 ## Pruning in steps:
 
 Pruning can composed step-by-step and customized:
 
 1. Analyze model layers:
 ```python
 from datasets import load_dataset
 from short_transformers import ShortTransformer
-from short_transformers.graph import draw_diagram
-
+from short_transformers.utils import (
+    draw_diagram,
+    get_scored_blocks,
+    get_best_pruning_start,
+)
 # load from path/hf_hub
 model_name = "meta-llama/Meta-Llama-3-8B"
 
 model = ShortTransformer.from_pretrained(model_name, device_map="auto")
 
 dataset = load_dataset("allenai/c4", "en", split="validation", streaming=True)
 
-# run inderence on a subset of the datsets
-model.analyse_layers(
+# calculate distances between inputs/outputs from/to model layers
+# results in a triangular numpy array of shape (layer_count, layer_count)
+# results[x, y] - averaged distances for block of size x starting at layer y
+results = model.analyse_layers(
     dataset=dataset,
     key="text",
     limit=100,
     max_length=1000,
 )
 
-# after this step, results will be saved to model.memory, which can be saved
-model.save_memory("memory.npz")
-
-# and visualized as seaborh graph (see examples in the README.md)
-draw_diagram("memory.npz", "memory.png")
+# draw results
+# diagrams style matches the style of original article
+# "The Unreasonable Ineffectiveness of the Deeper Layers"
+draw_diagram(results, "results.png", title="Meta-Llama-3-8B")
 ```
 
 Example output:
 <p align="center">
-<img src="./docs/memory.png" align="center" width='300'/>
+<img src="./docs/Meta-Llama-3-8B.png" align="center" width='300'/>
 </p>
 
-2. Find optimal block size and start_layer:
+2. Find optimal `block_size` and `start_layer`:
 ```python
-# finding optimial block of size 'num' to prune
-start_layer = model.get_optimal_cut(block_size=5)
+# find optimial block of size 'block_size' to prune
+start_layer = get_best_pruning_start(results, block_size=5)
 
-# evaluating all possibe block sizes to prune,
+# evaluate all possibe block sizes to prune,
 # for each block returns score 0-1
 # which is averaged over samples distance between input and output to/from a block
-block_score = model.get_block_score_stats(return_md=True, threshold=0.3)
+block_score = get_scored_blocks(results, return_md=True, threshold=0.3)
 ```
 
 Example output:
 
 | Block_size | Removed_layers | Score (avg dist)|
 | -------- | ------- | -------- |
 | 1 | 25-25 | 0.123|
@@ -112,23 +108,19 @@
 | 6 | 22-27 | 0.248|
 | 7 | 22-28 | 0.268|
 | 8 | 20-27 | 0.291|
 
 
 3. Pruning layers:
 ```python
-# pruning 5-layers block
-# this will also clean the `model.memory``
-model.cut(start_layer=start_layer, block_size=5)
-
-# or clean the model memory manually
-model.clean_memory()
+# prune 5-layers block
+model.prune(start_layer=start_layer, block_size=5)
 
 # save the pruned model
-model.save_pretrained("model_path")
+model.save_pretrained("model_output_dir")
 ```
 
 See `example/prune_in_steps.py` for a complete working example.
 
 
 ## Supported pruning methods:
 - based on layer input/output distances:
```

### Comparing `short_transformers-0.2.0/short_transformers/dist.py` & `short_transformers-0.3.0/short_transformers/dist.py`

 * *Files identical despite different names*

### Comparing `short_transformers-0.2.0/short_transformers/graph.py` & `short_transformers-0.3.0/short_transformers/utils/plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import matplotlib.pylab as plt
 import numpy as np
 import seaborn as sns
 
 
-def draw_diagram(input_file_path, output_file_path, title=None):
+def draw_diagram(results, output_file_path, title=None):
     plt.clf()
 
-    result = np.load(input_file_path)["arr_0"]
-    mask = np.zeros_like(result)
+    mask = np.zeros_like(results)
     mask[np.triu_indices_from(mask, k=1)] = True
     mask = np.flip(mask, axis=0)
 
     # @TODO make row-wise normalization optional
     # rescale scores to 0-1 for each cut_layers value
-    masked_result = np.ma.masked_array(result, mask)
-    max_dist = np.ma.max(masked_result, axis=1)[:, np.newaxis]
-    min_dist = np.ma.min(masked_result, axis=1)[:, np.newaxis]
+    masked_results = np.ma.masked_array(results, mask)
+    max_dist = np.ma.max(masked_results, axis=1)[:, np.newaxis]
+    min_dist = np.ma.min(masked_results, axis=1)[:, np.newaxis]
 
-    result = (result - min_dist) / (max_dist - min_dist)
+    results = (results - min_dist) / (max_dist - min_dist)
 
-    ax = sns.heatmap(result, linewidth=0.5, mask=mask, cmap="viridis_r")
+    ax = sns.heatmap(results, linewidth=0.5, mask=mask, cmap="viridis_r")
     ax.invert_yaxis()
     ax.set_xticklabels(ax.get_xticklabels(), ha="left")
     ax.set_yticklabels(ax.get_yticklabels(), va="bottom")
 
+    plt.xlabel("Layer number, l")
+    plt.ylabel("Block size, n")
+
     if title:
         ax.set_title(title)
 
     plt.savefig(output_file_path)
```

### Comparing `short_transformers-0.2.0/short_transformers/log.py` & `short_transformers-0.3.0/short_transformers/utils/log.py`

 * *Files identical despite different names*

### Comparing `short_transformers-0.2.0/short_transformers/short_transformer.py` & `short_transformers-0.3.0/short_transformers/short_transformer.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,80 +5,73 @@
 from tqdm import tqdm
 from transformers import AutoModelForCausalLM, AutoTokenizer, PreTrainedModel
 
 from short_transformers.dist import (
     angular_distance_all_tokens,
     angular_distance_last_token,
 )
-from short_transformers.log import get_logger
+from short_transformers.utils import (
+    get_best_pruning_start,
+    get_logger
+)
 
 logger = get_logger("short-transformers", debug=True)
 
 
 class Memory:
     def __init__(self, layer_count: int):
         self.examples_count: int = -1
         self.result = np.zeros((layer_count, layer_count))
         self.layers_outputs: dict = {}
 
-    def save(self, file_path: str) -> None:
-        np.savez(file_path, self.result)
-
 
 class ShortTransformer(PreTrainedModel):
+    default_io_distance = angular_distance_last_token
+
     @classmethod
     def from_model(cls, model):
         cls = model
-
-        # add memory for storing intermediate layers outputs
         cls.layer_count = len(cls.model.layers)
 
+        # add memory for storing intermediate layers outputs
         cls.memory = Memory(cls.layer_count)
 
         # @TODO add distances here
         # @TODO auto assign all methods from the class here
         cls.clear_memory = partial(ShortTransformer.clear_memory, cls)
-        cls.save_memory = partial(ShortTransformer.save_memory, cls.memory)
         cls.analyse_layers = partial(ShortTransformer.analyse_layers, cls)
-        cls.get_optimal_cut = partial(ShortTransformer.get_optimal_cut, cls)
-        cls.cut = partial(ShortTransformer.cut, cls)
+        cls.prune = partial(ShortTransformer.prune, cls)
         cls.remove_layers = partial(ShortTransformer.remove_layers, cls)
-        cls.get_block_score_stats = partial(ShortTransformer.get_block_score_stats, cls)
 
         # add decorators to each forward in layers
         for layer_idx, layer in enumerate(cls.model.layers):
-            layer.forward = ShortTransformer._layer_io(cls.memory, layer_idx)(
-                layer.forward
-            )
+            layer.forward = ShortTransformer._layer_io(
+                cls.memory, layer_idx, ShortTransformer.default_io_distance
+            )(layer.forward)
 
         return cls
 
     @classmethod
     def from_pretrained(cls, *args, **kw):
         # @TODO: support other AutoModels variants
         model = AutoModelForCausalLM.from_pretrained(*args, **kw)
         return cls.from_model(model)
 
     @staticmethod
     def clear_memory(model) -> None:
-        logger.debug("Cleaning `model.memory`.")
         model.memory = Memory(model.layer_count)
 
     @staticmethod
-    def save_memory(memory, file_path):
-        logger.debug(f"Saving `model.memory` to {file_path}.")
-        memory.save(file_path)
-
-    @staticmethod
-    def _layer_io(memory, layer_idx: int):
+    def _layer_io(memory, layer_idx: int, io_distance):
         def decorator(f):
             @wraps(f)
             def wrap(*args, **kw):
                 nonlocal memory
                 nonlocal layer_idx
+                nonlocal io_distance
 
                 input_hidden_states = args[0]
 
                 if layer_idx == 0:
                     # clear the memory of previous example outputs and remmeber the input
                     memory.layers_outputs = {
                         -1: torch.clone(input_hidden_states).to("cpu")
@@ -89,15 +82,15 @@
                 result = f(*args, **kw)
 
                 # calculate io metric for all layers:
                 output_hidden_states = torch.clone(result[0]).to("cpu")
 
                 # calculate scores from -1 to this layer:
                 for k, v in memory.layers_outputs.items():
-                    dist = angular_distance_last_token(v, output_hidden_states)
+                    dist = io_distance(v, output_hidden_states)
 
                     cut_layers = layer_idx - k - 1
 
                     memory.result[cut_layers, k + 1] = (
                         memory.result[cut_layers, k + 1] * memory.examples_count + dist
                     ) / (memory.examples_count + 1)
 
@@ -107,14 +100,18 @@
                 )
                 return result
 
             return wrap
 
         return decorator
 
+    # @TODO
+    # @staticmethod
+    # def set_pruning_criterion(model, criterion_callable):
+
     @staticmethod
     def analyse_layers(
         model,
         dataset,
         tokenizer=None,
         key: str = "content",
         limit: int = 1,
@@ -124,15 +121,15 @@
             logger.debug(
                 "Tokenizer not provided, will load tokenizer from config._name_or_path"
             )
             try:
                 tokenizer = AutoTokenizer.from_pretrained(model.config._name_or_path)
             except Exception as e:
                 logger.error(
-                    "Loading the tokenizer failed wwth error: {e}.\nUse analyse_layers(... tokenizer=...) to manually set the tokenizer."
+                    f"Loading the tokenizer failed wwth error: {e}.\nUse analyse_layers(... tokenizer=...) to manually set the tokenizer."
                 )
                 raise RuntimeError
 
         logger.debug(f"Running inference on {limit} samples.")
 
         model.model.eval()
         with torch.no_grad():
@@ -146,49 +143,20 @@
                     truncation=True,
                     max_length=max_length,
                 ).to(model.device)
                 model(**inputs)
                 count += 1
                 if count >= limit:
                     break
-        logger.debug("Inference results saved to `model.memory`.")
-
-    @staticmethod
-    def get_optimal_cut(model, block_size: int) -> int:
-        logger.debug(f"Choosing optimal {block_size}-layers block to prune.")
-        assert (
-            block_size < model.layer_count and block_size > 0
-        ), f"Expected `block_size` value between 1 and {model.layer_count -1}, got {block_size}."
-        layer_result = model.memory.result[block_size, : model.layer_count - block_size]
-        start_layer = np.argmin(layer_result)
-        logger.debug(f"Best 5-layers block to prune starts at layer: {start_layer}.")
-        return start_layer
-
-    @staticmethod
-    def get_block_score_stats(model, return_md=True, threshold=float("inf")) -> dict:
-        stats = {}
-        for i in range(1, model.layer_count):
-            layer_result = model.memory.result[i, : model.layer_count - i]
-            start_layer = np.argmin(layer_result)
-            score = layer_result[start_layer]
-            if score <= threshold:
-                stats[i] = {"start_layer": start_layer, "score": score}
-
-        if not return_md:
-            return stats
-
-        stats_md = "| Block_size | Removed_layers | Score (avg dist)|\n"
-        stats_md += "| -------- | ------- | -------- |\n"
-        for k, v in stats.items():
-            stats_md += f"| {k} | {v['start_layer']}-{v['start_layer']+k-1} | {round(v['score'], 3)}|\n"
-
-        return stats_md
+        result = model.memory.result
+        model.clear_memory()
+        return result
 
     @staticmethod
-    def cut(model, start_layer: int, block_size: int):
+    def prune(model, start_layer: int, block_size: int):
         new_layers = torch.nn.ModuleList()
 
         remove_layers = list(range(start_layer, start_layer + block_size))
         logger.debug(f"Removing layers: {remove_layers}")
 
         count = 0
         for i in range(0, model.layer_count):
@@ -209,16 +177,14 @@
         logger.debug(f"""Changing model config to reflect changes:
         config.num_hidden_layers: {model.config.num_hidden_layers} -> {changed_num_hidden_layers}
         config._name_or_path: {model.config._name_or_path} -> {changed_model_name_or_path}""")
 
         model.config.num_hidden_layers = changed_num_hidden_layers
         model.config._name_or_path = changed_model_name_or_path
 
-        model.clear_memory()
-
         return model
 
     @staticmethod
     def remove_layers(
         model,
         tokenizer,
         block_size,
@@ -227,16 +193,18 @@
         limit=1,
         batch_size=1,
         max_length=1000,
         return_outputs=False,
         distance=angular_distance_last_token,
     ):
         assert batch_size == 1, "batch_size > 1 is not supported yet."
-        model.analyse_layers(
+        result = model.analyse_layers(
             dataset=dataset,
             tokenizer=tokenizer,
             key=key,
             limit=limit,
             max_length=max_length,
         )
-        start_layer = model.get_optimal_cut(block_size=block_size)
-        return model.cut(start_layer=start_layer, block_size=block_size)
+        logger.debug(f"Choosing optimal {block_size}-layers block to prune.")
+        start_layer = get_best_pruning_start(result=result, block_size=block_size)
+        logger.debug(f"Best 5-layers block to prune starts at layer: {start_layer}.")
+        return model.prune(start_layer=start_layer, block_size=block_size)
```

### Comparing `short_transformers-0.2.0/PKG-INFO` & `short_transformers-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: short-transformers
-Version: 0.2.0
+Version: 0.3.0
 Summary: Cutting transformers layers
 License: MIT
 Author: Melisa Russak
 Author-email: melisa@russak.biz
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,112 +14,108 @@
 Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Description-Content-Type: text/markdown
 
 # :scissors: Short Transformers
 
-- Pytorch implementation of layer pruning proposed in [The Unreasonable Ineffectiveness of the Deeper Layers](https://arxiv.org/pdf/2403.17887.pdf).
+- [Unofficial] Pytorch implementation of layer pruning proposed in [The Unreasonable Ineffectiveness of the Deeper Layers](https://arxiv.org/pdf/2403.17887.pdf).
 - The repository reproduces and extends original methods by offering different layer pruning criteria.
 
 <p align="center">
-<img src="./docs/memory.png" align="center" width='300'/>
+<img src="./docs/merged.png" align="center" alt="Normalized angular distance from initial layer l (x-axis) with block size n (y-axis)." height='250'/>
 </p>
 
+
 [![pypi Version](https://img.shields.io/pypi/v/short-transformers.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/short-transformers/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 ## Installation:
 ```sh
 pip install short-transformers
 ```
 
 Required additional dependencies: `transformers`, `datasets`.
 
 ## Quickstart:
 ```python
 from short_transformers import ShortTransformer
+from datasets import load_dataset
 
 # load from path/hf_hub
 model = ShortTransformer.from_pretrained(model_name)
 
 # or use hf model
-model = ShortTransformer.from_model(hf_model)
+# model = ShortTransformer.from_model(hf_model)
 
-# remove n layers, use hf dataset to find the optimal cut
+# load hf dataset
+dataset = load_dataset("allenai/c4", "en", split="validation", streaming=True)
+
+# remove 5 layers, use the dataset to find the least important layers to remove
 short_model = model.remove_layers(block_size=5, dataset=dataset, limit=1000)
 
 # continue training to heal after the cut
 # ...
 
 # save as hf model
 short_mdoel.save_pretrained(output_path)
 ```
-Example log output:
-```sh
-[2024-05-04 18:39:03] [short-transformers] Running inference on 1000 samples.
-1000it [00:06, ?it/s]
-[2024-05-04 18:39:09] [short-transformers] Inference results saved to `model.memory`.
-[2024-05-04 18:39:09] [short-transformers] Choosing optimal 5-layers block to prune.
-[2024-05-04 18:39:09] [short-transformers] Best 5-layers block to prune starts at layer: 23.
-[2024-05-04 18:39:09] [short-transformers] Removing layers: [23, 24, 25, 26, 27]
-[2024-05-04 18:39:09] [short-transformers] Changing model config to reflect changes:
-        config.num_hidden_layers: 32 -> 27
-        config._name_or_path: meta-llama/Meta-Llama-3-8B -> meta-llama/Meta-Llama-3-8B-27L
-[2024-05-04 18:39:09] [short-transformers] Cleaning `model.memory`.
-```
 
 Both `short_model` and the saved model are fully compatible with transformers. See `examples/basic.py` for a complete working example.
 
 ## Pruning in steps:
 
 Pruning can composed step-by-step and customized:
 
 1. Analyze model layers:
 ```python
 from datasets import load_dataset
 from short_transformers import ShortTransformer
-from short_transformers.graph import draw_diagram
-
+from short_transformers.utils import (
+    draw_diagram,
+    get_scored_blocks,
+    get_best_pruning_start,
+)
 # load from path/hf_hub
 model_name = "meta-llama/Meta-Llama-3-8B"
 
 model = ShortTransformer.from_pretrained(model_name, device_map="auto")
 
 dataset = load_dataset("allenai/c4", "en", split="validation", streaming=True)
 
-# run inderence on a subset of the datsets
-model.analyse_layers(
+# calculate distances between inputs/outputs from/to model layers
+# results in a triangular numpy array of shape (layer_count, layer_count)
+# results[x, y] - averaged distances for block of size x starting at layer y
+results = model.analyse_layers(
     dataset=dataset,
     key="text",
     limit=100,
     max_length=1000,
 )
 
-# after this step, results will be saved to model.memory, which can be saved
-model.save_memory("memory.npz")
-
-# and visualized as seaborh graph (see examples in the README.md)
-draw_diagram("memory.npz", "memory.png")
+# draw results
+# diagrams style matches the style of original article
+# "The Unreasonable Ineffectiveness of the Deeper Layers"
+draw_diagram(results, "results.png", title="Meta-Llama-3-8B")
 ```
 
 Example output:
 <p align="center">
-<img src="./docs/memory.png" align="center" width='300'/>
+<img src="./docs/Meta-Llama-3-8B.png" align="center" width='300'/>
 </p>
 
-2. Find optimal block size and start_layer:
+2. Find optimal `block_size` and `start_layer`:
 ```python
-# finding optimial block of size 'num' to prune
-start_layer = model.get_optimal_cut(block_size=5)
+# find optimial block of size 'block_size' to prune
+start_layer = get_best_pruning_start(results, block_size=5)
 
-# evaluating all possibe block sizes to prune,
+# evaluate all possibe block sizes to prune,
 # for each block returns score 0-1
 # which is averaged over samples distance between input and output to/from a block
-block_score = model.get_block_score_stats(return_md=True, threshold=0.3)
+block_score = get_scored_blocks(results, return_md=True, threshold=0.3)
 ```
 
 Example output:
 
 | Block_size | Removed_layers | Score (avg dist)|
 | -------- | ------- | -------- |
 | 1 | 25-25 | 0.123|
@@ -130,23 +126,19 @@
 | 6 | 22-27 | 0.248|
 | 7 | 22-28 | 0.268|
 | 8 | 20-27 | 0.291|
 
 
 3. Pruning layers:
 ```python
-# pruning 5-layers block
-# this will also clean the `model.memory``
-model.cut(start_layer=start_layer, block_size=5)
-
-# or clean the model memory manually
-model.clean_memory()
+# prune 5-layers block
+model.prune(start_layer=start_layer, block_size=5)
 
 # save the pruned model
-model.save_pretrained("model_path")
+model.save_pretrained("model_output_dir")
 ```
 
 See `example/prune_in_steps.py` for a complete working example.
 
 
 ## Supported pruning methods:
 - based on layer input/output distances:
```

