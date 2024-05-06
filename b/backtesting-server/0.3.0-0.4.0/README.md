# Comparing `tmp/backtesting_server-0.3.0.tar.gz` & `tmp/backtesting_server-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtesting_server-0.3.0.tar", max compression
+gzip compressed data, was "backtesting_server-0.4.0.tar", max compression
```

## Comparing `backtesting_server-0.3.0.tar` & `backtesting_server-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 backtesting_server-0.3.0/LICENSE
--rw-r--r--   0        0        0      604 2024-04-29 14:41:20.099564 backtesting_server-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1858 2024-04-15 23:43:05.933161 backtesting_server-0.3.0/README.md
--rw-r--r--   0        0        0      185 2024-04-16 22:17:04.776709 backtesting_server-0.3.0/src/backtesting_server/__init__.py
--rw-r--r--   0        0        0    20813 2024-04-29 13:07:23.104806 backtesting_server-0.3.0/src/backtesting_server/main.py
--rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 backtesting_server-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 backtesting_server-0.4.0/LICENSE
+-rw-r--r--   0        0        0      628 2024-05-06 11:20:50.871945 backtesting_server-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1858 2024-04-15 23:43:05.933161 backtesting_server-0.4.0/README.md
+-rw-r--r--   0        0        0      202 2024-05-06 11:19:03.439830 backtesting_server-0.4.0/src/backtesting_server/__init__.py
+-rw-r--r--   0        0        0    24700 2024-05-06 11:19:03.441228 backtesting_server-0.4.0/src/backtesting_server/main.py
+-rw-r--r--   0        0        0     2465 1970-01-01 00:00:00.000000 backtesting_server-0.4.0/PKG-INFO
```

### Comparing `backtesting_server-0.3.0/LICENSE` & `backtesting_server-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `backtesting_server-0.3.0/pyproject.toml` & `backtesting_server-0.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "backtesting-server"
-version = "0.3.0"
+version = "0.4.0"
 description = "Package to interact with MySQL server, recording results of the backtesting."
 authors = ["hnewey7 <hnewey7@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 paramiko = "^3.4.0"
 pymysql = "^1.1.0"
-ig-package = "^1.0.4"
+ig-package = "^1.2.0"
+trading-ig = "^0.0.22"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 sphinx-autoapi = "^3.0.0"
 sphinx-rtd-theme = "^2.0.0"
 myst-nb = {version = "^1.1.0", python = "^3.9"}
```

### Comparing `backtesting_server-0.3.0/README.md` & `backtesting_server-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `backtesting_server-0.3.0/src/backtesting_server/main.py` & `backtesting_server-0.4.0/src/backtesting_server/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -103,16 +103,16 @@
         self.instrument_groups = self._get_instrument_groups()
 
       return channel, cursor
     except Exception as e:
       logger.info("Unable to connect to MySQL server.")
       raise e
 
-  def upload_historical_data(self, instrument:ig_package.Instrument, live_tracking:bool=False, dataset:pd.DataFrame=[], groups: list[InstrumentGroup] = []) -> None:
-    """ Uploading historical data to the backtesting server.
+  def upload_instrument(self, instrument:ig_package.Instrument, live_tracking:bool=False, dataset:pd.DataFrame=[], groups: list[InstrumentGroup] = []) -> None:
+    """ Uploading instrument to the backtesting server.
     
         Parameters
         ----------
         instrument: ig_package.Instrument
           Instrument the historical data corresponds to.
         live_tracking: bool = False
           OPTIONAL Enable/disable live tracking of instrument.
@@ -127,23 +127,21 @@
     # Checking if data is already present.
     if not self._check_instrument_in_historical_data(instrument):
       # Adding new instrument.
       self._add_historical_data_summary(instrument, live_tracking, groups)
 
     # Checking if data.
     if len(dataset) > 0:
