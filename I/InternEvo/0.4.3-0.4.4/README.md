# Comparing `tmp/InternEvo-0.4.3.tar.gz` & `tmp/InternEvo-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InternEvo-0.4.3.tar", last modified: Mon May  6 08:04:29 2024, max compression
+gzip compressed data, was "InternEvo-0.4.4.tar", last modified: Mon May  6 08:23:23 2024, max compression
```

## Comparing `InternEvo-0.4.3.tar` & `InternEvo-0.4.4.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:33.109109 InternEvo-0.4.3/
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.125640 InternEvo-0.4.3/InternEvo.egg-info/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5320 2024-05-06 08:04:28.000000 InternEvo-0.4.3/InternEvo.egg-info/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4662 2024-05-06 08:04:28.000000 InternEvo-0.4.3/InternEvo.egg-info/SOURCES.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-06 08:04:28.000000 InternEvo-0.4.3/InternEvo.egg-info/dependency_links.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       18 2024-05-06 08:04:28.000000 InternEvo-0.4.3/InternEvo.egg-info/requires.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       15 2024-05-06 08:04:28.000000 InternEvo-0.4.3/InternEvo.egg-info/top_level.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13656 2024-01-25 08:28:54.000000 InternEvo-0.4.3/LICENSE
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5320 2024-05-06 08:04:29.955825 InternEvo-0.4.3/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4730 2024-01-25 08:28:54.000000 InternEvo-0.4.3/README.md
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.132095 InternEvo-0.4.3/internlm/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      267 2024-01-30 08:18:31.000000 InternEvo-0.4.3/internlm/__init__.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.176155 InternEvo-0.4.3/internlm/accelerator/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      147 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/accelerator/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4017 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/accelerator/abstract_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11010 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/accelerator/cuda_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11446 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/accelerator/dipu_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10866 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/accelerator/npu_accelerator.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.194082 InternEvo-0.4.3/internlm/apis/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.3/internlm/apis/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    37532 2024-01-25 08:28:55.000000 InternEvo-0.4.3/internlm/apis/inference.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.235285 InternEvo-0.4.3/internlm/checkpoint/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       83 2024-03-15 18:58:58.000000 InternEvo-0.4.3/internlm/checkpoint/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27404 2024-04-17 07:54:31.000000 InternEvo-0.4.3/internlm/checkpoint/checkpoint_manager.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20076 2024-04-12 05:43:59.000000 InternEvo-0.4.3/internlm/checkpoint/components.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14174 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/checkpoint/load_funcs.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2474 2024-04-10 07:31:30.000000 InternEvo-0.4.3/internlm/checkpoint/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.271046 InternEvo-0.4.3/internlm/core/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      158 2024-01-25 08:28:55.000000 InternEvo-0.4.3/internlm/core/__init__.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.307060 InternEvo-0.4.3/internlm/core/communication/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      884 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/core/communication/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    23944 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/core/communication/isp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22670 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/core/communication/p2p.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10118 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/core/communication/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.340270 InternEvo-0.4.3/internlm/core/context/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1220 2024-03-18 08:30:10.000000 InternEvo-0.4.3/internlm/core/context/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27076 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/core/context/parallel_context.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    38371 2024-03-18 08:30:10.000000 InternEvo-0.4.3/internlm/core/context/process_group_initializer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4295 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/core/context/random.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7458 2024-03-15 18:58:58.000000 InternEvo-0.4.3/internlm/core/engine.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3113 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/core/gradient_handler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8195 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/core/naive_amp.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.370036 InternEvo-0.4.3/internlm/core/scheduler/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      303 2024-02-08 03:13:39.000000 InternEvo-0.4.3/internlm/core/scheduler/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5258 2024-03-22 07:04:00.000000 InternEvo-0.4.3/internlm/core/scheduler/base_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9071 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/core/scheduler/no_pipeline_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    64105 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/core/scheduler/pipeline_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7598 2024-04-19 04:15:42.000000 InternEvo-0.4.3/internlm/core/trainer.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.398847 InternEvo-0.4.3/internlm/data/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      209 2024-03-15 18:58:58.000000 InternEvo-0.4.3/internlm/data/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6991 2024-04-11 07:14:24.000000 InternEvo-0.4.3/internlm/data/build_dataloader.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.459101 InternEvo-0.4.3/internlm/data/tokenized/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      418 2024-03-22 07:04:00.000000 InternEvo-0.4.3/internlm/data/tokenized/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15158 2024-03-15 18:58:58.000000 InternEvo-0.4.3/internlm/data/tokenized/batch_sampler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4401 2024-04-10 08:53:30.000000 InternEvo-0.4.3/internlm/data/tokenized/collaters.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1714 2024-03-15 18:58:58.000000 InternEvo-0.4.3/internlm/data/tokenized/dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1406 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/data/tokenized/dummy_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1894 2024-04-10 08:53:30.000000 InternEvo-0.4.3/internlm/data/tokenized/dummy_dataset_multimodal.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22498 2024-04-10 13:25:54.000000 InternEvo-0.4.3/internlm/data/tokenized/packed_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3740 2024-03-15 18:58:58.000000 InternEvo-0.4.3/internlm/data/tokenized/single_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      454 2024-03-15 18:58:58.000000 InternEvo-0.4.3/internlm/data/train_state.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1919 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/data/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.473429 InternEvo-0.4.3/internlm/eval/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       86 2024-03-15 18:58:58.000000 InternEvo-0.4.3/internlm/eval/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4999 2024-04-11 02:31:26.000000 InternEvo-0.4.3/internlm/eval/evaluation.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.503218 InternEvo-0.4.3/internlm/initialize/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      368 2024-01-25 08:28:55.000000 InternEvo-0.4.3/internlm/initialize/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1793 2024-01-25 08:28:55.000000 InternEvo-0.4.3/internlm/initialize/initialize_tensor.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5922 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/initialize/initialize_trainer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27458 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/initialize/launch.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.516774 InternEvo-0.4.3/internlm/initialize/legacy/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.3/internlm/initialize/legacy/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1592 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/initialize/legacy/launch.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.570545 InternEvo-0.4.3/internlm/model/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1124 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/__init__.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.597459 InternEvo-0.4.3/internlm/model/llava_modules/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-03 18:56:44.000000 InternEvo-0.4.3/internlm/model/llava_modules/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      499 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/llava_modules/clip_builder.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2674 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/llava_modules/clip_encoder.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1407 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/llava_modules/projector_builder.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.614103 InternEvo-0.4.3/internlm/model/losses/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       73 2024-03-15 18:58:58.000000 InternEvo-0.4.3/internlm/model/losses/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1786 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/losses/ce_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16344 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/metrics.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    23422 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/modeling_internlm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    54060 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/modeling_internlm2.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    51790 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/modeling_llama.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20872 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/modeling_llava.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    25417 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/modeling_moe.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.640973 InternEvo-0.4.3/internlm/model/modules/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.4.3/internlm/model/modules/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20370 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/modules/embedding.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10093 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/modules/mlp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    40600 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/modules/multi_head_attention.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.683858 InternEvo-0.4.3/internlm/model/moe/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      678 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/moe/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1198 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/model/moe/base_layer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2762 2024-03-18 08:30:10.000000 InternEvo-0.4.3/internlm/model/moe/experts.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20490 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/moe/gshard_layer.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.720509 InternEvo-0.4.3/internlm/model/moe/megablock/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-17 08:44:20.000000 InternEvo-0.4.3/internlm/model/moe/megablock/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8705 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/moe/megablock/megablock_dmoe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13643 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/moe/megablock/megablock_moe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2555 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/moe/megablock/mlp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11986 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/moe/megablock/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4494 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/moe/moe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2021 2024-03-18 08:30:10.000000 InternEvo-0.4.3/internlm/model/moe/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.752271 InternEvo-0.4.3/internlm/model/ops/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.4.3/internlm/model/ops/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6316 2024-05-06 07:30:03.000000 InternEvo-0.4.3/internlm/model/ops/fusion_ops_import_helper.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16010 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/ops/linear.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1500 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/model/ops/norm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24931 2024-05-06 07:30:03.000000 InternEvo-0.4.3/internlm/model/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.784429 InternEvo-0.4.3/internlm/monitor/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      193 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/monitor/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1479 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/monitor/alert.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10213 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/monitor/monitor.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      776 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/monitor/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.810732 InternEvo-0.4.3/internlm/solver/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-15 18:58:59.000000 InternEvo-0.4.3/internlm/solver/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10095 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/solver/activation_checkpoint.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.856972 InternEvo-0.4.3/internlm/solver/optimizer/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-22 07:04:01.000000 InternEvo-0.4.3/internlm/solver/optimizer/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1080 2024-01-25 08:28:55.000000 InternEvo-0.4.3/internlm/solver/optimizer/base_optimizer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9173 2024-03-22 08:39:35.000000 InternEvo-0.4.3/internlm/solver/optimizer/fsdp_optimizer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    42555 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/solver/optimizer/hybrid_zero_optim.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10132 2024-03-22 08:39:35.000000 InternEvo-0.4.3/internlm/solver/optimizer/store.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20351 2024-04-08 13:12:08.000000 InternEvo-0.4.3/internlm/solver/optimizer/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1280 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/solver/pipeline_utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.879351 InternEvo-0.4.3/internlm/solver/schedulers/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      272 2024-03-15 18:58:59.000000 InternEvo-0.4.3/internlm/solver/schedulers/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      844 2024-03-26 03:26:29.000000 InternEvo-0.4.3/internlm/solver/schedulers/beta2_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5940 2024-03-15 18:58:59.000000 InternEvo-0.4.3/internlm/solver/schedulers/lr_scheduler.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.906571 InternEvo-0.4.3/internlm/train/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      591 2024-05-06 07:30:03.000000 InternEvo-0.4.3/internlm/train/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22392 2024-05-06 07:30:03.000000 InternEvo-0.4.3/internlm/train/pipeline.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3567 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/train/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:32.987562 InternEvo-0.4.3/internlm/utils/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.3/internlm/utils/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9244 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/utils/common.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6321 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/utils/gputest.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2112 2024-04-10 11:16:15.000000 InternEvo-0.4.3/internlm/utils/logger.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4156 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/utils/megatron_timers.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4061 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/utils/parallel.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2423 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/utils/registry.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24734 2024-03-26 03:26:29.000000 InternEvo-0.4.3/internlm/utils/simple_memory_profiler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    46133 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/utils/storage_manager.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3126 2024-03-15 18:58:59.000000 InternEvo-0.4.3/internlm/utils/timeout.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      709 2024-05-03 18:58:40.000000 InternEvo-0.4.3/internlm/utils/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7117 2024-04-07 02:41:24.000000 InternEvo-0.4.3/internlm/utils/writer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-06 08:04:29.959120 InternEvo-0.4.3/setup.cfg
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1191 2024-05-06 07:30:03.000000 InternEvo-0.4.3/setup.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:33.000269 InternEvo-0.4.3/tests/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.3/tests/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4536 2024-05-03 18:58:40.000000 InternEvo-0.4.3/tests/common_fixture.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:33.022191 InternEvo-0.4.3/tests/test_core/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.3/tests/test_core/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5841 2024-04-24 06:39:45.000000 InternEvo-0.4.3/tests/test_core/test_pipeline.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6978 2024-05-03 18:58:40.000000 InternEvo-0.4.3/tests/test_core/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:02:33.098659 InternEvo-0.4.3/tests/test_training/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5750 2024-04-12 05:43:59.000000 InternEvo-0.4.3/tests/test_training/7B_check_acc.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6360 2024-04-07 02:41:25.000000 InternEvo-0.4.3/tests/test_training/7B_check_init.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:46.000000 InternEvo-0.4.3/tests/test_training/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7882 2024-05-03 18:58:40.000000 InternEvo-0.4.3/tests/test_training/test_forward_output_no_fa.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11700 2024-05-03 18:58:40.000000 InternEvo-0.4.3/tests/test_training/test_load_ckpt_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14416 2024-05-03 18:58:40.000000 InternEvo-0.4.3/tests/test_training/test_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3845 2024-05-03 18:58:40.000000 InternEvo-0.4.3/tests/test_training/test_no_fa_train_temp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6763 2024-05-03 18:58:40.000000 InternEvo-0.4.3/tests/test_training/test_norm_weight.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12557 2024-05-03 18:58:40.000000 InternEvo-0.4.3/tests/test_training/test_swap_nb_loss_and_gradnorm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14000 2024-05-03 18:58:40.000000 InternEvo-0.4.3/tests/test_training/train_CI.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.589209 InternEvo-0.4.4/
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:25.715380 InternEvo-0.4.4/InternEvo.egg-info/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5320 2024-05-06 08:23:21.000000 InternEvo-0.4.4/InternEvo.egg-info/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4662 2024-05-06 08:23:22.000000 InternEvo-0.4.4/InternEvo.egg-info/SOURCES.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-06 08:23:21.000000 InternEvo-0.4.4/InternEvo.egg-info/dependency_links.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       18 2024-05-06 08:23:21.000000 InternEvo-0.4.4/InternEvo.egg-info/requires.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       15 2024-05-06 08:23:21.000000 InternEvo-0.4.4/InternEvo.egg-info/top_level.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13656 2024-01-25 08:28:54.000000 InternEvo-0.4.4/LICENSE
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5320 2024-05-06 08:23:23.437394 InternEvo-0.4.4/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4730 2024-01-25 08:28:54.000000 InternEvo-0.4.4/README.md
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:25.722330 InternEvo-0.4.4/internlm/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      267 2024-01-30 08:18:31.000000 InternEvo-0.4.4/internlm/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:25.755612 InternEvo-0.4.4/internlm/accelerator/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      147 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/accelerator/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4017 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/accelerator/abstract_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11010 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/accelerator/cuda_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11446 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/accelerator/dipu_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10866 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/accelerator/npu_accelerator.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:25.772519 InternEvo-0.4.4/internlm/apis/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.4/internlm/apis/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    37532 2024-01-25 08:28:55.000000 InternEvo-0.4.4/internlm/apis/inference.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:25.810208 InternEvo-0.4.4/internlm/checkpoint/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       83 2024-03-15 18:58:58.000000 InternEvo-0.4.4/internlm/checkpoint/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27404 2024-04-17 07:54:31.000000 InternEvo-0.4.4/internlm/checkpoint/checkpoint_manager.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20076 2024-04-12 05:43:59.000000 InternEvo-0.4.4/internlm/checkpoint/components.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14174 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/checkpoint/load_funcs.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2474 2024-04-10 07:31:30.000000 InternEvo-0.4.4/internlm/checkpoint/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:25.842758 InternEvo-0.4.4/internlm/core/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      158 2024-01-25 08:28:55.000000 InternEvo-0.4.4/internlm/core/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:25.870844 InternEvo-0.4.4/internlm/core/communication/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      884 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/core/communication/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    23944 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/core/communication/isp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22670 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/core/communication/p2p.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10118 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/core/communication/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:25.898867 InternEvo-0.4.4/internlm/core/context/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1220 2024-03-18 08:30:10.000000 InternEvo-0.4.4/internlm/core/context/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27076 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/core/context/parallel_context.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    38371 2024-03-18 08:30:10.000000 InternEvo-0.4.4/internlm/core/context/process_group_initializer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4295 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/core/context/random.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7458 2024-03-15 18:58:58.000000 InternEvo-0.4.4/internlm/core/engine.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3113 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/core/gradient_handler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8195 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/core/naive_amp.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:25.932162 InternEvo-0.4.4/internlm/core/scheduler/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      303 2024-02-08 03:13:39.000000 InternEvo-0.4.4/internlm/core/scheduler/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5258 2024-03-22 07:04:00.000000 InternEvo-0.4.4/internlm/core/scheduler/base_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9071 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/core/scheduler/no_pipeline_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    64105 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/core/scheduler/pipeline_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7598 2024-04-19 04:15:42.000000 InternEvo-0.4.4/internlm/core/trainer.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:25.957204 InternEvo-0.4.4/internlm/data/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      209 2024-03-15 18:58:58.000000 InternEvo-0.4.4/internlm/data/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6991 2024-04-11 07:14:24.000000 InternEvo-0.4.4/internlm/data/build_dataloader.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.011986 InternEvo-0.4.4/internlm/data/tokenized/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      418 2024-03-22 07:04:00.000000 InternEvo-0.4.4/internlm/data/tokenized/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15158 2024-03-15 18:58:58.000000 InternEvo-0.4.4/internlm/data/tokenized/batch_sampler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4401 2024-04-10 08:53:30.000000 InternEvo-0.4.4/internlm/data/tokenized/collaters.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1714 2024-03-15 18:58:58.000000 InternEvo-0.4.4/internlm/data/tokenized/dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1406 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/data/tokenized/dummy_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1894 2024-04-10 08:53:30.000000 InternEvo-0.4.4/internlm/data/tokenized/dummy_dataset_multimodal.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22498 2024-04-10 13:25:54.000000 InternEvo-0.4.4/internlm/data/tokenized/packed_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3740 2024-03-15 18:58:58.000000 InternEvo-0.4.4/internlm/data/tokenized/single_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      454 2024-03-15 18:58:58.000000 InternEvo-0.4.4/internlm/data/train_state.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1919 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/data/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.027644 InternEvo-0.4.4/internlm/eval/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       86 2024-03-15 18:58:58.000000 InternEvo-0.4.4/internlm/eval/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4999 2024-04-11 02:31:26.000000 InternEvo-0.4.4/internlm/eval/evaluation.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.057247 InternEvo-0.4.4/internlm/initialize/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      368 2024-01-25 08:28:55.000000 InternEvo-0.4.4/internlm/initialize/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1793 2024-01-25 08:28:55.000000 InternEvo-0.4.4/internlm/initialize/initialize_tensor.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5922 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/initialize/initialize_trainer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27458 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/initialize/launch.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.074777 InternEvo-0.4.4/internlm/initialize/legacy/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.4/internlm/initialize/legacy/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1592 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/initialize/legacy/launch.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.122849 InternEvo-0.4.4/internlm/model/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1124 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.147786 InternEvo-0.4.4/internlm/model/llava_modules/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-03 18:56:44.000000 InternEvo-0.4.4/internlm/model/llava_modules/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      499 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/llava_modules/clip_builder.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2674 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/llava_modules/clip_encoder.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1407 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/llava_modules/projector_builder.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.162849 InternEvo-0.4.4/internlm/model/losses/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       73 2024-03-15 18:58:58.000000 InternEvo-0.4.4/internlm/model/losses/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1786 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/losses/ce_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16344 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/metrics.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    23422 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/modeling_internlm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    54060 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/modeling_internlm2.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    51790 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/modeling_llama.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20872 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/modeling_llava.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    25417 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/modeling_moe.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.188413 InternEvo-0.4.4/internlm/model/modules/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.4.4/internlm/model/modules/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20370 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/modules/embedding.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10093 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/modules/mlp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    40600 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/modules/multi_head_attention.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.225857 InternEvo-0.4.4/internlm/model/moe/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      678 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/moe/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1198 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/model/moe/base_layer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2762 2024-03-18 08:30:10.000000 InternEvo-0.4.4/internlm/model/moe/experts.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20490 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/moe/gshard_layer.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.259199 InternEvo-0.4.4/internlm/model/moe/megablock/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-17 08:44:20.000000 InternEvo-0.4.4/internlm/model/moe/megablock/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8705 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/moe/megablock/megablock_dmoe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13643 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/moe/megablock/megablock_moe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2555 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/moe/megablock/mlp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11986 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/moe/megablock/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4494 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/moe/moe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2021 2024-03-18 08:30:10.000000 InternEvo-0.4.4/internlm/model/moe/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.284613 InternEvo-0.4.4/internlm/model/ops/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.4.4/internlm/model/ops/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6316 2024-05-06 07:30:03.000000 InternEvo-0.4.4/internlm/model/ops/fusion_ops_import_helper.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16010 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/ops/linear.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1500 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/model/ops/norm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24931 2024-05-06 07:30:03.000000 InternEvo-0.4.4/internlm/model/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.309168 InternEvo-0.4.4/internlm/monitor/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      193 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/monitor/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1479 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/monitor/alert.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10213 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/monitor/monitor.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      776 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/monitor/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.327421 InternEvo-0.4.4/internlm/solver/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-15 18:58:59.000000 InternEvo-0.4.4/internlm/solver/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10095 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/solver/activation_checkpoint.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.366221 InternEvo-0.4.4/internlm/solver/optimizer/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-22 07:04:01.000000 InternEvo-0.4.4/internlm/solver/optimizer/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1080 2024-01-25 08:28:55.000000 InternEvo-0.4.4/internlm/solver/optimizer/base_optimizer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9173 2024-03-22 08:39:35.000000 InternEvo-0.4.4/internlm/solver/optimizer/fsdp_optimizer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    42555 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/solver/optimizer/hybrid_zero_optim.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10132 2024-03-22 08:39:35.000000 InternEvo-0.4.4/internlm/solver/optimizer/store.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20351 2024-04-08 13:12:08.000000 InternEvo-0.4.4/internlm/solver/optimizer/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1280 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/solver/pipeline_utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.388893 InternEvo-0.4.4/internlm/solver/schedulers/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      272 2024-03-15 18:58:59.000000 InternEvo-0.4.4/internlm/solver/schedulers/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      844 2024-03-26 03:26:29.000000 InternEvo-0.4.4/internlm/solver/schedulers/beta2_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5940 2024-03-15 18:58:59.000000 InternEvo-0.4.4/internlm/solver/schedulers/lr_scheduler.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.408388 InternEvo-0.4.4/internlm/train/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      591 2024-05-06 07:30:03.000000 InternEvo-0.4.4/internlm/train/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22392 2024-05-06 07:30:03.000000 InternEvo-0.4.4/internlm/train/pipeline.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3567 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/train/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.487622 InternEvo-0.4.4/internlm/utils/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.4/internlm/utils/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9244 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/utils/common.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6321 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/utils/gputest.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2112 2024-04-10 11:16:15.000000 InternEvo-0.4.4/internlm/utils/logger.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4156 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/utils/megatron_timers.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4061 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/utils/parallel.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2423 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/utils/registry.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24734 2024-03-26 03:26:29.000000 InternEvo-0.4.4/internlm/utils/simple_memory_profiler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    46133 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/utils/storage_manager.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3126 2024-03-15 18:58:59.000000 InternEvo-0.4.4/internlm/utils/timeout.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      709 2024-05-03 18:58:40.000000 InternEvo-0.4.4/internlm/utils/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7117 2024-04-07 02:41:24.000000 InternEvo-0.4.4/internlm/utils/writer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-06 08:23:23.440800 InternEvo-0.4.4/setup.cfg
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1191 2024-05-06 07:30:03.000000 InternEvo-0.4.4/setup.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.498592 InternEvo-0.4.4/tests/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.4/tests/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4536 2024-05-03 18:58:40.000000 InternEvo-0.4.4/tests/common_fixture.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.518568 InternEvo-0.4.4/tests/test_core/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.4.4/tests/test_core/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5841 2024-04-24 06:39:45.000000 InternEvo-0.4.4/tests/test_core/test_pipeline.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6978 2024-05-03 18:58:40.000000 InternEvo-0.4.4/tests/test_core/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-06 08:21:26.580191 InternEvo-0.4.4/tests/test_training/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5750 2024-04-12 05:43:59.000000 InternEvo-0.4.4/tests/test_training/7B_check_acc.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6360 2024-04-07 02:41:25.000000 InternEvo-0.4.4/tests/test_training/7B_check_init.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:46.000000 InternEvo-0.4.4/tests/test_training/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7882 2024-05-03 18:58:40.000000 InternEvo-0.4.4/tests/test_training/test_forward_output_no_fa.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11700 2024-05-03 18:58:40.000000 InternEvo-0.4.4/tests/test_training/test_load_ckpt_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14416 2024-05-03 18:58:40.000000 InternEvo-0.4.4/tests/test_training/test_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3845 2024-05-03 18:58:40.000000 InternEvo-0.4.4/tests/test_training/test_no_fa_train_temp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6763 2024-05-03 18:58:40.000000 InternEvo-0.4.4/tests/test_training/test_norm_weight.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12557 2024-05-03 18:58:40.000000 InternEvo-0.4.4/tests/test_training/test_swap_nb_loss_and_gradnorm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14000 2024-05-03 18:58:40.000000 InternEvo-0.4.4/tests/test_training/train_CI.py
```

### Comparing `InternEvo-0.4.3/InternEvo.egg-info/PKG-INFO` & `InternEvo-0.4.4/InternEvo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternEvo
-Version: 0.4.3
+Version: 0.4.4
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
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: InternEvo Version: 0.4.3 Summary: an open-sourced
+Metadata-Version: 2.1 Name: InternEvo Version: 0.4.4 Summary: an open-sourced
 lightweight training framework aims to support model pre-training without the
 need for extensive dependencies Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Description-
 Content-Type: text/markdown License-File: LICENSE # InternEvo
