# Comparing `tmp/nixtla-0.5.0.tar.gz` & `tmp/nixtla-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nixtla-0.5.0.tar", last modified: Wed May  1 19:51:14 2024, max compression
+gzip compressed data, was "nixtla-0.5.1.tar", last modified: Mon May  6 19:07:57 2024, max compression
```

## Comparing `nixtla-0.5.0.tar` & `nixtla-0.5.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:14.927730 nixtla-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11414 2024-05-01 19:51:09.000000 nixtla-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-01 19:51:14.927730 nixtla-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-01 19:51:09.000000 nixtla-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:14.915730 nixtla-0.5.0/nixtla/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20657 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)   304758 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:14.919730 nixtla-0.5.0/nixtla/core/
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/api_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/client_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/jsonable_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/pydantic_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/remove_none_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/core/request_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/date_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:14.919730 nixtla-0.5.0/nixtla/distributed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/distributed/nixtla_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:14.919730 nixtla-0.5.0/nixtla/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/errors/unprocessable_entity_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    65345 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/nixtla_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:14.923730 nixtla-0.5.0/nixtla/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_anomaly.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_cross_validation_fewshot_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_cross_validation_finetune_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_forecast_fewshot_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_forecast_finetune_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/multi_series_insample_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/single_series_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/single_series_forecast_fewshot_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/single_series_forecast_finetune_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/single_series_insample_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/types/validation_error_loc_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-01 19:51:09.000000 nixtla-0.5.0/nixtla/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:51:14.923730 nixtla-0.5.0/nixtla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-01 19:51:14.000000 nixtla-0.5.0/nixtla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-01 19:51:14.000000 nixtla-0.5.0/nixtla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:51:14.000000 nixtla-0.5.0/nixtla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-01 19:51:14.000000 nixtla-0.5.0/nixtla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 19:51:14.000000 nixtla-0.5.0/nixtla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:51:14.927730 nixtla-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-01 19:51:09.000000 nixtla-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:07:57.787212 nixtla-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11414 2024-05-06 19:07:52.000000 nixtla-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-06 19:07:57.787212 nixtla-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-06 19:07:52.000000 nixtla-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:07:57.779212 nixtla-0.5.1/nixtla/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20657 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)   304758 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:07:57.783212 nixtla-0.5.1/nixtla/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/core/api_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/core/client_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/core/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/core/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/core/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/core/jsonable_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/core/pydantic_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/core/remove_none_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/core/request_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/date_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:07:57.783212 nixtla-0.5.1/nixtla/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/distributed/nixtla_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:07:57.783212 nixtla-0.5.1/nixtla/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/errors/unprocessable_entity_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65375 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/nixtla_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:07:57.787212 nixtla-0.5.1/nixtla/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/multi_series_anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/multi_series_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/multi_series_cross_validation_fewshot_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/multi_series_cross_validation_finetune_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/multi_series_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/multi_series_forecast_fewshot_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/multi_series_forecast_finetune_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/multi_series_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/multi_series_insample_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/single_series_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/single_series_forecast_fewshot_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/single_series_forecast_finetune_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/single_series_insample_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/types/validation_error_loc_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-06 19:07:52.000000 nixtla-0.5.1/nixtla/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:07:57.787212 nixtla-0.5.1/nixtla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-06 19:07:57.000000 nixtla-0.5.1/nixtla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-06 19:07:57.000000 nixtla-0.5.1/nixtla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:07:57.000000 nixtla-0.5.1/nixtla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-06 19:07:57.000000 nixtla-0.5.1/nixtla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 19:07:57.000000 nixtla-0.5.1/nixtla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:07:57.787212 nixtla-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-06 19:07:52.000000 nixtla-0.5.1/setup.py
```

### Comparing `nixtla-0.5.0/LICENSE` & `nixtla-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/PKG-INFO` & `nixtla-0.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nixtla
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python SDK for Nixtla API (TimeGPT)
 Home-page: https://github.com/Nixtla/nixtla
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -18,15 +18,17 @@
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: datasetsforecast; extra == "dev"
 Requires-Dist: nbdev; extra == "dev"
 Requires-Dist: plotly; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: python-dotenv; extra == "dev"
+Requires-Dist: pyreadr; extra == "dev"
 Requires-Dist: statsforecast; extra == "dev"
+Requires-Dist: neuralforecast; extra == "dev"
 Requires-Dist: hierarchicalforecast; extra == "dev"
 Requires-Dist: dask[dataframe]; extra == "dev"
 Requires-Dist: fugue[ray]>=0.8.7; extra == "dev"
 Requires-Dist: pyspark; extra == "dev"
 Requires-Dist: ray[serve-grpc]; extra == "dev"
 Requires-Dist: utilsforecast[plotting]>=0.1.7; extra == "dev"
 Requires-Dist: holidays; extra == "dev"
@@ -72,15 +74,15 @@
 With `Nixtla`, you can easily interact with TimeGPT through simple API calls, making the power of TimeGPT readily accessible in your projects.
 
 ## 💻 Installation
 
 Get `Nixtla` up and running with a simple pip command:
 
 ```python
-pip install nixtla>=0.4.0
+pip install nixtla>=0.5.1
 ```
 
 ## 🎈 Quick Start
 
 Get started with TimeGPT now:
 
 ```python
```

