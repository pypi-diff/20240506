# Comparing `tmp/giza_datasets-0.2.1.tar.gz` & `tmp/giza_datasets-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giza_datasets-0.2.1.tar", max compression
+gzip compressed data, was "giza_datasets-0.2.2.tar", max compression
```

## Comparing `giza_datasets-0.2.1.tar` & `giza_datasets-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2024-04-17 13:07:02.194124 giza_datasets-0.2.1/LICENSE
--rw-r--r--   0        0        0     3951 2024-04-17 13:07:02.194124 giza_datasets-0.2.1/README.md
--rw-r--r--   0        0        0      136 2024-04-17 13:07:02.194124 giza_datasets-0.2.1/giza_datasets/__init__.py
--rw-r--r--   0        0        0     2853 2024-04-17 13:07:02.194124 giza_datasets-0.2.1/giza_datasets/cache_manager.py
--rw-r--r--   0        0        0   150859 2024-04-17 13:07:02.198124 giza_datasets-0.2.1/giza_datasets/constants.py
--rw-r--r--   0        0        0      635 2024-04-17 13:07:02.198124 giza_datasets-0.2.1/giza_datasets/defillama_constants.py
--rw-r--r--   0        0        0     3240 2024-04-17 13:07:02.198124 giza_datasets-0.2.1/giza_datasets/hub.py
--rw-r--r--   0        0        0     5982 2024-04-17 13:07:02.198124 giza_datasets-0.2.1/giza_datasets/loaders.py
--rw-r--r--   0        0        0     1441 2024-04-17 13:07:02.198124 giza_datasets-0.2.1/giza_datasets/models.py
--rw-r--r--   0        0        0      554 2024-04-17 13:07:02.198124 giza_datasets-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4537 1970-01-01 00:00:00.000000 giza_datasets-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-06 11:49:43.531264 giza_datasets-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3951 2024-05-06 11:49:43.531264 giza_datasets-0.2.2/README.md
+-rw-r--r--   0        0        0      136 2024-05-06 11:49:43.531264 giza_datasets-0.2.2/giza_datasets/__init__.py
+-rw-r--r--   0        0        0     2853 2024-05-06 11:49:43.531264 giza_datasets-0.2.2/giza_datasets/cache_manager.py
+-rw-r--r--   0        0        0   151116 2024-05-06 11:49:43.535264 giza_datasets-0.2.2/giza_datasets/constants.py
+-rw-r--r--   0        0        0      635 2024-05-06 11:49:43.535264 giza_datasets-0.2.2/giza_datasets/defillama_constants.py
+-rw-r--r--   0        0        0     3240 2024-05-06 11:49:43.535264 giza_datasets-0.2.2/giza_datasets/hub.py
+-rw-r--r--   0        0        0     5982 2024-05-06 11:49:43.535264 giza_datasets-0.2.2/giza_datasets/loaders.py
+-rw-r--r--   0        0        0     1441 2024-05-06 11:49:43.535264 giza_datasets-0.2.2/giza_datasets/models.py
+-rw-r--r--   0        0        0      554 2024-05-06 11:49:43.535264 giza_datasets-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4537 1970-01-01 00:00:00.000000 giza_datasets-0.2.2/PKG-INFO
```

### Comparing `giza_datasets-0.2.1/LICENSE` & `giza_datasets-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.2.1/README.md` & `giza_datasets-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.2.1/giza_datasets/cache_manager.py` & `giza_datasets-0.2.2/giza_datasets/cache_manager.py`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.2.1/giza_datasets/constants.py` & `giza_datasets-0.2.2/giza_datasets/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -2283,8 +2283,16 @@
     Dataset(
         name="curve-daily-volume-fees",
         path="gs://datasets-giza/Curve/curve_daily_volume_fees.parquet",
         description="Daily Curve trade volume and fees generated in USD, per pool",
         tags=["Curve","Trade Volume","Fees" ,"daily", "DeFi", "DEX"],
         documentation="https://datasets.gizatech.xyz/hub/curve/daily-trade-volume-and-fees",
     ),
+        Dataset(
+        name="gora-competition-training",
+        path="gs://datasets-giza/Rocifi/gora_competition_training.parquet",
+        description="Training data for the Gora competition",
+        tags=["Lending"],
+        documentation="",
+    ),
 ]
+
```

### Comparing `giza_datasets-0.2.1/giza_datasets/defillama_constants.py` & `giza_datasets-0.2.2/giza_datasets/defillama_constants.py`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.2.1/giza_datasets/hub.py` & `giza_datasets-0.2.2/giza_datasets/hub.py`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.2.1/giza_datasets/loaders.py` & `giza_datasets-0.2.2/giza_datasets/loaders.py`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.2.1/giza_datasets/models.py` & `giza_datasets-0.2.2/giza_datasets/models.py`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.2.1/pyproject.toml` & `giza_datasets-0.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giza-datasets"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Fran Algaba <f.algaba@outlook.es>"]
 readme = "README.md"
 license = "MIT"
 include = ["datasets/*"]
```

### Comparing `giza_datasets-0.2.1/PKG-INFO` & `giza_datasets-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giza-datasets
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 License: MIT
 Author: Fran Algaba
 Author-email: f.algaba@outlook.es
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```
