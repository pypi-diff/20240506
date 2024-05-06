# Comparing `tmp/oda_data-1.1.6.tar.gz` & `tmp/oda_data-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oda_data-1.1.6.tar", max compression
+gzip compressed data, was "oda_data-1.2.0.tar", max compression
```

## Comparing `oda_data-1.1.6.tar` & `oda_data-1.2.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1069 2024-03-14 13:10:20.138595 oda_data-1.1.6/LICENSE
--rw-r--r--   0        0        0     5079 2024-03-14 13:10:20.138595 oda_data-1.1.6/README.md
--rw-r--r--   0        0        0      157 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/.raw_data/README.md
--rw-r--r--   0        0        0      184 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/README.md
--rw-r--r--   0        0        0     1411 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/__init__.py
--rw-r--r--   0        0        0      782 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/classes/README.md
--rw-r--r--   0        0        0        0 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/classes/__init__.py
--rw-r--r--   0        0        0    23889 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/classes/oda_data.py
--rw-r--r--   0        0        0      360 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/classes/representations.py
--rw-r--r--   0        0        0      476 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/clean_data/README.md
--rw-r--r--   0        0        0        0 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/clean_data/__init__.py
--rw-r--r--   0        0        0    22036 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/clean_data/channels.py
--rw-r--r--   0        0        0     5540 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/clean_data/common.py
--rw-r--r--   0        0        0    19114 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/clean_data/crs_channel_mapping.csv
--rw-r--r--   0        0        0     7977 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/clean_data/dtypes.py
--rw-r--r--   0        0        0    11277 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/clean_data/schema.py
--rw-r--r--   0        0        0      882 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/config.py
--rw-r--r--   0        0        0     3189 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/get_data/README.md
--rw-r--r--   0        0        0        0 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/get_data/__init__.py
--rw-r--r--   0        0        0    10117 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/get_data/common.py
--rw-r--r--   0        0        0     1858 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/get_data/crs.py
--rw-r--r--   0        0        0      704 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/get_data/dac1.py
--rw-r--r--   0        0        0      710 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/get_data/dac2a.py
--rw-r--r--   0        0        0      802 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/get_data/multisystem.py
--rw-r--r--   0        0        0      119 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/indicators/README.md
--rw-r--r--   0        0        0        0 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/indicators/__init__.py
--rw-r--r--   0        0        0     1586 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/indicators/linked_indicators.py
--rw-r--r--   0        0        0     8260 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/indicators/research_indicators.py
--rw-r--r--   0        0        0     6428 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/indicators/sector_components.py
--rw-r--r--   0        0        0      698 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/logger.py
--rw-r--r--   0        0        0      603 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/read_data/README.md
--rw-r--r--   0        0        0        0 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/read_data/__init__.py
--rw-r--r--   0        0        0     3129 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/read_data/read.py
--rw-r--r--   0        0        0    10207 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/settings/Available indicators.md
--rw-r--r--   0        0        0     5540 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/settings/README.md
--rw-r--r--   0        0        0     2570 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/settings/channel_codes.json
--rw-r--r--   0        0        0     7759 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/settings/donor_groupings.json
--rw-r--r--   0        0        0    27566 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/settings/indicators.json
--rw-r--r--   0        0        0     1862 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/settings/key_columns.json
--rw-r--r--   0        0        0    17756 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/settings/recipient_groupings.json
--rw-r--r--   0        0        0       78 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/tools/README.md
--rw-r--r--   0        0        0        0 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/tools/__init__.py
--rw-r--r--   0        0        0      799 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/tools/groupings.py
--rw-r--r--   0        0        0     6113 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/tools/names.py
--rw-r--r--   0        0        0    12207 2024-03-14 13:10:20.138595 oda_data-1.1.6/oda_data/tools/sector_lists.py
--rw-r--r--   0        0        0     1094 2024-03-14 13:10:20.138595 oda_data-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     6061 1970-01-01 00:00:00.000000 oda_data-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-06 10:57:11.453071 oda_data-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5079 2024-05-06 10:57:11.453071 oda_data-1.2.0/README.md
+-rw-r--r--   0        0        0      157 2024-05-06 10:57:11.453071 oda_data-1.2.0/oda_data/.raw_data/README.md
+-rw-r--r--   0        0        0      184 2024-05-06 10:57:11.453071 oda_data-1.2.0/oda_data/README.md
+-rw-r--r--   0        0        0     1411 2024-05-06 10:57:11.453071 oda_data-1.2.0/oda_data/__init__.py
+-rw-r--r--   0        0        0      782 2024-05-06 10:57:11.453071 oda_data-1.2.0/oda_data/classes/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 10:57:11.453071 oda_data-1.2.0/oda_data/classes/__init__.py
+-rw-r--r--   0        0        0    23889 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/classes/oda_data.py
+-rw-r--r--   0        0        0      360 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/classes/representations.py
+-rw-r--r--   0        0        0      476 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/clean_data/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/clean_data/__init__.py
+-rw-r--r--   0        0        0    22036 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/clean_data/channels.py
+-rw-r--r--   0        0        0     5540 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/clean_data/common.py
+-rw-r--r--   0        0        0    19114 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/clean_data/crs_channel_mapping.csv
+-rw-r--r--   0        0        0     7977 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/clean_data/dtypes.py
+-rw-r--r--   0        0        0    11277 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/clean_data/schema.py
+-rw-r--r--   0        0        0      882 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/config.py
+-rw-r--r--   0        0        0     3189 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/get_data/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/get_data/__init__.py
+-rw-r--r--   0        0        0    10117 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/get_data/common.py
+-rw-r--r--   0        0        0     1858 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/get_data/crs.py
+-rw-r--r--   0        0        0      827 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/get_data/dac1.py
+-rw-r--r--   0        0        0      818 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/get_data/dac2a.py
+-rw-r--r--   0        0        0      802 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/get_data/multisystem.py
+-rw-r--r--   0        0        0      119 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/indicators/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/indicators/__init__.py
+-rw-r--r--   0        0        0     1586 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/indicators/linked_indicators.py
+-rw-r--r--   0        0        0     8260 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/indicators/research_indicators.py
+-rw-r--r--   0        0        0     6428 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/indicators/sector_components.py
+-rw-r--r--   0        0        0      698 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/logger.py
+-rw-r--r--   0        0        0      603 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/read_data/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/read_data/__init__.py
+-rw-r--r--   0        0        0     3571 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/read_data/read.py
+-rw-r--r--   0        0        0    10207 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/settings/Available indicators.md
+-rw-r--r--   0        0        0     5540 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/settings/README.md
+-rw-r--r--   0        0        0     2570 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/settings/channel_codes.json
+-rw-r--r--   0        0        0     7759 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/settings/donor_groupings.json
+-rw-r--r--   0        0        0    27574 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/settings/indicators.json
+-rw-r--r--   0        0        0     1862 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/settings/key_columns.json
+-rw-r--r--   0        0        0    17756 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/settings/recipient_groupings.json
+-rw-r--r--   0        0        0       78 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/tools/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/tools/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/tools/groupings.py
+-rw-r--r--   0        0        0     6113 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/tools/names.py
+-rw-r--r--   0        0        0    12207 2024-05-06 10:57:11.457071 oda_data-1.2.0/oda_data/tools/sector_lists.py
+-rw-r--r--   0        0        0      897 2024-05-06 10:57:11.457071 oda_data-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5972 1970-01-01 00:00:00.000000 oda_data-1.2.0/PKG-INFO
```

### Comparing `oda_data-1.1.6/LICENSE` & `oda_data-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/README.md` & `oda_data-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/__init__.py` & `oda_data-1.2.0/oda_data/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1.6"
+__version__ = "1.2.0"
 
 from oda_data import tools
 from oda_data.classes.oda_data import ODAData
 from oda_data.clean_data.channels import get_spending_channel_mapping
 from oda_data.get_data.crs import download_crs
 from oda_data.get_data.dac1 import download_dac1
 from oda_data.get_data.dac2a import download_dac2a