-      # Filtering out NaN values.
-      dataset = dataset.dropna()
       # Inserting each row into database.
       logger.info("Inserting data into server-side dataset.")
       for data_point in dataset.index:
         try:
           insert_statement = f'INSERT INTO {instrument.name.replace(" ","_")}_HistoricalDataset (DatetimeIndex, Open, High, Low, Close) VALUES (%s, %s, %s, %s, %s)'
           values = [
-            (str(data_point), float(dataset["Open"][data_point]), float(dataset["High"][data_point]), float(dataset["Low"][data_point]), float(dataset["Close"][data_point])),
+            (str(data_point), dataset["Open"][data_point], dataset["High"][data_point], dataset["Low"][data_point], dataset["Close"][data_point]),
           ]
           self.cursor.executemany(insert_statement, values)
         except pymysql.err.IntegrityError:
           logging.info("Data point is already present in historical dataset.")
 
   def update_historical_data(self, ig:ig_package.IG, groups:list[InstrumentGroup] = []) -> None:
     """ Updating new historical data on instruments being tracked with the BacktestingServer.
@@ -263,18 +261,18 @@
     else:
       # Adding instrument to historical data summary.
       self.cursor.executemany(f"INSERT INTO HistoricalDataSummary (InstrumentName, Epic, LiveTracking) VALUES (%s, %s, %s)", [(instrument.name, instrument.epic, live_tracking)])
     # Creating new table for storing historical data.
     new_name = instrument.name.replace(" ","_")
     self.cursor.execute(f"CREATE TABLE {new_name}_HistoricalDataset (\
     DatetimeIndex DATETIME NOT NULL,\
-    Open FLOAT(20),\
-    High FLOAT(20),\
-    Low FLOAT(20),\
-    Close FLOAT(20),\
+    Open FLOAT(20) DEFAULT NULL,\
+    High FLOAT(20) DEFAULT NULL,\
+    Low FLOAT(20) DEFAULT NULL,\
+    Close FLOAT(20) DEFAULT NULL,\
     PRIMARY KEY (DatetimeIndex)\
     );")
   
   def _upload_clean_historical_data(self, instrument: ig_package.Instrument) -> None:
     """ Uploading historical data for an instrument with no previous data.
         
         Parameters
@@ -299,15 +297,15 @@
       start_time = current_epoch - 10 * resolution[1]
       start_time = datetime.fromtimestamp(start_time)
       start_time_str = start_time.strftime("%Y:%m:%d-%H:%M:%S")
       end_time_str = current_datetime.strftime("%Y:%m:%d-%H:%M:%S")
       # Getting historical prices.
       historical_data = instrument.get_historical_prices(resolution[0],start=start_time_str,end=end_time_str)
       # Uploading data.
-      self.upload_historical_data(instrument,dataset=historical_data)
+      self.upload_instrument(instrument,dataset=historical_data)
 
   def _upload_on_existing_historical_data(self, instrument:ig_package.Instrument, previous_datetime: datetime) -> None:
     """ Uploading up-to-date historical data on instrument already with existing historical data.
     
     Parameters
     ----------
     instrument: ig_package.Instrument
@@ -333,23 +331,28 @@
     ]
     # Collecting data for each resolution.
     for resolution in resolutions:
       if current_epoch - previous_epoch_time < 100 * resolution[1]:
         # Getting historical prices.
         historical_data = instrument.get_historical_prices(resolution[0],start=previous_str,end=current_str)
         # Uploading data.
-        self.upload_historical_data(instrument,dataset=historical_data)
+        self.upload_instrument(instrument,dataset=historical_data)
 
-  def add_instrument_group(self, name: str) -> None:
+  def add_instrument_group(self, name: str) -> InstrumentGroup | None:
     """ Creating an instrument group list for grouping various instruments together.
     
       Parameters
       ----------
       name: str
-        Name of the instrument group."""
+        Name of the instrument group.
+        
+      Returns
+      -------
+      InstrumentGroup | None
+        Instrument group created."""
     # Creating instrument groups table if not present.
     if not self._check_instrument_groups_table():
       self._create_instrument_groups_table()
     # Creating historical data summary.
     if not self._check_historical_data_summary_exists():
       self._create_historical_data_summary()
       
