# Comparing `tmp/pepperpepper-0.0.7.0.tar.gz` & `tmp/pepperpepper-0.0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.7.0.tar", last modified: Sat May  4 04:03:24 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.7.1.tar", last modified: Mon May  6 03:56:46 2024, max compression
```

## Comparing `pepperpepper-0.0.7.0.tar` & `pepperpepper-0.0.7.1.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 04:03:24.180194 pepperpepper-0.0.7.0/
--rw-rw-rw-   0        0        0      433 2024-05-04 04:03:24.178194 pepperpepper-0.0.7.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-04 04:03:24.053006 pepperpepper-0.0.7.0/PepperPepper/
--rw-rw-rw-   0        0        0     5142 2024-05-02 15:25:47.000000 pepperpepper-0.0.7.0/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:03:24.103651 pepperpepper-0.0.7.0/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.7.0/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.7.0/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.7.0/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:03:24.108063 pepperpepper-0.0.7.0/PepperPepper/core/
--rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.7.0/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.7.0/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.7.0/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:03:24.113975 pepperpepper-0.0.7.0/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1071 2024-05-04 04:01:49.000000 pepperpepper-0.0.7.0/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0     1016 2024-05-04 04:01:31.000000 pepperpepper-0.0.7.0/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.7.0/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.7.0/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.7.0/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:03:24.121848 pepperpepper-0.0.7.0/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.7.0/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.7.0/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.7.0/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.7.0/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:03:24.127575 pepperpepper-0.0.7.0/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.7.0/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.7.0/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.7.0/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:03:24.131649 pepperpepper-0.0.7.0/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.7.0/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.7.0/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:03:24.167056 pepperpepper-0.0.7.0/PepperPepper/models/
--rw-rw-rw-   0        0        0     1359 2024-05-03 11:01:15.000000 pepperpepper-0.0.7.0/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0    29938 2024-05-04 02:20:17.000000 pepperpepper-0.0.7.0/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.7.0/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.7.0/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.7.0/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:03:24.176196 pepperpepper-0.0.7.0/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.7.0/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.7.0/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.7.0/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:03:24.177197 pepperpepper-0.0.7.0/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      433 2024-05-04 04:03:23.000000 pepperpepper-0.0.7.0/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-05-04 04:03:23.000000 pepperpepper-0.0.7.0/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 04:03:23.000000 pepperpepper-0.0.7.0/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-05-04 04:03:23.000000 pepperpepper-0.0.7.0/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-04 04:03:23.000000 pepperpepper-0.0.7.0/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.7.0/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-04 04:03:24.180194 pepperpepper-0.0.7.0/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-05-04 04:03:04.000000 pepperpepper-0.0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.788361 pepperpepper-0.0.7.1/
+-rw-rw-rw-   0        0        0      433 2024-05-06 03:56:46.788361 pepperpepper-0.0.7.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.714031 pepperpepper-0.0.7.1/PepperPepper/
+-rw-rw-rw-   0        0        0     5237 2024-05-05 14:53:33.000000 pepperpepper-0.0.7.1/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.744814 pepperpepper-0.0.7.1/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.7.1/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.7.1/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.7.1/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.747814 pepperpepper-0.0.7.1/PepperPepper/core/
+-rw-rw-rw-   0        0        0     1219 2024-05-05 15:06:09.000000 pepperpepper-0.0.7.1/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.7.1/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     4678 2024-05-05 15:13:14.000000 pepperpepper-0.0.7.1/PepperPepper/core/text_utils.py
+-rw-rw-rw-   0        0        0     7067 2024-05-05 14:53:16.000000 pepperpepper-0.0.7.1/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.757853 pepperpepper-0.0.7.1/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1075 2024-05-04 04:08:04.000000 pepperpepper-0.0.7.1/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0     1016 2024-05-04 04:01:31.000000 pepperpepper-0.0.7.1/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.7.1/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.7.1/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      126 2024-05-05 14:57:43.000000 pepperpepper-0.0.7.1/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.760970 pepperpepper-0.0.7.1/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.7.1/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.7.1/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.7.1/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.7.1/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.763970 pepperpepper-0.0.7.1/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.7.1/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.7.1/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.7.1/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.767969 pepperpepper-0.0.7.1/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.7.1/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.7.1/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.781277 pepperpepper-0.0.7.1/PepperPepper/models/
+-rw-rw-rw-   0        0        0     1359 2024-05-03 11:01:15.000000 pepperpepper-0.0.7.1/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0    29938 2024-05-04 02:20:17.000000 pepperpepper-0.0.7.1/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.7.1/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.7.1/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.7.1/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.785360 pepperpepper-0.0.7.1/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.7.1/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.7.1/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.7.1/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.787359 pepperpepper-0.0.7.1/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-05-06 03:56:46.000000 pepperpepper-0.0.7.1/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1257 2024-05-06 03:56:46.000000 pepperpepper-0.0.7.1/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 03:56:46.000000 pepperpepper-0.0.7.1/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-05-06 03:56:46.000000 pepperpepper-0.0.7.1/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-06 03:56:46.000000 pepperpepper-0.0.7.1/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.7.1/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-06 03:56:46.788361 pepperpepper-0.0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-05-06 03:56:28.000000 pepperpepper-0.0.7.1/setup.py
```

### Comparing `pepperpepper-0.0.7.0/PepperPepper/__init__.py` & `pepperpepper-0.0.7.1/PepperPepper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 模块:
 
 core 模块
 功能：包含包的核心功能和基础类。
 子模块/文件：
 base_model.py：定义基础模型类，提供模型初始化、保存、加载等基础功能。
 utils.py：包含一些通用的工具函数，如数据处理、模型评估等。
