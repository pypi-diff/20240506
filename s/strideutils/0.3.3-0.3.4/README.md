# Comparing `tmp/strideutils-0.3.3.tar.gz` & `tmp/strideutils-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strideutils-0.3.3.tar", max compression
+gzip compressed data, was "strideutils-0.3.4.tar", max compression
```

## Comparing `strideutils-0.3.3.tar` & `strideutils-0.3.4.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     1835 2024-05-02 21:48:08.611212 strideutils-0.3.3/README.md
--rw-r--r--   0        0        0     1045 2024-05-02 21:48:08.611212 strideutils-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      373 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils/Makefile
--rw-r--r--   0        0        0        0 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils/__init__.py
--rw-r--r--   0        0        0     5408 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils/coingecko.py
--rw-r--r--   0        0        0     5673 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils/config_examples/strideutils_config.yaml.example
--rw-r--r--   0        0        0      443 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils/config_examples/strideutils_secrets.yaml.example
--rw-r--r--   0        0        0     1270 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils/cryptography.py
--rw-r--r--   0        0        0     1835 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils/exec_tx.py
--rw-r--r--   0        0        0     1664 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils/invariant_helpers.py
--rw-r--r--   0        0        0     1551 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils/run_safely.py
--rw-r--r--   0        0        0     6793 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils/sheets_connector.py
--rw-r--r--   0        0        0     1594 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils/slack_connector.py
--rw-r--r--   0        0        0     5642 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils/stride_alerts.py
--rw-r--r--   0        0        0    13252 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils/stride_config.py
--rw-r--r--   0        0        0    31030 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils/stride_requests.py
--rw-r--r--   0        0        0     2438 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils/stride_upstash.py
--rw-r--r--   0        0        0     1064 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils/twilio_connector.py
--rw-r--r--   0        0        0        0 2024-05-02 21:48:08.611212 strideutils-0.3.3/strideutils-stubs/__init__.pyi
--rw-r--r--   0        0        0      257 2024-05-02 21:48:08.611212 strideutils-0.3.3/strideutils-stubs/coingecko.pyi
--rw-r--r--   0        0        0      139 2024-05-02 21:48:08.611212 strideutils-0.3.3/strideutils-stubs/cryptography.pyi
--rw-r--r--   0        0        0      511 2024-05-02 21:48:08.611212 strideutils-0.3.3/strideutils-stubs/exec_tx.pyi
--rw-r--r--   0        0        0      237 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils-stubs/invariant_helpers.pyi
--rw-r--r--   0        0        0      290 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils-stubs/run_safely.pyi
--rw-r--r--   0        0        0      803 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils-stubs/sheets_connector.pyi
--rw-r--r--   0        0        0      242 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils-stubs/slack_connector.pyi
--rw-r--r--   0        0        0      987 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils-stubs/stride_alerts.pyi
--rw-r--r--   0        0        0     4591 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils-stubs/stride_config.pyi
--rw-r--r--   0        0        0     3977 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils-stubs/stride_requests.pyi
--rw-r--r--   0        0        0      419 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils-stubs/stride_upstash.pyi
--rw-r--r--   0        0        0      245 2024-05-02 21:48:08.615212 strideutils-0.3.3/strideutils-stubs/twilio_connector.pyi
--rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 strideutils-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1835 2024-05-06 15:58:06.265509 strideutils-0.3.4/README.md
+-rw-r--r--   0        0        0     1045 2024-05-06 15:58:06.265509 strideutils-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      373 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/Makefile
+-rw-r--r--   0        0        0        0 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/__init__.py
+-rw-r--r--   0        0        0     5408 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/coingecko.py
+-rw-r--r--   0        0        0     5673 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/config_examples/strideutils_config.yaml.example
+-rw-r--r--   0        0        0      443 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/config_examples/strideutils_secrets.yaml.example
+-rw-r--r--   0        0        0     1270 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/cryptography.py
+-rw-r--r--   0        0        0     1835 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/exec_tx.py
+-rw-r--r--   0        0        0     1664 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/invariant_helpers.py
+-rw-r--r--   0        0        0     1551 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/run_safely.py
+-rw-r--r--   0        0        0     6793 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/sheets_connector.py
+-rw-r--r--   0        0        0     1594 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/slack_connector.py
+-rw-r--r--   0        0        0     5642 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/stride_alerts.py
+-rw-r--r--   0        0        0    13332 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/stride_config.py
+-rw-r--r--   0        0        0    40333 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/stride_requests.py
+-rw-r--r--   0        0        0     2438 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/stride_upstash.py
+-rw-r--r--   0        0        0     1064 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/twilio_connector.py
+-rw-r--r--   0        0        0      659 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils/types.py
+-rw-r--r--   0        0        0        0 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/__init__.pyi
+-rw-r--r--   0        0        0      257 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/coingecko.pyi
+-rw-r--r--   0        0        0      139 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/cryptography.pyi
+-rw-r--r--   0        0        0      511 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/exec_tx.pyi
+-rw-r--r--   0        0        0      237 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/invariant_helpers.pyi
+-rw-r--r--   0        0        0      290 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/run_safely.pyi
+-rw-r--r--   0        0        0      803 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/sheets_connector.pyi
+-rw-r--r--   0        0        0      242 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/slack_connector.pyi
+-rw-r--r--   0        0        0      987 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/stride_alerts.pyi
+-rw-r--r--   0        0        0     4591 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/stride_config.pyi
+-rw-r--r--   0        0        0     3977 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/stride_requests.pyi
+-rw-r--r--   0        0        0      419 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/stride_upstash.pyi
+-rw-r--r--   0        0        0      245 2024-05-06 15:58:06.265509 strideutils-0.3.4/strideutils-stubs/twilio_connector.pyi
+-rw-r--r--   0        0        0     2861 1970-01-01 00:00:00.000000 strideutils-0.3.4/PKG-INFO
```

### Comparing `strideutils-0.3.3/README.md` & `strideutils-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.3/pyproject.toml` & `strideutils-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strideutils"
-version = "0.3.3"
+version = "0.3.4"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 include = ["strideutils", "strideutils-stubs"]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `strideutils-0.3.3/strideutils/coingecko.py` & `strideutils-0.3.4/strideutils/coingecko.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.3/strideutils/config_examples/strideutils_config.yaml.example` & `strideutils-0.3.4/strideutils/config_examples/strideutils_config.yaml.example`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.3/strideutils/cryptography.py` & `strideutils-0.3.4/strideutils/cryptography.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.3/strideutils/exec_tx.py` & `strideutils-0.3.4/strideutils/exec_tx.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.3/strideutils/invariant_helpers.py` & `strideutils-0.3.4/strideutils/invariant_helpers.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.3/strideutils/run_safely.py` & `strideutils-0.3.4/strideutils/run_safely.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.3/strideutils/sheets_connector.py` & `strideutils-0.3.4/strideutils/sheets_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.3/strideutils/slack_connector.py` & `strideutils-0.3.4/strideutils/slack_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.3/strideutils/stride_alerts.py` & `strideutils-0.3.4/strideutils/stride_alerts.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.3/strideutils/stride_config.py` & `strideutils-0.3.4/strideutils/stride_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,16 @@
     # Frequency with which staking rewards are issued
     # -1 indicates every block
     inflation_frequency_hours: int = -1
     # IBC denom of the native token as it sits on stride
     denom_on_stride: str = ""
     # Indicates whether the chain has ICA enabled
     ica_enabled: bool = True
