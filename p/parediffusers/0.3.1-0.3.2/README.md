# Comparing `tmp/parediffusers-0.3.1.tar.gz` & `tmp/parediffusers-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parediffusers-0.3.1.tar", last modified: Wed Jan 17 08:19:31 2024, max compression
+gzip compressed data, was "parediffusers-0.3.2.tar", last modified: Mon May  6 02:05:01 2024, max compression
```

## Comparing `parediffusers-0.3.1.tar` & `parediffusers-0.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2024-01-17 08:19:31.804084 parediffusers-0.3.1/
--rw-r--r--   0 masaishi   (501) staff       (20)     5113 2024-01-17 08:19:31.803972 parediffusers-0.3.1/PKG-INFO
--rw-r--r--   0 masaishi   (501) staff       (20)     4641 2024-01-17 07:57:54.000000 parediffusers-0.3.1/README.md
--rw-r--r--   0 masaishi   (501) staff       (20)       38 2024-01-17 08:19:31.804123 parediffusers-0.3.1/setup.cfg
--rw-r--r--   0 masaishi   (501) staff       (20)      756 2024-01-17 08:19:16.000000 parediffusers-0.3.1/setup.py
-drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2024-01-17 08:19:31.799125 parediffusers-0.3.1/src/
-drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2024-01-17 08:19:31.800728 parediffusers-0.3.1/src/parediffusers/
--rw-r--r--   0 masaishi   (501) staff       (20)      208 2024-01-17 08:19:12.000000 parediffusers-0.3.1/src/parediffusers/__init__.py
--rw-r--r--   0 masaishi   (501) staff       (20)     3237 2024-01-17 07:58:51.000000 parediffusers-0.3.1/src/parediffusers/defaults.py
-drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2024-01-17 08:19:31.803644 parediffusers-0.3.1/src/parediffusers/models/
--rw-r--r--   0 masaishi   (501) staff       (20)      257 2024-01-17 07:59:59.000000 parediffusers-0.3.1/src/parediffusers/models/__init__.py
--rw-r--r--   0 masaishi   (501) staff       (20)    12962 2024-01-17 07:57:54.000000 parediffusers-0.3.1/src/parediffusers/models/attension.py
--rw-r--r--   0 masaishi   (501) staff       (20)     2608 2024-01-17 07:57:54.000000 parediffusers-0.3.1/src/parediffusers/models/embeddings.py
--rw-r--r--   0 masaishi   (501) staff       (20)     2965 2024-01-17 07:58:09.000000 parediffusers-0.3.1/src/parediffusers/models/resnet.py
--rw-r--r--   0 masaishi   (501) staff       (20)     9541 2024-01-17 07:57:54.000000 parediffusers-0.3.1/src/parediffusers/models/transformer.py
--rw-r--r--   0 masaishi   (501) staff       (20)     5434 2024-01-17 07:57:54.000000 parediffusers-0.3.1/src/parediffusers/models/transformer_blocks.py
--rw-r--r--   0 masaishi   (501) staff       (20)    15707 2024-01-17 07:58:09.000000 parediffusers-0.3.1/src/parediffusers/models/unet_2d_blocks.py
--rw-r--r--   0 masaishi   (501) staff       (20)     4450 2024-01-17 07:58:09.000000 parediffusers-0.3.1/src/parediffusers/models/unet_2d_get_blocks.py
--rw-r--r--   0 masaishi   (501) staff       (20)     5430 2024-01-17 08:05:36.000000 parediffusers-0.3.1/src/parediffusers/models/unet_2d_mid_blocks.py
--rw-r--r--   0 masaishi   (501) staff       (20)     7024 2024-01-17 08:17:11.000000 parediffusers-0.3.1/src/parediffusers/models/vae_blocks.py
--rw-r--r--   0 masaishi   (501) staff       (20)     5595 2024-01-17 08:18:23.000000 parediffusers-0.3.1/src/parediffusers/pipeline.py
--rw-r--r--   0 masaishi   (501) staff       (20)     2358 2024-01-17 07:57:54.000000 parediffusers-0.3.1/src/parediffusers/scheduler.py
--rw-r--r--   0 masaishi   (501) staff       (20)    11606 2024-01-17 08:04:24.000000 parediffusers-0.3.1/src/parediffusers/unet.py
--rw-r--r--   0 masaishi   (501) staff       (20)      531 2024-01-17 07:57:54.000000 parediffusers-0.3.1/src/parediffusers/utils.py
--rw-r--r--   0 masaishi   (501) staff       (20)     3726 2024-01-17 08:06:39.000000 parediffusers-0.3.1/src/parediffusers/vae.py
-drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2024-01-17 08:19:31.801423 parediffusers-0.3.1/src/parediffusers.egg-info/
--rw-r--r--   0 masaishi   (501) staff       (20)     5113 2024-01-17 08:19:31.000000 parediffusers-0.3.1/src/parediffusers.egg-info/PKG-INFO
--rw-r--r--   0 masaishi   (501) staff       (20)      833 2024-01-17 08:19:31.000000 parediffusers-0.3.1/src/parediffusers.egg-info/SOURCES.txt
--rw-r--r--   0 masaishi   (501) staff       (20)        1 2024-01-17 08:19:31.000000 parediffusers-0.3.1/src/parediffusers.egg-info/dependency_links.txt
--rw-r--r--   0 masaishi   (501) staff       (20)       60 2024-01-17 08:19:31.000000 parediffusers-0.3.1/src/parediffusers.egg-info/requires.txt
--rw-r--r--   0 masaishi   (501) staff       (20)       14 2024-01-17 08:19:31.000000 parediffusers-0.3.1/src/parediffusers.egg-info/top_level.txt
+drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2024-05-06 02:05:01.340274 parediffusers-0.3.2/
+-rw-r--r--   0 masaishi   (501) staff       (20)     6190 2024-05-06 02:05:01.340067 parediffusers-0.3.2/PKG-INFO
+-rw-r--r--   0 masaishi   (501) staff       (20)     5738 2024-04-29 09:48:41.000000 parediffusers-0.3.2/README.md
+-rw-r--r--   0 masaishi   (501) staff       (20)       38 2024-05-06 02:05:01.340326 parediffusers-0.3.2/setup.cfg
+-rw-r--r--   0 masaishi   (501) staff       (20)      816 2024-05-05 22:08:42.000000 parediffusers-0.3.2/setup.py
+drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2024-05-06 02:05:01.332541 parediffusers-0.3.2/src/
+drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2024-05-06 02:05:01.335110 parediffusers-0.3.2/src/parediffusers/
+-rw-r--r--   0 masaishi   (501) staff       (20)      209 2024-05-05 22:08:42.000000 parediffusers-0.3.2/src/parediffusers/__init__.py
+-rw-r--r--   0 masaishi   (501) staff       (20)     3749 2024-05-05 22:08:42.000000 parediffusers-0.3.2/src/parediffusers/defaults.py
+drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2024-05-06 02:05:01.339628 parediffusers-0.3.2/src/parediffusers/models/
+-rw-r--r--   0 masaishi   (501) staff       (20)      258 2024-05-05 22:08:42.000000 parediffusers-0.3.2/src/parediffusers/models/__init__.py
+-rw-r--r--   0 masaishi   (501) staff       (20)    13459 2024-05-05 22:08:42.000000 parediffusers-0.3.2/src/parediffusers/models/attension.py
+-rw-r--r--   0 masaishi   (501) staff       (20)     3029 2024-05-05 22:08:42.000000 parediffusers-0.3.2/src/parediffusers/models/embeddings.py
+-rw-r--r--   0 masaishi   (501) staff       (20)     3517 2024-05-05 22:08:42.000000 parediffusers-0.3.2/src/parediffusers/models/resnet.py
+-rw-r--r--   0 masaishi   (501) staff       (20)    12423 2024-05-05 22:08:42.000000 parediffusers-0.3.2/src/parediffusers/models/transformer.py
+-rw-r--r--   0 masaishi   (501) staff       (20)     6662 2024-05-05 22:08:42.000000 parediffusers-0.3.2/src/parediffusers/models/transformer_blocks.py
+-rw-r--r--   0 masaishi   (501) staff       (20)    22613 2024-05-05 22:08:42.000000 parediffusers-0.3.2/src/parediffusers/models/unet_2d_blocks.py
+-rw-r--r--   0 masaishi   (501) staff       (20)     5863 2024-05-05 22:08:42.000000 parediffusers-0.3.2/src/parediffusers/models/unet_2d_get_blocks.py
+-rw-r--r--   0 masaishi   (501) staff       (20)     7136 2024-05-05 22:08:42.000000 parediffusers-0.3.2/src/parediffusers/models/unet_2d_mid_blocks.py
+-rw-r--r--   0 masaishi   (501) staff       (20)     8039 2024-05-05 22:08:42.000000 parediffusers-0.3.2/src/parediffusers/models/vae_blocks.py
+-rw-r--r--   0 masaishi   (501) staff       (20)     6666 2024-05-05 22:08:42.000000 parediffusers-0.3.2/src/parediffusers/pipeline.py
+-rw-r--r--   0 masaishi   (501) staff       (20)     2923 2024-05-05 22:08:42.000000 parediffusers-0.3.2/src/parediffusers/scheduler.py
+-rw-r--r--   0 masaishi   (501) staff       (20)    14534 2024-05-05 22:08:42.000000 parediffusers-0.3.2/src/parediffusers/unet.py
+-rw-r--r--   0 masaishi   (501) staff       (20)      582 2024-05-05 22:08:42.000000 parediffusers-0.3.2/src/parediffusers/utils.py
+-rw-r--r--   0 masaishi   (501) staff       (20)     4482 2024-05-05 22:08:42.000000 parediffusers-0.3.2/src/parediffusers/vae.py
+drwxr-xr-x   0 masaishi   (501) staff       (20)        0 2024-05-06 02:05:01.336397 parediffusers-0.3.2/src/parediffusers.egg-info/
+-rw-r--r--   0 masaishi   (501) staff       (20)     6190 2024-05-06 02:05:01.000000 parediffusers-0.3.2/src/parediffusers.egg-info/PKG-INFO
+-rw-r--r--   0 masaishi   (501) staff       (20)      833 2024-05-06 02:05:01.000000 parediffusers-0.3.2/src/parediffusers.egg-info/SOURCES.txt
+-rw-r--r--   0 masaishi   (501) staff       (20)        1 2024-05-06 02:05:01.000000 parediffusers-0.3.2/src/parediffusers.egg-info/dependency_links.txt
+-rw-r--r--   0 masaishi   (501) staff       (20)       60 2024-05-06 02:05:01.000000 parediffusers-0.3.2/src/parediffusers.egg-info/requires.txt
+-rw-r--r--   0 masaishi   (501) staff       (20)       14 2024-05-06 02:05:01.000000 parediffusers-0.3.2/src/parediffusers.egg-info/top_level.txt
```

### Comparing `parediffusers-0.3.1/PKG-INFO` & `parediffusers-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,28 @@
-Metadata-Version: 2.1
-Name: parediffusers
-Version: 0.3.1
-Summary: The library `pared` down the features of `diffusers` implemented the minimum function to generate images without using huggingface/diffusers to understand the inner workings of the library.
-Home-page: https://github.com/masaishi/parediffusers
-Author: Masamune Ishihara
-Author-email: mwishiha@ucsc.edu
-License: MIT License
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # PareDiffusers
 
