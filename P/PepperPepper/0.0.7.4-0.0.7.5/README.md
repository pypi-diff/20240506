# Comparing `tmp/pepperpepper-0.0.7.4.tar.gz` & `tmp/pepperpepper-0.0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.7.4.tar", last modified: Mon May  6 04:34:48 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.7.5.tar", last modified: Mon May  6 06:16:05 2024, max compression
```

## Comparing `pepperpepper-0.0.7.4.tar` & `pepperpepper-0.0.7.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.887399 pepperpepper-0.0.7.4/
--rw-rw-rw-   0        0        0      433 2024-05-06 04:34:48.887399 pepperpepper-0.0.7.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.855240 pepperpepper-0.0.7.4/PepperPepper/
--rw-rw-rw-   0        0        0     5237 2024-05-05 14:53:33.000000 pepperpepper-0.0.7.4/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.871272 pepperpepper-0.0.7.4/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.7.4/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.7.4/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.7.4/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.871272 pepperpepper-0.0.7.4/PepperPepper/core/
--rw-rw-rw-   0        0        0     1219 2024-05-05 15:06:09.000000 pepperpepper-0.0.7.4/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.7.4/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     4514 2024-05-06 04:34:26.000000 pepperpepper-0.0.7.4/PepperPepper/core/text_utils.py
--rw-rw-rw-   0        0        0     7067 2024-05-05 14:53:16.000000 pepperpepper-0.0.7.4/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.871272 pepperpepper-0.0.7.4/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1075 2024-05-04 04:08:04.000000 pepperpepper-0.0.7.4/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0     1016 2024-05-04 04:01:31.000000 pepperpepper-0.0.7.4/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.7.4/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.7.4/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      126 2024-05-05 14:57:43.000000 pepperpepper-0.0.7.4/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.871272 pepperpepper-0.0.7.4/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.7.4/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.7.4/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.7.4/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.7.4/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.871272 pepperpepper-0.0.7.4/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.7.4/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.7.4/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.7.4/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.886930 pepperpepper-0.0.7.4/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.7.4/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.7.4/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.887399 pepperpepper-0.0.7.4/PepperPepper/models/
--rw-rw-rw-   0        0        0     1359 2024-05-03 11:01:15.000000 pepperpepper-0.0.7.4/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0    29938 2024-05-04 02:20:17.000000 pepperpepper-0.0.7.4/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.7.4/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.7.4/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.7.4/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.887399 pepperpepper-0.0.7.4/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.7.4/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.7.4/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.7.4/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-06 04:34:48.887399 pepperpepper-0.0.7.4/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      433 2024-05-06 04:34:48.000000 pepperpepper-0.0.7.4/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1257 2024-05-06 04:34:48.000000 pepperpepper-0.0.7.4/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 04:34:48.000000 pepperpepper-0.0.7.4/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-05-06 04:34:48.000000 pepperpepper-0.0.7.4/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-06 04:34:48.000000 pepperpepper-0.0.7.4/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.7.4/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-06 04:34:48.887399 pepperpepper-0.0.7.4/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-05-06 04:34:42.000000 pepperpepper-0.0.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:16:05.118635 pepperpepper-0.0.7.5/
+-rw-rw-rw-   0        0        0      433 2024-05-06 06:16:05.118635 pepperpepper-0.0.7.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 06:16:05.006861 pepperpepper-0.0.7.5/PepperPepper/
+-rw-rw-rw-   0        0        0     5237 2024-05-05 14:53:33.000000 pepperpepper-0.0.7.5/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:16:05.038113 pepperpepper-0.0.7.5/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.7.5/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.7.5/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.7.5/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:16:05.038113 pepperpepper-0.0.7.5/PepperPepper/core/
+-rw-rw-rw-   0        0        0     1377 2024-05-06 06:15:39.000000 pepperpepper-0.0.7.5/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.7.5/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     7350 2024-05-06 06:14:50.000000 pepperpepper-0.0.7.5/PepperPepper/core/text_utils.py
+-rw-rw-rw-   0        0        0     7067 2024-05-05 14:53:16.000000 pepperpepper-0.0.7.5/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:16:05.053735 pepperpepper-0.0.7.5/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1075 2024-05-04 04:08:04.000000 pepperpepper-0.0.7.5/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0     1016 2024-05-04 04:01:31.000000 pepperpepper-0.0.7.5/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.7.5/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.7.5/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      141 2024-05-06 06:09:59.000000 pepperpepper-0.0.7.5/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:16:05.053735 pepperpepper-0.0.7.5/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.7.5/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.7.5/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.7.5/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.7.5/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:16:05.069358 pepperpepper-0.0.7.5/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.7.5/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.7.5/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.7.5/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:16:05.084984 pepperpepper-0.0.7.5/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.7.5/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.7.5/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:16:05.101001 pepperpepper-0.0.7.5/PepperPepper/models/
+-rw-rw-rw-   0        0        0     1359 2024-05-03 11:01:15.000000 pepperpepper-0.0.7.5/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0    29938 2024-05-04 02:20:17.000000 pepperpepper-0.0.7.5/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.7.5/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.7.5/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.7.5/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:16:05.116786 pepperpepper-0.0.7.5/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.7.5/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.7.5/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.7.5/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:16:05.118635 pepperpepper-0.0.7.5/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-05-06 06:16:04.000000 pepperpepper-0.0.7.5/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1257 2024-05-06 06:16:04.000000 pepperpepper-0.0.7.5/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 06:16:04.000000 pepperpepper-0.0.7.5/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-05-06 06:16:04.000000 pepperpepper-0.0.7.5/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-06 06:16:04.000000 pepperpepper-0.0.7.5/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.7.5/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-06 06:16:05.118635 pepperpepper-0.0.7.5/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-05-06 06:15:59.000000 pepperpepper-0.0.7.5/setup.py
```

### Comparing `pepperpepper-0.0.7.4/PepperPepper/__init__.py` & `pepperpepper-0.0.7.5/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.4/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.7.5/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.4/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.7.5/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.4/PepperPepper/core/__init__.py` & `pepperpepper-0.0.7.5/PepperPepper/core/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,21 +23,25 @@
 
 from .utils import evaluate_accuracy_gpu
 from .utils import train_custom
 from .utils import try_gpu
 from .utils import try_all_gpus
 from .text_utils import tokenize
 from .text_utils import Vocab