+    # Indicates whether the chain has LSM enabled
+    lsm_enabled: bool = False
 
     def __repr__(self) -> str:
         return f"HostChainConfig(name={self.name}, id={self.id})"
 
 
 @dataclass(repr=False)
 class HostChainsConfig(ConfigObj):
```

### Comparing `strideutils-0.3.3/strideutils/stride_requests.py` & `strideutils-0.3.4/strideutils/stride_requests.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import bech32
 import dateutil.parser
 import pandas as pd
 import pytz
 import requests
 from requests.adapters import HTTPAdapter, Retry
 
-from strideutils import stride_upstash
+from strideutils import stride_upstash, types
 from strideutils.stride_config import config
 
 ACCOUNT_QUERY = "cosmos/auth/v1beta1/accounts/{address}"
 ACCOUNT_BALANCE_QUERY = "cosmos/bank/v1beta1/balances/{address}"
 ACCOUNT_DELEGATIONS_QUERY = "cosmos/staking/v1beta1/delegations/{delegator_address}"
 ACCOUNT_UNBONDINGS_QUERY = "cosmos/staking/v1beta1/delegators/{delegator_address}/unbonding_delegations"
 MODULE_ACCOUNTS_QUERY = "cosmos/auth/v1beta1/module_accounts"
@@ -30,30 +30,36 @@
 CHANNEL_QUERY = "ibc/core/channel/v1/channels/{channel_id}/ports/{port_id}"
 
 TXS_QUERY = "cosmos/tx/v1beta1/txs"
 TX_BY_ACCOUNT_EVENT = "tx.acc_seq='{address}/{sequence}'"
 
 HOST_ZONE_QUERY = "Stride-Labs/stride/stakeibc/host_zone"
 EPOCHS_QUERY = "Stridelabs/stride/epochs"
