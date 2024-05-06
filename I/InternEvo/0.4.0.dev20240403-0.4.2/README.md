# Comparing `tmp/InternEvo-0.4.0.dev20240403.tar.gz` & `tmp/InternEvo-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InternEvo-0.4.0.dev20240403.tar", last modified: Wed Apr  3 14:30:19 2024, max compression
+gzip compressed data, was "InternEvo-0.4.2.tar", last modified: Mon May  6 07:52:31 2024, max compression
```

## Comparing `InternEvo-0.4.0.dev20240403.tar` & `InternEvo-0.4.2.tar`

### file list

```diff
@@ -1,161 +1,170 @@
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.723194 InternEvo-0.4.0.dev20240403/
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:36.816954 InternEvo-0.4.0.dev20240403/InternEvo.egg-info/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5332 2024-04-03 14:30:17.000000 InternEvo-0.4.0.dev20240403/InternEvo.egg-info/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4317 2024-04-03 14:30:17.000000 InternEvo-0.4.0.dev20240403/InternEvo.egg-info/SOURCES.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-04-03 14:30:17.000000 InternEvo-0.4.0.dev20240403/InternEvo.egg-info/dependency_links.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       15 2024-04-03 14:30:17.000000 InternEvo-0.4.0.dev20240403/InternEvo.egg-info/top_level.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13656 2024-01-25 08:28:54.000000 InternEvo-0.4.0.dev20240403/LICENSE
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5332 2024-04-03 14:30:19.044910 InternEvo-0.4.0.dev20240403/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4730 2024-01-25 08:28:54.000000 InternEvo-0.4.0.dev20240403/README.md
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:36.824243 InternEvo-0.4.0.dev20240403/internlm/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      267 2024-01-30 08:18:31.000000 InternEvo-0.4.0.dev20240403/internlm/__init__.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:36.867718 InternEvo-0.4.0.dev20240403/internlm/accelerator/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      147 2024-03-26 14:50:22.000000 InternEvo-0.4.0.dev20240403/internlm/accelerator/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4017 2024-04-02 03:03:24.000000 InternEvo-0.4.0.dev20240403/internlm/accelerator/abstract_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11010 2024-03-28 03:16:50.000000 InternEvo-0.4.0.dev20240403/internlm/accelerator/cuda_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11446 2024-04-02 03:03:24.000000 InternEvo-0.4.0.dev20240403/internlm/accelerator/dipu_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10866 2024-03-28 03:16:50.000000 InternEvo-0.4.0.dev20240403/internlm/accelerator/npu_accelerator.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:36.880860 InternEvo-0.4.0.dev20240403/internlm/apis/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.0.dev20240403/internlm/apis/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    37532 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/apis/inference.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:36.926106 InternEvo-0.4.0.dev20240403/internlm/checkpoint/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       83 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/checkpoint/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27404 2024-03-26 14:50:22.000000 InternEvo-0.4.0.dev20240403/internlm/checkpoint/checkpoint_manager.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20076 2024-03-26 14:50:22.000000 InternEvo-0.4.0.dev20240403/internlm/checkpoint/components.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8723 2024-03-26 14:50:23.000000 InternEvo-0.4.0.dev20240403/internlm/checkpoint/load_funcs.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2504 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/checkpoint/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:36.967895 InternEvo-0.4.0.dev20240403/internlm/core/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      158 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/core/__init__.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:36.998938 InternEvo-0.4.0.dev20240403/internlm/core/communication/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      884 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/core/communication/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    23944 2024-04-02 03:03:24.000000 InternEvo-0.4.0.dev20240403/internlm/core/communication/isp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22670 2024-03-26 14:50:23.000000 InternEvo-0.4.0.dev20240403/internlm/core/communication/p2p.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10352 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/core/communication/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.032423 InternEvo-0.4.0.dev20240403/internlm/core/context/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1220 2024-03-18 08:30:10.000000 InternEvo-0.4.0.dev20240403/internlm/core/context/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27076 2024-03-27 02:26:43.000000 InternEvo-0.4.0.dev20240403/internlm/core/context/parallel_context.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    38371 2024-03-18 08:30:10.000000 InternEvo-0.4.0.dev20240403/internlm/core/context/process_group_initializer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4295 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/core/context/random.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7458 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/core/engine.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3113 2024-03-28 03:16:50.000000 InternEvo-0.4.0.dev20240403/internlm/core/gradient_handler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8195 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/internlm/core/naive_amp.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.059207 InternEvo-0.4.0.dev20240403/internlm/core/scheduler/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      303 2024-02-08 03:13:39.000000 InternEvo-0.4.0.dev20240403/internlm/core/scheduler/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5258 2024-03-22 07:04:00.000000 InternEvo-0.4.0.dev20240403/internlm/core/scheduler/base_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9071 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/internlm/core/scheduler/no_pipeline_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    64105 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/internlm/core/scheduler/pipeline_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7598 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/core/trainer.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.090006 InternEvo-0.4.0.dev20240403/internlm/data/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      209 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/data/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5819 2024-03-26 10:32:52.000000 InternEvo-0.4.0.dev20240403/internlm/data/build_dataloader.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.138904 InternEvo-0.4.0.dev20240403/internlm/data/tokenized/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      418 2024-03-22 07:04:00.000000 InternEvo-0.4.0.dev20240403/internlm/data/tokenized/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15158 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/data/tokenized/batch_sampler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3767 2024-03-25 08:46:10.000000 InternEvo-0.4.0.dev20240403/internlm/data/tokenized/collaters.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1714 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/data/tokenized/dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1406 2024-03-26 10:32:52.000000 InternEvo-0.4.0.dev20240403/internlm/data/tokenized/dummy_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    18135 2024-03-26 10:32:52.000000 InternEvo-0.4.0.dev20240403/internlm/data/tokenized/packed_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3740 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/data/tokenized/single_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      454 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/data/train_state.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1919 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/internlm/data/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.156319 InternEvo-0.4.0.dev20240403/internlm/eval/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       86 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/eval/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5552 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/internlm/eval/evaluation.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.183331 InternEvo-0.4.0.dev20240403/internlm/initialize/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      368 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/initialize/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1793 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/initialize/initialize_tensor.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5922 2024-03-26 10:32:52.000000 InternEvo-0.4.0.dev20240403/internlm/initialize/initialize_trainer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27669 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/initialize/launch.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.199228 InternEvo-0.4.0.dev20240403/internlm/initialize/legacy/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.0.dev20240403/internlm/initialize/legacy/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1592 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/internlm/initialize/legacy/launch.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.250254 InternEvo-0.4.0.dev20240403/internlm/model/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1011 2024-03-25 08:46:10.000000 InternEvo-0.4.0.dev20240403/internlm/model/__init__.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.265555 InternEvo-0.4.0.dev20240403/internlm/model/losses/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       73 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/model/losses/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2275 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/model/losses/ce_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16750 2024-04-03 03:05:29.000000 InternEvo-0.4.0.dev20240403/internlm/model/metrics.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24429 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/model/modeling_internlm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    55789 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/model/modeling_internlm2.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    53658 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/model/modeling_llama.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    26623 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/model/modeling_moe.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.297343 InternEvo-0.4.0.dev20240403/internlm/model/modules/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.4.0.dev20240403/internlm/model/modules/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20285 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/model/modules/embedding.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9883 2024-04-01 07:02:19.000000 InternEvo-0.4.0.dev20240403/internlm/model/modules/mlp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    40988 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/model/modules/multi_head_attention.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.335707 InternEvo-0.4.0.dev20240403/internlm/model/moe/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      678 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1198 2024-03-28 03:16:50.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/base_layer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2762 2024-03-18 08:30:10.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/experts.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    17698 2024-04-02 09:15:26.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/gshard_layer.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.371323 InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8705 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/megablock_dmoe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13643 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/megablock_moe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2555 2024-03-15 18:58:58.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/mlp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11986 2024-03-26 14:50:23.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4494 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/moe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2021 2024-03-18 08:30:10.000000 InternEvo-0.4.0.dev20240403/internlm/model/moe/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.392015 InternEvo-0.4.0.dev20240403/internlm/model/ops/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.4.0.dev20240403/internlm/model/ops/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16010 2024-03-28 02:19:14.000000 InternEvo-0.4.0.dev20240403/internlm/model/ops/linear.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1500 2024-03-15 18:58:59.000000 InternEvo-0.4.0.dev20240403/internlm/model/ops/norm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    26403 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/model/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.423565 InternEvo-0.4.0.dev20240403/internlm/monitor/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      193 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/monitor/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1479 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/monitor/alert.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10213 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/monitor/monitor.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      776 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/monitor/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.444280 InternEvo-0.4.0.dev20240403/internlm/solver/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-15 18:58:59.000000 InternEvo-0.4.0.dev20240403/internlm/solver/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10095 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/solver/activation_checkpoint.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.485173 InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-22 07:04:01.000000 InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1080 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/base_optimizer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9173 2024-03-22 08:39:35.000000 InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/fsdp_optimizer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    42555 2024-04-02 03:03:24.000000 InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/hybrid_zero_optim.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10132 2024-03-22 08:39:35.000000 InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/store.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20351 2024-04-02 03:03:24.000000 InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1280 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/solver/pipeline_utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.509032 InternEvo-0.4.0.dev20240403/internlm/solver/schedulers/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      272 2024-03-15 18:58:59.000000 InternEvo-0.4.0.dev20240403/internlm/solver/schedulers/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      844 2024-03-26 03:26:29.000000 InternEvo-0.4.0.dev20240403/internlm/solver/schedulers/beta2_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5940 2024-03-15 18:58:59.000000 InternEvo-0.4.0.dev20240403/internlm/solver/schedulers/lr_scheduler.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.529815 InternEvo-0.4.0.dev20240403/internlm/train/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      635 2024-03-15 18:58:59.000000 InternEvo-0.4.0.dev20240403/internlm/train/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24865 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/train/pipeline.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3454 2024-03-25 08:46:10.000000 InternEvo-0.4.0.dev20240403/internlm/train/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.610026 InternEvo-0.4.0.dev20240403/internlm/utils/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.0.dev20240403/internlm/utils/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8886 2024-04-02 03:03:24.000000 InternEvo-0.4.0.dev20240403/internlm/utils/common.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6321 2024-04-02 07:54:06.000000 InternEvo-0.4.0.dev20240403/internlm/utils/gputest.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1353 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/internlm/utils/logger.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4156 2024-03-26 14:51:38.000000 InternEvo-0.4.0.dev20240403/internlm/utils/megatron_timers.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4038 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/internlm/utils/parallel.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2423 2024-01-25 08:28:55.000000 InternEvo-0.4.0.dev20240403/internlm/utils/registry.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24734 2024-03-26 03:26:29.000000 InternEvo-0.4.0.dev20240403/internlm/utils/simple_memory_profiler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    46133 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/internlm/utils/storage_manager.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3126 2024-03-15 18:58:59.000000 InternEvo-0.4.0.dev20240403/internlm/utils/timeout.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      709 2024-02-07 12:02:58.000000 InternEvo-0.4.0.dev20240403/internlm/utils/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7117 2024-03-28 03:16:51.000000 InternEvo-0.4.0.dev20240403/internlm/utils/writer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-04-03 14:30:19.047881 InternEvo-0.4.0.dev20240403/setup.cfg
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1103 2024-01-25 12:12:29.000000 InternEvo-0.4.0.dev20240403/setup.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.619324 InternEvo-0.4.0.dev20240403/tests/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.0.dev20240403/tests/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4510 2024-03-26 15:01:25.000000 InternEvo-0.4.0.dev20240403/tests/common_fixture.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.642253 InternEvo-0.4.0.dev20240403/tests/test_core/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.0.dev20240403/tests/test_core/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5875 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/tests/test_core/test_pipeline.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6978 2024-03-26 15:01:25.000000 InternEvo-0.4.0.dev20240403/tests/test_core/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-03 14:28:37.712084 InternEvo-0.4.0.dev20240403/tests/test_training/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5750 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/tests/test_training/7B_check_acc.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6360 2024-04-01 03:27:51.000000 InternEvo-0.4.0.dev20240403/tests/test_training/7B_check_init.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:46.000000 InternEvo-0.4.0.dev20240403/tests/test_training/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7939 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/tests/test_training/test_forward_output_no_fa.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11734 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/tests/test_training/test_load_ckpt_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12904 2024-04-01 04:38:33.000000 InternEvo-0.4.0.dev20240403/tests/test_training/test_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3845 2024-03-27 06:23:57.000000 InternEvo-0.4.0.dev20240403/tests/test_training/test_no_fa_train_temp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6521 2024-03-27 06:23:57.000000 InternEvo-0.4.0.dev20240403/tests/test_training/test_norm_weight.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12591 2024-04-03 02:12:20.000000 InternEvo-0.4.0.dev20240403/tests/test_training/test_swap_nb_loss_and_gradnorm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13964 2024-04-03 12:26:56.000000 InternEvo-0.4.0.dev20240403/tests/test_training/train_CI.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:35.081779 InternEvo-0.4.2/
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.208970 InternEvo-0.4.2/InternEvo.egg-info/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5320 2024-05-06 07:52:30.000000 InternEvo-0.4.2/InternEvo.egg-info/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4662 2024-05-06 07:52:30.000000 InternEvo-0.4.2/InternEvo.egg-info/SOURCES.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-06 07:52:30.000000 InternEvo-0.4.2/InternEvo.egg-info/dependency_links.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       18 2024-05-06 07:52:30.000000 InternEvo-0.4.2/InternEvo.egg-info/requires.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       15 2024-05-06 07:52:30.000000 InternEvo-0.4.2/InternEvo.egg-info/top_level.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13656 2024-01-25 08:28:54.000000 InternEvo-0.4.2/LICENSE
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5320 2024-05-06 07:52:31.908678 InternEvo-0.4.2/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4730 2024-01-25 08:28:54.000000 InternEvo-0.4.2/README.md
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.215635 InternEvo-0.4.2/internlm/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      267 2024-01-30 08:18:31.000000 InternEvo-0.4.2/internlm/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.251726 InternEvo-0.4.2/internlm/accelerator/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      147 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/accelerator/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4017 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/accelerator/abstract_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11010 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/accelerator/cuda_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11446 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/accelerator/dipu_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10866 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/accelerator/npu_accelerator.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.266484 InternEvo-0.4.2/internlm/apis/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.2/internlm/apis/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    37532 2024-01-25 08:28:55.000000 InternEvo-0.4.2/internlm/apis/inference.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.303899 InternEvo-0.4.2/internlm/checkpoint/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       83 2024-03-15 18:58:58.000000 InternEvo-0.4.2/internlm/checkpoint/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27404 2024-04-17 07:54:31.000000 InternEvo-0.4.2/internlm/checkpoint/checkpoint_manager.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20076 2024-04-12 05:43:59.000000 InternEvo-0.4.2/internlm/checkpoint/components.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14174 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/checkpoint/load_funcs.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2474 2024-04-10 07:31:30.000000 InternEvo-0.4.2/internlm/checkpoint/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.335677 InternEvo-0.4.2/internlm/core/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      158 2024-01-25 08:28:55.000000 InternEvo-0.4.2/internlm/core/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.365934 InternEvo-0.4.2/internlm/core/communication/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      884 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/core/communication/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    23944 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/core/communication/isp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22670 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/core/communication/p2p.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10118 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/core/communication/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.393716 InternEvo-0.4.2/internlm/core/context/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1220 2024-03-18 08:30:10.000000 InternEvo-0.4.2/internlm/core/context/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27076 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/core/context/parallel_context.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    38371 2024-03-18 08:30:10.000000 InternEvo-0.4.2/internlm/core/context/process_group_initializer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4295 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/core/context/random.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7458 2024-03-15 18:58:58.000000 InternEvo-0.4.2/internlm/core/engine.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3113 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/core/gradient_handler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8195 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/core/naive_amp.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.422162 InternEvo-0.4.2/internlm/core/scheduler/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      303 2024-02-08 03:13:39.000000 InternEvo-0.4.2/internlm/core/scheduler/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5258 2024-03-22 07:04:00.000000 InternEvo-0.4.2/internlm/core/scheduler/base_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9071 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/core/scheduler/no_pipeline_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    64105 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/core/scheduler/pipeline_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7598 2024-04-19 04:15:42.000000 InternEvo-0.4.2/internlm/core/trainer.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.447469 InternEvo-0.4.2/internlm/data/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      209 2024-03-15 18:58:58.000000 InternEvo-0.4.2/internlm/data/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6991 2024-04-11 07:14:24.000000 InternEvo-0.4.2/internlm/data/build_dataloader.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.502530 InternEvo-0.4.2/internlm/data/tokenized/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      418 2024-03-22 07:04:00.000000 InternEvo-0.4.2/internlm/data/tokenized/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15158 2024-03-15 18:58:58.000000 InternEvo-0.4.2/internlm/data/tokenized/batch_sampler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4401 2024-04-10 08:53:30.000000 InternEvo-0.4.2/internlm/data/tokenized/collaters.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1714 2024-03-15 18:58:58.000000 InternEvo-0.4.2/internlm/data/tokenized/dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1406 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/data/tokenized/dummy_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1894 2024-04-10 08:53:30.000000 InternEvo-0.4.2/internlm/data/tokenized/dummy_dataset_multimodal.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22498 2024-04-10 13:25:54.000000 InternEvo-0.4.2/internlm/data/tokenized/packed_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3740 2024-03-15 18:58:58.000000 InternEvo-0.4.2/internlm/data/tokenized/single_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      454 2024-03-15 18:58:58.000000 InternEvo-0.4.2/internlm/data/train_state.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1919 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/data/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.527469 InternEvo-0.4.2/internlm/eval/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       86 2024-03-15 18:58:58.000000 InternEvo-0.4.2/internlm/eval/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4999 2024-04-11 02:31:26.000000 InternEvo-0.4.2/internlm/eval/evaluation.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.552884 InternEvo-0.4.2/internlm/initialize/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      368 2024-01-25 08:28:55.000000 InternEvo-0.4.2/internlm/initialize/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1793 2024-01-25 08:28:55.000000 InternEvo-0.4.2/internlm/initialize/initialize_tensor.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5922 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/initialize/initialize_trainer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27458 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/initialize/launch.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.564725 InternEvo-0.4.2/internlm/initialize/legacy/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.2/internlm/initialize/legacy/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1592 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/initialize/legacy/launch.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.616577 InternEvo-0.4.2/internlm/model/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1124 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.644500 InternEvo-0.4.2/internlm/model/llava_modules/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-03 18:56:44.000000 InternEvo-0.4.2/internlm/model/llava_modules/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      499 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/llava_modules/clip_builder.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2674 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/llava_modules/clip_encoder.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1407 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/llava_modules/projector_builder.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.662130 InternEvo-0.4.2/internlm/model/losses/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       73 2024-03-15 18:58:58.000000 InternEvo-0.4.2/internlm/model/losses/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1786 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/losses/ce_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16344 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/metrics.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    23422 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/modeling_internlm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    54060 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/modeling_internlm2.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    51790 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/modeling_llama.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20872 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/modeling_llava.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    25417 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/modeling_moe.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.688245 InternEvo-0.4.2/internlm/model/modules/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.4.2/internlm/model/modules/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20370 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/modules/embedding.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10093 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/modules/mlp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    40600 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/modules/multi_head_attention.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.727318 InternEvo-0.4.2/internlm/model/moe/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      678 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/moe/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1198 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/model/moe/base_layer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2762 2024-03-18 08:30:10.000000 InternEvo-0.4.2/internlm/model/moe/experts.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20490 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/moe/gshard_layer.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.760648 InternEvo-0.4.2/internlm/model/moe/megablock/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-17 08:44:20.000000 InternEvo-0.4.2/internlm/model/moe/megablock/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8705 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/moe/megablock/megablock_dmoe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13643 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/moe/megablock/megablock_moe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2555 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/moe/megablock/mlp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11986 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/moe/megablock/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4494 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/moe/moe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2021 2024-03-18 08:30:10.000000 InternEvo-0.4.2/internlm/model/moe/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.786139 InternEvo-0.4.2/internlm/model/ops/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.4.2/internlm/model/ops/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6316 2024-05-06 07:30:03.000000 InternEvo-0.4.2/internlm/model/ops/fusion_ops_import_helper.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16010 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/ops/linear.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1500 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/model/ops/norm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24931 2024-05-06 07:30:03.000000 InternEvo-0.4.2/internlm/model/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.813860 InternEvo-0.4.2/internlm/monitor/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      193 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/monitor/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1479 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/monitor/alert.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10213 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/monitor/monitor.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      776 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/monitor/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.832296 InternEvo-0.4.2/internlm/solver/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-15 18:58:59.000000 InternEvo-0.4.2/internlm/solver/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10095 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/solver/activation_checkpoint.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.871281 InternEvo-0.4.2/internlm/solver/optimizer/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-22 07:04:01.000000 InternEvo-0.4.2/internlm/solver/optimizer/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1080 2024-01-25 08:28:55.000000 InternEvo-0.4.2/internlm/solver/optimizer/base_optimizer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9173 2024-03-22 08:39:35.000000 InternEvo-0.4.2/internlm/solver/optimizer/fsdp_optimizer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    42555 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/solver/optimizer/hybrid_zero_optim.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10132 2024-03-22 08:39:35.000000 InternEvo-0.4.2/internlm/solver/optimizer/store.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20351 2024-04-08 13:12:08.000000 InternEvo-0.4.2/internlm/solver/optimizer/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1280 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/solver/pipeline_utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.891251 InternEvo-0.4.2/internlm/solver/schedulers/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      272 2024-03-15 18:58:59.000000 InternEvo-0.4.2/internlm/solver/schedulers/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      844 2024-03-26 03:26:29.000000 InternEvo-0.4.2/internlm/solver/schedulers/beta2_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5940 2024-03-15 18:58:59.000000 InternEvo-0.4.2/internlm/solver/schedulers/lr_scheduler.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.909298 InternEvo-0.4.2/internlm/train/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      591 2024-05-06 07:30:03.000000 InternEvo-0.4.2/internlm/train/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22392 2024-05-06 07:30:03.000000 InternEvo-0.4.2/internlm/train/pipeline.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3567 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/train/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.982081 InternEvo-0.4.2/internlm/utils/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.2/internlm/utils/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9244 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/utils/common.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6321 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/utils/gputest.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2112 2024-04-10 11:16:15.000000 InternEvo-0.4.2/internlm/utils/logger.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4156 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/utils/megatron_timers.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4061 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/utils/parallel.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2423 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/utils/registry.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24734 2024-03-26 03:26:29.000000 InternEvo-0.4.2/internlm/utils/simple_memory_profiler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    46133 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/utils/storage_manager.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3126 2024-03-15 18:58:59.000000 InternEvo-0.4.2/internlm/utils/timeout.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      709 2024-05-03 18:58:40.000000 InternEvo-0.4.2/internlm/utils/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7117 2024-04-07 02:41:24.000000 InternEvo-0.4.2/internlm/utils/writer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-06 07:52:31.911655 InternEvo-0.4.2/setup.cfg
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1191 2024-05-06 07:30:03.000000 InternEvo-0.4.2/setup.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:34.992569 InternEvo-0.4.2/tests/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.2/tests/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4536 2024-05-03 18:58:40.000000 InternEvo-0.4.2/tests/common_fixture.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:35.012694 InternEvo-0.4.2/tests/test_core/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.2/tests/test_core/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5841 2024-04-24 06:39:45.000000 InternEvo-0.4.2/tests/test_core/test_pipeline.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6978 2024-05-03 18:58:40.000000 InternEvo-0.4.2/tests/test_core/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 07:50:35.072025 InternEvo-0.4.2/tests/test_training/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5750 2024-04-12 05:43:59.000000 InternEvo-0.4.2/tests/test_training/7B_check_acc.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6360 2024-04-07 02:41:25.000000 InternEvo-0.4.2/tests/test_training/7B_check_init.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:46.000000 InternEvo-0.4.2/tests/test_training/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7882 2024-05-03 18:58:40.000000 InternEvo-0.4.2/tests/test_training/test_forward_output_no_fa.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11700 2024-05-03 18:58:40.000000 InternEvo-0.4.2/tests/test_training/test_load_ckpt_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14416 2024-05-03 18:58:40.000000 InternEvo-0.4.2/tests/test_training/test_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3845 2024-05-03 18:58:40.000000 InternEvo-0.4.2/tests/test_training/test_no_fa_train_temp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6763 2024-05-03 18:58:40.000000 InternEvo-0.4.2/tests/test_training/test_norm_weight.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12557 2024-05-03 18:58:40.000000 InternEvo-0.4.2/tests/test_training/test_swap_nb_loss_and_gradnorm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14000 2024-05-03 18:58:40.000000 InternEvo-0.4.2/tests/test_training/train_CI.py
```

### Comparing `InternEvo-0.4.0.dev20240403/InternEvo.egg-info/PKG-INFO` & `InternEvo-0.4.2/InternEvo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternEvo
-Version: 0.4.0.dev20240403
+Version: 0.4.2
 Summary: an open-sourced lightweight training framework aims to support model pre-training without the need for extensive dependencies
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: InternEvo Version: 0.4.0.dev20240403 Summary: an
-open-sourced lightweight training framework aims to support model pre-training
-without the need for extensive dependencies Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Education Classifier: Intended Audience :: Science/Research
-Description-Content-Type: text/markdown License-File: LICENSE # InternEvo
+Metadata-Version: 2.1 Name: InternEvo Version: 0.4.2 Summary: an open-sourced
+lightweight training framework aims to support model pre-training without the
+need for extensive dependencies Classifier: Programming Language :: Python ::
+3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Education Classifier: Intended Audience :: Science/Research Description-
+Content-Type: text/markdown License-File: LICENSE # InternEvo
                              [./doc/imgs/logo.svg]
                                       Â 
                                  IInntteerrnnEEvvoo _H_O_T
                                       Â 
   [![Documentation Status](https://readthedocs.org/projects/internevo/badge/
 ?version=latest)](https://internevo.readthedocs.io/zh_CN/latest/?badge=latest)
 [![license](./doc/imgs/license.svg)](./LICENSE) [ðUsage](./doc/en/usage.md)
```

### Comparing `InternEvo-0.4.0.dev20240403/InternEvo.egg-info/SOURCES.txt` & `InternEvo-0.4.2/InternEvo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 InternEvo.egg-info/PKG-INFO
 InternEvo.egg-info/SOURCES.txt
 InternEvo.egg-info/dependency_links.txt
+InternEvo.egg-info/requires.txt
 InternEvo.egg-info/top_level.txt
 internlm/__init__.py
 internlm/accelerator/__init__.py
 internlm/accelerator/abstract_accelerator.py
 internlm/accelerator/cuda_accelerator.py
 internlm/accelerator/dipu_accelerator.py
 internlm/accelerator/npu_accelerator.py
@@ -40,14 +41,15 @@
 internlm/data/train_state.py
 internlm/data/utils.py
 internlm/data/tokenized/__init__.py
 internlm/data/tokenized/batch_sampler.py
 internlm/data/tokenized/collaters.py
 internlm/data/tokenized/dataset.py
 internlm/data/tokenized/dummy_dataset.py
+internlm/data/tokenized/dummy_dataset_multimodal.py
 internlm/data/tokenized/packed_dataset.py
 internlm/data/tokenized/single_dataset.py
 internlm/eval/__init__.py
 internlm/eval/evaluation.py
 internlm/initialize/__init__.py
 internlm/initialize/initialize_tensor.py
 internlm/initialize/initialize_trainer.py
@@ -55,16 +57,21 @@
 internlm/initialize/legacy/__init__.py
 internlm/initialize/legacy/launch.py
 internlm/model/__init__.py
 internlm/model/metrics.py
 internlm/model/modeling_internlm.py
 internlm/model/modeling_internlm2.py
 internlm/model/modeling_llama.py
+internlm/model/modeling_llava.py
 internlm/model/modeling_moe.py
 internlm/model/utils.py
+internlm/model/llava_modules/__init__.py
+internlm/model/llava_modules/clip_builder.py
+internlm/model/llava_modules/clip_encoder.py
+internlm/model/llava_modules/projector_builder.py
 internlm/model/losses/__init__.py
 internlm/model/losses/ce_loss.py
 internlm/model/modules/__init__.py
 internlm/model/modules/embedding.py
 internlm/model/modules/mlp.py
 internlm/model/modules/multi_head_attention.py
 internlm/model/moe/__init__.py
@@ -75,14 +82,15 @@
 internlm/model/moe/utils.py
 internlm/model/moe/megablock/__init__.py
 internlm/model/moe/megablock/megablock_dmoe.py
 internlm/model/moe/megablock/megablock_moe.py
 internlm/model/moe/megablock/mlp.py
 internlm/model/moe/megablock/utils.py
 internlm/model/ops/__init__.py
+internlm/model/ops/fusion_ops_import_helper.py
 internlm/model/ops/linear.py
 internlm/model/ops/norm.py
 internlm/monitor/__init__.py
 internlm/monitor/alert.py
 internlm/monitor/monitor.py
 internlm/monitor/utils.py
 internlm/solver/__init__.py
```

### Comparing `InternEvo-0.4.0.dev20240403/LICENSE` & `InternEvo-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/PKG-INFO` & `InternEvo-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternEvo
-Version: 0.4.0.dev20240403
+Version: 0.4.2
 Summary: an open-sourced lightweight training framework aims to support model pre-training without the need for extensive dependencies
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: InternEvo Version: 0.4.0.dev20240403 Summary: an
-open-sourced lightweight training framework aims to support model pre-training
-without the need for extensive dependencies Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Education Classifier: Intended Audience :: Science/Research
-Description-Content-Type: text/markdown License-File: LICENSE # InternEvo
+Metadata-Version: 2.1 Name: InternEvo Version: 0.4.2 Summary: an open-sourced
+lightweight training framework aims to support model pre-training without the
+need for extensive dependencies Classifier: Programming Language :: Python ::
+3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Education Classifier: Intended Audience :: Science/Research Description-
+Content-Type: text/markdown License-File: LICENSE # InternEvo
                              [./doc/imgs/logo.svg]
                                       Â 
                                  IInntteerrnnEEvvoo _H_O_T
                                       Â 
   [![Documentation Status](https://readthedocs.org/projects/internevo/badge/
 ?version=latest)](https://internevo.readthedocs.io/zh_CN/latest/?badge=latest)
 [![license](./doc/imgs/license.svg)](./LICENSE) [ðUsage](./doc/en/usage.md)
```

### Comparing `InternEvo-0.4.0.dev20240403/README.md` & `InternEvo-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/accelerator/abstract_accelerator.py` & `InternEvo-0.4.2/internlm/accelerator/abstract_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/accelerator/cuda_accelerator.py` & `InternEvo-0.4.2/internlm/accelerator/cuda_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/accelerator/dipu_accelerator.py` & `InternEvo-0.4.2/internlm/accelerator/dipu_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/accelerator/npu_accelerator.py` & `InternEvo-0.4.2/internlm/accelerator/npu_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/apis/inference.py` & `InternEvo-0.4.2/internlm/apis/inference.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/checkpoint/checkpoint_manager.py` & `InternEvo-0.4.2/internlm/checkpoint/checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/checkpoint/components.py` & `InternEvo-0.4.2/internlm/checkpoint/components.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/checkpoint/utils.py` & `InternEvo-0.4.2/internlm/checkpoint/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,23 +54,20 @@
     Returns:
         {
             '{name}': {'dim': int}
         }
         where name is the name of the module, and all parameters under this module are
         concatenated along the dimension 'dim'.
     """
-
-    from flash_attn.modules.embedding import VocabParallelEmbedding
-
     topos = {}
-    for name, module in model.named_modules():
-        # If it does not meet these conditions, it is shared between various tp/dp, and it is necessary to assert
+    for name, module in model.named_modules():  # pylint: disable=W0612
+        # TODO: If it does not meet these conditions, it is shared between various tp/dp, and it is necessary to assert
         # that they are consistent.
-        if isinstance(module, VocabParallelEmbedding):
-            topos[name] = {"dim": 0}
+        # In order to be compatible with CI, this function will not be deleted for now.
+        pass
     return topos
 
 
 def process_load_info(load_info):
     load_content_str = ""
     load_ckpt_folder = load_info["path"]
     load_content = load_info["content"]
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/core/communication/__init__.py` & `InternEvo-0.4.2/internlm/core/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/core/communication/isp.py` & `InternEvo-0.4.2/internlm/core/communication/isp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/core/communication/p2p.py` & `InternEvo-0.4.2/internlm/core/communication/p2p.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/core/communication/utils.py` & `InternEvo-0.4.2/internlm/core/communication/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -214,18 +214,14 @@
             # instead implement support for weight parallelism of embedding and head layers within the ISP.
 
             # NOTE: Although the layernorm layer does not have explicit processing,
             # both ISPCommunicator and ParamAsyncBcastHandler handle transformer blocks as granularity,
             # so everything is fine.
 
             embedding_head_cls = (Embedding1D, BaseScaleColumnParallelLinear)
-            if gpc.config.use_cuda_flash_attn:
-                from flash_attn.modules.embedding import ParallelGPT2Embeddings
-
-                embedding_head_cls = (Embedding1D, ParallelGPT2Embeddings, BaseScaleColumnParallelLinear)
 
             if isp_communicator is None or isinstance(block, embedding_head_cls):
                 block.register_forward_pre_hook(_pre_forward_hook)
         if isp_communicator:
             isp_communicator.register_prerequisite_for_forward_prefetch_hooks(_pre_forward_hook)
 
     def get_rank_by_param(self, param) -> int:
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/core/context/__init__.py` & `InternEvo-0.4.2/internlm/core/context/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/core/context/parallel_context.py` & `InternEvo-0.4.2/internlm/core/context/parallel_context.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/core/context/process_group_initializer.py` & `InternEvo-0.4.2/internlm/core/context/process_group_initializer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/core/context/random.py` & `InternEvo-0.4.2/internlm/core/context/random.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/core/engine.py` & `InternEvo-0.4.2/internlm/core/engine.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/core/gradient_handler.py` & `InternEvo-0.4.2/internlm/core/gradient_handler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/core/naive_amp.py` & `InternEvo-0.4.2/internlm/core/naive_amp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/core/scheduler/base_scheduler.py` & `InternEvo-0.4.2/internlm/core/scheduler/base_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/core/scheduler/no_pipeline_scheduler.py` & `InternEvo-0.4.2/internlm/core/scheduler/no_pipeline_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/core/scheduler/pipeline_scheduler.py` & `InternEvo-0.4.2/internlm/core/scheduler/pipeline_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/core/trainer.py` & `InternEvo-0.4.2/internlm/core/trainer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/data/build_dataloader.py` & `InternEvo-0.4.2/internlm/data/build_dataloader.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,41 +9,55 @@
 from internlm.data.tokenized.batch_sampler import (
     StaticBatchSampler,
     get_dpsampler_dataloader,
 )
 from internlm.data.tokenized.collaters import jsonl_ds_collate_fn, packed_collate_fn
 from internlm.data.tokenized.dataset import get_dataset_dict
 from internlm.data.tokenized.dummy_dataset import RandomDataset
+from internlm.data.tokenized.dummy_dataset_multimodal import RandomDatasetMultimodal
 from internlm.data.tokenized.packed_dataset import (
     PackedDatasetWithCut,
     PackedDatasetWithoutCuSeqlen,
+    PackedDatasetWithPadForMultimodal,
     get_packed_dataset_without_short_length,
 )
 from internlm.data.utils import get_dataset_type_ids_map
 from internlm.utils.logger import get_logger
 
 # global llm logger
 logger = get_logger(__file__)
 
 
 def get_tokenized_train_loader_items(data_cfg):
     """Get the training data loader for tokenized dataset."""
     if data_cfg.get("train_folder", None) is None:
-        train_ds = RandomDataset(
-            num_samples=1000000, max_len=data_cfg.seq_len, fixed_seqlen=data_cfg.fixed_random_dataset_seqlen
-        )
-
-        if data_cfg.pack_sample_into_one:
-            train_ds = PackedDatasetWithoutCuSeqlen(
+        if data_cfg.get("is_multimodal", False):
+            image_token_size = int(data_cfg.image_size // data_cfg.patch_size) ** 2
+            train_ds = RandomDatasetMultimodal(
+                num_samples=100000,
+                max_len=data_cfg.seq_len,
+                image_size=data_cfg.image_size,
+                image_token_size=image_token_size,
+            )
+            train_ds = PackedDatasetWithPadForMultimodal(
                 train_ds, max_length_per_sample=data_cfg.seq_len, packed_length=data_cfg.packed_length
             )
         else:
-            train_ds = PackedDatasetWithCut(
-                train_ds, max_length_per_sample=data_cfg.seq_len, packed_length=data_cfg.packed_length
+            train_ds = RandomDataset(
+                num_samples=1000000, max_len=data_cfg.seq_len, fixed_seqlen=data_cfg.fixed_random_dataset_seqlen
             )
+
+            if data_cfg.pack_sample_into_one:
+                train_ds = PackedDatasetWithoutCuSeqlen(
+                    train_ds, max_length_per_sample=data_cfg.seq_len, packed_length=data_cfg.packed_length
+                )
+            else:
+                train_ds = PackedDatasetWithCut(
+                    train_ds, max_length_per_sample=data_cfg.seq_len, packed_length=data_cfg.packed_length
+                )
     else:
         train_ds = get_packed_dataset_without_short_length(
             folder=data_cfg.train_folder,
             packed_length=data_cfg.packed_length,
             max_length_per_sample=data_cfg.seq_len,
             show_progress=dist.get_rank() == 0,
             min_length=data_cfg.get("min_length", 0),
@@ -65,19 +79,28 @@
 
     return train_ds, train_sampler, train_collate_fn
 
 
 def get_tokenized_valid_loader_items(data_cfg):
     """Get the validation data loader for tokenized dataset."""
     if not data_cfg.valid_folder:
-        valid_ds = RandomDataset(
-            num_samples=gpc.get_world_size(ParallelMode.DATA) * 500,
-            max_len=data_cfg.seq_len,
-            fixed_seqlen=data_cfg.fixed_random_dataset_seqlen,
-        )
+        if data_cfg.get("is_multimodal", False):
+            image_token_size = int(data_cfg.image_size // data_cfg.patch_size) ** 2
+            valid_ds = RandomDatasetMultimodal(
+                num_samples=gpc.get_world_size(ParallelMode.DATA) * 500,
+                max_len=data_cfg.seq_len,
+                image_size=data_cfg.image_size,
+                image_token_size=image_token_size,
+            )
+        else:
+            valid_ds = RandomDataset(
+                num_samples=gpc.get_world_size(ParallelMode.DATA) * 500,
+                max_len=data_cfg.seq_len,
+                fixed_seqlen=data_cfg.fixed_random_dataset_seqlen,
+            )
     else:
         valid_ds = get_dataset_dict(folder=data_cfg.valid_folder, split="")
 
     if not isinstance(valid_ds, dict):
         valid_ds = {"val": valid_ds}
 
     valid_collate_fn = partial(jsonl_ds_collate_fn, max_length_per_sample=data_cfg.seq_len)
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/data/tokenized/batch_sampler.py` & `InternEvo-0.4.2/internlm/data/tokenized/batch_sampler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/data/tokenized/collaters.py` & `InternEvo-0.4.2/internlm/data/tokenized/collaters.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,30 +18,35 @@
         Tuple[Dict[str, torch.Tensor], torch.Tensor]: A tuple containing a dictionary of tensors with "input_ids",
             "cu_seqlens", "indexes", and "type_ids" keys, and the tensor of padded "labels".
 
     Raises:
         AssertionError: If the length of a sample is not equal to packed_length.
         AssertionError: If the shape of the padded "input_ids" tensor does not have the correct shape.
     """
-
-    xs, ys, cu_seqlens, indexes, ts = [], [], [], [], []
+    have_image = False
+    xs, ys, cu_seqlens, indexes, ts, images = [], [], [], [], [], []
     for b in batch:
         assert (
             len(b["tokens"]) == packed_length
         ), f"length of a sample should be equal to packed_length, but got {len(b['tokens'])} and {packed_length})"
         assert (
             len(b["labels"]) == packed_length
         ), f"length of a sample should be equal to packed_length, but got {len(b['labels'])} and {packed_length})"
         assert (
             len(b["type_ids"]) == packed_length
         ), f"length of a sample should be equal to packed_length, but got {len(b['type_ids'])} and {packed_length})"
 
         tokens = [abs(w) for w in b["tokens"]]
         labels = [w if w > 0 else -100 for w in b["labels"]]
 
+        if b.get("images", None) is not None:
+            have_image = True
+            cur_images = torch.stack(b["images"])
+            images.append(cur_images)
+
         xs.append(torch.LongTensor(tokens))
         # The labels have been shifted here, so they are aligned with the output corresponding to the token
         ys.append(torch.LongTensor(labels))
         ts.append(torch.LongTensor(b["type_ids"]))
         cu_seqlens.append(torch.IntTensor(b["cu_seqlens"]))
         indexes.append(torch.LongTensor(b["indexes"]))
 
@@ -49,16 +54,18 @@
     ys = torch.nn.utils.rnn.pad_sequence(ys, batch_first=True, padding_value=-100)
     ts = torch.nn.utils.rnn.pad_sequence(ts, batch_first=True, padding_value=0)
     indexes = torch.stack(indexes, dim=0)
     if len(set(map(len, cu_seqlens))) == 1:  # if has uniform length, then stack to save device transfer time
         cu_seqlens = torch.stack(cu_seqlens, dim=0)
 
     assert xs.shape[1] == packed_length, (xs.shape[1], packed_length)
-
-    return {"input_ids": xs, "cu_seqlens": cu_seqlens, "indexes": indexes, "type_ids": ts}, ys
+    if have_image:
+        return {"input_ids": xs, "cu_seqlens": cu_seqlens, "indexes": indexes, "type_ids": ts, "images": images}, ys
+    else:
+        return {"input_ids": xs, "cu_seqlens": cu_seqlens, "indexes": indexes, "type_ids": ts}, ys
 
 
 def jsonl_ds_collate_fn(batch, max_length_per_sample):
     """
     Collate function for json dataset.
 
     Args:
@@ -67,22 +74,29 @@
         max_length_per_sample (int): The length of output sequence.
 
     Returns:
         Tuple[Dict[str, torch.Tensor], torch.Tensor]: A tuple containing a dictionary of tensors with "input_ids",
         and the tensor of padded "labels".
 
     """
-    xs, ys = [], []
+    xs, ys, images = [], [], []
+    have_image = False
     for x in batch:
         x["tokens"] = x["tokens"][:max_length_per_sample]
         tokens = [abs(w) for w in x["tokens"]]
         labels = [w if w > 0 else -100 for w in x["tokens"]]
         labels = labels[1:] + [-100]
+        if x.get("images", None) is not None:
+            have_image = True
+            cur_images = torch.stack(x["images"])
+            images.append(cur_images)
         xs.append(torch.as_tensor(tokens))
         ys.append(torch.as_tensor(labels))  # y has been shifted
     xs = torch.nn.utils.rnn.pad_sequence(xs, batch_first=True)
     ys = torch.nn.utils.rnn.pad_sequence(ys, batch_first=True, padding_value=-100)
 
     xs = torch.cat([xs, xs.new_zeros(len(xs), max_length_per_sample - len(xs[0]))], dim=-1)
     ys = torch.cat([ys, ys.new_full((len(ys), max_length_per_sample - len(ys[0])), fill_value=-100)], dim=-1)
-
-    return {"input_ids": xs}, ys
+    if have_image:
+        return {"input_ids": xs, "images": images}, ys
+    else:
+        return {"input_ids": xs}, ys
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/data/tokenized/dataset.py` & `InternEvo-0.4.2/internlm/data/tokenized/dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/data/tokenized/dummy_dataset.py` & `InternEvo-0.4.2/internlm/data/tokenized/dummy_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/data/tokenized/packed_dataset.py` & `InternEvo-0.4.2/internlm/data/tokenized/packed_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -374,15 +374,15 @@
             type_ids.extend([sample.get("type_id", 0)] * len(chunk))
             cu_seqlens.append(cu_seqlens[-1] + len(chunk))
             indexes.extend(list(range(length)))
             pre_pos = pre_pos + 1
 
         if cu_seqlens[-1] != self.packed_length:
             pack = pack + [0] * (self.packed_length - cu_seqlens[-1])
-            labels = labels + [0] * (self.packed_length - cu_seqlens[-1])
+            labels = labels + [-100] * (self.packed_length - cu_seqlens[-1])
             type_ids = type_ids + [0] * (self.packed_length - cu_seqlens[-1])
             indexes.extend(list(range(self.packed_length - cu_seqlens[-1])))
             cu_seqlens.append(self.packed_length)
 
         assert len(pack) == self.packed_length
 
         out = {"tokens": pack, "cu_seqlens": cu_seqlens, "indexes": indexes, "labels": labels, "type_ids": type_ids}
@@ -474,7 +474,129 @@
         logger.info(
             f"Find `{len(datasets)}` datasets, \
             {len(dataset)} samples, \
             delete `{delete_samples}` because of short length",
         )
 
     return dataset
+
+
+class PackedDatasetWithPadForMultimodal(PackedDataset):
+    """
+    The class PackedDataset takes in a dataset and aggregates samples of different
+    lengths together based on the packed_length using pad mode.
+
+    packed_length = 5
+    max_length_per_sample = 3
+
+    [1, 2]
+    [6, 7]
+    [3, 4, 5]
+    [8, 9, 10, 11, 12, 13]
+
+    --->
+    [1, 2, 6, 7, 0]
+    [3 ,4, 5, 0, 0]
+    [8, 9, 10, 0, 0]
+
+    Args:
+        dataset: The original dataset to pack.
+        max_length_per_sample: The maximum length of each original sample. Default is 2048.
+        packed_length: The length of each packed sample. Default is 4096.
+        padding_idx: The token id of padding. Default is 0.
+    """
+
+    def __init__(
+        self,
+        dataset,
+        max_length_per_sample: int = 2048,
+        packed_length: int = 4096,
+        padding_idx: int = 0,
+        image_token_id: int = 200000,
+    ):
+        super().__init__(dataset, max_length_per_sample, packed_length)
+        self.padding_idx = padding_idx
+        self.sample_indices, self.belongs = self.accu_sample_len(self.seed)
+        self.num_tokens = sum(self.lengths)
+        self.image_token_id = image_token_id
+
+    def get_dataset_name(self):
+        return self.dataset.get_dataset_name()
+
+    def accu_sample_len(self, seed=None):
+        """accumulative length of samples"""
+        if seed is not None:
+            rng = np.random.RandomState(seed)
+        else:
+            rng = np.random.RandomState(self.seed - 1)
+
+        sample_indices = np.arange(len(self.lengths))
+        rng.shuffle(sample_indices)
+        len_samples_shuffled = list(map(self.lengths.__getitem__, sample_indices))
+        belongs = np.zeros(len(self.lengths), dtype=np.int32)
+        cur_num = 0
+        cur_tot_len = 0
+        last_pos = 0
+        for idx, cur_sample_len in enumerate(len_samples_shuffled):
+            cur_sample_len = min(cur_sample_len, self.max_length_per_sample)
+            if cur_tot_len + cur_sample_len > self.packed_length:
+                cur_tot_len = 0
+                belongs[last_pos:idx] = cur_num
+                cur_num += 1
+                last_pos = idx
+            cur_tot_len += cur_sample_len
+        if cur_tot_len != 0:
+            belongs[last_pos:] = cur_num
+            cur_tot_len = 0
+            cur_num += 1
+        return sample_indices, belongs
+
+    def __len__(self):
+        return self.belongs[-1]
+
+    def build_pack(self, index):
+
+        pack, cu_seqlens, indexes, labels, type_ids, images = [], [0], [], [], [], []
+
+        start_pos = np.searchsorted(self.belongs, index, "left")
+        end_pos = np.searchsorted(self.belongs, index, "right")
+        assert self.belongs[end_pos - 1] == self.belongs[start_pos] and (
+            end_pos >= len(self.belongs) or self.belongs[end_pos] == self.belongs[start_pos] + 1
+        )
+        cur_samples = self.sample_indices[start_pos:end_pos]
+
+        for sample_idx in cur_samples:
+            sample = self.dataset[sample_idx]
+            length = min(len(sample["tokens"]), self.max_length_per_sample)
+            cur_images = sample["images"]
+            images.extend(cur_images)
+            chunk = sample["tokens"][:length]
+            pack.extend(chunk)
+            cu_seqlens.append(cu_seqlens[-1] + len(chunk))
+            _labels = deepcopy(chunk)
+            _labels = list(_labels[1:]) + [-100]
+            for i in range(len(_labels)):
+                if _labels[i] == self.image_token_id:
+                    _labels[i] = -100
+            labels.extend(_labels)
+            type_ids.extend([sample.get("type_id", 0)] * len(chunk))
+            indexes.extend(list(range(length)))
+
+        if cu_seqlens[-1] != self.packed_length:
+            pack = pack + [self.padding_idx] * (self.packed_length - cu_seqlens[-1])
+            labels = labels + [-100] * (self.packed_length - cu_seqlens[-1])
+            type_ids = type_ids + [0] * (self.packed_length - cu_seqlens[-1])
+            indexes.extend([0] * (self.packed_length - cu_seqlens[-1]))
+            cu_seqlens.append(self.packed_length)
+
+        out = {
+            "tokens": pack,
+            "images": images,
+            "cu_seqlens": cu_seqlens,
+            "indexes": indexes,
+            "labels": labels,
+            "type_ids": type_ids,
+        }
+        return out
+
+    def build_unpack(self, index):
+        raise NotImplementedError
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/data/tokenized/single_dataset.py` & `InternEvo-0.4.2/internlm/data/tokenized/single_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/data/utils.py` & `InternEvo-0.4.2/internlm/data/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/eval/evaluation.py` & `InternEvo-0.4.2/internlm/eval/evaluation.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
 def evaluate_on_val_dls(
     trainer,
     val_dls,
     writer,
     logger,
     step_count,
-    update_panel: bool = False,
     streaming: bool = False,
 ):
     val_metric = AccPerplex(
         device=get_current_device(),
         tp_pg=gpc.get_group(ParallelMode.TENSOR),
         dp_pg=gpc.get_group(ParallelMode.DATA),
     )
@@ -119,25 +118,14 @@
                     f"val/{val_name}_acc": val_res["acc"],
                     f"val/{val_name}_plex": val_res["perplexity"],
                 }
 
                 for key, value in infos.items():
                     writer.add_scalar(key=key, value=value, step=step_count)
 
-                if update_panel:
-                    logger.info(
-                        f"Validation on {val_name}: " + " ".join([f"{key}={value}" for key, value in infos.items()]),
-                        extra={
-                            "step": step_count,
-                            "val_loss": val_loss,
-                            "val_acc": val_res["acc"],
-                            "val_perplexity": val_res["perplexity"],
-                        },
-                    )
-                else:
-                    logger.info(
-                        f"Validation on {val_name}: " + " ".join([f"{key}={value}" for key, value in infos.items()])
-                    )
+                logger.info(
+                    f"Validation on {val_name}: " + " ".join([f"{key}={value}" for key, value in infos.items()])
+                )
 
         trainer.train()
         internlm_accelerator.empty_cache()
         dist.barrier()
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/initialize/initialize_tensor.py` & `InternEvo-0.4.2/internlm/initialize/initialize_tensor.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/initialize/initialize_trainer.py` & `InternEvo-0.4.2/internlm/initialize/initialize_trainer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/initialize/launch.py` & `InternEvo-0.4.2/internlm/initialize/launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,23 +317,17 @@
         logger.info("+" * 15 + " beta2_scheduler Info " + "+" * 15)  # pylint: disable=W1201
         logger.info(f"beta2_scheduler: {gpc.config.beta2_scheduler}")
 
     # process the model config
     if "use_flash_attn" not in gpc.config.model:
         gpc.config.model._add_item("use_flash_attn", True)
 
-    gpc.config["use_cuda_flash_attn"] = False
-    if gpc.config.model.use_flash_attn and (
-        internlm_accelerator.get_accelerator_backend() in [AcceleratorType.GPU, AcceleratorType.DIPU]
-    ):
-        gpc.config["use_cuda_flash_attn"] = True
-
     old_parallel_output = gpc.config.model.get("parallel_output", None)
     # Try to change user setting
-    if not gpc.config.use_cuda_flash_attn:
+    if internlm_accelerator.get_accelerator_backend() is not AcceleratorType.GPU:
         gpc.config.model.update({"parallel_output": False})
         if old_parallel_output is True and gpc.is_rank_for_log():
             logger.warning(
                 "'parallel_output' is converted from 'True' to 'False'."
                 "Because 'parallel_output' only support by FlashCrossEntropyLoss."
                 "Please make sure you are using flash attention in cuda device."
             )
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/initialize/legacy/launch.py` & `InternEvo-0.4.2/internlm/initialize/legacy/launch.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/__init__.py` & `InternEvo-0.4.2/internlm/model/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
 from .metrics import AccPerplex
 from .modeling_internlm import build_model_with_cfg
 from .modeling_internlm2 import build_model_with_cfg as build_model_with_cfg2
 from .modeling_llama import build_model_with_cfg as build_model_with_llama_cfg
+from .modeling_llava import build_model_with_cfg as build_model_with_llava_cfg
 from .modeling_moe import build_model_with_moe_cfg
 from .modules.embedding import Embedding1D, RotaryEmbedding
 from .modules.mlp import FeedForward
 from .modules.multi_head_attention import MHA, DistributedAttention
 from .moe.moe import MoE
 from .ops.linear import RewardModelLinear, ScaleColumnParallelLinear
 from .utils import gather_forward_split_backward
@@ -24,8 +25,9 @@
     "MHA",
     "DistributedAttention",
     "gather_forward_split_backward",
     "build_model_with_cfg",
     "build_model_with_cfg2",
     "build_model_with_moe_cfg",
     "build_model_with_llama_cfg",
+    "build_model_with_llava_cfg",
 ]
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/metrics.py` & `InternEvo-0.4.2/internlm/model/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from typing import Callable, List, Optional
 
 import torch
