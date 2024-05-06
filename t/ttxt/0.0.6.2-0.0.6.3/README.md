# Comparing `tmp/ttxt-0.0.6.2.tar.gz` & `tmp/ttxt-0.0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttxt-0.0.6.2.tar", last modified: Fri May  3 15:41:14 2024, max compression
+gzip compressed data, was "ttxt-0.0.6.3.tar", last modified: Mon May  6 12:01:40 2024, max compression
```

## Comparing `ttxt-0.0.6.2.tar` & `ttxt-0.0.6.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-03 15:41:14.864548 ttxt-0.0.6.2/
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11357 2023-11-29 00:08:24.000000 ttxt-0.0.6.2/LICENSE
--rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-05-03 15:41:14.864437 ttxt-0.0.6.2/PKG-INFO
--rw-r--r--   0 sushantkumar   (501) staff       (20)       58 2023-11-29 00:08:24.000000 ttxt-0.0.6.2/README.md
--rw-r--r--   0 sushantkumar   (501) staff       (20)       38 2024-05-03 15:41:14.864600 ttxt-0.0.6.2/setup.cfg
--rw-r--r--   0 sushantkumar   (501) staff       (20)      306 2024-05-03 15:40:39.000000 ttxt-0.0.6.2/setup.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-03 15:41:14.854431 ttxt-0.0.6.2/ttxt/
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1101 2024-05-03 15:38:46.000000 ttxt-0.0.6.2/ttxt/__init__.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-03 15:41:14.855608 ttxt-0.0.6.2/ttxt/base/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:39:15.000000 ttxt-0.0.6.2/ttxt/base/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1394 2024-01-23 17:20:28.000000 ttxt-0.0.6.2/ttxt/base/baseFuturesExchange.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1224 2024-03-14 09:27:50.000000 ttxt-0.0.6.2/ttxt/base/baseSpotExchange.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-03 15:41:14.862036 ttxt-0.0.6.2/ttxt/exchanges/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:36:21.000000 ttxt-0.0.6.2/ttxt/exchanges/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11341 2024-05-03 15:38:46.000000 ttxt-0.0.6.2/ttxt/exchanges/ascendex.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    13324 2023-12-21 12:03:19.000000 ttxt-0.0.6.2/ttxt/exchanges/biconomy.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     9966 2024-03-22 17:14:03.000000 ttxt-0.0.6.2/ttxt/exchanges/binance.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    13165 2024-03-22 17:15:32.000000 ttxt-0.0.6.2/ttxt/exchanges/bingx.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    12850 2024-03-22 17:15:07.000000 ttxt-0.0.6.2/ttxt/exchanges/bitget.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    10504 2024-01-26 15:22:11.000000 ttxt-0.0.6.2/ttxt/exchanges/bitgetFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    12255 2024-03-22 17:15:48.000000 ttxt-0.0.6.2/ttxt/exchanges/bitmart.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    21199 2024-05-02 08:57:55.000000 ttxt-0.0.6.2/ttxt/exchanges/bybit.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    17967 2024-01-23 17:20:48.000000 ttxt-0.0.6.2/ttxt/exchanges/bybitFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11712 2024-03-22 17:16:03.000000 ttxt-0.0.6.2/ttxt/exchanges/cryptocom.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    14163 2024-03-11 15:19:34.000000 ttxt-0.0.6.2/ttxt/exchanges/gateFutures.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    15302 2024-03-22 17:13:33.000000 ttxt-0.0.6.2/ttxt/exchanges/gateio.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    14560 2024-03-29 07:17:38.000000 ttxt-0.0.6.2/ttxt/exchanges/huobi.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11284 2024-03-22 17:12:44.000000 ttxt-0.0.6.2/ttxt/exchanges/kucoin.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11671 2024-03-22 17:16:57.000000 ttxt-0.0.6.2/ttxt/exchanges/mexc.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    11747 2024-04-05 05:36:24.000000 ttxt-0.0.6.2/ttxt/exchanges/okx.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-19 13:51:46.000000 ttxt-0.0.6.2/ttxt/exchanges/xt.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-03 15:41:14.862211 ttxt-0.0.6.2/ttxt/tests/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:02:46.000000 ttxt-0.0.6.2/ttxt/tests/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    10231 2024-05-03 15:38:46.000000 ttxt-0.0.6.2/ttxt/tests/testExchange.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-03 15:41:14.862534 ttxt-0.0.6.2/ttxt/types/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:42:34.000000 ttxt-0.0.6.2/ttxt/types/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)     1428 2023-12-28 02:37:11.000000 ttxt-0.0.6.2/ttxt/types/baseTypes.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-03 15:41:14.863424 ttxt-0.0.6.2/ttxt/utils/
--rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-20 23:39:43.000000 ttxt-0.0.6.2/ttxt/utils/__init__.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)      778 2024-03-11 15:19:34.000000 ttxt-0.0.6.2/ttxt/utils/general.py
--rw-r--r--   0 sushantkumar   (501) staff       (20)    42572 2023-12-20 23:39:43.000000 ttxt-0.0.6.2/ttxt/utils/xtUtils.py
-drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-03 15:41:14.855051 ttxt-0.0.6.2/ttxt.egg-info/
--rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-05-03 15:41:14.000000 ttxt-0.0.6.2/ttxt.egg-info/PKG-INFO
--rw-r--r--   0 sushantkumar   (501) staff       (20)      871 2024-05-03 15:41:14.000000 ttxt-0.0.6.2/ttxt.egg-info/SOURCES.txt
--rw-r--r--   0 sushantkumar   (501) staff       (20)        1 2024-05-03 15:41:14.000000 ttxt-0.0.6.2/ttxt.egg-info/dependency_links.txt
--rw-r--r--   0 sushantkumar   (501) staff       (20)        5 2024-05-03 15:41:14.000000 ttxt-0.0.6.2/ttxt.egg-info/top_level.txt
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-06 12:01:40.535079 ttxt-0.0.6.3/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11357 2023-11-29 00:08:24.000000 ttxt-0.0.6.3/LICENSE
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-05-06 12:01:40.534940 ttxt-0.0.6.3/PKG-INFO
+-rw-r--r--   0 sushantkumar   (501) staff       (20)       58 2023-11-29 00:08:24.000000 ttxt-0.0.6.3/README.md
+-rw-r--r--   0 sushantkumar   (501) staff       (20)       38 2024-05-06 12:01:40.535126 ttxt-0.0.6.3/setup.cfg
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      306 2024-05-06 12:01:06.000000 ttxt-0.0.6.3/setup.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-06 12:01:40.525102 ttxt-0.0.6.3/ttxt/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1101 2024-05-03 15:38:46.000000 ttxt-0.0.6.3/ttxt/__init__.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-06 12:01:40.526344 ttxt-0.0.6.3/ttxt/base/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:39:15.000000 ttxt-0.0.6.3/ttxt/base/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1394 2024-01-23 17:20:28.000000 ttxt-0.0.6.3/ttxt/base/baseFuturesExchange.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1224 2024-03-14 09:27:50.000000 ttxt-0.0.6.3/ttxt/base/baseSpotExchange.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-06 12:01:40.532938 ttxt-0.0.6.3/ttxt/exchanges/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:36:21.000000 ttxt-0.0.6.3/ttxt/exchanges/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11414 2024-05-06 11:38:54.000000 ttxt-0.0.6.3/ttxt/exchanges/ascendex.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    13324 2023-12-21 12:03:19.000000 ttxt-0.0.6.3/ttxt/exchanges/biconomy.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     9966 2024-03-22 17:14:03.000000 ttxt-0.0.6.3/ttxt/exchanges/binance.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    13165 2024-03-22 17:15:32.000000 ttxt-0.0.6.3/ttxt/exchanges/bingx.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    12850 2024-03-22 17:15:07.000000 ttxt-0.0.6.3/ttxt/exchanges/bitget.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    10504 2024-01-26 15:22:11.000000 ttxt-0.0.6.3/ttxt/exchanges/bitgetFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    12255 2024-03-22 17:15:48.000000 ttxt-0.0.6.3/ttxt/exchanges/bitmart.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    21199 2024-05-02 08:57:55.000000 ttxt-0.0.6.3/ttxt/exchanges/bybit.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    17967 2024-01-23 17:20:48.000000 ttxt-0.0.6.3/ttxt/exchanges/bybitFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11712 2024-03-22 17:16:03.000000 ttxt-0.0.6.3/ttxt/exchanges/cryptocom.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    14163 2024-03-11 15:19:34.000000 ttxt-0.0.6.3/ttxt/exchanges/gateFutures.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    15302 2024-03-22 17:13:33.000000 ttxt-0.0.6.3/ttxt/exchanges/gateio.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    14560 2024-03-29 07:17:38.000000 ttxt-0.0.6.3/ttxt/exchanges/huobi.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11284 2024-03-22 17:12:44.000000 ttxt-0.0.6.3/ttxt/exchanges/kucoin.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11671 2024-03-22 17:16:57.000000 ttxt-0.0.6.3/ttxt/exchanges/mexc.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    11747 2024-04-05 05:36:24.000000 ttxt-0.0.6.3/ttxt/exchanges/okx.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-19 13:51:46.000000 ttxt-0.0.6.3/ttxt/exchanges/xt.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-06 12:01:40.533139 ttxt-0.0.6.3/ttxt/tests/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-06 13:02:46.000000 ttxt-0.0.6.3/ttxt/tests/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    10235 2024-05-06 11:25:23.000000 ttxt-0.0.6.3/ttxt/tests/testExchange.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-06 12:01:40.533566 ttxt-0.0.6.3/ttxt/types/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-13 13:42:34.000000 ttxt-0.0.6.3/ttxt/types/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)     1428 2023-12-28 02:37:11.000000 ttxt-0.0.6.3/ttxt/types/baseTypes.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-06 12:01:40.534279 ttxt-0.0.6.3/ttxt/utils/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        0 2023-12-20 23:39:43.000000 ttxt-0.0.6.3/ttxt/utils/__init__.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      778 2024-03-11 15:19:34.000000 ttxt-0.0.6.3/ttxt/utils/general.py
+-rw-r--r--   0 sushantkumar   (501) staff       (20)    42572 2023-12-20 23:39:43.000000 ttxt-0.0.6.3/ttxt/utils/xtUtils.py
+drwxr-xr-x   0 sushantkumar   (501) staff       (20)        0 2024-05-06 12:01:40.525706 ttxt-0.0.6.3/ttxt.egg-info/
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      125 2024-05-06 12:01:40.000000 ttxt-0.0.6.3/ttxt.egg-info/PKG-INFO
+-rw-r--r--   0 sushantkumar   (501) staff       (20)      871 2024-05-06 12:01:40.000000 ttxt-0.0.6.3/ttxt.egg-info/SOURCES.txt
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        1 2024-05-06 12:01:40.000000 ttxt-0.0.6.3/ttxt.egg-info/dependency_links.txt
+-rw-r--r--   0 sushantkumar   (501) staff       (20)        5 2024-05-06 12:01:40.000000 ttxt-0.0.6.3/ttxt.egg-info/top_level.txt
```

### Comparing `ttxt-0.0.6.2/LICENSE` & `ttxt-0.0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/__init__.py` & `ttxt-0.0.6.3/ttxt/__init__.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/base/baseFuturesExchange.py` & `ttxt-0.0.6.3/ttxt/base/baseFuturesExchange.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/base/baseSpotExchange.py` & `ttxt-0.0.6.3/ttxt/base/baseSpotExchange.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/exchanges/ascendex.py` & `ttxt-0.0.6.3/ttxt/exchanges/ascendex.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,15 @@
         parsedOrder["tradeId"] = order.get('orderId', None)
         parsedOrder["symbol"] = order.get('symbol', None)
         parsedOrder["price"] = float(order["price"]) if "price" in order else None 
         parsedOrder["amount"] = float(order["orderQty"]) if "orderQty" in order else None
         parsedOrder["side"] = order['side'].lower() if "side" in order else None
         parsedOrder["timestamp"] = int(order["lastExecTime"]) if "lastExecTime" in order else None
         parsedOrder["status"] = order.get("status", None)
