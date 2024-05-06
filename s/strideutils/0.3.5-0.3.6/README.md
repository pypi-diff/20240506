# Comparing `tmp/strideutils-0.3.5.tar.gz` & `tmp/strideutils-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strideutils-0.3.5.tar", max compression
+gzip compressed data, was "strideutils-0.3.6.tar", max compression
```

## Comparing `strideutils-0.3.5.tar` & `strideutils-0.3.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1835 2024-05-06 16:21:11.846183 strideutils-0.3.5/README.md
--rw-r--r--   0        0        0     1045 2024-05-06 16:21:11.846183 strideutils-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      373 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils/Makefile
--rw-r--r--   0        0        0        0 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils/__init__.py
--rw-r--r--   0        0        0     5408 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils/coingecko.py
--rw-r--r--   0        0        0     5673 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/config_examples/strideutils_config.yaml.example
--rw-r--r--   0        0        0      443 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/config_examples/strideutils_secrets.yaml.example
--rw-r--r--   0        0        0     1270 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/cryptography.py
--rw-r--r--   0        0        0     1835 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/exec_tx.py
--rw-r--r--   0        0        0     1664 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/invariant_helpers.py
--rw-r--r--   0        0        0     1551 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/run_safely.py
--rw-r--r--   0        0        0     6793 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/sheets_connector.py
--rw-r--r--   0        0        0     1594 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/slack_connector.py
--rw-r--r--   0        0        0     5642 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/stride_alerts.py
--rw-r--r--   0        0        0    13332 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/stride_config.py
--rw-r--r--   0        0        0    40490 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/stride_requests.py
--rw-r--r--   0        0        0     2438 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/stride_upstash.py
--rw-r--r--   0        0        0     1064 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/twilio_connector.py
--rw-r--r--   0        0        0      659 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/types.py
--rw-r--r--   0        0        0        0 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/__init__.pyi
--rw-r--r--   0        0        0      257 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/coingecko.pyi
--rw-r--r--   0        0        0      139 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/cryptography.pyi
--rw-r--r--   0        0        0      511 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/exec_tx.pyi
--rw-r--r--   0        0        0      237 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/invariant_helpers.pyi
--rw-r--r--   0        0        0      290 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/run_safely.pyi
--rw-r--r--   0        0        0      803 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/sheets_connector.pyi
--rw-r--r--   0        0        0      242 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/slack_connector.pyi
--rw-r--r--   0        0        0      987 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/stride_alerts.pyi
--rw-r--r--   0        0        0     4591 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/stride_config.pyi
--rw-r--r--   0        0        0     3977 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/stride_requests.pyi
--rw-r--r--   0        0        0      419 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/stride_upstash.pyi
--rw-r--r--   0        0        0      245 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/twilio_connector.pyi
--rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 strideutils-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1835 2024-05-06 18:52:03.169662 strideutils-0.3.6/README.md
+-rw-r--r--   0        0        0     1046 2024-05-06 18:52:03.173662 strideutils-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      373 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils/Makefile
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils/__init__.py
+-rw-r--r--   0        0        0     5408 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils/coingecko.py
+-rw-r--r--   0        0        0     5673 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils/config_examples/strideutils_config.yaml.example
+-rw-r--r--   0        0        0      443 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils/config_examples/strideutils_secrets.yaml.example
+-rw-r--r--   0        0        0     1270 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils/cryptography.py
+-rw-r--r--   0        0        0     1835 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils/exec_tx.py
+-rw-r--r--   0        0        0     1664 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils/invariant_helpers.py
+-rw-r--r--   0        0        0     1551 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils/run_safely.py
+-rw-r--r--   0        0        0     6793 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils/sheets_connector.py
+-rw-r--r--   0        0        0     1594 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils/slack_connector.py
+-rw-r--r--   0        0        0     5642 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils/stride_alerts.py
+-rw-r--r--   0        0        0    13332 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils/stride_config.py
+-rw-r--r--   0        0        0    42551 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils/stride_requests.py
+-rw-r--r--   0        0        0     2438 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils/stride_upstash.py
+-rw-r--r--   0        0        0     1064 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils/twilio_connector.py
+-rw-r--r--   0        0        0      659 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils/types.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils-stubs/__init__.pyi
+-rw-r--r--   0        0        0      257 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils-stubs/coingecko.pyi
+-rw-r--r--   0        0        0      139 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils-stubs/cryptography.pyi
+-rw-r--r--   0        0        0      511 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils-stubs/exec_tx.pyi
+-rw-r--r--   0        0        0      237 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils-stubs/invariant_helpers.pyi
+-rw-r--r--   0        0        0      290 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils-stubs/run_safely.pyi
+-rw-r--r--   0        0        0      803 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils-stubs/sheets_connector.pyi
+-rw-r--r--   0        0        0      242 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils-stubs/slack_connector.pyi
+-rw-r--r--   0        0        0      987 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils-stubs/stride_alerts.pyi
+-rw-r--r--   0        0        0     4591 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils-stubs/stride_config.pyi
+-rw-r--r--   0        0        0     3977 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils-stubs/stride_requests.pyi
+-rw-r--r--   0        0        0      419 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils-stubs/stride_upstash.pyi
+-rw-r--r--   0        0        0      245 2024-05-06 18:52:03.173662 strideutils-0.3.6/strideutils-stubs/twilio_connector.pyi
+-rw-r--r--   0        0        0     2761 1970-01-01 00:00:00.000000 strideutils-0.3.6/PKG-INFO
```

### Comparing `strideutils-0.3.5/README.md` & `strideutils-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/pyproject.toml` & `strideutils-0.3.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "strideutils"
-version = "0.3.5"
+version = "0.3.6"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 include = ["strideutils", "strideutils-stubs"]
 
 [tool.poetry.dependencies]
