# Comparing `tmp/ibind-0.0.7.tar.gz` & `tmp/ibind-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibind-0.0.7.tar", last modified: Fri May  3 08:36:06 2024, max compression
+gzip compressed data, was "ibind-0.1.0.tar", last modified: Mon May  6 12:43:09 2024, max compression
```

## Comparing `ibind-0.0.7.tar` & `ibind-0.1.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 08:36:06.553532 ibind-0.0.7/
--rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibind-0.0.7/LICENSE
--rw-rw-rw-   0        0        0    22197 2024-05-03 08:36:06.550495 ibind-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     8112 2024-05-03 07:16:22.000000 ibind-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 08:36:06.391856 ibind-0.0.7/ibind/
--rw-rw-rw-   0        0        0     1062 2024-05-02 11:52:19.000000 ibind-0.0.7/ibind/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:36:06.428833 ibind-0.0.7/ibind/base/
--rw-rw-rw-   0        0        0        0 2024-04-04 04:03:06.000000 ibind-0.0.7/ibind/base/__init__.py
--rw-rw-rw-   0        0        0     5286 2024-05-02 07:49:30.000000 ibind-0.0.7/ibind/base/queue_controller.py
--rw-rw-rw-   0        0        0     8555 2024-05-03 06:26:53.000000 ibind-0.0.7/ibind/base/rest_client.py
--rw-rw-rw-   0        0        0    16433 2024-05-03 05:09:05.000000 ibind-0.0.7/ibind/base/subscription_controller.py
--rw-rw-rw-   0        0        0    18799 2024-05-02 07:52:05.000000 ibind-0.0.7/ibind/base/ws_client.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:36:06.446290 ibind-0.0.7/ibind/client/
--rw-rw-rw-   0        0        0        0 2024-04-03 12:59:53.000000 ibind-0.0.7/ibind/client/__init__.py
--rw-rw-rw-   0        0        0     3653 2024-05-03 03:15:23.000000 ibind-0.0.7/ibind/client/ibkr_client.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:36:06.477922 ibind-0.0.7/ibind/client/ibkr_client_mixins/
--rw-rw-rw-   0        0        0        0 2024-04-04 04:14:49.000000 ibind-0.0.7/ibind/client/ibkr_client_mixins/__init__.py
--rw-rw-rw-   0        0        0     3400 2024-05-02 04:33:53.000000 ibind-0.0.7/ibind/client/ibkr_client_mixins/accounts_mixin.py
--rw-rw-rw-   0        0        0    16132 2024-04-25 11:38:46.000000 ibind-0.0.7/ibind/client/ibkr_client_mixins/contract_mixin.py
--rw-rw-rw-   0        0        0    12508 2024-05-02 07:59:06.000000 ibind-0.0.7/ibind/client/ibkr_client_mixins/marketdata_mixin.py
--rw-rw-rw-   0        0        0    10477 2024-05-02 10:28:02.000000 ibind-0.0.7/ibind/client/ibkr_client_mixins/order_mixin.py
--rw-rw-rw-   0        0        0     9585 2024-05-02 10:28:35.000000 ibind-0.0.7/ibind/client/ibkr_client_mixins/portfolio_mixin.py
--rw-rw-rw-   0        0        0     4220 2024-05-02 10:28:35.000000 ibind-0.0.7/ibind/client/ibkr_client_mixins/scanner_mixin.py
--rw-rw-rw-   0        0        0     4611 2024-05-02 10:28:43.000000 ibind-0.0.7/ibind/client/ibkr_client_mixins/session_mixin.py
--rw-rw-rw-   0        0        0     2343 2024-05-02 10:30:13.000000 ibind-0.0.7/ibind/client/ibkr_client_mixins/watchlist_mixin.py
--rw-rw-rw-   0        0        0    12413 2024-04-24 12:43:26.000000 ibind-0.0.7/ibind/client/ibkr_definitions.py
--rw-rw-rw-   0        0        0    16278 2024-05-02 06:20:14.000000 ibind-0.0.7/ibind/client/ibkr_utils.py
--rw-rw-rw-   0        0        0    28501 2024-05-03 06:27:53.000000 ibind-0.0.7/ibind/client/ibkr_ws_client.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:36:06.490499 ibind-0.0.7/ibind/support/
--rw-rw-rw-   0        0        0        0 2024-04-03 13:00:28.000000 ibind-0.0.7/ibind/support/__init__.py
--rw-rw-rw-   0        0        0      227 2024-04-01 07:18:14.000000 ibind-0.0.7/ibind/support/errors.py
--rw-rw-rw-   0        0        0     5612 2024-05-02 10:37:05.000000 ibind-0.0.7/ibind/support/logs.py
--rw-rw-rw-   0        0        0    11297 2024-05-03 05:07:31.000000 ibind-0.0.7/ibind/support/py_utils.py
--rw-rw-rw-   0        0        0     2035 2024-04-25 10:00:26.000000 ibind-0.0.7/ibind/var.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:36:06.547493 ibind-0.0.7/ibind.egg-info/
--rw-rw-rw-   0        0        0    22197 2024-05-03 08:36:06.000000 ibind-0.0.7/ibind.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1595 2024-05-03 08:36:06.000000 ibind-0.0.7/ibind.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 08:36:06.000000 ibind-0.0.7/ibind.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-03 08:36:06.000000 ibind-0.0.7/ibind.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-03 08:36:06.000000 ibind-0.0.7/ibind.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1038 2024-05-03 08:35:52.000000 ibind-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       86 2024-05-03 08:36:06.556500 ibind-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      225 2024-05-02 11:52:19.000000 ibind-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:36:06.497470 ibind-0.0.7/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:08.000000 ibind-0.0.7/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:36:06.500496 ibind-0.0.7/test/integration/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.7/test/integration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:36:06.514498 ibind-0.0.7/test/integration/base/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:37:06.000000 ibind-0.0.7/test/integration/base/__init__.py
--rw-rw-rw-   0        0        0     3714 2024-04-03 12:45:17.000000 ibind-0.0.7/test/integration/base/test_rest_client_i.py
--rw-rw-rw-   0        0        0    11025 2024-04-24 10:05:09.000000 ibind-0.0.7/test/integration/base/test_websocket_client_i.py
--rw-rw-rw-   0        0        0     1477 2023-12-13 15:29:14.000000 ibind-0.0.7/test/integration/base/websocketapp_mock.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:36:06.531469 ibind-0.0.7/test/integration/client/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:57:40.000000 ibind-0.0.7/test/integration/client/__init__.py
--rw-rw-rw-   0        0        0    39617 2024-04-01 08:07:19.000000 ibind-0.0.7/test/integration/client/ibkr_responses.py
--rw-rw-rw-   0        0        0    14441 2024-04-25 11:38:46.000000 ibind-0.0.7/test/integration/client/test_ibkr_client_i.py
--rw-rw-rw-   0        0        0    11825 2024-04-03 12:28:11.000000 ibind-0.0.7/test/integration/client/test_ibkr_utils_i.py
--rw-rw-rw-   0        0        0    19149 2024-05-03 06:23:26.000000 ibind-0.0.7/test/integration/client/test_ibkr_ws_client_i.py
--rw-rw-rw-   0        0        0     8874 2024-04-03 12:27:51.000000 ibind-0.0.7/test/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:36:06.535497 ibind-0.0.7/test/unit/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.7/test/unit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 08:36:06.542479 ibind-0.0.7/test/unit/support/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:45:52.000000 ibind-0.0.7/test/unit/support/__init__.py
--rw-rw-rw-   0        0        0     4517 2024-04-03 12:30:12.000000 ibind-0.0.7/test/unit/support/test_py_utils_u.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.663785 ibind-0.1.0/
+-rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibind-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0    22426 2024-05-06 12:43:09.661766 ibind-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8341 2024-05-06 12:41:34.000000 ibind-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.461540 ibind-0.1.0/ibind/
+-rw-rw-rw-   0        0        0     1062 2024-05-02 11:52:19.000000 ibind-0.1.0/ibind/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.505550 ibind-0.1.0/ibind/base/
+-rw-rw-rw-   0        0        0        0 2024-04-04 04:03:06.000000 ibind-0.1.0/ibind/base/__init__.py
+-rw-rw-rw-   0        0        0     5286 2024-05-02 07:49:30.000000 ibind-0.1.0/ibind/base/queue_controller.py
+-rw-rw-rw-   0        0        0     8555 2024-05-03 06:26:53.000000 ibind-0.1.0/ibind/base/rest_client.py
+-rw-rw-rw-   0        0        0    16433 2024-05-03 05:09:05.000000 ibind-0.1.0/ibind/base/subscription_controller.py
+-rw-rw-rw-   0        0        0    18799 2024-05-02 07:52:05.000000 ibind-0.1.0/ibind/base/ws_client.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.526561 ibind-0.1.0/ibind/client/
+-rw-rw-rw-   0        0        0        0 2024-04-03 12:59:53.000000 ibind-0.1.0/ibind/client/__init__.py
+-rw-rw-rw-   0        0        0     3653 2024-05-03 03:15:23.000000 ibind-0.1.0/ibind/client/ibkr_client.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.568673 ibind-0.1.0/ibind/client/ibkr_client_mixins/
+-rw-rw-rw-   0        0        0        0 2024-04-04 04:14:49.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/__init__.py
+-rw-rw-rw-   0        0        0     3400 2024-05-02 04:33:53.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/accounts_mixin.py
+-rw-rw-rw-   0        0        0    16134 2024-05-03 09:06:05.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/contract_mixin.py
+-rw-rw-rw-   0        0        0    12508 2024-05-02 07:59:06.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/marketdata_mixin.py
+-rw-rw-rw-   0        0        0    10477 2024-05-02 10:28:02.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/order_mixin.py
+-rw-rw-rw-   0        0        0     9585 2024-05-02 10:28:35.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/portfolio_mixin.py
+-rw-rw-rw-   0        0        0     4220 2024-05-02 10:28:35.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/scanner_mixin.py
+-rw-rw-rw-   0        0        0     4611 2024-05-02 10:28:43.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/session_mixin.py
+-rw-rw-rw-   0        0        0     2343 2024-05-02 10:30:13.000000 ibind-0.1.0/ibind/client/ibkr_client_mixins/watchlist_mixin.py
+-rw-rw-rw-   0        0        0    12413 2024-04-24 12:43:26.000000 ibind-0.1.0/ibind/client/ibkr_definitions.py
+-rw-rw-rw-   0        0        0    16278 2024-05-02 06:20:14.000000 ibind-0.1.0/ibind/client/ibkr_utils.py
+-rw-rw-rw-   0        0        0    28501 2024-05-03 06:27:53.000000 ibind-0.1.0/ibind/client/ibkr_ws_client.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.586673 ibind-0.1.0/ibind/support/
+-rw-rw-rw-   0        0        0        0 2024-04-03 13:00:28.000000 ibind-0.1.0/ibind/support/__init__.py
+-rw-rw-rw-   0        0        0      227 2024-04-01 07:18:14.000000 ibind-0.1.0/ibind/support/errors.py
+-rw-rw-rw-   0        0        0     5612 2024-05-02 10:37:05.000000 ibind-0.1.0/ibind/support/logs.py
+-rw-rw-rw-   0        0        0    11297 2024-05-03 05:07:31.000000 ibind-0.1.0/ibind/support/py_utils.py
+-rw-rw-rw-   0        0        0     2035 2024-04-25 10:00:26.000000 ibind-0.1.0/ibind/var.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.657418 ibind-0.1.0/ibind.egg-info/
+-rw-rw-rw-   0        0        0    22426 2024-05-06 12:43:09.000000 ibind-0.1.0/ibind.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1595 2024-05-06 12:43:09.000000 ibind-0.1.0/ibind.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 12:43:09.000000 ibind-0.1.0/ibind.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-06 12:43:09.000000 ibind-0.1.0/ibind.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-06 12:43:09.000000 ibind-0.1.0/ibind.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1038 2024-05-06 12:42:22.000000 ibind-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2024-05-06 12:43:09.665820 ibind-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      225 2024-05-02 11:52:19.000000 ibind-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.594672 ibind-0.1.0/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:08.000000 ibind-0.1.0/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.598673 ibind-0.1.0/test/integration/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.1.0/test/integration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.615672 ibind-0.1.0/test/integration/base/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:37:06.000000 ibind-0.1.0/test/integration/base/__init__.py
+-rw-rw-rw-   0        0        0     3714 2024-04-03 12:45:17.000000 ibind-0.1.0/test/integration/base/test_rest_client_i.py
+-rw-rw-rw-   0        0        0    11025 2024-04-24 10:05:09.000000 ibind-0.1.0/test/integration/base/test_websocket_client_i.py
+-rw-rw-rw-   0        0        0     1477 2023-12-13 15:29:14.000000 ibind-0.1.0/test/integration/base/websocketapp_mock.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.639672 ibind-0.1.0/test/integration/client/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:57:40.000000 ibind-0.1.0/test/integration/client/__init__.py
+-rw-rw-rw-   0        0        0    39617 2024-04-01 08:07:19.000000 ibind-0.1.0/test/integration/client/ibkr_responses.py
+-rw-rw-rw-   0        0        0    14441 2024-04-25 11:38:46.000000 ibind-0.1.0/test/integration/client/test_ibkr_client_i.py
+-rw-rw-rw-   0        0        0    11825 2024-04-03 12:28:11.000000 ibind-0.1.0/test/integration/client/test_ibkr_utils_i.py
+-rw-rw-rw-   0        0        0    19149 2024-05-03 06:23:26.000000 ibind-0.1.0/test/integration/client/test_ibkr_ws_client_i.py
+-rw-rw-rw-   0        0        0     8874 2024-04-03 12:27:51.000000 ibind-0.1.0/test/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.643687 ibind-0.1.0/test/unit/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.1.0/test/unit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:43:09.651692 ibind-0.1.0/test/unit/support/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:45:52.000000 ibind-0.1.0/test/unit/support/__init__.py
+-rw-rw-rw-   0        0        0     4517 2024-04-03 12:30:12.000000 ibind-0.1.0/test/unit/support/test_py_utils_u.py
```

### Comparing `ibind-0.0.7/LICENSE` & `ibind-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/PKG-INFO` & `ibind-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibind
-Version: 0.0.7
+Version: 0.1.0
 Summary: IBind is a REST and WebSocket client library for Interactive Brokers Client Portal Web API.
 Author-email: Voy Zan <voy1982@yahoo.co.uk>
 License: Copyright 2020 Voy Zan
         
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -270,14 +270,18 @@
 * WebSocket:
   * [WebSocket thread lifecycle handling][wiki-ws-lifecycle]
   * [Thread-safe Queue data stream][wiki-ws-queues]
   * [Internal subscription tracking][wiki-ws-subscriptions]
   * [Health monitoring][wiki-ws-health-monitoring]
   * [and more][wiki-advanced-websocket]
 