+        parsedOrder['takerOrMaker'] = "taker" if order["orderType"] == "Market" else "maker"
         parsedOrder["orderJson"] = json.dumps(order) if order else None 
         return parsedOrder
         
     def _parseFetchOrder(self, order):
         if order['code'] != 0: raise Exception(order['message'])
         parsedOrder = {"id": None, "symbol": None, "price": None, "amount": None, "takerOrMaker": None, "datetime": None, "fee": None, "fee_currency": None,
                        "side": None, "timestamp": None, "status": None}
@@ -144,16 +145,15 @@
         
         
     def _parseFetchTrades(self, order):
         if order['code'] != 0: raise Exception(order['message'])
         parsedTradesList = []
         if "data" in order and order["data"] != []:
             for element in order['data']:
-                if element['status'] == "Filled":
-                    parsedTradesList.append(self._parseOrder(element))
+                parsedTradesList.append(self._parseOrder(element))
         return parsedTradesList
         
     ## Exchange functions
     def fetch_ticker(self, symbol):
         raise NotImplementedError("method not implemented")
     
     def fetch_balance(self, params={}) -> baseTypes.Balances:
@@ -166,15 +166,16 @@
         except Exception as e:
             raise e
     
     def fetch_my_trades(self, symbol=None, since=None, limit=None, params={}):
         apiUrl = f'{self.category}/order/hist/current'
         preHashString = "order/hist/current"
         params = {
-            "symbol": symbol
+            "symbol": symbol,
+            "executedOnly": True
         }
         if limit:
             params['n'] = limit
         try:
             resp = self._signedRequest(method="GET", request_path=apiUrl, preHashString=preHashString, params=params)
             return self._parseFetchTrades(resp)
         except Exception as e:
```

### Comparing `ttxt-0.0.6.2/ttxt/exchanges/biconomy.py` & `ttxt-0.0.6.3/ttxt/exchanges/biconomy.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/exchanges/binance.py` & `ttxt-0.0.6.3/ttxt/exchanges/binance.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/exchanges/bingx.py` & `ttxt-0.0.6.3/ttxt/exchanges/bingx.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/exchanges/bitget.py` & `ttxt-0.0.6.3/ttxt/exchanges/bitget.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/exchanges/bitgetFutures.py` & `ttxt-0.0.6.3/ttxt/exchanges/bitgetFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/exchanges/bitmart.py` & `ttxt-0.0.6.3/ttxt/exchanges/bitmart.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/exchanges/bybit.py` & `ttxt-0.0.6.3/ttxt/exchanges/bybit.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/exchanges/bybitFutures.py` & `ttxt-0.0.6.3/ttxt/exchanges/bybitFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/exchanges/cryptocom.py` & `ttxt-0.0.6.3/ttxt/exchanges/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/exchanges/gateFutures.py` & `ttxt-0.0.6.3/ttxt/exchanges/gateFutures.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/exchanges/gateio.py` & `ttxt-0.0.6.3/ttxt/exchanges/gateio.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/exchanges/huobi.py` & `ttxt-0.0.6.3/ttxt/exchanges/huobi.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/exchanges/kucoin.py` & `ttxt-0.0.6.3/ttxt/exchanges/kucoin.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/exchanges/mexc.py` & `ttxt-0.0.6.3/ttxt/exchanges/mexc.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/exchanges/okx.py` & `ttxt-0.0.6.3/ttxt/exchanges/okx.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/tests/testExchange.py` & `ttxt-0.0.6.3/ttxt/tests/testExchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             print(f"createOrder response: {resp}")
         except Exception as e:
             print("order could not be created")
             print(e)
     if "createLimitOrder" in params and params["createLimitOrder"]:
         print("testing limit create order...")
         try:
-            resp = ttxtExchange.create_limit_order(symbol=tickerToTest, amount=50, side="buy", price=0.2)
+            resp = ttxtExchange.create_limit_order(symbol=tickerToTest, amount=50, side="sell", price=0.2)
             print(f"createLimitOrder response: {resp}")
         except Exception as e:
             print("limit order could not be created")
             print(e)
     if "createMarketSellOrder" in params and params["createMarketSellOrder"]:
         print("testing market sell create order...")
         try:
@@ -113,15 +113,15 @@
             print(f"createMarketBuyOrder response: {resp}")
         except Exception as e:
             print("market buy order could not be created")
             print(e)
     if "create_market_order" in params and params["create_market_order"]:
         print("testing create market order...")
         try:
-            resp = ttxtExchange.create_market_order(symbol=tickerToTest, side="sell", amount=50)
+            resp = ttxtExchange.create_market_order(symbol=tickerToTest, side="sell", amount=100)
             print(f"create_market_order response: {resp}")
         except Exception as e:
             print("market order could not be created")
             print(e)
     if "fetchOrder" in params and params["fetchOrder"]:
         print("testing fetch order...")
         try:
@@ -222,10 +222,10 @@
                      "createLimitOrder": False,
                      "createMarketSellOrder": False, 
                      "createMarketBuyOrder": False, 
                      "orderbook": False, 
                      "candlestick": False,
                      "create_market_order": False, 
                      "cancelAllOrders": False, 
-                     "myTrades": False,
+                     "myTrades": True,
                      "accountInfo": False}
-    test(params=testingParams, exchangeName="bybit")
+    test(params=testingParams, exchangeName="ascendex")
```

### Comparing `ttxt-0.0.6.2/ttxt/types/baseTypes.py` & `ttxt-0.0.6.3/ttxt/types/baseTypes.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/utils/general.py` & `ttxt-0.0.6.3/ttxt/utils/general.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt/utils/xtUtils.py` & `ttxt-0.0.6.3/ttxt/utils/xtUtils.py`

 * *Files identical despite different names*

### Comparing `ttxt-0.0.6.2/ttxt.egg-info/SOURCES.txt` & `ttxt-0.0.6.3/ttxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

