# Comparing `tmp/hqq-0.1.7.post1.tar.gz` & `tmp/hqq-0.1.7.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hqq-0.1.7.post1.tar", last modified: Fri May  3 14:45:11 2024, max compression
+gzip compressed data, was "hqq-0.1.7.post2.tar", last modified: Mon May  6 16:38:05 2024, max compression
```

## Comparing `hqq-0.1.7.post1.tar` & `hqq-0.1.7.post2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.800661 hqq-0.1.7.post1/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    11360 2023-12-02 17:25:57.000000 hqq-0.1.7.post1/LICENSE
--rw-r--r--   0 hicham    (1009) hicham    (1009)      438 2024-05-03 14:45:11.800661 hqq-0.1.7.post1/PKG-INFO
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.784661 hqq-0.1.7.post1/hqq/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)       93 2024-05-03 14:43:06.000000 hqq-0.1.7.post1/hqq/__init__.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.788661 hqq-0.1.7.post1/hqq/backends/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2024-04-16 10:04:12.000000 hqq-0.1.7.post1/hqq/backends/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3228 2024-04-19 12:02:43.000000 hqq-0.1.7.post1/hqq/backends/marlin.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    10514 2024-04-24 08:49:06.000000 hqq-0.1.7.post1/hqq/backends/torchao.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.788661 hqq-0.1.7.post1/hqq/core/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-01 10:59:22.000000 hqq-0.1.7.post1/hqq/core/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     5195 2024-05-03 14:37:22.000000 hqq-0.1.7.post1/hqq/core/bitpack.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    14369 2024-05-03 14:37:54.000000 hqq-0.1.7.post1/hqq/core/optimize.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17172 2024-03-18 15:34:02.000000 hqq-0.1.7.post1/hqq/core/peft.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    28600 2024-05-03 14:41:05.000000 hqq-0.1.7.post1/hqq/core/quantize.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)      670 2024-05-03 14:37:54.000000 hqq-0.1.7.post1/hqq/core/utils.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.792661 hqq-0.1.7.post1/hqq/engine/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post1/hqq/engine/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3131 2024-03-25 11:05:14.000000 hqq-0.1.7.post1/hqq/engine/base.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2568 2024-03-15 09:12:21.000000 hqq-0.1.7.post1/hqq/engine/hf.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2458 2024-03-15 09:09:35.000000 hqq-0.1.7.post1/hqq/engine/timm.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     5287 2024-03-15 12:03:22.000000 hqq-0.1.7.post1/hqq/engine/vllm.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.792661 hqq-0.1.7.post1/hqq/kernels/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)       87 2024-03-15 10:04:14.000000 hqq-0.1.7.post1/hqq/kernels/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2670 2024-03-25 10:15:39.000000 hqq-0.1.7.post1/hqq/kernels/hqq_aten_cuda.cpp
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17933 2024-04-08 11:30:33.000000 hqq-0.1.7.post1/hqq/kernels/hqq_aten_cuda_kernel.cu
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3412 2024-02-21 11:27:07.000000 hqq-0.1.7.post1/hqq/kernels/hqq_aten_torch.cpp
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)      494 2024-03-19 10:48:06.000000 hqq-0.1.7.post1/hqq/kernels/setup_cuda.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)      292 2024-03-14 16:26:18.000000 hqq-0.1.7.post1/hqq/kernels/setup_torch.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.792661 hqq-0.1.7.post1/hqq/models/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-01 10:59:32.000000 hqq-0.1.7.post1/hqq/models/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17314 2024-04-22 18:40:37.000000 hqq-0.1.7.post1/hqq/models/base.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.796661 hqq-0.1.7.post1/hqq/models/hf/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post1/hqq/models/hf/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1057 2024-03-14 15:51:30.000000 hqq-0.1.7.post1/hqq/models/hf/base.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2703 2024-03-14 15:51:30.000000 hqq-0.1.7.post1/hqq/models/hf/llama.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2703 2024-03-14 15:51:30.000000 hqq-0.1.7.post1/hqq/models/hf/mistral.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3464 2024-03-14 15:51:30.000000 hqq-0.1.7.post1/hqq/models/hf/mixtral.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2487 2024-03-14 15:51:30.000000 hqq-0.1.7.post1/hqq/models/hf/phi.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2361 2024-03-14 15:51:30.000000 hqq-0.1.7.post1/hqq/models/hf/phi_opt.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.796661 hqq-0.1.7.post1/hqq/models/timm/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post1/hqq/models/timm/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)      750 2024-03-14 15:52:37.000000 hqq-0.1.7.post1/hqq/models/timm/base.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2815 2024-03-14 15:53:15.000000 hqq-0.1.7.post1/hqq/models/timm/vit_clip.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.796661 hqq-0.1.7.post1/hqq/models/vllm/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post1/hqq/models/vllm/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     6114 2024-03-15 12:07:03.000000 hqq-0.1.7.post1/hqq/models/vllm/base.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    16480 2024-03-14 15:55:27.000000 hqq-0.1.7.post1/hqq/models/vllm/llama.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.796661 hqq-0.1.7.post1/hqq/utils/
--rw-rw-r--   0 hicham    (1009) hicham    (1009)        0 2024-04-16 10:04:22.000000 hqq-0.1.7.post1/hqq/utils/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    10844 2024-04-23 16:50:10.000000 hqq-0.1.7.post1/hqq/utils/generation_hf.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     6066 2024-04-22 17:00:27.000000 hqq-0.1.7.post1/hqq/utils/patching.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.788661 hqq-0.1.7.post1/hqq.egg-info/
--rw-r--r--   0 hicham    (1009) hicham    (1009)      438 2024-05-03 14:43:35.000000 hqq-0.1.7.post1/hqq.egg-info/PKG-INFO
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1109 2024-05-03 14:43:35.000000 hqq-0.1.7.post1/hqq.egg-info/SOURCES.txt
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        1 2024-05-03 14:43:35.000000 hqq-0.1.7.post1/hqq.egg-info/dependency_links.txt
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)       92 2024-05-03 14:43:35.000000 hqq-0.1.7.post1/hqq.egg-info/requires.txt
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        4 2024-05-03 14:43:35.000000 hqq-0.1.7.post1/hqq.egg-info/top_level.txt
--rw-rw-r--   0 hicham    (1009) hicham    (1009)       38 2024-05-03 14:45:11.800661 hqq-0.1.7.post1/setup.cfg
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1706 2024-05-03 14:43:06.000000 hqq-0.1.7.post1/setup.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-03 14:45:11.800661 hqq-0.1.7.post1/tests/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3689 2024-03-25 10:44:50.000000 hqq-0.1.7.post1/tests/test_bitpack.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    11302 2024-03-01 10:40:44.000000 hqq-0.1.7.post1/tests/test_quantize.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.731692 hqq-0.1.7.post2/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    11360 2023-12-02 17:25:57.000000 hqq-0.1.7.post2/LICENSE
+-rw-r--r--   0 hicham    (1009) hicham    (1009)      438 2024-05-06 16:38:05.731692 hqq-0.1.7.post2/PKG-INFO
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.715691 hqq-0.1.7.post2/hqq/
+-rwxrwxr-x   0 hicham    (1009) hicham    (1009)       93 2024-05-06 15:26:52.000000 hqq-0.1.7.post2/hqq/__init__.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.719691 hqq-0.1.7.post2/hqq/backends/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2024-04-16 10:04:12.000000 hqq-0.1.7.post2/hqq/backends/__init__.py
+-rwxrwxr-x   0 hicham    (1009) hicham    (1009)     3351 2024-05-06 16:33:14.000000 hqq-0.1.7.post2/hqq/backends/marlin.py
+-rwxrwxr-x   0 hicham    (1009) hicham    (1009)    11856 2024-05-06 16:33:14.000000 hqq-0.1.7.post2/hqq/backends/torchao.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.723691 hqq-0.1.7.post2/hqq/core/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-01 10:59:22.000000 hqq-0.1.7.post2/hqq/core/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     5195 2024-05-03 14:37:22.000000 hqq-0.1.7.post2/hqq/core/bitpack.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    14369 2024-05-03 14:37:54.000000 hqq-0.1.7.post2/hqq/core/optimize.py
+-rwxrwxr-x   0 hicham    (1009) hicham    (1009)    17325 2024-05-06 15:26:52.000000 hqq-0.1.7.post2/hqq/core/peft.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    28621 2024-05-03 15:01:23.000000 hqq-0.1.7.post2/hqq/core/quantize.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)      670 2024-05-03 14:37:54.000000 hqq-0.1.7.post2/hqq/core/utils.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.723691 hqq-0.1.7.post2/hqq/engine/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post2/hqq/engine/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3159 2024-05-06 07:14:36.000000 hqq-0.1.7.post2/hqq/engine/base.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2568 2024-03-15 09:12:21.000000 hqq-0.1.7.post2/hqq/engine/hf.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2458 2024-03-15 09:09:35.000000 hqq-0.1.7.post2/hqq/engine/timm.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     5287 2024-03-15 12:03:22.000000 hqq-0.1.7.post2/hqq/engine/vllm.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.727692 hqq-0.1.7.post2/hqq/kernels/
+-rwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 15:26:46.000000 hqq-0.1.7.post2/hqq/kernels/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2670 2024-03-25 10:15:39.000000 hqq-0.1.7.post2/hqq/kernels/hqq_aten_cuda.cpp
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17933 2024-04-08 11:30:33.000000 hqq-0.1.7.post2/hqq/kernels/hqq_aten_cuda_kernel.cu
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3412 2024-02-21 11:27:07.000000 hqq-0.1.7.post2/hqq/kernels/hqq_aten_torch.cpp
+-rwxrwxr-x   0 hicham    (1009) hicham    (1009)      473 2024-05-06 15:26:46.000000 hqq-0.1.7.post2/hqq/kernels/setup_cuda.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)      292 2024-03-14 16:26:18.000000 hqq-0.1.7.post2/hqq/kernels/setup_torch.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.727692 hqq-0.1.7.post2/hqq/models/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-01 10:59:32.000000 hqq-0.1.7.post2/hqq/models/__init__.py
+-rwxrwxr-x   0 hicham    (1009) hicham    (1009)    18084 2024-05-06 15:26:52.000000 hqq-0.1.7.post2/hqq/models/base.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.727692 hqq-0.1.7.post2/hqq/models/hf/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post2/hqq/models/hf/__init__.py
+-rwxrwxr-x   0 hicham    (1009) hicham    (1009)     1255 2024-05-06 16:33:14.000000 hqq-0.1.7.post2/hqq/models/hf/base.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2703 2024-03-14 15:51:30.000000 hqq-0.1.7.post2/hqq/models/hf/llama.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2703 2024-03-14 15:51:30.000000 hqq-0.1.7.post2/hqq/models/hf/mistral.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3464 2024-03-14 15:51:30.000000 hqq-0.1.7.post2/hqq/models/hf/mixtral.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2487 2024-03-14 15:51:30.000000 hqq-0.1.7.post2/hqq/models/hf/phi.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2361 2024-03-14 15:51:30.000000 hqq-0.1.7.post2/hqq/models/hf/phi_opt.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.727692 hqq-0.1.7.post2/hqq/models/timm/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post2/hqq/models/timm/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)      750 2024-03-14 15:52:37.000000 hqq-0.1.7.post2/hqq/models/timm/base.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2815 2024-03-14 15:53:15.000000 hqq-0.1.7.post2/hqq/models/timm/vit_clip.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.731692 hqq-0.1.7.post2/hqq/models/vllm/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post2/hqq/models/vllm/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     6114 2024-03-15 12:07:03.000000 hqq-0.1.7.post2/hqq/models/vllm/base.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    16480 2024-03-14 15:55:27.000000 hqq-0.1.7.post2/hqq/models/vllm/llama.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.731692 hqq-0.1.7.post2/hqq/utils/
+-rw-rw-r--   0 hicham    (1009) hicham    (1009)        0 2024-05-06 15:26:46.000000 hqq-0.1.7.post2/hqq/utils/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    10844 2024-04-23 16:50:10.000000 hqq-0.1.7.post2/hqq/utils/generation_hf.py
+-rwxrwxr-x   0 hicham    (1009) hicham    (1009)     6319 2024-05-06 16:33:14.000000 hqq-0.1.7.post2/hqq/utils/patching.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.719691 hqq-0.1.7.post2/hqq.egg-info/
+-rw-r--r--   0 hicham    (1009) hicham    (1009)      438 2024-05-06 16:37:56.000000 hqq-0.1.7.post2/hqq.egg-info/PKG-INFO
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1109 2024-05-06 16:37:56.000000 hqq-0.1.7.post2/hqq.egg-info/SOURCES.txt
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        1 2024-05-06 16:37:56.000000 hqq-0.1.7.post2/hqq.egg-info/dependency_links.txt
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)       92 2024-05-06 16:37:56.000000 hqq-0.1.7.post2/hqq.egg-info/requires.txt
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        4 2024-05-06 16:37:56.000000 hqq-0.1.7.post2/hqq.egg-info/top_level.txt
+-rw-rw-r--   0 hicham    (1009) hicham    (1009)       38 2024-05-06 16:38:05.731692 hqq-0.1.7.post2/setup.cfg
+-rwxrwxr-x   0 hicham    (1009) hicham    (1009)     1706 2024-05-06 15:26:52.000000 hqq-0.1.7.post2/setup.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.731692 hqq-0.1.7.post2/tests/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3689 2024-03-25 10:44:50.000000 hqq-0.1.7.post2/tests/test_bitpack.py
+-rw-rw-r--   0 hicham    (1009) hicham    (1009)    11302 2024-05-06 15:26:46.000000 hqq-0.1.7.post2/tests/test_quantize.py
```

### Comparing `hqq-0.1.7.post1/LICENSE` & `hqq-0.1.7.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/backends/marlin.py` & `hqq-0.1.7.post2/hqq/backends/marlin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,96 +1,116 @@
 # Written by Dr. Hicham Badri @Mobius Labs GmbH - 2024
 #####################################################