@@ -362,36 +365,44 @@
       new_group = InstrumentGroup(name,self.cursor)
       if not self.instrument_groups:
         self.instrument_groups = [new_group]
       else:
         self.instrument_groups.append(new_group)
       # Updating group data type in historical summary.
       self._update_groups_in_historical_data()
+      return new_group
     except:
       logger.info(f"Unable to add, {name}, to the instrument groups table.")
+      return None
   
-  def del_instrument_group(self, name: str) -> None:
+  def del_instrument_group(self, name: str) -> InstrumentGroup | None:
     """ Deleting the instrument group.
     
       Parameters
       ----------
       name: str
-        Name of the instrument group."""
+        Name of the instrument group.
+        
+      Returns
+      -------
+      InstrumentGroup
+        Instrument group deleted."""
     # Getting instrument group.
     for instrument_group in self.instrument_groups:
       if instrument_group.name == name:
         # Remove group from server.
         self.cursor.execute(f"DELETE FROM InstrumentGroups WHERE GroupName = '{name}';")
         # Removing instrument group object.
         self.instrument_groups.remove(instrument_group)
         logger.info(f"Successfully removed Instrument Group, {name}.")
         # Updating group data type in historical summary.
         self._update_groups_in_historical_data()
-        return
+        return instrument_group
     logger.info(f"Unable to find Instrument Group, {name}.")
+    return None
     
   def _get_instrument_groups(self) -> list[InstrumentGroup] | None:
     """ Getting all instrument groups from the Backtesting Server.
     
       Returns
       -------
       list[InstrumentGroup] | None
@@ -458,14 +469,61 @@
         group_list = "'',"
       self.cursor.execute(f"ALTER TABLE HistoricalDataSummary\
       MODIFY COLUMN InstrumentGroup SET({group_list[:-1]}) DEFAULT NULL;")
       logger.info("Successfully updated the Historical Data Summary.")
     except:
       logger.info("Could not update the Historical Data Summary.")
 
+  def upload_live_data(self, instrument_list: list[ig_package.Instrument] = [], instrument_group: InstrumentGroup = None, capture_period: int = 0) -> None:
+    """ Uploading live data continuously for all instruments provided.
+    
+      Parameters
+      ----------
+      instrument_list: list[ig_package.Instrument] = []
+        OPTIONAL List of instruments to cycle through collecting live data and uploading to the server.
+      instrument_group: InstrumentGroup = None
+        OPTIONAL Instrument group defined on the Backtesting Server to cycle through.
+      capture_period: int = 0
+        OPTIONAL Capturing data for a certain amount of time."""
+    # Collecting all Instruments to upload.
+    upload_instruments = []
+    if instrument_group:
+      upload_instruments.extend(instrument_group.get_instruments())
+    elif instrument_list:
+      upload_instruments.extend(instrument_list)
+    else:
+      logger.info("No instruments provided.")
+    
+    # Starting tracking on each instrument.
+    for instrument in upload_instruments:
+      instrument.start_live_data()
+      logger.info("Started tracking {}.".format(instrument.epic))
+
+    previous_timestamps = {}
+    start_time = time.time()
+
+    # Uploading data.
+    while time.time() - start_time < capture_period:
+      for instrument in upload_instruments:
+        # Adding previous timestamp.
+        if instrument.epic not in previous_timestamps.keys():
+          previous_timestamps[instrument.epic] = instrument.ticker.timestamp
+        # Checking if timestamp has changed.
+        if instrument.ticker.timestamp != previous_timestamps[instrument.epic]:
+          # Formatting prices.
+          price_data = [[instrument.ticker.timestamp,instrument.ticker.bid,None,None,instrument.ticker.offer]]
+          # Creating dataframe.
+          df = pd.DataFrame(price_data, columns=['Datetime', 'Open', 'High', 'Low', 'Close'])
+          df.set_index("Datetime",inplace=True)
+          # Updating previous timestamp.
+          previous_timestamps[instrument.epic] = instrument.ticker.timestamp
+
+          # Uploading data.
+          self.upload_instrument(instrument,dataset=df)
+
 # - - - - - - - - - - - - - -
 
 class InstrumentGroup():
   """ Class for representing a group of instruments on the Backtesting Server. These instruments can have entire actions performed on them, allowing for easy management of specific instruments."""
 
   def __init__(self, name:str, cursor:pymysql.cursors.Cursor) -> None:
     self.name: str = name
