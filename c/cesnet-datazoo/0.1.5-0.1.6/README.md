# Comparing `tmp/cesnet_datazoo-0.1.5.tar.gz` & `tmp/cesnet_datazoo-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cesnet_datazoo-0.1.5.tar", last modified: Tue Apr 30 12:14:13 2024, max compression
+gzip compressed data, was "cesnet_datazoo-0.1.6.tar", last modified: Mon May  6 11:38:42 2024, max compression
```

## Comparing `cesnet_datazoo-0.1.5.tar` & `cesnet_datazoo-0.1.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 12:14:13.154084 cesnet_datazoo-0.1.5/
--rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet_datazoo-0.1.5/LICENCE
--rw-rw-rw-   0        0        0    12953 2024-04-30 12:14:13.153578 cesnet_datazoo-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    11374 2024-04-09 14:38:48.000000 cesnet_datazoo-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 12:14:13.110340 cesnet_datazoo-0.1.5/cesnet_datazoo/
--rw-rw-rw-   0        0        0        0 2023-09-04 15:14:00.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/__init__.py
--rw-rw-rw-   0        0        0    38406 2024-04-26 10:09:35.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/config.py
--rw-rw-rw-   0        0        0     1481 2024-04-26 10:10:11.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-30 12:14:13.136146 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/
--rw-rw-rw-   0        0        0      443 2023-10-09 14:50:14.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/__init__.py
--rw-rw-rw-   0        0        0    46988 2024-04-30 11:22:06.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/cesnet_dataset.py
--rw-rw-rw-   0        0        0     3617 2024-03-13 15:20:57.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/datasets.py
--rw-rw-rw-   0        0        0    29154 2024-03-13 15:20:40.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/datasets_constants.py
--rw-rw-rw-   0        0        0     1854 2024-03-14 10:53:21.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/loaders.py
-drwxrwxrwx   0        0        0        0 2024-04-30 12:14:13.139212 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/metadata/
--rw-rw-rw-   0        0        0        0 2023-08-21 14:08:44.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/metadata/__init__.py
--rw-rw-rw-   0        0        0     1623 2024-04-26 12:35:59.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/metadata/dataset_metadata.py
--rw-rw-rw-   0        0        0     2175 2024-03-19 11:54:21.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/metadata/metadata.csv
--rw-rw-rw-   0        0        0    15137 2024-04-26 12:36:13.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/statistics.py
-drwxrwxrwx   0        0        0        0 2024-04-30 12:14:13.141105 cesnet_datazoo-0.1.5/cesnet_datazoo/metrics/
--rw-rw-rw-   0        0        0        0 2023-08-17 21:32:34.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/metrics/__init__.py
--rw-rw-rw-   0        0        0     3981 2024-04-26 10:13:11.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/metrics/classification_report.py
--rw-rw-rw-   0        0        0     1374 2024-04-17 16:35:50.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/metrics/provider_metrics.py
-drwxrwxrwx   0        0        0        0 2024-04-30 12:14:13.145674 cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:24:29.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/__init__.py
--rw-rw-rw-   0        0        0     1411 2023-10-30 20:40:56.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/apps_split.py
--rw-rw-rw-   0        0        0     5236 2024-04-30 11:25:34.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/data_scalers.py
--rw-rw-rw-   0        0        0    13717 2024-04-26 12:13:42.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/indices_setup.py
--rw-rw-rw-   0        0        0    19431 2024-04-30 11:22:10.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/pytables_dataset.py
-drwxrwxrwx   0        0        0        0 2024-04-30 12:14:13.150684 cesnet_datazoo-0.1.5/cesnet_datazoo/utils/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:35:45.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/utils/__init__.py
--rw-rw-rw-   0        0        0     2462 2024-04-04 20:29:42.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/utils/class_info.py
--rw-rw-rw-   0        0        0     1441 2024-02-20 11:51:54.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/utils/download.py
--rw-rw-rw-   0        0        0      642 2023-09-01 13:43:06.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/utils/fileutils.py
--rw-rw-rw-   0        0        0      575 2023-09-26 08:58:11.000000 cesnet_datazoo-0.1.5/cesnet_datazoo/utils/random.py
-drwxrwxrwx   0        0        0        0 2024-04-30 12:14:13.150684 cesnet_datazoo-0.1.5/cesnet_datazoo.egg-info/
--rw-rw-rw-   0        0        0    12953 2024-04-30 12:14:13.000000 cesnet_datazoo-0.1.5/cesnet_datazoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2024-04-30 12:14:13.000000 cesnet_datazoo-0.1.5/cesnet_datazoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 12:14:13.000000 cesnet_datazoo-0.1.5/cesnet_datazoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      238 2024-04-30 12:14:13.000000 cesnet_datazoo-0.1.5/cesnet_datazoo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-30 12:14:13.000000 cesnet_datazoo-0.1.5/cesnet_datazoo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1792 2024-04-30 12:13:18.000000 cesnet_datazoo-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 12:14:13.154084 cesnet_datazoo-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 11:38:42.990233 cesnet_datazoo-0.1.6/
+-rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet_datazoo-0.1.6/LICENCE
+-rw-rw-rw-   0        0        0    12953 2024-05-06 11:38:42.989231 cesnet_datazoo-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11374 2024-04-09 14:38:48.000000 cesnet_datazoo-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 11:38:42.936158 cesnet_datazoo-0.1.6/cesnet_datazoo/
+-rw-rw-rw-   0        0        0        0 2023-09-04 15:14:00.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/__init__.py
+-rw-rw-rw-   0        0        0    38536 2024-05-06 10:36:48.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/config.py
+-rw-rw-rw-   0        0        0     1481 2024-04-26 10:10:11.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:38:42.967043 cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/
+-rw-rw-rw-   0        0        0      443 2023-10-09 14:50:14.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/__init__.py
+-rw-rw-rw-   0        0        0    46988 2024-04-30 11:22:06.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/cesnet_dataset.py
+-rw-rw-rw-   0        0        0     3617 2024-03-13 15:20:57.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/datasets.py
+-rw-rw-rw-   0        0        0    29154 2024-03-13 15:20:40.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/datasets_constants.py
+-rw-rw-rw-   0        0        0     1854 2024-03-14 10:53:21.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/loaders.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:38:42.975318 cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/metadata/
+-rw-rw-rw-   0        0        0        0 2023-08-21 14:08:44.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/metadata/__init__.py
+-rw-rw-rw-   0        0        0     1623 2024-04-26 12:35:59.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/metadata/dataset_metadata.py
+-rw-rw-rw-   0        0        0     2175 2024-03-19 11:54:21.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/metadata/metadata.csv
+-rw-rw-rw-   0        0        0    15137 2024-04-26 12:36:13.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/statistics.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:38:42.978157 cesnet_datazoo-0.1.6/cesnet_datazoo/metrics/
+-rw-rw-rw-   0        0        0        0 2023-08-17 21:32:34.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/metrics/__init__.py
+-rw-rw-rw-   0        0        0     3981 2024-04-26 10:13:11.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/metrics/classification_report.py
+-rw-rw-rw-   0        0        0     1374 2024-04-17 16:35:50.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/metrics/provider_metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:38:42.981592 cesnet_datazoo-0.1.6/cesnet_datazoo/pytables_data/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:24:29.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/pytables_data/__init__.py
+-rw-rw-rw-   0        0        0     1411 2023-10-30 20:40:56.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/pytables_data/apps_split.py
+-rw-rw-rw-   0        0        0     5236 2024-05-06 10:36:54.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/pytables_data/data_scalers.py
+-rw-rw-rw-   0        0        0    13717 2024-04-26 12:13:42.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/pytables_data/indices_setup.py
+-rw-rw-rw-   0        0        0    19431 2024-04-30 11:22:10.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/pytables_data/pytables_dataset.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:38:42.986093 cesnet_datazoo-0.1.6/cesnet_datazoo/utils/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:35:45.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/utils/__init__.py
+-rw-rw-rw-   0        0        0     2462 2024-04-04 20:29:42.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/utils/class_info.py
+-rw-rw-rw-   0        0        0     1441 2024-02-20 11:51:54.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/utils/download.py
+-rw-rw-rw-   0        0        0      642 2023-09-01 13:43:06.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/utils/fileutils.py
+-rw-rw-rw-   0        0        0      575 2023-09-26 08:58:11.000000 cesnet_datazoo-0.1.6/cesnet_datazoo/utils/random.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:38:42.988232 cesnet_datazoo-0.1.6/cesnet_datazoo.egg-info/
+-rw-rw-rw-   0        0        0    12953 2024-05-06 11:38:42.000000 cesnet_datazoo-0.1.6/cesnet_datazoo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2024-05-06 11:38:42.000000 cesnet_datazoo-0.1.6/cesnet_datazoo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 11:38:42.000000 cesnet_datazoo-0.1.6/cesnet_datazoo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      238 2024-05-06 11:38:42.000000 cesnet_datazoo-0.1.6/cesnet_datazoo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-06 11:38:42.000000 cesnet_datazoo-0.1.6/cesnet_datazoo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1792 2024-05-06 11:37:37.000000 cesnet_datazoo-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 11:38:42.990233 cesnet_datazoo-0.1.6/setup.cfg
```

### Comparing `cesnet_datazoo-0.1.5/LICENCE` & `cesnet_datazoo-0.1.6/LICENCE`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/PKG-INFO` & `cesnet_datazoo-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-datazoo
-Version: 0.1.5
+Version: 0.1.6
 Summary: A toolkit for large network traffic datasets
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-datazoo
 Project-URL: Documentation, https://cesnet.github.io/cesnet-datazoo/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-datazoo/issues
```

