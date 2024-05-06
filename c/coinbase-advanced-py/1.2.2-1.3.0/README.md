# Comparing `tmp/coinbase-advanced-py-1.2.2.tar.gz` & `tmp/coinbase-advanced-py-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinbase-advanced-py-1.2.2.tar", last modified: Tue Apr  9 20:55:52 2024, max compression
+gzip compressed data, was "coinbase-advanced-py-1.3.0.tar", last modified: Mon May  6 20:13:54 2024, max compression
```

## Comparing `coinbase-advanced-py-1.2.2.tar` & `coinbase-advanced-py-1.3.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-04-09 20:55:52.045608 coinbase-advanced-py-1.2.2/
--rw-r--r--   0 urischwartz   (501) staff       (20)    11343 2023-12-07 15:44:33.000000 coinbase-advanced-py-1.2.2/LICENSE.md
--rw-r--r--   0 urischwartz   (501) staff       (20)    15261 2024-04-09 20:55:52.045219 coinbase-advanced-py-1.2.2/PKG-INFO
--rw-r--r--   0 urischwartz   (501) staff       (20)    14147 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/README.md
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-04-09 20:55:52.027150 coinbase-advanced-py-1.2.2/coinbase/
--rw-r--r--   0 urischwartz   (501) staff       (20)        0 2023-11-21 15:58:27.000000 coinbase-advanced-py-1.2.2/coinbase/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)       22 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.2.2/coinbase/__version__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1986 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/coinbase/api_base.py
--rw-r--r--   0 urischwartz   (501) staff       (20)      746 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/coinbase/constants.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2350 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.2.2/coinbase/jwt_generator.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-04-09 20:55:52.032262 coinbase-advanced-py-1.2.2/coinbase/rest/
--rwxr-xr-x   0 urischwartz   (501) staff       (20)     2514 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.2.2/coinbase/rest/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1331 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/coinbase/rest/accounts.py
--rw-r--r--   0 urischwartz   (501) staff       (20)      641 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.2.2/coinbase/rest/common.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2974 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/coinbase/rest/convert.py
--rw-r--r--   0 urischwartz   (501) staff       (20)      927 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/coinbase/rest/fees.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     4806 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.2.2/coinbase/rest/futures.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1684 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/coinbase/rest/market_data.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    59432 2024-03-27 20:36:13.000000 coinbase-advanced-py-1.2.2/coinbase/rest/orders.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1280 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.2.2/coinbase/rest/payments.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2866 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/coinbase/rest/perpetuals.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     4125 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/coinbase/rest/portfolios.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     3223 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/coinbase/rest/products.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     6913 2024-03-27 20:36:13.000000 coinbase-advanced-py-1.2.2/coinbase/rest/rest_base.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-04-09 20:55:52.033390 coinbase-advanced-py-1.2.2/coinbase/websocket/
--rw-r--r--   0 urischwartz   (501) staff       (20)     1013 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/coinbase/websocket/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    15436 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.2.2/coinbase/websocket/channels.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    19199 2024-03-27 20:36:13.000000 coinbase-advanced-py-1.2.2/coinbase/websocket/websocket_base.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-04-09 20:55:52.035090 coinbase-advanced-py-1.2.2/coinbase_advanced_py.egg-info/
--rw-r--r--   0 urischwartz   (501) staff       (20)    15261 2024-04-09 20:55:51.000000 coinbase-advanced-py-1.2.2/coinbase_advanced_py.egg-info/PKG-INFO
--rw-r--r--   0 urischwartz   (501) staff       (20)     1339 2024-04-09 20:55:51.000000 coinbase-advanced-py-1.2.2/coinbase_advanced_py.egg-info/SOURCES.txt
--rw-r--r--   0 urischwartz   (501) staff       (20)        1 2024-04-09 20:55:51.000000 coinbase-advanced-py-1.2.2/coinbase_advanced_py.egg-info/dependency_links.txt
--rw-r--r--   0 urischwartz   (501) staff       (20)      167 2024-04-09 20:55:51.000000 coinbase-advanced-py-1.2.2/coinbase_advanced_py.egg-info/requires.txt
--rw-r--r--   0 urischwartz   (501) staff       (20)       15 2024-04-09 20:55:51.000000 coinbase-advanced-py-1.2.2/coinbase_advanced_py.egg-info/top_level.txt
--rw-r--r--   0 urischwartz   (501) staff       (20)       38 2024-04-09 20:55:52.045689 coinbase-advanced-py-1.2.2/setup.cfg
--rw-r--r--   0 urischwartz   (501) staff       (20)     1642 2024-02-12 19:40:21.000000 coinbase-advanced-py-1.2.2/setup.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-04-09 20:55:52.035706 coinbase-advanced-py-1.2.2/tests/
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-04-09 20:55:52.042138 coinbase-advanced-py-1.2.2/tests/rest/
--rw-r--r--   0 urischwartz   (501) staff       (20)        0 2023-12-18 21:35:16.000000 coinbase-advanced-py-1.2.2/tests/rest/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1389 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/rest/test_accounts.py
--rw-r--r--   0 urischwartz   (501) staff       (20)      872 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.2.2/tests/rest/test_common.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2924 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/rest/test_convert.py
--rw-r--r--   0 urischwartz   (501) staff       (20)      968 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/rest/test_fees.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     5011 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.2.2/tests/rest/test_futures.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1711 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/rest/test_market_data.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    54821 2024-03-27 20:36:13.000000 coinbase-advanced-py-1.2.2/tests/rest/test_orders.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1392 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.2.2/tests/rest/test_payments.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     3268 2024-02-01 19:31:57.000000 coinbase-advanced-py-1.2.2/tests/rest/test_perpetuals.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     4429 2024-01-29 17:15:12.000000 coinbase-advanced-py-1.2.2/tests/rest/test_portfolios.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2701 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/rest/test_products.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     6970 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.2.2/tests/rest/test_rest_base.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1936 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/test_api_base.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     1749 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.2.2/tests/test_jwt_generator.py
-drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-04-09 20:55:52.043764 coinbase-advanced-py-1.2.2/tests/websocket/
--rw-r--r--   0 urischwartz   (501) staff       (20)        0 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/websocket/__init__.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     2217 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/websocket/mock_ws_server.py
--rw-r--r--   0 urischwartz   (501) staff       (20)     6651 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/websocket/test_channels.py
--rw-r--r--   0 urischwartz   (501) staff       (20)    13978 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.2.2/tests/websocket/test_websocket_base.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-06 20:13:54.203229 coinbase-advanced-py-1.3.0/
+-rw-r--r--   0 urischwartz   (501) staff       (20)    11343 2023-12-07 15:44:33.000000 coinbase-advanced-py-1.3.0/LICENSE.md
+-rw-r--r--   0 urischwartz   (501) staff       (20)    17508 2024-05-06 20:13:54.202543 coinbase-advanced-py-1.3.0/PKG-INFO
+-rw-r--r--   0 urischwartz   (501) staff       (20)    16394 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/README.md
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-06 20:13:54.188504 coinbase-advanced-py-1.3.0/coinbase/
+-rw-r--r--   0 urischwartz   (501) staff       (20)        0 2023-11-21 15:58:27.000000 coinbase-advanced-py-1.3.0/coinbase/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)       22 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/__version__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2169 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/api_base.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)      773 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/constants.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2350 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.3.0/coinbase/jwt_generator.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-06 20:13:54.192585 coinbase-advanced-py-1.3.0/coinbase/rest/
+-rwxr-xr-x   0 urischwartz   (501) staff       (20)     3379 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/rest/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1466 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/rest/accounts.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2974 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.3.0/coinbase/rest/convert.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)      927 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.3.0/coinbase/rest/fees.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     4806 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.3.0/coinbase/rest/futures.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1684 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.3.0/coinbase/rest/market_data.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    85326 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/rest/orders.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1280 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.3.0/coinbase/rest/payments.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2866 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.3.0/coinbase/rest/perpetuals.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     4125 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.3.0/coinbase/rest/portfolios.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     3223 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.3.0/coinbase/rest/products.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     5457 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/rest/public.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     7258 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/rest/rest_base.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-06 20:13:54.193395 coinbase-advanced-py-1.3.0/coinbase/websocket/
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1013 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.3.0/coinbase/websocket/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    15436 2024-02-13 19:51:12.000000 coinbase-advanced-py-1.3.0/coinbase/websocket/channels.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    20143 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/coinbase/websocket/websocket_base.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-06 20:13:54.195039 coinbase-advanced-py-1.3.0/coinbase_advanced_py.egg-info/
+-rw-r--r--   0 urischwartz   (501) staff       (20)    17508 2024-05-06 20:13:54.000000 coinbase-advanced-py-1.3.0/coinbase_advanced_py.egg-info/PKG-INFO
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1339 2024-05-06 20:13:54.000000 coinbase-advanced-py-1.3.0/coinbase_advanced_py.egg-info/SOURCES.txt
+-rw-r--r--   0 urischwartz   (501) staff       (20)        1 2024-05-06 20:13:54.000000 coinbase-advanced-py-1.3.0/coinbase_advanced_py.egg-info/dependency_links.txt
+-rw-r--r--   0 urischwartz   (501) staff       (20)      167 2024-05-06 20:13:54.000000 coinbase-advanced-py-1.3.0/coinbase_advanced_py.egg-info/requires.txt
+-rw-r--r--   0 urischwartz   (501) staff       (20)       15 2024-05-06 20:13:54.000000 coinbase-advanced-py-1.3.0/coinbase_advanced_py.egg-info/top_level.txt
+-rw-r--r--   0 urischwartz   (501) staff       (20)       38 2024-05-06 20:13:54.203355 coinbase-advanced-py-1.3.0/setup.cfg
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1642 2024-02-12 19:40:21.000000 coinbase-advanced-py-1.3.0/setup.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-06 20:13:54.195575 coinbase-advanced-py-1.3.0/tests/
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-06 20:13:54.199953 coinbase-advanced-py-1.3.0/tests/rest/
+-rw-r--r--   0 urischwartz   (501) staff       (20)        0 2023-12-18 21:35:16.000000 coinbase-advanced-py-1.3.0/tests/rest/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1531 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/tests/rest/test_accounts.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2924 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.3.0/tests/rest/test_convert.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)      968 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.3.0/tests/rest/test_fees.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     5011 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.3.0/tests/rest/test_futures.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1711 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.3.0/tests/rest/test_market_data.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    77962 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/tests/rest/test_orders.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1392 2024-03-11 21:21:56.000000 coinbase-advanced-py-1.3.0/tests/rest/test_payments.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     3268 2024-02-01 19:31:57.000000 coinbase-advanced-py-1.3.0/tests/rest/test_perpetuals.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     4429 2024-01-29 17:15:12.000000 coinbase-advanced-py-1.3.0/tests/rest/test_portfolios.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2701 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.3.0/tests/rest/test_products.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     5600 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/tests/rest/test_public.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     7860 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/tests/rest/test_rest_base.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1860 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/tests/test_api_base.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     1749 2024-04-09 20:54:48.000000 coinbase-advanced-py-1.3.0/tests/test_jwt_generator.py
+drwxr-xr-x   0 urischwartz   (501) staff       (20)        0 2024-05-06 20:13:54.201259 coinbase-advanced-py-1.3.0/tests/websocket/
+-rw-r--r--   0 urischwartz   (501) staff       (20)        0 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.3.0/tests/websocket/__init__.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     2217 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.3.0/tests/websocket/mock_ws_server.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)     6651 2024-01-31 15:37:49.000000 coinbase-advanced-py-1.3.0/tests/websocket/test_channels.py
+-rw-r--r--   0 urischwartz   (501) staff       (20)    20856 2024-05-06 20:12:47.000000 coinbase-advanced-py-1.3.0/tests/websocket/test_websocket_base.py
```

### Comparing `coinbase-advanced-py-1.2.2/LICENSE.md` & `coinbase-advanced-py-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/PKG-INFO` & `coinbase-advanced-py-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinbase-advanced-py
-Version: 1.2.2
+Version: 1.3.0
 Summary: Coinbase Advanced API Python SDK
 Home-page: https://github.com/coinbase/coinbase-advanced-py
 Author: Coinbase
 License: Apache 2.0
 Keywords: Coinbase,Advanced Trade,API,Advanced API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -34,33 +34,36 @@
 [![Code Style](https://img.shields.io/badge/code_style-black-black)](https://black.readthedocs.io/en/stable/)
 
 Welcome to the official Coinbase Advanced API Python SDK. This python project was created to allow coders to easily plug into the [Coinbase Advanced API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/welcome).
 This SDK also supports easy connection to the [Coinbase Advanced Trade WebSocket API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview).
 
 For thorough documentation of all available functions, refer to the following link: https://coinbase.github.io/coinbase-advanced-py
 
+___
 ## Installation
 
 ```bash
 pip3 install coinbase-advanced-py
 ```
 
-## Cloud API Keys
+___
+## Coinbase Developer Platform (CDP) API Keys
 
-This SDK uses the Coinbase Cloud API keys. To use this SDK, you will need to create a Coinbase Cloud API key and secret by following the instructions [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/auth#cloud-api-keys).
+This SDK uses Cloud Developer Platform (CDP) API keys. To use this SDK, you will need to create a CDP API key and secret by following the instructions [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/auth#cloud-api-keys).
 Make sure to save your API key and secret in a safe place. You will not be able to retrieve your secret again.
 
 WARNING: We do not recommend that you save your API secrets directly in your code outside of testing purposes. Best practice is to use a secrets manager and access your secrets that way. You should be careful about exposing your secrets publicly if posting code that leverages this library.
 
 Optional: Set your API key and secret in your environment (make sure to put these in quotation marks). For example:
 ```bash
 export COINBASE_API_KEY="organizations/{org_id}/apiKeys/{key_id}"
 export COINBASE_API_SECRET="-----BEGIN EC PRIVATE KEY-----\nYOUR PRIVATE KEY\n-----END EC PRIVATE KEY-----\n"
 ```
 
+___
 ## REST API Client
 In your code, import the RESTClient class and instantiate it:
 ```python
 from coinbase.rest import RESTClient
 
 client = RESTClient() # Uses environment variables for API key and secret
 ```
@@ -125,14 +128,15 @@
 Once again, the built-in way to query these through the SDK would be:
 ```python
 market_trades = client.get_market_trades(product_id="BTC-USD", limit=5)
 
 portfolio = client.create_portfolio(name="TestPortfolio")
 ```
 
+___
 ## WebSocket API Client
 We offer a WebSocket API client that allows you to connect to the [Coinbase Advanced Trade WebSocket API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview).
 Refer to the [Advanced Trade WebSocket Channels](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels) page for detailed information on each offered channel.
 
 In your code, import the WSClient class and instantiate it. The WSClient requires an API key and secret to be passed in as arguments. You can also use a key file or environment variables as described in the RESTClient instructions above.
 
 You must specify an `on_message` function that will be called when a message is received from the WebSocket API. This function must take in a single argument, which will be the raw message received from the WebSocket API. For example:
@@ -250,26 +254,28 @@
 ```
 
 ### Async WebSocket Client
 The functions described above handle the asynchronous nature of WebSocket connections for you. However, if you wish to handle this yourself, you can use the `async_open`, `async_subscribe`, `async_unsubscribe`, and `async_close` methods.
 
 We similarly provide async channel specific methods for subscribing and unsubscribing such as `ticker_async`, `ticker_unsubscribe_async`, etc.
 
+___
 ## Debugging the Clients
 You can enable debug logging for the REST and WebSocket clients by setting the `verbose` variable to `True` when initializing the clients. This will log useful information throughout the lifecycle of the REST request or WebSocket connection, and is highly recommended for debugging purposes.
 ```python
 rest_client = RESTClient(api_key=api_key, api_secret=api_secret, verbose=True)
 
 ws_client = WSClient(api_key=api_key, api_secret=api_secret, on_message=on_message, verbose=True)
 ```
 
+___
 ## Authentication
-Authentication of Cloud API Keys is handled automatically by the SDK when making a REST request or sending a WebSocket message.
+Authentication of CDP API Keys is handled automatically by the SDK when making a REST request or sending a WebSocket message.
 
-However, if you wish to handle this yourself, you must create a JWT token and attach it to your request as detailed in the Cloud API docs [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/rest-api-auth#making-requests). Use the built in `jwt_generator` to create your JWT token. For example:
+However, if you wish to handle this yourself, you must create a JWT token and attach it to your request as detailed in the API docs [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/rest-api-auth#making-requests). Use the built in `jwt_generator` to create your JWT token. For example:
 ```python
 from coinbase import jwt_generator
 
 api_key = "organizations/{org_id}/apiKeys/{key_id}"
 api_secret = "-----BEGIN EC PRIVATE KEY-----\nYOUR PRIVATE KEY\n-----END EC PRIVATE KEY-----\n"
 
 uri = "/api/v3/brokerage/orders"
@@ -289,15 +295,79 @@
 api_key = "organizations/{org_id}/apiKeys/{key_id}"
 api_secret = "-----BEGIN EC PRIVATE KEY-----\nYOUR PRIVATE KEY\n-----END EC PRIVATE KEY-----\n"
 
 jwt = jwt_generator.build_ws_jwt(api_key, api_secret)
 ```
 Use this JWT to connect to the Websocket API by setting it in the "jwt" field of your subscription requests. See the docs [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview#sending-messages-using-cloud-api-keys) for more details.
 
+___
+## Accessing public endpoints without authentication
+
+Both clients contain public endpoints which can be accessed without authentication. 
+
+To do so, simply initialize the clients without providing any API keys as arguments. 
+
+**_Notes:_**
+
+- Making calls to private endpoints or channels while unauthenticated will return an error
+- Unauthenticated requests are rate-limited more aggressively. Because of this we recommend that you authenticate your requests
+
+### REST Client
+
+In the REST client, here is an example calling [Get Public Products](https://docs.cloud.coinbase.com/advanced-trade/reference/retailbrokerageapi_getpublicproducts). 
+It does _not_ require authentication and is the public counterpart to 
+[Get Products](https://docs.cloud.coinbase.com/advanced-trade/reference/retailbrokerageapi_getproducts), which _does_ require authentication.
+
+Both endpoints return the same data.
+
+
+```
+from coinbase.rest import RESTClient
+
+client = RESTClient()
+
+public_products = client.get_public_products()
+print(public_products)
+```
+_Full list of all public REST endpoints [here](https://docs.cloud.coinbase.com/advanced-trade/docs/rest-api-overview#public-endpoints)_
+
+_Rate limit details for REST endpoints [here](https://docs.cloud.coinbase.com/advanced-trade/docs/rest-api-rate-limits)_
+
+### Websocket Client
+
+In the Websocket client, here is an example subscribing to the [ticker](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-channels#ticker-channel) channel. 
+Unlike the REST client, Websocket channels handle both authenticated and unauthenticated requests. 
+At the moment, most channels in the Websocket client are public and can be used without keys.
+
+```
+import time
+from coinbase.websocket import WSClient
+
+def on_message(msg):
+    print(msg)
+
+client = WSClient(on_message=on_message)
+
+client.open()
+client.ticker(product_ids=["BTC-USD"])
+
+time.sleep(10)
+
+client.ticker_unsubscribe(product_ids=["BTC-USD"])
+client.close()
+```
+
+_Full list of all public Websocket channels [here](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-channels)_
+
+_Rate limit details for Websocket channels [here](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-rate-limits)_
+
+
+___
 ## Changelog
 For a detailed list of changes, see the [Changelog](https://github.com/coinbase/coinbase-advanced-py/blob/master/CHANGELOG.md).
 
+___
 ## Contributing
 
 If you've found a bug within this project, open an issue on this repo and add the "bug" label to it.
 If you would like to request a new feature, open an issue on this repo and add the "enhancement" label to it.
 Direct concerns or questions on the API to the [Advanced API Developer Forum](https://forums.coinbasecloud.dev/c/advanced-trade-api/20).
```

### Comparing `coinbase-advanced-py-1.2.2/README.md` & `coinbase-advanced-py-1.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,33 +4,36 @@
 [![Code Style](https://img.shields.io/badge/code_style-black-black)](https://black.readthedocs.io/en/stable/)
 
 Welcome to the official Coinbase Advanced API Python SDK. This python project was created to allow coders to easily plug into the [Coinbase Advanced API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/welcome).
 This SDK also supports easy connection to the [Coinbase Advanced Trade WebSocket API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview).
 
 For thorough documentation of all available functions, refer to the following link: https://coinbase.github.io/coinbase-advanced-py
 
+___
 ## Installation
 
 ```bash
 pip3 install coinbase-advanced-py
 ```
 
-## Cloud API Keys
+___
+## Coinbase Developer Platform (CDP) API Keys
 
-This SDK uses the Coinbase Cloud API keys. To use this SDK, you will need to create a Coinbase Cloud API key and secret by following the instructions [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/auth#cloud-api-keys).
+This SDK uses Cloud Developer Platform (CDP) API keys. To use this SDK, you will need to create a CDP API key and secret by following the instructions [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/auth#cloud-api-keys).
 Make sure to save your API key and secret in a safe place. You will not be able to retrieve your secret again.
 
 WARNING: We do not recommend that you save your API secrets directly in your code outside of testing purposes. Best practice is to use a secrets manager and access your secrets that way. You should be careful about exposing your secrets publicly if posting code that leverages this library.
 
 Optional: Set your API key and secret in your environment (make sure to put these in quotation marks). For example:
 ```bash
 export COINBASE_API_KEY="organizations/{org_id}/apiKeys/{key_id}"
 export COINBASE_API_SECRET="-----BEGIN EC PRIVATE KEY-----\nYOUR PRIVATE KEY\n-----END EC PRIVATE KEY-----\n"
 ```
 
+___
 ## REST API Client
 In your code, import the RESTClient class and instantiate it:
 ```python
 from coinbase.rest import RESTClient
 
 client = RESTClient() # Uses environment variables for API key and secret
 ```
@@ -95,14 +98,15 @@
 Once again, the built-in way to query these through the SDK would be:
 ```python
 market_trades = client.get_market_trades(product_id="BTC-USD", limit=5)
 
 portfolio = client.create_portfolio(name="TestPortfolio")
 ```
 
+___
 ## WebSocket API Client
 We offer a WebSocket API client that allows you to connect to the [Coinbase Advanced Trade WebSocket API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview).
 Refer to the [Advanced Trade WebSocket Channels](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels) page for detailed information on each offered channel.
 
 In your code, import the WSClient class and instantiate it. The WSClient requires an API key and secret to be passed in as arguments. You can also use a key file or environment variables as described in the RESTClient instructions above.
 
 You must specify an `on_message` function that will be called when a message is received from the WebSocket API. This function must take in a single argument, which will be the raw message received from the WebSocket API. For example:
@@ -220,26 +224,28 @@
 ```
 
 ### Async WebSocket Client
 The functions described above handle the asynchronous nature of WebSocket connections for you. However, if you wish to handle this yourself, you can use the `async_open`, `async_subscribe`, `async_unsubscribe`, and `async_close` methods.
 
 We similarly provide async channel specific methods for subscribing and unsubscribing such as `ticker_async`, `ticker_unsubscribe_async`, etc.
 
+___
 ## Debugging the Clients
 You can enable debug logging for the REST and WebSocket clients by setting the `verbose` variable to `True` when initializing the clients. This will log useful information throughout the lifecycle of the REST request or WebSocket connection, and is highly recommended for debugging purposes.
 ```python
 rest_client = RESTClient(api_key=api_key, api_secret=api_secret, verbose=True)
 
 ws_client = WSClient(api_key=api_key, api_secret=api_secret, on_message=on_message, verbose=True)
 ```
 
+___
 ## Authentication
-Authentication of Cloud API Keys is handled automatically by the SDK when making a REST request or sending a WebSocket message.
+Authentication of CDP API Keys is handled automatically by the SDK when making a REST request or sending a WebSocket message.
 
-However, if you wish to handle this yourself, you must create a JWT token and attach it to your request as detailed in the Cloud API docs [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/rest-api-auth#making-requests). Use the built in `jwt_generator` to create your JWT token. For example:
+However, if you wish to handle this yourself, you must create a JWT token and attach it to your request as detailed in the API docs [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/rest-api-auth#making-requests). Use the built in `jwt_generator` to create your JWT token. For example:
 ```python
 from coinbase import jwt_generator
 
 api_key = "organizations/{org_id}/apiKeys/{key_id}"
 api_secret = "-----BEGIN EC PRIVATE KEY-----\nYOUR PRIVATE KEY\n-----END EC PRIVATE KEY-----\n"
 
 uri = "/api/v3/brokerage/orders"
@@ -259,15 +265,79 @@
 api_key = "organizations/{org_id}/apiKeys/{key_id}"
 api_secret = "-----BEGIN EC PRIVATE KEY-----\nYOUR PRIVATE KEY\n-----END EC PRIVATE KEY-----\n"
 
 jwt = jwt_generator.build_ws_jwt(api_key, api_secret)
 ```
 Use this JWT to connect to the Websocket API by setting it in the "jwt" field of your subscription requests. See the docs [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview#sending-messages-using-cloud-api-keys) for more details.
 
+___
+## Accessing public endpoints without authentication
+
+Both clients contain public endpoints which can be accessed without authentication. 
+
+To do so, simply initialize the clients without providing any API keys as arguments. 
+
+**_Notes:_**
+
+- Making calls to private endpoints or channels while unauthenticated will return an error
+- Unauthenticated requests are rate-limited more aggressively. Because of this we recommend that you authenticate your requests
+
+### REST Client
+
+In the REST client, here is an example calling [Get Public Products](https://docs.cloud.coinbase.com/advanced-trade/reference/retailbrokerageapi_getpublicproducts). 
+It does _not_ require authentication and is the public counterpart to 
+[Get Products](https://docs.cloud.coinbase.com/advanced-trade/reference/retailbrokerageapi_getproducts), which _does_ require authentication.
+
+Both endpoints return the same data.
+
+
+```
+from coinbase.rest import RESTClient
+
+client = RESTClient()
+
+public_products = client.get_public_products()
+print(public_products)
+```
+_Full list of all public REST endpoints [here](https://docs.cloud.coinbase.com/advanced-trade/docs/rest-api-overview#public-endpoints)_
+
+_Rate limit details for REST endpoints [here](https://docs.cloud.coinbase.com/advanced-trade/docs/rest-api-rate-limits)_
+
+### Websocket Client
+
+In the Websocket client, here is an example subscribing to the [ticker](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-channels#ticker-channel) channel. 
+Unlike the REST client, Websocket channels handle both authenticated and unauthenticated requests. 
+At the moment, most channels in the Websocket client are public and can be used without keys.
+
+```
+import time
+from coinbase.websocket import WSClient
+
+def on_message(msg):
+    print(msg)
+
+client = WSClient(on_message=on_message)
+
+client.open()
+client.ticker(product_ids=["BTC-USD"])
+
+time.sleep(10)
+
+client.ticker_unsubscribe(product_ids=["BTC-USD"])
+client.close()
+```
+
+_Full list of all public Websocket channels [here](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-channels)_
+
+_Rate limit details for Websocket channels [here](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-rate-limits)_
+
+
+___
 ## Changelog
 For a detailed list of changes, see the [Changelog](https://github.com/coinbase/coinbase-advanced-py/blob/master/CHANGELOG.md).
 
+___
 ## Contributing
 
 If you've found a bug within this project, open an issue on this repo and add the "bug" label to it.
 If you would like to request a new feature, open an issue on this repo and add the "enhancement" label to it.
 Direct concerns or questions on the API to the [Advanced API Developer Forum](https://forums.coinbasecloud.dev/c/advanced-trade-api/20).
```

### Comparing `coinbase-advanced-py-1.2.2/coinbase/api_base.py` & `coinbase-advanced-py-1.3.0/coinbase/api_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,19 +41,25 @@
                 else:
                     key_json = json.load(key_file)
                 api_key = key_json["name"]
                 api_secret = key_json["privateKey"]
             except json.JSONDecodeError as e:
                 raise Exception(f"Error decoding JSON: {e}")
 
-        if api_key is None:
+        self.is_authenticated = False
+        if api_key is not None and api_secret is not None:
+            self.api_key = api_key
+            self.api_secret = bytes(api_secret, encoding="utf8").decode(
+                "unicode_escape"
+            )
+            self.is_authenticated = True
+        elif api_key is not None:
             raise Exception(
-                f"Must specify env var COINBASE_API_KEY or pass api_key in constructor"
+                f"Only api_key provided in constructor. Please also provide api_secret"
             )
-        if api_secret is None:
+        elif api_secret is not None:
             raise Exception(
-                f"Must specify env var COINBASE_API_SECRET or pass api_secret in constructor"
+                f"Only api_secret provided in constructor. Please also provide api_key"
             )
-        self.api_key = api_key
-        self.api_secret = bytes(api_secret, encoding="utf8").decode("unicode_escape")
+
         self.base_url = base_url
         self.timeout = timeout
```

### Comparing `coinbase-advanced-py-1.2.2/coinbase/constants.py` & `coinbase-advanced-py-1.3.0/coinbase/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,7 +26,9 @@
 CANDLES = "candles"
 MARKET_TRADES = "market_trades"
 STATUS = "status"
 TICKER = "ticker"
 TICKER_BATCH = "ticker_batch"
 LEVEL2 = "level2"
 USER = "user"
+
+WS_AUTH_CHANNELS = {USER}
```

### Comparing `coinbase-advanced-py-1.2.2/coinbase/jwt_generator.py` & `coinbase-advanced-py-1.3.0/coinbase/jwt_generator.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/coinbase/rest/__init__.py` & `coinbase-advanced-py-1.3.0/coinbase/rest/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from .rest_base import RESTBase
 
 
 class RESTClient(RESTBase):
     from .accounts import get_account, get_accounts
-    from .common import get_unix_time
     from .convert import commit_convert_trade, create_convert_quote, get_convert_trade
     from .fees import get_transaction_summary
     from .futures import (
         cancel_pending_futures_sweep,
         close_position,
         get_futures_balance_summary,
         get_futures_position,
@@ -18,28 +17,34 @@
     from .market_data import get_candles, get_market_trades
     from .orders import (
         cancel_orders,
         create_order,
         edit_order,
         get_fills,
         get_order,
+        limit_order_fok,
+        limit_order_fok_buy,
+        limit_order_fok_sell,
         limit_order_gtc,
         limit_order_gtc_buy,
         limit_order_gtc_sell,
         limit_order_gtd,
         limit_order_gtd_buy,
         limit_order_gtd_sell,
         limit_order_ioc,
         limit_order_ioc_buy,
         limit_order_ioc_sell,
         list_orders,
         market_order,
         market_order_buy,
         market_order_sell,
         preview_edit_order,
+        preview_limit_order_fok,
+        preview_limit_order_fok_buy,
+        preview_limit_order_fok_sell,
         preview_limit_order_gtc,
         preview_limit_order_gtc_buy,
         preview_limit_order_gtc_sell,
         preview_limit_order_gtd,
         preview_limit_order_gtd_buy,
         preview_limit_order_gtd_sell,
         preview_limit_order_ioc,
@@ -51,20 +56,32 @@
         preview_order,
         preview_stop_limit_order_gtc,
         preview_stop_limit_order_gtc_buy,
         preview_stop_limit_order_gtc_sell,
         preview_stop_limit_order_gtd,
         preview_stop_limit_order_gtd_buy,
         preview_stop_limit_order_gtd_sell,
+        preview_trigger_bracket_order_gtc,
+        preview_trigger_bracket_order_gtc_buy,
+        preview_trigger_bracket_order_gtc_sell,
+        preview_trigger_bracket_order_gtd,
+        preview_trigger_bracket_order_gtd_buy,
+        preview_trigger_bracket_order_gtd_sell,
         stop_limit_order_gtc,
         stop_limit_order_gtc_buy,
         stop_limit_order_gtc_sell,
         stop_limit_order_gtd,
         stop_limit_order_gtd_buy,
         stop_limit_order_gtd_sell,
+        trigger_bracket_order_gtc,
+        trigger_bracket_order_gtc_buy,
+        trigger_bracket_order_gtc_sell,
+        trigger_bracket_order_gtd,
+        trigger_bracket_order_gtd_buy,
+        trigger_bracket_order_gtd_sell,
     )
     from .payments import get_payment_method, list_payment_methods
     from .perpetuals import (
         allocate_portfolio,
         get_perps_portfolio_summary,
         get_perps_position,
         list_perps_positions,
@@ -74,7 +91,15 @@
         delete_portfolio,
         edit_portfolio,
         get_portfolio_breakdown,
         get_portfolios,
         move_portfolio_funds,
     )
     from .products import get_best_bid_ask, get_product, get_product_book, get_products
+    from .public import (
+        get_public_candles,
+        get_public_market_trades,
+        get_public_product,
+        get_public_product_book,
+        get_public_products,
+        get_unix_time,
+    )
```

### Comparing `coinbase-advanced-py-1.2.2/coinbase/rest/accounts.py` & `coinbase-advanced-py-1.3.0/coinbase/rest/accounts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from typing import Any, Dict, Optional
 
 from coinbase.constants import API_PREFIX
 
 
 def get_accounts(
-    self, limit: Optional[int] = None, cursor: Optional[str] = None, **kwargs
+    self,
+    limit: Optional[int] = None,
+    cursor: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
 ) -> Dict[str, Any]:
     """
     **List Accounts**
     _________________
     [GET] https://api.coinbase.com/api/v3/brokerage/accounts
 
     __________
@@ -19,15 +23,19 @@
 
     __________
 
     **Read more on the official documentation:** `List Accounts <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_getaccounts>`_
 
     """
     endpoint = f"{API_PREFIX}/accounts"
-    params = {"limit": limit, "cursor": cursor}
+    params = {
+        "limit": limit,
+        "cursor": cursor,
+        "retail_portfolio_id": retail_portfolio_id,
+    }
 
     return self.get(endpoint, params=params, **kwargs)
 
 
 def get_account(self, account_uuid: str, **kwargs) -> Dict[str, Any]:
     """
```

### Comparing `coinbase-advanced-py-1.2.2/coinbase/rest/convert.py` & `coinbase-advanced-py-1.3.0/coinbase/rest/convert.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/coinbase/rest/fees.py` & `coinbase-advanced-py-1.3.0/coinbase/rest/fees.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/coinbase/rest/futures.py` & `coinbase-advanced-py-1.3.0/coinbase/rest/futures.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/coinbase/rest/market_data.py` & `coinbase-advanced-py-1.3.0/coinbase/rest/market_data.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/coinbase/rest/orders.py` & `coinbase-advanced-py-1.3.0/coinbase/rest/orders.py`

 * *Files 17% similar despite different names*

```diff
@@ -629,14 +629,157 @@
         leverage=leverage,
         margin_type=margin_type,
         retail_portfolio_id=retail_portfolio_id,
         **kwargs,
     )
 
 
+# Limit FOK Orders
+def limit_order_fok(
+    self,
+    client_order_id: str,
+    product_id: str,
+    side: str,
+    base_size: str,
+    limit_price: str,
+    self_trade_prevention_id: Optional[str] = None,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Limit FOK Order**
+    ________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders
+
+    __________
+
+    **Description:**
+
+    Place a Limit Order with a FOK time-in-force policy. Provide the base_size (quantity of your base currency to
+    spend) as well as a limit_price that indicates the maximum price at which the order should be filled.
+
+    __________
+
+    **Read more on the official documentation:** `Create Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    """
+
+    limit_limit_fok = {"base_size": base_size, "limit_price": limit_price}
+
+    order_configuration = {"limit_limit_fok": limit_limit_fok}
+
+    return create_order(
+        self,
+        client_order_id,
+        product_id,
+        side,
+        order_configuration,
+        self_trade_prevention_id=self_trade_prevention_id,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
+def limit_order_fok_buy(
+    self,
+    client_order_id: str,
+    product_id: str,
+    base_size: str,
+    limit_price: str,
+    self_trade_prevention_id: Optional[str] = None,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Limit FOK Order Buy**
+    ________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders
+
+    __________
+
+    **Description:**
+
+    Place a Buy Limit Order with a FOK time-in-force policy. Provide the base_size (quantity of your base currency to
+    spend) as well as a limit_price that indicates the maximum price at which the order should be filled.
+
+    __________
+
+    **Read more on the official documentation:** `Create Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    """
+
+    return limit_order_fok(
+        self,
+        client_order_id,
+        product_id,
+        "BUY",
+        base_size=base_size,
+        limit_price=limit_price,
+        self_trade_prevention_id=self_trade_prevention_id,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
+def limit_order_fok_sell(
+    self,
+    client_order_id: str,
+    product_id: str,
+    base_size: str,
+    limit_price: str,
+    self_trade_prevention_id: Optional[str] = None,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Limit FOK Order Sell**
+    ________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders
+
+    __________
+
+    **Description:**
+
+    Place a Sell Limit Order with a FOK time-in-force policy. Provide the base_size (quantity of your base currency to
+    spend) as well as a limit_price that indicates the maximum price at which the order should be filled.
+
+    __________
+
+    **Read more on the official documentation:** `Create Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    """
+
+    return limit_order_fok(
+        self,
+        client_order_id,
+        product_id,
+        "SELL",
+        base_size=base_size,
+        limit_price=limit_price,
+        self_trade_prevention_id=self_trade_prevention_id,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
 # Stop-Limit GTC orders
 def stop_limit_order_gtc(
     self,
     client_order_id: str,
     product_id: str,
     side: str,
     base_size: str,
@@ -945,14 +1088,318 @@
         leverage=leverage,
         margin_type=margin_type,
         retail_portfolio_id=retail_portfolio_id,
         **kwargs,
     )
 
 
+# Trigger Bracket GTC orders
+def trigger_bracket_order_gtc(
+    self,
+    client_order_id: str,
+    product_id: str,
+    side: str,
+    base_size: str,
+    limit_price: str,
+    stop_trigger_price: str,
+    self_trade_prevention_id: Optional[str] = None,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Trigger Bracket Order GTC**
+    ________________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders
+
+    __________
+
+    **Description:**
+
+    Place a Trigger Bracket order with a GTC time-in-force policy. Trigger Bracket orders become active and wait to trigger based on
+    the movement of the last trade price. The last trade price is the last price at which an order was filled.
+
+    __________
+
+    **Read more on the official documentation:** `Create Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    """
+    order_configuration = {
+        "trigger_bracket_gtc": {
+            "base_size": base_size,
+            "limit_price": limit_price,
+            "stop_trigger_price": stop_trigger_price,
+        }
+    }
+
+    return create_order(
+        self,
+        client_order_id,
+        product_id,
+        side,
+        order_configuration,
+        self_trade_prevention_id=self_trade_prevention_id,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
+def trigger_bracket_order_gtc_buy(
+    self,
+    client_order_id: str,
+    product_id: str,
+    base_size: str,
+    limit_price: str,
+    stop_trigger_price: str,
+    self_trade_prevention_id: Optional[str] = None,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Trigger Bracket Order GTC Buy**
+    ____________________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders
+
+    __________
+
+    **Description:**
+
+    Place a BUY Trigger Bracket order with a GTC time-in-force policy. Trigger Bracket orders become active and wait to trigger based on
+    the movement of the last trade price. The last trade price is the last price at which an order was filled.
+
+    __________
+
+    **Read more on the official documentation:** `Create Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    """
+    return trigger_bracket_order_gtc(
+        self,
+        client_order_id,
+        product_id,
+        "BUY",
+        base_size=base_size,
+        limit_price=limit_price,
+        stop_trigger_price=stop_trigger_price,
+        self_trade_prevention_id=self_trade_prevention_id,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
+def trigger_bracket_order_gtc_sell(
+    self,
+    client_order_id: str,
+    product_id: str,
+    base_size: str,
+    limit_price: str,
+    stop_trigger_price: str,
+    self_trade_prevention_id: Optional[str] = None,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Trigger Bracket Order GTC Sell**
+    _____________________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders
+
+    __________
+
+    **Description:**
+
+    Place a SELL Trigger Bracket order with a GTC time-in-force policy. Trigger Bracket orders become active and wait to trigger based on
+    the movement of the last trade price. The last trade price is the last price at which an order was filled.
+
+    __________
+
+    **Read more on the official documentation:** `Create Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    """
+    return trigger_bracket_order_gtc(
+        self,
+        client_order_id,
+        product_id,
+        "SELL",
+        base_size=base_size,
+        limit_price=limit_price,
+        stop_trigger_price=stop_trigger_price,
+        self_trade_prevention_id=self_trade_prevention_id,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
+# Trigger Bracket GTD orders
+def trigger_bracket_order_gtd(
+    self,
+    client_order_id: str,
+    product_id: str,
+    side: str,
+    base_size: str,
+    limit_price: str,
+    stop_trigger_price: str,
+    end_time: str,
+    self_trade_prevention_id: Optional[str] = None,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Trigger Bracket Order GTD**
+    ________________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders
+
+    __________
+
+    **Description:**
+
+    Place a Trigger Bracket order with a GTD time-in-force policy. Trigger Bracket orders become active and wait to trigger based on
+    the movement of the last trade price. The last trade price is the last price at which an order was filled.
+
+    __________
+
+    **Read more on the official documentation:** `Create Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    """
+    order_configuration = {
+        "trigger_bracket_gtd": {
+            "base_size": base_size,
+            "limit_price": limit_price,
+            "stop_trigger_price": stop_trigger_price,
+            "end_time": end_time,
+        }
+    }
+
+    return create_order(
+        self,
+        client_order_id,
+        product_id,
+        side,
+        order_configuration,
+        self_trade_prevention_id=self_trade_prevention_id,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
+def trigger_bracket_order_gtd_buy(
+    self,
+    client_order_id: str,
+    product_id: str,
+    base_size: str,
+    limit_price: str,
+    stop_trigger_price: str,
+    end_time: str,
+    self_trade_prevention_id: Optional[str] = None,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Trigger Bracket Order GTD Buy**
+    ____________________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders
+
+    __________
+
+    **Description:**
+
+    Place a BUY Trigger Bracket order with a GTD time-in-force policy. Trigger Bracket orders become active and wait to trigger based on
+    the movement of the last trade price. The last trade price is the last price at which an order was filled.
+
+    __________
+
+    **Read more on the official documentation:** `Create Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    """
+    return trigger_bracket_order_gtd(
+        self,
+        client_order_id,
+        product_id,
+        "BUY",
+        base_size=base_size,
+        limit_price=limit_price,
+        stop_trigger_price=stop_trigger_price,
+        end_time=end_time,
+        self_trade_prevention_id=self_trade_prevention_id,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
+def trigger_bracket_order_gtd_sell(
+    self,
+    client_order_id: str,
+    product_id: str,
+    base_size: str,
+    limit_price: str,
+    stop_trigger_price: str,
+    end_time: str,
+    self_trade_prevention_id: Optional[str] = None,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Trigger Bracket Order GTD Sell**
+    _____________________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders
+
+    __________
+
+    **Description:**
+
+    Place a SELL Trigger Bracket order with a GTD time-in-force policy. Trigger Bracket orders become active and wait to trigger based on
+    the movement of the last trade price. The last trade price is the last price at which an order was filled.
+
+    __________
+
+    **Read more on the official documentation:** `Create Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_postorder>`_
+    """
+    return trigger_bracket_order_gtd(
+        self,
+        client_order_id,
+        product_id,
+        "SELL",
+        base_size=base_size,
+        limit_price=limit_price,
+        stop_trigger_price=stop_trigger_price,
+        end_time=end_time,
+        self_trade_prevention_id=self_trade_prevention_id,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
 def get_order(self, order_id: str, **kwargs) -> Dict[str, Any]:
     """
     **Get Order**
     _____________
 
     [GET] https://api.coinbase.com/api/v3/brokerage/orders/historical/{order_id}
 
@@ -1828,14 +2275,162 @@
         leverage=leverage,
         margin_type=margin_type,
         retail_portfolio_id=retail_portfolio_id,
         **kwargs,
     )
 
 
+def preview_limit_order_fok(
+    self,
+    product_id: str,
+    side: str,
+    base_size: str,
+    limit_price: str,
+    commission_rate: Optional[str] = None,
+    is_max: Optional[bool] = False,
+    tradable_balance: Optional[str] = None,
+    skip_fcm_risk_check: Optional[bool] = False,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Preview Limit Order FOK**
+    ___________________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders/preview
+
+    __________
+
+    **Description:**
+
+    Preview the results of a limit order FOK request before sending.
+
+    __________
+
+    **Read more on the official documentation:** `Preview Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    """
+    order_configuration = {
+        "limit_limit_fok": {"base_size": base_size, "limit_price": limit_price}
+    }
+
+    return preview_order(
+        self,
+        product_id,
+        side,
+        order_configuration,
+        commission_rate=commission_rate,
+        is_max=is_max,
+        tradable_balance=tradable_balance,
+        skip_fcm_risk_check=skip_fcm_risk_check,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
+def preview_limit_order_fok_buy(
+    self,
+    product_id: str,
+    base_size: str,
+    limit_price: str,
+    commission_rate: Optional[str] = None,
+    is_max: Optional[bool] = False,
+    tradable_balance: Optional[str] = None,
+    skip_fcm_risk_check: Optional[bool] = False,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Preview Limit Order FOK Buy**
+    ___________________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders/preview
+
+    __________
+
+    **Description:**
+
+    Preview the results of a limit order FOK buy request before sending.
+
+    __________
+
+    **Read more on the official documentation:** `Preview Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    """
+    return preview_limit_order_fok(
+        self,
+        product_id,
+        "BUY",
+        base_size=base_size,
+        limit_price=limit_price,
+        commission_rate=commission_rate,
+        is_max=is_max,
+        tradable_balance=tradable_balance,
+        skip_fcm_risk_check=skip_fcm_risk_check,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
+def preview_limit_order_fok_sell(
+    self,
+    product_id: str,
+    base_size: str,
+    limit_price: str,
+    commission_rate: Optional[str] = None,
+    is_max: Optional[bool] = False,
+    tradable_balance: Optional[str] = None,
+    skip_fcm_risk_check: Optional[bool] = False,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Preview Limit Order FOK Sell**
+    ___________________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders/preview
+
+    __________
+
+    **Description:**
+
+    Preview the results of a limit order FOK sell request before sending.
+
+    __________
+
+    **Read more on the official documentation:** `Preview Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    """
+    return preview_limit_order_fok(
+        self,
+        product_id,
+        "SELL",
+        base_size=base_size,
+        limit_price=limit_price,
+        commission_rate=commission_rate,
+        is_max=is_max,
+        tradable_balance=tradable_balance,
+        skip_fcm_risk_check=skip_fcm_risk_check,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
 # Preview Stop-Limit GTC orders
 def preview_stop_limit_order_gtc(
     self,
     product_id: str,
     side: str,
     base_size: str,
     limit_price: str,
@@ -2158,9 +2753,331 @@
         commission_rate=commission_rate,
         is_max=is_max,
         tradable_balance=tradable_balance,
         skip_fcm_risk_check=skip_fcm_risk_check,
         leverage=leverage,
         margin_type=margin_type,
         retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
+# Preview Trigger Bracket GTC orders
+def preview_trigger_bracket_order_gtc(
+    self,
+    product_id: str,
+    side: str,
+    base_size: str,
+    limit_price: str,
+    stop_trigger_price: str,
+    commission_rate: Optional[str] = None,
+    is_max: Optional[bool] = False,
+    tradable_balance: Optional[str] = None,
+    skip_fcm_risk_check: Optional[bool] = False,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Preview Trigger Bracket Order GTC**
+    ________________________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders/preview
+
+    __________
+
+    **Description:**
+
+    Preview the results of a trigger bracket GTC order request before sending.
+
+    __________
+
+    **Read more on the official documentation:** `Preview Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    """
+    order_configuration = {
+        "trigger_bracket_gtc": {
+            "base_size": base_size,
+            "limit_price": limit_price,
+            "stop_trigger_price": stop_trigger_price,
+        }
+    }
+
+    return preview_order(
+        self,
+        product_id,
+        side,
+        order_configuration,
+        commission_rate=commission_rate,
+        is_max=is_max,
+        tradable_balance=tradable_balance,
+        skip_fcm_risk_check=skip_fcm_risk_check,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
+def preview_trigger_bracket_order_gtc_buy(
+    self,
+    product_id: str,
+    base_size: str,
+    limit_price: str,
+    stop_trigger_price: str,
+    commission_rate: Optional[str] = None,
+    is_max: Optional[bool] = False,
+    tradable_balance: Optional[str] = None,
+    skip_fcm_risk_check: Optional[bool] = False,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Preview Trigger Bracket Order GTC Buy**
+    ____________________________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders/preview
+
+    __________
+
+    **Description:**
+
+    Preview the results of a trigger bracket GTC order buy request before sending.
+
+    __________
+
+    **Read more on the official documentation:** `Preview Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    """
+    return preview_trigger_bracket_order_gtc(
+        self,
+        product_id,
+        "BUY",
+        base_size=base_size,
+        limit_price=limit_price,
+        stop_trigger_price=stop_trigger_price,
+        commission_rate=commission_rate,
+        is_max=is_max,
+        tradable_balance=tradable_balance,
+        skip_fcm_risk_check=skip_fcm_risk_check,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
+def preview_trigger_bracket_order_gtc_sell(
+    self,
+    product_id: str,
+    base_size: str,
+    limit_price: str,
+    stop_trigger_price: str,
+    commission_rate: Optional[str] = None,
+    is_max: Optional[bool] = False,
+    tradable_balance: Optional[str] = None,
+    skip_fcm_risk_check: Optional[bool] = False,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Preview Trigger Bracket Order GTC Sell**
+    _____________________________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders/preview
+
+    __________
+
+    **Description:**
+
+    Preview the results of a trigger bracket GTC order sell request before sending.
+
+    __________
+
+    **Read more on the official documentation:** `Preview Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    """
+    return preview_trigger_bracket_order_gtc(
+        self,
+        product_id,
+        "SELL",
+        base_size=base_size,
+        limit_price=limit_price,
+        stop_trigger_price=stop_trigger_price,
+        commission_rate=commission_rate,
+        is_max=is_max,
+        tradable_balance=tradable_balance,
+        skip_fcm_risk_check=skip_fcm_risk_check,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
+# Preview Trigger Bracket GTD orders
+def preview_trigger_bracket_order_gtd(
+    self,
+    product_id: str,
+    side: str,
+    base_size: str,
+    limit_price: str,
+    stop_trigger_price: str,
+    end_time: str,
+    commission_rate: Optional[str] = None,
+    is_max: Optional[bool] = False,
+    tradable_balance: Optional[str] = None,
+    skip_fcm_risk_check: Optional[bool] = False,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Preview Trigger Bracket Order GTD**
+    ________________________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders/preview
+
+    __________
+
+    **Description:**
+
+    Preview the results of a trigger bracket GTD order request before sending.
+
+    __________
+
+    **Read more on the official documentation:** `Preview Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    """
+    order_configuration = {
+        "trigger_bracket_gtd": {
+            "base_size": base_size,
+            "limit_price": limit_price,
+            "stop_trigger_price": stop_trigger_price,
+            "end_time": end_time,
+        }
+    }
+
+    return preview_order(
+        self,
+        product_id,
+        side,
+        order_configuration,
+        commission_rate=commission_rate,
+        is_max=is_max,
+        tradable_balance=tradable_balance,
+        skip_fcm_risk_check=skip_fcm_risk_check,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
+def preview_trigger_bracket_order_gtd_buy(
+    self,
+    product_id: str,
+    base_size: str,
+    limit_price: str,
+    stop_trigger_price: str,
+    end_time: str,
+    commission_rate: Optional[str] = None,
+    is_max: Optional[bool] = False,
+    tradable_balance: Optional[str] = None,
+    skip_fcm_risk_check: Optional[bool] = False,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Preview Trigger Bracket Order GTD Buy**
+    ____________________________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders/preview
+
+    __________
+
+    **Description:**
+
+    Preview the results of a trigger bracket GTD order buy request before sending.
+
+    __________
+
+    **Read more on the official documentation:** `Preview Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    """
+    return preview_trigger_bracket_order_gtd(
+        self,
+        product_id,
+        "BUY",
+        base_size=base_size,
+        limit_price=limit_price,
+        stop_trigger_price=stop_trigger_price,
+        end_time=end_time,
+        commission_rate=commission_rate,
+        is_max=is_max,
+        tradable_balance=tradable_balance,
+        skip_fcm_risk_check=skip_fcm_risk_check,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
+        **kwargs,
+    )
+
+
+def preview_trigger_bracket_order_gtd_sell(
+    self,
+    product_id: str,
+    base_size: str,
+    limit_price: str,
+    stop_trigger_price: str,
+    end_time: str,
+    commission_rate: Optional[str] = None,
+    is_max: Optional[bool] = False,
+    tradable_balance: Optional[str] = None,
+    skip_fcm_risk_check: Optional[bool] = False,
+    leverage: Optional[str] = None,
+    margin_type: Optional[str] = None,
+    retail_portfolio_id: Optional[str] = None,
+    **kwargs,
+) -> Dict[str, Any]:
+    """
+    **Preview Trigger Bracket Order GTD Sell**
+    _____________________________________
+
+    [POST] https://api.coinbase.com/api/v3/brokerage/orders/preview
+
+    __________
+
+    **Description:**
+
+    Preview the results of a trigger bracket GTD order sell request before sending.
+
+    __________
+
+    **Read more on the official documentation:** `Preview Order
+    <https://docs.cloud.coinbase.com/advanced-trade-api/reference/retailbrokerageapi_previeworder>`_
+    """
+    return preview_trigger_bracket_order_gtd(
+        self,
+        product_id,
+        "SELL",
+        base_size=base_size,
+        limit_price=limit_price,
+        stop_trigger_price=stop_trigger_price,
+        end_time=end_time,
+        commission_rate=commission_rate,
+        is_max=is_max,
+        tradable_balance=tradable_balance,
+        skip_fcm_risk_check=skip_fcm_risk_check,
+        leverage=leverage,
+        margin_type=margin_type,
+        retail_portfolio_id=retail_portfolio_id,
         **kwargs,
     )
```

### Comparing `coinbase-advanced-py-1.2.2/coinbase/rest/payments.py` & `coinbase-advanced-py-1.3.0/coinbase/rest/payments.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/coinbase/rest/perpetuals.py` & `coinbase-advanced-py-1.3.0/coinbase/rest/perpetuals.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/coinbase/rest/portfolios.py` & `coinbase-advanced-py-1.3.0/coinbase/rest/portfolios.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/coinbase/rest/products.py` & `coinbase-advanced-py-1.3.0/coinbase/rest/products.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/coinbase/rest/rest_base.py` & `coinbase-advanced-py-1.3.0/coinbase/rest/rest_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+from multiprocessing import AuthenticationError
 from typing import IO, Any, Dict, Optional, Union
 
 import requests
 from requests.exceptions import HTTPError
 
 from coinbase import jwt_generator
 from coinbase.api_base import APIBase, get_logger
@@ -194,14 +195,19 @@
         params: Optional[dict] = None,
         data: Optional[dict] = None,
         public=False,
     ):
         """
         :meta private:
         """
+        if not self.is_authenticated and not public:
+            raise AuthenticationError(
+                "Unauthenticated request to private endpoint. If you wish to access private endpoints, you must provide your API key and secret when initializing the RESTClient."
+            )
+
         headers = self.set_headers(http_method, url_path, public)
 
         if params is not None:
             params = {key: value for key, value in params.items() if value is not None}
 
         if data is not None:
             data = {key: value for key, value in data.items() if value is not None}
@@ -242,11 +248,11 @@
         return {
             "User-Agent": USER_AGENT,
             "Content-Type": "application/json",
             **(
                 {
                     "Authorization": f"Bearer {jwt_generator.build_rest_jwt(uri, self.api_key, self.api_secret)}",
                 }
-                if not public
+                if self.is_authenticated
                 else {}
             ),
         }
```

### Comparing `coinbase-advanced-py-1.2.2/coinbase/websocket/__init__.py` & `coinbase-advanced-py-1.3.0/coinbase/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/coinbase/websocket/channels.py` & `coinbase-advanced-py-1.3.0/coinbase/websocket/channels.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/coinbase/websocket/websocket_base.py` & `coinbase-advanced-py-1.3.0/coinbase/websocket/websocket_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import asyncio
 import json
 import logging
 import os
 import ssl
 import threading
 import time
+from multiprocessing import AuthenticationError
 from typing import IO, Callable, List, Optional, Union
 
 import backoff
 import websockets
 
 from coinbase import jwt_generator
 from coinbase.api_base import APIBase, get_logger
 from coinbase.constants import (
     API_ENV_KEY,
     API_SECRET_ENV_KEY,
     SUBSCRIBE_MESSAGE_TYPE,
     UNSUBSCRIBE_MESSAGE_TYPE,
     USER_AGENT,
+    WS_AUTH_CHANNELS,
     WS_BASE_URL,
     WS_RETRY_BASE,
     WS_RETRY_FACTOR,
     WS_RETRY_MAX,
 )
 
 logger = get_logger("coinbase.WSClient")
@@ -260,16 +262,22 @@
 
         - **product_ids** - product ids to subscribe to
         - **channels** - channels to subscribe to
         """
         self._ensure_websocket_open()
         for channel in channels:
             try:
+                if not self.is_authenticated and channel in WS_AUTH_CHANNELS:
+                    raise AuthenticationError(
+                        "Unauthenticated request to private channel."
+                    )
+
+                is_public = False if channel in WS_AUTH_CHANNELS else True
                 message = self._build_subscription_message(
-                    product_ids, channel, SUBSCRIBE_MESSAGE_TYPE
+                    product_ids, channel, SUBSCRIBE_MESSAGE_TYPE, is_public
                 )
                 json_message = json.dumps(message)
 
                 logger.debug(
                     "Subscribing to channel %s for product IDs: %s",
                     channel,
                     product_ids,
@@ -326,16 +334,21 @@
 
         - **product_ids** - product ids to unsubscribe from
         - **channels** - channels to unsubscribe from
         """
         self._ensure_websocket_open()
         for channel in channels:
             try:
+                if not self.is_authenticated and channel in WS_AUTH_CHANNELS:
+                    raise AuthenticationError(
+                        "Unauthenticated request to private channel. If you wish to access private channels, you must provide your API key and secret when initializing the WSClient."
+                    )
+                is_public = False if channel in WS_AUTH_CHANNELS else True
                 message = self._build_subscription_message(
-                    product_ids, channel, UNSUBSCRIBE_MESSAGE_TYPE
+                    product_ids, channel, UNSUBSCRIBE_MESSAGE_TYPE, is_public
                 )
                 json_message = json.dumps(message)
 
                 logger.debug(
                     "Unsubscribing from channel %s for product IDs: %s",
                     channel,
                     product_ids,
@@ -549,24 +562,30 @@
                 logger.error("Exception in message handler: %s", e)
                 self._background_exception = WSClientException(
                     f"Exception in message handler: {e}"
                 )
                 break
 
     def _build_subscription_message(
-        self, product_ids: List[str], channel: str, message_type: str
+        self, product_ids: List[str], channel: str, message_type: str, public: bool
     ):
         """
         :meta private:
         """
         return {
             "type": message_type,
             "product_ids": product_ids,
             "channel": channel,
-            "jwt": jwt_generator.build_ws_jwt(self.api_key, self.api_secret),
+            **(
+                {
+                    "jwt": jwt_generator.build_ws_jwt(self.api_key, self.api_secret),
+                }
+                if self.is_authenticated
+                else {}
+            ),
         }
 
     def _ensure_websocket_not_open(self):
         """
         :meta private:
         """
         if self._is_websocket_open():
```

### Comparing `coinbase-advanced-py-1.2.2/coinbase_advanced_py.egg-info/PKG-INFO` & `coinbase-advanced-py-1.3.0/coinbase_advanced_py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinbase-advanced-py
-Version: 1.2.2
+Version: 1.3.0
 Summary: Coinbase Advanced API Python SDK
 Home-page: https://github.com/coinbase/coinbase-advanced-py
 Author: Coinbase
 License: Apache 2.0
 Keywords: Coinbase,Advanced Trade,API,Advanced API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -34,33 +34,36 @@
 [![Code Style](https://img.shields.io/badge/code_style-black-black)](https://black.readthedocs.io/en/stable/)
 
 Welcome to the official Coinbase Advanced API Python SDK. This python project was created to allow coders to easily plug into the [Coinbase Advanced API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/welcome).
 This SDK also supports easy connection to the [Coinbase Advanced Trade WebSocket API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview).
 
 For thorough documentation of all available functions, refer to the following link: https://coinbase.github.io/coinbase-advanced-py
 
+___
 ## Installation
 
 ```bash
 pip3 install coinbase-advanced-py
 ```
 
-## Cloud API Keys
+___
+## Coinbase Developer Platform (CDP) API Keys
 
-This SDK uses the Coinbase Cloud API keys. To use this SDK, you will need to create a Coinbase Cloud API key and secret by following the instructions [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/auth#cloud-api-keys).
+This SDK uses Cloud Developer Platform (CDP) API keys. To use this SDK, you will need to create a CDP API key and secret by following the instructions [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/auth#cloud-api-keys).
 Make sure to save your API key and secret in a safe place. You will not be able to retrieve your secret again.
 
 WARNING: We do not recommend that you save your API secrets directly in your code outside of testing purposes. Best practice is to use a secrets manager and access your secrets that way. You should be careful about exposing your secrets publicly if posting code that leverages this library.
 
 Optional: Set your API key and secret in your environment (make sure to put these in quotation marks). For example:
 ```bash
 export COINBASE_API_KEY="organizations/{org_id}/apiKeys/{key_id}"
 export COINBASE_API_SECRET="-----BEGIN EC PRIVATE KEY-----\nYOUR PRIVATE KEY\n-----END EC PRIVATE KEY-----\n"
 ```
 
+___
 ## REST API Client
 In your code, import the RESTClient class and instantiate it:
 ```python
 from coinbase.rest import RESTClient
 
 client = RESTClient() # Uses environment variables for API key and secret
 ```
@@ -125,14 +128,15 @@
 Once again, the built-in way to query these through the SDK would be:
 ```python
 market_trades = client.get_market_trades(product_id="BTC-USD", limit=5)
 
 portfolio = client.create_portfolio(name="TestPortfolio")
 ```
 
+___
 ## WebSocket API Client
 We offer a WebSocket API client that allows you to connect to the [Coinbase Advanced Trade WebSocket API](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview).
 Refer to the [Advanced Trade WebSocket Channels](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-channels) page for detailed information on each offered channel.
 
 In your code, import the WSClient class and instantiate it. The WSClient requires an API key and secret to be passed in as arguments. You can also use a key file or environment variables as described in the RESTClient instructions above.
 
 You must specify an `on_message` function that will be called when a message is received from the WebSocket API. This function must take in a single argument, which will be the raw message received from the WebSocket API. For example:
@@ -250,26 +254,28 @@
 ```
 
 ### Async WebSocket Client
 The functions described above handle the asynchronous nature of WebSocket connections for you. However, if you wish to handle this yourself, you can use the `async_open`, `async_subscribe`, `async_unsubscribe`, and `async_close` methods.
 
 We similarly provide async channel specific methods for subscribing and unsubscribing such as `ticker_async`, `ticker_unsubscribe_async`, etc.
 
+___
 ## Debugging the Clients
 You can enable debug logging for the REST and WebSocket clients by setting the `verbose` variable to `True` when initializing the clients. This will log useful information throughout the lifecycle of the REST request or WebSocket connection, and is highly recommended for debugging purposes.
 ```python
 rest_client = RESTClient(api_key=api_key, api_secret=api_secret, verbose=True)
 
 ws_client = WSClient(api_key=api_key, api_secret=api_secret, on_message=on_message, verbose=True)
 ```
 
+___
 ## Authentication
-Authentication of Cloud API Keys is handled automatically by the SDK when making a REST request or sending a WebSocket message.
+Authentication of CDP API Keys is handled automatically by the SDK when making a REST request or sending a WebSocket message.
 
-However, if you wish to handle this yourself, you must create a JWT token and attach it to your request as detailed in the Cloud API docs [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/rest-api-auth#making-requests). Use the built in `jwt_generator` to create your JWT token. For example:
+However, if you wish to handle this yourself, you must create a JWT token and attach it to your request as detailed in the API docs [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/rest-api-auth#making-requests). Use the built in `jwt_generator` to create your JWT token. For example:
 ```python
 from coinbase import jwt_generator
 
 api_key = "organizations/{org_id}/apiKeys/{key_id}"
 api_secret = "-----BEGIN EC PRIVATE KEY-----\nYOUR PRIVATE KEY\n-----END EC PRIVATE KEY-----\n"
 
 uri = "/api/v3/brokerage/orders"
@@ -289,15 +295,79 @@
 api_key = "organizations/{org_id}/apiKeys/{key_id}"
 api_secret = "-----BEGIN EC PRIVATE KEY-----\nYOUR PRIVATE KEY\n-----END EC PRIVATE KEY-----\n"
 
 jwt = jwt_generator.build_ws_jwt(api_key, api_secret)
 ```
 Use this JWT to connect to the Websocket API by setting it in the "jwt" field of your subscription requests. See the docs [here](https://docs.cloud.coinbase.com/advanced-trade-api/docs/ws-overview#sending-messages-using-cloud-api-keys) for more details.
 
+___
+## Accessing public endpoints without authentication
+
+Both clients contain public endpoints which can be accessed without authentication. 
+
+To do so, simply initialize the clients without providing any API keys as arguments. 
+
+**_Notes:_**
+
+- Making calls to private endpoints or channels while unauthenticated will return an error
+- Unauthenticated requests are rate-limited more aggressively. Because of this we recommend that you authenticate your requests
+
+### REST Client
+
+In the REST client, here is an example calling [Get Public Products](https://docs.cloud.coinbase.com/advanced-trade/reference/retailbrokerageapi_getpublicproducts). 
+It does _not_ require authentication and is the public counterpart to 
+[Get Products](https://docs.cloud.coinbase.com/advanced-trade/reference/retailbrokerageapi_getproducts), which _does_ require authentication.
+
+Both endpoints return the same data.
+
+
+```
+from coinbase.rest import RESTClient
+
+client = RESTClient()
+
+public_products = client.get_public_products()
+print(public_products)
+```
+_Full list of all public REST endpoints [here](https://docs.cloud.coinbase.com/advanced-trade/docs/rest-api-overview#public-endpoints)_
+
+_Rate limit details for REST endpoints [here](https://docs.cloud.coinbase.com/advanced-trade/docs/rest-api-rate-limits)_
+
+### Websocket Client
+
+In the Websocket client, here is an example subscribing to the [ticker](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-channels#ticker-channel) channel. 
+Unlike the REST client, Websocket channels handle both authenticated and unauthenticated requests. 
+At the moment, most channels in the Websocket client are public and can be used without keys.
+
+```
+import time
+from coinbase.websocket import WSClient
+
+def on_message(msg):
+    print(msg)
+
+client = WSClient(on_message=on_message)
+
+client.open()
+client.ticker(product_ids=["BTC-USD"])
+
+time.sleep(10)
+
+client.ticker_unsubscribe(product_ids=["BTC-USD"])
+client.close()
+```
+
+_Full list of all public Websocket channels [here](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-channels)_
+
+_Rate limit details for Websocket channels [here](https://docs.cloud.coinbase.com/advanced-trade/docs/ws-rate-limits)_
+
+
+___
 ## Changelog
 For a detailed list of changes, see the [Changelog](https://github.com/coinbase/coinbase-advanced-py/blob/master/CHANGELOG.md).
 
+___
 ## Contributing
 
 If you've found a bug within this project, open an issue on this repo and add the "bug" label to it.
 If you would like to request a new feature, open an issue on this repo and add the "enhancement" label to it.
 Direct concerns or questions on the API to the [Advanced API Developer Forum](https://forums.coinbasecloud.dev/c/advanced-trade-api/20).
```

### Comparing `coinbase-advanced-py-1.2.2/coinbase_advanced_py.egg-info/SOURCES.txt` & `coinbase-advanced-py-1.3.0/coinbase_advanced_py.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,45 +4,45 @@
 coinbase/__init__.py
 coinbase/__version__.py
 coinbase/api_base.py
 coinbase/constants.py
 coinbase/jwt_generator.py
 coinbase/rest/__init__.py
 coinbase/rest/accounts.py
-coinbase/rest/common.py
 coinbase/rest/convert.py
 coinbase/rest/fees.py
 coinbase/rest/futures.py
 coinbase/rest/market_data.py
 coinbase/rest/orders.py
 coinbase/rest/payments.py
 coinbase/rest/perpetuals.py
 coinbase/rest/portfolios.py
 coinbase/rest/products.py
+coinbase/rest/public.py
 coinbase/rest/rest_base.py
 coinbase/websocket/__init__.py
 coinbase/websocket/channels.py
 coinbase/websocket/websocket_base.py
 coinbase_advanced_py.egg-info/PKG-INFO
 coinbase_advanced_py.egg-info/SOURCES.txt
 coinbase_advanced_py.egg-info/dependency_links.txt
 coinbase_advanced_py.egg-info/requires.txt
 coinbase_advanced_py.egg-info/top_level.txt
 tests/test_api_base.py
 tests/test_jwt_generator.py
 tests/rest/__init__.py
 tests/rest/test_accounts.py
-tests/rest/test_common.py
 tests/rest/test_convert.py
 tests/rest/test_fees.py
 tests/rest/test_futures.py
 tests/rest/test_market_data.py
 tests/rest/test_orders.py
 tests/rest/test_payments.py
 tests/rest/test_perpetuals.py
 tests/rest/test_portfolios.py
 tests/rest/test_products.py
+tests/rest/test_public.py
 tests/rest/test_rest_base.py
 tests/websocket/__init__.py
 tests/websocket/mock_ws_server.py
 tests/websocket/test_channels.py
 tests/websocket/test_websocket_base.py
```

### Comparing `coinbase-advanced-py-1.2.2/setup.py` & `coinbase-advanced-py-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/tests/rest/test_accounts.py` & `coinbase-advanced-py-1.3.0/tests/rest/test_accounts.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,19 +15,24 @@
 
         with Mocker() as m:
             m.request(
                 "GET",
                 "https://api.coinbase.com/api/v3/brokerage/accounts",
                 json=expected_response,
             )
-            accounts = client.get_accounts(limit=2, cursor="abcd")
+            accounts = client.get_accounts(
+                limit=2, cursor="abcd", retail_portfolio_id="portfolio1"
+            )
 
             captured_request = m.request_history[0]
 
-            self.assertEqual(captured_request.query, "limit=2&cursor=abcd")
+            self.assertEqual(
+                captured_request.query,
+                "limit=2&cursor=abcd&retail_portfolio_id=portfolio1",
+            )
             self.assertEqual(accounts, expected_response)
 
     def test_get_account(self):
         client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
 
         expected_response = {"uuid": "account1"}
```

### Comparing `coinbase-advanced-py-1.2.2/tests/rest/test_common.py` & `coinbase-advanced-py-1.3.0/tests/rest/test_fees.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 from requests_mock import Mocker
 
 from coinbase.rest import RESTClient
 
 from ..constants import TEST_API_KEY, TEST_API_SECRET
 
 
-class TimeTest(unittest.TestCase):
-    def test_get_time(self):
+class FeesTest(unittest.TestCase):
+    def test_get_transaction_summary(self):
         client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
 
-        expected_response = {"iso": "2022-01-01T00:00:00Z", "epoch": 1640995200}
+        expected_response = {"key_1": "value_1", "key_2": "value_2"}
 
         with Mocker() as m:
             m.request(
                 "GET",
-                "https://api.coinbase.com/api/v3/brokerage/time",
+                "https://api.coinbase.com/api/v3/brokerage/transaction_summary",
                 json=expected_response,
             )
-            time = client.get_unix_time()
+            summary = client.get_transaction_summary(
+                "product_type", "contract_expiry_type"
+            )
 
             captured_request = m.request_history[0]
-            captured_headers = captured_request.headers
 
-            self.assertEqual(captured_request.query, "")
-            self.assertEqual(time, expected_response)
-            self.assertNotIn("Authorization", captured_headers)
+            self.assertEqual(
+                captured_request.query,
+                "product_type=product_type&contract_expiry_type=contract_expiry_type",
+            )
+            self.assertEqual(summary, expected_response)
```

### Comparing `coinbase-advanced-py-1.2.2/tests/rest/test_convert.py` & `coinbase-advanced-py-1.3.0/tests/rest/test_convert.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/tests/rest/test_fees.py` & `coinbase-advanced-py-1.3.0/tests/rest/test_market_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,30 +3,52 @@
 from requests_mock import Mocker
 
 from coinbase.rest import RESTClient
 
 from ..constants import TEST_API_KEY, TEST_API_SECRET
 
 
-class FeesTest(unittest.TestCase):
-    def test_get_transaction_summary(self):
+class MarketDataTest(unittest.TestCase):
+    def test_get_candles(self):
         client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
 
         expected_response = {"key_1": "value_1", "key_2": "value_2"}
 
         with Mocker() as m:
             m.request(
                 "GET",
-                "https://api.coinbase.com/api/v3/brokerage/transaction_summary",
+                "https://api.coinbase.com/api/v3/brokerage/products/product_id_1/candles",
                 json=expected_response,
             )
-            summary = client.get_transaction_summary(
-                "product_type", "contract_expiry_type"
+            candles = client.get_candles(
+                "product_id_1", "1640995200", "1641081600", "FIVE_MINUTE"
             )
 
             captured_request = m.request_history[0]
 
             self.assertEqual(
                 captured_request.query,
-                "product_type=product_type&contract_expiry_type=contract_expiry_type",
+                "start=1640995200&end=1641081600&granularity=five_minute",
             )
-            self.assertEqual(summary, expected_response)
+            self.assertEqual(candles, expected_response)
+
+    def test_get_market_trades(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"key_1": "value_1", "key_2": "value_2"}
+
+        with Mocker() as m:
+            m.request(
+                "GET",
+                "https://api.coinbase.com/api/v3/brokerage/products/product_id/ticker",
+                json=expected_response,
+            )
+            trades = client.get_market_trades(
+                "product_id", 10, "1640995200", "1641081600"
+            )
+
+            captured_request = m.request_history[0]
+
+            self.assertEqual(
+                captured_request.query, "limit=10&start=1640995200&end=1641081600"
+            )
+            self.assertEqual(trades, expected_response)
```

### Comparing `coinbase-advanced-py-1.2.2/tests/rest/test_futures.py` & `coinbase-advanced-py-1.3.0/tests/rest/test_futures.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/tests/rest/test_orders.py` & `coinbase-advanced-py-1.3.0/tests/rest/test_orders.py`

 * *Files 20% similar despite different names*

```diff
@@ -469,14 +469,110 @@
                             "post_only": False,
                         }
                     },
                 },
             )
             self.assertEqual(order, expected_response)
 
+    def test_limit_order_fok(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders",
+                json=expected_response,
+            )
+            order = client.limit_order_fok(
+                "client_order_id_1", "product_id_1", "BUY", "1", "100"
+            )
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "client_order_id": "client_order_id_1",
+                    "product_id": "product_id_1",
+                    "side": "BUY",
+                    "order_configuration": {
+                        "limit_limit_fok": {"base_size": "1", "limit_price": "100"}
+                    },
+                },
+            )
+            self.assertEqual(order, expected_response)
+
+    def test_limit_order_fok_buy(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders",
+                json=expected_response,
+            )
+            order = client.limit_order_fok_buy(
+                "client_order_id_1", "product_id_1", "1", "100"
+            )
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "client_order_id": "client_order_id_1",
+                    "product_id": "product_id_1",
+                    "side": "BUY",
+                    "order_configuration": {
+                        "limit_limit_fok": {"base_size": "1", "limit_price": "100"}
+                    },
+                },
+            )
+            self.assertEqual(order, expected_response)
+
+    def test_limit_order_fok_sell(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders",
+                json=expected_response,
+            )
+            order = client.limit_order_fok_sell(
+                "client_order_id_1", "product_id_1", "1", "100"
+            )
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "client_order_id": "client_order_id_1",
+                    "product_id": "product_id_1",
+                    "side": "SELL",
+                    "order_configuration": {
+                        "limit_limit_fok": {"base_size": "1", "limit_price": "100"}
+                    },
+                },
+            )
+            self.assertEqual(order, expected_response)
+
     def test_stop_limit_order_gtc(self):
         client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
 
         expected_response = {"order_id": "1234"}
 
         with Mocker() as m:
             m.request(
@@ -729,14 +825,254 @@
                             "stop_direction": "STOP_DIRECTION_STOP_UP",
                         }
                     },
                 },
             )
             self.assertEqual(order, expected_response)
 
+    def test_trigger_bracket_order_gtc(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders",
+                json=expected_response,
+            )
+            order = client.trigger_bracket_order_gtc(
+                "client_order_id_1",
+                "product_id_1",
+                "BUY",
+                "1",
+                "100",
+                "90",
+            )
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "client_order_id": "client_order_id_1",
+                    "product_id": "product_id_1",
+                    "side": "BUY",
+                    "order_configuration": {
+                        "trigger_bracket_gtc": {
+                            "base_size": "1",
+                            "limit_price": "100",
+                            "stop_trigger_price": "90",
+                        }
+                    },
+                },
+            )
+            self.assertEqual(order, expected_response)
+
+    def test_trigger_bracket_order_gtc_buy(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders",
+                json=expected_response,
+            )
+            order = client.trigger_bracket_order_gtc_buy(
+                "client_order_id_1", "product_id_1", "1", "100", "90"
+            )
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "client_order_id": "client_order_id_1",
+                    "product_id": "product_id_1",
+                    "side": "BUY",
+                    "order_configuration": {
+                        "trigger_bracket_gtc": {
+                            "base_size": "1",
+                            "limit_price": "100",
+                            "stop_trigger_price": "90",
+                        }
+                    },
+                },
+            )
+            self.assertEqual(order, expected_response)
+
+    def test_trigger_bracket_order_gtc_sell(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders",
+                json=expected_response,
+            )
+            order = client.trigger_bracket_order_gtc_sell(
+                "client_order_id_1", "product_id_1", "1", "100", "90"
+            )
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "client_order_id": "client_order_id_1",
+                    "product_id": "product_id_1",
+                    "side": "SELL",
+                    "order_configuration": {
+                        "trigger_bracket_gtc": {
+                            "base_size": "1",
+                            "limit_price": "100",
+                            "stop_trigger_price": "90",
+                        }
+                    },
+                },
+            )
+            self.assertEqual(order, expected_response)
+
+    def test_trigger_bracket_order_gtd(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders",
+                json=expected_response,
+            )
+            order = client.trigger_bracket_order_gtd(
+                "client_order_id_1",
+                "product_id_1",
+                "BUY",
+                "1",
+                "100",
+                "90",
+                "2022-01-01T00:00:00Z",
+            )
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "client_order_id": "client_order_id_1",
+                    "product_id": "product_id_1",
+                    "side": "BUY",
+                    "order_configuration": {
+                        "trigger_bracket_gtd": {
+                            "base_size": "1",
+                            "limit_price": "100",
+                            "stop_trigger_price": "90",
+                            "end_time": "2022-01-01T00:00:00Z",
+                        }
+                    },
+                },
+            )
+            self.assertEqual(order, expected_response)
+
+    def test_trigger_bracket_order_gtd_buy(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders",
+                json=expected_response,
+            )
+            order = client.trigger_bracket_order_gtd_buy(
+                "client_order_id_1",
+                "product_id_1",
+                "1",
+                "100",
+                "90",
+                "2022-01-01T00:00:00Z",
+            )
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "client_order_id": "client_order_id_1",
+                    "product_id": "product_id_1",
+                    "side": "BUY",
+                    "order_configuration": {
+                        "trigger_bracket_gtd": {
+                            "base_size": "1",
+                            "limit_price": "100",
+                            "stop_trigger_price": "90",
+                            "end_time": "2022-01-01T00:00:00Z",
+                        }
+                    },
+                },
+            )
+            self.assertEqual(order, expected_response)
+
+    def test_trigger_bracket_order_gtd_sell(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders",
+                json=expected_response,
+            )
+            order = client.trigger_bracket_order_gtd_sell(
+                "client_order_id_1",
+                "product_id_1",
+                "1",
+                "100",
+                "90",
+                "2022-01-01T00:00:00Z",
+            )
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "client_order_id": "client_order_id_1",
+                    "product_id": "product_id_1",
+                    "side": "SELL",
+                    "order_configuration": {
+                        "trigger_bracket_gtd": {
+                            "base_size": "1",
+                            "limit_price": "100",
+                            "stop_trigger_price": "90",
+                            "end_time": "2022-01-01T00:00:00Z",
+                        }
+                    },
+                },
+            )
+            self.assertEqual(order, expected_response)
+
     def test_get_order(self):
         client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
 
         expected_response = {"order_id": "1234"}
 
         with Mocker() as m:
             m.request(
@@ -1330,14 +1666,107 @@
                     },
                     "is_max": False,
                     "skip_fcm_risk_check": False,
                 },
             )
             self.assertEqual(preview, expected_response)
 