-from torch import nn
 
 from internlm.accelerator import AcceleratorType, get_accelerator
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
+from internlm.model.ops.fusion_ops_import_helper import (
+    internlm_init_CrossEntropyLoss,
+    try_import_scatter_sum,
+)
 from internlm.utils.common import SchedulerHook, get_current_device
 from internlm.utils.megatron_timers import megatron_timer as timer
 
-try:
-    from torch_scatter import scatter as cuda_scatter
-except (ModuleNotFoundError, ImportError):
-    pass
-
 internlm_accelerator = get_accelerator()
+scatter_sum = try_import_scatter_sum()
 
 
 def broadcast(src: torch.Tensor, other: torch.Tensor, dim: int):
     if dim < 0:
         dim = other.dim() + dim
     if src.dim() == 1:
         for _ in range(0, dim):
@@ -85,19 +84,15 @@
         if dataset_types is not None:
             self.dataset_types = dataset_types
             self.total_type_count = len(dataset_types)
             self.ds_right = torch.zeros(self.total_type_count, dtype=torch.long, device=device)
             self.ds_tokens = torch.zeros(self.total_type_count, dtype=torch.long, device=device)
 
         self.loss_with_type_id = LossWithTypeId(device, dp_pg, dataset_types)
-
-        if internlm_accelerator.get_accelerator_backend() in [AcceleratorType.GPU, AcceleratorType.DIPU]:
-            self.scatter_sum = cuda_scatter
-        else:
-            self.scatter_sum = vanilla_scatter
+        self.scatter_sum = scatter_sum if scatter_sum else vanilla_scatter
 
     def set_current_type_ids(self, type_ids: torch.Tensor):
         self.batch_shift = 0
         self.type_ids = type_ids.to(get_current_device())
 
     def set_cu_seqlens(self, cu_seqlens: List):
         self.cu_seqlens = cu_seqlens
