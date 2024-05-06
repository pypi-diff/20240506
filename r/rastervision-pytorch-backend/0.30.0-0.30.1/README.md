# Comparing `tmp/rastervision_pytorch_backend-0.30.0.tar.gz` & `tmp/rastervision_pytorch_backend-0.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastervision_pytorch_backend-0.30.0.tar", last modified: Wed Apr 10 22:11:09 2024, max compression
+gzip compressed data, was "rastervision_pytorch_backend-0.30.1.tar", last modified: Mon May  6 21:02:14 2024, max compression
```

## Comparing `rastervision_pytorch_backend-0.30.0.tar` & `rastervision_pytorch_backend-0.30.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/
--rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_pytorch_backend-0.30.0/MANIFEST.in
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      586 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/PKG-INFO
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.479691 rastervision_pytorch_backend-0.30.0/rastervision/
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      911 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/__init__.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        0 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/__init__.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/chip_classification/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       45 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/chip_classification/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7410 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/chip_classification/spacenet_rio.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       45 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8108 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        0 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      728 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/merge_geojson.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2631 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/prepare_potsdam.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      804 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/resample_geotiffs.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      978 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/transfer_georeference.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4984 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/xview.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       45 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     9562 2024-04-07 00:38:15.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/isprs_potsdam.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    10068 2024-04-07 00:38:15.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/isprs_potsdam_multi_source.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8255 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/spacenet_vegas.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1480 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/utils.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    21848 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/test.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3650 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/tiny_spacenet.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3788 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/utils.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2990 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_chip_classification.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2344 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_chip_classification_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7949 2024-04-07 00:38:15.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_learner_backend.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3575 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_learner_backend_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4908 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_object_detection.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2349 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_object_detection_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3417 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_semantic_segmentation.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2401 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_semantic_segmentation_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1363 2024-04-07 00:38:15.000000 rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/utils.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      586 2024-04-10 22:11:09.000000 rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/PKG-INFO
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2338 2024-04-10 22:11:09.000000 rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/SOURCES.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 22:11:09.000000 rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/dependency_links.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 21:24:49.000000 rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/not-zip-safe
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       89 2024-04-10 22:11:09.000000 rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/requires.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       24 2024-04-10 22:11:09.000000 rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/top_level.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      121 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/requirements.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-04-10 22:11:09.483691 rastervision_pytorch_backend-0.30.0/setup.cfg
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1753 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.0/setup.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.363126 rastervision_pytorch_backend-0.30.1/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_pytorch_backend-0.30.1/MANIFEST.in
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      586 2024-05-06 21:02:14.363126 rastervision_pytorch_backend-0.30.1/PKG-INFO
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.359126 rastervision_pytorch_backend-0.30.1/rastervision/
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.359126 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      911 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/__init__.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.359126 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        0 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/__init__.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.363126 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/chip_classification/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       45 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/chip_classification/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7410 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/chip_classification/spacenet_rio.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.363126 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/object_detection/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       45 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/object_detection/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8108 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.363126 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        0 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      728 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/merge_geojson.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2631 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/prepare_potsdam.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      804 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/resample_geotiffs.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      978 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/transfer_georeference.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4984 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/object_detection/xview.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.363126 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/semantic_segmentation/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       45 2023-08-22 15:58:07.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/semantic_segmentation/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     9562 2024-04-07 00:38:15.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/semantic_segmentation/isprs_potsdam.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    10068 2024-04-07 00:38:15.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/semantic_segmentation/isprs_potsdam_multi_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8255 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/semantic_segmentation/spacenet_vegas.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1480 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/semantic_segmentation/utils.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    21848 2024-04-27 00:58:26.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/test.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3650 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/tiny_spacenet.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3788 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/utils.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2990 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/pytorch_chip_classification.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2344 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/pytorch_chip_classification_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7949 2024-04-07 00:38:15.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/pytorch_learner_backend.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3575 2024-04-10 21:55:10.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/pytorch_learner_backend_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4908 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/pytorch_object_detection.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2349 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/pytorch_object_detection_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3417 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/pytorch_semantic_segmentation.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2401 2024-04-06 20:13:30.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/pytorch_semantic_segmentation_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1363 2024-04-07 00:38:15.000000 rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/utils.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:14.363126 rastervision_pytorch_backend-0.30.1/rastervision_pytorch_backend.egg-info/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      586 2024-05-06 21:02:14.000000 rastervision_pytorch_backend-0.30.1/rastervision_pytorch_backend.egg-info/PKG-INFO
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2338 2024-05-06 21:02:14.000000 rastervision_pytorch_backend-0.30.1/rastervision_pytorch_backend.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-05-06 21:02:14.000000 rastervision_pytorch_backend-0.30.1/rastervision_pytorch_backend.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-05-06 21:02:14.000000 rastervision_pytorch_backend-0.30.1/rastervision_pytorch_backend.egg-info/not-zip-safe
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       89 2024-05-06 21:02:14.000000 rastervision_pytorch_backend-0.30.1/rastervision_pytorch_backend.egg-info/requires.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       13 2024-05-06 21:02:14.000000 rastervision_pytorch_backend-0.30.1/rastervision_pytorch_backend.egg-info/top_level.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      121 2024-05-06 20:16:58.000000 rastervision_pytorch_backend-0.30.1/requirements.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-05-06 21:02:14.363126 rastervision_pytorch_backend-0.30.1/setup.cfg
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1753 2024-05-06 20:16:58.000000 rastervision_pytorch_backend-0.30.1/setup.py
```

### Comparing `rastervision_pytorch_backend-0.30.0/PKG-INFO` & `rastervision_pytorch_backend-0.30.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision_pytorch_backend
-Version: 0.30.0
+Version: 0.30.1
 Summary: A rastervision plugin that adds PyTorch backends for rastervision.core pipelines
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/__init__.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/chip_classification/spacenet_rio.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/chip_classification/spacenet_rio.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/merge_geojson.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/merge_geojson.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/prepare_potsdam.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/prepare_potsdam.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/resample_geotiffs.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/resample_geotiffs.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/transfer_georeference.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/object_detection/cowc_potsdam_data_prep/transfer_georeference.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/object_detection/xview.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/object_detection/xview.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/isprs_potsdam.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/semantic_segmentation/isprs_potsdam.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/isprs_potsdam_multi_source.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/semantic_segmentation/isprs_potsdam_multi_source.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/spacenet_vegas.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/semantic_segmentation/spacenet_vegas.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/semantic_segmentation/utils.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/semantic_segmentation/utils.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/test.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/test.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/tiny_spacenet.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/tiny_spacenet.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/examples/utils.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/examples/utils.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_chip_classification.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/pytorch_chip_classification.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_chip_classification_config.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/pytorch_chip_classification_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_learner_backend.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/pytorch_learner_backend.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_learner_backend_config.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/pytorch_learner_backend_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_object_detection.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/pytorch_object_detection.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_object_detection_config.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/pytorch_object_detection_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_semantic_segmentation.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/pytorch_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/pytorch_semantic_segmentation_config.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/pytorch_semantic_segmentation_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision/pytorch_backend/utils.py` & `rastervision_pytorch_backend-0.30.1/rastervision/pytorch_backend/utils.py`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/PKG-INFO` & `rastervision_pytorch_backend-0.30.1/rastervision_pytorch_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision-pytorch-backend
-Version: 0.30.0
+Version: 0.30.1
 Summary: A rastervision plugin that adds PyTorch backends for rastervision.core pipelines
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_pytorch_backend-0.30.0/rastervision_pytorch_backend.egg-info/SOURCES.txt` & `rastervision_pytorch_backend-0.30.1/rastervision_pytorch_backend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rastervision_pytorch_backend-0.30.0/setup.py` & `rastervision_pytorch_backend-0.30.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 from os.path import abspath, dirname, join
 from setuptools import setup, find_namespace_packages
 import re
 
 name = 'rastervision_pytorch_backend'
-version = '0.30.0'
+version = '0.30.1'
 description = 'A rastervision plugin that adds PyTorch backends for rastervision.core pipelines'
 requirement_constraints = {}
 
 here = abspath(dirname(__file__))
 
 
 def parse_requirements(requirements_path: str) -> list[str]:
```

