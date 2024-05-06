# Comparing `tmp/picsellia-6.9.0.tar.gz` & `tmp/picsellia-6.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picsellia-6.9.0.tar", max compression
+gzip compressed data, was "picsellia-6.9.1.tar", max compression
```

## Comparing `picsellia-6.9.0.tar` & `picsellia-6.9.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    11678 2023-07-10 14:26:30.067305 picsellia-6.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2023-03-15 15:46:10.361461 picsellia-6.9.0/LICENSE
--rw-r--r--   0        0        0     1660 2023-05-10 08:40:15.009117 picsellia-6.9.0/README.md
--rw-r--r--   0        0        0     2590 2023-07-10 14:26:30.067305 picsellia-6.9.0/picsellia/__init__.py
--rw-r--r--   0        0        0    39378 2023-07-10 14:02:19.237641 picsellia-6.9.0/picsellia/client.py
--rw-r--r--   0        0        0      267 2022-10-18 10:06:13.118336 picsellia-6.9.0/picsellia/colors.py
--rw-r--r--   0        0        0     1706 2023-05-10 08:40:15.013117 picsellia-6.9.0/picsellia/decorators.py
--rw-r--r--   0        0        0     4918 2023-06-16 13:05:20.597718 picsellia-6.9.0/picsellia/exceptions.py
--rw-r--r--   0        0        0     3342 2023-07-10 14:02:19.237641 picsellia-6.9.0/picsellia/exif.py
--rw-r--r--   0        0        0     3410 2023-05-10 08:40:15.013117 picsellia-6.9.0/picsellia/pxl_multithreading.py
--rw-r--r--   0        0        0        0 2022-08-09 13:11:44.816343 picsellia-6.9.0/picsellia/sdk/__init__.py
--rw-r--r--   0        0        0    21739 2023-03-15 15:46:10.365461 picsellia-6.9.0/picsellia/sdk/annotation.py
--rw-r--r--   0        0        0     3227 2023-05-10 08:40:15.013117 picsellia-6.9.0/picsellia/sdk/artifact.py
--rw-r--r--   0        0        0    17063 2023-06-16 13:11:15.864325 picsellia-6.9.0/picsellia/sdk/asset.py
--rw-r--r--   0        0        0     2509 2023-03-15 15:46:10.365461 picsellia-6.9.0/picsellia/sdk/classification.py
--rw-r--r--   0        0        0    19558 2023-06-16 07:22:12.477468 picsellia-6.9.0/picsellia/sdk/connexion.py
--rw-r--r--   0        0        0     1986 2023-03-15 15:46:10.365461 picsellia-6.9.0/picsellia/sdk/dao.py
--rw-r--r--   0        0        0     9259 2023-06-16 13:11:15.864325 picsellia-6.9.0/picsellia/sdk/data.py
--rw-r--r--   0        0        0    18388 2023-07-10 14:02:19.241641 picsellia-6.9.0/picsellia/sdk/datalake.py
--rw-r--r--   0        0        0     7203 2023-05-10 08:40:15.017117 picsellia-6.9.0/picsellia/sdk/dataset.py
--rw-r--r--   0        0        0    60790 2023-07-06 07:37:34.607828 picsellia-6.9.0/picsellia/sdk/dataset_version.py
--rw-r--r--   0        0        0     2113 2023-03-15 15:46:10.369461 picsellia-6.9.0/picsellia/sdk/datasource.py
--rw-r--r--   0        0        0    38557 2023-07-10 14:02:19.241641 picsellia-6.9.0/picsellia/sdk/deployment.py
--rw-r--r--   0        0        0     3485 2023-05-10 08:40:15.017117 picsellia-6.9.0/picsellia/sdk/downloadable.py
--rw-r--r--   0        0        0     4219 2023-05-10 08:40:15.017117 picsellia-6.9.0/picsellia/sdk/evaluation.py
--rw-r--r--   0        0        0    40734 2023-06-21 12:38:00.020248 picsellia-6.9.0/picsellia/sdk/experiment.py
--rw-r--r--   0        0        0     8130 2023-06-16 13:05:20.597718 picsellia-6.9.0/picsellia/sdk/job.py
--rw-r--r--   0        0        0     2096 2023-03-15 15:46:10.373461 picsellia-6.9.0/picsellia/sdk/label.py
--rw-r--r--   0        0        0     2871 2023-03-15 15:46:10.373461 picsellia-6.9.0/picsellia/sdk/line.py
--rw-r--r--   0        0        0     3473 2023-03-15 15:46:10.373461 picsellia-6.9.0/picsellia/sdk/log.py
--rw-r--r--   0        0        0     2872 2023-05-10 08:40:15.017117 picsellia-6.9.0/picsellia/sdk/logging_file.py
--rw-r--r--   0        0        0     8755 2023-07-10 14:02:19.241641 picsellia-6.9.0/picsellia/sdk/model.py
--rw-r--r--   0        0        0     5061 2023-03-15 15:46:10.373461 picsellia-6.9.0/picsellia/sdk/model_context.py
--rw-r--r--   0        0        0     2311 2023-05-10 08:40:15.017117 picsellia-6.9.0/picsellia/sdk/model_file.py
--rw-r--r--   0        0        0    12952 2023-07-10 14:02:19.241641 picsellia-6.9.0/picsellia/sdk/model_version.py
--rw-r--r--   0        0        0     4453 2023-05-05 09:14:03.113478 picsellia-6.9.0/picsellia/sdk/multi_object.py
--rw-r--r--   0        0        0     3024 2023-03-15 15:46:10.373461 picsellia-6.9.0/picsellia/sdk/point.py
--rw-r--r--   0        0        0     2926 2023-03-15 15:46:10.373461 picsellia-6.9.0/picsellia/sdk/polygon.py
--rw-r--r--   0        0        0    16844 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/sdk/project.py
--rw-r--r--   0        0        0     3403 2023-03-15 15:46:10.377461 picsellia-6.9.0/picsellia/sdk/rectangle.py
--rw-r--r--   0        0        0     5374 2023-03-15 15:46:10.377461 picsellia-6.9.0/picsellia/sdk/run.py
--rw-r--r--   0        0        0     6923 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/sdk/scan.py
--rw-r--r--   0        0        0     3103 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/sdk/scan_file.py
--rw-r--r--   0        0        0     4417 2023-03-15 15:46:10.377461 picsellia-6.9.0/picsellia/sdk/tag.py
--rw-r--r--   0        0        0     2959 2023-03-15 15:46:10.377461 picsellia-6.9.0/picsellia/sdk/taggable.py
--rw-r--r--   0        0        0     1492 2023-03-15 15:46:10.377461 picsellia-6.9.0/picsellia/sdk/worker.py
--rw-r--r--   0        0        0        0 2023-03-15 15:46:10.377461 picsellia-6.9.0/picsellia/services/__init__.py
--rw-r--r--   0        0        0     2112 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/services/asset_splitter.py
--rw-r--r--   0        0        0     5988 2023-03-15 15:46:10.377461 picsellia-6.9.0/picsellia/services/coco_file_builder.py
--rw-r--r--   0        0        0     3558 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/services/coco_importer.py
--rw-r--r--   0        0        0     1941 2023-03-15 15:46:10.377461 picsellia-6.9.0/picsellia/services/datasource.py
--rw-r--r--   0        0        0      798 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/services/error_manager.py
--rw-r--r--   0        0        0      974 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/services/splitter.py
--rw-r--r--   0        0        0     2658 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/services/voc_importer.py
--rw-r--r--   0        0        0     8268 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/services/yolo_importer.py
--rw-r--r--   0        0        0        0 2022-08-09 13:11:44.820343 picsellia-6.9.0/picsellia/types/__init__.py
--rw-r--r--   0        0        0     4572 2023-06-16 07:21:46.349339 picsellia-6.9.0/picsellia/types/enums.py
--rw-r--r--   0        0        0     4588 2023-06-16 13:11:15.864325 picsellia-6.9.0/picsellia/types/schemas.py
--rw-r--r--   0        0        0     3658 2023-05-10 08:40:15.021117 picsellia-6.9.0/picsellia/types/schemas_prediction.py
--rw-r--r--   0        0        0     7735 2023-07-10 14:02:19.241641 picsellia-6.9.0/picsellia/utils.py
--rw-r--r--   0        0        0     1368 2023-07-10 14:26:30.067305 picsellia-6.9.0/pyproject.toml
--rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 picsellia-6.9.0/setup.py
--rw-r--r--   0        0        0     3153 1970-01-01 00:00:00.000000 picsellia-6.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11830 2023-09-06 07:32:26.499931 picsellia-6.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2023-03-15 15:46:10.361461 picsellia-6.9.1/LICENSE
+-rw-r--r--   0        0        0     1660 2023-05-10 08:40:15.009117 picsellia-6.9.1/README.md
+-rw-r--r--   0        0        0     2590 2023-09-06 07:32:43.320069 picsellia-6.9.1/picsellia/__init__.py
+-rw-r--r--   0        0        0    39378 2023-09-06 07:29:34.198200 picsellia-6.9.1/picsellia/client.py
+-rw-r--r--   0        0        0      267 2022-10-18 10:06:13.118336 picsellia-6.9.1/picsellia/colors.py
+-rw-r--r--   0        0        0     1706 2023-07-13 10:22:09.880352 picsellia-6.9.1/picsellia/decorators.py
+-rw-r--r--   0        0        0     4918 2023-06-16 13:05:20.597718 picsellia-6.9.1/picsellia/exceptions.py
+-rw-r--r--   0        0        0     3342 2023-07-10 14:02:19.237641 picsellia-6.9.1/picsellia/exif.py
+-rw-r--r--   0        0        0     3410 2023-05-10 08:40:15.013117 picsellia-6.9.1/picsellia/pxl_multithreading.py
+-rw-r--r--   0        0        0        0 2022-08-09 13:11:44.816343 picsellia-6.9.1/picsellia/sdk/__init__.py
+-rw-r--r--   0        0        0    21739 2023-03-15 15:46:10.365461 picsellia-6.9.1/picsellia/sdk/annotation.py
+-rw-r--r--   0        0        0     3227 2023-05-10 08:40:15.013117 picsellia-6.9.1/picsellia/sdk/artifact.py
+-rw-r--r--   0        0        0    17063 2023-06-16 13:11:15.864325 picsellia-6.9.1/picsellia/sdk/asset.py
+-rw-r--r--   0        0        0     2509 2023-03-15 15:46:10.365461 picsellia-6.9.1/picsellia/sdk/classification.py
+-rw-r--r--   0        0        0    19558 2023-09-06 07:29:34.198200 picsellia-6.9.1/picsellia/sdk/connexion.py
+-rw-r--r--   0        0        0     1986 2023-03-15 15:46:10.365461 picsellia-6.9.1/picsellia/sdk/dao.py
+-rw-r--r--   0        0        0     9259 2023-06-16 13:11:15.864325 picsellia-6.9.1/picsellia/sdk/data.py
+-rw-r--r--   0        0        0    18388 2023-07-10 14:02:19.241641 picsellia-6.9.1/picsellia/sdk/datalake.py
+-rw-r--r--   0        0        0     7203 2023-09-06 07:29:34.198200 picsellia-6.9.1/picsellia/sdk/dataset.py
+-rw-r--r--   0        0        0    60790 2023-07-06 07:37:34.607828 picsellia-6.9.1/picsellia/sdk/dataset_version.py
+-rw-r--r--   0        0        0     2113 2023-03-15 15:46:10.369461 picsellia-6.9.1/picsellia/sdk/datasource.py
+-rw-r--r--   0        0        0    38772 2023-09-06 07:29:38.154247 picsellia-6.9.1/picsellia/sdk/deployment.py
+-rw-r--r--   0        0        0     3485 2023-05-10 08:40:15.017117 picsellia-6.9.1/picsellia/sdk/downloadable.py
+-rw-r--r--   0        0        0     4219 2023-05-10 08:40:15.017117 picsellia-6.9.1/picsellia/sdk/evaluation.py
+-rw-r--r--   0        0        0    40734 2023-06-21 12:38:00.020248 picsellia-6.9.1/picsellia/sdk/experiment.py
+-rw-r--r--   0        0        0     8130 2023-06-16 13:05:20.597718 picsellia-6.9.1/picsellia/sdk/job.py
+-rw-r--r--   0        0        0     2096 2023-03-15 15:46:10.373461 picsellia-6.9.1/picsellia/sdk/label.py
+-rw-r--r--   0        0        0     2871 2023-03-15 15:46:10.373461 picsellia-6.9.1/picsellia/sdk/line.py
+-rw-r--r--   0        0        0     3473 2023-03-15 15:46:10.373461 picsellia-6.9.1/picsellia/sdk/log.py
+-rw-r--r--   0        0        0     2872 2023-05-10 08:40:15.017117 picsellia-6.9.1/picsellia/sdk/logging_file.py
+-rw-r--r--   0        0        0     8755 2023-09-06 07:29:34.198200 picsellia-6.9.1/picsellia/sdk/model.py
+-rw-r--r--   0        0        0     5061 2023-03-15 15:46:10.373461 picsellia-6.9.1/picsellia/sdk/model_context.py
+-rw-r--r--   0        0        0     2311 2023-05-10 08:40:15.017117 picsellia-6.9.1/picsellia/sdk/model_file.py
+-rw-r--r--   0        0        0    12952 2023-07-10 14:02:19.241641 picsellia-6.9.1/picsellia/sdk/model_version.py
+-rw-r--r--   0        0        0     4453 2023-05-05 09:14:03.113478 picsellia-6.9.1/picsellia/sdk/multi_object.py
+-rw-r--r--   0        0        0     3024 2023-03-15 15:46:10.373461 picsellia-6.9.1/picsellia/sdk/point.py
+-rw-r--r--   0        0        0     2926 2023-03-15 15:46:10.373461 picsellia-6.9.1/picsellia/sdk/polygon.py
+-rw-r--r--   0        0        0    16844 2023-09-06 07:29:34.198200 picsellia-6.9.1/picsellia/sdk/project.py
+-rw-r--r--   0        0        0     3403 2023-03-15 15:46:10.377461 picsellia-6.9.1/picsellia/sdk/rectangle.py
+-rw-r--r--   0        0        0     5374 2023-09-04 16:37:35.924696 picsellia-6.9.1/picsellia/sdk/run.py
+-rw-r--r--   0        0        0     6923 2023-09-04 16:37:35.924696 picsellia-6.9.1/picsellia/sdk/scan.py
+-rw-r--r--   0        0        0     3103 2023-09-04 16:37:35.924696 picsellia-6.9.1/picsellia/sdk/scan_file.py
+-rw-r--r--   0        0        0     4417 2023-03-15 15:46:10.377461 picsellia-6.9.1/picsellia/sdk/tag.py
+-rw-r--r--   0        0        0     2959 2023-03-15 15:46:10.377461 picsellia-6.9.1/picsellia/sdk/taggable.py
+-rw-r--r--   0        0        0     1492 2023-03-15 15:46:10.377461 picsellia-6.9.1/picsellia/sdk/worker.py
+-rw-r--r--   0        0        0        0 2023-03-15 15:46:10.377461 picsellia-6.9.1/picsellia/services/__init__.py
+-rw-r--r--   0        0        0     2112 2023-05-10 08:40:15.021117 picsellia-6.9.1/picsellia/services/asset_splitter.py
+-rw-r--r--   0        0        0     5988 2023-09-06 07:29:34.198200 picsellia-6.9.1/picsellia/services/coco_file_builder.py
+-rw-r--r--   0        0        0     3558 2023-05-10 08:40:15.021117 picsellia-6.9.1/picsellia/services/coco_importer.py
+-rw-r--r--   0        0        0     1941 2023-03-15 15:46:10.377461 picsellia-6.9.1/picsellia/services/datasource.py
+-rw-r--r--   0        0        0      798 2023-05-10 08:40:15.021117 picsellia-6.9.1/picsellia/services/error_manager.py
+-rw-r--r--   0        0        0      974 2023-05-10 08:40:15.021117 picsellia-6.9.1/picsellia/services/splitter.py
+-rw-r--r--   0        0        0     2658 2023-05-10 08:40:15.021117 picsellia-6.9.1/picsellia/services/voc_importer.py
+-rw-r--r--   0        0        0     8268 2023-05-10 08:40:15.021117 picsellia-6.9.1/picsellia/services/yolo_importer.py
+-rw-r--r--   0        0        0        0 2022-08-09 13:11:44.820343 picsellia-6.9.1/picsellia/types/__init__.py
+-rw-r--r--   0        0        0     4572 2023-06-16 07:21:46.349339 picsellia-6.9.1/picsellia/types/enums.py
+-rw-r--r--   0        0        0     4588 2023-09-04 16:37:35.924696 picsellia-6.9.1/picsellia/types/schemas.py
+-rw-r--r--   0        0        0     3658 2023-08-21 13:45:42.155054 picsellia-6.9.1/picsellia/types/schemas_prediction.py
+-rw-r--r--   0        0        0     7735 2023-07-10 14:02:19.241641 picsellia-6.9.1/picsellia/utils.py
+-rw-r--r--   0        0        0     1368 2023-09-06 07:32:54.552158 picsellia-6.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 picsellia-6.9.1/setup.py
+-rw-r--r--   0        0        0     3153 1970-01-01 00:00:00.000000 picsellia-6.9.1/PKG-INFO
```

### Comparing `picsellia-6.9.0/CHANGELOG.md` & `picsellia-6.9.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 
 # Changelog
 
 Picsellia SDK Python is a library that allows users to connect to Picsellia backend.
 
 All notable changes to this project will be documented in this file.
 
