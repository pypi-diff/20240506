# Comparing `tmp/orbs_orderbook_sdk-0.9.1.tar.gz` & `tmp/orbs_orderbook_sdk-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbs_orderbook_sdk-0.9.1.tar", max compression
+gzip compressed data, was "orbs_orderbook_sdk-0.9.2.tar", max compression
```

## Comparing `orbs_orderbook_sdk-0.9.1.tar` & `orbs_orderbook_sdk-0.9.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1175 2024-02-15 13:55:11.199500 orbs_orderbook_sdk-0.9.1/README.md
--rw-r--r--   0        0        0      113 2024-02-15 13:55:11.199500 orbs_orderbook_sdk-0.9.1/orbs_orderbook/__init__.py
--rw-r--r--   0        0        0     4634 2024-02-15 13:55:11.199500 orbs_orderbook_sdk-0.9.1/orbs_orderbook/client.py
--rw-r--r--   0        0        0      799 2024-02-15 13:55:11.199500 orbs_orderbook_sdk-0.9.1/orbs_orderbook/exceptions.py
--rw-r--r--   0        0        0     8705 2024-02-15 13:55:11.199500 orbs_orderbook_sdk-0.9.1/orbs_orderbook/order_signer.py
--rw-r--r--   0        0        0     1077 2024-02-15 13:55:11.199500 orbs_orderbook_sdk-0.9.1/orbs_orderbook/signer.py
--rw-r--r--   0        0        0     2083 2024-02-15 13:55:11.199500 orbs_orderbook_sdk-0.9.1/orbs_orderbook/types.py
--rw-r--r--   0        0        0      769 2024-02-15 13:55:11.199500 orbs_orderbook_sdk-0.9.1/orbs_orderbook/utils.py
--rw-r--r--   0        0        0      578 2024-02-15 13:55:11.199500 orbs_orderbook_sdk-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1878 1970-01-01 00:00:00.000000 orbs_orderbook_sdk-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1175 2024-02-22 09:32:12.219256 orbs_orderbook_sdk-0.9.2/README.md
+-rw-r--r--   0        0        0      113 2024-02-22 09:32:12.219256 orbs_orderbook_sdk-0.9.2/orbs_orderbook/__init__.py
+-rw-r--r--   0        0        0     4634 2024-02-22 09:32:12.219256 orbs_orderbook_sdk-0.9.2/orbs_orderbook/client.py
+-rw-r--r--   0        0        0      799 2024-02-22 09:32:12.223255 orbs_orderbook_sdk-0.9.2/orbs_orderbook/exceptions.py
+-rw-r--r--   0        0        0     8779 2024-02-22 09:32:12.223255 orbs_orderbook_sdk-0.9.2/orbs_orderbook/order_signer.py
+-rw-r--r--   0        0        0     1077 2024-02-22 09:32:12.223255 orbs_orderbook_sdk-0.9.2/orbs_orderbook/signer.py
+-rw-r--r--   0        0        0     2083 2024-02-22 09:32:12.223255 orbs_orderbook_sdk-0.9.2/orbs_orderbook/types.py
+-rw-r--r--   0        0        0      769 2024-02-22 09:32:12.223255 orbs_orderbook_sdk-0.9.2/orbs_orderbook/utils.py
+-rw-r--r--   0        0        0      578 2024-02-22 09:32:12.223255 orbs_orderbook_sdk-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     1878 1970-01-01 00:00:00.000000 orbs_orderbook_sdk-0.9.2/PKG-INFO
```

### Comparing `orbs_orderbook_sdk-0.9.1/README.md` & `orbs_orderbook_sdk-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `orbs_orderbook_sdk-0.9.1/orbs_orderbook/client.py` & `orbs_orderbook_sdk-0.9.2/orbs_orderbook/client.py`

 * *Files identical despite different names*

### Comparing `orbs_orderbook_sdk-0.9.1/orbs_orderbook/exceptions.py` & `orbs_orderbook_sdk-0.9.2/orbs_orderbook/exceptions.py`

 * *Files identical despite different names*

### Comparing `orbs_orderbook_sdk-0.9.1/orbs_orderbook/order_signer.py` & `orbs_orderbook_sdk-0.9.2/orbs_orderbook/order_signer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 from datetime import datetime, timedelta
 from decimal import Decimal
-from typing import Any, Dict, Tuple
+from typing import Any, Dict, Optional, Tuple
 
 from eth_account import Account
 
 from orbs_orderbook.client import OrderBookSDK
 from orbs_orderbook.exceptions import (
     ErrDecimalPlaces,
     ErrInvalidSide,
@@ -26,15 +26,15 @@
 
         self.__account = Account.from_key(private_key)
         self.__sdk = sdk
 
     def prepare_and_sign_order(
         self,
         order: CreateOrderInput,
-        deadline: datetime = datetime.now() + timedelta(days=1),
+        deadline: Optional[datetime] = None,
     ) -> (str, dict):
         """Prepare EIP-712 message and sign it.
 
         Args:
             order: Order to sign.
             deadline (optional): How long the order signature is valid for.
 
@@ -42,14 +42,17 @@
             Tuple of signature and EIP712 message data (needed for signature validation)
 
         Raises:
             - ErrInvalidSymbolFormat: Raised when symbol does not follow "TOKEN1-TOKEN2" format
             - ErrInvalidSide: Raised when side is not "buy" or "sell"
             - ErrInvalidToken: Raised when token is not supported
         """
+        if not deadline:
+            deadline = datetime.now() + timedelta(days=1)
+
         in_token, out_token = self.__get_token_details(
             symbol=order.symbol, side=order.side
         )
 
         domain_data = self._construct_domain_data()
         message_types = self._construct_message_types()
         message_data = self._construct_message_data(
```

### Comparing `orbs_orderbook_sdk-0.9.1/orbs_orderbook/signer.py` & `orbs_orderbook_sdk-0.9.2/orbs_orderbook/signer.py`

 * *Files identical despite different names*

### Comparing `orbs_orderbook_sdk-0.9.1/orbs_orderbook/types.py` & `orbs_orderbook_sdk-0.9.2/orbs_orderbook/types.py`

 * *Files identical despite different names*

### Comparing `orbs_orderbook_sdk-0.9.1/orbs_orderbook/utils.py` & `orbs_orderbook_sdk-0.9.2/orbs_orderbook/utils.py`

 * *Files identical despite different names*

### Comparing `orbs_orderbook_sdk-0.9.1/pyproject.toml` & `orbs_orderbook_sdk-0.9.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbs-orderbook-sdk"
-version = "0.9.1"
+version = "0.9.2"
 description = "Python SDK for the Orbs order book"
 authors = ["Luke Rogerson <contact@lukerogerson.me>"]
 readme = "README.md"
 packages = [
     { include = "orbs_orderbook" },
 ]
 include = ["orbs_orderbook/supportedTokens.json"]
```

### Comparing `orbs_orderbook_sdk-0.9.1/PKG-INFO` & `orbs_orderbook_sdk-0.9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbs-orderbook-sdk
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python SDK for the Orbs order book
 Author: Luke Rogerson
 Author-email: contact@lukerogerson.me
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