+<a href="https://www.youtube.com/watch?v=34iHETvbdas">
+    <img src="https://raw.githubusercontent.com/Voyz/voyz_public/master/ibind_promo_vidA_A01.gif" alt="IBind showcase gif" title="IBind showcase gif" width="500"/>
+</a>
+
 ## Overview
 
 IBind's core functionality consists of two client classes:
 
 * [`IbkrClient`][ibkr-client-docs] - for [IBKR REST API][ibkr-endpoints]
 
   Using the `IbkrClient` requires constructing it with appropriate arguments, then calling the API methods.
```

### Comparing `ibind-0.0.7/README.md` & `ibind-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,18 @@
 * WebSocket:
   * [WebSocket thread lifecycle handling][wiki-ws-lifecycle]
   * [Thread-safe Queue data stream][wiki-ws-queues]
   * [Internal subscription tracking][wiki-ws-subscriptions]
   * [Health monitoring][wiki-ws-health-monitoring]
   * [and more][wiki-advanced-websocket]
 
+<a href="https://www.youtube.com/watch?v=34iHETvbdas">
+    <img src="https://raw.githubusercontent.com/Voyz/voyz_public/master/ibind_promo_vidA_A01.gif" alt="IBind showcase gif" title="IBind showcase gif" width="500"/>
+</a>
+
 ## Overview
 
 IBind's core functionality consists of two client classes:
 
 * [`IbkrClient`][ibkr-client-docs] - for [IBKR REST API][ibkr-endpoints]
 
   Using the `IbkrClient` requires constructing it with appropriate arguments, then calling the API methods.
