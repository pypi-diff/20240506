# Comparing `tmp/backtesting_server-0.4.0.tar.gz` & `tmp/backtesting_server-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtesting_server-0.4.0.tar", max compression
+gzip compressed data, was "backtesting_server-0.4.1.tar", max compression
```

## Comparing `backtesting_server-0.4.0.tar` & `backtesting_server-0.4.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 backtesting_server-0.4.0/LICENSE
--rw-r--r--   0        0        0      628 2024-05-06 11:20:50.871945 backtesting_server-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1858 2024-04-15 23:43:05.933161 backtesting_server-0.4.0/README.md
--rw-r--r--   0        0        0      202 2024-05-06 11:19:03.439830 backtesting_server-0.4.0/src/backtesting_server/__init__.py
--rw-r--r--   0        0        0    24700 2024-05-06 11:19:03.441228 backtesting_server-0.4.0/src/backtesting_server/main.py
--rw-r--r--   0        0        0     2465 1970-01-01 00:00:00.000000 backtesting_server-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 backtesting_server-0.4.1/LICENSE
+-rw-r--r--   0        0        0      628 2024-05-06 16:53:04.522719 backtesting_server-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1858 2024-04-15 23:43:05.933161 backtesting_server-0.4.1/README.md
+-rw-r--r--   0        0        0      202 2024-05-06 11:19:03.439830 backtesting_server-0.4.1/src/backtesting_server/__init__.py
+-rw-r--r--   0        0        0    24794 2024-05-06 16:52:41.967220 backtesting_server-0.4.1/src/backtesting_server/main.py
+-rw-r--r--   0        0        0     2465 1970-01-01 00:00:00.000000 backtesting_server-0.4.1/PKG-INFO
```

### Comparing `backtesting_server-0.4.0/LICENSE` & `backtesting_server-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `backtesting_server-0.4.0/pyproject.toml` & `backtesting_server-0.4.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "backtesting-server"
-version = "0.4.0"
+version = "0.4.1"
 description = "Package to interact with MySQL server, recording results of the backtesting."
 authors = ["hnewey7 <hnewey7@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `backtesting_server-0.4.0/README.md` & `backtesting_server-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `backtesting_server-0.4.0/src/backtesting_server/main.py` & `backtesting_server-0.4.1/src/backtesting_server/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -469,44 +469,46 @@
         group_list = "'',"
       self.cursor.execute(f"ALTER TABLE HistoricalDataSummary\
       MODIFY COLUMN InstrumentGroup SET({group_list[:-1]}) DEFAULT NULL;")
       logger.info("Successfully updated the Historical Data Summary.")
     except:
       logger.info("Could not update the Historical Data Summary.")
 
-  def upload_live_data(self, instrument_list: list[ig_package.Instrument] = [], instrument_group: InstrumentGroup = None, capture_period: int = 0) -> None:
+  def upload_live_data(self,ig: ig_package.IG, instrument_list: list[ig_package.Instrument] = [], instrument_group: InstrumentGroup = None, capture_period: int = None) -> None:
     """ Uploading live data continuously for all instruments provided.
     
       Parameters
       ----------
+      ig: ig_package.IG
+        IG object.
       instrument_list: list[ig_package.Instrument] = []
         OPTIONAL List of instruments to cycle through collecting live data and uploading to the server.
       instrument_group: InstrumentGroup = None
         OPTIONAL Instrument group defined on the Backtesting Server to cycle through.
       capture_period: int = 0
         OPTIONAL Capturing data for a certain amount of time."""
     # Collecting all Instruments to upload.
     upload_instruments = []
     if instrument_group:
-      upload_instruments.extend(instrument_group.get_instruments())
+      upload_instruments.extend(instrument_group.get_instruments(ig))
     elif instrument_list:
       upload_instruments.extend(instrument_list)
     else:
       logger.info("No instruments provided.")
     
     # Starting tracking on each instrument.
     for instrument in upload_instruments:
       instrument.start_live_data()
       logger.info("Started tracking {}.".format(instrument.epic))
 
     previous_timestamps = {}
     start_time = time.time()
 
     # Uploading data.
-    while time.time() - start_time < capture_period:
+    while capture_period == None or time.time() - start_time < capture_period:
       for instrument in upload_instruments:
         # Adding previous timestamp.
         if instrument.epic not in previous_timestamps.keys():
           previous_timestamps[instrument.epic] = instrument.ticker.timestamp
         # Checking if timestamp has changed.
         if instrument.ticker.timestamp != previous_timestamps[instrument.epic]:
           # Formatting prices.
```

### Comparing `backtesting_server-0.4.0/PKG-INFO` & `backtesting_server-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backtesting-server
-Version: 0.4.0
+Version: 0.4.1
 Summary: Package to interact with MySQL server, recording results of the backtesting.
 License: MIT
 Author: hnewey7
 Author-email: hnewey7@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