-
+PENDING_ICQ_QUERY = "Stride-Labs/stride/interchainquery/pending_queries"
 RATE_LIMIT_QUERY = "Stride-Labs/ibc-rate-limiting/ratelimit/ratelimits"
+DEPOSIT_RECORDS_QUERY = "Stride-Labs/stride/records/deposit_record_by_host_zone/{chain_id}"
+UNBONDING_RECORDS_QUERY = "Stride-Labs/stride/records/epoch_unbonding_record"
+LSM_RECORDS_QUERY = "Stride-Labs/stride/stakeibc/lsm_deposits"
+CALLBACK_DATA_QUERY = "Stride-Labs/stride/icacallbacks/callback_data"
 
 STAKETIA = "staketia"
 STAKEDYM = "stakedym"
 
 CELESTIA_CHAIN_ID = "celestia"
 DYMENSION_CHAIN_ID = "dymension_1100-1"
 
 MULTISIG_HOST_ZONE_QUERY = "Stride-Labs/stride/{module}/host_zone"
 MULTISIG_DELEGATION_RECORDS_QUERY = "Stride-Labs/stride/{module}/delegation_records"
 MULTISIG_UNBONDING_RECORDS_QUERY = "Stride-Labs/stride/{module}/unbonding_records"
 MULTISIG_REDEMPTION_RECORDS_QUERY = "Stride-Labs/stride/{module}/redemption_records"
 
 COSMWASM_CONTRACT_QUERY = "cosmwasm/wasm/v1/contract/{contract_address}/smart/{query}"
 
+HOST_CHANNELS_QUERY = "https://channels.main.stridenet.co/api/data/{chain_id}"
+
 requests_session = requests.Session()
 
 retries = Retry(total=5, backoff_factor=0.5, status_forcelist=[400, 403, 404, 500, 502, 503, 504])
 
 requests_session.mount("http://", HTTPAdapter(max_retries=retries))
 requests_session.mount("https://", HTTPAdapter(max_retries=retries))
 
@@ -240,14 +246,114 @@
 
     if cast_types:
         host_zone = _cast_host_zone_fields(host_zone)
 
     return host_zone
 
 