@@ -258,29 +253,21 @@
 
         if dataset_types is not None:
             self.dataset_types = dataset_types
             self.total_type_count = len(dataset_types)
             self.ds_loss = torch.zeros(self.total_type_count, dtype=torch.float, device=device)
             self.ds_token_num = torch.zeros(self.total_type_count, dtype=torch.float, device=device)
 
-        if gpc.config.use_cuda_flash_attn and AcceleratorType.GPU == get_accelerator():
-            from flash_attn.losses.cross_entropy import (
-                CrossEntropyLoss as FlashCrossEntropyLoss,
-            )
-
-            self.loss_fn = FlashCrossEntropyLoss(
-                reduction="none", inplace_backward=True, process_group=gpc.get_group(ParallelMode.TENSOR)
-            )
-        else:
-            self.loss_fn = nn.CrossEntropyLoss(reduction="none")
-
-        if internlm_accelerator.get_accelerator_backend() in [AcceleratorType.GPU, AcceleratorType.DIPU]:
-            self.scatter_sum = cuda_scatter
-        else:
-            self.scatter_sum = vanilla_scatter
+        self.loss_fn = internlm_init_CrossEntropyLoss(
+            parallel_output=gpc.config.model.parallel_output,
+            reduction="none",
+            inplace_backward=True,
+            process_group=gpc.get_group(ParallelMode.TENSOR),
+        )
+        self.scatter_sum = scatter_sum if scatter_sum else vanilla_scatter
 
     def update(self, logits, labels, type_ids=None):
         with torch.no_grad():
             if isinstance(logits, (list, tuple)):
                 logits = logits[0]
             logits = logits.contiguous().view(-1, logits.size(-1))
             labels = labels.contiguous().view(-1)
@@ -316,14 +303,15 @@
             if hasattr(self, "total_type_count"):
                 torch.distributed.all_reduce(self.ds_loss, op=torch.distributed.ReduceOp.SUM, group=self.dp_pg)
                 torch.distributed.all_reduce(self.ds_token_num, op=torch.distributed.ReduceOp.SUM, group=self.dp_pg)
 
         loss = round((self.loss / self.token_num).item(), 4)
         res = {
             "loss_from_metric": loss,
+            "real_token_num": self.token_num.item(),
         }
         if hasattr(self, "total_type_count"):
             ds_loss = {}
             for i in range(self.total_type_count):
                 ds_loss[f"loss/{self.dataset_types[i]}"] = round((self.ds_loss[i] / self.ds_token_num[i]).item(), 4)
             res.update(ds_loss)
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/modeling_internlm.py` & `InternEvo-0.4.2/internlm/model/modeling_internlm.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from internlm.core.context import ParallelMode
 from internlm.core.context.parallel_context import global_context as gpc
 from internlm.core.naive_amp import set_output_attr_to_module
 from internlm.initialize.initialize_tensor import normal_, scaled_init_method_normal
 from internlm.model.modules.embedding import Embedding1D
 from internlm.model.modules.mlp import get_mlp_cls
 from internlm.model.modules.multi_head_attention import MHA
+from internlm.model.ops.fusion_ops_import_helper import try_import_RMSNorm
 from internlm.model.ops.linear import RewardModelLinear, ScaleColumnParallelLinear
 from internlm.model.utils import (
     gather_forward_split_backward,
     split_forward_gather_backward,
-    try_import_RMSNorm,
 )
 from internlm.solver.activation_checkpoint import activation_checkpoint
 from internlm.solver.pipeline_utils import partition_uniform
 from internlm.utils.common import filter_kwargs, get_current_device
 from internlm.utils.logger import get_logger
 from internlm.utils.registry import MODEL_INITIALIZER
 
@@ -127,32 +127,14 @@
                 bias=False,
                 device=device,
                 dtype=dtype,
                 mlp_layer_fusion=mlp_layer_fusion,
                 sequence_parallel=gpc.config.parallel.sequence_parallel,
                 multiple_of=multiple_of,
             )
-        else:
-            assert gpc.config.use_cuda_flash_attn is True
-            from flash_attn.modules.mlp import ParallelFusedMLP
-
-            self.mlp = ParallelFusedMLP(
-                hidden_size,
-                int(hidden_size * mlp_ratio),
-                out_features=hidden_size,
-                activation="gelu_approx",
-                process_group=gpc.get_group(parallel_mode),
-                bias1=False,
-                bias2=False,
-                sequence_parallel=gpc.config.parallel.sequence_parallel,
-                checkpoint_lvl=0,
-                heuristic="auto",
-                device=device,
-                dtype=dtype,
-            )
 
         self.dropout2 = nn.Dropout(drop_rate)
         self.use_swiglu = use_swiglu
         self.use_scaled_init = use_scaled_init
         self.residual_in_fp32 = residual_in_fp32  # only make sense when using prenorm
         self.return_residual = False
         self.reset_parameters()
@@ -314,29 +296,17 @@
             self.tp_mode = gpc.config.parallel["tensor"].get("mode", "mtp")
 
         if is_reward:
             head_cls = RewardModelLinear
         else:
             head_cls = ScaleColumnParallelLinear
         if first:
-            if embed_split_hidden or not gpc.config.use_cuda_flash_attn:
-                self.embedding = Embedding1D(num_embeddings=vocab_size, embedding_dim=hidden_size)
-            else:
-                from flash_attn.modules.embedding import ParallelGPT2Embeddings
-
-                self.embedding = ParallelGPT2Embeddings(
-                    embed_dim=hidden_size,
-                    vocab_size=vocab_size,
-                    max_position_embeddings=-1,
-                    process_group=gpc.get_group(ParallelMode.TENSOR),
-                    padding_idx=None,
-                    sequence_parallel=gpc.config.parallel.sequence_parallel,
-                    device=device,
-                    dtype=dtype,
-                )
+            self.embedding = Embedding1D(
+                num_embeddings=vocab_size, embedding_dim=hidden_size, embed_split_hidden=embed_split_hidden
+            )
             for _, param in self.embedding.named_parameters():
                 normal_(std=0.0052)(param)
         self.embed_grad_scale = embed_grad_scale
 
         self.blocks = nn.ModuleList(
             [
                 PackedFlashBaseLayer1D(
@@ -384,15 +354,15 @@
             for _, param in self.head.named_parameters():
                 normal_(std=0.0052)(param)
 
         self.parallel_output = parallel_output
 
     def forward(self, hidden_states=None, cu_seqlens=None, input_ids=None, indexes=None, inference_params=None):
         # attention_mask: compute attention on the places where the value is 1
-        if hasattr(self, "embedding"):
+        if hasattr(self, "embedding") and input_ids is not None:
             hidden_states = self.embedding(input_ids)
             if self.embed_grad_scale != 1:
                 hidden_states = (
                     self.embed_grad_scale * hidden_states + (1 - self.embed_grad_scale) * hidden_states.detach()
                 )
 
         if isinstance(cu_seqlens, list):
@@ -447,31 +417,33 @@
 
     all_parts = partition_uniform(num_layers, pipeline_size, num_chunks)
     parts = all_parts[pipeline_rank]
     if gpc.is_rank_for_log():
         logger.info(f"The layer sharding is {all_parts}.")
 
     models = []
-
+    start_idx, end_idx = 0, 0
     for start, end in parts:
+        start_idx, end_idx = start, end
         kwargs["num_layers"] = end - start
         kwargs["first"] = start == 0
         # If there is no content in the final layer, assign the last layer.
         kwargs["last"] = end == num_layers and len(all_parts[-1]) != 0
         kwargs["device"] = device
         kwargs["start_layer_idx"] = start
         chunk = PackedFlashInternLm1D(**filter_kwargs(PackedFlashInternLm1D.__init__, kwargs)).to(device)
 
         models.append(chunk)
     torch.distributed.barrier()
     if len(models) == 1:
         model = models[0]
     else:
         model = nn.ModuleList(models)
-
+    setattr(model, "first_layer", start_idx)
+    setattr(model, "last_layer", end_idx)
     return model
 
 
 @MODEL_INITIALIZER.register_module(module_name=MODEL_TYPE)
 def build_model_with_cfg(
     num_chunks=1,
     checkpoint=0.0,
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/modeling_internlm2.py` & `InternEvo-0.4.2/internlm/model/modeling_internlm2.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,24 +22,24 @@
     RotaryEmbedding,
 )
 from internlm.model.modules.mlp import get_mlp_cls
 from internlm.model.modules.multi_head_attention import (
     _update_kv_cache,
     get_gqa_attn_cls,
 )
+from internlm.model.ops.fusion_ops_import_helper import try_import_RMSNorm
 from internlm.model.ops.linear import (
     RewardModelLinear,
     ScaleColumnParallelLinearWithNormHead,
     get_linear_cls,
 )
 from internlm.model.utils import (
     gather_forward_split_backward,
     pack_output_after_attn,
     split_forward_gather_backward,
-    try_import_RMSNorm,
     unpack_qkv_before_attn,
 )
 from internlm.solver.activation_checkpoint import activation_checkpoint
 from internlm.solver.pipeline_utils import partition_uniform
 from internlm.utils.common import filter_kwargs, get_current_device
 from internlm.utils.logger import get_logger
 from internlm.utils.registry import MODEL_INITIALIZER
@@ -236,26 +236,24 @@
                         if empties[i] != 0:
                             q[i][empties[i] :] = moved_q[i][: -empties[i]]
                             k[i][empties[i] :] = moved_k[i][: -empties[i]]
                         else:
                             q[i] = moved_q[i]
                             k[i] = moved_k[i]
                 else:
-                    q = q.squeeze(1)
-                    k = k.squeeze(1)
                     q = self.rotary_emb._single_forward(
                         q,
                         inference_params.sequence_len_offset * torch.ones(q.size(0), dtype=torch.int, device=q.device)
                         - empties,
-                    ).unsqueeze(1)
+                    )
                     k = self.rotary_emb._single_forward(
                         k,
                         inference_params.sequence_len_offset * torch.ones(k.size(0), dtype=torch.int, device=k.device)
                         - empties,
-                    ).unsqueeze(1)
+                    )
             else:
                 raise NotImplementedError(
                     "You should make sure you are aware that you are changing the method of generating."
                     "According to your generation function instead of inference/seq_generator_module.py, "
                     "You may implement here for normal running."
                 )
 
@@ -283,15 +281,14 @@
 
             # When using FP16, there is a high probability of NAN in the KV.
             # Since NAN cannot be removed by multiplying with and 0, it needs
             # to be removed manually here.
             kv = torch.where(torch.isnan(kv), 0, kv)
 
             if hasattr(inference_params, "attention_mask") and inference_params.attention_mask is not None:
-                assert gpc.config.use_cuda_flash_attn is True
                 from flash_attn import flash_attn_varlen_kvpacked_func
 
                 if inference_params.sequence_len_offset == 0:  # First entrance, attnmask (bs*seqlen*seqlen)
                     attn_mask = inference_params.attention_mask[:, None, ...]
                     attn_mask = torch.logical_or(
                         torch.ones_like(attn_mask, dtype=torch.bool).triu(diagonal=1), attn_mask
                     )
@@ -585,53 +582,30 @@
         self.dropout1 = nn.Dropout(drop_rate)
         if norm_type == "rmsnorm":
             self.attention_norm = RMSNorm(hidden_size, eps=layer_norm_epsilon)
             self.ffn_norm = RMSNorm(hidden_size, eps=layer_norm_epsilon)
         else:
             self.attention_norm = nn.LayerNorm(hidden_size, eps=layer_norm_epsilon)
             self.ffn_norm = nn.LayerNorm(hidden_size, eps=layer_norm_epsilon)
-        if self.fused_dropout_add_ln and gpc.config.use_cuda_flash_attn:
-            from flash_attn.ops.layer_norm import dropout_add_layer_norm
-
-            assert dropout_add_layer_norm is not None, "dropout_add_ln is not installed"
-            assert isinstance(self.attention_norm, nn.LayerNorm) and isinstance(self.dropout1, nn.Dropout)
 
         sequence_parallel = gpc.config.parallel.get("sequence_parallel", False)
-        if use_swiglu or not gpc.config.model.use_flash_attn:
-            ffn = get_mlp_cls(self.tp_mode)
-            self.feed_forward = ffn(
-                hidden_size,
-                int(hidden_size * mlp_ratio),
-                out_features=hidden_size,
-                process_group=gpc.get_group(parallel_mode),
-                bias=False,
-                device=device,
-                dtype=dtype,
-                mlp_layer_fusion=mlp_layer_fusion,
-                sequence_parallel=sequence_parallel,
-                multiple_of=multiple_of,
-            )
-        else:
-            from flash_attn.modules.mlp import ParallelFusedMLP
-
-            self.feed_forward = ParallelFusedMLP(
-                hidden_size,
-                int(hidden_size * mlp_ratio),
-                out_features=hidden_size,
-                activation="gelu_approx",
-                process_group=gpc.get_group(parallel_mode),
-                bias1=False,
-                bias2=False,
-                sequence_parallel=sequence_parallel,
-                checkpoint_lvl=0,
-                heuristic="auto",
-                device=device,
-                dtype=dtype,
-            )
+        self.feed_forward = get_mlp_cls(self.tp_mode)(
+            hidden_size,
+            int(hidden_size * mlp_ratio),
+            out_features=hidden_size,
+            process_group=gpc.get_group(parallel_mode),
+            bias=False,
+            device=device,
+            dtype=dtype,
+            mlp_layer_fusion=mlp_layer_fusion,
+            sequence_parallel=sequence_parallel,
+            multiple_of=multiple_of,
+        )
 
+        assert use_swiglu is True, "InternLM2 only support swiglu."
         self.dropout2 = nn.Dropout(drop_rate)
         self.use_swiglu = use_swiglu
         self.use_scaled_init = use_scaled_init
         self.residual_in_fp32 = residual_in_fp32  # only make sense when using prenorm
         self.return_residual = False
 
         if init_type == "normal":
@@ -868,32 +842,18 @@
             self.tp_mode = gpc.config.parallel["tensor"].get("mode", "mtp")
 
         if is_reward:
             head_cls = RewardModelLinear
         else:
             head_cls = ScaleColumnParallelLinearWithNormHead
 
-        sequence_parallel = gpc.config.parallel.get("sequence_parallel", False)
-
         if first:
-            if embed_split_hidden or not gpc.config.model.use_flash_attn:
-                self.tok_embeddings = Embedding1D(num_embeddings=vocab_size, embedding_dim=hidden_size)
-            else:
-                from flash_attn.modules.embedding import ParallelGPT2Embeddings
-
-                self.tok_embeddings = ParallelGPT2Embeddings(
-                    embed_dim=hidden_size,
-                    vocab_size=vocab_size,
-                    max_position_embeddings=-1,
-                    process_group=gpc.get_group(ParallelMode.TENSOR),
-                    padding_idx=None,
-                    sequence_parallel=sequence_parallel,
-                    device=device,
-                    dtype=dtype,
-                )
+            self.tok_embeddings = Embedding1D(
+                num_embeddings=vocab_size, embedding_dim=hidden_size, embed_split_hidden=embed_split_hidden
+            )
             for _, param in self.tok_embeddings.named_parameters():
                 if init_type == "normal":
                     normal_(std=embedding_init_std)(param)
                 else:
                     uniform_(std=embedding_init_std)(param)
 
         self.embed_grad_scale = embed_grad_scale
@@ -966,15 +926,15 @@
                 else:
                     uniform_(std=out_head_init_std)(param)
 
         self.parallel_output = parallel_output
 
     def forward(self, hidden_states=None, cu_seqlens=None, input_ids=None, indexes=None, inference_params=None):
         # attention_mask: compute attention on the places where the value is 1
-        if hasattr(self, "tok_embeddings"):
+        if hasattr(self, "tok_embeddings") and input_ids is not None:
             hidden_states = self.tok_embeddings(input_ids)
             if self.embed_grad_scale != 1:
                 hidden_states = (
                     self.embed_grad_scale * hidden_states + (1 - self.embed_grad_scale) * hidden_states.detach()
                 )
         if isinstance(cu_seqlens, list):
             assert len(cu_seqlens) == 1
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/modeling_llama.py` & `InternEvo-0.4.2/internlm/model/modeling_llama.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 )
 from internlm.model.modules.embedding import Embedding1D, RotaryEmbedding
 from internlm.model.modules.mlp import get_mlp_cls
 from internlm.model.modules.multi_head_attention import (
     _update_kv_cache,
     get_gqa_attn_cls,
 )
+from internlm.model.ops.fusion_ops_import_helper import try_import_RMSNorm
 from internlm.model.ops.linear import (
     RewardModelLinear,
     ScaleColumnParallelLinear,
     get_linear_cls,
 )
 from internlm.model.utils import (
     gather_forward_split_backward,
     pack_output_after_attn,
     split_forward_gather_backward,
-    try_import_RMSNorm,
     unpack_qkv_before_attn,
 )
 from internlm.solver.activation_checkpoint import activation_checkpoint
 from internlm.solver.pipeline_utils import partition_uniform
 from internlm.utils.common import filter_kwargs, get_current_device
 from internlm.utils.logger import get_logger
 from internlm.utils.registry import MODEL_INITIALIZER
@@ -230,26 +230,24 @@
                         if empties[i] != 0:
                             q[i][empties[i] :] = moved_q[i][: -empties[i]]
                             k[i][empties[i] :] = moved_k[i][: -empties[i]]
                         else:
                             q[i] = moved_q[i]
                             k[i] = moved_k[i]
                 else:
-                    q = q.squeeze(1)
-                    k = k.squeeze(1)
                     q = self.rotary_emb._single_forward(
                         q,
                         inference_params.sequence_len_offset * torch.ones(q.size(0), dtype=torch.int, device=q.device)
                         - empties,
-                    ).unsqueeze(1)
+                    )
                     k = self.rotary_emb._single_forward(
                         k,
                         inference_params.sequence_len_offset * torch.ones(k.size(0), dtype=torch.int, device=k.device)
                         - empties,
-                    ).unsqueeze(1)
+                    )
             else:
                 raise NotImplementedError(
                     "You should make sure you are aware that you are changing the method of generating."
                     "According to your generation function instead of inference/seq_generator_module.py, "
                     "You may implement here for normal running."
                 )
 
@@ -277,15 +275,14 @@
 
             # When using FP16, there is a high probability of NAN in the KV.
             # Since NAN cannot be removed by multiplying with and 0, it needs
             # to be removed manually here.
             kv = torch.where(torch.isnan(kv), 0, kv)
 
             if hasattr(inference_params, "attention_mask") and inference_params.attention_mask is not None:
-                assert gpc.config.use_cuda_flash_attn is True
                 from flash_attn.flash_attn_interface import FlashAttnVarlenKVPackedFunc
 
                 if inference_params.sequence_len_offset == 0:  # First entrance, attnmask (bs*seqlen*seqlen)
                     attn_mask = inference_params.attention_mask[:, None, ...]
                     attn_mask = torch.logical_or(
                         torch.ones_like(attn_mask, dtype=torch.bool).triu(diagonal=1), attn_mask
                     )
@@ -572,52 +569,27 @@
         self.dropout1 = nn.Dropout(drop_rate)
         if norm_type == "rmsnorm":
             self.attention_norm = RMSNorm(hidden_size, eps=layer_norm_epsilon)
             self.ffn_norm = RMSNorm(hidden_size, eps=layer_norm_epsilon)
         else:
             self.attention_norm = nn.LayerNorm(hidden_size, eps=layer_norm_epsilon)
             self.ffn_norm = nn.LayerNorm(hidden_size, eps=layer_norm_epsilon)
-        if self.fused_dropout_add_ln and gpc.config.use_cuda_flash_attn:
-            from flash_attn.ops.layer_norm import dropout_add_layer_norm
-
-            assert dropout_add_layer_norm is not None, "dropout_add_ln is not installed"
-            assert isinstance(self.attention_norm, nn.LayerNorm) and isinstance(self.dropout1, nn.Dropout)
-
-        sequence_parallel = gpc.config.parallel.get("sequence_parallel", False)
-        if use_swiglu or not gpc.config.use_cuda_flash_attn:
-            mlp_cls = get_mlp_cls(self.tp_mode)
-            self.feed_forward = mlp_cls(
-                hidden_size,
-                int(hidden_size * mlp_ratio),
-                out_features=hidden_size,
-                process_group=gpc.get_group(parallel_mode),
-                bias=False,
-                device=device,
-                dtype=dtype,
-                mlp_layer_fusion=mlp_layer_fusion,
-                sequence_parallel=gpc.config.parallel.sequence_parallel,
-                multiple_of=multiple_of,
-            )
-        else:
-            from flash_attn.modules.mlp import ParallelFusedMLP
 
-            self.feed_forward = ParallelFusedMLP(
-                hidden_size,
-                int(hidden_size * mlp_ratio),
-                out_features=hidden_size,
-                activation="gelu_approx",
-                process_group=gpc.get_group(parallel_mode),
-                bias1=False,
-                bias2=False,
-                sequence_parallel=sequence_parallel,
-                checkpoint_lvl=0,
-                heuristic="auto",
-                device=device,
-                dtype=dtype,
-            )
+        self.feed_forward = get_mlp_cls(self.tp_mode)(
+            hidden_size,
+            int(hidden_size * mlp_ratio),
+            out_features=hidden_size,
+            process_group=gpc.get_group(parallel_mode),
+            bias=False,
+            device=device,
+            dtype=dtype,
+            mlp_layer_fusion=mlp_layer_fusion,
+            sequence_parallel=gpc.config.parallel.get("sequence_parallel", False),
+            multiple_of=multiple_of,
+        )
 
         self.dropout2 = nn.Dropout(drop_rate)
         self.use_swiglu = use_swiglu
         self.use_scaled_init = use_scaled_init
         self.residual_in_fp32 = residual_in_fp32  # only make sense when using prenorm
         self.return_residual = False
 
@@ -835,40 +807,27 @@
 
         self.use_flash_attn = use_flash_attn
         if checkpoint_fraction <= 0:
             checkpoint = False
         if not checkpoint:
             checkpoint_fraction = 0
         checkpoint_layer_num = num_layers * checkpoint_fraction
-        sequence_parallel = gpc.config.parallel.get("sequence_parallel", False)
         self.tp_mode = "mtp"
         if isinstance(gpc.config.parallel["tensor"], dict):
             self.tp_mode = gpc.config.parallel["tensor"].get("mode", "mtp")
 
         if is_reward:
             head_cls = RewardModelLinear
         else:
             head_cls = ScaleColumnParallelLinear
 
         if first:
-            if embed_split_hidden or not gpc.config.use_cuda_flash_attn:
-                self.tok_embeddings = Embedding1D(num_embeddings=vocab_size, embedding_dim=hidden_size)
-            else:
-                from flash_attn.modules.embedding import ParallelGPT2Embeddings
-
-                self.tok_embeddings = ParallelGPT2Embeddings(
-                    embed_dim=hidden_size,
-                    vocab_size=vocab_size,
-                    max_position_embeddings=-1,
-                    process_group=gpc.get_group(ParallelMode.TENSOR),
-                    padding_idx=None,
-                    sequence_parallel=sequence_parallel,
-                    device=device,
-                    dtype=dtype,
-                )
+            self.tok_embeddings = Embedding1D(
+                num_embeddings=vocab_size, embedding_dim=hidden_size, embed_split_hidden=embed_split_hidden
+            )
             for _, param in self.tok_embeddings.named_parameters():
                 if init_type == "normal":
                     normal_(std=embedding_init_std)(param)
                 else:
                     uniform_(std=embedding_init_std)(param)
         self.embed_grad_scale = embed_grad_scale
 
@@ -933,15 +892,15 @@
                 else:
                     uniform_(std=out_head_init_std)(param)
 
         self.parallel_output = parallel_output
 
     def forward(self, hidden_states=None, cu_seqlens=None, input_ids=None, indexes=None, inference_params=None):
         # attention_mask: compute attention on the places where the value is 1
-        if hasattr(self, "tok_embeddings"):
+        if hasattr(self, "tok_embeddings") and input_ids is not None:
             hidden_states = self.tok_embeddings(input_ids)
             if self.embed_grad_scale != 1:
                 hidden_states = (
                     self.embed_grad_scale * hidden_states + (1 - self.embed_grad_scale) * hidden_states.detach()
                 )
         if isinstance(cu_seqlens, list):
             assert len(cu_seqlens) == 1
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/modeling_moe.py` & `InternEvo-0.4.2/internlm/model/modeling_moe.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 from internlm.core.context.parallel_context import global_context as gpc
 from internlm.core.naive_amp import set_fp32_attr_to_module
 from internlm.initialize.initialize_tensor import normal_, scaled_init_method_normal
 from internlm.model.modules.embedding import Embedding1D
 from internlm.model.modules.mlp import get_mlp_cls
 from internlm.model.modules.multi_head_attention import MHA
 from internlm.model.moe import MoE
+from internlm.model.ops.fusion_ops_import_helper import try_import_RMSNorm
 from internlm.model.ops.linear import RewardModelLinear, ScaleColumnParallelLinear
 from internlm.model.utils import (
     gather_forward_split_backward,
     split_forward_gather_backward,
-    try_import_RMSNorm,
 )
 from internlm.solver.activation_checkpoint import activation_checkpoint
 from internlm.solver.pipeline_utils import partition_uniform
 from internlm.utils.common import filter_kwargs, get_current_device
 from internlm.utils.logger import get_logger
 from internlm.utils.registry import MODEL_INITIALIZER
 
@@ -118,45 +118,28 @@
         else:
             self.norm1 = nn.LayerNorm(hidden_size, eps=layer_norm_epsilon)
             self.norm2 = nn.LayerNorm(hidden_size, eps=layer_norm_epsilon)
 
         self.num_experts = num_experts
         ep_size = gpc.get_world_size(ParallelMode.EXPERT)
         if num_experts <= 1:  # dense, not MoE
-            if use_swiglu or not gpc.config.use_cuda_flash_attn:
+            if use_swiglu:
                 mlp_cls = get_mlp_cls(self.tp_mode)
                 self.mlp = mlp_cls(
                     hidden_size,
                     int(hidden_size * mlp_ratio),
                     out_features=hidden_size,
                     process_group=gpc.get_group(parallel_mode),
                     bias=False,
                     device=device,
                     dtype=dtype,
                     mlp_layer_fusion=mlp_layer_fusion,
                     sequence_parallel=gpc.config.parallel.sequence_parallel,
                     multiple_of=multiple_of,
                 )