-import torch 
+import torch
+
 try:
     import marlin
 except Exception:
     marlin = None
 from ..core.quantize import Quantizer
 
+
 class MarlinLinear(torch.nn.Module):
-    def __init__(self, W: torch.Tensor, scales: torch.Tensor, u=None, bias=None, groupsize=-1):
+    def __init__(
+        self, W: torch.Tensor, scales: torch.Tensor, u=None, bias=None, groupsize=-1
+    ):
         super().__init__()
 
-        m, n   = W.shape
+        m, n = W.shape
         device = W.device
         _linear = torch.nn.Linear(m, n)
         _linear.weight.data = W.half().t()
 
-        effective_groupsize = m if (groupsize==-1) else groupsize
+        effective_groupsize = m if (groupsize == -1) else groupsize
 
-        _layer   = marlin.Layer(m, n, groupsize=groupsize)
+        _layer = marlin.Layer(m, n, groupsize=groupsize)
         _layer.k = m
         _layer.n = n
         _layer.groupsize = effective_groupsize
         _layer.B = torch.empty((m // 16, n * 16 // 8), dtype=torch.int, device=device)
-        _layer.s = torch.empty((m // effective_groupsize, n), dtype=torch.half, device=device)
+        _layer.s = torch.empty(
+            (m // effective_groupsize, n), dtype=torch.half, device=device
+        )
         _layer.pack(_linear, scales.t())
 
-        self.bias          = bias.half() if (bias is not None) else None
-        self.Wq_packed     = _layer.B.clone()
-        self.scales        = _layer.s.clone()
-        self.workspace_fp  = torch.zeros(n // 128 * 16, device=device)
-        self.in_features   = m
-        self.out_features  = n
-        self.group_size    = effective_groupsize
-        self.axis          = 1
-        self.device        = device 
+        self.bias = bias.half() if (bias is not None) else None
+        self.Wq_packed = _layer.B.clone()
+        self.scales = _layer.s.clone()
+        self.workspace_fp = torch.zeros(n // 128 * 16, device=device)
+        self.in_features = m
+        self.out_features = n
+        self.group_size = effective_groupsize
+        self.axis = 1
+        self.device = device
         self.compute_dtype = torch.float16
-        self.u             = torch.nn.Parameter(u, requires_grad=False) if (u is not None) else None
+        self.u = torch.nn.Parameter(u, requires_grad=False) if (u is not None) else None
 
         del _linear, _layer
         torch.cuda.empty_cache()
 
     @torch.no_grad()
     def matmul(self, x):
-        out = torch.empty(x.shape[:-1] + (self.scales.shape[1],), dtype=x.dtype, device=x.device)
-        marlin.mul(x.view((-1, x.shape[-1])), self.Wq_packed, out.view((-1, out.shape[-1])), self.scales, self.workspace_fp)
+        out = torch.empty(
+            x.shape[:-1] + (self.scales.shape[1],), dtype=x.dtype, device=x.device
+        )
+        marlin.mul(
+            x.view((-1, x.shape[-1])),
+            self.Wq_packed,
+            out.view((-1, out.shape[-1])),
+            self.scales,
+            self.workspace_fp,
+        )
         return out
 
     @torch.jit.ignore
     def forward(self, x):
         out = self.matmul(x)
 
-        if(self.u is not None):
+        if self.u is not None:
             out += torch.matmul(x.sum(axis=-1, keepdim=True), self.u)
 
-        if(self.bias is not None):
+        if self.bias is not None:
             out += self.bias
 
         return out
 
-#ONLY WORKS WITH AXIS=1, group_size= - 1
+
+# ONLY WORKS WITH AXIS=1, group_size= - 1
 def patch_hqq_to_marlin(layer, patch_params):
-    if(marlin is None):
+    if marlin is None:
         return layer
 
-    z_shift   = 8.
-    hqq_layer = layer.linear_layer if hasattr(layer, 'linear_layer') else layer
+    z_shift = 8.0
+    hqq_layer = layer.linear_layer if hasattr(layer, "linear_layer") else layer
 
-    #Check config suppport
-    w_q_config = hqq_layer.quant_config['weight_quant_params']
-    if((w_q_config['axis']==0) or (w_q_config['group_size'] is not None) or (w_q_config['nbits']!=4)):
+    # Check config suppport
+    if (
+        (hqq_layer.meta["axis"] == 0)
+        or (hqq_layer.meta["group_size"] is not None)
+        or (hqq_layer.meta["nbits"] != 4)
+    ):
+        print("Skipping marlin conversion for", hqq_layer.name)
         return layer
 
-
-    W_r  = Quantizer.unpack[hqq_layer.meta['packing']](hqq_layer.W_q, dtype=hqq_layer.compute_dtype).t()
-    z    = hqq_layer.meta['zero']
-    s    = hqq_layer.meta['scale'].t()
-    W_r  = (W_r - z_shift) * s
-
-    if(type(z) in [torch.Tensor, torch.nn.Parameter]):
-        z  = z.t()
-        u  = (s*(-z + z_shift)).view([1, -1])
+    W_r = Quantizer.unpack[hqq_layer.meta["packing"]](
+        hqq_layer.W_q, dtype=hqq_layer.compute_dtype
+    ).t()
+    z = hqq_layer.meta["zero"]
+    s = hqq_layer.meta["scale"].t()
+    W_r = (W_r - z_shift) * s
+
+    if type(z) in [torch.Tensor, torch.nn.Parameter]:
+        z = z.t()
+        u = (s * (-z + z_shift)).view([1, -1])
     else:
         u = None
 
     marlin_layer = MarlinLinear(W_r, s, u=u, bias=hqq_layer.bias)
 
-    if hasattr(layer, 'linear_layer'):
+    if hasattr(layer, "linear_layer"):
         del layer.linear_layer
         layer.linear_layer = marlin_layer
     else:
         del hqq_layer
         layer = marlin_layer
 
     torch.cuda.empty_cache()
```

### Comparing `hqq-0.1.7.post1/hqq/backends/torchao.py` & `hqq-0.1.7.post2/hqq/backends/torchao.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,311 +1,388 @@
 # Written by Dr. Hicham Badri @Mobius Labs GmbH - 2024
 #####################################################
 
-#Makes HQQ 4-bit (axis=1) compatbile with torch.ops.aten._weight_int4pack_mm
+# Makes HQQ 4-bit (axis=1) compatbile with torch.ops.aten._weight_int4pack_mm
 
-#The code is partially based on: https://github.com/pytorch-labs/gpt-fast/blob/main/quantize.py (BSD-3-Clause license)
-#Only the packing logic is copied, the rest is rewritten to support HQQ's logic
+# The code is partially based on: https://github.com/pytorch-labs/gpt-fast/blob/main/quantize.py (BSD-3-Clause license)
+# Only the packing logic is copied, the rest is rewritten to support HQQ's logic
 
-#Only works with: bfloat16, axis=1. 
-#Only tested on Ada gpus.
+# Only works with: bfloat16, axis=1.
+# Only tested on Ada gpus.
 
 import torch
 import copy
 from torch import bfloat16, nn, Tensor
 import torch.nn.functional as F
+from typing import Union
 
 from ..core.quantize import HQQLinear, Quantizer
 from ..core.peft import HQQLinearLoRA
 from ..core.utils import cleanup
 
+
 class HQQLinearTorchWeightOnlynt4(torch.nn.Module):
     def __init__(
         self,
-        linear_layer: nn.Module | None,
+        linear_layer: Union[nn.Module, None],
         quant_config: dict,
         del_orig: bool = True,
         compute_dtype: torch.dtype = bfloat16,
         device: str = "cuda",
         initialize: bool = True,
-        inner_k_tiles=8, 
+        inner_k_tiles=8,
         padding=True,
     ):
         super().__init__()
 
         self.ready = False
         self.in_gpu = False
         self.bias = None
         self.device = device
         self.compute_dtype = compute_dtype
-        self.quant_config = copy.deepcopy(quant_config)
+        self.quant_config = (
+            copy.deepcopy(quant_config) if (quant_config is not None) else None
+        )
         self.del_orig = del_orig
 
-        weight_quant_params = self.quant_config['weight_quant_params']
-        self.groupsize      = weight_quant_params['group_size']
-        self.nbits          = weight_quant_params['nbits']
-        self.inner_k_tiles  = inner_k_tiles
-        self.padding        = padding
+        if (quant_config is None) and (linear_layer is None):
+            raise Exception(
+                "Invalid parameters: Both quant_config and linear_layer are None."
+            )
+
+        if (quant_config is None) and (initialize is True):
+            raise Exception(
+                "Invalid parameters: setting initialize to True requires a quant_config."
+            )
+
+        if self.quant_config is not None:
+            weight_quant_params = self.quant_config["weight_quant_params"]
+            self.groupsize = weight_quant_params["group_size"]
+            self.nbits = weight_quant_params["nbits"]
+            self.axis = weight_quant_params["axis"]
+
+        if linear_layer is not None:
+            self.groupsize = linear_layer.meta["group_size"]
+            self.nbits = linear_layer.meta["nbits"]
+            self.axis = linear_layer.meta["axis"]
+
+        self.inner_k_tiles = inner_k_tiles
+        self.padding = padding
 
-        assert weight_quant_params['axis']==1, "Only axis==1 is supported"
-        assert self.compute_dtype is bfloat16, "Only bfloat16 compute_dtype is supported."
+        assert self.axis==1, "Only axis==1 is supported"
         assert self.nbits in [4], "Unsupported nbits."
+        assert (
+            self.compute_dtype is bfloat16
+        ), "Only bfloat16 compute_dtype is supported."
         assert self.groupsize in [None, 32, 64, 128, 256], "Unsupported groupsize."
         assert self.inner_k_tiles in [2, 4, 8], "Unsupported tile."
 
-        self.linear_layer  = linear_layer
-        
+        self.linear_layer = linear_layer
+
         if initialize:
             self.initialize()
 
-    ###################### Initializers ###################### 
+    ###################### Initializers ######################
     def initialize_with_hqq_quants(self, W_q, meta, bias=None):
+        self.padding = (
+            False  # Force padding off, a bit tricky to post-pad with grouping
+        )
 
-        self.padding = False #Force padding off, a bit tricky to post-pad with grouping
-
-        self.set_shape(meta['shape'])
+        self.set_shape(meta["shape"])
         self.process_hqq_quants(W_q, meta)
-        self.bias   = bias
-        self.ready  = True
+        self.bias = bias
+        self.ready = True
         self.in_gpu = True
         torch.cuda.empty_cache()
 
         return self
 
     def initialize(self):
         if self.linear_layer is not None:
-
             W = self.linear_layer.weight.data
             self.set_shape(W.shape)
 
-            if(self.in_features_diff>0):
-                W =  F.pad(W, pad=(0, self.in_features_diff), value=0)
-            
+            if self.in_features_diff > 0:
+                W = F.pad(W, pad=(0, self.in_features_diff), value=0)
+
             W_q, meta = self.quantize(W, **self.quant_config)
             self.process_hqq_quants(W_q, meta)
             del W_q, meta
 
             self.bias = (
                 None
                 if (self.linear_layer.bias is None)
-                else self.linear_layer.bias.to(dtype=self.compute_dtype, device=self.device)
+                else self.linear_layer.bias.to(
+                    dtype=self.compute_dtype, device=self.device
+                )
             )
 
         if self.del_orig:
             del self.linear_layer
 
-        self.ready  = True
+        self.ready = True
         self.in_gpu = True
         torch.cuda.empty_cache()
 
         return self
 
     ###################### Quantize/packing ######################
 
-    def quantize(self, W: Tensor, weight_quant_params: dict, scale_quant_params=dict | None, zero_quant_params=dict | None, offload_meta=False):
-
-        W_q, meta = Quantizer.quantize(W, **weight_quant_params, device=self.device, compute_dtype=self.compute_dtype, bitpack=False)
-
-        #ToDO: meta quantization
+    def quantize(
+        self,
+        W: Tensor,
+        weight_quant_params: dict,
+        scale_quant_params=dict | None,
+        zero_quant_params=dict | None,
+        offload_meta=False,
+    ):
+        W_q, meta = Quantizer.quantize(
+            W,
+            **weight_quant_params,
+            device=self.device,
+            compute_dtype=self.compute_dtype,
+            bitpack=False,
+        )
 
-        return W_q, meta 
+        # ToDO: meta quantization
 
+        return W_q, meta
 
-    #TODO: move these to utils
+    # TODO: move these to utils
     @torch.no_grad()
     def reshape_meta_axis1(self, meta_tensor, new_group_size, shape):
         meta_tensor = meta_tensor.repeat([1, shape[1]]).reshape(shape)
-        meta_tensor = torch.mean(meta_tensor.reshape([-1, new_group_size]), axis=1, keepdim=True)
+        meta_tensor = torch.mean(
+            meta_tensor.reshape([-1, new_group_size]), axis=1, keepdim=True
+        )
         return meta_tensor
 
     def find_multiple(self, n: int, k: int) -> int:
-        if n % k == 0: 
+        if n % k == 0:
             return n
         return n + k - (n % k)
 
     def set_shape(self, shape):
-        self.shape         = shape
-        self.in_features   = shape[1]
-        self.out_features  = shape[0]
-        
+        self.shape = shape
+        self.in_features = shape[1]
+        self.out_features = shape[0]
+
         self.origin_in_features = self.in_features
-        if(self.padding):
+        if self.padding:
             self.in_features = self.find_multiple(self.in_features, 1024)
-        
+
         self.in_features_diff = self.in_features - self.origin_in_features
 
     @torch.no_grad()
     def process_hqq_quants(self, W_q, meta):
+        scales = meta["scale"]
+        zeros = meta["zero"]
+        shape = meta["shape"]
 
-        scales = meta['scale']
-        zeros  = meta['zero']
-        shape  = meta['shape']
-
-        if(meta["packing"] is not None):
-            W_q = Quantizer.unpack[meta['packing']](W_q)
+        if meta["packing"] is not None:
+            W_q = Quantizer.unpack[meta["packing"]](W_q)
 
-        if(self.groupsize is None):
+        if self.groupsize is None:
             self.groupsize = 128
-            W_q    = W_q.reshape([-1, self.groupsize])
+            W_q = W_q.reshape([-1, self.groupsize])
             scales = self.reshape_meta_axis1(scales, self.groupsize, shape)
-            zeros  = self.reshape_meta_axis1(zeros,  self.groupsize, shape)
-
+            zeros = self.reshape_meta_axis1(zeros, self.groupsize, shape)
 
-        W_q_torch, scales_torch, zeros_torch = self.hqq_quants_to_torch_quants(W_q=W_q, scales=scales, zeros=zeros, shape=shape, nbits=self.nbits)
-        self.weight_int4pack  = torch.ops.aten._convert_weight_to_int4pack(W_q_torch, self.inner_k_tiles)
+        W_q_torch, scales_torch, zeros_torch = self.hqq_quants_to_torch_quants(
+            W_q=W_q, scales=scales, zeros=zeros, shape=shape, nbits=self.nbits
+        )
+        self.weight_int4pack = torch.ops.aten._convert_weight_to_int4pack(
+            W_q_torch, self.inner_k_tiles
+        )
         self.scales_and_zeros = self.pack_scales_and_zeros(scales_torch, zeros_torch)
 
         del W_q_torch, scales_torch, zeros_torch
         torch.cuda.empty_cache()
 
     @torch.no_grad()
-    def hqq_quants_to_torch_quants(self, W_q: Tensor, scales: Tensor, zeros: Tensor, shape, nbits=4):
-
-        W_q    = W_q.to(dtype=self.compute_dtype, device=self.device)
+    def hqq_quants_to_torch_quants(
+        self, W_q: Tensor, scales: Tensor, zeros: Tensor, shape, nbits=4
+    ):
+        W_q = W_q.to(dtype=self.compute_dtype, device=self.device)
         scales = scales.to(dtype=self.compute_dtype, device=self.device)
-        zeros  = zeros.to(dtype=self.compute_dtype, device=self.device)
+        zeros = zeros.to(dtype=self.compute_dtype, device=self.device)
 
         max_int = 2**nbits - 1
         min_int = 0
-        dump    = 2 ** (nbits - 1)
+        dump = 2 ** (nbits - 1)
 
-        #HQQ -> torch logic
-        new_zeros   = (scales * dump) - zeros*scales
+        # HQQ -> torch logic
+        new_zeros = (scales * dump) - zeros * scales
 
         min_val = new_zeros - scales * dump
 
-        #group_quantize_tensor_from_qparams
-        W_r  = (W_q - zeros)*scales
+        # group_quantize_tensor_from_qparams
+        W_r = (W_q - zeros) * scales
 
-        W_q = W_r.sub(min_val).div(scales).round().clamp_(min_int, max_int).to(torch.int32).reshape(shape).contiguous()
+        W_q = (
+            W_r.sub(min_val)
+            .div(scales)
+            .round()
+            .clamp_(min_int, max_int)
+            .to(torch.int32)
+            .reshape(shape)
+            .contiguous()
+        )
 
-        #group_dequantize_tensor_from_qparams
-        #W_r = W_q*scales + min_val
+        # group_dequantize_tensor_from_qparams
+        # W_r = W_q*scales + min_val
 
-        scales     = scales.contiguous().reshape(shape[0], -1)
-        new_zeros  = new_zeros.contiguous().reshape(shape[0], -1)
+        scales = scales.contiguous().reshape(shape[0], -1)
+        new_zeros = new_zeros.contiguous().reshape(shape[0], -1)
 
         return W_q, scales, new_zeros
 
     def pack_scales_and_zeros(self, scales, zeros):
         assert scales.shape == zeros.shape
         assert scales.dtype == bfloat16
-        assert zeros.dtype  == bfloat16
+        assert zeros.dtype == bfloat16
         return (
             torch.cat(
                 [
                     scales.reshape(scales.size(0), scales.size(1), 1),
                     zeros.reshape(zeros.size(0), zeros.size(1), 1),
                 ],
                 2,
             )
             .transpose(0, 1)
             .contiguous()
         )
 
     ###################### Forward/matmul ######################
 
-    #@torch.jit.ignore()
+    # @torch.jit.ignore()
     def matmul(self, x: Tensor) -> Tensor:
         origin_x_size = x.size()
         x = x.reshape(-1, origin_x_size[-1])
-        c = torch.ops.aten._weight_int4pack_mm(x, self.weight_int4pack, self.groupsize, self.scales_and_zeros)
+        c = torch.ops.aten._weight_int4pack_mm(
+            x, self.weight_int4pack, self.groupsize, self.scales_and_zeros
+        )
         new_shape = origin_x_size[:-1] + (self.out_features,)
         c = c.reshape(new_shape)
         return c
 
-    #TODO without matmul
+    # TODO without matmul
     def dequantize(self) -> Tensor:
-        return self.matmul(torch.eye(self.in_features, dtype=self.compute_dtype, device=self.device))[:self.origin_in_features].t()
+        return self.matmul(
+            torch.eye(self.in_features, dtype=self.compute_dtype, device=self.device)
+        )[: self.origin_in_features].t()
 
-    #TODO: backward
+    # TODO: backward
     def forward(self, x: Tensor) -> Tensor:
         if self.in_features_diff > 0:
             x = F.pad(x, pad=(0, self.in_features_diff))
 
         out = self.matmul(x)
 
-        if(self.bias is not None):
+        if self.bias is not None:
             out += self.bias
         return out
 
 
 ###################### Patching ######################
 def patch_linearlayers(model, fct, patch_param=None):
-    model.base_class.patch_linearlayers(model, fct, {lin_tag:patch_param for lin_tag in model.base_class.get_linear_tags()})
+    model.base_class.patch_linearlayers(
+        model,
+        fct,
+        {lin_tag: patch_param for lin_tag in model.base_class.get_linear_tags()},
+    )
 
-def patch_hqq_to_aoint4(layer, patch_params):
 
+def patch_hqq_to_aoint4(layer, patch_params):
     hqq_layer = None
-    if(type(layer) is HQQLinear):
-        hqq_layer = layer 
-    if(type(layer) is HQQLinearLoRA):
+    if type(layer) is HQQLinear:
+        hqq_layer = layer
+    if type(layer) is HQQLinearLoRA:
         hqq_layer = layer.linear_layer
 
-    if(hqq_layer is None): 
+    if hqq_layer is None:
         return layer
 
-    w_q_config = hqq_layer.quant_config['weight_quant_params']
-    if(w_q_config['nbits']!=4 or w_q_config['axis']==0):
+    if hqq_layer.meta["nbits"] != 4 or hqq_layer.meta["axis"] != 1:
+        print("Skipping aoint4 conversion for ", hqq_layer.name)
         return layer
 
-    hqq_aoint4_layer  = HQQLinearTorchWeightOnlynt4(None, quant_config=hqq_layer.quant_config, compute_dtype=hqq_layer.compute_dtype, device=hqq_layer.device, del_orig=False, initialize=False, padding=False)
-    hqq_aoint4_layer.initialize_with_hqq_quants(hqq_layer.W_q, hqq_layer.meta, hqq_layer.bias)
+    quant_config = getattr(hqq_layer, "quant_config", None)
+
+    hqq_aoint4_layer = HQQLinearTorchWeightOnlynt4(
+        None,
+        quant_config=quant_config,
+        compute_dtype=hqq_layer.compute_dtype,
+        device=hqq_layer.device,
+        del_orig=False,
+        initialize=False,
+        padding=False,
+    )
+    hqq_aoint4_layer.initialize_with_hqq_quants(
+        hqq_layer.W_q, hqq_layer.meta, hqq_layer.bias
+    )
 
     del hqq_layer
     torch.cuda.empty_cache()
 
-    if(type(layer) is HQQLinear):
+    if type(layer) is HQQLinear:
         return hqq_aoint4_layer
 
-    if(type(layer) is HQQLinearLoRA):
+    if type(layer) is HQQLinearLoRA:
         layer.linear_layer = hqq_aoint4_layer
 
     return layer
 
 
-
 def replace_with_torchInt4(model):
     patch_linearlayers(model, patch_hqq_to_aoint4)
     cleanup()
 
 
-#Force requantize, mainly to check if the padding with int4mm is faster
+# Force requantize, mainly to check if the padding with int4mm is faster
 def patch_hqq_to_aoint4_force_requantize(layer, patch_params):
-
     hqq_layer = None
-    if(type(layer) is HQQLinear):
-        hqq_layer = layer 
-    if(type(layer) is HQQLinearLoRA):
+    if type(layer) is HQQLinear:
+        hqq_layer = layer
+    if type(layer) is HQQLinearLoRA:
         hqq_layer = layer.linear_layer
 
-    if(hqq_layer is None): 
+    if hqq_layer is None:
         return layer
 
-    w_q_config = hqq_layer.quant_config['weight_quant_params']
-    if(w_q_config['nbits']!=4 or w_q_config['axis']==0):
+    if hqq_layer.meta["nbits"] != 4 or hqq_layer.meta["axis"] != 1:
+        print("Skipping aoint4 conversion for ", hqq_layer.name)
         return layer
 
-    #Create dummy linear layer to store dequantize weights
+    # Create dummy linear layer to store dequantize weights
     dummy_linear = torch.nn.Linear(1, 1, bias=False)
     dummy_linear.weight.data = hqq_layer.dequantize()
 
-    #Disable optimizer on already dequantized weights
+    # Disable optimizer on already dequantized weights
     quant_config = hqq_layer.quant_config
-    quant_config['weight_quant_params']['optimize'] = False
+    quant_config["weight_quant_params"]["optimize"] = False
 
-    hqq_aoint4_layer = HQQLinearTorchWeightOnlynt4(dummy_linear, quant_config=quant_config, compute_dtype=hqq_layer.compute_dtype, device=hqq_layer.device, del_orig=True, initialize=True, padding=True)
+    hqq_aoint4_layer = HQQLinearTorchWeightOnlynt4(
+        dummy_linear,
+        quant_config=quant_config,
+        compute_dtype=hqq_layer.compute_dtype,
+        device=hqq_layer.device,
+        del_orig=True,
+        initialize=True,
+        padding=True,
+    )
 
     del hqq_layer
     torch.cuda.empty_cache()
 
-    if(type(layer) is HQQLinear):
+    if type(layer) is HQQLinear:
         return hqq_aoint4_layer
-        
-    if(type(layer) is HQQLinearLoRA):
+
+    if type(layer) is HQQLinearLoRA:
         layer.linear_layer = hqq_aoint4_layer
 
     return layer
 
+
 def replace_with_torchInt4_force_requantize(model):
     patch_linearlayers(model, patch_hqq_to_aoint4_force_requantize)
     cleanup()
```

### Comparing `hqq-0.1.7.post1/hqq/core/bitpack.py` & `hqq-0.1.7.post2/hqq/core/bitpack.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/core/optimize.py` & `hqq-0.1.7.post2/hqq/core/optimize.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/core/peft.py` & `hqq-0.1.7.post2/hqq/core/peft.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Written by Dr. Hicham Badri @Mobius Labs GmbH - 2023
 #####################################################
 import torch
 from torch import float16, bfloat16, float32
-from torch import Tensor
-from torch import nn
+from torch import Tensor, nn
 import numpy as np
 from .quantize import HQQLinear, Quantizer
 from .utils import cleanup
 
 
 # Return trainable weight matrix
 def _get_dense_param(
@@ -398,29 +397,32 @@
 
 
 # Putting it all together
 class PeftUtils:
     @classmethod
     def get_base_class(cls, model, base_class):
         # Get base class
-        if (base_class is None) and hasattr(model, "base_class"):
-            base_class = model.base_class
+        if base_class is None:
+            base_class = getattr(model, "base_class", None)
 
         assert (
             base_class is not None
-        ), "You need to provide the base HQQ class (LlamaHQQ, MixtralHQQ, etc.) as model.base_class or as an argument base_class=LlamaHQQ"
+        ), "You need to provide the base HQQ class (LlamaHQQ, MixtralHQQ, etc.) as model.base_class or as an argument base_class=LlamaHQQ. Use AutoHQQHFMode if the model architecture is not supported."
+
         return base_class
 
     @classmethod
     def add_lora(
         cls, model, peft_config, base_class: bool = None, verbose: bool = True
     ) -> None:
         # Base classs
         base_class = cls.get_base_class(model, base_class)
 
+        base_class.setup_model(model)
+
         # Freeze
         for param in model.parameters():
             param.requires_grad = False
 
         # Patch
         base_class.patch_linearlayers(
             model, patch_linear_add_peft, peft_config, verbose=verbose
@@ -447,16 +449,18 @@
     @classmethod
     def cast_lora_weights(
         cls, model, dtype: torch.dtype, base_class: bool = None, verbose: bool = True
     ) -> None:
         # Base classs
         base_class = cls.get_base_class(model, base_class)
 
+        base_class.setup_model(model)
+
         # Linear tags
-        linear_tags = base_class.get_linear_tags()
+        linear_tags = model.linear_tags
 
         # Patch
         base_class.patch_linearlayers(
             model,
             patch_linear_cast_peft,
             dict([(linear_tag, dtype) for linear_tag in linear_tags]),
             verbose=verbose,
@@ -465,24 +469,26 @@
     @classmethod
     def save_lora_weights(
         cls, model, filename: str, base_class: bool = None, verbose: bool = True
     ) -> None:
         # Base classs
         base_class = cls.get_base_class(model, base_class)
 
+        base_class.setup_model(model)
+
         lora_global_params = {}
 
         def _patch_linear_save_weights(layer, patch_params, return_layer=True):
             if is_hqq_lora_layer(layer):
                 lora_global_params[layer.name] = layer.state_dict()
             if return_layer:
                 return layer
 
         # Linear tags
-        linear_tags = base_class.get_linear_tags()
+        linear_tags = model.linear_tags
 
         # Patch
         base_class.patch_linearlayers(
             model,
             _patch_linear_save_weights,
             dict([(linear_tag, None) for linear_tag in linear_tags]),
             verbose=verbose,
@@ -497,14 +503,16 @@
     @classmethod
     def load_lora_weights(
         cls, model, filename: str, base_class: bool = None, verbose: bool = True
     ) -> None:
         # Base classs
         base_class = cls.get_base_class(model, base_class)
 
+        base_class.setup_model(model)
+
         lora_data = torch.load(filename, map_location="cpu")
 
         # V0.2 format: automatically creates lora modules if the model doesn't contain it
         if ("peft_config" in lora_data) and ("parameters" in lora_data):
             peft_config = lora_data["peft_config"]
             lora_global_params = lora_data["parameters"]
             if not hasattr(model, "peft_config"):
@@ -521,15 +529,15 @@
         def _patch_linear_load_weights(layer, patch_params, return_layer=True):
             if is_hqq_lora_layer(layer):
                 layer.load_state_dict(lora_global_params[layer.name])
             if return_layer:
                 return layer
 
         # Linear tags
-        linear_tags = base_class.get_linear_tags()
+        linear_tags = model.linear_tags
 
         # Patch
         base_class.patch_linearlayers(
             model,
             _patch_linear_load_weights,
             dict([(linear_tag, None) for linear_tag in linear_tags]),
             verbose=verbose,
```

### Comparing `hqq-0.1.7.post1/hqq/core/quantize.py` & `hqq-0.1.7.post2/hqq/core/quantize.py`

 * *Files 0% similar despite different names*

```diff
@@ -473,16 +473,17 @@
 
         return self
 
     def to(self, *args, **kwargs):
         # TODO: later
         return self
 
-    def to_empty(self, device, recurse=True):
-        return self.cuda(device)
+    #TODO: later
+    # def to_empty(self, device, recurse=True):
+    #     return self.cuda(device)
 
     def type(self, dst_type):
         # TODO: later
         return self
 
     def half(self, *args, **kwargs):
         return self
```

### Comparing `hqq-0.1.7.post1/hqq/core/utils.py` & `hqq-0.1.7.post2/hqq/core/utils.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/engine/base.py` & `hqq-0.1.7.post2/hqq/engine/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,19 +71,19 @@
 
     @classmethod
     def from_quantized(
         cls,
         save_dir_or_hub,
         compute_dtype: torch.dtype = float16,
         device="cuda",
-        cache_dir: str = "",
+        cache_dir: str | None = "",
         adapter: str = None,
     ):
         # Both local and hub-support
-        save_dir = BaseHQQModel.try_snapshot_download(save_dir_or_hub)
+        save_dir = BaseHQQModel.try_snapshot_download(save_dir_or_hub, cache_dir=cache_dir)
         arch_key = cls._get_arch_key_from_save_dir(save_dir)
         cls._check_arch_support(arch_key)
 
         model = cls._get_hqq_class(arch_key).from_quantized(
             save_dir,
             compute_dtype=compute_dtype,
             device=device,
```

### Comparing `hqq-0.1.7.post1/hqq/engine/hf.py` & `hqq-0.1.7.post2/hqq/engine/hf.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/engine/timm.py` & `hqq-0.1.7.post2/hqq/engine/timm.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/engine/vllm.py` & `hqq-0.1.7.post2/hqq/engine/vllm.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/kernels/hqq_aten_cuda.cpp` & `hqq-0.1.7.post2/hqq/kernels/hqq_aten_cuda.cpp`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/kernels/hqq_aten_cuda_kernel.cu` & `hqq-0.1.7.post2/hqq/kernels/hqq_aten_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/kernels/hqq_aten_torch.cpp` & `hqq-0.1.7.post2/hqq/kernels/hqq_aten_torch.cpp`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/models/base.py` & `hqq-0.1.7.post2/hqq/models/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 from torch import nn
 from torch import float16
 from os.path import join as pjoin
 from typing import Callable
 from tqdm import tqdm
 from abc import abstractmethod
 from functools import partial
+from typing import Union
 
 from huggingface_hub import snapshot_download
 from ..core.quantize import HQQLinear
-from ..core.peft import PeftUtils
+from ..core.peft import PeftUtils, _HQQ_LORA_CLASSES
+
 
 # Defined what is qualified as "linear layer"
-_QUANT_LAYERS = [nn.Linear]
+_QUANT_LAYERS = [nn.Linear, HQQLinear] + _HQQ_LORA_CLASSES
 _IGNORE_LINEAR = ["lm_head"]
 
 
 # Cleanup GPU vram
 def cleanup() -> None:
     torch.cuda.empty_cache()
     gc.collect()
@@ -68,21 +70,25 @@
             linear_tags.add(name_to_linear_tag(name))
     return list(linear_tags)
 
 
 def forward_device_hooked(self, *args, **kwargs):
     args = list(args)
 
-    #eddit this to make torch.compile compatible
+    # eddit this to make torch.compile compatible
     for i in range(len(args)):
-        if(isinstance(args[i], (torch.Tensor, torch.nn.Parameter))):#if hasattr(args[i], "to"):
+        if isinstance(
+            args[i], (torch.Tensor, torch.nn.Parameter)
+        ):  # if hasattr(args[i], "to"):
             args[i] = args[i].to(self.device)
 
     for i in kwargs:
-        if(isinstance(kwargs[i], (torch.Tensor, torch.nn.Parameter))):#if hasattr(kwargs[i], "to"):
+        if isinstance(
+            kwargs[i], (torch.Tensor, torch.nn.Parameter)
+        ):  # if hasattr(kwargs[i], "to"):
             kwargs[i] = kwargs[i].to(self.device)
 
     # return self.__class__.forward(self, *args, **kwargs)
     return self.forward_orig(*args, **kwargs)
 
 
 # Base patching class. Patching defines how nn.Linear and other layers are replaced via a patching function.
@@ -104,18 +110,24 @@
         for name in tqdm(tmp_mapping, disable=not verbose):
             setattr(
                 find_parent(model, name),
                 name.split(".")[-1],
                 patch_fct(tmp_mapping[name]),
             )
 
+        cleanup()
+
     # This method iterates through layers of the model that are nn.Linear and processes them via new_nodule = patch_fct(module, params)
     @classmethod
     def patch_linearlayers(
-        cls, model, patch_fct: Callable, patch_params: dict | None, verbose: bool = True
+        cls,
+        model,
+        patch_fct: Callable,
+        patch_params: Union[dict, None],
+        verbose: bool = True,
     ) -> None:
         ignore_tags = cls.get_ignore_layers(model)
 
         tmp_mapping = {}
         for name, module in model.named_modules():
             if (type(module) in _QUANT_LAYERS) and (name not in ignore_tags):
                 tmp_mapping[name] = module
@@ -127,21 +139,28 @@
             )
             setattr(
                 find_parent(model, name),
                 name.split(".")[-1],
                 patch_fct(tmp_mapping[name], patch_param),
             )
 
+        cleanup()
+
     ############################################
     # These tags are used to specfiy parameters of the patching in patch_linearlayers()
     @classmethod
     def set_auto_linear_tags(cls, model, ignore: list = _IGNORE_LINEAR) -> None:
-        if len(cls.get_linear_tags()) == 0:
-            cls.linear_tags = get_linear_tags_from_model(model, ignore=ignore)
-            cls.get_linear_tags = lambda: cls.linear_tags
+        if hasattr(model, "linear_tags") is False:
+            linear_tags = cls.get_linear_tags()
+            model.linear_tags = (
+                linear_tags
+                if len(linear_tags) > 0
+                else get_linear_tags_from_model(model, ignore=ignore)
+            )
+            model.base_class = cls
 
     # Returns the current linear tags
     @classmethod
     def get_linear_tags(cls) -> list:
         return []
 
     @classmethod
@@ -213,38 +232,47 @@
     # Save weights to disk
     @classmethod
     def save_weights(cls, weights: dict, save_dir: str) -> None:
         torch.save(weights, cls.get_weight_file(save_dir))
 
     # Load weights from disk
     @classmethod
-    def load_weights(cls, save_dir: str, map_location: bool = None):
+    def load_weights(cls, save_dir: str, map_location=None):
         return torch.load(cls.get_weight_file(save_dir), map_location=map_location)
 
+    # Set-up model with the necessary data
+    @classmethod
+    def setup_model(cls, model):
+        cls.autoname_modules(model)
+        cls.set_auto_linear_tags(model)
+
     # Main function to quantize a model. Basically goes through the linear layers specfied in the patching function and replaces them with HQQLinear
     @classmethod
     def quantize_model(
         cls,
         model,
         quant_config: dict,
         compute_dtype: torch.dtype = float16,
-        device: str | list | dict = "cuda",
+        device: Union[str, list, dict] = "cuda",
     ):
+        if hasattr(model, "hqq_quantized"):
+            print("Model was already quantized")
+            return
+
         # Set linear tags automatically
-        cls.autoname_modules(model)
-        cls.set_auto_linear_tags(model)
+        cls.setup_model(model)
 
         # Use the same quantization config for all linear layers. Use None to skip quantizing a specfic layer.
-        if True in [(key in cls.get_linear_tags()) for key in quant_config.keys()]:
+        if True in [(key in model.linear_tags) for key in quant_config.keys()]:
             # If the user doesn't specify a key from get_linear_tags, the layer is not quantized via (key, None)
-            patch_params = {key: None for key in cls.get_linear_tags()}
+            patch_params = {key: None for key in model.linear_tags}
             patch_params.update(quant_config)
         else:
             # Same quant_config for all layers
-            patch_params = {k: quant_config for k in cls.get_linear_tags()}
+            patch_params = {k: quant_config for k in model.linear_tags}
 
         # Get list of all nodes in order
         all_nodes = get_all_children_from_model(model, [])  # ordered nodes
         try:
             # Extract block names: This is following Hugging Face models.
             num_blocks = (
                 len(model.model.layers)
@@ -256,15 +284,15 @@
             all_blocks = None
             print(
                 "Default model structure not supported. Make sure you feed device as dictionary as {name_block: device}"
             )
 
         if isinstance(
             device, dict
-        ):  # input as {module block name (str): device (str | torch.device)}
+        ):  # input as {module block name (str): device (str or torch.device)}
             device_map = device
             num_devices = len(set([device_map[k] for k in device_map]))
             all_blocks = list(device_map.keys())
 
         node_to_block = {}
         for node in all_nodes:
             res = [block for block in all_blocks if (block in node)]
@@ -298,14 +326,17 @@
 
         # Map nodes to block devices
         for node in all_nodes:
             device_map[node] = device_map[node_to_block[node]]
 
         # We replace the nn.Linear layers with HQQLinear
         def _patch_linear(linear_layer, quant_config):
+            if type(linear_layer) is HQQLinear:
+                return linear_layer
+
             current_device = device_map[linear_layer.name]
 
             if quant_config is not None:
                 out_module = HQQLinear(
                     linear_layer,
                     quant_config,
                     compute_dtype=compute_dtype,
@@ -343,14 +374,16 @@
                 core_model.layers[i].forward = partial(
                     forward_device_hooked, core_model.layers[i]
                 )
 
         # Set base class
         model.base_class = cls
 
+        model.hqq_quantized = True
+
         # Sync
         torch.cuda.synchronize()
 
         return model
 
     # Prepares model weights by iterating through modules. It might some parameters that are NOT modules like model.param1
     @classmethod
@@ -379,16 +412,21 @@
         # Serialization
         weights = cls.serialize_weights(model, verbose=verbose)
 
         # Save
         cls.save_weights(weights, save_dir)
 
     @classmethod
-    def try_snapshot_download(cls, save_dir_or_hub: str, cache_dir: str = ""):
-        save_dir = pjoin(cache_dir, save_dir_or_hub)
+    def try_snapshot_download(
+        cls, save_dir_or_hub: str, cache_dir: Union[str, None] = ""
+    ):
+        if cache_dir is None:
+            save_dir = pjoin("", save_dir_or_hub)
+        else:
+            save_dir = pjoin(cache_dir, save_dir_or_hub)
 
         if not os.path.exists(save_dir):
             save_dir = snapshot_download(repo_id=save_dir_or_hub, cache_dir=cache_dir)
             save_dir = pjoin(save_dir)
 
         # Check
         if not os.path.exists(cls.get_weight_file(save_dir)):
@@ -406,31 +444,28 @@
     # Main function to load an HQQ quantized model from either HF hub or locally
     @classmethod
     def from_quantized(
         cls,
         save_dir_or_hub,
         compute_dtype: torch.dtype = float16,
         device="cuda",
-        cache_dir: str = "",
+        cache_dir: Union[str, None] = "",
         adapter: str = None,
     ):
         # Get directory path
         save_dir = cls.try_snapshot_download(save_dir_or_hub, cache_dir)
 
         # Load model from config
         model = cls.create_model(save_dir)
 
         # Track save directory
         model.save_dir = save_dir
 
         # Name the layers
-        cls.autoname_modules(model)
-
-        # Set linear tags automatically
-        cls.set_auto_linear_tags(model)
+        cls.setup_model(model)
 
         # Load weights
         try:
             weights = cls.load_weights(save_dir)
         except Exception:
             print("Failed to load the weights")
             raise FileNotFoundError
@@ -463,20 +498,22 @@
                         ),
                     )
 
             return module
 
         # Load modules
         cls.patch_model(
-            model, _load_module, _load_module, {k: None for k in cls.get_linear_tags()}
+            model, _load_module, _load_module, {k: None for k in model.linear_tags}
         )
 
         # Load other weights that are not part of any module
         cls.post_module_load(model, weights)
 
+        model.hqq_quantized = True
+
         # Set base class
         model.base_class = cls
 
         # Add adapter
         if adapter is not None:
             try:
                 PeftUtils.load_lora_weights(model, filename=pjoin(save_dir, adapter))
```

### Comparing `hqq-0.1.7.post1/hqq/models/hf/base.py` & `hqq-0.1.7.post2/hqq/models/hf/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,23 @@
     # Save model architecture
     @classmethod
     def cache_model(cls, model, save_dir):
         model.config.save_pretrained(save_dir)
 
     # Create empty model from config
     @classmethod
-    def create_model(cls, save_dir):
-        config = transformers.AutoConfig.from_pretrained(cls.get_config_file(save_dir))
+    def create_model(cls, save_dir, kwargs):
+        config_kwargs = {}
+        for key in ["attn_implementation"]:
+            if key in kwargs:
+                config_kwargs[key] = kwargs[key]
+
+        config = transformers.AutoConfig.from_pretrained(
+            cls.get_config_file(save_dir), **config_kwargs
+        )
 
         auto_class = transformers.AutoModel
 
         # Todo: add support for other auto models
         archs = config.architectures
         if len(archs) == 1 and ("CausalLM" in archs[0]):
             auto_class = transformers.AutoModelForCausalLM
```

### Comparing `hqq-0.1.7.post1/hqq/models/hf/llama.py` & `hqq-0.1.7.post2/hqq/models/hf/llama.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/models/hf/mistral.py` & `hqq-0.1.7.post2/hqq/models/hf/mistral.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/models/hf/mixtral.py` & `hqq-0.1.7.post2/hqq/models/hf/mixtral.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/models/hf/phi.py` & `hqq-0.1.7.post2/hqq/models/hf/phi.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/models/hf/phi_opt.py` & `hqq-0.1.7.post2/hqq/models/hf/phi_opt.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/models/timm/base.py` & `hqq-0.1.7.post2/hqq/models/timm/base.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/models/timm/vit_clip.py` & `hqq-0.1.7.post2/hqq/models/timm/vit_clip.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/models/vllm/base.py` & `hqq-0.1.7.post2/hqq/models/vllm/base.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/models/vllm/llama.py` & `hqq-0.1.7.post2/hqq/models/vllm/llama.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/utils/generation_hf.py` & `hqq-0.1.7.post2/hqq/utils/generation_hf.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/hqq/utils/patching.py` & `hqq-0.1.7.post2/hqq/utils/patching.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,161 +1,181 @@
 # Written by Dr. Hicham Badri @Mobius Labs GmbH - 2024
 #####################################################
 import torch
 from torch import Tensor
 from ..core.quantize import Quantizer, HQQLinear
 from ..core.utils import cleanup
 from ..core.peft import HQQLinearLoRA
-
+from ..models.hf.base import AutoHQQHFModel
 from ..backends.torchao import patch_hqq_to_aoint4
 from ..backends.marlin import patch_hqq_to_marlin
 
+
 def patch_linearlayers(model, fct, patch_param=None, verbse=False):
-    model.base_class.patch_linearlayers(model, fct, dict([(k, patch_param) for k in model.base_class.get_linear_tags()]), verbose=verbse)
+    base_class = model.base_class if (hasattr(model, "base_class")) else AutoHQQHFModel
+    base_class.setup_model(model)
+    model.base_class.patch_linearlayers(
+        model, fct, dict([(k, patch_param) for k in model.linear_tags]), verbose=verbse
+    )
+
 
 def patch_add_quant_config(layer, patch_param):
-    if(type(layer) is HQQLinear):
+    if type(layer) is HQQLinear:
         layer.quant_config = patch_param
-    if(type(layer) is HQQLinearLoRA):
+    if type(layer) is HQQLinearLoRA:
         layer.linear_layer.quant_config = patch_param
     return layer
 
-#add dummy weights to a layer
-def patch_add_weight_param(layer, patch_param): 
-    if(hasattr(layer, 'weight') is False):
-        if(hasattr(layer, 'device')):
+
+# add dummy weights to a layer
+def patch_add_weight_param(layer, patch_param):
+    if hasattr(layer, "weight") is False:
+        if hasattr(layer, "device"):
             device_ = layer.device
         else:
-            param  = [p for p in layer.parameters()]
-            device_ = param[0].device if(len(param)>0) else patch_param["device"]
+            param = [p for p in layer.parameters()]
+            device_ = param[0].device if (len(param) > 0) else patch_param["device"]
 
         fp_param = [p for p in layer.parameters() if p.is_floating_point()]
-        dtype_ = fp_param[0].dtype if(len(fp_param)>0) else patch_param["dtype"]
+        dtype_ = fp_param[0].dtype if (len(fp_param) > 0) else patch_param["dtype"]
 
-        layer.weight = torch.nn.Parameter(torch.zeros((1,), device=device_, dtype=dtype_), requires_grad=False)
+        layer.weight = torch.nn.Parameter(
+            torch.zeros((1,), device=device_, dtype=dtype_), requires_grad=False
+        )
     return layer
 
-#Optimize HQQLinear.forward for inference
+
+# Optimize HQQLinear.forward for inference
 def patch_hqq_inference(layer, patch_param):
     def forward_hqq_inferece(self, x):
-        out = torch.matmul(x, self.dequantize().T) #TODO GEMV use-case
-        if(self.bias is not None):
-            out += self.bias 
-        return out 
+        out = torch.matmul(x, self.dequantize().T)  # TODO GEMV use-case
+        if self.bias is not None:
+            out += self.bias
+        return out
 
-    if(type(layer) is HQQLinear):
+    if type(layer) is HQQLinear:
         layer.forward = lambda x: forward_hqq_inferece(layer, x)
 
-    if(type(layer) is HQQLinearLoRA):
-        if(type(layer.linear_layer) is HQQLinear):
-            layer.linear_layer.forward = lambda x: forward_hqq_inferece(layer.linear_layer, x)
+    if type(layer) is HQQLinearLoRA:
+        if type(layer.linear_layer) is HQQLinear:
+            layer.linear_layer.forward = lambda x: forward_hqq_inferece(
+                layer.linear_layer, x
+            )
 
     return layer
 
-#Optimize HQQLinearLoRA.forward for inference
+
+# Optimize HQQLinearLoRA.forward for inference
 def patch_lora_inference(layer, patch_param):
     def forward_lora_inference(self, x):
-        out = torch.matmul(torch.matmul(x, self.lora_A), self.lora_B)* self.scaling
-        return out 
-                
-    if(type(layer) is HQQLinearLoRA):
+        out = torch.matmul(torch.matmul(x, self.lora_A), self.lora_B) * self.scaling
+        return out
+
+    if type(layer) is HQQLinearLoRA:
         layer.forward_lora = lambda x: forward_lora_inference(layer, x)
     return layer
 
 
 def prepare_for_inference(model, allow_merge=False, backend="default"):
-
-    if(backend =="torchao_int4"):
+    if backend == "torchao_int4":
         allow_merge = False
 
     patch_linearlayers(model, patch_hqq_inference)
     patch_linearlayers(model, patch_lora_inference)
+    cleanup()
 
-    if(backend =="torchao_int4"):
+    if backend == "torchao_int4":
         patch_linearlayers(model, patch_hqq_to_aoint4)
-    if(allow_merge): #only compatible with symmetric quant kernels
-        patch_linearlayers(model, patch_merge_zeros_with_lora, {'z_shift':8, 'keep_lora':False})
-    if(backend =="marlin"):
+        cleanup()
+    if allow_merge:  # only compatible with symmetric quant kernels
+        patch_linearlayers(
+            model, patch_merge_zeros_with_lora, {"z_shift": 8, "keep_lora": False}
+        )
+        cleanup()
+    if backend == "marlin":
         patch_linearlayers(model, patch_hqq_to_marlin, verbse=True)
+        cleanup()
 
-    patch_linearlayers(model, patch_add_weight_param, {"device":model.device, "dtype":model.dtype})
+    patch_linearlayers(
+        model, patch_add_weight_param, {"device": model.device, "dtype": model.dtype}
+    )
     cleanup()
 
+
 def get_lowrank_tuple_torch_gpu(tensor, max_rank, eps=None):
-    t       = tensor.t().float()
+    t = tensor.t().float()
     u, s, v = torch.linalg.svd(t)
-    u, s, v = u[:,:max_rank], s[:max_rank], v[:max_rank, :]
-    us      = torch.matmul(u, torch.diag(s))
-    A, B    = (v.t(), us.t()) #t ~ AB
-    if(eps is not None):
-        A  = A.clamp(min=-eps, max=eps)
-        B   = B.clamp(min=-eps, max=eps)
+    u, s, v = u[:, :max_rank], s[:max_rank], v[:max_rank, :]
+    us = torch.matmul(u, torch.diag(s))
+    A, B = (v.t(), us.t())  # t ~ AB
+    if eps is not None:
+        A = A.clamp(min=-eps, max=eps)
+        B = B.clamp(min=-eps, max=eps)
     return A.to(tensor.dtype), B.to(tensor.dtype)
 
 
-#Merges HQQ's zeros with LoRA weights. ONLY works with group_size=None and axis=1
-def patch_merge_zeros_with_lora(layer, patch_params={'z_shift':8, 'keep_lora':False}):
-    if(type(layer) is HQQLinearLoRA):
-
-        #Check config suppport
-        w_q_config = layer.linear_layer.quant_config['weight_quant_params']
-        if((w_q_config['axis']==0) or (w_q_config['group_size'] is not None)):
+# Merges HQQ's zeros with LoRA weights. ONLY works with group_size=None and axis=1
+def patch_merge_zeros_with_lora(layer, patch_params={"z_shift": 8, "keep_lora": False}):
+    if type(layer) is HQQLinearLoRA:
+        # Check config suppport
+        hqq_layer = layer.linear_layer
+        if (hqq_layer.meta["axis"] == 0) or (hqq_layer.meta["group_size"] is not None):
+            print('Skipping zeros lora merging for', layer.name)
             return layer
 
-        layer.z_shift   = patch_params['z_shift']
-        layer.keep_lora = patch_params['keep_lora']
-        
-        shape = layer.linear_layer.meta['shape']
-        z     = layer.linear_layer.meta['zero']
-        s     = layer.linear_layer.meta['scale']
-        u     = (s*(-z + layer.z_shift)).flatten().view([1, -1])
-        
+        layer.z_shift = patch_params["z_shift"]
+        layer.keep_lora = patch_params["keep_lora"]
+
+        shape = layer.linear_layer.meta["shape"]
+        z = layer.linear_layer.meta["zero"]
+        s = layer.linear_layer.meta["scale"]
+        u = (s * (-z + layer.z_shift)).flatten().view([1, -1])
+
         ###########################################
-        if(layer.keep_lora is False):
-            A, B  = layer.lora_A.data, layer.lora_B.data
-            onz   = torch.ones((shape[1], 1), device=u.device, dtype=u.dtype) 
+        if layer.keep_lora is False:
+            A, B = layer.lora_A.data, layer.lora_B.data
+            onz = torch.ones((shape[1], 1), device=u.device, dtype=u.dtype)
 
-            #Cat
+            # Cat
             A = torch.cat([A, onz], axis=1)
-            B = torch.cat([B,   u], axis=0)
+            B = torch.cat([B, u], axis=0)
 
             # #Re-rank
             # #A, B = get_lowrank_tuple_torch_gpu(torch.matmul(A, B) + torch.matmul(onz, u), max_rank=layer.r + 1)
 
             layer.lora_A.data = A.to(dtype=layer.lora_A.dtype)
             layer.lora_B.data = B.to(dtype=layer.lora_B.dtype)
 
             layer.u = None
 
         else:
             layer.u = torch.nn.Parameter(u, requires_grad=False)
         ###########################################
-        layer.linear_layer.meta['zero']  = 0.
+        layer.linear_layer.meta["zero"] = 0.0
 
         torch.cuda.empty_cache()
 
         def forward_linear_updated(self, x: Tensor) -> Tensor:
-
             compute_dtype = self.linear_layer.compute_dtype
-            meta          = self.linear_layer.meta 
-            W_q           = self.linear_layer.W_q 
+            meta = self.linear_layer.meta
+            W_q = self.linear_layer.W_q
 
-            W_r           = Quantizer.unpack[meta["packing"]](W_q, dtype=compute_dtype).t()
-            scale         = meta['scale'].t()
+            W_r = Quantizer.unpack[meta["packing"]](W_q, dtype=compute_dtype).t()
+            scale = meta["scale"].t()
 
-            out           = torch.matmul(x, (W_r - self.z_shift))*scale #Symmetric quant
+            out = torch.matmul(x, (W_r - self.z_shift)) * scale  # Symmetric quant
             return out
 
         layer.linear_layer.forward = lambda x: forward_linear_updated(layer, x)
 
         def forward_updated(self, x: Tensor) -> Tensor:
-            out  = self.linear_layer.forward(x)
+            out = self.linear_layer.forward(x)
 
-            if(self.u is not None):
+            if self.u is not None:
                 out += torch.matmul(x.sum(axis=-1, keepdim=True), self.u)
 
             out += self.forward_lora(x) + self.bias
             return out
 
         layer.forward = lambda x: forward_updated(layer, x)
 
-    return layer
+    return layer
```

### Comparing `hqq-0.1.7.post1/hqq.egg-info/SOURCES.txt` & `hqq-0.1.7.post2/hqq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/setup.py` & `hqq-0.1.7.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def run(self):
         egg_info.run(self)
         run_setup_cuda()
 
 
 setup(
     name="hqq",
-    version="0.1.7.post1",
+    version="0.1.7.post2",
     description="Half-Quadratic Quantization (HQQ)",
     url="https://github.com/mobiusml/hqq/",
     author="Dr. Hicham Badri",
     author_email="hicham@mobiuslabs.com",
     license="Apache 2",
     packages=find_packages(include=["hqq", "hqq.*"]),
     package_data={
```

### Comparing `hqq-0.1.7.post1/tests/test_bitpack.py` & `hqq-0.1.7.post2/tests/test_bitpack.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post1/tests/test_quantize.py` & `hqq-0.1.7.post2/tests/test_quantize.py`

 * *Files identical despite different names*

