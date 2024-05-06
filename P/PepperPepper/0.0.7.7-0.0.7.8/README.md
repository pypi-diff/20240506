# Comparing `tmp/pepperpepper-0.0.7.7.tar.gz` & `tmp/pepperpepper-0.0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.7.7.tar", last modified: Mon May  6 07:55:45 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.7.8.tar", last modified: Mon May  6 13:10:26 2024, max compression
```

## Comparing `pepperpepper-0.0.7.7.tar` & `pepperpepper-0.0.7.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 07:55:45.211714 pepperpepper-0.0.7.7/
--rw-rw-rw-   0        0        0      433 2024-05-06 07:55:45.210713 pepperpepper-0.0.7.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 07:55:45.174154 pepperpepper-0.0.7.7/PepperPepper/
--rw-rw-rw-   0        0        0     5237 2024-05-05 14:53:33.000000 pepperpepper-0.0.7.7/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 07:55:45.185863 pepperpepper-0.0.7.7/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.7.7/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.7.7/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.7.7/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-05-06 07:55:45.189586 pepperpepper-0.0.7.7/PepperPepper/core/
--rw-rw-rw-   0        0        0     1438 2024-05-06 06:39:00.000000 pepperpepper-0.0.7.7/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.7.7/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     9642 2024-05-06 07:55:18.000000 pepperpepper-0.0.7.7/PepperPepper/core/text_utils.py
--rw-rw-rw-   0        0        0     7067 2024-05-05 14:53:16.000000 pepperpepper-0.0.7.7/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-06 07:55:45.192097 pepperpepper-0.0.7.7/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1075 2024-05-04 04:08:04.000000 pepperpepper-0.0.7.7/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0     1016 2024-05-04 04:01:31.000000 pepperpepper-0.0.7.7/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.7.7/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.7.7/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      141 2024-05-06 06:09:59.000000 pepperpepper-0.0.7.7/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-05-06 07:55:45.194482 pepperpepper-0.0.7.7/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.7.7/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.7.7/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.7.7/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.7.7/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-06 07:55:45.196486 pepperpepper-0.0.7.7/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.7.7/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.7.7/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.7.7/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-06 07:55:45.198358 pepperpepper-0.0.7.7/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.7.7/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.7.7/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-05-06 07:55:45.205441 pepperpepper-0.0.7.7/PepperPepper/models/
--rw-rw-rw-   0        0        0     1359 2024-05-03 11:01:15.000000 pepperpepper-0.0.7.7/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0    29938 2024-05-04 02:20:17.000000 pepperpepper-0.0.7.7/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.7.7/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.7.7/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.7.7/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-05-06 07:55:45.209710 pepperpepper-0.0.7.7/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.7.7/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.7.7/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.7.7/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-06 07:55:45.210713 pepperpepper-0.0.7.7/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      433 2024-05-06 07:55:45.000000 pepperpepper-0.0.7.7/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1257 2024-05-06 07:55:45.000000 pepperpepper-0.0.7.7/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 07:55:45.000000 pepperpepper-0.0.7.7/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-05-06 07:55:45.000000 pepperpepper-0.0.7.7/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-06 07:55:45.000000 pepperpepper-0.0.7.7/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.7.7/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-06 07:55:45.211714 pepperpepper-0.0.7.7/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-05-06 07:55:31.000000 pepperpepper-0.0.7.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:10:26.122559 pepperpepper-0.0.7.8/
+-rw-rw-rw-   0        0        0      433 2024-05-06 13:10:26.106805 pepperpepper-0.0.7.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 13:10:26.059213 pepperpepper-0.0.7.8/PepperPepper/
+-rw-rw-rw-   0        0        0     5237 2024-05-05 14:53:33.000000 pepperpepper-0.0.7.8/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:10:26.092771 pepperpepper-0.0.7.8/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.7.8/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.7.8/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.7.8/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:10:26.092771 pepperpepper-0.0.7.8/PepperPepper/core/
+-rw-rw-rw-   0        0        0     1438 2024-05-06 06:39:00.000000 pepperpepper-0.0.7.8/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.7.8/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     9642 2024-05-06 07:55:18.000000 pepperpepper-0.0.7.8/PepperPepper/core/text_utils.py
+-rw-rw-rw-   0        0        0     7067 2024-05-05 14:53:16.000000 pepperpepper-0.0.7.8/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:10:26.101298 pepperpepper-0.0.7.8/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1075 2024-05-04 04:08:04.000000 pepperpepper-0.0.7.8/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0     1016 2024-05-04 04:01:31.000000 pepperpepper-0.0.7.8/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.7.8/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.7.8/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      141 2024-05-06 06:09:59.000000 pepperpepper-0.0.7.8/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:10:26.106805 pepperpepper-0.0.7.8/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.7.8/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.7.8/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.7.8/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.7.8/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:10:26.106805 pepperpepper-0.0.7.8/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.7.8/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.7.8/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.7.8/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:10:26.106805 pepperpepper-0.0.7.8/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.7.8/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.7.8/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:10:26.106805 pepperpepper-0.0.7.8/PepperPepper/models/
+-rw-rw-rw-   0        0        0     1359 2024-05-03 11:01:15.000000 pepperpepper-0.0.7.8/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0    29938 2024-05-04 02:20:17.000000 pepperpepper-0.0.7.8/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.7.8/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.7.8/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.7.8/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:10:26.106805 pepperpepper-0.0.7.8/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      499 2024-05-06 13:09:24.000000 pepperpepper-0.0.7.8/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0      638 2024-05-06 10:04:20.000000 pepperpepper-0.0.7.8/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.7.8/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:10:26.106805 pepperpepper-0.0.7.8/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-05-06 13:10:25.000000 pepperpepper-0.0.7.8/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1257 2024-05-06 13:10:25.000000 pepperpepper-0.0.7.8/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 13:10:25.000000 pepperpepper-0.0.7.8/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-05-06 13:10:25.000000 pepperpepper-0.0.7.8/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-06 13:10:25.000000 pepperpepper-0.0.7.8/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.7.8/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-06 13:10:26.122559 pepperpepper-0.0.7.8/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-05-06 13:09:53.000000 pepperpepper-0.0.7.8/setup.py
```

### Comparing `pepperpepper-0.0.7.7/PepperPepper/__init__.py` & `pepperpepper-0.0.7.8/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.7/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.7.8/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.7/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.7.8/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.7/PepperPepper/core/__init__.py` & `pepperpepper-0.0.7.8/PepperPepper/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.7/PepperPepper/core/text_utils.py` & `pepperpepper-0.0.7.8/PepperPepper/core/text_utils.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.7/PepperPepper/core/utils.py` & `pepperpepper-0.0.7.8/PepperPepper/core/utils.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.7/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.7.8/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.7/PepperPepper/datasets/custom_dataset.py` & `pepperpepper-0.0.7.8/PepperPepper/datasets/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.7/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.7.8/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.7/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.7.8/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.7/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.7.8/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.7/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.7.8/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.7/PepperPepper/models/__init__.py` & `pepperpepper-0.0.7.8/PepperPepper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.7/PepperPepper/models/cnn.py` & `pepperpepper-0.0.7.8/PepperPepper/models/cnn.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.7/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.7.8/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.7.7/setup.py` & `pepperpepper-0.0.7.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.7.7",
+    version="0.0.7.8",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```

