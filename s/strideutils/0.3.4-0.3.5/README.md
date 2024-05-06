# Comparing `tmp/strideutils-0.3.4.tar.gz` & `tmp/strideutils-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strideutils-0.3.4.tar", max compression
+gzip compressed data, was "strideutils-0.3.5.tar", max compression
```

## Comparing `strideutils-0.3.4.tar` & `strideutils-0.3.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1835 2024-05-06 15:58:06.265509 strideutils-0.3.4/README.md
--rw-r--r--   0        0        0     1045 2024-05-06 15:58:06.265509 strideutils-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      373 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/Makefile
--rw-r--r--   0        0        0        0 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/__init__.py
--rw-r--r--   0        0        0     5408 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/coingecko.py
--rw-r--r--   0        0        0     5673 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/config_examples/strideutils_config.yaml.example
--rw-r--r--   0        0        0      443 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/config_examples/strideutils_secrets.yaml.example
--rw-r--r--   0        0        0     1270 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/cryptography.py
--rw-r--r--   0        0        0     1835 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/exec_tx.py
--rw-r--r--   0        0        0     1664 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/invariant_helpers.py
--rw-r--r--   0        0        0     1551 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/run_safely.py
--rw-r--r--   0        0        0     6793 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/sheets_connector.py
--rw-r--r--   0        0        0     1594 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/slack_connector.py
--rw-r--r--   0        0        0     5642 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/stride_alerts.py
--rw-r--r--   0        0        0    13332 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/stride_config.py
--rw-r--r--   0        0        0    40333 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/stride_requests.py
--rw-r--r--   0        0        0     2438 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/stride_upstash.py
--rw-r--r--   0        0        0     1064 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/twilio_connector.py
--rw-r--r--   0        0        0      659 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/types.py
--rw-r--r--   0        0        0        0 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/__init__.pyi
--rw-r--r--   0        0        0      257 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/coingecko.pyi
--rw-r--r--   0        0        0      139 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/cryptography.pyi
--rw-r--r--   0        0        0      511 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/exec_tx.pyi
--rw-r--r--   0        0        0      237 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/invariant_helpers.pyi
--rw-r--r--   0        0        0      290 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/run_safely.pyi
--rw-r--r--   0        0        0      803 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/sheets_connector.pyi
--rw-r--r--   0        0        0      242 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/slack_connector.pyi
--rw-r--r--   0        0        0      987 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/stride_alerts.pyi
--rw-r--r--   0        0        0     4591 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/stride_config.pyi
--rw-r--r--   0        0        0     3977 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/stride_requests.pyi
--rw-r--r--   0        0        0      419 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/stride_upstash.pyi
--rw-r--r--   0        0        0      245 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/twilio_connector.pyi
--rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 strideutils-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1835 2024-05-06 16:21:11.846183 strideutils-0.3.5/README.md
+-rw-r--r--   0        0        0     1045 2024-05-06 16:21:11.846183 strideutils-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      373 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils/Makefile
+-rw-r--r--   0        0        0        0 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils/__init__.py
+-rw-r--r--   0        0        0     5408 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils/coingecko.py
+-rw-r--r--   0        0        0     5673 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/config_examples/strideutils_config.yaml.example
+-rw-r--r--   0        0        0      443 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/config_examples/strideutils_secrets.yaml.example
+-rw-r--r--   0        0        0     1270 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/cryptography.py
+-rw-r--r--   0        0        0     1835 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/exec_tx.py
+-rw-r--r--   0        0        0     1664 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/invariant_helpers.py
+-rw-r--r--   0        0        0     1551 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/run_safely.py
+-rw-r--r--   0        0        0     6793 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/sheets_connector.py
+-rw-r--r--   0        0        0     1594 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/slack_connector.py
+-rw-r--r--   0        0        0     5642 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/stride_alerts.py
+-rw-r--r--   0        0        0    13332 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/stride_config.py
+-rw-r--r--   0        0        0    40490 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/stride_requests.py
+-rw-r--r--   0        0        0     2438 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/stride_upstash.py
+-rw-r--r--   0        0        0     1064 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/twilio_connector.py
+-rw-r--r--   0        0        0      659 2024-05-06 16:21:11.850183 strideutils-0.3.5/strideutils/types.py
+-rw-r--r--   0        0        0        0 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/__init__.pyi
+-rw-r--r--   0        0        0      257 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/coingecko.pyi
+-rw-r--r--   0        0        0      139 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/cryptography.pyi
+-rw-r--r--   0        0        0      511 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/exec_tx.pyi
+-rw-r--r--   0        0        0      237 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/invariant_helpers.pyi
+-rw-r--r--   0        0        0      290 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/run_safely.pyi
+-rw-r--r--   0        0        0      803 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/sheets_connector.pyi
+-rw-r--r--   0        0        0      242 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/slack_connector.pyi
+-rw-r--r--   0        0        0      987 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/stride_alerts.pyi
+-rw-r--r--   0        0        0     4591 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/stride_config.pyi
+-rw-r--r--   0        0        0     3977 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/stride_requests.pyi
+-rw-r--r--   0        0        0      419 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/stride_upstash.pyi
+-rw-r--r--   0        0        0      245 2024-05-06 16:21:11.846183 strideutils-0.3.5/strideutils-stubs/twilio_connector.pyi
+-rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 strideutils-0.3.5/PKG-INFO
```

### Comparing `strideutils-0.3.4/README.md` & `strideutils-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/pyproject.toml` & `strideutils-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strideutils"
-version = "0.3.4"
+version = "0.3.5"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 include = ["strideutils", "strideutils-stubs"]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `strideutils-0.3.4/strideutils/coingecko.py` & `strideutils-0.3.5/strideutils/coingecko.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/strideutils/config_examples/strideutils_config.yaml.example` & `strideutils-0.3.5/strideutils/config_examples/strideutils_config.yaml.example`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/strideutils/cryptography.py` & `strideutils-0.3.5/strideutils/cryptography.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/strideutils/exec_tx.py` & `strideutils-0.3.5/strideutils/exec_tx.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/strideutils/invariant_helpers.py` & `strideutils-0.3.5/strideutils/invariant_helpers.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/strideutils/run_safely.py` & `strideutils-0.3.5/strideutils/run_safely.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/strideutils/sheets_connector.py` & `strideutils-0.3.5/strideutils/sheets_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/strideutils/slack_connector.py` & `strideutils-0.3.5/strideutils/slack_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/strideutils/stride_alerts.py` & `strideutils-0.3.5/strideutils/stride_alerts.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/strideutils/stride_config.py` & `strideutils-0.3.5/strideutils/stride_config.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/strideutils/stride_requests.py` & `strideutils-0.3.5/strideutils/stride_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,14 +285,15 @@
 ) -> List[Dict[str, Any]]:
     """
     Queries all the unbonding records for a given host zone with optional status filter
 
     E.g.
     [
         {
+            "epoch_number": "575",
             "st_token_amount": "3218590",
             "native_token_amount": "0",
             "denom": "ucmdx",
             "host_zone_id": "comdex-1",
             "unbonding_time": "1713812526371636619",
             "status": "CLAIMABLE",
             "user_redemption_records": [
@@ -309,20 +310,22 @@
 
     # The structure from the response consists of:
     # - List of epoch unbonding records - one record per epoch
     # - Within each epoch unbonding record, there's one host zone unbonding record per host
     # This function returns the host zone unbonding record
     host_zone_unbondings = []
     for epoch_unbonding in epoch_unbondings:
+        epoch_number = epoch_unbonding["epoch_number"]
         for host_zone_unbonding in epoch_unbonding["host_zone_unbondings"]:
 
             chain_id_match = host_zone_unbonding["host_zone_id"] == chain_id
             status_match = not status or host_zone_unbonding["status"] == status
 
             if chain_id_match and status_match:
+                host_zone_unbonding["epoch_number"] = epoch_number
                 host_zone_unbondings.append(host_zone_unbonding)
 
     return host_zone_unbondings
 
 
 def get_lsm_deposit_records(chain_id: str) -> List[Dict[str, Any]]:
     """
```

### Comparing `strideutils-0.3.4/strideutils/stride_upstash.py` & `strideutils-0.3.5/strideutils/stride_upstash.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/strideutils/twilio_connector.py` & `strideutils-0.3.5/strideutils/twilio_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/strideutils/types.py` & `strideutils-0.3.5/strideutils/types.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/strideutils-stubs/sheets_connector.pyi` & `strideutils-0.3.5/strideutils-stubs/sheets_connector.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/strideutils-stubs/stride_alerts.pyi` & `strideutils-0.3.5/strideutils-stubs/stride_alerts.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/strideutils-stubs/stride_config.pyi` & `strideutils-0.3.5/strideutils-stubs/stride_config.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/strideutils-stubs/stride_requests.pyi` & `strideutils-0.3.5/strideutils-stubs/stride_requests.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.4/PKG-INFO` & `strideutils-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strideutils
-Version: 0.3.4
+Version: 0.3.5
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

