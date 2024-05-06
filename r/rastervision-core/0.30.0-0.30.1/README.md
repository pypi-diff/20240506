# Comparing `tmp/rastervision_core-0.30.0.tar.gz` & `tmp/rastervision_core-0.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastervision_core-0.30.0.tar", last modified: Wed Apr 10 22:11:08 2024, max compression
+gzip compressed data, was "rastervision_core-0.30.1.tar", last modified: Mon May  6 21:02:13 2024, max compression
```

## Comparing `rastervision_core-0.30.0.tar` & `rastervision_core-0.30.1.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.951692 rastervision_core-0.30.0/
--rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/MANIFEST.in
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      564 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/PKG-INFO
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.939692 rastervision_core-0.30.0/rastervision/
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.939692 rastervision_core-0.30.0/rastervision/core/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      744 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/__init__.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.939692 rastervision_core-0.30.0/rastervision/core/analyzer/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      371 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/analyzer/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      404 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/analyzer/analyzer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      776 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/analyzer/analyzer_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1214 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/analyzer/stats_analyzer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2351 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/analyzer/stats_analyzer_config.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.939692 rastervision_core-0.30.0/rastervision/core/backend/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      184 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/backend/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2143 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/backend/backend.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1078 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/backend/backend_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    18054 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/box.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3880 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/cli.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.939692 rastervision_core-0.30.0/rastervision/core/data/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      663 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5315 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/class_config.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.939692 rastervision_core-0.30.0/rastervision/core/data/crs_transformer/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      359 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/crs_transformer/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6574 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/crs_transformer/crs_transformer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      745 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/crs_transformer/identity_crs_transformer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4873 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/crs_transformer/rasterio_crs_transformer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3477 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/dataset_config.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.943692 rastervision_core-0.30.0/rastervision/core/data/label/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      606 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/label/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6026 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/label/chip_classification_labels.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2506 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/label/labels.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    12458 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label/object_detection_labels.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    26544 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label/semantic_segmentation_labels.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.943692 rastervision_core-0.30.0/rastervision/core/data/label/tfod_utils/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       15 2023-08-22 15:58:07.000000 rastervision_core-0.30.0/rastervision/core/data/label/tfod_utils/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4365 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label/tfod_utils/np_box_list.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    23023 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label/tfod_utils/np_box_list_ops.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3498 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label/tfod_utils/np_box_ops.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1091 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label/utils.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.943692 rastervision_core-0.30.0/rastervision/core/data/label_source/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1019 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    10328 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/chip_classification_label_source.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4782 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/chip_classification_label_source_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1792 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/label_source.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      897 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/label_source_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5107 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/object_detection_label_source.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1817 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/object_detection_label_source_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3711 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/semantic_segmentation_label_source.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1376 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/semantic_segmentation_label_source_config.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.943692 rastervision_core-0.30.0/rastervision/core/data/label_store/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1211 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2799 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/chip_classification_geojson_store.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1085 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/chip_classification_geojson_store_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1116 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/label_store.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      892 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/label_store_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2825 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/object_detection_geojson_store.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1119 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/object_detection_geojson_store_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    15901 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/semantic_segmentation_label_store.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7087 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/semantic_segmentation_label_store_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2897 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/utils.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.943692 rastervision_core-0.30.0/rastervision/core/data/raster_source/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1343 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8218 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/multi_raster_source.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3717 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/multi_raster_source_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6584 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/raster_source.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2026 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/raster_source_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8740 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/rasterio_source.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1976 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/rasterio_source_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5570 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/rasterized_source.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2876 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/rasterized_source_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1760 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/stac_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5030 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/temporal_multi_raster_source.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    11943 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/xarray_source.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2225 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/xarray_source_config.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.943692 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1612 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      922 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/cast_transformer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      662 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/cast_transformer_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      712 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/min_max_transformer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      417 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/min_max_transformer_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      956 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/nan_transformer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      634 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/nan_transformer_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      837 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/raster_transformer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      550 2023-09-08 19:48:40.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/raster_transformer_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1405 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/reclass_transformer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      593 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/reclass_transformer_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2334 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/rgb_class_transformer.py
--rw-r--r--   0 ahassan   (1001) ahassan   (1001)      715 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/rgb_class_transformer_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5835 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/stats_transformer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2311 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/stats_transformer_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2814 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/scene.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3656 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/scene_config.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/rastervision/core/data/utils/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      380 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/data/utils/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7993 2024-04-09 23:04:37.000000 rastervision_core-0.30.0/rastervision/core/data/utils/aoi_sampler.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    14755 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/utils/factory.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    13266 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/utils/geojson.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8785 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/utils/misc.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2415 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/utils/raster.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8271 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/utils/rasterio.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6264 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/utils/vectorization.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/rastervision/core/data/vector_source/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      455 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/vector_source/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2024 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/vector_source/geojson_vector_source.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1491 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/vector_source/geojson_vector_source_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6518 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/vector_source/vector_source.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2345 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/vector_source/vector_source_config.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/
--rw-r--r--   0 ahassan   (1001) ahassan   (1001)      968 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1826 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/buffer_transformer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1834 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/buffer_transformer_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8483 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/class_inference_transformer.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2144 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/class_inference_transformer_config.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/label_maker/
--rw-r--r--   0 ahassan   (1001) ahassan   (1001)        0 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/label_maker/__init__.py
--rw-r--r--   0 ahassan   (1001) ahassan   (1001)     3488 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/label_maker/filter.py
--rw-r--r--   0 ahassan   (1001) ahassan   (1001)     2290 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/shift_transformer.py
--rw-r--r--   0 ahassan   (1001) ahassan   (1001)     1153 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/shift_transformer_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1213 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/vector_transformer.py
--rw-r--r--   0 ahassan   (1001) ahassan   (1001)      760 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/vector_transformer_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      402 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/data_sample.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/rastervision/core/evaluation/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1792 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/evaluation/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1596 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/evaluation/chip_classification_evaluation.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      458 2023-08-22 15:58:07.000000 rastervision_core-0.30.0/rastervision/core/evaluation/chip_classification_evaluator.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1030 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/evaluation/chip_classification_evaluator_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6285 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/evaluation/class_evaluation_item.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5510 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/evaluation/classification_evaluation.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1989 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/evaluation/classification_evaluator.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      289 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/evaluation/classification_evaluator_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      496 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/evaluation/evaluation_item.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1250 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/evaluation/evaluator.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1414 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/evaluation/evaluator_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4340 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/evaluation/object_detection_evaluation.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      342 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/evaluation/object_detection_evaluator.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1011 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/evaluation/object_detection_evaluator_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1826 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/evaluation/semantic_segmentation_evaluation.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1263 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/evaluation/semantic_segmentation_evaluator.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1366 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/evaluation/semantic_segmentation_evaluator_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8333 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/predictor.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    10644 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/raster_stats.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/rastervision/core/rv_pipeline/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1328 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      114 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/chip_classification.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      794 2024-02-06 21:37:22.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/chip_classification_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6655 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/chip_options.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       99 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/object_detection.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3509 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/object_detection_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     9327 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/rv_pipeline.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6672 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/rv_pipeline_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      104 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/semantic_segmentation.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5691 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/semantic_segmentation_config.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      798 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/utils.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/rastervision/core/utils/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      102 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/utils/__init__.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3261 2023-08-22 15:58:07.000000 rastervision_core-0.30.0/rastervision/core/utils/cog.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      981 2023-08-22 15:58:07.000000 rastervision_core-0.30.0/rastervision/core/utils/filter_geojson.py
--rw-r--r--   0 ahassan   (1001) ahassan   (1001)       65 2023-09-26 14:00:58.000000 rastervision_core-0.30.0/rastervision/core/utils/misc.py
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6240 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/utils/stac.py
-drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/rastervision_core.egg-info/
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      564 2024-04-10 22:11:08.000000 rastervision_core-0.30.0/rastervision_core.egg-info/PKG-INFO
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7852 2024-04-10 22:11:08.000000 rastervision_core-0.30.0/rastervision_core.egg-info/SOURCES.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 22:11:08.000000 rastervision_core-0.30.0/rastervision_core.egg-info/dependency_links.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 21:24:48.000000 rastervision_core-0.30.0/rastervision_core.egg-info/not-zip-safe
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      168 2024-04-10 22:11:08.000000 rastervision_core-0.30.0/rastervision_core.egg-info/requires.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       24 2024-04-10 22:11:08.000000 rastervision_core-0.30.0/rastervision_core.egg-info/top_level.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      308 2024-04-10 21:55:37.000000 rastervision_core-0.30.0/requirements.txt
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-04-10 22:11:08.951692 rastervision_core-0.30.0/setup.cfg
--rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1731 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/setup.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.847123 rastervision_core-0.30.1/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/MANIFEST.in
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      564 2024-05-06 21:02:13.847123 rastervision_core-0.30.1/PKG-INFO
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.835123 rastervision_core-0.30.1/rastervision/
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.839123 rastervision_core-0.30.1/rastervision/core/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      744 2024-04-10 21:55:10.000000 rastervision_core-0.30.1/rastervision/core/__init__.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.839123 rastervision_core-0.30.1/rastervision/core/analyzer/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      371 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/analyzer/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      404 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/analyzer/analyzer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      776 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/analyzer/analyzer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1214 2024-04-03 20:58:32.000000 rastervision_core-0.30.1/rastervision/core/analyzer/stats_analyzer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2351 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/analyzer/stats_analyzer_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.839123 rastervision_core-0.30.1/rastervision/core/backend/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      184 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/backend/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2143 2024-04-06 20:13:30.000000 rastervision_core-0.30.1/rastervision/core/backend/backend.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1078 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/backend/backend_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    18054 2024-04-10 21:55:10.000000 rastervision_core-0.30.1/rastervision/core/box.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3880 2024-04-17 14:19:05.000000 rastervision_core-0.30.1/rastervision/core/cli.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.839123 rastervision_core-0.30.1/rastervision/core/data/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      663 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/data/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5315 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/class_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.839123 rastervision_core-0.30.1/rastervision/core/data/crs_transformer/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      359 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/data/crs_transformer/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6574 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/crs_transformer/crs_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      745 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/data/crs_transformer/identity_crs_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4873 2024-04-10 21:55:10.000000 rastervision_core-0.30.1/rastervision/core/data/crs_transformer/rasterio_crs_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3828 2024-05-03 19:36:10.000000 rastervision_core-0.30.1/rastervision/core/data/dataset_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.839123 rastervision_core-0.30.1/rastervision/core/data/label/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      606 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/data/label/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6026 2024-04-10 21:55:10.000000 rastervision_core-0.30.1/rastervision/core/data/label/chip_classification_labels.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2506 2024-04-10 21:55:10.000000 rastervision_core-0.30.1/rastervision/core/data/label/labels.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    12458 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/label/object_detection_labels.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    26544 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/label/semantic_segmentation_labels.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.839123 rastervision_core-0.30.1/rastervision/core/data/label/tfod_utils/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       15 2023-08-22 15:58:07.000000 rastervision_core-0.30.1/rastervision/core/data/label/tfod_utils/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4365 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/label/tfod_utils/np_box_list.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    23023 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/label/tfod_utils/np_box_list_ops.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3498 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/label/tfod_utils/np_box_ops.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1091 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/label/utils.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.839123 rastervision_core-0.30.1/rastervision/core/data/label_source/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1019 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/data/label_source/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    10328 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/label_source/chip_classification_label_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4782 2024-04-06 20:13:30.000000 rastervision_core-0.30.1/rastervision/core/data/label_source/chip_classification_label_source_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1792 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/label_source/label_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      897 2024-04-03 20:58:32.000000 rastervision_core-0.30.1/rastervision/core/data/label_source/label_source_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5107 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/label_source/object_detection_label_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1817 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/data/label_source/object_detection_label_source_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3711 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/label_source/semantic_segmentation_label_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1376 2024-04-06 20:13:30.000000 rastervision_core-0.30.1/rastervision/core/data/label_source/semantic_segmentation_label_source_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.839123 rastervision_core-0.30.1/rastervision/core/data/label_store/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1211 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/data/label_store/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2799 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/label_store/chip_classification_geojson_store.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1085 2024-04-03 20:58:32.000000 rastervision_core-0.30.1/rastervision/core/data/label_store/chip_classification_geojson_store_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1116 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/label_store/label_store.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      892 2024-04-03 20:58:32.000000 rastervision_core-0.30.1/rastervision/core/data/label_store/label_store_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2825 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/label_store/object_detection_geojson_store.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1119 2024-04-03 20:58:32.000000 rastervision_core-0.30.1/rastervision/core/data/label_store/object_detection_geojson_store_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    15901 2024-04-10 21:55:10.000000 rastervision_core-0.30.1/rastervision/core/data/label_store/semantic_segmentation_label_store.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7087 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/label_store/semantic_segmentation_label_store_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2897 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/label_store/utils.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.843123 rastervision_core-0.30.1/rastervision/core/data/raster_source/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1343 2024-04-06 20:13:30.000000 rastervision_core-0.30.1/rastervision/core/data/raster_source/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8218 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/raster_source/multi_raster_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3717 2024-04-06 20:13:30.000000 rastervision_core-0.30.1/rastervision/core/data/raster_source/multi_raster_source_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6507 2024-05-03 19:36:02.000000 rastervision_core-0.30.1/rastervision/core/data/raster_source/raster_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2026 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/raster_source/raster_source_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8740 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/raster_source/rasterio_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1976 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/raster_source/rasterio_source_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5570 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/raster_source/rasterized_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2876 2024-04-03 20:58:32.000000 rastervision_core-0.30.1/rastervision/core/data/raster_source/rasterized_source_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1760 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/raster_source/stac_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5030 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/raster_source/temporal_multi_raster_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    11943 2024-04-10 21:55:10.000000 rastervision_core-0.30.1/rastervision/core/data/raster_source/xarray_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2225 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/raster_source/xarray_source_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.843123 rastervision_core-0.30.1/rastervision/core/data/raster_transformer/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1612 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/data/raster_transformer/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      922 2024-04-03 20:58:32.000000 rastervision_core-0.30.1/rastervision/core/data/raster_transformer/cast_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      662 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/data/raster_transformer/cast_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      712 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/raster_transformer/min_max_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      417 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/data/raster_transformer/min_max_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      956 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/data/raster_transformer/nan_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      634 2024-04-03 20:58:32.000000 rastervision_core-0.30.1/rastervision/core/data/raster_transformer/nan_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      837 2024-04-06 20:13:30.000000 rastervision_core-0.30.1/rastervision/core/data/raster_transformer/raster_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      550 2023-09-08 19:48:40.000000 rastervision_core-0.30.1/rastervision/core/data/raster_transformer/raster_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1405 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/raster_transformer/reclass_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      593 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/raster_transformer/reclass_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2334 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/raster_transformer/rgb_class_transformer.py
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)      715 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/data/raster_transformer/rgb_class_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5835 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/raster_transformer/stats_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2311 2024-04-03 20:58:32.000000 rastervision_core-0.30.1/rastervision/core/data/raster_transformer/stats_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2814 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/scene.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3656 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/scene_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.843123 rastervision_core-0.30.1/rastervision/core/data/utils/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      380 2024-04-06 20:13:30.000000 rastervision_core-0.30.1/rastervision/core/data/utils/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7993 2024-04-09 23:04:37.000000 rastervision_core-0.30.1/rastervision/core/data/utils/aoi_sampler.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    14755 2024-04-10 21:55:10.000000 rastervision_core-0.30.1/rastervision/core/data/utils/factory.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    13266 2024-04-10 21:55:10.000000 rastervision_core-0.30.1/rastervision/core/data/utils/geojson.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8785 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/utils/misc.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2415 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/utils/raster.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8271 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/utils/rasterio.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6264 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/utils/vectorization.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.843123 rastervision_core-0.30.1/rastervision/core/data/vector_source/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      455 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/data/vector_source/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2024 2024-04-10 21:55:10.000000 rastervision_core-0.30.1/rastervision/core/data/vector_source/geojson_vector_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1491 2024-04-10 21:55:10.000000 rastervision_core-0.30.1/rastervision/core/data/vector_source/geojson_vector_source_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6518 2024-04-10 21:55:10.000000 rastervision_core-0.30.1/rastervision/core/data/vector_source/vector_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2345 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/vector_source/vector_source_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.843123 rastervision_core-0.30.1/rastervision/core/data/vector_transformer/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)      968 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/data/vector_transformer/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1826 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/vector_transformer/buffer_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1834 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/vector_transformer/buffer_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8483 2024-04-10 21:55:10.000000 rastervision_core-0.30.1/rastervision/core/data/vector_transformer/class_inference_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2144 2024-04-10 21:55:10.000000 rastervision_core-0.30.1/rastervision/core/data/vector_transformer/class_inference_transformer_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.843123 rastervision_core-0.30.1/rastervision/core/data/vector_transformer/label_maker/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)        0 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/data/vector_transformer/label_maker/__init__.py
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)     3488 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/data/vector_transformer/label_maker/filter.py
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)     2290 2024-04-03 20:58:32.000000 rastervision_core-0.30.1/rastervision/core/data/vector_transformer/shift_transformer.py
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)     1153 2024-04-03 20:58:32.000000 rastervision_core-0.30.1/rastervision/core/data/vector_transformer/shift_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1213 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/data/vector_transformer/vector_transformer.py
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)      760 2024-04-03 20:58:32.000000 rastervision_core-0.30.1/rastervision/core/data/vector_transformer/vector_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      402 2024-04-06 20:13:30.000000 rastervision_core-0.30.1/rastervision/core/data_sample.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.843123 rastervision_core-0.30.1/rastervision/core/evaluation/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1792 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/evaluation/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1596 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/evaluation/chip_classification_evaluation.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      458 2023-08-22 15:58:07.000000 rastervision_core-0.30.1/rastervision/core/evaluation/chip_classification_evaluator.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1030 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/evaluation/chip_classification_evaluator_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6285 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/evaluation/class_evaluation_item.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5510 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/evaluation/classification_evaluation.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1989 2024-04-03 20:58:32.000000 rastervision_core-0.30.1/rastervision/core/evaluation/classification_evaluator.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      289 2024-04-06 20:13:30.000000 rastervision_core-0.30.1/rastervision/core/evaluation/classification_evaluator_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      496 2024-04-06 20:13:30.000000 rastervision_core-0.30.1/rastervision/core/evaluation/evaluation_item.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1250 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/evaluation/evaluator.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1414 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/evaluation/evaluator_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4340 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/evaluation/object_detection_evaluation.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      342 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/evaluation/object_detection_evaluator.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1011 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/evaluation/object_detection_evaluator_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1826 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/evaluation/semantic_segmentation_evaluation.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1263 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/evaluation/semantic_segmentation_evaluator.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1366 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/evaluation/semantic_segmentation_evaluator_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8333 2024-04-10 21:55:10.000000 rastervision_core-0.30.1/rastervision/core/predictor.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    10644 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/raster_stats.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.847123 rastervision_core-0.30.1/rastervision/core/rv_pipeline/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1328 2024-04-06 20:13:30.000000 rastervision_core-0.30.1/rastervision/core/rv_pipeline/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      114 2024-04-06 20:13:30.000000 rastervision_core-0.30.1/rastervision/core/rv_pipeline/chip_classification.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      794 2024-02-06 21:37:22.000000 rastervision_core-0.30.1/rastervision/core/rv_pipeline/chip_classification_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6655 2024-04-10 21:55:10.000000 rastervision_core-0.30.1/rastervision/core/rv_pipeline/chip_options.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       99 2024-04-06 20:13:30.000000 rastervision_core-0.30.1/rastervision/core/rv_pipeline/object_detection.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3509 2024-04-06 20:13:30.000000 rastervision_core-0.30.1/rastervision/core/rv_pipeline/object_detection_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     9327 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/rv_pipeline/rv_pipeline.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6672 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/rv_pipeline/rv_pipeline_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      104 2024-04-06 20:13:30.000000 rastervision_core-0.30.1/rastervision/core/rv_pipeline/semantic_segmentation.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5691 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/rv_pipeline/semantic_segmentation_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      798 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/rv_pipeline/utils.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.847123 rastervision_core-0.30.1/rastervision/core/utils/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      102 2023-08-24 18:41:21.000000 rastervision_core-0.30.1/rastervision/core/utils/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3261 2023-08-22 15:58:07.000000 rastervision_core-0.30.1/rastervision/core/utils/cog.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      981 2023-08-22 15:58:07.000000 rastervision_core-0.30.1/rastervision/core/utils/filter_geojson.py
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)       65 2023-09-26 14:00:58.000000 rastervision_core-0.30.1/rastervision/core/utils/misc.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6240 2024-04-07 00:38:15.000000 rastervision_core-0.30.1/rastervision/core/utils/stac.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-05-06 21:02:13.847123 rastervision_core-0.30.1/rastervision_core.egg-info/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      564 2024-05-06 21:02:13.000000 rastervision_core-0.30.1/rastervision_core.egg-info/PKG-INFO
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7852 2024-05-06 21:02:13.000000 rastervision_core-0.30.1/rastervision_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-05-06 21:02:13.000000 rastervision_core-0.30.1/rastervision_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-05-06 21:02:13.000000 rastervision_core-0.30.1/rastervision_core.egg-info/not-zip-safe
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      177 2024-05-06 21:02:13.000000 rastervision_core-0.30.1/rastervision_core.egg-info/requires.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       13 2024-05-06 21:02:13.000000 rastervision_core-0.30.1/rastervision_core.egg-info/top_level.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      327 2024-05-06 20:16:58.000000 rastervision_core-0.30.1/requirements.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-05-06 21:02:13.847123 rastervision_core-0.30.1/setup.cfg
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1731 2024-05-06 20:16:58.000000 rastervision_core-0.30.1/setup.py
```

### Comparing `rastervision_core-0.30.0/PKG-INFO` & `rastervision_core-0.30.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision_core
-Version: 0.30.0
+Version: 0.30.1
 Summary: A rastervision plugin that adds geospatial machine learning pipelines
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_core-0.30.0/rastervision/core/__init__.py` & `rastervision_core-0.30.1/rastervision/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/analyzer/analyzer_config.py` & `rastervision_core-0.30.1/rastervision/core/analyzer/analyzer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/analyzer/stats_analyzer.py` & `rastervision_core-0.30.1/rastervision/core/analyzer/stats_analyzer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/analyzer/stats_analyzer_config.py` & `rastervision_core-0.30.1/rastervision/core/analyzer/stats_analyzer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/backend/backend.py` & `rastervision_core-0.30.1/rastervision/core/backend/backend.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/backend/backend_config.py` & `rastervision_core-0.30.1/rastervision/core/backend/backend_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/box.py` & `rastervision_core-0.30.1/rastervision/core/box.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/cli.py` & `rastervision_core-0.30.1/rastervision/core/cli.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/__init__.py` & `rastervision_core-0.30.1/rastervision/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/class_config.py` & `rastervision_core-0.30.1/rastervision/core/data/class_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/crs_transformer/crs_transformer.py` & `rastervision_core-0.30.1/rastervision/core/data/crs_transformer/crs_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/crs_transformer/identity_crs_transformer.py` & `rastervision_core-0.30.1/rastervision/core/data/crs_transformer/identity_crs_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/crs_transformer/rasterio_crs_transformer.py` & `rastervision_core-0.30.1/rastervision/core/data/crs_transformer/rasterio_crs_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/dataset_config.py` & `rastervision_core-0.30.1/rastervision/core/data/dataset_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -86,7 +86,16 @@
                 split_ind] if split_ind < len(groups) else []
 
         return new_cfg
 
     @property
     def all_scenes(self) -> List[SceneConfig]:
         return self.train_scenes + self.validation_scenes + self.test_scenes