+    def test_preview_limit_order_fok(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders/preview",
+                json=expected_response,
+            )
+            preview = client.preview_limit_order_fok("product_id_1", "BUY", "1", "100")
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "product_id": "product_id_1",
+                    "side": "BUY",
+                    "order_configuration": {
+                        "limit_limit_fok": {"base_size": "1", "limit_price": "100"}
+                    },
+                    "is_max": False,
+                    "skip_fcm_risk_check": False,
+                },
+            )
+            self.assertEqual(preview, expected_response)
+
+    def test_preview_limit_order_fok_buy(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders/preview",
+                json=expected_response,
+            )
+            preview = client.preview_limit_order_fok_buy("product_id_1", "1", "100")
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "product_id": "product_id_1",
+                    "side": "BUY",
+                    "order_configuration": {
+                        "limit_limit_fok": {"base_size": "1", "limit_price": "100"}
+                    },
+                    "is_max": False,
+                    "skip_fcm_risk_check": False,
+                },
+            )
+            self.assertEqual(preview, expected_response)
+
+    def test_preview_limit_order_fok_sell(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders/preview",
+                json=expected_response,
+            )
+            preview = client.preview_limit_order_fok_sell("product_id_1", "1", "100")
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "product_id": "product_id_1",
+                    "side": "SELL",
+                    "order_configuration": {
+                        "limit_limit_fok": {"base_size": "1", "limit_price": "100"}
+                    },
+                    "is_max": False,
+                    "skip_fcm_risk_check": False,
+                },
+            )
+            self.assertEqual(preview, expected_response)
+
     def test_preview_stop_limit_order_gtc(self):
         client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
 
         expected_response = {"order_id": "1234"}
 
         with Mocker() as m:
             m.request(
@@ -1589,7 +2018,245 @@
                         }
                     },
                     "is_max": False,
                     "skip_fcm_risk_check": False,
                 },
             )
             self.assertEqual(preview, expected_response)
