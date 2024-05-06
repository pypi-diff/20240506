# Comparing `tmp/auto_circuit-0.1.1.tar.gz` & `tmp/auto_circuit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_circuit-0.1.1.tar", max compression
+gzip compressed data, was "auto_circuit-0.1.2.tar", max compression
```

## Comparing `auto_circuit-0.1.1.tar` & `auto_circuit-0.1.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1188 2024-04-29 00:57:42.137579 auto_circuit-0.1.1/README.md
--rw-r--r--   0        0        0    14880 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/data.py
--rw-r--r--   0        0        0     8438 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/experiment_utils.py
--rw-r--r--   0        0        0    10338 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/experiments.py
--rw-r--r--   0        0        0    13917 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/language_rotations.py
--rw-r--r--   0        0        0     6259 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/area_under_curve.py
--rw-r--r--   0        0        0     3741 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/avoid_edges.py
--rw-r--r--   0        0        0     9754 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/completeness_metrics/same_under_knockouts.py
--rw-r--r--   0        0        0     8595 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/completeness_metrics/train_same_under_knockouts.py
--rw-r--r--   0        0        0     8888 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/official_circuits/circuits/docstring_official.py
--rw-r--r--   0        0        0     5322 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/official_circuits/circuits/greaterthan_official.py
--rw-r--r--   0        0        0    11697 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/official_circuits/circuits/ioi_official.py
--rw-r--r--   0        0        0     8481 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/official_circuits/circuits/sports_players_official.py
--rw-r--r--   0        0        0     4896 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/official_circuits/circuits/tracr/reverse_official.py
--rw-r--r--   0        0        0     4648 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/official_circuits/circuits/tracr/xproportion_official.py
--rw-r--r--   0        0        0     4396 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/official_circuits/measure_roc.py
--rw-r--r--   0        0        0     4070 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/official_circuits/roc_plot.py
--rw-r--r--   0        0        0     2091 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/prune_metrics/answer_diff.py
--rw-r--r--   0        0        0     5344 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/prune_metrics/answer_diff_percent.py
--rw-r--r--   0        0        0     2208 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/prune_metrics/answer_value.py
--rw-r--r--   0        0        0     2709 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/prune_metrics/correct_answer_percent.py
--rw-r--r--   0        0        0     2264 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/prune_metrics/kl_div.py
--rw-r--r--   0        0        0     7097 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/prune_metrics/measure_prune_metrics.py
--rw-r--r--   0        0        0     6360 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/prune_metrics/prune_metrics.py
--rw-r--r--   0        0        0     3896 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/prune_metrics/prune_metrics_plot.py
--rw-r--r--   0        0        0     6359 2024-04-29 00:57:42.141579 auto_circuit-0.1.1/auto_circuit/metrics/prune_scores_similarity.py
--rw-r--r--   0        0        0     5426 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/model_utils/micro_model_utils.py
--rw-r--r--   0        0        0     6135 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/model_utils/sparse_autoencoders/autoencoder_training.py
--rw-r--r--   0        0        0    11709 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/model_utils/sparse_autoencoders/autoencoder_transformer.py
--rw-r--r--   0        0        0     7190 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/model_utils/sparse_autoencoders/sparse_autoencoder.py
--rw-r--r--   0        0        0     9047 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/model_utils/task_projectors/projector_transformer.py
--rw-r--r--   0        0        0     5846 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/model_utils/task_projectors/task_projector.py
--rw-r--r--   0        0        0    12255 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/model_utils/task_projectors/task_projector_training.py
--rw-r--r--   0        0        0     7950 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/model_utils/tracr_model_utils.py
--rw-r--r--   0        0        0     7622 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/model_utils/transformer_lens_utils.py
--rw-r--r--   0        0        0    14863 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/playground.py
--rw-r--r--   0        0        0     5123 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/prune.py
--rw-r--r--   0        0        0     7888 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/prune_algos/ACDC.py
--rw-r--r--   0        0        0     1718 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/prune_algos/activation_magnitude.py
--rw-r--r--   0        0        0     3759 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/prune_algos/circuit_probing.py
--rw-r--r--   0        0        0     4373 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/prune_algos/edge_attribution_patching.py
--rw-r--r--   0        0        0     1054 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/prune_algos/ground_truth.py
--rw-r--r--   0        0        0     5064 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/prune_algos/mask_gradient.py
--rw-r--r--   0        0        0     2699 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/prune_algos/parameter_integrated_gradients.py
--rw-r--r--   0        0        0    10248 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/prune_algos/prune_algos.py
--rw-r--r--   0        0        0      994 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/prune_algos/random_edges.py
--rw-r--r--   0        0        0    11955 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/prune_algos/subnetwork_probing.py
--rw-r--r--   0        0        0     7465 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/pythia-2_8b-sports.py
--rw-r--r--   0        0        0    16984 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/tasks.py
--rw-r--r--   0        0        0     3729 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/tracr_experiments.py
--rw-r--r--   0        0        0    11715 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/types.py
--rw-r--r--   0        0        0     6091 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/uniqueness_experiments.py
--rw-r--r--   0        0        0     6775 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/utils/ablation_activations.py
--rw-r--r--   0        0        0      590 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/utils/custom_tqdm.py
--rw-r--r--   0        0        0    19341 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/utils/graph_utils.py
--rw-r--r--   0        0        0     7165 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/utils/misc.py
--rw-r--r--   0        0        0     6295 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/utils/patch_wrapper.py
--rw-r--r--   0        0        0     9112 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/utils/patchable_model.py
--rw-r--r--   0        0        0     9933 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/utils/tensor_ops.py
--rw-r--r--   0        0        0    11460 2024-04-29 00:57:42.145578 auto_circuit-0.1.1/auto_circuit/visualize.py
--rw-r--r--   0        0        0     1397 2024-04-29 00:59:42.133556 auto_circuit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 auto_circuit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1276 2024-05-06 00:21:23.358464 auto_circuit-0.1.2/README.md
+-rw-r--r--   0        0        0    14880 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/data.py
+-rw-r--r--   0        0        0     8438 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/experiment_utils.py
+-rw-r--r--   0        0        0    10338 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/experiments.py
+-rw-r--r--   0        0        0    13917 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/language_rotations.py
+-rw-r--r--   0        0        0     6259 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/area_under_curve.py
+-rw-r--r--   0        0        0     3741 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/avoid_edges.py
+-rw-r--r--   0        0        0     9754 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/completeness_metrics/same_under_knockouts.py
+-rw-r--r--   0        0        0     8595 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/completeness_metrics/train_same_under_knockouts.py
+-rw-r--r--   0        0        0     8888 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/docstring_official.py
+-rw-r--r--   0        0        0     5322 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/greaterthan_official.py
+-rw-r--r--   0        0        0    11697 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/ioi_official.py
+-rw-r--r--   0        0        0     8481 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/sports_players_official.py
+-rw-r--r--   0        0        0     4896 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/tracr/reverse_official.py
+-rw-r--r--   0        0        0     4648 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/tracr/xproportion_official.py
+-rw-r--r--   0        0        0     4396 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/measure_roc.py
+-rw-r--r--   0        0        0     4070 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/roc_plot.py
+-rw-r--r--   0        0        0     2091 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/answer_diff.py
+-rw-r--r--   0        0        0     5344 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/answer_diff_percent.py
+-rw-r--r--   0        0        0     2208 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/answer_value.py
+-rw-r--r--   0        0        0     2709 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/correct_answer_percent.py
+-rw-r--r--   0        0        0     2264 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/kl_div.py
+-rw-r--r--   0        0        0     7097 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/measure_prune_metrics.py
+-rw-r--r--   0        0        0     6360 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/prune_metrics.py
+-rw-r--r--   0        0        0     3896 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/prune_metrics_plot.py
+-rw-r--r--   0        0        0     6359 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/metrics/prune_scores_similarity.py
+-rw-r--r--   0        0        0     5426 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/micro_model_utils.py
+-rw-r--r--   0        0        0     6135 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/sparse_autoencoders/autoencoder_training.py
+-rw-r--r--   0        0        0    11709 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/sparse_autoencoders/autoencoder_transformer.py
+-rw-r--r--   0        0        0     7190 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/sparse_autoencoders/sparse_autoencoder.py
+-rw-r--r--   0        0        0     9047 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/task_projectors/projector_transformer.py
+-rw-r--r--   0        0        0     5846 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/task_projectors/task_projector.py
+-rw-r--r--   0        0        0    12255 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/task_projectors/task_projector_training.py
+-rw-r--r--   0        0        0     7950 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/tracr_model_utils.py
+-rw-r--r--   0        0        0     7622 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/model_utils/transformer_lens_utils.py
+-rw-r--r--   0        0        0    14863 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/playground.py
+-rw-r--r--   0        0        0     5123 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune.py
+-rw-r--r--   0        0        0     7888 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/ACDC.py
+-rw-r--r--   0        0        0     1718 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/activation_magnitude.py
+-rw-r--r--   0        0        0     3759 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/circuit_probing.py
+-rw-r--r--   0        0        0     4373 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/edge_attribution_patching.py
+-rw-r--r--   0        0        0     1054 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/ground_truth.py
+-rw-r--r--   0        0        0     5064 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/mask_gradient.py
+-rw-r--r--   0        0        0     2699 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/parameter_integrated_gradients.py
+-rw-r--r--   0        0        0    10248 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/prune_algos.py
+-rw-r--r--   0        0        0      994 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/random_edges.py
+-rw-r--r--   0        0        0    11955 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/prune_algos/subnetwork_probing.py
+-rw-r--r--   0        0        0     7465 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/pythia-2_8b-sports.py
+-rw-r--r--   0        0        0    16984 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/tasks.py
+-rw-r--r--   0        0        0     3729 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/tracr_experiments.py
+-rw-r--r--   0        0        0    11715 2024-05-06 00:21:23.362464 auto_circuit-0.1.2/auto_circuit/types.py
+-rw-r--r--   0        0        0     6091 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/uniqueness_experiments.py
+-rw-r--r--   0        0        0     6775 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/utils/ablation_activations.py
+-rw-r--r--   0        0        0      590 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/utils/custom_tqdm.py
+-rw-r--r--   0        0        0    19341 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/utils/graph_utils.py
+-rw-r--r--   0        0        0     7165 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/utils/misc.py
+-rw-r--r--   0        0        0     6295 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/utils/patch_wrapper.py
+-rw-r--r--   0        0        0     9609 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/utils/patchable_model.py
+-rw-r--r--   0        0        0     9933 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/utils/tensor_ops.py
+-rw-r--r--   0        0        0    11460 2024-05-06 00:21:23.366464 auto_circuit-0.1.2/auto_circuit/visualize.py
+-rw-r--r--   0        0        0     1397 2024-05-06 00:23:34.131356 auto_circuit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2064 1970-01-01 00:00:00.000000 auto_circuit-0.1.2/PKG-INFO
```

### Comparing `auto_circuit-0.1.1/README.md` & `auto_circuit-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-![PyPI - Version](https://img.shields.io/pypi/v/auto-circuit?logo=pypi&logoColor=white)
-![GitHub Release](https://img.shields.io/github/v/release/UFO-101/auto-circuit?logo=github&logoColor=white)
+[![PyPI - Version](https://img.shields.io/pypi/v/auto-circuit?logo=pypi&logoColor=white)](https://pypi.org/project/auto-circuit/)
+[![GitHub Release](https://img.shields.io/github/v/release/UFO-101/auto-circuit?logo=github&logoColor=white)](https://github.com/UFO-101/auto-circuit/releases)
 # AutoCircuit
 ![](docs/assets/Edge_Patching_Rounded.png)
 
-A library for testing automatic circuit discovery algorithms.
+A library for efficient patching and automatic circuit discovery.
 
-![Static Badge](https://img.shields.io/badge/Read%20the%20Docs-414A82?style=for-the-badge&logo=Google%20Docs&logoColor=white&labelColor=CB5AD9&link=https%3A%2F%2Fufo-101.github.io%2Fauto-circuit)
+[![Static Badge](https://img.shields.io/badge/Read%20the%20Docs-414A82?style=for-the-badge&logo=Google%20Docs&logoColor=white&labelColor=CB5AD9)](https://UFO-101.github.io/auto-circuit)
 
 ## Read the draft paper
 [Transformer Circuit Metrics are not Robust](Transformer%20Circuit%20Metrics%20are%20not%20Robust.pdf)
 
 ## Getting Started
 
 ```bash
```

### Comparing `auto_circuit-0.1.1/auto_circuit/data.py` & `auto_circuit-0.1.2/auto_circuit/data.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/experiment_utils.py` & `auto_circuit-0.1.2/auto_circuit/experiment_utils.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/experiments.py` & `auto_circuit-0.1.2/auto_circuit/experiments.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/language_rotations.py` & `auto_circuit-0.1.2/auto_circuit/language_rotations.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/area_under_curve.py` & `auto_circuit-0.1.2/auto_circuit/metrics/area_under_curve.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/avoid_edges.py` & `auto_circuit-0.1.2/auto_circuit/metrics/avoid_edges.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/completeness_metrics/same_under_knockouts.py` & `auto_circuit-0.1.2/auto_circuit/metrics/completeness_metrics/same_under_knockouts.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/completeness_metrics/train_same_under_knockouts.py` & `auto_circuit-0.1.2/auto_circuit/metrics/completeness_metrics/train_same_under_knockouts.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/official_circuits/circuits/docstring_official.py` & `auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/docstring_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/official_circuits/circuits/greaterthan_official.py` & `auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/greaterthan_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/official_circuits/circuits/ioi_official.py` & `auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/ioi_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/official_circuits/circuits/sports_players_official.py` & `auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/sports_players_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/official_circuits/circuits/tracr/reverse_official.py` & `auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/tracr/reverse_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/official_circuits/circuits/tracr/xproportion_official.py` & `auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/circuits/tracr/xproportion_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/official_circuits/measure_roc.py` & `auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/measure_roc.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/official_circuits/roc_plot.py` & `auto_circuit-0.1.2/auto_circuit/metrics/official_circuits/roc_plot.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/prune_metrics/answer_diff.py` & `auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/answer_diff.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/prune_metrics/answer_diff_percent.py` & `auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/answer_diff_percent.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/prune_metrics/answer_value.py` & `auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/answer_value.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/prune_metrics/correct_answer_percent.py` & `auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/correct_answer_percent.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/prune_metrics/kl_div.py` & `auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/kl_div.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/prune_metrics/measure_prune_metrics.py` & `auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/measure_prune_metrics.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/prune_metrics/prune_metrics.py` & `auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/prune_metrics.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/prune_metrics/prune_metrics_plot.py` & `auto_circuit-0.1.2/auto_circuit/metrics/prune_metrics/prune_metrics_plot.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/metrics/prune_scores_similarity.py` & `auto_circuit-0.1.2/auto_circuit/metrics/prune_scores_similarity.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/model_utils/micro_model_utils.py` & `auto_circuit-0.1.2/auto_circuit/model_utils/micro_model_utils.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/model_utils/sparse_autoencoders/autoencoder_training.py` & `auto_circuit-0.1.2/auto_circuit/model_utils/sparse_autoencoders/autoencoder_training.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/model_utils/sparse_autoencoders/autoencoder_transformer.py` & `auto_circuit-0.1.2/auto_circuit/model_utils/sparse_autoencoders/autoencoder_transformer.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/model_utils/sparse_autoencoders/sparse_autoencoder.py` & `auto_circuit-0.1.2/auto_circuit/model_utils/sparse_autoencoders/sparse_autoencoder.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/model_utils/task_projectors/projector_transformer.py` & `auto_circuit-0.1.2/auto_circuit/model_utils/task_projectors/projector_transformer.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/model_utils/task_projectors/task_projector.py` & `auto_circuit-0.1.2/auto_circuit/model_utils/task_projectors/task_projector.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/model_utils/task_projectors/task_projector_training.py` & `auto_circuit-0.1.2/auto_circuit/model_utils/task_projectors/task_projector_training.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/model_utils/tracr_model_utils.py` & `auto_circuit-0.1.2/auto_circuit/model_utils/tracr_model_utils.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/model_utils/transformer_lens_utils.py` & `auto_circuit-0.1.2/auto_circuit/model_utils/transformer_lens_utils.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/playground.py` & `auto_circuit-0.1.2/auto_circuit/playground.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/prune.py` & `auto_circuit-0.1.2/auto_circuit/prune.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/prune_algos/ACDC.py` & `auto_circuit-0.1.2/auto_circuit/prune_algos/ACDC.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/prune_algos/activation_magnitude.py` & `auto_circuit-0.1.2/auto_circuit/prune_algos/activation_magnitude.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/prune_algos/circuit_probing.py` & `auto_circuit-0.1.2/auto_circuit/prune_algos/circuit_probing.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/prune_algos/edge_attribution_patching.py` & `auto_circuit-0.1.2/auto_circuit/prune_algos/edge_attribution_patching.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/prune_algos/ground_truth.py` & `auto_circuit-0.1.2/auto_circuit/prune_algos/ground_truth.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/prune_algos/mask_gradient.py` & `auto_circuit-0.1.2/auto_circuit/prune_algos/mask_gradient.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/prune_algos/parameter_integrated_gradients.py` & `auto_circuit-0.1.2/auto_circuit/prune_algos/parameter_integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/prune_algos/prune_algos.py` & `auto_circuit-0.1.2/auto_circuit/prune_algos/prune_algos.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/prune_algos/random_edges.py` & `auto_circuit-0.1.2/auto_circuit/prune_algos/random_edges.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/prune_algos/subnetwork_probing.py` & `auto_circuit-0.1.2/auto_circuit/prune_algos/subnetwork_probing.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/pythia-2_8b-sports.py` & `auto_circuit-0.1.2/auto_circuit/pythia-2_8b-sports.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/tasks.py` & `auto_circuit-0.1.2/auto_circuit/tasks.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/tracr_experiments.py` & `auto_circuit-0.1.2/auto_circuit/tracr_experiments.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/types.py` & `auto_circuit-0.1.2/auto_circuit/types.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/uniqueness_experiments.py` & `auto_circuit-0.1.2/auto_circuit/uniqueness_experiments.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/utils/ablation_activations.py` & `auto_circuit-0.1.2/auto_circuit/utils/ablation_activations.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/utils/custom_tqdm.py` & `auto_circuit-0.1.2/auto_circuit/utils/custom_tqdm.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/utils/graph_utils.py` & `auto_circuit-0.1.2/auto_circuit/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/utils/misc.py` & `auto_circuit-0.1.2/auto_circuit/utils/misc.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/utils/patch_wrapper.py` & `auto_circuit-0.1.2/auto_circuit/utils/patch_wrapper.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/utils/patchable_model.py` & `auto_circuit-0.1.2/auto_circuit/utils/patchable_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,27 @@
         if self.kv_caches is None:
             return self.wrapped_model.run_with_cache(*args, **kwargs)
         else:
             batch_size = args[0].shape[0]
             kv = self.kv_caches[batch_size]
             return self.wrapped_model.run_with_cache(*args, past_kv_cache=kv, **kwargs)
 
+    def input_to_embed(self, *args: Any, **kwargs: Any) -> Any:
+        """
+        Wrapper around the `input_to_embed` method of the wrapped TransformerLens
+        `HookedTransformer`. If `kv_caches` is not `None`, the KV cache is passed to the
+        wrapped model as a keyword argument.
+        """
+        if self.kv_caches is None:
+            return self.wrapped_model.input_to_embed(*args, **kwargs)
+        else:
+            batch_size = args[0].shape[0]
+            kv = self.kv_caches[batch_size]
+            return self.wrapped_model.input_to_embed(*args, past_kv_cache=kv, **kwargs)
+
     def new_prune_scores(self, init_val: float = 0.0) -> PruneScores:
         """
         A new [`PruneScores`][auto_circuit.types.PruneScores] instance with the same
         keys and shapes as the current patch masks, initialized to `init_val`.
 
         Args:
             init_val: The initial value to set all the prune scores to.
@@ -207,18 +220,14 @@
         return self.wrapped_model.cfg
 
     @property
     def tokenizer(self) -> Any:
         return self.wrapped_model.tokenizer
 
     @property
-    def input_to_embed(self) -> Any:
-        return self.wrapped_model.input_to_embed
-
-    @property
     def blocks(self) -> Any:
         return self.wrapped_model.blocks
 
     def to_tokens(self) -> Any:
         return self.wrapped_model.to_tokens
 
     def to_str_tokens(self) -> Any:
```

### Comparing `auto_circuit-0.1.1/auto_circuit/utils/tensor_ops.py` & `auto_circuit-0.1.2/auto_circuit/utils/tensor_ops.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/auto_circuit/visualize.py` & `auto_circuit-0.1.2/auto_circuit/visualize.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.1/pyproject.toml` & `auto_circuit-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "auto-circuit"
-version = "0.1.1"  # This isn't used. Version set during Github action.
+version = "0.1.2"  # This isn't used. Version set during Github action.
 description = ""
 authors = ["UFO-101 <josephmiller101@gmail.com>"]
 readme = "README.md"
 packages = [{include = "auto_circuit"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `auto_circuit-0.1.1/PKG-INFO` & `auto_circuit-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-circuit
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: UFO-101
 Author-email: josephmiller101@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -17,22 +17,22 @@
 Requires-Dist: torch (>=2.1.1,<3.0.0)
 Requires-Dist: tracr-pypi (==1.0.0)
 Requires-Dist: transformer-lens (>=1.13.0,<2.0.0)
 Requires-Dist: vscode-tqdm (==4.66.2)
 Requires-Dist: word2word (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
-![PyPI - Version](https://img.shields.io/pypi/v/auto-circuit?logo=pypi&logoColor=white)
-![GitHub Release](https://img.shields.io/github/v/release/UFO-101/auto-circuit?logo=github&logoColor=white)
+[![PyPI - Version](https://img.shields.io/pypi/v/auto-circuit?logo=pypi&logoColor=white)](https://pypi.org/project/auto-circuit/)
+[![GitHub Release](https://img.shields.io/github/v/release/UFO-101/auto-circuit?logo=github&logoColor=white)](https://github.com/UFO-101/auto-circuit/releases)
 # AutoCircuit
 ![](docs/assets/Edge_Patching_Rounded.png)
 
-A library for testing automatic circuit discovery algorithms.
+A library for efficient patching and automatic circuit discovery.
 
-![Static Badge](https://img.shields.io/badge/Read%20the%20Docs-414A82?style=for-the-badge&logo=Google%20Docs&logoColor=white&labelColor=CB5AD9&link=https%3A%2F%2Fufo-101.github.io%2Fauto-circuit)
+[![Static Badge](https://img.shields.io/badge/Read%20the%20Docs-414A82?style=for-the-badge&logo=Google%20Docs&logoColor=white&labelColor=CB5AD9)](https://UFO-101.github.io/auto-circuit)
 
 ## Read the draft paper
 [Transformer Circuit Metrics are not Robust](Transformer%20Circuit%20Metrics%20are%20not%20Robust.pdf)
 
 ## Getting Started
 
 ```bash
```