+def get_deposit_records(
+    chain_id: str,
+    status: Optional[types.DepositRecordStatus] = None,
+    block_height: int = 0,
+) -> List[Dict[str, Any]]:
+    """
+    Queries all the deposit records for a given host zone with optional status filter
+
+    E.g.
+    [
+        {
+            "id": "36310",
+            "amount": "5305210",
+            "denom": "uluna",
+            "host_zone_id": "phoenix-1",
+            "status": "DELEGATION_QUEUE",
+            "deposit_epoch_number": "2424",
+            "source": "STRIDE"
+        },
+    ]
+    """
+    url = f"{config.stride.api_endpoint}/{DEPOSIT_RECORDS_QUERY.format(chain_id=chain_id)}"
+    deposit_records = request(url, block_height=block_height)["deposit_record"]
+    if status:
+        deposit_records = [dr for dr in deposit_records if dr["status"] == status]
+    return deposit_records
+
+
+def get_unbonding_records(
+    chain_id: str,
+    status: Optional[types.UnbondingRecordStatus] = None,
+    block_height: int = 0,
+) -> List[Dict[str, Any]]:
+    """
+    Queries all the unbonding records for a given host zone with optional status filter
+
+    E.g.
+    [
+        {
+            "st_token_amount": "3218590",
+            "native_token_amount": "0",
+            "denom": "ucmdx",
+            "host_zone_id": "comdex-1",
+            "unbonding_time": "1713812526371636619",
+            "status": "CLAIMABLE",
+            "user_redemption_records": [
+                "comdex-1.575.comdex1gwnfjj65zhxmtnpxzy625cpx692lfjuwlqeg8p",
+                ...
+            ]
+        },
+        ...
+    ]
+    """
+    # Query the epoch unbonding records
+    url = f"{config.stride.api_endpoint}/{UNBONDING_RECORDS_QUERY}"
+    epoch_unbondings = query_list_with_pagination(url, rel_key="epoch_unbonding_record", block_height=block_height)
+
+    # The structure from the response consists of:
+    # - List of epoch unbonding records - one record per epoch
+    # - Within each epoch unbonding record, there's one host zone unbonding record per host
+    # This function returns the host zone unbonding record
+    host_zone_unbondings = []
+    for epoch_unbonding in epoch_unbondings:
+        for host_zone_unbonding in epoch_unbonding["host_zone_unbondings"]:
+
+            chain_id_match = host_zone_unbonding["host_zone_id"] == chain_id
+            status_match = not status or host_zone_unbonding["status"] == status
+
+            if chain_id_match and status_match:
+                host_zone_unbondings.append(host_zone_unbonding)
+
+    return host_zone_unbondings
+
+
+def get_lsm_deposit_records(chain_id: str) -> List[Dict[str, Any]]:
+    """
+    Queries all the LSM deposit records
+
+    [
+        {
+            "deposit_id": "800000.cosmoshub-4.strideXXX.cosmosvaloperXXX/1",
+            "chain_id": "cosmoshub-4",
+            "ibc_denom": "ibc/cosmosvaloperXXX/1",
+            "staker_address": "strideXXX",
+            "validator_address": "cosmosvaloperXXX",
+            "amount": "10000",
+            "st_token": {
+                "amount": "10000",
+                "denom": "stuatom"
+            }
+            "status": "DEPOSIT_PENDING"
+        },
+    ]
+    """
+    params = {"chain_id": chain_id}
+    url = f"{config.stride.api_endpoint}/{LSM_RECORDS_QUERY}"
+    deposit_records = request(url, params=params)["deposits"]
+    return deposit_records
+
+
 def get_multisig_delegation_records(module: str, include_archived: bool = False) -> List[Dict]:
     """
     Queries the delegation records from staketia or stakedym
     Optionally include archive records
 
     Example response:
     [
@@ -334,14 +440,84 @@
              'channel_value': '15104662663116448541290611'}}, ...]
     """
     endpoint = f"{config.stride.api_endpoint}/{RATE_LIMIT_QUERY}"
     host_zone = request(endpoint, **kwargs)["rate_limits"]
     return host_zone
 
 