+
+    def test_preview_trigger_bracket_order_gtc(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders/preview",
+                json=expected_response,
+            )
+            preview = client.preview_trigger_bracket_order_gtc(
+                "product_id_1",
+                "BUY",
+                "1",
+                "100",
+                "90",
+            )
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "product_id": "product_id_1",
+                    "side": "BUY",
+                    "order_configuration": {
+                        "trigger_bracket_gtc": {
+                            "base_size": "1",
+                            "limit_price": "100",
+                            "stop_trigger_price": "90",
+                        }
+                    },
+                    "is_max": False,
+                    "skip_fcm_risk_check": False,
+                },
+            )
+            self.assertEqual(preview, expected_response)
+
+    def test_preview_trigger_bracket_order_gtc_buy(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders/preview",
+                json=expected_response,
+            )
+            preview = client.preview_trigger_bracket_order_gtc_buy(
+                "product_id_1", "1", "100", "90"
+            )
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "product_id": "product_id_1",
+                    "side": "BUY",
+                    "order_configuration": {
+                        "trigger_bracket_gtc": {
+                            "base_size": "1",
+                            "limit_price": "100",
+                            "stop_trigger_price": "90",
+                        }
+                    },
+                    "is_max": False,
+                    "skip_fcm_risk_check": False,
+                },
+            )
+            self.assertEqual(preview, expected_response)
+
+    def test_preview_trigger_bracket_gtc_sell(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders/preview",
+                json=expected_response,
+            )
+            preview = client.preview_trigger_bracket_order_gtc_sell(
+                "product_id_1", "1", "100", "90"
+            )
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "product_id": "product_id_1",
+                    "side": "SELL",
+                    "order_configuration": {
+                        "trigger_bracket_gtc": {
+                            "base_size": "1",
+                            "limit_price": "100",
+                            "stop_trigger_price": "90",
+                        }
+                    },
+                    "is_max": False,
+                    "skip_fcm_risk_check": False,
+                },
+            )
+            self.assertEqual(preview, expected_response)
+
+    def test_preview_trigger_bracket_order_gtd(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders/preview",
+                json=expected_response,
+            )
+            preview = client.preview_trigger_bracket_order_gtd(
+                "product_id_1",
+                "BUY",
+                "1",
+                "100",
+                "90",
+                "2022-01-01T00:00:00Z",
+            )
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "product_id": "product_id_1",
+                    "side": "BUY",
+                    "order_configuration": {
+                        "trigger_bracket_gtd": {
+                            "base_size": "1",
+                            "limit_price": "100",
+                            "stop_trigger_price": "90",
+                            "end_time": "2022-01-01T00:00:00Z",
+                        }
+                    },
+                    "is_max": False,
+                    "skip_fcm_risk_check": False,
+                },
+            )
+            self.assertEqual(preview, expected_response)
+
+    def test_preview_trigger_bracket_order_gtd_buy(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders/preview",
+                json=expected_response,
+            )
+            preview = client.preview_trigger_bracket_order_gtd_buy(
+                "product_id_1",
+                "1",
+                "100",
+                "90",
+                "2022-01-01T00:00:00Z",
+            )
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "product_id": "product_id_1",
+                    "side": "BUY",
+                    "order_configuration": {
+                        "trigger_bracket_gtd": {
+                            "base_size": "1",
+                            "limit_price": "100",
+                            "stop_trigger_price": "90",
+                            "end_time": "2022-01-01T00:00:00Z",
+                        }
+                    },
+                    "is_max": False,
+                    "skip_fcm_risk_check": False,
+                },
+            )
+            self.assertEqual(preview, expected_response)
+
+    def test_preview_trigger_bracket_gtd_sell(self):
+        client = RESTClient(TEST_API_KEY, TEST_API_SECRET)
+
+        expected_response = {"order_id": "1234"}
+
+        with Mocker() as m:
+            m.request(
+                "POST",
+                "https://api.coinbase.com/api/v3/brokerage/orders/preview",
+                json=expected_response,
+            )
+            preview = client.preview_trigger_bracket_order_gtd_sell(
+                "product_id_1", "1", "100", "90", "2022-01-01T00:00:00Z"
+            )
+
+            captured_request = m.request_history[0]
+            captured_json = captured_request.json()
+
+            self.assertEqual(captured_request.query, "")
+            self.assertEqual(
+                captured_json,
+                {
+                    "product_id": "product_id_1",
+                    "side": "SELL",
+                    "order_configuration": {
+                        "trigger_bracket_gtd": {
+                            "base_size": "1",
+                            "limit_price": "100",
+                            "stop_trigger_price": "90",
+                            "end_time": "2022-01-01T00:00:00Z",
+                        }
+                    },
+                    "is_max": False,
+                    "skip_fcm_risk_check": False,
+                },
+            )
+            self.assertEqual(preview, expected_response)
```

### Comparing `coinbase-advanced-py-1.2.2/tests/rest/test_payments.py` & `coinbase-advanced-py-1.3.0/tests/rest/test_payments.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/tests/rest/test_perpetuals.py` & `coinbase-advanced-py-1.3.0/tests/rest/test_perpetuals.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/tests/rest/test_portfolios.py` & `coinbase-advanced-py-1.3.0/tests/rest/test_portfolios.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/tests/rest/test_products.py` & `coinbase-advanced-py-1.3.0/tests/rest/test_products.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/tests/rest/test_rest_base.py` & `coinbase-advanced-py-1.3.0/tests/rest/test_rest_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,39 @@
                 )
 
                 client.get("/api/v3/brokerage/time", public=True)
 
                 captured_request = m.request_history[0]
                 captured_headers = captured_request.headers
 