-python = ">=3.9"
+python = ">=3.11"
 google-api-python-client = ">=2.100.0"
 google-auth-httplib2 = ">=0.1.1"
 google-auth-oauthlib = ">=1.1.0"
 google-cloud-bigquery = ">=3.11.4"
 gspread = ">=6.0.2"
 pytz = ">=2023.3"
 redis = ">=4.5.4"
```

### Comparing `strideutils-0.3.5/strideutils/coingecko.py` & `strideutils-0.3.6/strideutils/coingecko.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/strideutils/config_examples/strideutils_config.yaml.example` & `strideutils-0.3.6/strideutils/config_examples/strideutils_config.yaml.example`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/strideutils/cryptography.py` & `strideutils-0.3.6/strideutils/cryptography.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/strideutils/exec_tx.py` & `strideutils-0.3.6/strideutils/exec_tx.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/strideutils/invariant_helpers.py` & `strideutils-0.3.6/strideutils/invariant_helpers.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/strideutils/run_safely.py` & `strideutils-0.3.6/strideutils/run_safely.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/strideutils/sheets_connector.py` & `strideutils-0.3.6/strideutils/sheets_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/strideutils/slack_connector.py` & `strideutils-0.3.6/strideutils/slack_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/strideutils/stride_alerts.py` & `strideutils-0.3.6/strideutils/stride_alerts.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/strideutils/stride_config.py` & `strideutils-0.3.6/strideutils/stride_config.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/strideutils/stride_requests.py` & `strideutils-0.3.6/strideutils/stride_requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import json
 import time
 import urllib.parse
 from functools import lru_cache
 from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
 import bech32
-import dateutil.parser
 import pandas as pd
 import pytz
 import requests
 from requests.adapters import HTTPAdapter, Retry
 
 from strideutils import stride_upstash, types
 from strideutils.stride_config import config
@@ -323,14 +322,69 @@
             if chain_id_match and status_match:
                 host_zone_unbonding["epoch_number"] = epoch_number
                 host_zone_unbondings.append(host_zone_unbonding)
 
     return host_zone_unbondings
 
 
+def get_unbonding_queue_records(chain_id: str, block_height: int = 0) -> List[Dict[str, Any]]:
+    """
+    Queries all the unbonding records that are ready to initiate an unbonding
+    This is identified by records in status UNBONDING_QUEUE with a non-zero unbonding amount
+    """
+    unbonding_records = get_unbonding_records(
+        chain_id=chain_id,
+        block_height=block_height,
+        status=types.UnbondingRecordStatus.UNBONDING_QUEUE,
+    )
+    return [ur for ur in unbonding_records if int(ur["native_token_amount"]) > 0]
+
+
+def get_unbonded_records(
+    chain_id: str,
+    block_height: int = 0,
+    filter_unbonded_last_epoch: bool = False,
+) -> List[Dict[str, Any]]:
+    """
+    Queries the list of all unbonding records records that have finished unbonding
+    This is identified by records in status EXIT_TRANSFER_QUEUE with an unbonding time
+    in the past
+    Optionally filter to records that just unbonded last epoch
+    """
+    unbonding_records = get_unbonding_records(
+        chain_id=chain_id,
+        block_height=block_height,
+        status=types.UnbondingRecordStatus.EXIT_TRANSFER_QUEUE,
+    )
+
+    # If we're fetching an older block, use that block's time as the "current time"
+    current_time = int(datetime.datetime.now().timestamp() * 1e9)
+    if block_height != 0:
+        current_time = int(get_block_time(block_height).timestamp() * 1e9)
+
+    # Filter to the records that have finished unbonding, and optionally also
+    # filter to records that just finished during the last epoch
+    day = 24 * 60 * 60 * 1e9
+    filtered_unbonding_records = []
+    for unbonding_record in unbonding_records:
+        unbonding_time = int(unbonding_record["unbonding_time"])
+
+        # Ignore records that haven't finished unbonding yet
+        if unbonding_time > current_time:
+            continue
+
+        # If filtering from last epoch, ignore records that unbonded over a day ago
+        if filter_unbonded_last_epoch and (current_time - unbonding_time) > day:
+            continue
+
+        filtered_unbonding_records.append(unbonding_record)
+
+    return filtered_unbonding_records
+
+
 def get_lsm_deposit_records(chain_id: str) -> List[Dict[str, Any]]:
     """
     Queries all the LSM deposit records
 
     [
         {
             "deposit_id": "800000.cosmoshub-4.strideXXX.cosmosvaloperXXX/1",
@@ -626,15 +680,15 @@
 def get_block_time(height: int, rpc_endpoint: str = config.stride.rpc_endpoint) -> datetime.datetime:
     """
     Returns the timestamp of the given block height on a chain
     """
     url = f"{rpc_endpoint}/block?height={height}"
     resp = request(url)
     block_time = resp["result"]["block"]["header"]["time"]
-    block_datetime = dateutil.parser.parse(block_time).replace(tzinfo=None)
+    block_datetime = datetime.datetime.fromisoformat(block_time)
     return block_datetime
 
 
 @lru_cache
 def get_icns_name(address: str) -> str:
     """
     Returns the ICNS name for the given Cosmos-SDK address, if it exists
@@ -1026,23 +1080,23 @@
 
 
 def get_stride_epoch_start_time() -> datetime.datetime:
     """
     Returns the epoch start time for the current "stride" epoch
     """
     stride_epoch = get_stride_epoch()
-    return dateutil.parser.parse(stride_epoch["current_epoch_start_time"]).replace(tzinfo=None)
+    return datetime.datetime.fromisoformat(stride_epoch["current_epoch_start_time"])
 
 
 def get_day_epoch_start_time() -> datetime.datetime:
     """
     Returns the epoch start time for the current "day" epoch
     """
     day_epoch = get_day_epoch()
-    return dateutil.parser.parse(day_epoch["current_epoch_start_time"]).replace(tzinfo=None)
+    return datetime.datetime.fromisoformat(day_epoch["current_epoch_start_time"])
 
 
 def get_stride_epoch_start_height() -> int:
     """
     Returns the epoch start time for the current "stride" epoch
     """
     stride_epoch = get_stride_epoch()
```