### Comparing `nixtla-0.5.0/README.md` & `nixtla-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 With `Nixtla`, you can easily interact with TimeGPT through simple API calls, making the power of TimeGPT readily accessible in your projects.
 
 ## 💻 Installation
 
 Get `Nixtla` up and running with a simple pip command:
 
 ```python
-pip install nixtla>=0.4.0
+pip install nixtla>=0.5.1
 ```
 
 ## 🎈 Quick Start
 
 Get started with TimeGPT now:
 
 ```python
```

### Comparing `nixtla-0.5.0/nixtla/_modidx.py` & `nixtla-0.5.1/nixtla/_modidx.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/client.py` & `nixtla-0.5.1/nixtla/client.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/core/__init__.py` & `nixtla-0.5.1/nixtla/core/__init__.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/core/client_wrapper.py` & `nixtla-0.5.1/nixtla/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/core/datetime_utils.py` & `nixtla-0.5.1/nixtla/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/core/file.py` & `nixtla-0.5.1/nixtla/core/file.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/core/http_client.py` & `nixtla-0.5.1/nixtla/core/http_client.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/core/jsonable_encoder.py` & `nixtla-0.5.1/nixtla/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/core/request_options.py` & `nixtla-0.5.1/nixtla/core/request_options.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/date_features.py` & `nixtla-0.5.1/nixtla/date_features.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/distributed/nixtla_client.py` & `nixtla-0.5.1/nixtla/distributed/nixtla_client.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/nixtla_client.py` & `nixtla-0.5.1/nixtla/nixtla_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -694,14 +694,15 @@
             level=self.level,
             fh=self.h,
             y=y,
             x=x,
             n_windows=n_windows,
             step_size=step_size,
             clean_ex_first=self.clean_ex_first,
+            model=self.model,
         )
         response = self._call_api(self.client.cross_validation_multi_series, payload)
         cv_df = pd.DataFrame(**response["forecast"])
         cv_df["cutoff"] = pd.to_datetime(cv_df["cutoff"])
         cv_df = self.transform_outputs(cv_df, level_to_quantiles=True)
         return cv_df
```

### Comparing `nixtla-0.5.0/nixtla/types/__init__.py` & `nixtla-0.5.1/nixtla/types/__init__.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/types/http_validation_error.py` & `nixtla-0.5.1/nixtla/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/types/multi_series_anomaly.py` & `nixtla-0.5.1/nixtla/types/multi_series_anomaly.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/types/multi_series_cross_validation.py` & `nixtla-0.5.1/nixtla/types/multi_series_cross_validation.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/types/multi_series_forecast.py` & `nixtla-0.5.1/nixtla/types/multi_series_forecast.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/types/multi_series_input.py` & `nixtla-0.5.1/nixtla/types/multi_series_input.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/types/multi_series_insample_forecast.py` & `nixtla-0.5.1/nixtla/types/multi_series_insample_forecast.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/types/single_series_forecast.py` & `nixtla-0.5.1/nixtla/types/single_series_forecast.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/types/single_series_insample_forecast.py` & `nixtla-0.5.1/nixtla/types/single_series_insample_forecast.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla/types/validation_error.py` & `nixtla-0.5.1/nixtla/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/nixtla.egg-info/PKG-INFO` & `nixtla-0.5.1/nixtla.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nixtla
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python SDK for Nixtla API (TimeGPT)
 Home-page: https://github.com/Nixtla/nixtla
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -18,15 +18,17 @@
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: datasetsforecast; extra == "dev"
 Requires-Dist: nbdev; extra == "dev"
 Requires-Dist: plotly; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: python-dotenv; extra == "dev"
+Requires-Dist: pyreadr; extra == "dev"
 Requires-Dist: statsforecast; extra == "dev"
+Requires-Dist: neuralforecast; extra == "dev"
 Requires-Dist: hierarchicalforecast; extra == "dev"
 Requires-Dist: dask[dataframe]; extra == "dev"
 Requires-Dist: fugue[ray]>=0.8.7; extra == "dev"
 Requires-Dist: pyspark; extra == "dev"
 Requires-Dist: ray[serve-grpc]; extra == "dev"
 Requires-Dist: utilsforecast[plotting]>=0.1.7; extra == "dev"
 Requires-Dist: holidays; extra == "dev"
@@ -72,15 +74,15 @@
 With `Nixtla`, you can easily interact with TimeGPT through simple API calls, making the power of TimeGPT readily accessible in your projects.
 
 ## 💻 Installation
 
 Get `Nixtla` up and running with a simple pip command:
 
 ```python
-pip install nixtla>=0.4.0
+pip install nixtla>=0.5.1
 ```
 
 ## 🎈 Quick Start
 
 Get started with TimeGPT now:
 
 ```python
```

### Comparing `nixtla-0.5.0/nixtla.egg-info/SOURCES.txt` & `nixtla-0.5.1/nixtla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nixtla-0.5.0/setup.py` & `nixtla-0.5.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 dev = [
     "black",
     "datasetsforecast",
     "nbdev",
     "plotly",
     "pre-commit",
     "python-dotenv",
+    "pyreadr",
     "statsforecast",
+    "neuralforecast",
     "hierarchicalforecast",
 ]
 distributed = ["dask[dataframe]", "fugue[ray]>=0.8.7", "pyspark", "ray[serve-grpc]"]
 plotting = ["utilsforecast[plotting]>=0.1.7"]
 date_extras = ["holidays"]
 
 setuptools.setup(
     name="nixtla",
-    version="0.5.0",
+    version="0.5.1",
     description="Python SDK for Nixtla API (TimeGPT)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nixtla/nixtla",
     packages=setuptools.find_packages(exclude=["action_files"]),
     classifiers=[
         "Programming Language :: Python :: 3",
```