+                self.assertIn("Authorization", captured_headers)
+                self.assertTrue("User-Agent" in captured_headers)
+                self.assertEqual(
+                    captured_headers["User-Agent"],
+                    "coinbase-advanced-py/" + __version__,
+                )
+
+    def test_get_public_unauthenticated(self):
+        client = RESTClient()
+
+        with Mocker() as m:
+            expected_response = {"iso": "2022-01-01T00:00:00Z", "epoch": 1640995200}
+
+            with Mocker() as m:
+                m.request(
+                    "GET",
+                    "https://api.coinbase.com/api/v3/brokerage/time",
+                    json=expected_response,
+                )
+
+                client.get("/api/v3/brokerage/time", public=True)
+
+                captured_request = m.request_history[0]
+                captured_headers = captured_request.headers
+
                 self.assertNotIn("Authorization", captured_headers)
                 self.assertTrue("User-Agent" in captured_headers)
                 self.assertEqual(
                     captured_headers["User-Agent"],
                     "coinbase-advanced-py/" + __version__,
                 )
```

### Comparing `coinbase-advanced-py-1.2.2/tests/test_api_base.py` & `coinbase-advanced-py-1.3.0/tests/test_api_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 
 from .constants import TEST_API_KEY, TEST_API_SECRET
 
 
 class RestBaseTest(unittest.TestCase):
     def test_no_api_key(self):
         with self.assertRaises(Exception):