+def get_pending_interchain_queries(chain_id: Optional[str] = None, block_height: int = 0) -> List[Dict[str, Any]]:
+    """
+    Gets the list of all pending ICQs on stride
+
+    E.g.
+    [
+        {
+            "id": "86170fade2b01f18a1f5e448c8a9dabdc60293151828f881a40708396ec383e0",
+            "connection_id": "connection-0",
+            "chain_id": "cosmoshub-4",
+            "query_type": "store/bank/key",
+            "request_data": ...bytestring...,
+            "callback_module": "stakeibc",
+            "callback_id": "withdrawalbalance",
+            "callback_data": ...bytestring...,
+            "timeout_policy": "REJECT_QUERY_RESPONSE",
+            "timeout_duration": "1hr",
+            "timeout_timestamp": "1714689884000000000",
+            "request_sent": true,
+            "submission_height": 80000
+        }
+        ...
+    ]
+    """
+    url = f"{config.stride.api_endpoint}/{PENDING_ICQ_QUERY}"
+    queries = request(url, block_height=block_height)["pending_queries"]
+    if chain_id:
+        queries = [query for query in queries if query["chain_id"] == chain_id]
+    return queries
+
+
+def get_callback_data(
+    chain_id: Optional[str] = None,
+    channel_id: Optional[str] = None,
+    port_id: Optional[str] = None,
+    callback_id: Optional[str] = None,
+    block_height: int = 0,
+) -> List[Dict[str, Any]]:
+    """
+    Gets all the ica or ibc callback data stored on stride, with optional filters
+
+    E.g.
+    [
+        {
+            "callback_key": "icacontroller-cosmoshub-4.DELEGATION.channel-1.23",
+            "port_id": "icacontroller-cosmoshub-4.DELEGATION",
+            "channel_id": "channel-1",
+            "sequence": "23",
+            "callback_id": "delegate",
+            "callback_args": "...bytestring..."
+        }
+    ]
+    """
+    url = f"{config.stride.api_endpoint}/{CALLBACK_DATA_QUERY}"
+    callback_data = query_list_with_pagination(url, rel_key="callback_data", block_height=block_height)
+
+    filtered_callback_data = []
+    for data in callback_data:
+
+        chain_id_match = not chain_id or chain_id in data["port_id"]
+        channel_id_match = not channel_id or data["channel_id"] == channel_id
+        port_id_match = not port_id or data["port_id"] == port_id
+        callback_id_match = not callback_id or data["callback_id"] == callback_id
+
+        if all([chain_id_match, channel_id_match, port_id_match, callback_id_match]):
+            filtered_callback_data.append(data)
+
+    return filtered_callback_data
+
+
 def get_validators(api_endpoint: str = config.stride.api_endpoint) -> List[Dict[str, Any]]:
     """
     Queries the list of validators from a chain
     """
     url = f"{api_endpoint}/{VALIDATORS_QUERY}"
     return query_list_with_pagination(url, rel_key="validators")
 
@@ -786,25 +962,132 @@
     }
     """
     url = f"{config.stride.api_endpoint}/{EPOCHS_QUERY}"
     epochs = request(url)
     return epochs["epochs"]
 
 
-def get_day_epoch() -> int:
+def get_day_epoch() -> Dict[str, Any]:
     """
