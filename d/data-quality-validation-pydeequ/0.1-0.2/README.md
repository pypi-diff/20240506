# Comparing `tmp/data-quality-validation-pydeequ-0.1.tar.gz` & `tmp/data-quality-validation-pydeequ-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-quality-validation-pydeequ-0.1.tar", last modified: Mon May  6 06:21:29 2024, max compression
+gzip compressed data, was "data-quality-validation-pydeequ-0.2.tar", last modified: Mon May  6 09:55:28 2024, max compression
```

## Comparing `data-quality-validation-pydeequ-0.1.tar` & `data-quality-validation-pydeequ-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:21:29.954075 data-quality-validation-pydeequ-0.1/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      223 2024-05-06 06:21:29.953268 data-quality-validation-pydeequ-0.1/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     3218 2024-05-06 06:17:24.000000 data-quality-validation-pydeequ-0.1/README.md
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:21:29.952732 data-quality-validation-pydeequ-0.1/data_quality_validation_pydeequ.egg-info/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      223 2024-05-06 06:21:29.000000 data-quality-validation-pydeequ-0.1/data_quality_validation_pydeequ.egg-info/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-06 06:21:29.000000 data-quality-validation-pydeequ-0.1/data_quality_validation_pydeequ.egg-info/SOURCES.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-06 06:21:29.000000 data-quality-validation-pydeequ-0.1/data_quality_validation_pydeequ.egg-info/dependency_links.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       21 2024-05-06 06:21:29.000000 data-quality-validation-pydeequ-0.1/data_quality_validation_pydeequ.egg-info/requires.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-06 06:21:29.000000 data-quality-validation-pydeequ-0.1/data_quality_validation_pydeequ.egg-info/top_level.txt
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:21:29.951857 data-quality-validation-pydeequ-0.1/dqv/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-0.1/dqv/__init__.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 06:15:36.000000 data-quality-validation-pydeequ-0.1/dqv/data_quality_validation_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     1800 2024-05-06 06:15:30.000000 data-quality-validation-pydeequ-0.1/dqv/dqv_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-06 06:21:29.954180 data-quality-validation-pydeequ-0.1/setup.cfg
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      368 2024-05-06 06:20:23.000000 data-quality-validation-pydeequ-0.1/setup.py
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 09:55:28.847597 data-quality-validation-pydeequ-0.2/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      439 2024-05-06 09:55:28.847151 data-quality-validation-pydeequ-0.2/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     3218 2024-05-06 06:17:24.000000 data-quality-validation-pydeequ-0.2/README.md
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 09:55:28.846562 data-quality-validation-pydeequ-0.2/data_quality_validation_pydeequ.egg-info/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      439 2024-05-06 09:55:28.000000 data-quality-validation-pydeequ-0.2/data_quality_validation_pydeequ.egg-info/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-06 09:55:28.000000 data-quality-validation-pydeequ-0.2/data_quality_validation_pydeequ.egg-info/SOURCES.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-06 09:55:28.000000 data-quality-validation-pydeequ-0.2/data_quality_validation_pydeequ.egg-info/dependency_links.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-06 09:55:28.000000 data-quality-validation-pydeequ-0.2/data_quality_validation_pydeequ.egg-info/requires.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-06 09:55:28.000000 data-quality-validation-pydeequ-0.2/data_quality_validation_pydeequ.egg-info/top_level.txt
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 09:55:28.844797 data-quality-validation-pydeequ-0.2/dqv/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-0.2/dqv/__init__.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 data-quality-validation-pydeequ-0.2/dqv/data_quality_validation_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     1650 2024-05-06 09:01:46.000000 data-quality-validation-pydeequ-0.2/dqv/dqv_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-06 09:55:28.847667 data-quality-validation-pydeequ-0.2/setup.cfg
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      586 2024-05-06 09:24:21.000000 data-quality-validation-pydeequ-0.2/setup.py
```

### Comparing `data-quality-validation-pydeequ-0.1/README.md` & `data-quality-validation-pydeequ-0.2/README.md`

 * *Files identical despite different names*

### Comparing `data-quality-validation-pydeequ-0.1/dqv/data_quality_validation_pydeequ.py` & `data-quality-validation-pydeequ-0.2/dqv/data_quality_validation_pydeequ.py`

 * *Files identical despite different names*

### Comparing `data-quality-validation-pydeequ-0.1/dqv/dqv_pydeequ.py` & `data-quality-validation-pydeequ-0.2/dqv/dqv_pydeequ.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,51 @@
-import yaml
-import os
 from data_quality_validation_pydeequ import DataQualityValidation
-from pyspark.sql import SparkSession
 from pathlib import Path
+from pyspark.sql import SparkSession
 import pydeequ
+import yaml
 
 
 class DqvPydeequ:
-    """Class for performing data quality validation using PyDeequ and sending email notifications."""
+    """Class for performing data quality validation using PyDeequ"""
 
     def __init__(
-        self, 
-        config_path: str, 
-        source_path: str, 
-        target_path: str, 
-        **kwargs) -> None:
+        self,
+        config_path: str,
+        source_path: str,
+        target_path: str,
+        **kwargs
+    ) -> None:
         """Initialize the DqvPydeequ class.
 
         Args:
             config_path (str): Path to configuration file.
             source_path (str): Path to source data.
             target_path (str): Path to target data.
-            email_config (dict): Email configuration settings.
         """
         spark = (
             SparkSession.builder.appName("data_quality_validation_pydeequ")
-                .enableHiveSupport()
-                .config("spark.dynamicAllocation.enabled", "true")
-                .config("spark.jars.packages", pydeequ.deequ_maven_coord)
-                .config("spark.jars.excludes", pydeequ.f2j_maven_coord)
-                .config("spark.default.parallelism", "10")
-                .config("spark.sql.shuffle.partitions", "10")
-                .config("spark.sql.files.ignoreCorruptFiles", "true")
-                .getOrCreate()
+            .enableHiveSupport()
+            .config("spark.dynamicAllocation.enabled", "true")
+            .config("spark.jars.packages", pydeequ.deequ_maven_coord)
+            .config("spark.jars.excludes", pydeequ.f2j_maven_coord)
+            .config("spark.default.parallelism", "10")
+            .config("spark.sql.shuffle.partitions", "10")
+            .config("spark.sql.files.ignoreCorruptFiles", "true")
+            .getOrCreate()
         )
         with open(config_path, "r") as stream:
             data = yaml.safe_load(stream)
         config = data["DQ_ASSERTIONS"]["DIR1"]["PRODUCT_FILE"]
         print(config)
-        try :
+        try:
             bolosse = DataQualityValidation(
                 spark,
                 source_path,
                 target_path,
                 config,
             )
             bolosse.execute()
             spark.stop()
         except Exception as ex:
             print(ex)
             spark.stop()
-
```