-            APIBase(None, None)
-
-        with self.assertRaises(Exception):
             APIBase("test_key", None)
 
     def test_key_api_key_vars(self):
         try:
             APIBase(api_key=TEST_API_KEY, api_secret=TEST_API_SECRET)
         except Exception as e:
             self.fail(f"An unexpected exception occurred: {e}")
```

### Comparing `coinbase-advanced-py-1.2.2/tests/test_jwt_generator.py` & `coinbase-advanced-py-1.3.0/tests/test_jwt_generator.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/tests/websocket/mock_ws_server.py` & `coinbase-advanced-py-1.3.0/tests/websocket/mock_ws_server.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/tests/websocket/test_channels.py` & `coinbase-advanced-py-1.3.0/tests/websocket/test_channels.py`

 * *Files identical despite different names*

### Comparing `coinbase-advanced-py-1.2.2/tests/websocket/test_websocket_base.py` & `coinbase-advanced-py-1.3.0/tests/websocket/test_websocket_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 import json
 import unittest
 from unittest.mock import AsyncMock, patch
 
 import websockets
 
 from coinbase.constants import SUBSCRIBE_MESSAGE_TYPE, UNSUBSCRIBE_MESSAGE_TYPE
-from coinbase.websocket import (
-    WSClient,
-    WSClientConnectionClosedException,
-    WSClientException,
-)
+from coinbase.websocket import WSClient, WSClientConnectionClosedException
 
 from ..constants import TEST_API_KEY, TEST_API_SECRET
 from . import mock_ws_server
 
 
 class WSBaseTest(unittest.IsolatedAsyncioTestCase):
     async def asyncSetUp(self):