### Comparing `cesnet_datazoo-0.1.5/README.md` & `cesnet_datazoo-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/config.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import hashlib
 import json
 import os
 import warnings
 from dataclasses import InitVar, field
 from datetime import datetime
 from enum import Enum
+from importlib.metadata import version
 from typing import TYPE_CHECKING, Callable, Literal, Optional
 
 import yaml
 from pydantic import model_validator
 from pydantic.dataclasses import dataclass
 
 from cesnet_datazoo.constants import (PHIST_BIN_COUNT, PPI_MAX_LEN, QUIC_SNI_COLUMN,
@@ -79,28 +80,30 @@
     """Iterate train data in random order."""
     SEQUENTIAL = "sequential"
     """Iterate train data in sequential (datetime) order."""
     def __str__(self): return self.value
 
 @dataclass(frozen=True)
 class TrainDataParams():
+    datazoo_version: str
     database_filename: str
     train_period_name: str
     train_tables_paths: list[str]
     apps_selection: AppSelection
     apps_selection_topx: int
     apps_selection_background_unknown: list[str]
     apps_selection_fixed_known: list[str]
     apps_selection_fixed_unknown: list[str]
     disabled_apps: list[str]
     min_train_samples_check: MinTrainSamplesCheck
     min_train_samples_per_app: int
 
 @dataclass(frozen=True)
 class TestDataParams():
+    datazoo_version: str
     database_filename: str
     test_period_name: str
     test_tables_paths: list[str]
     known_apps: list[str]
     unknown_apps: list[str]
 
 class C:
@@ -493,22 +496,20 @@
     def _get_train_data_hash(self) -> str:
         train_data_params = self._get_train_data_params()
         params_hash = hashlib.sha256(json.dumps(dataclasses.asdict(train_data_params), sort_keys=True, default=str).encode()).hexdigest()
         params_hash = params_hash[:10]
         return params_hash
 
     def _get_train_data_path(self) -> str:
-        if self.need_train_set:
-            params_hash = self._get_train_data_hash()
-            return os.path.join(self.data_root, "train-data", f"{params_hash}_{self.random_state}", f"fold_{self.fold_id}")
-        else:
-            return os.path.join(self.data_root, "train-data", "default")
+        params_hash = self._get_train_data_hash()
+        return os.path.join(self.data_root, "train-data", f"{params_hash}_{self.random_state}", f"fold_{self.fold_id}")
 
     def _get_train_data_params(self) -> TrainDataParams:
         return TrainDataParams(
+            datazoo_version=version("cesnet_datazoo"),
             database_filename=self.database_filename,
             train_period_name=self.train_period_name,
             train_tables_paths=self._get_train_tables_paths(),
             apps_selection=self.apps_selection,
             apps_selection_topx=self.apps_selection_topx,
             apps_selection_background_unknown=self.apps_selection_background_unknown,
             apps_selection_fixed_known=self.apps_selection_fixed_known,
@@ -516,26 +517,28 @@
             disabled_apps=self.disabled_apps,
             min_train_samples_per_app=self.min_train_samples_per_app,
             min_train_samples_check=self.min_train_samples_check,)
 
     def _get_val_data_params_and_path(self, known_apps: list[str], unknown_apps: list[str]) -> tuple[TestDataParams, str]:
         assert self.val_approach == ValidationApproach.VALIDATION_DATES
         val_data_params = TestDataParams(
+            datazoo_version=version("cesnet_datazoo"),
             database_filename=self.database_filename,
             test_period_name=self.val_period_name,
             test_tables_paths=self._get_val_tables_paths(),
             known_apps=known_apps,
             unknown_apps=unknown_apps,)
         params_hash = hashlib.sha256(json.dumps(dataclasses.asdict(val_data_params), sort_keys=True).encode()).hexdigest()
         params_hash = params_hash[:10]
         val_data_path = os.path.join(self.data_root, "val-data", f"{params_hash}_{self.random_state}")
         return val_data_params, val_data_path
 
     def _get_test_data_params_and_path(self, known_apps: list[str], unknown_apps: list[str]) -> tuple[TestDataParams, str]:
         test_data_params = TestDataParams(
+            datazoo_version=version("cesnet_datazoo"),
             database_filename=self.database_filename,
             test_period_name=self.test_period_name,
             test_tables_paths=self._get_test_tables_paths(),
             known_apps=known_apps,
             unknown_apps=unknown_apps,)
         params_hash = hashlib.sha256(json.dumps(dataclasses.asdict(test_data_params), sort_keys=True).encode()).hexdigest()
         params_hash = params_hash[:10]
```

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/constants.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/constants.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/cesnet_dataset.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/cesnet_dataset.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/datasets.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/datasets_constants.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/datasets_constants.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/loaders.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/loaders.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/metadata/dataset_metadata.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/metadata/dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/metadata/metadata.csv` & `cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/metadata/metadata.csv`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/datasets/statistics.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/datasets/statistics.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/metrics/classification_report.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/metrics/classification_report.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/metrics/provider_metrics.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/metrics/provider_metrics.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/apps_split.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/pytables_data/apps_split.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/data_scalers.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/pytables_data/data_scalers.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/indices_setup.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/pytables_data/indices_setup.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/pytables_data/pytables_dataset.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/pytables_data/pytables_dataset.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/utils/class_info.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/utils/class_info.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/utils/download.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/utils/download.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/utils/fileutils.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/utils/fileutils.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo/utils/random.py` & `cesnet_datazoo-0.1.6/cesnet_datazoo/utils/random.py`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo.egg-info/PKG-INFO` & `cesnet_datazoo-0.1.6/cesnet_datazoo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-datazoo
-Version: 0.1.5
+Version: 0.1.6
 Summary: A toolkit for large network traffic datasets
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-datazoo
 Project-URL: Documentation, https://cesnet.github.io/cesnet-datazoo/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-datazoo/issues
```

### Comparing `cesnet_datazoo-0.1.5/cesnet_datazoo.egg-info/SOURCES.txt` & `cesnet_datazoo-0.1.6/cesnet_datazoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cesnet_datazoo-0.1.5/pyproject.toml` & `cesnet_datazoo-0.1.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cesnet-datazoo"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
 ]
 maintainers = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
```