-            else:
-                from flash_attn.modules.mlp import ParallelFusedMLP
-
-                self.mlp = ParallelFusedMLP(
-                    hidden_size,
-                    int(hidden_size * mlp_ratio),
-                    out_features=hidden_size,
-                    activation="gelu_approx",
-                    process_group=gpc.get_group(parallel_mode),
-                    bias1=False,
-                    bias2=False,
-                    sequence_parallel=gpc.config.parallel.sequence_parallel,
-                    checkpoint_lvl=0,
-                    heuristic="auto",
-                    device=device,
-                    dtype=dtype,
-                )
         else:
             # replace mlp by MoE module. The expert in MoE is a FeedForward module.
             mlp_cls = get_mlp_cls(self.tp_mode)
             self.mlp = MoE(
                 hidden_size,
                 int(hidden_size * mlp_ratio),
                 out_features=hidden_size,
@@ -341,29 +324,17 @@
 
         if is_reward:
             head_cls = RewardModelLinear
         else:
             head_cls = ScaleColumnParallelLinear
 
         if first:
-            if embed_split_hidden or not gpc.config.use_cuda_flash_attn:
-                self.embedding = Embedding1D(num_embeddings=vocab_size, embedding_dim=hidden_size)
-            else:
-                from flash_attn.modules.embedding import ParallelGPT2Embeddings
-
-                self.embedding = ParallelGPT2Embeddings(
-                    embed_dim=hidden_size,
-                    vocab_size=vocab_size,
-                    max_position_embeddings=-1,
-                    process_group=gpc.get_group(ParallelMode.TENSOR),
-                    padding_idx=None,
-                    sequence_parallel=gpc.config.parallel.sequence_parallel,
-                    device=device,
-                    dtype=dtype,
-                )
+            self.embedding = Embedding1D(
+                num_embeddings=vocab_size, embedding_dim=hidden_size, embed_split_hidden=embed_split_hidden
+            )
             for _, param in self.embedding.named_parameters():
                 normal_(std=0.0052)(param)
         self.embed_grad_scale = embed_grad_scale
         self.blocks = nn.ModuleList(
             [
                 PackedFlashBaseLayer1D(
                     hidden_size=hidden_size,
@@ -410,15 +381,15 @@
                 normal_(std=0.0052)(param)
 
         self.parallel_output = parallel_output
 
     def forward(self, hidden_states=None, cu_seqlens=None, input_ids=None, indexes=None, inference_params=None):
         # attention_mask: compute attention on the places where the value is 1
         # old condition may fail when use shared embedding
-        if gpc.is_pipeline_first_stage():
+        if gpc.is_pipeline_first_stage() and input_ids is not None:
             hidden_states = self.embedding(input_ids)
             if self.embed_grad_scale != 1:
                 hidden_states = (
                     self.embed_grad_scale * hidden_states + (1 - self.embed_grad_scale) * hidden_states.detach()
                 )
         if isinstance(cu_seqlens, list):
             assert len(cu_seqlens) == 1
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/modules/embedding.py` & `InternEvo-0.4.2/internlm/model/modules/embedding.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,67 +4,73 @@
 from typing import Tuple
 
 import torch
 import torch.nn.functional as F
 from einops import rearrange
 from torch import Tensor, nn
 
-from internlm.accelerator import AcceleratorType, get_accelerator
+from internlm.accelerator import get_accelerator
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
+from internlm.model.ops.fusion_ops_import_helper import try_import_fused_rotary
 
 from ..utils import gather_forward_split_backward, split_forward_gather_backward
 
-try:
-    import rotary_emb
-except (ModuleNotFoundError, ImportError):
-    pass
-
 internlm_accelerator = get_accelerator()
 
+apply_rotary_emb, apply_rotary_emb_qkv_, apply_rotary_func = None, None, None
+
 
 class Embedding1D(nn.Module):
     """
     1D Embedding.
 
     Args:
         num_embeddings (int): The size of vocab.
         embedding_dim (int): The dimention of model.
         padding_idx (int): If specified, the entries at :attr:`padding_idx` do not contribute to the gradient;
                             therefore, the embedding vector at :attr:`padding_idx` is not updated during training,
                             i.e. it remains as a fixed "pad". None by default.
         dtype (Optional[torch.dtype]): Data type None by default.
+        embed_split_hidden (Optional[Bool]): Whether to split the embed_dim in tensor parallel style.
 
     """
 
     def __init__(
         self,
         num_embeddings: int,
         embedding_dim: int,
         *args,
         padding_idx: int = None,
         dtype: torch.dtype = None,
+        embed_split_hidden: bool = True,
         **kwargs,
     ):
         super().__init__()
 
         self.num_embeddings = num_embeddings
         self.embed_dim = embedding_dim
-        embed_dim_per_partition = embedding_dim // gpc.tensor_parallel_size
+        self.embed_split_hidden = embed_split_hidden
+        if self.embed_split_hidden:
+            self.embed_split_hidden = gpc.tensor_parallel_size > 1
+
+        split_nums = 1 if not self.embed_split_hidden else gpc.tensor_parallel_size
+        embed_dim_per_partition = embedding_dim // split_nums
 
         self.padding_idx = padding_idx
         self.embed_args = args
         self.embed_kwargs = kwargs
 
         self.weight = nn.Parameter(torch.empty((num_embeddings, embed_dim_per_partition), dtype=dtype))
 
     def forward(self, input_: Tensor) -> Tensor:
-        output_parallel = F.embedding(input_, self.weight, self.padding_idx, *self.embed_args, **self.embed_kwargs)
+        output = F.embedding(input_, self.weight, self.padding_idx, *self.embed_args, **self.embed_kwargs)
 
-        output = gather_forward_split_backward(output_parallel, ParallelMode.TENSOR, dim=-1)
+        if self.embed_split_hidden:
+            output = gather_forward_split_backward(output, ParallelMode.TENSOR, dim=-1)
 
         if gpc.config.parallel.sequence_parallel:
             output = split_forward_gather_backward(output, ParallelMode.TENSOR, dim=1)
 
         return output
 
 
@@ -90,21 +96,14 @@
     else:
         out1.copy_(x1 * cos - x2 * sin)
         out2.copy_(x1 * sin + x2 * cos)
 
     return out1, out2
 
 
-def get_rotary_func():
-    if gpc.config.use_cuda_flash_attn:
-        return rotary_emb.apply_rotary
-    else:
-        return _torch_apply_rotary_func
-
-
 class ApplyRotaryEmb(torch.autograd.Function):
     """
     ApplyRotaryEmb
     """
 
     @staticmethod
     def forward(ctx, x, cos, sin, interleaved=False):
@@ -124,15 +123,15 @@
         assert sin.shape == (rotary_seqlen, rotary_dim // 2)
         x_ro = x[..., :rotary_dim]
         x1, x2 = x_ro.chunk(2, dim=-1) if not interleaved else (x_ro[..., ::2], x_ro[..., 1::2])
         out = torch.empty_like(x)
         out_ro = out[..., :rotary_dim]
         o1, o2 = out_ro.chunk(2, dim=-1) if not interleaved else (out_ro[..., ::2], out_ro[..., 1::2])
 
-        get_rotary_func()(
+        apply_rotary_func(
             x1,
             x2,
             rearrange(cos[:seqlen], "s d -> s 1 d"),
             rearrange(sin[:seqlen], "s d -> s 1 d"),
             o1,
             o2,
             False,
@@ -152,36 +151,28 @@
         rotary_dim *= 2
         do_ro = do[..., :rotary_dim]
         do1, do2 = do_ro.chunk(2, dim=-1) if not ctx.interleaved else (do_ro[..., ::2], do_ro[..., 1::2])
         dx = torch.empty_like(do)
         dx_ro = dx[..., :rotary_dim]
         dx1, dx2 = dx_ro.chunk(2, dim=-1) if not ctx.interleaved else (dx_ro[..., ::2], dx_ro[..., 1::2])
 
-        get_rotary_func()(
+        apply_rotary_func(
             do1,
             do2,
             rearrange(cos[:seqlen], "s d -> s 1 d"),
             rearrange(sin[:seqlen], "s d -> s 1 d"),
             dx1,
             dx2,
             True,
         )
         if rotary_dim < headdim:
             dx[..., rotary_dim:].copy_(do[..., rotary_dim:])
         return dx, None, None, None, None
 
 
-if AcceleratorType.DIPU == internlm_accelerator.get_accelerator_backend():
-    from deeplink_ext.internlm_ops.rotary.deeplink import DeeplinkApplyRotaryEmb
-
-    apply_rotary_emb = DeeplinkApplyRotaryEmb.apply
-else:
-    apply_rotary_emb = ApplyRotaryEmb.apply
-
-
 class ApplyRotaryEmbQKV_(torch.autograd.Function):
     """
     ApplyRotaryEmbQKV_
     """
 
     @staticmethod
     def forward(ctx, qkv, cos, sin, cos_k=None, sin_k=None, interleaved=False):
@@ -210,26 +201,26 @@
         sin_k = sin if sin_k is None else sin_k
         assert sin.shape == cos_k.shape == sin_k.shape == (rotary_seqlen, rotary_dim // 2)
         q_ro = qkv[:, 0, :, :rotary_dim] if len(qkv.shape) == 4 else qkv[:, :, 0, :, :rotary_dim]
         q1, q2 = q_ro.chunk(2, dim=-1) if not interleaved else (q_ro[..., ::2], q_ro[..., 1::2])
         re_cos = rearrange(cos, "s d -> s 1 d") if len(qkv.shape) == 4 else rearrange(cos[:seqlen], "s d -> s 1 d")
         re_sin = rearrange(sin, "s d -> s 1 d") if len(qkv.shape) == 4 else rearrange(sin[:seqlen], "s d -> s 1 d")
 
-        get_rotary_func()(q1, q2, re_cos, re_sin, q1, q2, False)
+        apply_rotary_func(q1, q2, re_cos, re_sin, q1, q2, False)
 
         k_ro = qkv[:, 1, :, :rotary_dim] if len(qkv.shape) == 4 else qkv[:, :, 1, :, :rotary_dim]
         k1, k2 = k_ro.chunk(2, dim=-1) if not interleaved else (k_ro[..., ::2], k_ro[..., 1::2])
         re_cos_k = (
             rearrange(cos_k, "s d -> s 1 d") if len(qkv.shape) == 4 else rearrange(cos_k[:seqlen], "s d -> s 1 d")
         )
         re_sin_k = (
             rearrange(sin_k, "s d -> s 1 d") if len(qkv.shape) == 4 else rearrange(sin_k[:seqlen], "s d -> s 1 d")
         )
 
-        get_rotary_func()(k1, k2, re_cos_k, re_sin_k, k1, k2, False)
+        apply_rotary_func(k1, k2, re_cos_k, re_sin_k, k1, k2, False)
 
         ctx.save_for_backward(cos, sin, cos_k, sin_k)
         ctx.interleaved = interleaved
         return qkv
 
     @staticmethod
     def backward(ctx, dqkv):
@@ -238,36 +229,37 @@
         rotary_dim = cos.shape[-1]
         rotary_dim *= 2
         dq_ro = dqkv[:, 0, :, :rotary_dim] if len(dqkv.shape) == 4 else dqkv[:, :, 0, :, :rotary_dim]
         dq1, dq2 = dq_ro.chunk(2, dim=-1) if not ctx.interleaved else (dq_ro[..., ::2], dq_ro[..., 1::2])
         re_cos = rearrange(cos, "s d -> s 1 d") if len(dqkv.shape) == 4 else rearrange(cos[:seqlen], "s d -> s 1 d")
         re_sin = rearrange(sin, "s d -> s 1 d") if len(dqkv.shape) == 4 else rearrange(sin[:seqlen], "s d -> s 1 d")
 
-        get_rotary_func()(dq1, dq2, re_cos, re_sin, dq1, dq2, True)
+        apply_rotary_func(dq1, dq2, re_cos, re_sin, dq1, dq2, True)
 
         dk_ro = dqkv[:, 1, :, :rotary_dim] if len(dqkv.shape) == 4 else dqkv[:, :, 1, :, :rotary_dim]
         dk1, dk2 = dk_ro.chunk(2, dim=-1) if not ctx.interleaved else (dk_ro[..., ::2], dk_ro[..., 1::2])
         re_cos_k = (
             rearrange(cos_k, "s d -> s 1 d") if len(dqkv.shape) == 4 else rearrange(cos_k[:seqlen], "s d -> s 1 d")
         )
         re_sin_k = (
             rearrange(sin_k, "s d -> s 1 d") if len(dqkv.shape) == 4 else rearrange(sin_k[:seqlen], "s d -> s 1 d")
         )
 
-        get_rotary_func()(dk1, dk2, re_cos_k, re_sin_k, dk1, dk2, True)
+        apply_rotary_func(dk1, dk2, re_cos_k, re_sin_k, dk1, dk2, True)
 
         return dqkv, None, None, None, None, None
 
 
-if AcceleratorType.DIPU == internlm_accelerator.get_accelerator_backend():
-    from deeplink_ext.internlm_ops.rotary.deeplink import DeeplinkApplyRotaryEmbQKV_
-
-    apply_rotary_emb_qkv_ = DeeplinkApplyRotaryEmbQKV_.apply
-else:
+apply_rotary_emb, apply_rotary_emb_qkv_, apply_rotary_func = try_import_fused_rotary()
+if apply_rotary_emb is None:
+    apply_rotary_emb = ApplyRotaryEmb.apply
+if apply_rotary_emb_qkv_ is None:
     apply_rotary_emb_qkv_ = ApplyRotaryEmbQKV_.apply
+if apply_rotary_func is None:
+    apply_rotary_func = _torch_apply_rotary_func
 
 
 class RotaryEmbedding(torch.nn.Module):
     """
     The rotary position embeddings from RoFormer_ (Su et. al).
     A crucial insight from the method is that the query and keys are
     transformed by rotation matrices which depend on the relative positions.
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/modules/mlp.py` & `InternEvo-0.4.2/internlm/model/modules/mlp.py`

 * *Files 13% similar despite different names*

```diff
@@ -95,27 +95,33 @@
         return w1, w3
 
     @staticmethod
     def split_fused_mlp_output(w1_w3_out):
         w1_o, w3_o = torch.split(w1_w3_out, w1_w3_out.shape[-1] // 2, dim=-1)
         return w1_o, w3_o
 
-    def _mlp_pre_load_convert(self, state_dict, *args, **kwargs) -> None:  # pylint: disable=W0613
-        if self.mlp_layer_fusion and "fused_w1_w3.weight" not in state_dict:
-            w1, w3 = state_dict.pop("w1.weight"), state_dict.pop("w3.weight")
-            state_dict["fused_w1_w3.weight"] = torch.cat([w1, w3], dim=0)
-        if not self.mlp_layer_fusion and ("w1.weight" not in state_dict or "w3.weight" not in state_dict):
-            state_dict["w1.weight"], state_dict["w3.weight"] = self.split_fused_mlp_weight(
-                state_dict.pop("fused_w1_w3.weight")
-            )
+    def _mlp_pre_load_convert(self, state_dict, prefix, *args, **kwargs) -> None:  # pylint: disable=W0613
+        w1_name = f"{prefix}w1.weight"
+        w3_name = f"{prefix}w3.weight"
+        fused_w1_w3_name = f"{prefix}fused_w1_w3.weight"
+
+        if self.mlp_layer_fusion and fused_w1_w3_name not in state_dict:
+            w1, w3 = state_dict.pop(w1_name), state_dict.pop(w3_name)
+            state_dict[fused_w1_w3_name] = torch.cat([w1, w3], dim=0)
+        if not self.mlp_layer_fusion and (w1_name not in state_dict or w3_name not in state_dict):
+            state_dict[w1_name], state_dict[w3_name] = self.split_fused_mlp_weight(state_dict.pop(fused_w1_w3_name))
+
+    def _mlp_save_convert(self, state_dict, prefix, *args, **kwargs) -> Dict:  # pylint: disable=W0613
+        w1_name = f"{prefix}w1.weight"
+        w3_name = f"{prefix}w3.weight"
+        fused_w1_w3_name = f"{prefix}fused_w1_w3.weight"
 
-    def _mlp_save_convert(self, state_dict, *args, **kwargs) -> Dict:  # pylint: disable=W0613
         if self.mlp_layer_fusion:
-            state_dict["w1.weight"], state_dict["w3.weight"] = self.split_fused_mlp_weight(
-                w1_w3=state_dict.pop("fused_w1_w3.weight")
+            state_dict[w1_name], state_dict[w3_name] = self.split_fused_mlp_weight(
+                w1_w3=state_dict.pop(fused_w1_w3_name)
             )
 
         return state_dict
 
 
 class FeedForward(BaseFeedForward):
     """
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/modules/multi_head_attention.py` & `InternEvo-0.4.2/internlm/model/modules/multi_head_attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,20 +42,20 @@
             from internlm.model.modules.multi_head_attention import (
                 AscendFlashSelfAttention,
             )
 
             inner_attn_cls, inner_cross_attn_cls = AscendFlashSelfAttention, AscendFlashSelfAttention
             inner_attn = inner_attn_cls(causal=causal, softmax_scale=softmax_scale, attention_dropout=dropout)
         elif device_backend == AcceleratorType.DIPU:
-            from deeplink_ext.internlm_ops.mha import (
-                DeepLinkCrossAttention,
-                DeepLinkSelfAttention,
+            from deeplink_ext.internevo_ops import (
+                FlashCrossAttention,
+                FlashSelfAttention,
             )
 
-            inner_attn_cls, inner_cross_attn_cls = DeepLinkSelfAttention, DeepLinkCrossAttention
+            inner_attn_cls, inner_cross_attn_cls = FlashSelfAttention, FlashCrossAttention
             inner_attn = inner_attn_cls(causal=causal, softmax_scale=softmax_scale, attention_dropout=dropout)
         else:
             raise NotImplementedError(f"Unsupport device type: {device_backend} for flash attention")
     else:
         inner_attn_cls, inner_cross_attn_cls = SelfAttention, CrossAttention
         inner_attn = inner_attn_cls(causal=causal, softmax_scale=softmax_scale, attention_dropout=dropout)
 
@@ -561,21 +561,19 @@
                 from flash_attn.modules.mha import (
                     FlashCrossAttention,
                     FlashSelfAttention,
                 )
             elif internlm_accelerator.get_accelerator_backend() == AcceleratorType.NPU:
                 FlashCrossAttention, FlashSelfAttention = AscendFlashSelfAttention, AscendFlashSelfAttention
             elif internlm_accelerator.get_accelerator_backend() == AcceleratorType.DIPU:
-                from deeplink_ext.internlm_ops.mha import (
-                    DeepLinkCrossAttention,
-                    DeepLinkSelfAttention,
+                from deeplink_ext.internevo_ops import (
+                    FlashCrossAttention,
+                    FlashSelfAttention,
                 )
 
-                FlashCrossAttention, FlashSelfAttention = DeepLinkCrossAttention, DeepLinkSelfAttention
-
             inner_attn_cls = FlashSelfAttention
             inner_cross_attn_cls = FlashCrossAttention
         else:
             inner_attn_cls = SelfAttention
             inner_cross_attn_cls = CrossAttention
 
         self.inner_attn = inner_attn_cls(causal=causal, softmax_scale=softmax_scale, attention_dropout=dropout)
@@ -683,36 +681,33 @@
                                 k[i] = moved_k[i]
                     elif not self.use_dynamic_ntk_rope:
                         if inference_params.sequence_len_offset > self.max_position_embeddings:
                             warnings.warn(
                                 "Notice your prompt's length is longer than model's max_position_embeddings: "
                                 f"{self.max_position_embeddings}, may cause deviations in dynamic ntk calculations."
                             )
-                        q = q.squeeze(1)
-                        k = k.squeeze(1)
                         q = self.rotary_emb._single_forward(
                             q,
                             inference_params.sequence_len_offset
                             * torch.ones(q.size(0), dtype=torch.int, device=q.device)
                             - empties,
-                        ).unsqueeze(1)
+                        )
                         k = self.rotary_emb._single_forward(
                             k,
                             inference_params.sequence_len_offset
                             * torch.ones(k.size(0), dtype=torch.int, device=k.device)
                             - empties,
-                        ).unsqueeze(1)
+                        )
                     else:
-                        q = q.squeeze(1)
                         q = self.rotary_emb._single_forward(
                             q,
                             inference_params.sequence_len_offset
                             * torch.ones(q.size(0), dtype=torch.int, device=q.device)
                             - empties,
-                        ).unsqueeze(1)
+                        )
                         moved_k = k.clone()
                         for i in range(len(empties)):
                             if empties[i] != 0:
                                 moved_k[i][: -empties[i]] = k[i][empties[i] :]
                         moved_k = self.rotary_emb._single_eval_forward(moved_k, seqlen_offset=0)
                         for i in range(len(empties)):
                             if empties[i] != 0:
@@ -751,31 +746,30 @@
                     if gpc.config.model.dtype is torch.float32 and gpc.config.model.use_flash_attn:
                         with internlm_accelerator.amp.autocast(dtype=torch.bfloat16):
                             if total_q.dtype not in [torch.float16, torch.bfloat16]:
                                 total_q = total_q.to(torch.bfloat16)
                             if total_kv.dtype not in [torch.float16, torch.bfloat16]:
                                 total_kv = total_kv.to(torch.bfloat16)
 
-                    if gpc.config.use_cuda_flash_attn:
+                    try:
+                        from flash_attn.flash_attn_interface import (
+                            flash_attn_unpadded_func,
+                        )
+                    except ImportError:
                         try:
                             from flash_attn.flash_attn_interface import (
-                                flash_attn_unpadded_func,
+                                flash_attn_unpadded_kvpacked_func as flash_attn_unpadded_func,
                             )
                         except ImportError:
                             try:
                                 from flash_attn.flash_attn_interface import (
-                                    flash_attn_unpadded_kvpacked_func as flash_attn_unpadded_func,
+                                    flash_attn_varlen_kvpacked_func as flash_attn_unpadded_func,
                                 )
                             except ImportError:
-                                try:
-                                    from flash_attn.flash_attn_interface import (
-                                        flash_attn_varlen_kvpacked_func as flash_attn_unpadded_func,
-                                    )
-                                except ImportError:
-                                    raise ImportError("Please check your flash_attn version >= 1.0.5.")
+                                raise ImportError("Please check your flash_attn version >= 1.0.5.")
 
                         output = flash_attn_unpadded_func(
                             total_q,
                             total_kv,
                             cu_seqlens,
                             cu_seqlens,
                             max_seqlen_q,
@@ -834,21 +828,22 @@
         qkv = self.Wqkv(x)  # bsz x total x hsz
         qkv = rearrange(
             qkv, "b t (three h d) -> b t three h d", three=3, d=self.head_dim
         )  # bsz x total x 3 x n_head x d
         qkv = self.rotary_emb(qkv, **kwargs)
 
         kwargs.pop("indexes")
+        cu_seqlens = kwargs["cu_seqlens"]
 
         # for packed data, batch dimension with a size of 1 should be directly squeezed off.
         if internlm_accelerator.get_accelerator_backend() == AcceleratorType.GPU:
             qkv = qkv.squeeze(0)
         # since torch_npu only supports fa with no packed data currently, qkv should be unpacked
         elif internlm_accelerator.get_accelerator_backend() in [AcceleratorType.NPU, AcceleratorType.DIPU]:
-            qkv = unpack_qkv_before_attn(qkv, kwargs["cu_seqlens"])
+            qkv = unpack_qkv_before_attn(qkv, cu_seqlens)
             kwargs.pop("cu_seqlens")
             kwargs.pop("max_seqlen")
 
         if inference_params is None:
             if gpc.config.model.dtype is torch.float32 and gpc.config.model.use_flash_attn:
                 with internlm_accelerator.amp.autocast(dtype=torch.bfloat16):
                     if qkv.dtype not in [torch.float16, torch.bfloat16]:
@@ -861,12 +856,12 @@
             raise RuntimeError("Not support this right now")
 
         if internlm_accelerator.get_accelerator_backend() == AcceleratorType.GPU:
             context = rearrange(context, "s h d -> s (h d)")  # recover the shape
             context = context.unsqueeze(0)  # restore bsz dimension
         elif internlm_accelerator.get_accelerator_backend() in [AcceleratorType.NPU, AcceleratorType.DIPU]:
             context = rearrange(context, "b s h d -> b s (h d)")  # recover the shape
-            context = pack_output_after_attn(context, kwargs["cu_seqlens"])
+            context = pack_output_after_attn(context, cu_seqlens)
 
         out = self.out_proj(context)
 
         return out
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/moe/__init__.py` & `InternEvo-0.4.2/internlm/model/moe/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/moe/base_layer.py` & `InternEvo-0.4.2/internlm/model/moe/base_layer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/moe/experts.py` & `InternEvo-0.4.2/internlm/model/moe/experts.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/moe/gshard_layer.py` & `InternEvo-0.4.2/internlm/model/moe/gshard_layer.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,41 +71,50 @@
 
 # einsum dimensions: (g)roup, (s)equence, (e)xpert, (m)odel, (c)apacity
 # See https://arxiv.org/pdf/2006.16668.pdf for details.
 def einsum(rule, a, b):
     if USE_EINSUM:
         return torch.einsum(rule, a, b)
     elif rule == "s,se->se":
-        # [1, s] * [s, e]
+        # [s, 1] * [s, e]
         return a.reshape(a.shape[0], -1) * b
+    elif rule == "ks,kse->kse":
+        # [k, s, 1] * [s, e]
+        return a.reshape(a.shape[0], a.shape[1], -1) * b
     elif rule == "se,sc->sec":
         # [s,e,1] * [s,1,c]
         return a.unsqueeze(2) * b.unsqueeze(1)
+    elif rule == "kse,ksc->ksec":
+        # [k,s,e,1] * [k,s,1,c]
+        return a.unsqueeze(3) * b.unsqueeze(2)
     elif rule == "se,se->s":
-        # [s,1,e] * [s,e,1]
+        # [s,1,e] @ [s,e,1]
         return torch.bmm(a.unsqueeze(1), b.unsqueeze(2)).reshape(-1)
+    elif rule == "se,kse->ks":
+        # [s,1,e] @ [k,s,e,1]
+        return torch.matmul(a.unsqueeze(1), b.unsqueeze(3)).reshape(b.shape[0], -1)
     elif rule == "sec,sm->ecm":
-        # [e*c, s] * [s, m]
+        # [e, c, s] @ [s, m]
         s = a.shape[0]
         e = a.shape[1]
         c = a.shape[2]
         m = b.shape[1]
         return torch.matmul(a.reshape(s, -1).t(), b).reshape(e, c, m)
     elif rule == "sec,ecm->sm":
-        # [s, e*c] * [e*c, m]
+        # [s, e*c] @ [e*c, m]
         return torch.matmul(a.reshape(a.shape[0], -1), b.reshape(-1, b.shape[-1]))
     elif rule == "ks,ksm->sm":
         k = b.shape[0]
         s = b.shape[1]
         m = b.shape[2]
         # [k, s] -> [s, k] -> [s, 1, k]
         a = a.t().unsqueeze(1)
         # [k,s,m] -> [k, sm] -> [sm, k] -> [s, m, k]
         b = b.reshape(k, -1).t().reshape(s, m, k)
-        # bmm([s, 1, k], [s, m, k]^t) -> [s, m, 1]
+        # [s, 1, k] @ [s, k, m]
         return torch.bmm(a, b.transpose(1, 2)).squeeze(2)
     else:
         return torch.einsum(rule, a, b)
 
 
 # The following functions are extracted and scripted
 # because otherwise during a torch.jit.trace, the non-Tensor
@@ -279,14 +288,71 @@
     combine2_sec = einsum("se,sc->sec", gates2, locations2_sc)
     combine_weights = combine1_sec + combine2_sec
     dispatch_mask = combine_weights.bool()
 
     return l_aux, combine_weights, dispatch_mask, exp_counts
 
 
+def fused_topkgating(
+    logits: Tensor,
+    k: int,
+    capacity_factor: float,
+    min_capacity: int,
+) -> Tuple[Tensor, Tensor, Tensor, Tensor]:
+    """Implements TopKGating on logits."""
+    # everything is in fp32 in this function
+    gates = F.softmax(logits, dim=1)
+    num_experts = int(gates.shape[1])
+
+    capacity = _capacity(gates, torch.tensor(capacity_factor * k), torch.tensor(min_capacity))
+
+    # Create a mask by top-k experts
+    indices_s = torch.topk(gates, k, dim=1).indices
+    indices_s = indices_s.permute(1, 0).reshape(-1)
+    masks = F.one_hot(indices_s, num_classes=num_experts)
+
+    # Compute locations in capacity buffer
+    locations = torch.cumsum(masks, dim=0) - 1
+
+    # reshape (s,e) to (k,s,e)
+    masks = masks.reshape(-1, gates.shape[0], num_experts)
+    locations = locations.reshape(-1, gates.shape[0], num_experts)
+
+    # gating decisions
+    exp_counts = torch.sum(masks[0], dim=0).detach().to("cpu")
+
+    # Compute l_aux
+    me = torch.mean(gates, dim=0)
+    ce = torch.mean(masks[0].type_as(logits), dim=0)
+    l_aux = torch.mean(me * ce) * num_experts * num_experts
+
+    # Remove locations outside capacity from mask
+    masks *= torch.lt(locations, capacity)
+
+    # Store the capacity location for each token
+    locations_s = torch.sum(locations * masks, dim=2)
+
+    # Normalize gate probabilities
+    mask_float = masks.type_as(logits)
+    gate_s = einsum("se,kse->ks", gates, mask_float)
+    denom_s = torch.sum(gate_s, dim=0)
+    # Avoid divide-by-zero
+    denom_s = torch.clamp(denom_s, min=torch.finfo(denom_s.dtype).eps)
+    gate_s /= denom_s
+
+    # Calculate combine_weights and dispatch_mask
+    gate_all = einsum("ks,kse->kse", gate_s, mask_float)
+    locations_sc = F.one_hot(locations_s, num_classes=capacity).type_as(logits)
+    combine_sec = einsum("kse,ksc->ksec", gate_all, locations_sc)
+    combine_weights = torch.sum(combine_sec, dim=0)
+    dispatch_mask = combine_weights.bool()
+
+    return l_aux, combine_weights, dispatch_mask, exp_counts
+
+
 class TopKGate(Module):
     """Gate module which implements Top2Gating as described in Gshard_.
     ::
 
         gate = TopKGate(model_dim, num_experts)
         l_aux, combine_weights, dispatch_mask = gate(input)
 
@@ -308,58 +374,64 @@
         topk: int = 1,
         capacity_factor: float = 1.0,
         eval_capacity_factor: float = 1.0,
         min_capacity: int = 8,
         noisy_gate_policy: Optional[str] = None,
         drop_tokens: bool = True,
         use_rts: bool = True,
+        use_fused_gating: bool = False,
     ) -> None:
         super().__init__()
-
-        # Only top-1 and top-2 are supported at the moment.
-        if topk not in (1, 2):
-            raise ValueError("Only top-1 and top-2 gatings are supported.")
-        # Deepspeed's mechisms, alway use fp32
+        # alway use fp32
         self.wg = torch.nn.Linear(model_dim, num_experts, bias=False)
         self.k = topk
         self.capacity_factor = capacity_factor
         self.eval_capacity_factor = eval_capacity_factor
         self.min_capacity = min_capacity
         self.noisy_gate_policy = noisy_gate_policy
         self.wall_clock_breakdown = False
         self.gate_time = 0.0
         self.drop_tokens = drop_tokens
         self.use_rts = use_rts
+        self.use_fused_gating = use_fused_gating
 
     def forward(
         self, inputs: torch.Tensor, used_token: torch.Tensor = None
     ) -> Tuple[Tensor, Tensor, Tensor]:  # type: ignore
         if self.wall_clock_breakdown:
             timer("TopKGate").start()
 
         # input jittering
         if self.noisy_gate_policy == "Jitter" and self.training:
             inputs = multiplicative_jitter(inputs, device=inputs.device)
         logits = self.wg(inputs)
 
-        if self.k == 1:
+        if self.use_fused_gating or self.k > 2:
+            assert self.noisy_gate_policy != "RSample", "RSample noisy is not supported by fused_gating policy"
+            gate_output = fused_topkgating(
+                logits, self.k, self.capacity_factor if self.training else self.eval_capacity_factor, self.min_capacity
+            )
+        # deepspeed-style code
+        elif self.k == 1:
             gate_output = top1gating(
                 logits,
                 self.capacity_factor if self.training else self.eval_capacity_factor,
                 self.min_capacity,
                 used_token,
                 self.noisy_gate_policy if self.training else None,
                 self.drop_tokens,
                 self.use_rts,
             )
 
-        else:
+        elif self.k == 2:
             gate_output = top2gating(
                 logits, self.capacity_factor if self.training else self.eval_capacity_factor, self.min_capacity
             )
+        else:
+            assert False, "Unsupported gating policy"
 
         if self.wall_clock_breakdown:
             timer("TopKGate").stop()
             self.gate_time = timer("TopKGate").elapsed(reset=False)
 
         return gate_output
 
@@ -395,14 +467,15 @@
         top_k: int = 1,
         capacity_factor: float = 1.0,
         eval_capacity_factor: float = 1.0,
         min_capacity: int = 4,
         noisy_gate_policy: str = None,
         drop_tokens: bool = True,
         use_rts: bool = True,
+        use_fused_gating: bool = False,
         device: Optional[torch.device] = None,
         dtype: Optional[torch.device] = None,
     ) -> None:
         assert noisy_gate_policy is None or noisy_gate_policy in ["None", "Jitter", "RSample"], (
             "Unsupported noisy_gate_policy: " + noisy_gate_policy
         )
         assert (
@@ -415,14 +488,15 @@
                 top_k,
                 capacity_factor,
                 eval_capacity_factor,
                 min_capacity,
                 noisy_gate_policy,
                 drop_tokens,
                 use_rts,
+                use_fused_gating,
             ),
             torch.nn.ModuleList(
                 [
                     ep_cls(
                         in_features,
                         hidden_features,
                         out_features,
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/megablock_dmoe.py` & `InternEvo-0.4.2/internlm/model/moe/megablock/megablock_dmoe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/megablock_moe.py` & `InternEvo-0.4.2/internlm/model/moe/megablock/megablock_moe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/mlp.py` & `InternEvo-0.4.2/internlm/model/moe/megablock/mlp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/moe/megablock/utils.py` & `InternEvo-0.4.2/internlm/model/moe/megablock/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/moe/moe.py` & `InternEvo-0.4.2/internlm/model/moe/moe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/moe/utils.py` & `InternEvo-0.4.2/internlm/model/moe/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/ops/linear.py` & `InternEvo-0.4.2/internlm/model/ops/linear.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/ops/norm.py` & `InternEvo-0.4.2/internlm/model/ops/norm.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/model/utils.py` & `InternEvo-0.4.2/internlm/model/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,31 +6,37 @@
 import torch
 import torch.distributed as dist
 import torch.nn.functional as F
 from torch import Tensor
 from torch.distributed import ProcessGroup
 from torch.nn.utils.rnn import pad_sequence
 
-from internlm.accelerator import AcceleratorType, get_accelerator
+from internlm.accelerator import get_accelerator
 from internlm.core.context import global_context as gpc
 from internlm.utils.logger import get_logger
 
-try:
-    import fused_dense_lib as fused_dense_cuda
-except (ModuleNotFoundError, ImportError):
-    print("Import fused_dense_lib failed!")
-
 internlm_accelerator = get_accelerator()
 
 custom_bwd = internlm_accelerator.return_custom_bwd()
 custom_fwd = internlm_accelerator.return_custom_fwd()
 
 logger = get_logger(__file__)
 
 
+def linear_bias_wgrad_torch(my_input, grad_output, has_d_bias):
+    assert my_input.dtype == grad_output.dtype
+    grad_weight = torch.matmul(grad_output.t(), my_input)
+    grad_bias = grad_output.sum(dim=0) if has_d_bias else None
+    return grad_weight, grad_bias
+
+
+linear_bias_wgrad = linear_bias_wgrad_torch
+is_using_cuda_linear_bias_wgrad = False
+
+
 # Raw operation, does not support autograd, but does support async
 def all_reduce_raw(input_: Tensor, process_group: ProcessGroup, async_op: bool = False):
     input_ = input_.contiguous()
     handle = torch.distributed.all_reduce(input_, group=process_group, async_op=async_op)
     return input_, handle
 
 
@@ -219,21 +225,14 @@
             device=input_.device,
         ).contiguous()
 
     handle = dist.reduce_scatter_tensor(output, input_.contiguous(), op=op, group=process_group, async_op=async_op)
     return output, handle
 
 
-def linear_bias_wgrad_torch(my_input, grad_output, has_d_bias):
-    assert my_input.dtype == grad_output.dtype
-    grad_weight = torch.matmul(grad_output.t(), my_input)
-    grad_bias = grad_output.sum(dim=0) if has_d_bias else None
-    return grad_weight, grad_bias
-
-
 # adpated from https://github.com/Dao-AILab/flash-attention/blob/main/flash_attn/ops/fused_dense.py
 class FusedDenseFunc(torch.autograd.Function):
     "FusedDenseFunc for tensor parallel in flash-attn implementation."
 
     @staticmethod
     @custom_fwd
     def forward(
@@ -241,26 +240,31 @@
         x,
         weight,
         bias,
         return_residual=False,
         process_group=None,
         sequence_parallel=True,
         gather_dim=0,
-        is_using_cuda: bool = True,
+        dtype_eligible: bool = True,
     ):
         """
         If process_group is not None and sequence_parallel=True, we're doing Tensor Parallel
         with sequence parallelism: we do an all_gather_raw of x before doing the matmul.
         """
         ctx.compute_weight_gradient = weight.requires_grad
         ctx.return_residual = return_residual
         ctx.process_group = process_group
         ctx.sequence_parallel = sequence_parallel
         ctx.gather_dim = gather_dim
-        ctx.is_using_cuda = is_using_cuda
+        ctx.dtype_eligible = dtype_eligible
+
+        if ctx.dtype_eligible is False:
+            global linear_bias_wgrad, is_using_cuda_linear_bias_wgrad
+            linear_bias_wgrad = linear_bias_wgrad_torch
+            is_using_cuda_linear_bias_wgrad = False
 
         if torch.is_autocast_enabled():
             x = x.to(dtype=torch.get_autocast_gpu_dtype())
         x = x.contiguous()
         if process_group is not None and sequence_parallel:
             # We want to kick off the all_gather early, before weight dtype conversion
             total_x, handle_x = all_gather_raw(x, process_group, async_op=True, gather_dim=gather_dim)
@@ -274,15 +278,15 @@
         if process_group is not None and sequence_parallel and handle_x is not None:
             handle_x.wait()
         batch_shape, n = total_x.shape[:-1], total_x.shape[-1]
         batch_dim = batch_shape.numel()
         # https://github.com/pytorch/pytorch/blob/5b51849b48a7dbccd297286cc0110def4706f9e7/aten/src/ATen/native/cuda/Blas.cpp#L174
         if min(batch_dim, n, *weight.shape) > 65535 * 32:
             raise RuntimeError("fused_dense only supports matrix dims <= 2M")
-        output = F.linear(total_x, weight, bias)
+        output = F.linear(total_x, weight, bias)  # pylint: disable=E1102
         if ctx.compute_weight_gradient:
             ctx.save_for_backward(x, weight)
         else:
             ctx.save_for_backward(weight)
         return output if not return_residual else (output, x)
 
     @staticmethod
@@ -291,36 +295,29 @@
         grad_output = grad_output.contiguous()
         if ctx.return_residual:
             (grad_input,) = args
             grad_input = grad_input.contiguous()
         process_group = ctx.process_group
         sequence_parallel = ctx.sequence_parallel
         gather_dim = ctx.gather_dim
-
-        if gpc.config.use_cuda_flash_attn and AcceleratorType.GPU == get_accelerator().get_accelerator_backend():
-            assert ctx.is_using_cuda, "CUDA Flash Attention only support GPU device"
-            backward_func = fused_dense_cuda.linear_bias_wgrad
-        else:
-            backward_func = linear_bias_wgrad_torch
-
         if ctx.compute_weight_gradient:
             x, weight = ctx.saved_tensors
             if process_group is not None and sequence_parallel:
                 total_x, handle_x = all_gather_raw(x, process_group, async_op=True, gather_dim=gather_dim)
             else:
                 total_x = x
         else:
             (weight,) = ctx.saved_tensors
             total_x = None
         batch_shape = grad_output.shape[:-1]
         batch_dim = batch_shape.numel()
         grad_output = grad_output.reshape(batch_dim, grad_output.shape[-1])
         if ctx.needs_input_grad[0]:
             if not ctx.return_residual:
-                grad_input = F.linear(grad_output, weight.t())
+                grad_input = F.linear(grad_output, weight.t())  # pylint: disable=E1102
             else:
                 grad_input = torch.addmm(
                     grad_input.reshape(batch_dim, grad_input.shape[-1]),
                     grad_output,
                     weight,
                 )
             grad_input = grad_input.reshape(*batch_shape, grad_input.shape[-1])
@@ -333,15 +330,15 @@
                     grad_input, handle_grad_input = all_reduce_raw(grad_input, process_group, async_op=True)
         else:
             grad_input = None
         if ctx.needs_input_grad[1]:
             assert ctx.compute_weight_gradient
             if process_group is not None and sequence_parallel and handle_x is not None:
                 handle_x.wait()
-            grad_weight, grad_bias = backward_func(
+            grad_weight, grad_bias = linear_bias_wgrad(
                 total_x.reshape(batch_dim, total_x.shape[-1]),
                 grad_output,
                 ctx.needs_input_grad[2],
             )
         else:
             grad_weight = None
             grad_bias = grad_output if ctx.needs_input_grad[2] else None
@@ -364,25 +361,30 @@
         x,
         weight,
         bias,
         return_residual=False,
         process_group=None,
         sequence_parallel=True,
         gather_dim=0,
-        is_using_cuda: bool = True,
+        dtype_eligible: bool = True,
     ):
         """
         If process_group is not None and sequence_parallel=True, we're doing Tensor Parallel
         with sequence parallelism: we do an all_gather_raw of x before doing the matmul.
         """
         ctx.compute_weight_gradient = weight.requires_grad
         ctx.return_residual = return_residual
         ctx.process_group = process_group
         ctx.sequence_parallel = sequence_parallel
-        ctx.is_using_cuda = is_using_cuda
+        ctx.dtype_eligible = dtype_eligible
+
+        if ctx.dtype_eligible is False:
+            global linear_bias_wgrad, is_using_cuda_linear_bias_wgrad
+            linear_bias_wgrad = linear_bias_wgrad_torch
+            is_using_cuda_linear_bias_wgrad = False
 
         if torch.is_autocast_enabled():
             x = x.to(dtype=torch.get_autocast_gpu_dtype())
         x = x.contiguous()
         if process_group is not None and sequence_parallel:
             # We want to kick off the all_gather early, before weight dtype conversion
             total_x, handle_x = all_gather_raw(x, process_group, async_op=True, gather_dim=gather_dim)
@@ -396,15 +398,15 @@
         if process_group is not None and sequence_parallel and handle_x is not None:
             handle_x.wait()
         batch_shape, n = total_x.shape[:-1], total_x.shape[-1]
         batch_dim = batch_shape.numel()
         # https://github.com/pytorch/pytorch/blob/5b51849b48a7dbccd297286cc0110def4706f9e7/aten/src/ATen/native/cuda/Blas.cpp#L174
         if min(batch_dim, n, *weight.shape) > 65535 * 32:
             raise RuntimeError("fused_dense only supports matrix dims <= 2M")
-        output = F.linear(total_x, weight, bias)
+        output = F.linear(total_x, weight, bias)  # pylint: disable=E1102
         if ctx.compute_weight_gradient:
             ctx.save_for_backward(total_x, weight)
         else:
             ctx.save_for_backward(weight)
         return output if not return_residual else (output, x)
 
     @staticmethod
@@ -412,32 +414,25 @@
     def backward(ctx, grad_output, *args):
         grad_output = grad_output.contiguous()
         if ctx.return_residual:
             (grad_input,) = args
             grad_input = grad_input.contiguous()
         process_group = ctx.process_group
         sequence_parallel = ctx.sequence_parallel
-
-        if gpc.config.use_cuda_flash_attn and AcceleratorType.GPU == get_accelerator().get_accelerator_backend():
-            assert ctx.is_using_cuda, "CUDA Flash Attention only support GPU device"
-            backward_func = fused_dense_cuda.linear_bias_wgrad
-        else:
-            backward_func = linear_bias_wgrad_torch
-
         if ctx.compute_weight_gradient:
             total_x, weight = ctx.saved_tensors
         else:
             (weight,) = ctx.saved_tensors
             total_x = None
         batch_shape = grad_output.shape[:-1]
         batch_dim = batch_shape.numel()
         grad_output = grad_output.reshape(batch_dim, grad_output.shape[-1])
         if ctx.needs_input_grad[0]:
             if not ctx.return_residual:
-                grad_input = F.linear(grad_output, weight.t())
+                grad_input = F.linear(grad_output, weight.t())  # pylint: disable=E1102
             else:
                 grad_input = torch.addmm(
                     grad_input.reshape(batch_dim, grad_input.shape[-1]),
                     grad_output,
                     weight,
                 )
             grad_input = grad_input.reshape(*batch_shape, grad_input.shape[-1])
@@ -448,15 +443,15 @@
                     )
                 else:
                     grad_input, handle_grad_input = all_reduce_raw(grad_input, process_group, async_op=True)
         else:
             grad_input = None
         if ctx.needs_input_grad[1]:
             assert ctx.compute_weight_gradient
-            grad_weight, grad_bias = backward_func(
+            grad_weight, grad_bias = linear_bias_wgrad(
                 total_x.reshape(batch_dim, total_x.shape[-1]),
                 grad_output,
                 ctx.needs_input_grad[2],
             )
         else:
             grad_weight = None
             grad_bias = grad_output if ctx.needs_input_grad[2] else None
@@ -474,21 +469,26 @@
         ctx,
         x,
         weight,
         bias,
         module,
         communicator,
         return_residual=False,
-        is_using_cuda: bool = True,
+        dtype_eligible: bool = True,
     ):
         ctx.compute_weight_gradient = weight.requires_grad
         ctx.return_residual = return_residual
         ctx.module = module
         ctx.communicator = communicator
-        ctx.is_using_cuda = is_using_cuda
+        ctx.dtype_eligible = dtype_eligible
+
+        if ctx.dtype_eligible is False:
+            global linear_bias_wgrad, is_using_cuda_linear_bias_wgrad
+            linear_bias_wgrad = linear_bias_wgrad_torch
+            is_using_cuda_linear_bias_wgrad = False
 
         if torch.is_autocast_enabled():
             x = x.to(dtype=torch.get_autocast_gpu_dtype())
         x = x.contiguous()
 
         total_weight = communicator.all_gather(weight, module)
         total_bias = bias if bias is None else communicator.all_gather(bias, module, is_bias=True)
@@ -501,15 +501,15 @@
         total_weight = total_weight.contiguous()
         batch_shape, n = x.shape[:-1], x.shape[-1]
         batch_dim = batch_shape.numel()
         # https://github.com/pytorch/pytorch/blob/5b51849b48a7dbccd297286cc0110def4706f9e7/aten/src/ATen/native/cuda/Blas.cpp#L174
         if min(batch_dim, n, *total_weight.shape) > 65535 * 32:
             raise RuntimeError("fused_dense only supports matrix dims <= 2M")
 
-        output = F.linear(x, total_weight, total_bias)
+        output = F.linear(x, total_weight, total_bias)  # pylint: disable=E1102
 
         # release memory
         del total_weight
         del total_bias
         if ctx.compute_weight_gradient:
             ctx.save_for_backward(x, weight)
         else:
@@ -517,21 +517,14 @@
         return output if not return_residual else (output, x)
 
     @staticmethod
     @custom_bwd
     def backward(ctx, grad_output, *args):
         module = ctx.module
         communicator = ctx.communicator
-
-        if gpc.config.use_cuda_flash_attn and AcceleratorType.GPU == get_accelerator().get_accelerator_backend():
-            assert ctx.is_using_cuda, "CUDA Flash Attention only support GPU device"
-            backward_func = fused_dense_cuda.linear_bias_wgrad
-        else:
-            backward_func = linear_bias_wgrad_torch
-
         grad_output = grad_output.contiguous()
         if ctx.return_residual:
             (grad_input,) = args
             grad_input = grad_input.contiguous()
 
         if ctx.compute_weight_gradient:
             x, weight = ctx.saved_tensors
@@ -543,15 +536,15 @@
         grad_output = grad_output.reshape(batch_dim, grad_output.shape[-1])
 
         total_weight = communicator.all_gather(weight, module)
 
         # compute weight grad
         if ctx.needs_input_grad[1]:
             assert ctx.compute_weight_gradient
-            grad_weight, grad_bias = backward_func(
+            grad_weight, grad_bias = linear_bias_wgrad(
                 x.reshape(batch_dim, x.shape[-1]),
                 grad_output,
                 ctx.needs_input_grad[2],
             )
 
             grad_weight, grad_weight_sync = communicator.reduce_scatter(grad_weight, module, op=dist.ReduceOp.AVG)
             if grad_bias is not None:
@@ -560,15 +553,15 @@
                 )
         else:
             grad_weight = None
             grad_bias = grad_output if ctx.needs_input_grad[2] else None
 
         if ctx.needs_input_grad[0]:
             if not ctx.return_residual:
-                grad_input = F.linear(grad_output, total_weight.t())
+                grad_input = F.linear(grad_output, total_weight.t())  # pylint: disable=E1102
             else:
                 grad_input = torch.addmm(
                     grad_input.reshape(batch_dim, grad_input.shape[-1]),
                     grad_output,
                     total_weight,
                 )
             grad_input = grad_input.reshape(*batch_shape, grad_input.shape[-1])
@@ -594,26 +587,23 @@
     process_group: Optional[ProcessGroup] = None,
     sequence_parallel: bool = True,
     gather_dim: int = 0,
 ):
     dtype_eligible = x.dtype in [torch.float16, torch.bfloat16] or (
         x.dtype == torch.float32 and torch.is_autocast_enabled()
     )
-    is_using_cuda = (
-        internlm_accelerator.get_accelerator_backend() in [AcceleratorType.GPU, AcceleratorType.DIPU]
-    ) and dtype_eligible
     return FusedDenseFunc.apply(
         x,
         weight,
         bias,
         return_residual,
         process_group,
         sequence_parallel,
         gather_dim,
-        is_using_cuda,
+        dtype_eligible,
     )
 
 
 def megatron_fused_dense_func(
     x: Tensor,
     weight: Tensor,
     bias: Optional[Tensor] = None,
@@ -621,78 +611,48 @@
     process_group: Optional[ProcessGroup] = None,
     sequence_parallel: bool = True,
     gather_dim: int = 0,
 ):
     dtype_eligible = x.dtype in [torch.float16, torch.bfloat16] or (
         x.dtype == torch.float32 and torch.is_autocast_enabled()
     )
-    is_using_cuda = (
-        internlm_accelerator.get_accelerator_backend() in [AcceleratorType.GPU, AcceleratorType.DIPU]
-    ) and dtype_eligible
     return MegatronFusedDenseFunc.apply(
         x,
         weight,
         bias,
         return_residual,
         process_group,
         sequence_parallel,
         gather_dim,
-        is_using_cuda,
+        dtype_eligible,
     )
 
 
 def isp_fused_dense_func(
     x: Tensor,
     weight: Tensor,
     module,
     communicator,
     bias: Optional[Tensor] = None,
     return_residual: bool = False,
 ):
     dtype_eligible = x.dtype in [torch.float16, torch.bfloat16] or (
         x.dtype == torch.float32 and torch.is_autocast_enabled()
     )
-    is_using_cuda = (
-        internlm_accelerator.get_accelerator_backend() in [AcceleratorType.GPU, AcceleratorType.DIPU]
-    ) and dtype_eligible
     return ISPFusedDenseFunc.apply(
         x,
         weight,
         bias,
         module,
         communicator,
         return_residual,
-        is_using_cuda,
+        dtype_eligible,
     )
 
 
-def try_import_RMSNorm():
-    """
-    Try import MixFusedRMSNorm from apex, if failed, return our RMSNorm
-
-    """
-    try:
-        device_backend = internlm_accelerator.get_accelerator_backend()
-        if device_backend == AcceleratorType.DIPU:
-            from deeplink_ext.internlm_ops.rms_norm import (
-                DeepLinkRMSNormWithNormalizedShape as RMSNorm,
-            )
-
-            return RMSNorm
-        else:
-            from apex.normalization.fused_layer_norm import MixedFusedRMSNorm as RMSNorm
-
-            return RMSNorm
-    except (ModuleNotFoundError, ImportError):
-        logger.warning("The torch implementation for MixFusedRMSNorm is slower than apex. Please note this!")
-        from internlm.model.ops.norm import RMSNormTorch as RMSNorm
-
-        return RMSNorm
-
-
 def is_moe_param(param: torch.Tensor) -> bool:
     if hasattr(param, "is_expert") and param.is_expert:
         return True
     return False
 
 
 def Silu(w1_o, w2_o):
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/monitor/alert.py` & `InternEvo-0.4.2/internlm/monitor/alert.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/monitor/monitor.py` & `InternEvo-0.4.2/internlm/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/monitor/utils.py` & `InternEvo-0.4.2/internlm/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/solver/activation_checkpoint.py` & `InternEvo-0.4.2/internlm/solver/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/base_optimizer.py` & `InternEvo-0.4.2/internlm/solver/optimizer/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/fsdp_optimizer.py` & `InternEvo-0.4.2/internlm/solver/optimizer/fsdp_optimizer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/hybrid_zero_optim.py` & `InternEvo-0.4.2/internlm/solver/optimizer/hybrid_zero_optim.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/store.py` & `InternEvo-0.4.2/internlm/solver/optimizer/store.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/solver/optimizer/utils.py` & `InternEvo-0.4.2/internlm/solver/optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/solver/pipeline_utils.py` & `InternEvo-0.4.2/internlm/solver/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/solver/schedulers/beta2_scheduler.py` & `InternEvo-0.4.2/internlm/solver/schedulers/beta2_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/solver/schedulers/lr_scheduler.py` & `InternEvo-0.4.2/internlm/solver/schedulers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/train/__init__.py` & `InternEvo-0.4.2/internlm/train/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,22 +4,20 @@
     initialize_llm_profile,
     initialize_model,
     initialize_optimizer,
     load_new_batch,
     record_current_batch_training_metrics,
     set_fp32_attr_for_model,
     set_parallel_attr_for_param_groups,
-    wrap_FSDP_model,
 )
 
 __all__ = [
     "initialize_llm_profile",
     "initialize_model",
     "initialize_isp_communicator",
     "initialize_optimizer",
     "load_new_batch",
     "record_current_batch_training_metrics",
-    "wrap_FSDP_model",
     "get_scheduler_hooks",
     "set_parallel_attr_for_param_groups",
     "set_fp32_attr_for_model",
 ]
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/train/pipeline.py` & `InternEvo-0.4.2/internlm/train/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
-import functools
+import math
 import time
 from typing import Callable, Iterable, List, Optional, Union
 
 import torch
 from torch import nn
-from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
-from torch.distributed.fsdp.fully_sharded_data_parallel import (
-    BackwardPrefetch,
-    ShardingStrategy,
-)
-from torch.distributed.fsdp.wrap import transformer_auto_wrap_policy
 from torch.utils.data import DataLoader
 
 from internlm.accelerator import AcceleratorType, get_accelerator
 from internlm.core.communication.isp import (
     ISPCommModelConfig,
     ISPCommunicator,
     ISPCommunicatorSchedulerHook,
@@ -33,30 +27,30 @@
 from internlm.core.context import global_context as gpc
 from internlm.core.context.random import set_mode
 from internlm.core.naive_amp import NaiveAMPModel, set_fp32_attr_to_module
 from internlm.core.trainer import TrainState
 from internlm.data.utils import unpack_data
 from internlm.model.metrics import SchedulerMetricHook
 from internlm.model.modules.embedding import Embedding1D
-from internlm.model.modules.mlp import FeedForward
-from internlm.model.modules.multi_head_attention import MHA
 from internlm.model.moe.megablock.mlp import (
     MegaBlockFeedForward,
     MegaBlockGroupedFeedForward,
 )
 from internlm.model.moe.moe import MoE
+from internlm.model.ops.fusion_ops_import_helper import (
+    try_import_FusedAdamW,
+    try_import_RMSNorm,
+)
 from internlm.model.ops.linear import (
     BaseScaleColumnParallelLinear,
     ColumnParallelLinearTorch,
     ISPLinear,
-    RewardModelLinear,
     RowParallelLinearTorch,
-    ScaleColumnParallelLinear,
 )
-from internlm.model.utils import is_moe_param, try_import_RMSNorm
+from internlm.model.utils import is_moe_param
 from internlm.monitor import set_env_var
 from internlm.monitor.monitor import monitor_manager as mm
 from internlm.solver.optimizer import FSDPadaptOptimizer, HybridZeroOptimizer
 from internlm.solver.schedulers.beta2_scheduler import Beta2Scheduler
 from internlm.solver.schedulers.lr_scheduler import FineTuneCosineAnnealingWarmupLR
 from internlm.train.utils import create_param_groups
 from internlm.utils.common import DummyProfile, SchedulerHook, get_current_device
@@ -92,31 +86,28 @@
     for _chunk in model:
         for _, module in _chunk.named_modules():
             if isinstance(module, (RMSNorm, nn.LayerNorm)) and gpc.config.get("use_fp32_norm", False):
                 set_fp32_attr_to_module(module)
 
 
 def set_parallel_attr_for_param_groups(model: Union[nn.Module, nn.ModuleList]):
-    def _check_module(module):
+    def _check_module(name, module):
         # layer_norm
         if isinstance(module, (RMSNorm, nn.LayerNorm)):
             for param in module.parameters():
                 setattr(param, IS_REPLICA_ZERO_PARALLEL, True)
 
         if isinstance(module, MoE):
             for param in module.moe_layer.gate.parameters():
                 setattr(param, IS_REPLICA_ZERO_PARALLEL, True)
 
         # embedding and head
-        if gpc.config.use_cuda_flash_attn:
-            from flash_attn.modules.embedding import ParallelGPT2Embeddings
+        embedding_head_cls = (Embedding1D, BaseScaleColumnParallelLinear)
 
-        if isinstance(module, (Embedding1D, BaseScaleColumnParallelLinear)) or (
-            gpc.config.use_cuda_flash_attn and isinstance(module, ParallelGPT2Embeddings)
-        ):
+        if isinstance(module, embedding_head_cls):
             for param in module.parameters():
                 if gpc.is_initialized(ParallelMode.TENSOR) and is_using_isp():
                     setattr(param, IS_TENSOR_DATA_PARALLEL, True)
                 elif gpc.is_initialized(ParallelMode.TENSOR) and not is_using_isp():
                     setattr(param, IS_TENSOR_ZERO_PARALLEL, True)
 
         # for linear module
@@ -129,24 +120,32 @@
                     # module should be MoE experts's linear
                     setattr(param, IS_TENSOR_EXPERT_DATA_PARALLEL, True)
                 elif not is_moe_param(param) and gpc.is_initialized(ParallelMode.TENSOR) and not is_using_isp():
                     setattr(param, IS_TENSOR_ZERO_PARALLEL, True)
                 elif not is_moe_param(param) and gpc.is_initialized(ParallelMode.WEIGHT) and is_using_isp():
                     setattr(param, IS_WEIGHT_ZERO_PARALLEL, True)
 
+        # for vit and vit project
+        if "vision_tower" in name.lower() or "vision_proj" in name.lower():
+            for param in module.parameters():
+                if gpc.is_initialized(ParallelMode.TENSOR) and is_using_isp():
+                    setattr(param, IS_TENSOR_DATA_PARALLEL, True)
+                elif gpc.is_initialized(ParallelMode.TENSOR) and not is_using_isp():
+                    setattr(param, IS_TENSOR_ZERO_PARALLEL, True)
+
     if not isinstance(model, nn.ModuleList):
         model = [model]
 
     for _chunk in model:
         if isinstance(_chunk, NaiveAMPModel):
             _chunk = _chunk.model
 
         # set param parallel attribute
         for name, module in _chunk.named_modules():
-            _check_module(module)
+            _check_module(name, module)
 
         for name, param in _chunk.named_parameters():
             assert (
                 is_replica_zero_parallel_parameter(param)
                 or is_tensor_data_parallel_parameter(param)
                 or is_tensor_zero_parallel_parameter(param)
                 or is_weight_zero_parallel_parameter(param)
@@ -204,53 +203,14 @@
     sync_model_replica_param_group(model)
 
     # Change random state mode to ParallelMode.DATA after model is built, guaranteeing the random
     # state in the same dp group are all the same.
     random_mode = ParallelMode.WEIGHT_DATA if is_using_isp() else ParallelMode.DATA
     set_mode(random_mode)
 
-    # if fsdp enabled, wrap the model
-    model = wrap_FSDP_model(model)
-
-    return model
-
-
-def wrap_FSDP_model(model: Union[nn.Module, nn.ModuleList]):
-    if gpc.config.parallel.zero1.fsdp and gpc.config.model.use_flash_attn:
-        from flash_attn.modules.embedding import ParallelGPT2Embeddings
-        from flash_attn.modules.mlp import ParallelFusedMLP
-
-        # set wrap_policy for fsdp wrap
-        transformer_wrap_policy = functools.partial(
-            transformer_auto_wrap_policy,
-            transformer_layer_cls={
-                Embedding1D,
-                ParallelGPT2Embeddings,
-                MHA,
-                RMSNorm,
-                FeedForward,
-                ParallelFusedMLP,
-                RewardModelLinear,
-                ScaleColumnParallelLinear,
-            },
-        )
-
-        # wrap the model
-        grp = gpc.get_group(ParallelMode.ZERO1)
-        model = FSDP(  # pylint: disable=unexpected-keyword-arg
-            module=model,
-            process_group=grp,
-            sharding_strategy=ShardingStrategy.FULL_SHARD,
-            auto_wrap_policy=transformer_wrap_policy,
-            forward_prefetch=True,
-            backward_prefetch=BackwardPrefetch.BACKWARD_PRE,
-            limit_all_gathers=True,
-            use_orig_params=True,
-        )
-
     return model
 
 
 def initialize_isp_communicator(model: Union[nn.Module, nn.ModuleList]):
     """
     Initialize communicator for isp tensor parallel mode.
 
@@ -292,24 +252,17 @@
     """
 
     adam_cfg = gpc.config.adam
     zero_cfg = gpc.config.hybrid_zero_optimizer
     grad_scal_cfg = gpc.config.grad_scaler
 
     params = create_param_groups(model, adam_cfg.weight_decay)
-    adam_extra_kwargs = {}
-    # set fused=True to avoid nan grad norm when model size is larger and use_fp32_norm=True
 
     # TODO(caikun): add DIPU backend adamw
-    if internlm_accelerator.get_accelerator_backend() == AcceleratorType.NPU:
-        internlm_adamw = torch_npu.optim.NpuFusedAdamW
-    else:
-        internlm_adamw = torch.optim.AdamW
-        if torch.__version__ >= "2.1.0" and internlm_accelerator.get_accelerator_backend() == AcceleratorType.GPU:
-            adam_extra_kwargs["fused"] = True
+    adam_extra_kwargs, internlm_adamw = try_import_FusedAdamW()
 
     naive_optimizer = internlm_adamw(
         params=params,
         lr=adam_cfg.lr,
         betas=(adam_cfg.adam_beta1, adam_cfg.adam_beta2),
         eps=adam_cfg.adam_eps,
         **adam_extra_kwargs,
@@ -473,15 +426,14 @@
     beta2_scheduler,
     trainer,
     start_time,
     loss,
     moe_loss,
     grad_norm,
     metric,
-    update_panel,
 ):
     """
     Print some training metrics of current batch.
     """
 
     set_env_var(key="LAST_ACTIVE_TIMESTAMP", value=int(time.time()))
 
@@ -495,14 +447,15 @@
         lr = optimizer.param_groups[0]["lr"]
         if hasattr(trainer.engine.optimizer, "grad_scaler"):
             scaler = trainer.engine.optimizer.grad_scaler._scale.item()
         elif hasattr(trainer.engine.optimizer.optim, "grad_scaler"):
             scaler = trainer.engine.optimizer.optim.grad_scaler._scale.item()
 
         num_tokens_in_batch = batch[1].nelement()
+        real_num_tokens = math.ceil(acc_perplex.pop("real_token_num") / gpc.get_world_size(ParallelMode.GLOBAL))
         num_samples_in_batch = sum([len(b) - 1 for b in batch[0]["cu_seqlens"]])
         max_length_in_batch = max([(b[1:] - b[:-1]).max().item() for b in batch[0]["cu_seqlens"]])
         max_samples_in_batch = max([len(b) - 1 for b in batch[0]["cu_seqlens"]])
         min_samples_in_batch = min([len(b) - 1 for b in batch[0]["cu_seqlens"]])
         time_cost = time.time() - start_time
         tk_per_gpu = round(
             num_tokens_in_batch * gpc.get_world_size(ParallelMode.DATA) / gpc.get_world_size(ParallelMode.GLOBAL),
@@ -542,28 +495,34 @@
         last_tgs_10 = tgs_statistic["last_tgs_10"]
         last_tgs_50 = tgs_statistic["last_tgs_50"]
 
         tgs_all = round(tgs_statistic["sum_tg"] / tgs_statistic["sum_time"], 2)
         tgs_avg = round(tgs_statistic["sum_tgs"] / tgs_statistic["sum_step"], 2)
         tgs_SMA = round(tgs_statistic["SMA_tg_50"] / tgs_statistic["SMA_time_50"], 2)
 
-        tflops = get_tflops_func((time.time() - start_time))
+        tflops = get_tflops_func(time_cost)
 
         tgs_origin = round(
             num_tokens_in_batch
             * gpc.get_world_size(ParallelMode.DATA)
             / gpc.get_world_size(ParallelMode.GLOBAL)
-            / (time.time() - start_time),
+            / time_cost,
+            2,
+        )
+
+        real_tgs = round(
+            real_num_tokens / time_cost,
             2,
         )
 
         infos = {
             "tflops": tflops,
             "step": batch_count,
             "loss": loss.item() - moe_loss.item() if moe_loss is not None else loss.item(),
+            "real_tgs": real_tgs,
             "tgs (tokens/gpu/second)": tgs_origin,
             "tgs/last_tgs_1": last_tgs_1,
             "tgs/tgs_all": tgs_all,
             "tgs/tgs_avg": tgs_avg,
             "tgs/tgs_SMA": tgs_SMA,
             "tgs/last_tgs_10": last_tgs_10,
             "tgs/last_tgs_50": last_tgs_50,
@@ -593,39 +552,15 @@
         for key, value in infos.items():
             line += f"{key}={value} "
             if isinstance(value, dict):
                 writer.add_scalars(key=key, value=value, step=train_state.step_count)
             else:
                 writer.add_scalar(key=key, value=value, step=train_state.step_count)
 
-        if update_panel:
-            # metrics shown with dashboard panels
-            panel_metrics = {
-                "step": batch_count,
-                "lr": lr,
-                "num_consumed_tokens": train_state.num_consumed_tokens,
-                "loss": loss.item() - moe_loss.item() if moe_loss is not None else loss.item(),
-                "flops": tflops,
-                "tgs": last_tgs_1,
-                "acc": acc_perplex["acc"],
-                "perplexity": acc_perplex["perplexity"],
-                "fwd_bwd_time": fwd_bwd_time,
-            }
-            if moe_loss is not None:
-                panel_metrics["moe_loss"] = moe_loss.item()
-            for norm_key, norm_value in grad_norm.items():
-                panel_metrics[norm_key] = norm_value
-
-            logger.info(
-                "{line}",
-                line=line,
-                extra=panel_metrics,
-            )
-        else:
-            logger.info(line)
+        logger.info(line)
 
         # if loss spike occurs, send alert info to feishu
         mm.monitor_loss_spike(
             alert_address=gpc.config.monitor.alert.feishu_alert_address,
             step_count=batch_count,
             cur_step_loss=loss.item(),
         )
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/train/utils.py` & `InternEvo-0.4.2/internlm/train/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,28 +57,32 @@
                     group[ori_key] = pgroup[ori_key]
         # assign param
         origin_params = []
         for param in pgroup["params"]:
             if is_tensor_data_parallel_parameter(param):
                 # should not be here if not isp mode
                 new_groups["embed_head"]["params"].append(param)
-            elif param.dtype == torch.float32:
-                new_groups["fp32"]["params"].append(param)
             # moe param means MoE is enabled
             elif is_moe_param(param):
                 new_groups[param.group_name]["params"].append(param)
+            elif param.dtype == torch.float32 and gpc.config.model.dtype != torch.float32:
+                new_groups["fp32"]["params"].append(param)
             else:
                 origin_params.append(param)
 
         # default param group, which is the first group in the param groups
         pgroup["params"] = origin_params
         pgroup["optimizer_mode"] = ParallelMode.ZERO1
 
     # param groups may contain empty groups, such as fp32
     param_groups.extend(new_groups.values())
 
     return tuple(param_groups)
 
 
 def create_param_groups(model, weight_decay):
-    parameters = {"params": list(model.parameters()), "name": "default", "weight_decay": weight_decay}
+    parameters = {
+        "params": [param for param in model.parameters() if param.requires_grad],
+        "name": "default",
+        "weight_decay": weight_decay,
+    }
     return split_params_into_different_groups_for_optimizer(parameters)
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/utils/common.py` & `InternEvo-0.4.2/internlm/utils/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,26 +136,33 @@
 def launch_time():
     global CURRENT_TIME
     if not CURRENT_TIME:
         CURRENT_TIME = datetime.now().strftime("%m-%d-%H:%M:%S")
     return CURRENT_TIME
 
 
-def set_random_seed(seed):
-    """Set random seed for reproducability."""
+def set_random_seed(seed, cuda_deterministic=False):
+    """Set all random seed for reproducability."""
     # It is recommended to use this only when inference.
-    if seed is not None:
-        assert seed > 0
-        random.seed(seed)
-        np.random.seed(seed)
-        torch.manual_seed(seed)
+    assert seed > 0, f"Seed should be a positive integer, but got {seed}"
+    random.seed(seed)
+    np.random.seed(seed)
+    torch.manual_seed(seed)
+    if internlm_accelerator.is_available():
         internlm_accelerator.manual_seed(seed)
         # if you are using multi-GPU.
         internlm_accelerator.manual_seed_all(seed)
 
+    if cuda_deterministic:  # slower, more reproducible
+        torch.backends.cudnn.deterministic = True
+        torch.backends.cudnn.benchmark = False
+    else:
+        torch.backends.cudnn.deterministic = False
+        torch.backends.cudnn.benchmark = True
+
 
 @contextmanager
 def conditional_context(context_manager, enable=True):
     if enable:
         with context_manager:
             yield
     else:
@@ -237,16 +244,17 @@
     tflops = flops_per_iteration / (elapsed_time_per_iter * global_world_size * (10**12))
     return tflops
 
 
 def enable_pytorch_expandable_segments():
     if torch.__version__ >= "2.1.0" and AcceleratorType.GPU == internlm_accelerator.get_accelerator_backend():
         _alloc_setting = "expandable_segments:True"
-        if os.getenv("PYTORCH_CUDA_ALLOC_CONF", None) is not None:
-            _alloc_setting = os.getenv("PYTORCH_CUDA_ALLOC_CONF") + "," + _alloc_setting
+        assert (
+            os.getenv("PYTORCH_CUDA_ALLOC_CONF", None) is None
+        ), "PYTORCH_CUDA_ALLOC_CONF should not be set when using expandable_segments"
         internlm_accelerator.memory._set_allocator_settings(_alloc_setting)
     else:
         logger.warning("To support the 'expandable_segments' configuration, please upgrade torch to version 2.1.0.")
 
 
 class DummyProfile:
     """
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/utils/gputest.py` & `InternEvo-0.4.2/internlm/utils/gputest.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/utils/logger.py` & `InternEvo-0.4.2/internlm/utils/logger.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,70 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
 import logging
+import os
 
 LOGGER_NAME = "internlm"
 LOGGER_FORMAT = "%(asctime)s\t%(levelname)s %(filename)s:%(lineno)s in %(funcName)s -- %(message)s"
 LOGGER_LEVEL = "info"
 LOGGER_LEVEL_CHOICES = ["debug", "info", "warning", "error", "critical"]
 LOGGER_LEVEL_HELP = (
     "The logging level threshold, choices=['debug', 'info', 'warning', 'error', 'critical'], default='info'"
 )
 
+std_logger = None
 
-def get_logger(logger_name: str = LOGGER_NAME, logging_level: str = LOGGER_LEVEL) -> logging.Logger:
+
+def get_logger(
+    logger_name: str = LOGGER_NAME,
+    logging_level: str = LOGGER_LEVEL,
+    launch_time: str = None,
+    job_name: str = None,
+    file_name: str = None,
+) -> logging.Logger:
     """Configure the logger that is used for uniscale framework.
 
     Args:
         logger_name (str): used to create or get the correspoding logger in
             getLogger call. It will be "internlm" by default.
         logging_level (str, optional): Logging level in string or logging enum.
 
     Returns:
         logger (logging.Logger): the created or modified logger.
 
     """
+    global std_logger
+    if std_logger is not None:
+        return std_logger
 
     logger = logging.getLogger(logger_name)
 
     if logging_level not in LOGGER_LEVEL_CHOICES:
         logging_level = LOGGER_LEVEL
         print(LOGGER_LEVEL_HELP)
 
     logging_level = logging.getLevelName(logging_level.upper())
 
+    # add stream handler
     handler = logging.StreamHandler()
     handler.setLevel(logging_level)
     logger.setLevel(logging_level)
     handler.setFormatter(logging.Formatter(LOGGER_FORMAT))
     logger.addHandler(handler)
 
+    # add file handler
+    if file_name is not None:
+        log_folder = os.path.join("RUN", job_name, launch_time, "logs")
+        log_filepath = os.path.join(log_folder, file_name)
+        try:
+            os.makedirs(log_folder, exist_ok=True)
+        except FileExistsError:
+            pass
+        filehandler = logging.FileHandler(log_filepath)
+        filehandler.setLevel(logging_level)
+        filehandler.setFormatter(logging.Formatter(LOGGER_FORMAT))
+        logger.addHandler(filehandler)
+
+        std_logger = logger
+
     return logger
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/utils/megatron_timers.py` & `InternEvo-0.4.2/internlm/utils/megatron_timers.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/utils/parallel.py` & `InternEvo-0.4.2/internlm/utils/parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     IS_TENSOR_DATA_PARALLEL,
     IS_TENSOR_EXPERT_DATA_PARALLEL,
     IS_TENSOR_ZERO_PARALLEL,
     IS_WEIGHT_ZERO_PARALLEL,
     ParallelMode,
 )
 from internlm.core.context import global_context as gpc
-from internlm.model.utils import try_import_RMSNorm
+from internlm.model.ops.fusion_ops_import_helper import try_import_RMSNorm
 
 RMSNorm = try_import_RMSNorm()
 
 
 def is_using_sequence_parallel():
     return (
         isinstance(gpc.config.parallel["tensor"], dict)
```

### Comparing `InternEvo-0.4.0.dev20240403/internlm/utils/registry.py` & `InternEvo-0.4.2/internlm/utils/registry.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/utils/simple_memory_profiler.py` & `InternEvo-0.4.2/internlm/utils/simple_memory_profiler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/utils/storage_manager.py` & `InternEvo-0.4.2/internlm/utils/storage_manager.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/utils/timeout.py` & `InternEvo-0.4.2/internlm/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/utils/utils.py` & `InternEvo-0.4.2/internlm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/internlm/utils/writer.py` & `InternEvo-0.4.2/internlm/utils/writer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/setup.py` & `InternEvo-0.4.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,30 +4,35 @@
 import subprocess
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
 pwd = os.path.dirname(__file__)
 
 def readme():
-    with open(os.path.join(pwd, 'README.md'), encoding='utf-8') as f:
+    with open(os.path.join(pwd, 'README.md')) as f:
         content = f.read()
     return content
 
 def get_version():
     with open(os.path.join(pwd, 'version.txt'), 'r') as f:
         content = f.read()
     return content
 
+proj_version = get_version()
+
 setup(
     name='InternEvo',
-    version=get_version(),
+    version=proj_version,
     description='an open-sourced lightweight training framework aims to support model pre-training without the need for extensive dependencies',
     long_description=readme(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
+    install_requires=[
+        'rotary_emb=={}'.format(proj_version),
+    ],
 
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Intended Audience :: Developers',
```

### Comparing `InternEvo-0.4.0.dev20240403/tests/common_fixture.py` & `InternEvo-0.4.2/tests/common_fixture.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
             total_steps=10,
             valid_micro_num=4,
             valid_every=300,
             rampup_batch_size=None,
             diag_outlier_ratio=1.1,
             train_folder=None,
             valid_folder=None,
+            num_worker=0,
         ),
         model=dict(
             checkpoint=False,
             num_attention_heads=32,
             embed_split_hidden=True,
             vocab_size=103168,
             embed_grad_scale=1,
```

### Comparing `InternEvo-0.4.0.dev20240403/tests/test_core/test_pipeline.py` & `InternEvo-0.4.2/tests/test_core/test_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,14 @@
         lr_scheduler=dict(
             total_steps=100,
             init_steps=0,
             warmup_ratio=0.01,
             eta_min=1e-5,
             last_epoch=-1,
         ),
-        use_cuda_flash_attn=True,
     )
 )
 
 
 def exam_pipeline_parallel(args):
     # init
     rank, world_size, micro_num, num_chunks, interleaved_overlap = args
```

### Comparing `InternEvo-0.4.0.dev20240403/tests/test_core/utils.py` & `InternEvo-0.4.2/tests/test_core/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/tests/test_training/7B_check_acc.py` & `InternEvo-0.4.2/tests/test_training/7B_check_acc.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/tests/test_training/7B_check_init.py` & `InternEvo-0.4.2/tests/test_training/7B_check_init.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/tests/test_training/test_forward_output_no_fa.py` & `InternEvo-0.4.2/tests/test_training/test_forward_output_no_fa.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,14 @@
         ckpt=dict(
             enable_save_ckpt=False,
             auto_resume=False,
         ),
         loss=dict(
             label_smoothing=0,
         ),
-        use_cuda_flash_attn=True,
     )
 )
 
 
 def find_free_port():
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         s.bind(("", 0))
@@ -124,15 +123,14 @@
 def build_environment(rank, world_size, free_port, config):
     os.environ["RANK"] = str(rank)
     os.environ["LOCAL_RANK"] = str(rank)
     os.environ["WORLD_SIZE"] = str(world_size)
     os.environ["MASTER_ADDR"] = "localhost"
     os.environ["MASTER_PORT"] = str(free_port)
     internlm_accelerator.empty_cache()
-    # launcher="torch"
     internlm.launch_from_torch(config=config, seed=1024)
     args_sanity_check()
 
 
 def seed_all(seed, cuda_deterministic=False):
     random.seed(seed)
     np.random.seed(seed)
```

### Comparing `InternEvo-0.4.0.dev20240403/tests/test_training/test_load_ckpt_loss.py` & `InternEvo-0.4.2/tests/test_training/test_load_ckpt_loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,14 @@
             save_ckpt_folder=f"local:{temp_folder}/",
             auto_resume=False,
             checkpoint_every=5,
         ),
         loss=dict(
             label_smoothing=0,
         ),
-        use_cuda_flash_attn=True,
     )
 )
 
 
 def find_free_port():
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         s.bind(("", 0))
```

### Comparing `InternEvo-0.4.0.dev20240403/tests/test_training/test_loss.py` & `InternEvo-0.4.2/tests/test_training/test_loss.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import math
 import os
 
 import pytest
+import torch
 import torch.distributed as dist
 
 import internlm
 from internlm.checkpoint import CheckpointManager
-from internlm.core.context import ParallelMode
+from internlm.core.context import Config, ParallelMode
 from internlm.core.context import global_context as gpc
 from internlm.core.trainer import TrainState
 from internlm.data import build_train_loader_with_data_type
 from internlm.initialize import initialize_distributed_env
 from internlm.model.losses import FlashGPTLMLoss
 from internlm.model.metrics import AccPerplex
 from internlm.train import (
@@ -21,31 +22,33 @@
     load_new_batch,
 )
 from internlm.utils.common import BatchSkipper, get_current_device, launch_time
 from internlm.utils.gputest import empty_cache_and_diag
 from internlm.utils.megatron_timers import megatron_timer as timer
 
 CONFIG_FILE_PATH = os.getenv("CONFIG_FILE_PATH", "./configs/7B_sft.py")
+INTERNLM1_CKPT_PATH = os.path.join(os.environ["share_path"], "quailty_assurance/test_loss/model_ckpt")
 TOTAL_STEPS = 10
 LOSS_SPIKE_LIMIT = 1.5
-LOSS_DEVIATION_LIMIT = 0.2
+LOSS_DEVIATION_LIMIT = 0.02
 # dp_size = 4
 BASELINE_LOSS_LIST = [
     11.63298511505127,
-    7.826552391052246,
-    6.727715969085693,
-    6.182102680206299,
-    5.395875930786133,
-    5.394404411315918,
-    5.053983688354492,
-    4.741974353790283,
-    4.629222869873047,
-    4.6164231300354,
+    7.82645320892334,
+    6.727725505828857,
+    6.182029724121094,
+    5.395882606506348,
+    5.394383430480957,
+    5.053952217102051,
+    4.742049694061279,
+    4.629276752471924,
+    4.616517543792725,
 ]
 
+
 cur_loss_list = []
 
 
 def train(
     dp_size: int = 1,
     tp_size: int = 1,
     wp_size: int = 1,
@@ -54,15 +57,47 @@
     interleaved: bool = False,
     tp_mode: str = "mtp",
     enable_sp: bool = False,
     enable_ckpt: bool = False,
     model_type: str = "INTERNLM",
 ):
     # initialize distributed environment
-    initialize_distributed_env(config=CONFIG_FILE_PATH)
+    config = Config.from_file(CONFIG_FILE_PATH)
+
+    # init setting
+    config.data.total_steps = TOTAL_STEPS
+    config.data.fixed_random_dataset_seqlen = False
+    config.lr_scheduler.total_steps = TOTAL_STEPS
+    config.model_type = model_type
+    total_steps = config.data.total_steps
+    skip_batches = config.data.skip_batches
+    label_smoothing = config.loss.label_smoothing
+
+    # update ckpt config
+    if model_type == "INTERNLM" and tp_mode != "isp" and interleaved is False:
+        config.ckpt.load_ckpt_info = dict(path=INTERNLM1_CKPT_PATH, content=("model",), ckpt_type="internlm_test")
+        config.ckpt.auto_resume = False
+
+    if enable_ckpt:
+        config.ckpt.enable_save_ckpt = True
+        config.ckpt.checkpoint_every = 10
+        config.ckpt.save_ckpt_folder = "local:llm_ckpts/"
+        config.ckpt.load_ckpt_folder = "local:llm_ckpts/"
+        config.ckpt.load_ckpt_info["content"] = ("all",)
+        config.ckpt.oss_snapshot_freq = 100
+
+    # update parallel config
+    config.parallel.tensor = dict(size=tp_size, mode=tp_mode)
+    config.parallel.pipeline = dict(size=pp_size)
+    config.parallel.weight = dict(size=wp_size, overlap=True, memory_pool=True)
+    if interleaved is True:
+        config.parallel.pipeline = dict(size=pp_size, interleaved_overlap=True)
+        config.model.num_chunks = num_chunks
+
+    initialize_distributed_env(config=config)
     assert hasattr(gpc, "config") and gpc.config is not None
 
     # check parallel config
     assert (
         gpc.get_world_size(ParallelMode.DATA) == dp_size
     ), f"data parallel size: {gpc.get_world_size(ParallelMode.DATA)} is not as expected {dp_size}"
     assert (
@@ -85,32 +120,14 @@
         ), "interleaved overlap must be enabled when using interleave pipeline scheduler"
     if enable_sp:
         assert gpc.config.parallel.get(
             "sequence_parallel", False
         ), "sequence_parallel must be True when enable_sp is True"
     assert gpc.config.parallel["tensor"]["mode"] == tp_mode
 
-    # init setting
-    gpc.config.data.total_steps = TOTAL_STEPS
-    gpc.config.data.fixed_random_dataset_seqlen = False
-    gpc.config.lr_scheduler.total_steps = TOTAL_STEPS
-    gpc.config.model_type = model_type
-    total_steps = gpc.config.data.total_steps
-    skip_batches = gpc.config.data.skip_batches
-    label_smoothing = gpc.config.loss.label_smoothing
-
-    # update ckpt config
-    if enable_ckpt:
-        gpc.config.ckpt.enable_save_ckpt = True
-        gpc.config.ckpt.checkpoint_every = 10
-        gpc.config.ckpt.save_ckpt_folder = "local:llm_ckpts/"
-        gpc.config.ckpt.load_ckpt_folder = "local:llm_ckpts/"
-        gpc.config.ckpt.load_ckpt_info["content"] = ("all",)
-        gpc.config.ckpt.oss_snapshot_freq = 100
-
     # get and broadcast current time
     current_time = launch_time()
     objs = [current_time]
     dist.broadcast_object_list(objs, src=0)
     current_time = objs[0]
 
     # initialize model
@@ -166,24 +183,32 @@
     )
 
     # initialize the batch skipper
     batch_skipper = BatchSkipper(skip_batches)
 
     trainer.train()
 
-    # transfer the train data loader into train data iterator
     train_iter = iter(train_dl)
 
+    if model_type == "INTERNLM":
+        data_path = os.path.join(os.environ["share_path"], "quailty_assurance/test_loss/data_batch_4DP")
+        data_batch = torch.load(f"{data_path}/{gpc.get_local_rank(ParallelMode.DATA)}_data_batch.pt")
+
     # start iterating the train data and begin training
     for batch_count in range(train_state.batch_count, total_steps):
         empty_cache_and_diag(batch_count, interval=gpc.config.data.empty_cache_and_diag_interval)
         timer("one-batch").start()
 
-        # load batch data
-        batch, train_iter = load_new_batch(train_dl=train_dl, train_iter=train_iter, train_state=train_state)
+        if model_type == "INTERNLM":
+            if batch_count >= 10:
+                batch = data_batch[batch_count - 10]
+            else:
+                batch = data_batch[batch_count]
+        else:
+            batch, train_iter = load_new_batch(train_dl=train_dl, train_iter=train_iter, train_state=train_state)
 
         # record the consumed samples in training
         train_state.batch_count = batch_count
         train_state.num_consumed_samples_in_epoch += len(batch[1])
         if batch_skipper(batch_count):  # skip this batch
             if gpc.is_rank_for_log():
                 print(f"Skip batch count:`{batch_count}`...")
@@ -309,15 +334,14 @@
     # model training
     train(dp_size=4, pp_size=2, interleaved=True)
 
     # print loss value
     print(f"cur_loss_list: {cur_loss_list}", flush=True)
 
     check_loss_spike()
-    check_loss_accuracy()
 
 
 @pytest.mark.training_16GPU_4DP2TP2PP_MTP
 def test_training_loss_with_dp4_tp2_pp2_mtp():
     # model training
     train(dp_size=4, tp_size=2, pp_size=2)
 
@@ -351,20 +375,37 @@
     check_loss_spike()
     check_loss_accuracy()
 
 
 @pytest.mark.training_8GPU_ISP
 def test_training_with_isp():
     # update config file
-    global CONFIG_FILE_PATH
+    global CONFIG_FILE_PATH, BASELINE_LOSS_LIST
     CONFIG_FILE_PATH = "./configs/7B_isp_sft.py"
-
+    BASELINE_LOSS_LIST = [
+        11.594964981079102,
+        8.874114990234375,
+        7.090242385864258,
+        6.782063961029053,
+        5.961512088775635,
+        5.606202125549316,
+        5.305666446685791,
+        5.0156569480896,
+        4.9411516189575195,
+        4.983800411224365,
+    ]
     # model training
     train(dp_size=4, tp_size=2, wp_size=4, tp_mode="isp", enable_sp=True)
 
+    # print loss value
+    print(f"cur_loss_list: {cur_loss_list}", flush=True)
+
+    check_loss_spike()
+    check_loss_accuracy()
+
 
 @pytest.mark.training_8GPU_ISP_SAVE_CKPT
 def test_training_with_isp_save_ckpt():
     # update config file
     global CONFIG_FILE_PATH
     CONFIG_FILE_PATH = "./configs/7B_isp_sft.py"
```

### Comparing `InternEvo-0.4.0.dev20240403/tests/test_training/test_no_fa_train_temp.py` & `InternEvo-0.4.2/tests/test_training/test_no_fa_train_temp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.0.dev20240403/tests/test_training/test_norm_weight.py` & `InternEvo-0.4.2/tests/test_training/test_norm_weight.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,14 +102,16 @@
 
     # transfer the train data loader into train data iterator
     trainer.train()
 
     train_iter = iter(train_dl)
 
     for batch_count in range(total_steps):
+        if gpc.is_rank_for_log() and batch_count % 100 == 0:
+            print(f"batch_count: {batch_count}", flush=True)
         if batch_count % 100 == 0:
             internlm_accelerator.empty_cache()
             gc.collect()
 
         # load batch data
         batch, train_iter = load_new_batch(train_dl=train_dl, train_iter=train_iter)
 
@@ -176,14 +178,15 @@
             train_check_norm_weight,
             [[rank, 8, free_port, "msp"] for rank in range(8)],
         )
         pool.close()
         pool.join()
 
     check_result(result)
+    print("msp check pass", flush=True)
 
 
 @pytest.mark.check_norm_fsp
 def test_check_norm_fsp():
     free_port = find_free_port()
     ctx = mp.get_context("spawn")
     with ctx.Pool(processes=8) as pool:
@@ -191,14 +194,15 @@
             train_check_norm_weight,
             [[rank, 8, free_port, "fsp"] for rank in range(8)],
         )
         pool.close()
         pool.join()
 
     check_result(result)
+    print("fsp check pass", flush=True)
 
 
 @pytest.mark.check_norm_isp
 def test_check_norm_isp():
     free_port = find_free_port()
     ctx = mp.get_context("spawn")
     with ctx.Pool(processes=8) as pool:
@@ -206,7 +210,8 @@
             train_check_norm_weight,
             [[rank, 8, free_port, "isp"] for rank in range(8)],
         )
         pool.close()
         pool.join()
 
     check_result(result)