-    Get the day epoch from the stride-labs/stride/epochs endpoint
+    Returns the "day" epoch struct on Stride
+
+    E.g.
+    {
+        "identifier": "day",
+        "start_time": "2022-09-04T19:00:00.451745Z",
+        "duration": "86400s",
+        "current_epoch": "607",
+        "current_epoch_start_time": "2024-05-02T19:00:00.451745Z",
+        "epoch_counting_started": true,
+        "current_epoch_start_height": "8829138"
+    }
     """
-    epochs_request = f"{config.stride.api_endpoint}/Stridelabs/stride/epochs"
-    epochs = request(epochs_request)["epochs"]
-    epochs_df = pd.DataFrame(epochs)
-    day_epoch = int(epochs_df[epochs_df["identifier"] == "day"]["current_epoch"].values[0])
+    epochs = get_epochs()
+    day_epoch = [epoch for epoch in epochs if epoch["identifier"] == "day"][0]
     return day_epoch
 
 
+def get_stride_epoch() -> Dict[str, Any]:
+    """
+    Returns the "stride" epoch struct on stride
+
+    E.g.
+    {
+        "identifier": "stride_epoch",
+        "start_time": "2022-09-04T19:00:00.451745Z",
+        "duration": "21600s",
+        "current_epoch": "2425",
+        "current_epoch_start_time": "2024-05-02T19:00:00.451745Z",
+        "epoch_counting_started": true,
+        "current_epoch_start_height": "8829138"
+    }
+    """
+    epochs = get_epochs()
+    stride_epoch = [epoch for epoch in epochs if epoch["identifier"] == "stride_epoch"][0]
+    return stride_epoch
+
+
+def get_stride_epoch_number() -> int:
+    """
+    Returns the epoch number for the current "stride" epoch
+    """
+    stride_epoch = get_stride_epoch()
+    return int(stride_epoch["current_epoch"])
+
+
+def get_day_epoch_number() -> int:
+    """
+    Returns the epoch number for the current "day" epoch
+    """
+    day_epoch = get_day_epoch()
+    return int(day_epoch["current_epoch"])
+
+
+def get_stride_epoch_start_time() -> datetime.datetime:
+    """
+    Returns the epoch start time for the current "stride" epoch
+    """
+    stride_epoch = get_stride_epoch()
+    return dateutil.parser.parse(stride_epoch["current_epoch_start_time"]).replace(tzinfo=None)
+
+
+def get_day_epoch_start_time() -> datetime.datetime:
+    """
+    Returns the epoch start time for the current "day" epoch
+    """
+    day_epoch = get_day_epoch()
+    return dateutil.parser.parse(day_epoch["current_epoch_start_time"]).replace(tzinfo=None)
+
+
+def get_stride_epoch_start_height() -> int:
+    """
+    Returns the epoch start time for the current "stride" epoch
+    """
+    stride_epoch = get_stride_epoch()
+    return int(stride_epoch["current_epoch_start_height"])
+
+
+def get_day_epoch_start_height() -> int:
+    """
+    Returns the epoch start time for the current "day" epoch
+    """
+    day_epoch = get_day_epoch()
+    return int(day_epoch["current_epoch_start_height"])
+
+
+def get_host_zone_channels(chain_id: str) -> Dict[str, Any]:
+    """
+    Returns the JSON response from the channels endpoint, which holds the client and connection info,
+    as well as all the ICA channels
+
+    E.g.
+    {
+        "chain_id": "cosmoshub-4",
+        "client_id": "07-tendermint-0",
+        "counterparty_client_id": "07-tendermint-913",
+        "connection_id": "connection-0",
+        "counterparty_connection_id": "connection-635",
+        "transfer_channel_id": "channel-0",
+        "counterparty_transfer_channel_id": "channel-391",
+        "ica_channels": [
+            {
+            "type": "DELEGATION",
+            "port_id": "icacontroller-cosmoshub-4.DELEGATION",
+            "channel_id": "channel-203",
+            "counterparty_channel_id": "channel-810",
+            "state": "STATE_OPEN",
+            "counterparty_state": "STATE_OPEN"
+            },
+        ...
+        ]
+    }
+    """
+    return request(HOST_CHANNELS_QUERY.format(chain_id=chain_id))
+
+
 def query_wasm_contract(contract_address: str, query_msg: Dict, api_endpoint: str, block_height: int = 0) -> Dict:
     """
     Queries a cosmowasm contract address with the provided query message
     Response structure is dependent on the particular query
     """
     query_msg_string = json.dumps(query_msg)
     query_msg_encoded = base64.b64encode(query_msg_string.encode("utf-8")).decode("utf-8")
```

### Comparing `strideutils-0.3.3/strideutils/stride_upstash.py` & `strideutils-0.3.4/strideutils/stride_upstash.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.3/strideutils/twilio_connector.py` & `strideutils-0.3.4/strideutils/twilio_connector.py`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.3/strideutils-stubs/sheets_connector.pyi` & `strideutils-0.3.4/strideutils-stubs/sheets_connector.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.3/strideutils-stubs/stride_alerts.pyi` & `strideutils-0.3.4/strideutils-stubs/stride_alerts.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.3/strideutils-stubs/stride_config.pyi` & `strideutils-0.3.4/strideutils-stubs/stride_config.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.3/strideutils-stubs/stride_requests.pyi` & `strideutils-0.3.4/strideutils-stubs/stride_requests.pyi`

 * *Files identical despite different names*

### Comparing `strideutils-0.3.3/PKG-INFO` & `strideutils-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strideutils
-Version: 0.3.3
+Version: 0.3.4
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

