# Comparing `tmp/rastervision_pytorch_learner-0.30.0.tar.gz` & `tmp/rastervision_pytorch_learner-0.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastervision_pytorch_learner-0.30.0.tar", last modified: Wed Apr 10 22:11:09 2024, max compression
+gzip compressed data, was "rastervision_pytorch_learner-0.30.1.tar", last modified: Mon May  6 21:02:14 2024, max compression
```

## Comparing `rastervision_pytorch_learner-0.30.0.tar` & `rastervision_pytorch_learner-0.30.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.251691 rastervision_pytorch_learner-0.30.0/
--rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.30.0/MANIFEST.in
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      564 2024-04-10 22:11:09.251691 rastervision_pytorch_learner-0.30.0/PKG-INFO
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.247691 rastervision_pytorch_learner-0.30.0/rastervision/
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.247691 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3813 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1888 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/classification_learner.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6605 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/classification_learner_config.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.247691 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1542 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5360 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/classification_dataset.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    22638 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/dataset.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    12981 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/object_detection_dataset.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1979 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/regression_dataset.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7110 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/semantic_segmentation_dataset.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8253 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/transform.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.251691 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/utils/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      278 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/utils/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2574 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/utils/utils.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.251691 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/
--rw-r--r--   0 ahassan   (1001) ahassan   (1001)      645 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3345 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/classification_visualizer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1259 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/object_detection_visualizer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3590 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/regression_visualizer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3284 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/semantic_segmentation_visualizer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     9916 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/visualizer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    70836 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/learner.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    57769 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/learner_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7031 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/object_detection_learner.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     9205 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/object_detection_learner_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    14607 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/object_detection_utils.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4381 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/regression_learner.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8727 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/regression_learner_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4456 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/semantic_segmentation_learner.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8409 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/semantic_segmentation_learner_config.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.251691 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1008 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3593 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/distributed.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4655 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/prediction.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5394 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/torch_hub.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    19003 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/utils.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.251691 rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      564 2024-04-10 22:11:09.000000 rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/PKG-INFO
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2192 2024-04-10 22:11:09.000000 rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/SOURCES.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 22:11:09.000000 rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/dependency_links.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 21:24:49.000000 rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/not-zip-safe
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      168 2024-04-10 22:11:09.000000 rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/requires.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       24 2024-04-10 22:11:09.000000 rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/top_level.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      285 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/requirements.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-04-10 22:11:09.251691 rastervision_pytorch_learner-0.30.0/setup.cfg
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1731 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.0/setup.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.123125 rastervision_pytorch_learner-0.30.1/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.30.1/MANIFEST.in
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      564 2024-05-06 21:02:14.123125 rastervision_pytorch_learner-0.30.1/PKG-INFO
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.119125 rastervision_pytorch_learner-0.30.1/rastervision/
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.123125 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3813 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1888 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/classification_learner.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6605 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/classification_learner_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.123125 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1542 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5360 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/classification_dataset.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    22638 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/dataset.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    12981 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/object_detection_dataset.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1979 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/regression_dataset.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7110 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/semantic_segmentation_dataset.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8253 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/transform.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.123125 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/utils/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      278 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/utils/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2574 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/utils/utils.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.123125 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/visualizer/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)      645 2023-08-24 18:41:21.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/visualizer/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3345 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/visualizer/classification_visualizer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1259 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/visualizer/object_detection_visualizer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3590 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/visualizer/regression_visualizer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3284 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/visualizer/semantic_segmentation_visualizer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     9916 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/visualizer/visualizer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    70922 2024-05-03 19:36:20.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/learner.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    57753 2024-05-03 19:36:10.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/learner_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7031 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/object_detection_learner.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     9205 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/object_detection_learner_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    14607 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/object_detection_utils.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4381 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/regression_learner.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8727 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/regression_learner_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4456 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/semantic_segmentation_learner.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8409 2024-04-10 21:55:10.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/semantic_segmentation_learner_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.123125 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/utils/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1008 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/utils/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3593 2024-04-06 20:13:30.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/utils/distributed.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4655 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/utils/prediction.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5394 2024-04-07 00:38:15.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/utils/torch_hub.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    18940 2024-05-06 20:46:22.000000 rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/utils/utils.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.123125 rastervision_pytorch_learner-0.30.1/rastervision_pytorch_learner.egg-info/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      564 2024-05-06 21:02:14.000000 rastervision_pytorch_learner-0.30.1/rastervision_pytorch_learner.egg-info/PKG-INFO
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2192 2024-05-06 21:02:14.000000 rastervision_pytorch_learner-0.30.1/rastervision_pytorch_learner.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-05-06 21:02:14.000000 rastervision_pytorch_learner-0.30.1/rastervision_pytorch_learner.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-05-06 21:02:14.000000 rastervision_pytorch_learner-0.30.1/rastervision_pytorch_learner.egg-info/not-zip-safe
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      168 2024-05-06 21:02:14.000000 rastervision_pytorch_learner-0.30.1/rastervision_pytorch_learner.egg-info/requires.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       13 2024-05-06 21:02:14.000000 rastervision_pytorch_learner-0.30.1/rastervision_pytorch_learner.egg-info/top_level.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      285 2024-05-06 20:16:58.000000 rastervision_pytorch_learner-0.30.1/requirements.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-05-06 21:02:14.123125 rastervision_pytorch_learner-0.30.1/setup.cfg
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1731 2024-05-06 20:16:58.000000 rastervision_pytorch_learner-0.30.1/setup.py
```

### Comparing `rastervision_pytorch_learner-0.30.0/PKG-INFO` & `rastervision_pytorch_learner-0.30.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision_pytorch_learner
-Version: 0.30.0
+Version: 0.30.1
 Summary: A rastervision plugin that adds PyTorch training pipelines
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/__init__.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/classification_learner.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/classification_learner.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/classification_learner_config.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/classification_learner_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/__init__.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/classification_dataset.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/classification_dataset.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/dataset.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/object_detection_dataset.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/object_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/regression_dataset.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/regression_dataset.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/semantic_segmentation_dataset.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/semantic_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/transform.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/transform.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/utils/utils.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/__init__.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/visualizer/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/classification_visualizer.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/visualizer/classification_visualizer.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/object_detection_visualizer.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/visualizer/object_detection_visualizer.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/regression_visualizer.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/visualizer/regression_visualizer.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/semantic_segmentation_visualizer.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/visualizer/semantic_segmentation_visualizer.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/dataset/visualizer/visualizer.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/dataset/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/learner.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/learner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1114,15 +1114,16 @@
         """
         if self.onnx_mode:
             self.model = self.load_onnx_model(model_weights_path)
             return
         if self.model is None:
             self.model = self.build_model(model_def_path=model_def_path)
         self.model.to(device=self.device)
-        if self.is_ddp_process:  # pragma: no cover
+        if self.is_ddp_process and not isinstance(self.model,
+                                                  DDP):  # pragma: no cover
             self.model = nn.SyncBatchNorm.convert_sync_batchnorm(self.model)
             self.model = DDP(self.model, device_ids=[self.ddp_local_rank])
         self.load_init_weights(model_weights_path=model_weights_path)
 
     def build_model(self, model_def_path: Optional[str] = None) -> nn.Module:
         """Build a PyTorch model."""
         cfg = self.cfg
```

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/learner_config.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/learner_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1176,19 +1176,20 @@
 
     scene_dataset: Optional['SceneDatasetConfig'] = Field(None, description='')
     sampling: Union[WindowSamplingConfig, Dict[
         str, WindowSamplingConfig]] = Field(
             {}, description='Window sampling config.')
 
     def __repr_args__(self):
-        ds = self.scene_dataset
-        ds_repr = (f'<{len(ds.train_scenes)} train_scenes, '
-                   f'{len(ds.validation_scenes)} validation_scenes, '
-                   f'{len(ds.test_scenes)} test_scenes>')
-        out = [('scene_dataset', ds_repr), ('sampling', str(self.sampling))]
+        ds_str = repr(self.scene_dataset)
+        if isinstance(self.sampling, dict):
+            sampling_str = f'Dict with {len(self.sampling)} keys'
+        else:
+            sampling_str = str(self.sampling)
+        out = [('scene_dataset', ds_str), ('sampling', sampling_str)]
         return out
 
     @validator('sampling')
     def validate_sampling(
             cls,
             v: Union[WindowSamplingConfig, Dict[str, WindowSamplingConfig]],
             values: dict
```

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/object_detection_learner.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/object_detection_learner.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/object_detection_learner_config.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/object_detection_learner_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/object_detection_utils.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/object_detection_utils.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/regression_learner.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/regression_learner.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/regression_learner_config.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/regression_learner_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/semantic_segmentation_learner.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/semantic_segmentation_learner.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/semantic_segmentation_learner_config.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/semantic_segmentation_learner_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/__init__.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/distributed.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/prediction.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/utils/prediction.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/torch_hub.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/utils/torch_hub.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision/pytorch_learner/utils/utils.py` & `rastervision_pytorch_learner-0.30.1/rastervision/pytorch_learner/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,17 +212,14 @@
 
 
 class Parallel(nn.ModuleList):
     """ Passes inputs through multiple `nn.Module`s in parallel.
         Returns a tuple of outputs.
     """
 
-    def __init__(self, *args):
-        super().__init__(args)
-
     def forward(self, xs):
         if isinstance(xs, torch.Tensor):
             return tuple(m(xs) for m in self)
         assert len(xs) == len(self)
         return tuple(m(x) for m, x in zip(self, xs))
```

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/PKG-INFO` & `rastervision_pytorch_learner-0.30.1/rastervision_pytorch_learner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision-pytorch-learner
-Version: 0.30.0
+Version: 0.30.1
 Summary: A rastervision plugin that adds PyTorch training pipelines
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_pytorch_learner-0.30.0/rastervision_pytorch_learner.egg-info/SOURCES.txt` & `rastervision_pytorch_learner-0.30.1/rastervision_pytorch_learner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_learner-0.30.0/setup.py` & `rastervision_pytorch_learner-0.30.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 from os.path import abspath, dirname, join
 from setuptools import setup, find_namespace_packages
 import re
 
 name = 'rastervision_pytorch_learner'
-version = '0.30.0'
+version = '0.30.1'
 description = 'A rastervision plugin that adds PyTorch training pipelines'
 requirement_constraints = {}
 
 here = abspath(dirname(__file__))
 
 
 def parse_requirements(requirements_path: str) -> list[str]:
```