+
+    def __repr__(self):
+        num_train = len(self.train_scenes)
+        num_val = len(self.validation_scenes)
+        num_test = len(self.test_scenes)
+        out = (f'DatasetConfig(train_scenes=<{num_train} scenes>, '
+               f'validation_scenes=<{num_val} scenes>, '
+               f'test_scenes=<{num_test} scenes>)')
+        return out
```

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label/__init__.py` & `rastervision_core-0.30.1/rastervision/core/data/label/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label/chip_classification_labels.py` & `rastervision_core-0.30.1/rastervision/core/data/label/chip_classification_labels.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label/labels.py` & `rastervision_core-0.30.1/rastervision/core/data/label/labels.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label/object_detection_labels.py` & `rastervision_core-0.30.1/rastervision/core/data/label/object_detection_labels.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label/semantic_segmentation_labels.py` & `rastervision_core-0.30.1/rastervision/core/data/label/semantic_segmentation_labels.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label/tfod_utils/np_box_list.py` & `rastervision_core-0.30.1/rastervision/core/data/label/tfod_utils/np_box_list.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label/tfod_utils/np_box_list_ops.py` & `rastervision_core-0.30.1/rastervision/core/data/label/tfod_utils/np_box_list_ops.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label/tfod_utils/np_box_ops.py` & `rastervision_core-0.30.1/rastervision/core/data/label/tfod_utils/np_box_ops.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label/utils.py` & `rastervision_core-0.30.1/rastervision/core/data/label/utils.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_source/__init__.py` & `rastervision_core-0.30.1/rastervision/core/data/label_source/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_source/chip_classification_label_source.py` & `rastervision_core-0.30.1/rastervision/core/data/label_source/chip_classification_label_source.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_source/chip_classification_label_source_config.py` & `rastervision_core-0.30.1/rastervision/core/data/label_source/chip_classification_label_source_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_source/label_source.py` & `rastervision_core-0.30.1/rastervision/core/data/label_source/label_source.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_source/label_source_config.py` & `rastervision_core-0.30.1/rastervision/core/data/label_source/label_source_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_source/object_detection_label_source.py` & `rastervision_core-0.30.1/rastervision/core/data/label_source/object_detection_label_source.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_source/object_detection_label_source_config.py` & `rastervision_core-0.30.1/rastervision/core/data/label_source/object_detection_label_source_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_source/semantic_segmentation_label_source.py` & `rastervision_core-0.30.1/rastervision/core/data/label_source/semantic_segmentation_label_source.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_source/semantic_segmentation_label_source_config.py` & `rastervision_core-0.30.1/rastervision/core/data/label_source/semantic_segmentation_label_source_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_store/__init__.py` & `rastervision_core-0.30.1/rastervision/core/data/label_store/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_store/chip_classification_geojson_store.py` & `rastervision_core-0.30.1/rastervision/core/data/label_store/chip_classification_geojson_store.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_store/chip_classification_geojson_store_config.py` & `rastervision_core-0.30.1/rastervision/core/data/label_store/chip_classification_geojson_store_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_store/label_store.py` & `rastervision_core-0.30.1/rastervision/core/data/label_store/label_store.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_store/label_store_config.py` & `rastervision_core-0.30.1/rastervision/core/data/label_store/label_store_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_store/object_detection_geojson_store.py` & `rastervision_core-0.30.1/rastervision/core/data/label_store/object_detection_geojson_store.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_store/object_detection_geojson_store_config.py` & `rastervision_core-0.30.1/rastervision/core/data/label_store/object_detection_geojson_store_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_store/semantic_segmentation_label_store.py` & `rastervision_core-0.30.1/rastervision/core/data/label_store/semantic_segmentation_label_store.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_store/semantic_segmentation_label_store_config.py` & `rastervision_core-0.30.1/rastervision/core/data/label_store/semantic_segmentation_label_store_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/label_store/utils.py` & `rastervision_core-0.30.1/rastervision/core/data/label_store/utils.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_source/__init__.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_source/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_source/multi_raster_source.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_source/multi_raster_source.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_source/multi_raster_source_config.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_source/multi_raster_source_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_source/raster_source.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_source/raster_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,32 +143,28 @@
         chip = chip[..., self.channel_order]
 
         for transformer in self.raster_transformers:
             chip = transformer.transform(chip, self.channel_order)
 
         return chip
 
-    def get_chip_by_map_window(
-            self,
-            window_map_coords: 'Box',
-            out_shape: Optional[Tuple[int, int]] = None) -> 'np.ndarray':
-        """Same as get_chip(), but input is a window in map coords. """
+    def get_chip_by_map_window(self, window_map_coords: 'Box', *args,
+                               **kwargs) -> 'np.ndarray':
+        """Same as get_chip(), but input is a window in map coords."""
         window_pixel_coords = self.crs_transformer.map_to_pixel(
             window_map_coords, bbox=self.bbox).normalize()
-        chip = self.get_chip(window_pixel_coords, out_shape=out_shape)
+        chip = self.get_chip(window_pixel_coords, *args, **kwargs)
         return chip
 
-    def _get_chip_by_map_window(
-            self,
-            window_map_coords: 'Box',
-            out_shape: Optional[Tuple[int, int]] = None) -> 'np.ndarray':
-        """Same as _get_chip(), but input is a window in map coords. """
+    def _get_chip_by_map_window(self, window_map_coords: 'Box', *args,
+                                **kwargs) -> 'np.ndarray':
+        """Same as _get_chip(), but input is a window in map coords."""
         window_pixel_coords = self.crs_transformer.map_to_pixel(
             window_map_coords, bbox=self.bbox)
-        chip = self._get_chip(window_pixel_coords, out_shape=out_shape)
+        chip = self._get_chip(window_pixel_coords, *args, **kwargs)
         return chip
 
     def get_raw_chip(self,
                      window: 'Box',
                      out_shape: Optional[Tuple[int, int]] = None
                      ) -> 'np.ndarray':
         """Return raw chip without applying channel_order or transforms.
```

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_source/raster_source_config.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_source/raster_source_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_source/rasterio_source.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_source/rasterio_source.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_source/rasterio_source_config.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_source/rasterio_source_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_source/rasterized_source.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_source/rasterized_source.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_source/rasterized_source_config.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_source/rasterized_source_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_source/stac_config.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_source/stac_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_source/temporal_multi_raster_source.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_source/temporal_multi_raster_source.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_source/xarray_source.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_source/xarray_source.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_source/xarray_source_config.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_source/xarray_source_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/__init__.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/cast_transformer.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_transformer/cast_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/cast_transformer_config.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_transformer/cast_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/min_max_transformer.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_transformer/min_max_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/nan_transformer.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_transformer/nan_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/nan_transformer_config.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_transformer/nan_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/raster_transformer.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_transformer/raster_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/raster_transformer_config.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_transformer/raster_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/reclass_transformer.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_transformer/reclass_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/reclass_transformer_config.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_transformer/reclass_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/rgb_class_transformer.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_transformer/rgb_class_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/rgb_class_transformer_config.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_transformer/rgb_class_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/stats_transformer.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_transformer/stats_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/stats_transformer_config.py` & `rastervision_core-0.30.1/rastervision/core/data/raster_transformer/stats_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/scene.py` & `rastervision_core-0.30.1/rastervision/core/data/scene.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/scene_config.py` & `rastervision_core-0.30.1/rastervision/core/data/scene_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/utils/aoi_sampler.py` & `rastervision_core-0.30.1/rastervision/core/data/utils/aoi_sampler.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/utils/factory.py` & `rastervision_core-0.30.1/rastervision/core/data/utils/factory.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/utils/geojson.py` & `rastervision_core-0.30.1/rastervision/core/data/utils/geojson.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/utils/misc.py` & `rastervision_core-0.30.1/rastervision/core/data/utils/misc.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/utils/raster.py` & `rastervision_core-0.30.1/rastervision/core/data/utils/raster.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/utils/rasterio.py` & `rastervision_core-0.30.1/rastervision/core/data/utils/rasterio.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/utils/vectorization.py` & `rastervision_core-0.30.1/rastervision/core/data/utils/vectorization.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/vector_source/geojson_vector_source.py` & `rastervision_core-0.30.1/rastervision/core/data/vector_source/geojson_vector_source.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/vector_source/geojson_vector_source_config.py` & `rastervision_core-0.30.1/rastervision/core/data/vector_source/geojson_vector_source_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/vector_source/vector_source.py` & `rastervision_core-0.30.1/rastervision/core/data/vector_source/vector_source.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/vector_source/vector_source_config.py` & `rastervision_core-0.30.1/rastervision/core/data/vector_source/vector_source_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/__init__.py` & `rastervision_core-0.30.1/rastervision/core/data/vector_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/buffer_transformer.py` & `rastervision_core-0.30.1/rastervision/core/data/vector_transformer/buffer_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/buffer_transformer_config.py` & `rastervision_core-0.30.1/rastervision/core/data/vector_transformer/buffer_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/class_inference_transformer.py` & `rastervision_core-0.30.1/rastervision/core/data/vector_transformer/class_inference_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/class_inference_transformer_config.py` & `rastervision_core-0.30.1/rastervision/core/data/vector_transformer/class_inference_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/label_maker/filter.py` & `rastervision_core-0.30.1/rastervision/core/data/vector_transformer/label_maker/filter.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/shift_transformer.py` & `rastervision_core-0.30.1/rastervision/core/data/vector_transformer/shift_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/shift_transformer_config.py` & `rastervision_core-0.30.1/rastervision/core/data/vector_transformer/shift_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/vector_transformer.py` & `rastervision_core-0.30.1/rastervision/core/data/vector_transformer/vector_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/vector_transformer_config.py` & `rastervision_core-0.30.1/rastervision/core/data/vector_transformer/vector_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/evaluation/__init__.py` & `rastervision_core-0.30.1/rastervision/core/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/evaluation/chip_classification_evaluation.py` & `rastervision_core-0.30.1/rastervision/core/evaluation/chip_classification_evaluation.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/evaluation/chip_classification_evaluator_config.py` & `rastervision_core-0.30.1/rastervision/core/evaluation/chip_classification_evaluator_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/evaluation/class_evaluation_item.py` & `rastervision_core-0.30.1/rastervision/core/evaluation/class_evaluation_item.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/evaluation/classification_evaluation.py` & `rastervision_core-0.30.1/rastervision/core/evaluation/classification_evaluation.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/evaluation/classification_evaluator.py` & `rastervision_core-0.30.1/rastervision/core/evaluation/classification_evaluator.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/evaluation/evaluator.py` & `rastervision_core-0.30.1/rastervision/core/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/evaluation/evaluator_config.py` & `rastervision_core-0.30.1/rastervision/core/evaluation/evaluator_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/evaluation/object_detection_evaluation.py` & `rastervision_core-0.30.1/rastervision/core/evaluation/object_detection_evaluation.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/evaluation/object_detection_evaluator_config.py` & `rastervision_core-0.30.1/rastervision/core/evaluation/object_detection_evaluator_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/evaluation/semantic_segmentation_evaluation.py` & `rastervision_core-0.30.1/rastervision/core/evaluation/semantic_segmentation_evaluation.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/evaluation/semantic_segmentation_evaluator.py` & `rastervision_core-0.30.1/rastervision/core/evaluation/semantic_segmentation_evaluator.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/evaluation/semantic_segmentation_evaluator_config.py` & `rastervision_core-0.30.1/rastervision/core/evaluation/semantic_segmentation_evaluator_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/predictor.py` & `rastervision_core-0.30.1/rastervision/core/predictor.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/raster_stats.py` & `rastervision_core-0.30.1/rastervision/core/raster_stats.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/rv_pipeline/__init__.py` & `rastervision_core-0.30.1/rastervision/core/rv_pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/rv_pipeline/chip_classification_config.py` & `rastervision_core-0.30.1/rastervision/core/rv_pipeline/chip_classification_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/rv_pipeline/chip_options.py` & `rastervision_core-0.30.1/rastervision/core/rv_pipeline/chip_options.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/rv_pipeline/object_detection_config.py` & `rastervision_core-0.30.1/rastervision/core/rv_pipeline/object_detection_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/rv_pipeline/rv_pipeline.py` & `rastervision_core-0.30.1/rastervision/core/rv_pipeline/rv_pipeline.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/rv_pipeline/rv_pipeline_config.py` & `rastervision_core-0.30.1/rastervision/core/rv_pipeline/rv_pipeline_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/rv_pipeline/semantic_segmentation_config.py` & `rastervision_core-0.30.1/rastervision/core/rv_pipeline/semantic_segmentation_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/rv_pipeline/utils.py` & `rastervision_core-0.30.1/rastervision/core/rv_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/utils/cog.py` & `rastervision_core-0.30.1/rastervision/core/utils/cog.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/utils/filter_geojson.py` & `rastervision_core-0.30.1/rastervision/core/utils/filter_geojson.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision/core/utils/stac.py` & `rastervision_core-0.30.1/rastervision/core/utils/stac.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/rastervision_core.egg-info/PKG-INFO` & `rastervision_core-0.30.1/rastervision_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision-core
-Version: 0.30.0
+Version: 0.30.1
 Summary: A rastervision plugin that adds geospatial machine learning pipelines
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_core-0.30.0/rastervision_core.egg-info/SOURCES.txt` & `rastervision_core-0.30.1/rastervision_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.30.0/setup.py` & `rastervision_core-0.30.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 from os.path import abspath, dirname, join
 from setuptools import setup, find_namespace_packages
 import re
 
 name = 'rastervision_core'
-version = '0.30.0'
+version = '0.30.1'
 description = 'A rastervision plugin that adds geospatial machine learning pipelines'
 requirement_constraints = {}
 
 here = abspath(dirname(__file__))
 
 
 def parse_requirements(requirements_path: str) -> list[str]:
```