```

#### html2text {}

```diff
@@ -13,65 +13,66 @@
 client] - WebSocket Python client for [IBKR WebSocket API][ibkr-websocket]. *
 [API Reference][api-ibkr-client] Features: * REST: * [Automated question/answer
 handling][wiki-question-answer] * [Parallel requests][wiki-parallel-requests] *
 [Rate limiting][wiki-rate-limiting] * [Conid unpacking][wiki-conid-unpacking] *
 [and more][wiki-advanced-api] * WebSocket: * [WebSocket thread lifecycle
 handling][wiki-ws-lifecycle] * [Thread-safe Queue data stream][wiki-ws-queues]
 * [Internal subscription tracking][wiki-ws-subscriptions] * [Health monitoring]
-[wiki-ws-health-monitoring] * [and more][wiki-advanced-websocket] ## Overview
-IBind's core functionality consists of two client classes: * [`IbkrClient`]
-[ibkr-client-docs] - for [IBKR REST API][ibkr-endpoints] Using the `IbkrClient`
-requires constructing it with appropriate arguments, then calling the API
-methods. * [`IbkrWsClient`][ibkr-ws-client-docs] - for [IBKR WebSocket API]
-[ibkr-websocket] Using the `IbkrWsClient` involves handling three areas: *
-Managing its lifecycle. It is asynchronous and it will run on a separate
-thread, hence we need to construct it, start it and then manage its lifecycle
-on the originating thread. * Subscribing and unsubscribing. It is subscription-
-based, hence we need to specify which channels we want to subscribe to and
-remember to unsubscribe later. * Consuming data. It uses a queue system, hence
-we need to access these queues and consume their data. Their usage differs
-substantially. Users are encouraged to familiarise themselves with the
-`IbkrClient` class first. ## Examples See [all examples][examples]. ### Basic
-REST Example ```python from ibind import IbkrClient # Construct the client
-client = IbkrClient() # Call some endpoints print('\n#### check_health ####')
-print(client.check_health()) print('\n\n#### tickle ####') print(client.tickle
-().data) print('\n\n#### get_accounts ####') print(client.portfolio_accounts
-().data) ``` ### Basic WebSocket Example ```python from ibind import IbkrWsKey,
-IbkrWsClient # Construct the client. Assumes IBIND_ACCOUNT_ID and IBIND_CACERT
-environment variables have been set. ws_client = IbkrWsClient(start=True) #
-Choose the WebSocket channel ibkr_ws_key = IbkrWsKey.PNL # Subscribe to the PNL
-channel ws_client.subscribe(channel=ibkr_ws_key.channel) # Wait for new items
-in the PNL queue. while True: while not ws_client.empty(ibkr_ws_key): print
-(ws_client.get(ibkr_ws_key)) ``` ## Licence See [LICENSE](https://github.com/
-Voyz/ibind/blob/master/LICENSE) ## Disclaimer IBind is not built, maintained,
-or endorsed by the Interactive Brokers. Use at own discretion. IBind and its
-authors give no guarantee of uninterrupted run of and access to the Interactive
-Brokers Client Portal Web API. You should prepare for breaks in connectivity to
-IBKR servers and should not depend on continuous uninterrupted connection and
-functionality. To partially reduce the potential risk use Paper Account
-credentials. IBind is provided on an AS IS and AS AVAILABLE basis without any
-representation or endorsement made and without warranty of any kind whether
-express or implied, including but not limited to the implied warranties of
-satisfactory quality, fitness for a particular purpose, non-infringement,
-compatibility, security and accuracy. To the extent permitted by law, IBind's
-authors will not be liable for any indirect or consequential loss or damage
-whatever (including without limitation loss of business, opportunity, data,
-profits) arising out of or in connection with the use of IBind. IBind's authors
-make no warranty that the functionality of IBind will be uninterrupted or error
-free, that defects will be corrected or that IBind or the server that makes it
-available are free of viruses or anything else which may be harmful or
-destructive. ## Acknowledgement IBind has been enriched by incorporating work
-developed in collaboration with [Kinetic](https://www.kinetic.xyz/) and [Grant
-Stenger](https://github.com/GrantStenger), which now forms part of the initial
-open-source release. I appreciate their significant contribution to this
-community-driven initiative. Cheers Kinetic! ð» ## Built by Voy Hi! Thanks
-for checking out and using this library. If you are interested in discussing
-your project, require mentorship, consider hiring me, or just wanna chat - I'm
-happy to talk. You can email me to get in touch: hello@voyzan.com Or if you'd
-just want to give something back, I've got a Buy Me A Coffee account: _[_B_u_y_ _M_e_ _A
+[wiki-ws-health-monitoring] * [and more][wiki-advanced-websocket] _[_I_B_i_n_d
+_s_h_o_w_c_a_s_e_ _g_i_f_]## Overview IBind's core functionality consists of two client
+classes: * [`IbkrClient`][ibkr-client-docs] - for [IBKR REST API][ibkr-
+endpoints] Using the `IbkrClient` requires constructing it with appropriate
+arguments, then calling the API methods. * [`IbkrWsClient`][ibkr-ws-client-
+docs] - for [IBKR WebSocket API][ibkr-websocket] Using the `IbkrWsClient`
+involves handling three areas: * Managing its lifecycle. It is asynchronous and
+it will run on a separate thread, hence we need to construct it, start it and
+then manage its lifecycle on the originating thread. * Subscribing and
+unsubscribing. It is subscription-based, hence we need to specify which
+channels we want to subscribe to and remember to unsubscribe later. * Consuming
+data. It uses a queue system, hence we need to access these queues and consume
+their data. Their usage differs substantially. Users are encouraged to
+familiarise themselves with the `IbkrClient` class first. ## Examples See [all
+examples][examples]. ### Basic REST Example ```python from ibind import
+IbkrClient # Construct the client client = IbkrClient() # Call some endpoints
+print('\n#### check_health ####') print(client.check_health()) print('\n\n####
+tickle ####') print(client.tickle().data) print('\n\n#### get_accounts ####')
+print(client.portfolio_accounts().data) ``` ### Basic WebSocket Example
+```python from ibind import IbkrWsKey, IbkrWsClient # Construct the client.
+Assumes IBIND_ACCOUNT_ID and IBIND_CACERT environment variables have been set.
+ws_client = IbkrWsClient(start=True) # Choose the WebSocket channel ibkr_ws_key
+= IbkrWsKey.PNL # Subscribe to the PNL channel ws_client.subscribe
+(channel=ibkr_ws_key.channel) # Wait for new items in the PNL queue. while
+True: while not ws_client.empty(ibkr_ws_key): print(ws_client.get(ibkr_ws_key))
+``` ## Licence See [LICENSE](https://github.com/Voyz/ibind/blob/master/LICENSE)
+## Disclaimer IBind is not built, maintained, or endorsed by the Interactive
+Brokers. Use at own discretion. IBind and its authors give no guarantee of
+uninterrupted run of and access to the Interactive Brokers Client Portal Web
+API. You should prepare for breaks in connectivity to IBKR servers and should
+not depend on continuous uninterrupted connection and functionality. To
+partially reduce the potential risk use Paper Account credentials. IBind is
+provided on an AS IS and AS AVAILABLE basis without any representation or
+endorsement made and without warranty of any kind whether express or implied,
+including but not limited to the implied warranties of satisfactory quality,
+fitness for a particular purpose, non-infringement, compatibility, security and
+accuracy. To the extent permitted by law, IBind's authors will not be liable
+for any indirect or consequential loss or damage whatever (including without
+limitation loss of business, opportunity, data, profits) arising out of or in
+connection with the use of IBind. IBind's authors make no warranty that the
+functionality of IBind will be uninterrupted or error free, that defects will
+be corrected or that IBind or the server that makes it available are free of
+viruses or anything else which may be harmful or destructive. ##
+Acknowledgement IBind has been enriched by incorporating work developed in
+collaboration with [Kinetic](https://www.kinetic.xyz/) and [Grant Stenger]
+(https://github.com/GrantStenger), which now forms part of the initial open-
+source release. I appreciate their significant contribution to this community-
+driven initiative. Cheers Kinetic! ð» ## Built by Voy Hi! Thanks for checking
+out and using this library. If you are interested in discussing your project,
+require mentorship, consider hiring me, or just wanna chat - I'm happy to talk.
+You can email me to get in touch: hello@voyzan.com Or if you'd just want to
+give something back, I've got a Buy Me A Coffee account: _[_B_u_y_ _M_e_ _A
 _C_o_f_f_e_e_]Thanks and have an awesome day ð [ibeam]: https://github.com/Voyz/
 ibeam [examples]: https://github.com/Voyz/ibind/blob/master/examples [issues]:
 https://github.com/Voyz/ibind/issues [api-ibkr-client]: https://github.com/
 Voyz/ibind/wiki/API-Reference-%E2%80%90-IbkrClient [ibkr-client-docs]: https://
 github.com/Voyz/ibind/wiki/Ibkr-Client [ibkr-ws-client-docs]: https://
 github.com/Voyz/ibind/wiki/Ibkr-Ws-Client [ibkr-docs]: https://ibkrcampus.com/
 ibkr-api-page/webapi-doc/ [ibkr-endpoints]: https://ibkrcampus.com/ibkr-api-
```

### Comparing `ibind-0.0.7/ibind/__init__.py` & `ibind-0.1.0/ibind/__init__.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/base/queue_controller.py` & `ibind-0.1.0/ibind/base/queue_controller.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/base/rest_client.py` & `ibind-0.1.0/ibind/base/rest_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/base/subscription_controller.py` & `ibind-0.1.0/ibind/base/subscription_controller.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/base/ws_client.py` & `ibind-0.1.0/ibind/base/ws_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/client/ibkr_client.py` & `ibind-0.1.0/ibind/client/ibkr_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/client/ibkr_client_mixins/accounts_mixin.py` & `ibind-0.1.0/ibind/client/ibkr_client_mixins/accounts_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/client/ibkr_client_mixins/contract_mixin.py` & `ibind-0.1.0/ibind/client/ibkr_client_mixins/contract_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         """
         Obtains the exchange rates of the currency pair.
 
         Parameters:
             source (str): Specify the base currency to request data for. Valid Structure: “AUD”
             target (str): Specify the quote currency to request data for. Valid Structure: “USD”
         """
-        return self.get(f'iserver/exchangerate', {'source': source, target: target})
+        return self.get(f'iserver/exchangerate', {'source': source, 'target': target})
 
     def info_and_rules_by_conid(self: 'IbkrClient', conid: str, is_buy: bool) -> Result:  # pragma: no cover
         """
         Returns both contract info and rules from a single endpoint.
 
         Parameters:
             conid (str): Contract identifier for the given contract.
```

### Comparing `ibind-0.0.7/ibind/client/ibkr_client_mixins/marketdata_mixin.py` & `ibind-0.1.0/ibind/client/ibkr_client_mixins/marketdata_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/client/ibkr_client_mixins/order_mixin.py` & `ibind-0.1.0/ibind/client/ibkr_client_mixins/order_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/client/ibkr_client_mixins/portfolio_mixin.py` & `ibind-0.1.0/ibind/client/ibkr_client_mixins/portfolio_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/client/ibkr_client_mixins/scanner_mixin.py` & `ibind-0.1.0/ibind/client/ibkr_client_mixins/scanner_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/client/ibkr_client_mixins/session_mixin.py` & `ibind-0.1.0/ibind/client/ibkr_client_mixins/session_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/client/ibkr_client_mixins/watchlist_mixin.py` & `ibind-0.1.0/ibind/client/ibkr_client_mixins/watchlist_mixin.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/client/ibkr_definitions.py` & `ibind-0.1.0/ibind/client/ibkr_definitions.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/client/ibkr_utils.py` & `ibind-0.1.0/ibind/client/ibkr_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/client/ibkr_ws_client.py` & `ibind-0.1.0/ibind/client/ibkr_ws_client.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/support/logs.py` & `ibind-0.1.0/ibind/support/logs.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/support/py_utils.py` & `ibind-0.1.0/ibind/support/py_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind/var.py` & `ibind-0.1.0/ibind/var.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/ibind.egg-info/PKG-INFO` & `ibind-0.1.0/ibind.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibind
-Version: 0.0.7
+Version: 0.1.0
 Summary: IBind is a REST and WebSocket client library for Interactive Brokers Client Portal Web API.
 Author-email: Voy Zan <voy1982@yahoo.co.uk>
 License: Copyright 2020 Voy Zan
         
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -270,14 +270,18 @@
 * WebSocket:
   * [WebSocket thread lifecycle handling][wiki-ws-lifecycle]
   * [Thread-safe Queue data stream][wiki-ws-queues]
   * [Internal subscription tracking][wiki-ws-subscriptions]
   * [Health monitoring][wiki-ws-health-monitoring]
   * [and more][wiki-advanced-websocket]
 
+<a href="https://www.youtube.com/watch?v=34iHETvbdas">
+    <img src="https://raw.githubusercontent.com/Voyz/voyz_public/master/ibind_promo_vidA_A01.gif" alt="IBind showcase gif" title="IBind showcase gif" width="500"/>
+</a>
+
 ## Overview
 
 IBind's core functionality consists of two client classes:
 
 * [`IbkrClient`][ibkr-client-docs] - for [IBKR REST API][ibkr-endpoints]
 
   Using the `IbkrClient` requires constructing it with appropriate arguments, then calling the API methods.
```

### Comparing `ibind-0.0.7/ibind.egg-info/SOURCES.txt` & `ibind-0.1.0/ibind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/pyproject.toml` & `ibind-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ibind"
-version = "0.0.7"
+version = "0.1.0"
 authors = [
     { name="Voy Zan", email="voy1982@yahoo.co.uk" },
 ]
 description = "IBind is a REST and WebSocket client library for Interactive Brokers Client Portal Web API."
 readme = "README.md"
 requires-python = ">=3.8"
 license={ file = "LICENSE" }
```

### Comparing `ibind-0.0.7/test/integration/base/test_rest_client_i.py` & `ibind-0.1.0/test/integration/base/test_rest_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/test/integration/base/test_websocket_client_i.py` & `ibind-0.1.0/test/integration/base/test_websocket_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/test/integration/base/websocketapp_mock.py` & `ibind-0.1.0/test/integration/base/websocketapp_mock.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/test/integration/client/ibkr_responses.py` & `ibind-0.1.0/test/integration/client/ibkr_responses.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/test/integration/client/test_ibkr_client_i.py` & `ibind-0.1.0/test/integration/client/test_ibkr_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/test/integration/client/test_ibkr_utils_i.py` & `ibind-0.1.0/test/integration/client/test_ibkr_utils_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/test/integration/client/test_ibkr_ws_client_i.py` & `ibind-0.1.0/test/integration/client/test_ibkr_ws_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/test/test_utils.py` & `ibind-0.1.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.7/test/unit/support/test_py_utils_u.py` & `ibind-0.1.0/test/unit/support/test_py_utils_u.py`

 * *Files identical despite different names*