```

### Comparing `oda_data-1.1.6/oda_data/classes/README.md` & `oda_data-1.2.0/oda_data/classes/README.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/classes/oda_data.py` & `oda_data-1.2.0/oda_data/classes/oda_data.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/clean_data/channels.py` & `oda_data-1.2.0/oda_data/clean_data/channels.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/clean_data/common.py` & `oda_data-1.2.0/oda_data/clean_data/common.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/clean_data/crs_channel_mapping.csv` & `oda_data-1.2.0/oda_data/clean_data/crs_channel_mapping.csv`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/clean_data/dtypes.py` & `oda_data-1.2.0/oda_data/clean_data/dtypes.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/clean_data/schema.py` & `oda_data-1.2.0/oda_data/clean_data/schema.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/config.py` & `oda_data-1.2.0/oda_data/config.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/get_data/README.md` & `oda_data-1.2.0/oda_data/get_data/README.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/get_data/common.py` & `oda_data-1.2.0/oda_data/get_data/common.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/get_data/crs.py` & `oda_data-1.2.0/oda_data/get_data/crs.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/get_data/dac1.py` & `oda_data-1.2.0/oda_data/get_data/multisystem.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from oda_data import config
+
 from oda_data.get_data import common
 from oda_data.logger import logger
 
 
-def download_dac1() -> None:
+def download_multisystem() -> None:
     """Download the DAC1 file from OECD.Stat. Data for all years is downloaded at once.
     This function stores the raw data as a feather file in the raw data folder.
 
     Args:
         small_version: optionally save a smaller version of the file with only key
-            columns (default is False)."""
-    logger.info(f"Downloading DAC1 data... This may take a while.")
+             columns (default is False)."""
+
+    logger.info(f"Downloading Multisystem data... This may take a while.")
     common.download_single_table(
-        bulk_url=config.TABLE1_URL,
-        raw_file_name="Table1_Data.csv",
-        output_file_name="table1_raw",
+        bulk_url=config.MULTISYSTEM_URL,
+        raw_file_name="MultiSystem entire dataset.txt",
+        output_file_name="multisystem_raw",
         save_path=config.OdaPATHS.raw_data,
     )
+
+
+if __name__ == "__main__":
+    download_multisystem()
```