@@ -41,14 +37,20 @@
         self.ws = WSClient(
             TEST_API_KEY,
             TEST_API_SECRET,
             on_message=self.on_message_mock,
             retry=False,
         )
 
+        # initialize public client
+        self.ws_public = WSClient(
+            on_message=self.on_message_mock,
+            retry=False,
+        )
+
     @patch("websockets.connect", new_callable=AsyncMock)
     def test_open_twice(self, mock_connect):
         # assert you cannot open a websocket client twice consecutively
         mock_connect.return_value = self.mock_websocket
 
         self.ws.open()
         self.assertIsNotNone(self.ws.websocket)
@@ -102,14 +104,30 @@
         self.on_message_mock.assert_called_once_with("test message")
 
         # close
         self.ws.close()
         self.mock_websocket.close.assert_awaited_once()
 
     @patch("websockets.connect", new_callable=AsyncMock)
+    def test_open_and_close_unauthenticated(self, mock_connect):
+        # assert you can open and close a websocket client
+        mock_connect.return_value = self.mock_websocket
+
+        # open
+        self.ws_public.open()
+        self.assertIsNotNone(self.ws_public.websocket)
+
+        # assert on_message received
+        self.on_message_mock.assert_called_once_with("test message")
+
+        # close
+        self.ws_public.close()
+        self.mock_websocket.close.assert_awaited_once()
+
+    @patch("websockets.connect", new_callable=AsyncMock)
     def test_reopen(self, mock_connect):
         # assert you can open, close, reopen and close a websocket client
         mock_connect.return_value = self.mock_websocket
 
         # open
         self.ws.open()
         self.assertIsNotNone(self.ws.websocket)