+## [6.9.1] - 2023-09-06
+
+### Fixed
+- `Deployment.predict_bytes()` needs parameter `filename` to work. It was sending prediction with filename `media`.
+
 ## [6.9.0] - 2023-07-10
 
 ### Added
 - `Datalake.upload()` can now be called with parameter `fill_metadata`. On upload, set this parameter to True to read exif metadata flags and push metadata to Picsellia. By default, `fill_metadata` is False.
 - `Client.get_datalake()` can now be called with parameter `id` or `name` to retrieve the Datalake you want. If nothing is given, this method will retrieve your default datalake.
 - `Deployment.predict_bytes()` can now be called if you want to send image as bytes on Serving service
 - `ModelVersion.update()` and `Model.create_version()` can now be called with `docker_tag` parameter
```

### Comparing `picsellia-6.9.0/LICENSE` & `picsellia-6.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/README.md` & `picsellia-6.9.1/README.md`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/__init__.py` & `picsellia-6.9.1/picsellia/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "6.9.0"
+__version__ = "6.9.1"
 
 import logging.config
 import os
 
 from picsellia.client import Client
 from picsellia.sdk.annotation import Annotation
 from picsellia.sdk.artifact import Artifact
```

### Comparing `picsellia-6.9.0/picsellia/client.py` & `picsellia-6.9.1/picsellia/client.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/decorators.py` & `picsellia-6.9.1/picsellia/decorators.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/exceptions.py` & `picsellia-6.9.1/picsellia/exceptions.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/exif.py` & `picsellia-6.9.1/picsellia/exif.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/pxl_multithreading.py` & `picsellia-6.9.1/picsellia/pxl_multithreading.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/annotation.py` & `picsellia-6.9.1/picsellia/sdk/annotation.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/artifact.py` & `picsellia-6.9.1/picsellia/sdk/artifact.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/asset.py` & `picsellia-6.9.1/picsellia/sdk/asset.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/classification.py` & `picsellia-6.9.1/picsellia/sdk/classification.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/connexion.py` & `picsellia-6.9.1/picsellia/sdk/connexion.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/dao.py` & `picsellia-6.9.1/picsellia/sdk/dao.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/data.py` & `picsellia-6.9.1/picsellia/sdk/data.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/datalake.py` & `picsellia-6.9.1/picsellia/sdk/datalake.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/dataset.py` & `picsellia-6.9.1/picsellia/sdk/dataset.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/dataset_version.py` & `picsellia-6.9.1/picsellia/sdk/dataset_version.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/datasource.py` & `picsellia-6.9.1/picsellia/sdk/datasource.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/deployment.py` & `picsellia-6.9.1/picsellia/sdk/deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,36 +316,42 @@
             source (str or DataSource, optional): a source to attach to the data that will be created on the platform.
 
         Returns:
             A (dict) with information of the prediction
         """
         with open(file_path, "rb") as file:
             file_data = file.read()
-            return self.predict_bytes(raw_image=file_data, tags=tags, source=source)
+            filename = Path(file_path).name
+            return self.predict_bytes(
+                filename=filename, raw_image=file_data, tags=tags, source=source
+            )
 
     @exception_handler
     @beartype
     def predict_bytes(
         self,
+        filename: str,
         raw_image: bytes,
         tags: Union[str, Tag, List[Union[Tag, str]], None] = None,
         source: Union[str, DataSource, None] = None,
     ) -> dict:
         """Run a prediction on our Serving platform
 
         Examples:
             ```python
             deployment = client.get_deployment(
                 name="awesome-deploy"
             )
-            with open('image_420.png', 'rb') as img:
+            filename = "frame.png"
+            with open(filename, 'rb') as img:
                 img_bytes = img.read()
-            deployment.predict_bytes(img_bytes, tags=["gonna", "give"], source="camera-1")
+            deployment.predict_bytes(filename, img_bytes, tags=["tag1", "tag2"], source="camera-1")
             ```
         Arguments:
+            filename (str): filename of the image.
             raw_image (bytes): bytes of the image to predict.
             tags (str, (Tag), list of str or Tag, optional): a list of tag to add to the data that will be created on the platform.
             source (str or DataSource, optional): a source to attach to the data that will be created on the platform.
 
         Returns:
             A (dict) with information of the prediction
         """
@@ -361,15 +367,15 @@
                 else:
                     sent_tags.append(tag)
 
         if isinstance(source, DataSource):
             source = source.name
 
         payload = {"tags": sent_tags}
-        files = {"media": raw_image}
+        files = {"media": (filename, raw_image)}
 
         if source:
             payload["source"] = source
 
         resp = self.serving_connexion.post(
             path=f"/api/deployment/{self.id}/predict",
             data=payload,
@@ -880,19 +886,18 @@
         if not content_type:
             content_type = mimetypes.guess_type(image_path, strict=False)[0]
             if content_type is None:  # pragma: no cover
                 raise ContentTypeUnknown(
                     f"Content type of {image_path} could not be inferred"
                 )
 
-        filename = image_path.split("/")[-1]
-
         # Open image, encode it into base64, read filename and content type.
         with open(image_path, "rb") as img_file:
             raw_image = img_file.read()
+            filename = Path(image_path).name
 
         return self.monitor_bytes(
             raw_image,
             content_type,
             filename,
             latency,
             height,
```

### Comparing `picsellia-6.9.0/picsellia/sdk/downloadable.py` & `picsellia-6.9.1/picsellia/sdk/downloadable.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/evaluation.py` & `picsellia-6.9.1/picsellia/sdk/evaluation.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/experiment.py` & `picsellia-6.9.1/picsellia/sdk/experiment.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/job.py` & `picsellia-6.9.1/picsellia/sdk/job.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/label.py` & `picsellia-6.9.1/picsellia/sdk/label.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/line.py` & `picsellia-6.9.1/picsellia/sdk/line.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/log.py` & `picsellia-6.9.1/picsellia/sdk/log.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/logging_file.py` & `picsellia-6.9.1/picsellia/sdk/logging_file.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/model.py` & `picsellia-6.9.1/picsellia/sdk/model.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/model_context.py` & `picsellia-6.9.1/picsellia/sdk/model_context.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/model_file.py` & `picsellia-6.9.1/picsellia/sdk/model_file.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/model_version.py` & `picsellia-6.9.1/picsellia/sdk/model_version.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/multi_object.py` & `picsellia-6.9.1/picsellia/sdk/multi_object.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/point.py` & `picsellia-6.9.1/picsellia/sdk/point.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/polygon.py` & `picsellia-6.9.1/picsellia/sdk/polygon.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/project.py` & `picsellia-6.9.1/picsellia/sdk/project.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/rectangle.py` & `picsellia-6.9.1/picsellia/sdk/rectangle.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/run.py` & `picsellia-6.9.1/picsellia/sdk/run.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/scan.py` & `picsellia-6.9.1/picsellia/sdk/scan.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/scan_file.py` & `picsellia-6.9.1/picsellia/sdk/scan_file.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/tag.py` & `picsellia-6.9.1/picsellia/sdk/tag.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/taggable.py` & `picsellia-6.9.1/picsellia/sdk/taggable.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/sdk/worker.py` & `picsellia-6.9.1/picsellia/sdk/worker.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/services/asset_splitter.py` & `picsellia-6.9.1/picsellia/services/asset_splitter.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/services/coco_file_builder.py` & `picsellia-6.9.1/picsellia/services/coco_file_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/services/coco_importer.py` & `picsellia-6.9.1/picsellia/services/coco_importer.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/services/datasource.py` & `picsellia-6.9.1/picsellia/services/datasource.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/services/error_manager.py` & `picsellia-6.9.1/picsellia/services/error_manager.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/services/splitter.py` & `picsellia-6.9.1/picsellia/services/splitter.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/services/voc_importer.py` & `picsellia-6.9.1/picsellia/services/voc_importer.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/services/yolo_importer.py` & `picsellia-6.9.1/picsellia/services/yolo_importer.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/types/enums.py` & `picsellia-6.9.1/picsellia/types/enums.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/types/schemas.py` & `picsellia-6.9.1/picsellia/types/schemas.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/types/schemas_prediction.py` & `picsellia-6.9.1/picsellia/types/schemas_prediction.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/picsellia/utils.py` & `picsellia-6.9.1/picsellia/utils.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.9.0/pyproject.toml` & `picsellia-6.9.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 src_paths = ["picsellia", "tests"]
 
 [tool.pycln]
 all = true
 
 [tool.poetry]
 name = "picsellia"
-version = "6.9.0"
+version = "6.9.1"
 description = "Python SDK package for Picsellia MLOps platform"
 authors = ["Pierre-Nicolas Tiffreau <pierre-nicolas@picsellia.com>", "Thomas Darget <thomas.darget@picsellia.com>"]
 maintainers = ["Pierre-Nicolas Tiffreau <pierre-nicolas@picsellia.com>", "Thomas Darget <thomas.darget@picsellia.com>", "Lucien Haurat <lucien.haurat@picsellia.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.picsellia.com/"
 documentation = "https://documentation.picsellia.com/reference/client"
```

### Comparing `picsellia-6.9.0/setup.py` & `picsellia-6.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'pydantic>=1.9.1,<2.0.0',
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.1,<3.0.0',
  'tdqm>=0.0.1,<0.0.2']
 
 setup_kwargs = {
     'name': 'picsellia',
-    'version': '6.9.0',
+    'version': '6.9.1',
     'description': 'Python SDK package for Picsellia MLOps platform',
     'long_description': '# Picsellia SDK\n\nPicsellia Python SDK is a python library that allows connecting to Picsellia platform.\n\n## Documentation\n\nReference of the SDK can be found at [reference](https://documentation.picsellia.com/reference/client)\n\n## Getting started\nDocumentation can be found at [docs](https://documentation.picsellia.com/docs/getting-started).\nStart by installing the Picsellia python package in your environment.\n```\npip install picsellia\n```\n\nThen, initialize a client\n```python\nfrom picsellia import Client\nclient = Client(api_token=<your api token>)\n```\n\nNow, use it to upload data and create a dataset !\n```python\nlake = client.get_datalake()\nuploaded_data = lake.upload_data(filepaths=["pics/twingo.png", "pics/ferrari.png"], tags=["tag_car"])\n\ndataset = client.create_dataset("cars").create_version("first")\ndataset.add_data(uploaded_data)\n```\n\n## What is Picsellia ?\n\nOur mission is to give you all the necessary tools to relieve the burden of AI projects off of your shoulders. As a data scientist / ML engineer / Researcher, you shouldn\'t have to worry about the following topics :\n\n- [💾 Data Management](https://documentation.picsellia.com/docs/data-management)\n- [📈 Experiment Tracking](https://documentation.picsellia.com/docs/experiment-tracking)\n- [📘 Model Management](https://documentation.picsellia.com/docs/export-an-experiment)\n- [🚀 Model Deployment](https://documentation.picsellia.com/docs/serverless)\n- [👀 Model Monitoring](https://documentation.picsellia.com/docs/monitor-model)\n\nPicsellia is the one-stop place for all the life-cycle of your Computer Vision projects, from ideation to production in a single platform 🚀.\n',
     'author': 'Pierre-Nicolas Tiffreau',
     'author_email': 'pierre-nicolas@picsellia.com',
     'maintainer': 'Pierre-Nicolas Tiffreau',
     'maintainer_email': 'pierre-nicolas@picsellia.com',
     'url': 'https://www.picsellia.com/',
```

### Comparing `picsellia-6.9.0/PKG-INFO` & `picsellia-6.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picsellia
-Version: 6.9.0
+Version: 6.9.1
 Summary: Python SDK package for Picsellia MLOps platform
 Home-page: https://www.picsellia.com/
 License: MIT
 Keywords: ai,picsellia,sdk,cvops
 Author: Pierre-Nicolas Tiffreau
 Author-email: pierre-nicolas@picsellia.com
 Maintainer: Pierre-Nicolas Tiffreau
```