+[![Screenshot 2024-01-17 at 10 53 49 PM](https://github.com/masaishi/parediffusers/assets/1396267/c02bd298-c894-4fb6-b17a-a72f1b736748)](https://github.com/masaishi/parediffusers/blob/main/src/parediffusers/pipeline.py)
+
 [![parediffusers on PyPI](https://img.shields.io/pypi/v/parediffusers.svg)](https://pypi.org/project/parediffusers)
 
-The library `pared` down the features of `diffusers` implemented the minimum function to generate images without using [huggingface/diffusers](https://github.com/huggingface/diffusers/tree/main) to understand the inner workings of the library.
+The library `pared` down the features of `diffusers` implemented the minimum function to generate images without using [huggingface/diffusers](https://github.com/huggingface/diffusers/tree/main) functions to understand the inner workings of the library.
 
 
 ## Why PareDiffusers?
 PareDiffusers was born out of a curiosity and a desire to demystify the processes of generating images by diffusion models and the workings of the diffusers library.
 
 I will write blog-style [notebooks](./notebooks) understanding how works using a top-down approach. First, generate images using diffusers to understand the overall flow, then gradually replace code with Pytorch code. In the end, we will write the code for the [PareDiffusers code](./src/parediffusers) that does not include diffusers code.
 
 I hope that it helps others who share a similar interest in the inner workings of image generation.
 
 ## Versions
 - v0.0.0: After Ch0.0.0, inprement StableDiffusionPipeline.
 - v0.1.2: After Ch0.1.0, imprement DDIMScheduler.
 - v0.2.0: After Ch0.2.0, imprement UNet2DConditionModel.
+- v0.3.1: After Ch0.3.0, imprement AutoencoderKL.
 
 ## Table of Contents
 ### [Ch0.0.0 PareDiffusersPipeline](./notebooks/ch0.0.0_ParedDiffusionPipeline.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/masaishi/parediffusers/blob/main/notebooks/ch0.0.0_ParedDiffusionPipeline.ipynb)
 version: v0.0.0
 - [x] Generate images using diffusers
 - [x] Imprement StableDiffusionPipeline
 - [ ] Imprement DDIMScheduler
@@ -55,14 +46,23 @@
 - [x] Generate images using diffusers
 - [x] Imprement StableDiffusionPipeline
 - [x] Imprement DDIMScheduler
 - [x] Imprement UNet2DConditionModel
 - [ ] Imprement AutoencoderKL
 ### [Ch0.2.1: Test parediffusers](./notebooks/ch0.2.1_Test_PareDiffusersPipeline.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/masaishi/parediffusers/blob/main/notebooks/ch0.2.1_Test_PareDiffusersPipeline.ipynb)
 - Test PareDiffusersPipeline by pip install parediffusers.
+### [Ch0.3.0: PareAutoencoderKL](./notebooks/ch0.3.0_PareAutoencoderKL.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/masaishi/parediffusers/blob/main/notebooks/ch0.3.0_PareAutoencoderKL.ipynb)
+version: v0.3.1
+- [x] Generate images using diffusers
+- [x] Imprement StableDiffusionPipeline
+- [x] Imprement DDIMScheduler
+- [x] Imprement UNet2DConditionModel
+- [x] Imprement AutoencoderKL
+### [Ch0.3.1: Test parediffusers](./notebooks/ch0.3.1_Test_PareDiffusersPipeline.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/masaishi/parediffusers/blob/main/notebooks/ch0.3.1_Test_PareDiffusersPipeline.ipynb)
+- Test PareDiffusersPipeline by pip install parediffusers.
 
 
 ## Usage
 ```python
 import torch
 from parediffusers import PareDiffusionPipeline
 
@@ -74,8 +74,7 @@
 prompt = "painting depicting the sea, sunrise, ship, artstation, 4k, concept art"
 image = pipe(prompt)
 display(image)
 ```
 
 ## Contribution
 I am starting this project to help me understand the code in order to participate in diffusers' OSS. So, I think there may be some mistakes in my explanation, so if you find any, please feel free to correct them via an issue or pull request.
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `parediffusers-0.3.1/README.md` & `parediffusers-0.3.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,39 @@
+Metadata-Version: 2.1
+Name: parediffusers
+Version: 0.3.2
+Summary: The library `pared` down the features of `diffusers` implemented the minimum function to generate images without using huggingface/diffusers to understand the inner workings of the library.
+Home-page: https://github.com/masaishi/parediffusers
+Author: Masamune Ishihara
+Author-email: mwishiha@ucsc.edu
+License: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # PareDiffusers
 
+[![Screenshot 2024-01-17 at 10 53 49 PM](https://github.com/masaishi/parediffusers/assets/1396267/c02bd298-c894-4fb6-b17a-a72f1b736748)](https://github.com/masaishi/parediffusers/blob/main/src/parediffusers/pipeline.py)
+
 [![parediffusers on PyPI](https://img.shields.io/pypi/v/parediffusers.svg)](https://pypi.org/project/parediffusers)
 
-The library `pared` down the features of `diffusers` implemented the minimum function to generate images without using [huggingface/diffusers](https://github.com/huggingface/diffusers/tree/main) to understand the inner workings of the library.
+The library `pared` down the features of `diffusers` implemented the minimum function to generate images without using [huggingface/diffusers](https://github.com/huggingface/diffusers/tree/main) functions to understand the inner workings of the library.
 
 
 ## Why PareDiffusers?
 PareDiffusers was born out of a curiosity and a desire to demystify the processes of generating images by diffusion models and the workings of the diffusers library.
 
 I will write blog-style [notebooks](./notebooks) understanding how works using a top-down approach. First, generate images using diffusers to understand the overall flow, then gradually replace code with Pytorch code. In the end, we will write the code for the [PareDiffusers code](./src/parediffusers) that does not include diffusers code.
 
 I hope that it helps others who share a similar interest in the inner workings of image generation.
 
 ## Versions
 - v0.0.0: After Ch0.0.0, inprement StableDiffusionPipeline.
 - v0.1.2: After Ch0.1.0, imprement DDIMScheduler.
 - v0.2.0: After Ch0.2.0, imprement UNet2DConditionModel.
+- v0.3.1: After Ch0.3.0, imprement AutoencoderKL.
 
 ## Table of Contents
 ### [Ch0.0.0 PareDiffusersPipeline](./notebooks/ch0.0.0_ParedDiffusionPipeline.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/masaishi/parediffusers/blob/main/notebooks/ch0.0.0_ParedDiffusionPipeline.ipynb)
 version: v0.0.0
 - [x] Generate images using diffusers
 - [x] Imprement StableDiffusionPipeline
 - [ ] Imprement DDIMScheduler
@@ -43,14 +57,23 @@
 - [x] Generate images using diffusers
 - [x] Imprement StableDiffusionPipeline
 - [x] Imprement DDIMScheduler
 - [x] Imprement UNet2DConditionModel
 - [ ] Imprement AutoencoderKL
 ### [Ch0.2.1: Test parediffusers](./notebooks/ch0.2.1_Test_PareDiffusersPipeline.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/masaishi/parediffusers/blob/main/notebooks/ch0.2.1_Test_PareDiffusersPipeline.ipynb)
 - Test PareDiffusersPipeline by pip install parediffusers.
+### [Ch0.3.0: PareAutoencoderKL](./notebooks/ch0.3.0_PareAutoencoderKL.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/masaishi/parediffusers/blob/main/notebooks/ch0.3.0_PareAutoencoderKL.ipynb)
+version: v0.3.1
+- [x] Generate images using diffusers
+- [x] Imprement StableDiffusionPipeline
+- [x] Imprement DDIMScheduler
+- [x] Imprement UNet2DConditionModel
+- [x] Imprement AutoencoderKL
+### [Ch0.3.1: Test parediffusers](./notebooks/ch0.3.1_Test_PareDiffusersPipeline.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/masaishi/parediffusers/blob/main/notebooks/ch0.3.1_Test_PareDiffusersPipeline.ipynb)
+- Test PareDiffusersPipeline by pip install parediffusers.
 
 
 ## Usage
 ```python
 import torch
 from parediffusers import PareDiffusionPipeline
 
@@ -61,8 +84,8 @@
 pipe = PareDiffusionPipeline.from_pretrained(model_name, device=device, dtype=dtype)
 prompt = "painting depicting the sea, sunrise, ship, artstation, 4k, concept art"
 image = pipe(prompt)
 display(image)
 ```
 
 ## Contribution
-I am starting this project to help me understand the code in order to participate in diffusers' OSS. So, I think there may be some mistakes in my explanation, so if you find any, please feel free to correct them via an issue or pull request.
+I am starting this project to help me understand the code in order to participate in diffusers' OSS. So, I think there may be some mistakes in my explanation, so if you find any, please feel free to correct them via an issue or pull request.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `parediffusers-0.3.1/src/parediffusers/models/attension.py` & `parediffusers-0.3.2/src/parediffusers/models/attension.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import torch
 from torch import nn
 from torch.nn import functional as F
-from typing import Optional, Dict, Any
+from typing import Optional
+
 
 class PareGEGLU(nn.Module):
     def __init__(self, dim_in: int, dim_out: int, bias: bool = True):
         super().__init__()
         linear_cls = nn.Linear
         self.proj = linear_cls(dim_in, dim_out * 2, bias=bias)
 
@@ -66,30 +67,40 @@
         if attn.spatial_norm is not None:
             hidden_states = attn.spatial_norm(hidden_states, temb)
 
         input_ndim = hidden_states.ndim
 
         if input_ndim == 4:
             batch_size, channel, height, width = hidden_states.shape
-            hidden_states = hidden_states.view(batch_size, channel, height * width).transpose(1, 2)
+            hidden_states = hidden_states.view(
+                batch_size, channel, height * width
+            ).transpose(1, 2)
 
         batch_size, sequence_length, _ = (
-            hidden_states.shape if encoder_hidden_states is None else encoder_hidden_states.shape
+            hidden_states.shape
+            if encoder_hidden_states is None
+            else encoder_hidden_states.shape
+        )
+        attention_mask = attn.prepare_attention_mask(
+            attention_mask, sequence_length, batch_size
         )
-        attention_mask = attn.prepare_attention_mask(attention_mask, sequence_length, batch_size)
 
         if attn.group_norm is not None:
-            hidden_states = attn.group_norm(hidden_states.transpose(1, 2)).transpose(1, 2)
+            hidden_states = attn.group_norm(hidden_states.transpose(1, 2)).transpose(
+                1, 2
+            )
 
         query = attn.to_q(hidden_states, *args)
 
         if encoder_hidden_states is None:
             encoder_hidden_states = hidden_states
         elif attn.norm_cross:
-            encoder_hidden_states = attn.norm_encoder_hidden_states(encoder_hidden_states)
+            encoder_hidden_states = attn.norm_encoder_hidden_states(
+                encoder_hidden_states
+            )
 
         key = attn.to_k(encoder_hidden_states, *args)
         value = attn.to_v(encoder_hidden_states, *args)
 
         query = attn.head_to_batch_dim(query)
         key = attn.head_to_batch_dim(key)
         value = attn.head_to_batch_dim(value)
@@ -100,15 +111,17 @@
 
         # linear proj
         hidden_states = attn.to_out[0](hidden_states, *args)
         # dropout
         hidden_states = attn.to_out[1](hidden_states)
 
         if input_ndim == 4:
-            hidden_states = hidden_states.transpose(-1, -2).reshape(batch_size, channel, height, width)
+            hidden_states = hidden_states.transpose(-1, -2).reshape(
+                batch_size, channel, height, width
+            )
 
         if attn.residual_connection:
             hidden_states = hidden_states + residual
 
         hidden_states = hidden_states / attn.rescale_output_factor
 
         return hidden_states
@@ -139,15 +152,17 @@
         _from_deprecated_attn_block: bool = False,
         processor: Optional["PareAttnProcessor"] = None,
         out_dim: int = None,
     ):
         super().__init__()
         self.inner_dim = out_dim if out_dim is not None else dim_head * heads
         self.query_dim = query_dim
-        self.cross_attention_dim = cross_attention_dim if cross_attention_dim is not None else query_dim
+        self.cross_attention_dim = (
+            cross_attention_dim if cross_attention_dim is not None else query_dim
+        )
         self.upcast_attention = upcast_attention
         self.upcast_softmax = upcast_softmax
         self.rescale_output_factor = rescale_output_factor
         self.residual_connection = residual_connection
         self.dropout = dropout
         self.fused_projections = False
         self.out_dim = out_dim if out_dim is not None else query_dim
@@ -160,15 +175,17 @@
         self.heads = out_dim // dim_head if out_dim is not None else heads
         self.sliceable_head_dim = heads
 
         self.added_kv_proj_dim = added_kv_proj_dim
         self.only_cross_attention = only_cross_attention
 
         if norm_num_groups is not None:
-            self.group_norm = nn.GroupNorm(num_channels=query_dim, num_groups=norm_num_groups, eps=eps, affine=True)
+            self.group_norm = nn.GroupNorm(
+                num_channels=query_dim, num_groups=norm_num_groups, eps=eps, affine=True
+            )
         else:
             self.group_norm = None
 
         self.spatial_norm = None
 
         if cross_attention_norm is None:
             self.norm_cross = None
@@ -177,15 +194,18 @@
         elif cross_attention_norm == "group_norm":
             if self.added_kv_proj_dim is not None:
                 norm_cross_num_channels = added_kv_proj_dim
             else:
                 norm_cross_num_channels = self.cross_attention_dim
 
             self.norm_cross = nn.GroupNorm(
-                num_channels=norm_cross_num_channels, num_groups=cross_attention_norm_num_groups, eps=1e-5, affine=True
+                num_channels=norm_cross_num_channels,
+                num_groups=cross_attention_norm_num_groups,
+                eps=1e-5,
+                affine=True,
             )
         else:
             raise ValueError(
                 f"unknown cross_attention_norm: {cross_attention_norm}. Should be None, 'layer_norm' or 'group_norm'"
             )
 
         linear_cls = nn.Linear
@@ -206,23 +226,19 @@
             self.add_v_proj = linear_cls(added_kv_proj_dim, self.inner_dim)
 
         self.to_out = nn.ModuleList([])
         self.to_out.append(linear_cls(self.inner_dim, self.out_dim, bias=out_bias))
         self.to_out.append(nn.Dropout(dropout))
 
         if processor is None:
-            processor = (
-                PareAttnProcessor()
-            )
+            processor = PareAttnProcessor()
         self.set_processor(processor)
 
     def set_attention_slice(self, slice_size: int) -> None:
-        processor = (
-			PareAttnProcessor()
-		)
+        processor = PareAttnProcessor()
         self.set_processor(processor)
 
     def set_processor(self, processor: "PareAttnProcessor") -> None:
         self.processor = processor
 
     def forward(
         self,
@@ -239,39 +255,48 @@
             **cross_attention_kwargs,
         )
 
     def batch_to_head_dim(self, tensor: torch.Tensor) -> torch.Tensor:
         head_size = self.heads
         batch_size, seq_len, dim = tensor.shape
         tensor = tensor.reshape(batch_size // head_size, head_size, seq_len, dim)
-        tensor = tensor.permute(0, 2, 1, 3).reshape(batch_size // head_size, seq_len, dim * head_size)
+        tensor = tensor.permute(0, 2, 1, 3).reshape(
+            batch_size // head_size, seq_len, dim * head_size
+        )
         return tensor
 
     def head_to_batch_dim(self, tensor: torch.Tensor, out_dim: int = 3) -> torch.Tensor:
         head_size = self.heads
         batch_size, seq_len, dim = tensor.shape
         tensor = tensor.reshape(batch_size, seq_len, head_size, dim // head_size)
         tensor = tensor.permute(0, 2, 1, 3)
 
         if out_dim == 3:
             tensor = tensor.reshape(batch_size * head_size, seq_len, dim // head_size)
 
         return tensor
 
     def get_attention_scores(
-        self, query: torch.Tensor, key: torch.Tensor, attention_mask: torch.Tensor = None
+        self,
+        query: torch.Tensor,
+        key: torch.Tensor,
+        attention_mask: torch.Tensor = None,
     ) -> torch.Tensor:
         dtype = query.dtype
         if self.upcast_attention:
             query = query.float()
             key = key.float()
 
         if attention_mask is None:
             baddbmm_input = torch.empty(
-                query.shape[0], query.shape[1], key.shape[1], dtype=query.dtype, device=query.device
+                query.shape[0],
+                query.shape[1],
+                key.shape[1],
+                dtype=query.dtype,
+                device=query.device,
             )
             beta = 0
         else:
             baddbmm_input = attention_mask
             beta = 1
 
         attention_scores = torch.baddbmm(
@@ -290,15 +315,19 @@
         del attention_scores
 
         attention_probs = attention_probs.to(dtype)
 
         return attention_probs
 
     def prepare_attention_mask(
-        self, attention_mask: torch.Tensor, target_length: int, batch_size: int, out_dim: int = 3
+        self,
+        attention_mask: torch.Tensor,
+        target_length: int,
+        batch_size: int,
+        out_dim: int = 3,
     ) -> torch.Tensor:
         head_size = self.heads
         if attention_mask is None:
             return attention_mask
 
         current_length: int = attention_mask.shape[-1]
         if current_length != target_length:
@@ -309,15 +338,17 @@
                 attention_mask = attention_mask.repeat_interleave(head_size, dim=0)
         elif out_dim == 4:
             attention_mask = attention_mask.unsqueeze(1)
             attention_mask = attention_mask.repeat_interleave(head_size, dim=1)
 
         return attention_mask
 
-    def norm_encoder_hidden_states(self, encoder_hidden_states: torch.Tensor) -> torch.Tensor:
+    def norm_encoder_hidden_states(
+        self, encoder_hidden_states: torch.Tensor
+    ) -> torch.Tensor:
         if isinstance(self.norm_cross, nn.LayerNorm):
             encoder_hidden_states = self.norm_cross(encoder_hidden_states)
         elif isinstance(self.norm_cross, nn.GroupNorm):
             encoder_hidden_states = encoder_hidden_states.transpose(1, 2)
             encoder_hidden_states = self.norm_cross(encoder_hidden_states)
             encoder_hidden_states = encoder_hidden_states.transpose(1, 2)
         else:
@@ -329,24 +360,32 @@
     def fuse_projections(self, fuse=True):
         is_cross_attention = self.cross_attention_dim != self.query_dim
         device = self.to_q.weight.data.device
         dtype = self.to_q.weight.data.dtype
 
         if not is_cross_attention:
             # fetch weight matrices.
-            concatenated_weights = torch.cat([self.to_q.weight.data, self.to_k.weight.data, self.to_v.weight.data])
+            concatenated_weights = torch.cat(
+                [self.to_q.weight.data, self.to_k.weight.data, self.to_v.weight.data]
+            )
             in_features = concatenated_weights.shape[1]
             out_features = concatenated_weights.shape[0]
 
             # create a new single projection layer and copy over the weights.
-            self.to_qkv = self.linear_cls(in_features, out_features, bias=False, device=device, dtype=dtype)
+            self.to_qkv = self.linear_cls(
+                in_features, out_features, bias=False, device=device, dtype=dtype
+            )
             self.to_qkv.weight.copy_(concatenated_weights)
 
         else:
-            concatenated_weights = torch.cat([self.to_k.weight.data, self.to_v.weight.data])
+            concatenated_weights = torch.cat(
+                [self.to_k.weight.data, self.to_v.weight.data]
+            )
             in_features = concatenated_weights.shape[1]
             out_features = concatenated_weights.shape[0]
 
-            self.to_kv = self.linear_cls(in_features, out_features, bias=False, device=device, dtype=dtype)
+            self.to_kv = self.linear_cls(
+                in_features, out_features, bias=False, device=device, dtype=dtype
+            )
             self.to_kv.weight.copy_(concatenated_weights)
 
         self.fused_projections = fuse
```

### Comparing `parediffusers-0.3.1/src/parediffusers/utils.py` & `parediffusers-0.3.2/src/parediffusers/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from torch import nn
 
+
 class DotDict(dict):
-	"""dot.notation access to dictionary attributes"""
-	__getattr__ = dict.get
-	__setattr__ = dict.__setitem__
-	__delattr__ = dict.__delitem__
+    """dot.notation access to dictionary attributes"""
+
+    __getattr__ = dict.get
+    __setattr__ = dict.__setitem__
+    __delattr__ = dict.__delitem__
 
 
 ACTIVATION_FUNCTIONS = {
-	"swish": nn.SiLU(),
-	"silu": nn.SiLU(),
-	"mish": nn.Mish(),
-	"gelu": nn.GELU(),
-	"relu": nn.ReLU(),
+    "swish": nn.SiLU(),
+    "silu": nn.SiLU(),
+    "mish": nn.Mish(),
+    "gelu": nn.GELU(),
+    "relu": nn.ReLU(),
 }
 
+
 def get_activation(act_fn: str) -> nn.Module:
-	act_fn = act_fn.lower()
-	if act_fn in ACTIVATION_FUNCTIONS:
-		return ACTIVATION_FUNCTIONS[act_fn]
-	else:
-		raise ValueError(f"Unsupported activation function: {act_fn}")
+    act_fn = act_fn.lower()
+    if act_fn in ACTIVATION_FUNCTIONS:
+        return ACTIVATION_FUNCTIONS[act_fn]
+    else:
+        raise ValueError(f"Unsupported activation function: {act_fn}")
```

### Comparing `parediffusers-0.3.1/src/parediffusers.egg-info/PKG-INFO` & `parediffusers-0.3.2/src/parediffusers.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: parediffusers
-Version: 0.3.1
+Version: 0.3.2
 Summary: The library `pared` down the features of `diffusers` implemented the minimum function to generate images without using huggingface/diffusers to understand the inner workings of the library.
 Home-page: https://github.com/masaishi/parediffusers
 Author: Masamune Ishihara
 Author-email: mwishiha@ucsc.edu
 License: MIT License
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # PareDiffusers
 
+[![Screenshot 2024-01-17 at 10 53 49 PM](https://github.com/masaishi/parediffusers/assets/1396267/c02bd298-c894-4fb6-b17a-a72f1b736748)](https://github.com/masaishi/parediffusers/blob/main/src/parediffusers/pipeline.py)
+
 [![parediffusers on PyPI](https://img.shields.io/pypi/v/parediffusers.svg)](https://pypi.org/project/parediffusers)
 
-The library `pared` down the features of `diffusers` implemented the minimum function to generate images without using [huggingface/diffusers](https://github.com/huggingface/diffusers/tree/main) to understand the inner workings of the library.
+The library `pared` down the features of `diffusers` implemented the minimum function to generate images without using [huggingface/diffusers](https://github.com/huggingface/diffusers/tree/main) functions to understand the inner workings of the library.
 
 
 ## Why PareDiffusers?
 PareDiffusers was born out of a curiosity and a desire to demystify the processes of generating images by diffusion models and the workings of the diffusers library.
 
 I will write blog-style [notebooks](./notebooks) understanding how works using a top-down approach. First, generate images using diffusers to understand the overall flow, then gradually replace code with Pytorch code. In the end, we will write the code for the [PareDiffusers code](./src/parediffusers) that does not include diffusers code.
 
 I hope that it helps others who share a similar interest in the inner workings of image generation.
 
 ## Versions
 - v0.0.0: After Ch0.0.0, inprement StableDiffusionPipeline.
 - v0.1.2: After Ch0.1.0, imprement DDIMScheduler.
 - v0.2.0: After Ch0.2.0, imprement UNet2DConditionModel.
+- v0.3.1: After Ch0.3.0, imprement AutoencoderKL.
 
 ## Table of Contents
 ### [Ch0.0.0 PareDiffusersPipeline](./notebooks/ch0.0.0_ParedDiffusionPipeline.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/masaishi/parediffusers/blob/main/notebooks/ch0.0.0_ParedDiffusionPipeline.ipynb)
 version: v0.0.0
 - [x] Generate images using diffusers
 - [x] Imprement StableDiffusionPipeline
 - [ ] Imprement DDIMScheduler
@@ -55,14 +57,23 @@
 - [x] Generate images using diffusers
 - [x] Imprement StableDiffusionPipeline
 - [x] Imprement DDIMScheduler
 - [x] Imprement UNet2DConditionModel
 - [ ] Imprement AutoencoderKL
 ### [Ch0.2.1: Test parediffusers](./notebooks/ch0.2.1_Test_PareDiffusersPipeline.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/masaishi/parediffusers/blob/main/notebooks/ch0.2.1_Test_PareDiffusersPipeline.ipynb)
 - Test PareDiffusersPipeline by pip install parediffusers.
+### [Ch0.3.0: PareAutoencoderKL](./notebooks/ch0.3.0_PareAutoencoderKL.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/masaishi/parediffusers/blob/main/notebooks/ch0.3.0_PareAutoencoderKL.ipynb)
+version: v0.3.1
+- [x] Generate images using diffusers
+- [x] Imprement StableDiffusionPipeline
+- [x] Imprement DDIMScheduler
+- [x] Imprement UNet2DConditionModel
+- [x] Imprement AutoencoderKL
+### [Ch0.3.1: Test parediffusers](./notebooks/ch0.3.1_Test_PareDiffusersPipeline.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/masaishi/parediffusers/blob/main/notebooks/ch0.3.1_Test_PareDiffusersPipeline.ipynb)
+- Test PareDiffusersPipeline by pip install parediffusers.
 
 
 ## Usage
 ```python
 import torch
 from parediffusers import PareDiffusionPipeline
 
@@ -74,8 +85,7 @@
 prompt = "painting depicting the sea, sunrise, ship, artstation, 4k, concept art"
 image = pipe(prompt)
 display(image)
 ```
 
 ## Contribution
 I am starting this project to help me understand the code in order to participate in diffusers' OSS. So, I think there may be some mistakes in my explanation, so if you find any, please feel free to correct them via an issue or pull request.
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `parediffusers-0.3.1/src/parediffusers.egg-info/SOURCES.txt` & `parediffusers-0.3.2/src/parediffusers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