@@ -157,14 +175,51 @@
         self.assertEqual(unsubscribe["channel"], "ticker")
 
         # close
         self.ws.close()
         self.mock_websocket.close.assert_awaited_once()
 
     @patch("websockets.connect", new_callable=AsyncMock)
+    def test_subscribe_and_unsubscribe_channel_unauthenticated(self, mock_connect):
+        # assert you can subscribe and unsubscribe to a channel
+        mock_connect.return_value = self.mock_websocket
+
+        # open
+        self.ws_public.open()
+        self.assertIsNotNone(self.ws_public.websocket)
+
+        # subscribe
+        self.ws_public.subscribe(
+            product_ids=["BTC-USD", "ETH-USD"], channels=["ticker"]
+        )
+        self.mock_websocket.send.assert_awaited_once()
+
+        # assert subscribe message
+        subscribe = json.loads(self.mock_websocket.send.call_args_list[0][0][0])
+        self.assertEqual(subscribe["type"], SUBSCRIBE_MESSAGE_TYPE)
+        self.assertEqual(subscribe["product_ids"], ["BTC-USD", "ETH-USD"])
+        self.assertEqual(subscribe["channel"], "ticker")
+
+        # unsubscribe
+        self.ws_public.unsubscribe(
+            product_ids=["BTC-USD", "ETH-USD"], channels=["ticker"]
+        )
+        self.assertEqual(self.mock_websocket.send.await_count, 2)
+
+        # assert unsubscribe message
+        unsubscribe = json.loads(self.mock_websocket.send.call_args_list[1][0][0])
+        self.assertEqual(unsubscribe["type"], UNSUBSCRIBE_MESSAGE_TYPE)
+        self.assertEqual(unsubscribe["product_ids"], ["BTC-USD", "ETH-USD"])
+        self.assertEqual(unsubscribe["channel"], "ticker")
+
+        # close
+        self.ws_public.close()
+        self.mock_websocket.close.assert_awaited_once()
+
+    @patch("websockets.connect", new_callable=AsyncMock)
     def test_subscribe_and_unsubscribe_channels(self, mock_connect):
         # assert you can subscribe and unsubscribe to multiple channels
         mock_connect.return_value = self.mock_websocket
 
         # open
         self.ws.open()
         self.assertIsNotNone(self.ws.websocket)