### Comparing `oda_data-1.1.6/oda_data/indicators/linked_indicators.py` & `oda_data-1.2.0/oda_data/indicators/linked_indicators.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/indicators/research_indicators.py` & `oda_data-1.2.0/oda_data/indicators/research_indicators.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/indicators/sector_components.py` & `oda_data-1.2.0/oda_data/indicators/sector_components.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/logger.py` & `oda_data-1.2.0/oda_data/logger.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/read_data/README.md` & `oda_data-1.2.0/oda_data/read_data/README.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/read_data/read.py` & `oda_data-1.2.0/oda_data/read_data/read.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,18 +7,25 @@
 from oda_data.get_data.crs import download_crs
 from oda_data.get_data.dac1 import download_dac1
 from oda_data.get_data.dac2a import download_dac2a
 from oda_data.get_data.multisystem import download_multisystem
 from oda_data.logger import logger
 
 
-def __read_table(years: int | list | range, file_name: str) -> pd.DataFrame:
+def __read_table(
+    years: int | list | range, file_name: str, check_years: bool = False
+) -> pd.DataFrame:
     # Check that list of years is valid
     years = common.check_integers(years)
 
+    if check_years:
+        start_year = min(years)
+        end_year = max(years)
+        file_name = f"{file_name.split('.')[0]}_{start_year}_{end_year}.feather"
+
     # Read the table
     df = pd.read_feather(config.OdaPATHS.raw_data / file_name)
 
     return df.loc[lambda d: d.year.isin(years)].reset_index(drop=True)
 
 
 def read_crs(years: int | list | range) -> pd.DataFrame:
@@ -51,30 +58,40 @@
     return df
 
 
 def read_dac1(years: int | list | range) -> pd.DataFrame:
     """Read the DAC1 data for the specified years."""
     # Check that list of years is valid
     try:
-        return __read_table(years=years, file_name="table1_raw.feather")
+        return __read_table(
+            years=years, file_name="table1_raw.feather", check_years=True
+        )
     except FileNotFoundError:
-        logger.info("DAC1 data not found. Downloading...")
-        download_dac1()
-        return __read_table(years=years, file_name="table1_raw.feather")
+        start_year = min(years)
+        end_year = max(years)
+        download_dac1(start_year=start_year, end_year=end_year)
+        return __read_table(
+            years=years, file_name="table1_raw.feather", check_years=True
+        )
 
 
 def read_dac2a(years: int | list | range) -> pd.DataFrame:
     """Read the DAC2a data for the specified years."""
     # Check that list of years is valid
     try:
-        return __read_table(years=years, file_name="table2a_raw.feather")
+        return __read_table(
+            years=years, file_name="table2a_raw.feather", check_years=True
+        )
     except FileNotFoundError:
-        logger.info("DAC2a data not found. Downloading...")
-        download_dac2a()
-        return __read_table(years=years, file_name="table2a_raw.feather")
+        start_year = min(years)
+        end_year = max(years)
+        download_dac2a(start_year=start_year, end_year=end_year)
+        return __read_table(
+            years=years, file_name="table2a_raw.feather", check_years=True
+        )
 
 
 def read_multisystem(years: int | list | range) -> pd.DataFrame:
     """Read the Multisystem data for the specified years."""
     # Check that list of years is valid
     try:
         return __read_table(years=years, file_name="multisystem_raw.feather")
