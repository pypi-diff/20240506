# Comparing `tmp/pepperpepper-0.0.7.1.tar.gz` & `tmp/pepperpepper-0.0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.7.1.tar", last modified: Mon May  6 03:56:46 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.7.2.tar", last modified: Mon May  6 04:06:56 2024, max compression
```

## Comparing `pepperpepper-0.0.7.1.tar` & `pepperpepper-0.0.7.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.788361 pepperpepper-0.0.7.1/
--rw-rw-rw-   0        0        0      433 2024-05-06 03:56:46.788361 pepperpepper-0.0.7.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.714031 pepperpepper-0.0.7.1/PepperPepper/
--rw-rw-rw-   0        0        0     5237 2024-05-05 14:53:33.000000 pepperpepper-0.0.7.1/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.744814 pepperpepper-0.0.7.1/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.7.1/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.7.1/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.7.1/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.747814 pepperpepper-0.0.7.1/PepperPepper/core/
--rw-rw-rw-   0        0        0     1219 2024-05-05 15:06:09.000000 pepperpepper-0.0.7.1/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.7.1/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     4678 2024-05-05 15:13:14.000000 pepperpepper-0.0.7.1/PepperPepper/core/text_utils.py
--rw-rw-rw-   0        0        0     7067 2024-05-05 14:53:16.000000 pepperpepper-0.0.7.1/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.757853 pepperpepper-0.0.7.1/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1075 2024-05-04 04:08:04.000000 pepperpepper-0.0.7.1/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0     1016 2024-05-04 04:01:31.000000 pepperpepper-0.0.7.1/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.7.1/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.7.1/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      126 2024-05-05 14:57:43.000000 pepperpepper-0.0.7.1/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.760970 pepperpepper-0.0.7.1/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.7.1/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.7.1/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.7.1/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.7.1/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.763970 pepperpepper-0.0.7.1/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.7.1/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.7.1/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.7.1/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.767969 pepperpepper-0.0.7.1/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.7.1/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.7.1/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.781277 pepperpepper-0.0.7.1/PepperPepper/models/
--rw-rw-rw-   0        0        0     1359 2024-05-03 11:01:15.000000 pepperpepper-0.0.7.1/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0    29938 2024-05-04 02:20:17.000000 pepperpepper-0.0.7.1/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.7.1/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.7.1/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.7.1/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.785360 pepperpepper-0.0.7.1/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.7.1/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.7.1/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.7.1/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-06 03:56:46.787359 pepperpepper-0.0.7.1/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      433 2024-05-06 03:56:46.000000 pepperpepper-0.0.7.1/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1257 2024-05-06 03:56:46.000000 pepperpepper-0.0.7.1/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 03:56:46.000000 pepperpepper-0.0.7.1/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-05-06 03:56:46.000000 pepperpepper-0.0.7.1/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-06 03:56:46.000000 pepperpepper-0.0.7.1/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.7.1/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-06 03:56:46.788361 pepperpepper-0.0.7.1/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-05-06 03:56:28.000000 pepperpepper-0.0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:06:56.288215 pepperpepper-0.0.7.2/
+-rw-rw-rw-   0        0        0      433 2024-05-06 04:06:56.288215 pepperpepper-0.0.7.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 04:06:56.159497 pepperpepper-0.0.7.2/PepperPepper/
+-rw-rw-rw-   0        0        0     5237 2024-05-05 14:53:33.000000 pepperpepper-0.0.7.2/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:06:56.206805 pepperpepper-0.0.7.2/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.7.2/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.7.2/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.7.2/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:06:56.206805 pepperpepper-0.0.7.2/PepperPepper/core/
+-rw-rw-rw-   0        0        0     1219 2024-05-05 15:06:09.000000 pepperpepper-0.0.7.2/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.7.2/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     4701 2024-05-06 04:06:02.000000 pepperpepper-0.0.7.2/PepperPepper/core/text_utils.py
+-rw-rw-rw-   0        0        0     7067 2024-05-05 14:53:16.000000 pepperpepper-0.0.7.2/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:06:56.227994 pepperpepper-0.0.7.2/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1075 2024-05-04 04:08:04.000000 pepperpepper-0.0.7.2/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0     1016 2024-05-04 04:01:31.000000 pepperpepper-0.0.7.2/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.7.2/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.7.2/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      126 2024-05-05 14:57:43.000000 pepperpepper-0.0.7.2/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:06:56.227994 pepperpepper-0.0.7.2/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.7.2/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.7.2/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.7.2/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.7.2/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:06:56.240728 pepperpepper-0.0.7.2/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.7.2/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.7.2/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.7.2/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:06:56.254253 pepperpepper-0.0.7.2/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.7.2/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.7.2/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:06:56.269907 pepperpepper-0.0.7.2/PepperPepper/models/
+-rw-rw-rw-   0        0        0     1359 2024-05-03 11:01:15.000000 pepperpepper-0.0.7.2/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0    29938 2024-05-04 02:20:17.000000 pepperpepper-0.0.7.2/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.7.2/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.7.2/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.7.2/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:06:56.288215 pepperpepper-0.0.7.2/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.7.2/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.7.2/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.7.2/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:06:56.288215 pepperpepper-0.0.7.2/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-05-06 04:06:56.000000 pepperpepper-0.0.7.2/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1257 2024-05-06 04:06:56.000000 pepperpepper-0.0.7.2/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 04:06:56.000000 pepperpepper-0.0.7.2/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-05-06 04:06:56.000000 pepperpepper-0.0.7.2/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-06 04:06:56.000000 pepperpepper-0.0.7.2/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.7.2/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-06 04:06:56.288215 pepperpepper-0.0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-05-06 04:06:50.000000 pepperpepper-0.0.7.2/setup.py
```

### Comparing `pepperpepper-0.0.7.1/PepperPepper/__init__.py` & `pepperpepper-0.0.7.2/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.1/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.7.2/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.1/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.7.2/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.1/PepperPepper/core/__init__.py` & `pepperpepper-0.0.7.2/PepperPepper/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.1/PepperPepper/core/text_utils.py` & `pepperpepper-0.0.7.2/PepperPepper/core/text_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,15 @@
             return 0
 
         @property
         def token_freqs(self):
             """返回词元及其频率的列表"""
             return self._token_freqs
 
+        @staticmethod
         def count_corpus(tokens):
             """
             统计词元的频率。
 
             Parameters:
                 tokens (list): 用于统计的词元列表，可以是一维或二维列表。
```

### Comparing `pepperpepper-0.0.7.1/PepperPepper/core/utils.py` & `pepperpepper-0.0.7.2/PepperPepper/core/utils.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.1/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.7.2/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.1/PepperPepper/datasets/custom_dataset.py` & `pepperpepper-0.0.7.2/PepperPepper/datasets/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.1/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.7.2/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.1/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.7.2/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.1/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.7.2/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.1/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.7.2/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.1/PepperPepper/models/__init__.py` & `pepperpepper-0.0.7.2/PepperPepper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.1/PepperPepper/models/cnn.py` & `pepperpepper-0.0.7.2/PepperPepper/models/cnn.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.1/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.7.2/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.1/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.7.2/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.1/setup.py` & `pepperpepper-0.0.7.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.7.1",
+    version="0.0.7.2",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```