+text.utils: 负责处理文本数据相关的功能，例如词表构建、词频统计等。
 
 models 模块
 功能：包含各种深度学习模型的实现。
 子模块/文件：
 cnn.py：卷积神经网络（CNN）相关模型的实现。
 rnn.py：循环神经网络（RNN）相关模型的实现。
 transformer.py：Transformer模型及其变体的实现。
```

### Comparing `pepperpepper-0.0.7.0/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.7.1/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.0/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.7.1/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.0/PepperPepper/core/utils.py` & `pepperpepper-0.0.7.1/PepperPepper/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,8 +196,26 @@
     devices = []
     # 遍历所有检测到的GPU设备
     for i in range(torch.cuda.device_count()):
         # 将每个GPU设备添加到列表中
         devices.append(torch.device(f'cuda:{i}'))
         # 如果devices列表不为空（即存在GPU设备），则返回该列表
     # 否则，返回只包含CPU设备的列表
-    return devices if devices else [torch.device('cpu')]
+    return devices if devices else [torch.device('cpu')]
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
```

### Comparing `pepperpepper-0.0.7.0/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.7.1/PepperPepper/datasets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,7 +37,9 @@
 # 注意：通常不推荐使用 from package import *
 __all__ = [
     'load_data_minist',
     'load_data_fashion_mnist',
     'load_arrays'
 ]
 
+
+
```

### Comparing `pepperpepper-0.0.7.0/PepperPepper/datasets/custom_dataset.py` & `pepperpepper-0.0.7.1/PepperPepper/datasets/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.0/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.7.1/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.0/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.7.1/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.0/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.7.1/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.0/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.7.1/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.0/PepperPepper/models/__init__.py` & `pepperpepper-0.0.7.1/PepperPepper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.0/PepperPepper/models/cnn.py` & `pepperpepper-0.0.7.1/PepperPepper/models/cnn.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.0/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.7.1/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.0/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.7.1/PepperPepper.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 PepperPepper.egg-info/top_level.txt
 PepperPepper.egg-info/zip-safe
 PepperPepper/callbacks/__init__.py
 PepperPepper/callbacks/custom_callback.py
 PepperPepper/callbacks/learning_rate_scheduler.py
 PepperPepper/core/__init__.py
 PepperPepper/core/base_model.py
+PepperPepper/core/text_utils.py
 PepperPepper/core/utils.py
 PepperPepper/datasets/__init__.py
 PepperPepper/datasets/custom_dataset.py
 PepperPepper/datasets/image_datasets.py
 PepperPepper/datasets/text_datasets.py
 PepperPepper/examples/__init__.py
 PepperPepper/examples/custom_task.py
```

### Comparing `pepperpepper-0.0.7.0/setup.py` & `pepperpepper-0.0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.7.0",
+    version="0.0.7.1",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```