@@ -479,25 +537,65 @@
     
       Returns
       -------
       list[str] | None
         List of instrument names or None."""
     try:
       # Selecting instrument names with group tag.
-      self.cursor.execute('Select InstrumentName from HistoricalDataSummary WHERE InstrumentGroup = {}'.format(self.name))
+      self.cursor.execute('Select InstrumentName from HistoricalDataSummary WHERE InstrumentGroup = "{}"'.format(self.name))
       results = self.cursor.fetchall()
       # Creating list of names.
       instrument_names: list[str] = []
       for instrument_name in results:
         instrument_names.append(instrument_name[0])
       logger.info("Successfully got all instrument names for {}.".format(self.name))
       return instrument_names
     except:
       logger.info("Could not get instrument names for {}.".format(self.name))
       return None
+  
+  def _get_instrument_epics(self) -> list[str] | None:
+    """ Getting all instrument epics associated with the Instrument Group.
+      
+      Returns
+      -------
+      list[str] | None"""
+    try:
+      # Selecting instrument epics with group tag.
+      self.cursor.execute('Select Epic from HistoricalDataSummary WHERE InstrumentGroup = "{}"'.format(self.name))
+      results = self.cursor.fetchall()
+      # Creating list of epics.
+      instrument_epics: list[str] = []
+      for instrument_epic in results:
+        instrument_epics.append(instrument_epic[0])
+      logger.info("Successfully got all instrument epics for {}.".format(self.name))
+      return instrument_epics
+    except:
+      logger.info("Could not get instrument epics for {}.".format(self.name))
+      return None
+
+  def get_instruments(self,ig:ig_package.IG) -> list[ig_package.Instrument]:
+    """ Getting instruments from IG associated with the Instrument Group.
+
+      Parameters
+      ----------
+      ig: ig_package.IG
+        IG object to interact with IG REST API.
+
+      Returns
+      -------
+      list[ig_package.Instrument]
+        List of Instrument objects from the Instrument Group."""
+    # Getting epics.
+    epics = self._get_instrument_epics()
+    # Creating instruments.
+    instrument_list = []
+    for epic in epics:
+      instrument_list.append(ig_package.Instrument(epic,ig))
+    return instrument_list
     
 # - - - - - - - - - - - - - -
 
 if __name__ == "__main__":
 
   with open("logging_config.json") as f:
     config_dict = json.load(f)
```

### Comparing `backtesting_server-0.3.0/PKG-INFO` & `backtesting_server-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: backtesting-server
-Version: 0.3.0
+Version: 0.4.0
 Summary: Package to interact with MySQL server, recording results of the backtesting.
 License: MIT
 Author: hnewey7
 Author-email: hnewey7@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ig-package (>=1.0.4,<2.0.0)
+Requires-Dist: ig-package (>=1.2.0,<2.0.0)
 Requires-Dist: paramiko (>=3.4.0,<4.0.0)
 Requires-Dist: pymysql (>=1.1.0,<2.0.0)
+Requires-Dist: trading-ig (>=0.0.22,<0.0.23)
 Description-Content-Type: text/markdown
 
 # Python Package for transferring backtesting data to a MySQL server.
 
 ## A package allowing transferring of historical price data and strategy results to a MySQL server.
 
 This project is intended to allow users to connect to a MySQL server, transferring backtesting data between the two. Historical data can be uploaded and stored for later use, meaning backtesting won't be limited by the trading API.
```