```

### Comparing `InternEvo-0.4.3/InternEvo.egg-info/SOURCES.txt` & `InternEvo-0.4.4/InternEvo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/LICENSE` & `InternEvo-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/PKG-INFO` & `InternEvo-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternEvo
-Version: 0.4.3
+Version: 0.4.4
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
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: InternEvo Version: 0.4.3 Summary: an open-sourced
+Metadata-Version: 2.1 Name: InternEvo Version: 0.4.4 Summary: an open-sourced
 lightweight training framework aims to support model pre-training without the
 need for extensive dependencies Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Description-
 Content-Type: text/markdown License-File: LICENSE # InternEvo
```

### Comparing `InternEvo-0.4.3/README.md` & `InternEvo-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/accelerator/abstract_accelerator.py` & `InternEvo-0.4.4/internlm/accelerator/abstract_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/accelerator/cuda_accelerator.py` & `InternEvo-0.4.4/internlm/accelerator/cuda_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/accelerator/dipu_accelerator.py` & `InternEvo-0.4.4/internlm/accelerator/dipu_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/accelerator/npu_accelerator.py` & `InternEvo-0.4.4/internlm/accelerator/npu_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/apis/inference.py` & `InternEvo-0.4.4/internlm/apis/inference.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/checkpoint/checkpoint_manager.py` & `InternEvo-0.4.4/internlm/checkpoint/checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/checkpoint/components.py` & `InternEvo-0.4.4/internlm/checkpoint/components.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/checkpoint/load_funcs.py` & `InternEvo-0.4.4/internlm/checkpoint/load_funcs.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/checkpoint/utils.py` & `InternEvo-0.4.4/internlm/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/core/communication/__init__.py` & `InternEvo-0.4.4/internlm/core/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/core/communication/isp.py` & `InternEvo-0.4.4/internlm/core/communication/isp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/core/communication/p2p.py` & `InternEvo-0.4.4/internlm/core/communication/p2p.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/core/communication/utils.py` & `InternEvo-0.4.4/internlm/core/communication/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/core/context/__init__.py` & `InternEvo-0.4.4/internlm/core/context/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/core/context/parallel_context.py` & `InternEvo-0.4.4/internlm/core/context/parallel_context.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/core/context/process_group_initializer.py` & `InternEvo-0.4.4/internlm/core/context/process_group_initializer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/core/context/random.py` & `InternEvo-0.4.4/internlm/core/context/random.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/core/engine.py` & `InternEvo-0.4.4/internlm/core/engine.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/core/gradient_handler.py` & `InternEvo-0.4.4/internlm/core/gradient_handler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/core/naive_amp.py` & `InternEvo-0.4.4/internlm/core/naive_amp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/core/scheduler/base_scheduler.py` & `InternEvo-0.4.4/internlm/core/scheduler/base_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/core/scheduler/no_pipeline_scheduler.py` & `InternEvo-0.4.4/internlm/core/scheduler/no_pipeline_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/core/scheduler/pipeline_scheduler.py` & `InternEvo-0.4.4/internlm/core/scheduler/pipeline_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/core/trainer.py` & `InternEvo-0.4.4/internlm/core/trainer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/data/build_dataloader.py` & `InternEvo-0.4.4/internlm/data/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/data/tokenized/batch_sampler.py` & `InternEvo-0.4.4/internlm/data/tokenized/batch_sampler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/data/tokenized/collaters.py` & `InternEvo-0.4.4/internlm/data/tokenized/collaters.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/data/tokenized/dataset.py` & `InternEvo-0.4.4/internlm/data/tokenized/dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/data/tokenized/dummy_dataset.py` & `InternEvo-0.4.4/internlm/data/tokenized/dummy_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/data/tokenized/dummy_dataset_multimodal.py` & `InternEvo-0.4.4/internlm/data/tokenized/dummy_dataset_multimodal.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/data/tokenized/packed_dataset.py` & `InternEvo-0.4.4/internlm/data/tokenized/packed_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/data/tokenized/single_dataset.py` & `InternEvo-0.4.4/internlm/data/tokenized/single_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/data/utils.py` & `InternEvo-0.4.4/internlm/data/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/eval/evaluation.py` & `InternEvo-0.4.4/internlm/eval/evaluation.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/initialize/initialize_tensor.py` & `InternEvo-0.4.4/internlm/initialize/initialize_tensor.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/initialize/initialize_trainer.py` & `InternEvo-0.4.4/internlm/initialize/initialize_trainer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/initialize/launch.py` & `InternEvo-0.4.4/internlm/initialize/launch.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/initialize/legacy/launch.py` & `InternEvo-0.4.4/internlm/initialize/legacy/launch.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/__init__.py` & `InternEvo-0.4.4/internlm/model/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/llava_modules/clip_encoder.py` & `InternEvo-0.4.4/internlm/model/llava_modules/clip_encoder.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/llava_modules/projector_builder.py` & `InternEvo-0.4.4/internlm/model/llava_modules/projector_builder.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/losses/ce_loss.py` & `InternEvo-0.4.4/internlm/model/losses/ce_loss.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/metrics.py` & `InternEvo-0.4.4/internlm/model/metrics.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/modeling_internlm.py` & `InternEvo-0.4.4/internlm/model/modeling_internlm.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/modeling_internlm2.py` & `InternEvo-0.4.4/internlm/model/modeling_internlm2.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/modeling_llama.py` & `InternEvo-0.4.4/internlm/model/modeling_llama.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/modeling_llava.py` & `InternEvo-0.4.4/internlm/model/modeling_llava.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/modeling_moe.py` & `InternEvo-0.4.4/internlm/model/modeling_moe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/modules/embedding.py` & `InternEvo-0.4.4/internlm/model/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/modules/mlp.py` & `InternEvo-0.4.4/internlm/model/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/modules/multi_head_attention.py` & `InternEvo-0.4.4/internlm/model/modules/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/moe/__init__.py` & `InternEvo-0.4.4/internlm/model/moe/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/moe/base_layer.py` & `InternEvo-0.4.4/internlm/model/moe/base_layer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/moe/experts.py` & `InternEvo-0.4.4/internlm/model/moe/experts.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/moe/gshard_layer.py` & `InternEvo-0.4.4/internlm/model/moe/gshard_layer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/moe/megablock/megablock_dmoe.py` & `InternEvo-0.4.4/internlm/model/moe/megablock/megablock_dmoe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/moe/megablock/megablock_moe.py` & `InternEvo-0.4.4/internlm/model/moe/megablock/megablock_moe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/moe/megablock/mlp.py` & `InternEvo-0.4.4/internlm/model/moe/megablock/mlp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/moe/megablock/utils.py` & `InternEvo-0.4.4/internlm/model/moe/megablock/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/moe/moe.py` & `InternEvo-0.4.4/internlm/model/moe/moe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/moe/utils.py` & `InternEvo-0.4.4/internlm/model/moe/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/ops/fusion_ops_import_helper.py` & `InternEvo-0.4.4/internlm/model/ops/fusion_ops_import_helper.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/ops/linear.py` & `InternEvo-0.4.4/internlm/model/ops/linear.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/ops/norm.py` & `InternEvo-0.4.4/internlm/model/ops/norm.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/model/utils.py` & `InternEvo-0.4.4/internlm/model/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/monitor/alert.py` & `InternEvo-0.4.4/internlm/monitor/alert.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/monitor/monitor.py` & `InternEvo-0.4.4/internlm/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/monitor/utils.py` & `InternEvo-0.4.4/internlm/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/solver/activation_checkpoint.py` & `InternEvo-0.4.4/internlm/solver/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/solver/optimizer/base_optimizer.py` & `InternEvo-0.4.4/internlm/solver/optimizer/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/solver/optimizer/fsdp_optimizer.py` & `InternEvo-0.4.4/internlm/solver/optimizer/fsdp_optimizer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/solver/optimizer/hybrid_zero_optim.py` & `InternEvo-0.4.4/internlm/solver/optimizer/hybrid_zero_optim.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/solver/optimizer/store.py` & `InternEvo-0.4.4/internlm/solver/optimizer/store.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/solver/optimizer/utils.py` & `InternEvo-0.4.4/internlm/solver/optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/solver/pipeline_utils.py` & `InternEvo-0.4.4/internlm/solver/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/solver/schedulers/beta2_scheduler.py` & `InternEvo-0.4.4/internlm/solver/schedulers/beta2_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/solver/schedulers/lr_scheduler.py` & `InternEvo-0.4.4/internlm/solver/schedulers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/train/__init__.py` & `InternEvo-0.4.4/internlm/train/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/train/pipeline.py` & `InternEvo-0.4.4/internlm/train/pipeline.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/train/utils.py` & `InternEvo-0.4.4/internlm/train/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/utils/common.py` & `InternEvo-0.4.4/internlm/utils/common.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/utils/gputest.py` & `InternEvo-0.4.4/internlm/utils/gputest.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/utils/logger.py` & `InternEvo-0.4.4/internlm/utils/logger.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/utils/megatron_timers.py` & `InternEvo-0.4.4/internlm/utils/megatron_timers.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/utils/parallel.py` & `InternEvo-0.4.4/internlm/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/utils/registry.py` & `InternEvo-0.4.4/internlm/utils/registry.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/utils/simple_memory_profiler.py` & `InternEvo-0.4.4/internlm/utils/simple_memory_profiler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/utils/storage_manager.py` & `InternEvo-0.4.4/internlm/utils/storage_manager.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/utils/timeout.py` & `InternEvo-0.4.4/internlm/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/utils/utils.py` & `InternEvo-0.4.4/internlm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/internlm/utils/writer.py` & `InternEvo-0.4.4/internlm/utils/writer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/setup.py` & `InternEvo-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/tests/common_fixture.py` & `InternEvo-0.4.4/tests/common_fixture.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/tests/test_core/test_pipeline.py` & `InternEvo-0.4.4/tests/test_core/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/tests/test_core/utils.py` & `InternEvo-0.4.4/tests/test_core/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/tests/test_training/7B_check_acc.py` & `InternEvo-0.4.4/tests/test_training/7B_check_acc.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/tests/test_training/7B_check_init.py` & `InternEvo-0.4.4/tests/test_training/7B_check_init.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/tests/test_training/test_forward_output_no_fa.py` & `InternEvo-0.4.4/tests/test_training/test_forward_output_no_fa.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/tests/test_training/test_load_ckpt_loss.py` & `InternEvo-0.4.4/tests/test_training/test_load_ckpt_loss.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/tests/test_training/test_loss.py` & `InternEvo-0.4.4/tests/test_training/test_loss.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/tests/test_training/test_no_fa_train_temp.py` & `InternEvo-0.4.4/tests/test_training/test_no_fa_train_temp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/tests/test_training/test_norm_weight.py` & `InternEvo-0.4.4/tests/test_training/test_norm_weight.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/tests/test_training/test_swap_nb_loss_and_gradnorm.py` & `InternEvo-0.4.4/tests/test_training/test_swap_nb_loss_and_gradnorm.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.4.3/tests/test_training/train_CI.py` & `InternEvo-0.4.4/tests/test_training/train_CI.py`

 * *Files identical despite different names*