```

### Comparing `oda_data-1.1.6/oda_data/settings/Available indicators.md` & `oda_data-1.2.0/oda_data/settings/Available indicators.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/settings/README.md` & `oda_data-1.2.0/oda_data/settings/README.md`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/settings/channel_codes.json` & `oda_data-1.2.0/oda_data/settings/channel_codes.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/settings/donor_groupings.json` & `oda_data-1.2.0/oda_data/settings/donor_groupings.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/settings/indicators.json` & `oda_data-1.2.0/oda_data/settings/indicators.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967320261437905%*

 * *Differences: {"'recipient_bilateral_flow_gross'": "{'filters': {'data_type_code': 'A', delete: "*

 * *                                     "['datatype_code']}}",*

 * * "'recipient_bilateral_flow_net'": "{'filters': {'data_type_code': 'A', delete: "*

 * *                                   "['datatype_code']}}",*

 * * "'recipient_grants_flow'": "{'filters': {'data_type_code': 'A', delete: ['datatype_code']}}",*

 * * "'recipient_humanitarian_flow'": "{'filters': {'data_type_code': 'A', delete: ['datatype_code']}}",*

 * * "'recipient_imputed_multi_flow_ […]*

```diff
@@ -733,78 +733,78 @@
         "share_of": "total_oda_ge",
         "source": "dac1",
         "type": "one_research"
     },
     "recipient_bilateral_flow_gross": {
         "filters": {
             "aidtype_code": 240,
-            "datatype_code": "A"
+            "data_type_code": "A"
         },
         "share_of": "",
         "source": "dac2a",
         "type": "dac"
     },
     "recipient_bilateral_flow_net": {
         "filters": {
             "aidtype_code": 206,
-            "datatype_code": "A"
+            "data_type_code": "A"
         },
         "share_of": "recipient_total_flow_net",
         "source": "dac2a",
         "type": "dac"
     },
     "recipient_grants_flow": {
         "filters": {
             "aidtype_code": 201,
-            "datatype_code": "A"
+            "data_type_code": "A"
         },
         "share_of": "recipient_total_flow_net",
         "source": "dac2a",
         "type": "dac"
     },
     "recipient_humanitarian_flow": {
         "filters": {
             "aidtype_code": 216,
-            "datatype_code": "A"
+            "data_type_code": "A"
         },
         "share_of": "recipient_total_flow_net",
         "source": "dac2a",
         "type": "dac"
     },
     "recipient_imputed_multi_flow_net": {
         "filters": {
             "aidtype_code": 106,
-            "datatype_code": "A"
+            "data_type_code": "A"
         },
         "share_of": "recipient_total_flow_net",
         "source": "dac2a",
         "type": "dac"
     },
     "recipient_interest_received_flow": {
         "filters": {
             "aidtype_code": 209,
-            "datatype_code": "A"
+            "data_type_code": "A"
         },
         "share_of": "recipient_total_flow_net",
         "source": "dac2a",
         "type": "dac"
     },
     "recipient_loans_flow_gross": {
         "filters": {
             "aidtype_code": 204,
-            "datatype_code": "A"
+            "data_type_code": "A"
         },
         "share_of": "",
         "source": "dac2a",
         "type": "dac"
     },
     "recipient_loans_flow_net": {
         "filters": {
             "aidtype_code": 218,
-            "datatype_code": "A"
+            "data_type_code": "A"
         },
         "share_of": "recipient_total_flow_net",
         "source": "dac2a",
         "type": "dac"
     },
     "recipient_total_flow_net": {
         "group_by": [
```

### Comparing `oda_data-1.1.6/oda_data/settings/key_columns.json` & `oda_data-1.2.0/oda_data/settings/key_columns.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/settings/recipient_groupings.json` & `oda_data-1.2.0/oda_data/settings/recipient_groupings.json`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/tools/groupings.py` & `oda_data-1.2.0/oda_data/tools/groupings.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/tools/names.py` & `oda_data-1.2.0/oda_data/tools/names.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/oda_data/tools/sector_lists.py` & `oda_data-1.2.0/oda_data/tools/sector_lists.py`

 * *Files identical despite different names*

### Comparing `oda_data-1.1.6/pyproject.toml` & `oda_data-1.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 [tool.poetry]
 name = "oda_data"
-version = "1.1.6"
+version = "1.2.0"
 description = "A python package to work with Official Development Assistance data from the OECD DAC."
 readme = "README.md"
 authors = ["Jorge Rivera <jorge.rivera@one.org>"]
 packages = [{ include = "oda_data" }]
-classifiers = ["Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Development Status :: 4 - Beta",
-]
+
 [project.urls]
 "Homepage" = "https://github.com/ONEcampaign/oda_data_package"
 "Bug Tracker" = "https://github.com/ONEcampaign/oda_data_package/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2"
 bblocks = "^1"
 requests = "^2"
-beautifulsoup4 = "^4"
 pydeflate = "^1"
 lxml = "^5"
-selenium = "^4.11.2"
-webdriver-manager = "^4.0.0"
-pyarrow = "^15"
+pyarrow = ">=14, <17"
 thefuzz = "^0.22.1"
+oda-reader = "^0.2.1"
+beautifulsoup4 = "^4.12.3"
+selenium = "^4.20.0"
+webdriver-manager = "^4.0.1"
 
 
 [tool.poetry.dev-dependencies]
 black = "^24"
 pytest = "^8"
 pytest-cov = "^4.0.0"
 bump2version = "^1.0.1"
```

### Comparing `oda_data-1.1.6/PKG-INFO` & `oda_data-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: oda_data
-Version: 1.1.6
+Version: 1.2.0
 Summary: A python package to work with Official Development Assistance data from the OECD DAC.
 Author: Jorge Rivera
 Author-email: jorge.rivera@one.org
 Requires-Python: >=3.10,<4.0
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: bblocks (>=1,<2)
-Requires-Dist: beautifulsoup4 (>=4,<5)
+Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: lxml (>=5,<6)
+Requires-Dist: oda-reader (>=0.2.1,<0.3.0)
 Requires-Dist: pandas (>=2,<3)
-Requires-Dist: pyarrow (>=15,<16)
+Requires-Dist: pyarrow (>=14,<17)
 Requires-Dist: pydeflate (>=1,<2)
 Requires-Dist: requests (>=2,<3)
-Requires-Dist: selenium (>=4.11.2,<5.0.0)
+Requires-Dist: selenium (>=4.20.0,<5.0.0)
 Requires-Dist: thefuzz (>=0.22.1,<0.23.0)
-Requires-Dist: webdriver-manager (>=4.0.0,<5.0.0)
+Requires-Dist: webdriver-manager (>=4.0.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 [![pypi](https://img.shields.io/pypi/v/oda_data.svg)](https://pypi.org/project/oda_data/)
 [![python](https://img.shields.io/pypi/pyversions/oda_data.svg)](https://pypi.org/project/oda_data/)
 [![codecov](https://codecov.io/gh/ONEcampaign/oda_data_package/branch/main/graph/badge.svg?token=G8N8BWWPL8)](https://codecov.io/gh/ONEcampaign/oda_data_package)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