### Comparing `strideutils-0.3.5/strideutils/stride_upstash.py` & `strideutils-0.3.6/strideutils/stride_upstash.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/strideutils/twilio_connector.py` & `strideutils-0.3.6/strideutils/twilio_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/strideutils/types.py` & `strideutils-0.3.6/strideutils/types.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/strideutils-stubs/sheets_connector.pyi` & `strideutils-0.3.6/strideutils-stubs/sheets_connector.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/strideutils-stubs/stride_alerts.pyi` & `strideutils-0.3.6/strideutils-stubs/stride_alerts.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/strideutils-stubs/stride_config.pyi` & `strideutils-0.3.6/strideutils-stubs/stride_config.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/strideutils-stubs/stride_requests.pyi` & `strideutils-0.3.6/strideutils-stubs/stride_requests.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.5/PKG-INFO` & `strideutils-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: strideutils
-Version: 0.3.5
+Version: 0.3.6
 Summary: 
 Author: Your Name
 Author-email: you@example.com
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: bech32 (>=1.2.0)
 Requires-Dist: google-api-python-client (>=2.100.0)
 Requires-Dist: google-auth-httplib2 (>=0.1.1)
 Requires-Dist: google-auth-oauthlib (>=1.1.0)
 Requires-Dist: google-cloud-bigquery (>=3.11.4)
```