+from .text_utils import seq_data_iter_random
+from .text_utils import seq_data_iter_sequential
 # from .data_structures import CustomDataStructure
 # from .utils import some_utility_function
 # from .model_builder import build_model
 #
 # __all__ 变量定义了当使用 from core import * 时导入哪些对象
 # 注意：通常不推荐使用 from package import *
 __all__ = [
     'evaluate_accuracy_gpu',
     'train_custom',
     'try_gpu',
     'try_all_gpus',
     'tokenize',
-    'Vocab'
+    'Vocab',
+    'seq_data_iter_random',
+    'seq_data_iter_sequential'
 ]
```

### Comparing `pepperpepper-0.0.7.4/PepperPepper/core/utils.py` & `pepperpepper-0.0.7.5/PepperPepper/core/utils.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.4/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.7.5/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.4/PepperPepper/datasets/custom_dataset.py` & `pepperpepper-0.0.7.5/PepperPepper/datasets/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.4/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.7.5/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.4/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.7.5/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.4/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.7.5/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.4/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.7.5/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.4/PepperPepper/models/__init__.py` & `pepperpepper-0.0.7.5/PepperPepper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.4/PepperPepper/models/cnn.py` & `pepperpepper-0.0.7.5/PepperPepper/models/cnn.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.4/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.7.5/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.4/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.7.5/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.4/setup.py` & `pepperpepper-0.0.7.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.7.4",
+    version="0.0.7.5",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```