+    print("isp check pass", flush=True)
```

### Comparing `InternEvo-0.4.0.dev20240403/tests/test_training/test_swap_nb_loss_and_gradnorm.py` & `InternEvo-0.4.2/tests/test_training/test_swap_nb_loss_and_gradnorm.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,14 @@
             enable_save_ckpt=False,
             auto_resume=False,
         ),
         loss=dict(
             label_smoothing=0,
         ),
         cudnn_deterministic=True,
-        use_cuda_flash_attn=True,
     )
 )
 
 
 def build_environment(rank, world_size, config):
     os.environ["RANK"] = str(rank)
     os.environ["LOCAL_RANK"] = str(rank)
```

### Comparing `InternEvo-0.4.0.dev20240403/tests/test_training/train_CI.py` & `InternEvo-0.4.2/tests/test_training/train_CI.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,28 +299,26 @@
                 beta2_scheduler=beta2_scheduler,
                 trainer=trainer,
                 start_time=start_time,
                 loss=loss,
                 moe_loss=moe_loss,
                 grad_norm=grad_norm_groups,
                 metric=metric,
-                update_panel=False,
             )
 
             timer("one-batch").stop()
 
             # evaluate on validation data loaders
             if valid_every > 0 and train_state.step_count % valid_every == 0:
                 evaluate_on_val_dls(
                     trainer=trainer,
                     val_dls=val_dls,
                     writer=writer,
                     logger=logger,
                     step_count=train_state.step_count,
-                    update_panel=False,
                 )
 
             # check model weights
             if gpc.is_rank_for_log() and batch_count > 0 and batch_count % 100 == 0:
                 ckpt_path = os.path.join(
                     os.environ["share_path"],
                     "quailty_assurance/7B_model_weights_ckpt",
@@ -354,14 +352,18 @@
 
     # initialize monitor manager context
     with initialize_monitor_manager(
         job_name=gpc.config.JOB_NAME, alert_address=gpc.config.monitor.alert.feishu_alert_address
     ):
         try:
             main(args)
+        except AssertionError as e:
+            logger.error(e)
+            sys.exit(1)
         except Exception:
             logger.error(
                 f"Raise exception from {hostname} with rank id: {gpc.get_global_rank()}\n{traceback.format_exc()}",
             )
             mm.monitor_exception(
                 alert_address=gpc.config.monitor.alert.feishu_alert_address, excp_info=traceback.format_exc()
             )
+            sys.exit(1)
```