@@ -204,14 +259,61 @@
         self.assertEqual(unsubscribe_2["channel"], "level2")
 
         # close
         self.ws.close()
         self.mock_websocket.close.assert_awaited_once()
 
     @patch("websockets.connect", new_callable=AsyncMock)
+    def test_subscribe_and_unsubscribe_channels_unauthenticated(self, mock_connect):
+        # assert you can subscribe and unsubscribe to multiple channels
+        mock_connect.return_value = self.mock_websocket
+
+        # open
+        self.ws_public.open()
+        self.assertIsNotNone(self.ws_public.websocket)
+
+        # subscribe
+        self.ws_public.subscribe(
+            product_ids=["BTC-USD", "ETH-USD"], channels=["ticker", "level2"]
+        )
+        self.assertEqual(self.mock_websocket.send.await_count, 2)
+
+        # assert subscribe messages
+        subscribe_1 = json.loads(self.mock_websocket.send.call_args_list[0][0][0])
+        self.assertEqual(subscribe_1["type"], SUBSCRIBE_MESSAGE_TYPE)
+        self.assertEqual(subscribe_1["product_ids"], ["BTC-USD", "ETH-USD"])
+        self.assertEqual(subscribe_1["channel"], "ticker")
+
+        subscribe_2 = json.loads(self.mock_websocket.send.call_args_list[1][0][0])
+        self.assertEqual(subscribe_2["type"], SUBSCRIBE_MESSAGE_TYPE)
+        self.assertEqual(subscribe_2["product_ids"], ["BTC-USD", "ETH-USD"])
+        self.assertEqual(subscribe_2["channel"], "level2")
+
+        # unsubscribe
+        self.ws_public.unsubscribe(
+            product_ids=["BTC-USD", "ETH-USD"], channels=["ticker", "level2"]
+        )
+        self.assertEqual(self.mock_websocket.send.await_count, 4)
+
+        # assert unsubscribe messages
+        unsubscribe_1 = json.loads(self.mock_websocket.send.call_args_list[2][0][0])
+        self.assertEqual(unsubscribe_1["type"], UNSUBSCRIBE_MESSAGE_TYPE)
+        self.assertEqual(unsubscribe_1["product_ids"], ["BTC-USD", "ETH-USD"])
+        self.assertEqual(unsubscribe_1["channel"], "ticker")
+
+        unsubscribe_2 = json.loads(self.mock_websocket.send.call_args_list[3][0][0])
+        self.assertEqual(unsubscribe_2["type"], UNSUBSCRIBE_MESSAGE_TYPE)
+        self.assertEqual(unsubscribe_2["product_ids"], ["BTC-USD", "ETH-USD"])
+        self.assertEqual(unsubscribe_2["channel"], "level2")
+
+        # close
+        self.ws_public.close()
+        self.mock_websocket.close.assert_awaited_once()
+
+    @patch("websockets.connect", new_callable=AsyncMock)
     async def test_open_and_close_async(self, mock_connect):
         # assert you can open and close a websocket client
         mock_connect.return_value = self.mock_websocket
 
         # open
         await self.ws.open_async()
         self.assertIsNotNone(self.ws.websocket)
@@ -221,14 +323,31 @@
         self.on_message_mock.assert_called_once_with("test message")
 
         # close
         await self.ws.close_async()
         self.mock_websocket.close.assert_awaited_once()
 
     @patch("websockets.connect", new_callable=AsyncMock)
+    async def test_open_and_close_async_unauthenticated(self, mock_connect):
+        # assert you can open and close a websocket client
+        mock_connect.return_value = self.mock_websocket
+
+        # open
+        await self.ws_public.open_async()
+        self.assertIsNotNone(self.ws_public.websocket)
+
+        # assert on_message received
+        await self.message_received_event.wait()
+        self.on_message_mock.assert_called_once_with("test message")
+
+        # close
+        await self.ws_public.close_async()
+        self.mock_websocket.close.assert_awaited_once()
+
+    @patch("websockets.connect", new_callable=AsyncMock)
     async def test_reopen_async(self, mock_connect):
         # assert you can open, close, reopen and close a websocket client
         mock_connect.return_value = self.mock_websocket
 
         # open
         await self.ws.open_async()
         self.assertIsNotNone(self.ws.websocket)
@@ -279,14 +398,62 @@
         self.assertEqual(unsubscribe["product_ids"], ["BTC-USD", "ETH-USD"])
         self.assertEqual(unsubscribe["channel"], "ticker")
 
         # close
         await self.ws.close_async()
         self.mock_websocket.close.assert_awaited_once()
 
+    @patch("websockets.connect", new_callable=AsyncMock)
+    async def test_subscribe_and_unsubscribes_channel_async_unauthenticated(
+        self, mock_connect
+    ):
+        # assert you can subscribe and unsubscribe to a channel
+        mock_connect.return_value = self.mock_websocket
+
+        # open
+        await self.ws_public.open_async()
+        self.assertIsNotNone(self.ws_public.websocket)
+
+        # subscribe
+        await self.ws_public.subscribe_async(
+            product_ids=["BTC-USD", "ETH-USD"], channels=["ticker"]
+        )
+        self.mock_websocket.send.assert_awaited_once()
+
+        # assert subscribe message
+        subscribe = json.loads(self.mock_websocket.send.call_args_list[0][0][0])
+        self.assertEqual(subscribe["type"], SUBSCRIBE_MESSAGE_TYPE)
+        self.assertEqual(subscribe["product_ids"], ["BTC-USD", "ETH-USD"])
+        self.assertEqual(subscribe["channel"], "ticker")
+
+        # unsubscribe
+        await self.ws_public.unsubscribe_async(
+            product_ids=["BTC-USD", "ETH-USD"], channels=["ticker"]
+        )
+        self.assertEqual(self.mock_websocket.send.await_count, 2)
+
+        # assert unsubscribe message
+        unsubscribe = json.loads(self.mock_websocket.send.call_args_list[1][0][0])
+        self.assertEqual(unsubscribe["type"], UNSUBSCRIBE_MESSAGE_TYPE)
+        self.assertEqual(unsubscribe["product_ids"], ["BTC-USD", "ETH-USD"])
+        self.assertEqual(unsubscribe["channel"], "ticker")
+
+        # close
+        await self.ws_public.close_async()
+        self.mock_websocket.close.assert_awaited_once()
+
+    def test_err_calling_private_unauthenticated(self):
+        # open
+        self.ws_public.open()
+        self.assertIsNotNone(self.ws_public.websocket)
+
+        # assert you cannot call a private endpoint unauthenticated
+        with self.assertRaises(Exception):
+            self.ws.subscribe(product_ids=["BTC-USD"], channels=["user"])
+
 
 class WSDisconnectionTests(unittest.IsolatedAsyncioTestCase):
     # tests that run against a mock websocket server to simulate disconnections
     async def mock_send(self, message):
         self.messages_queue.put_nowait(message)
 
     async def asyncSetUp(self):
```

