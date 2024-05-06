# Comparing `tmp/pqsdk-0.0.5.tar.gz` & `tmp/pqsdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqsdk-0.0.5.tar", last modified: Sun May  5 10:12:10 2024, max compression
+gzip compressed data, was "pqsdk-0.0.6.tar", last modified: Mon May  6 11:09:20 2024, max compression
```

## Comparing `pqsdk-0.0.5.tar` & `pqsdk-0.0.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 10:12:10.825346 pqsdk-0.0.5/
--rw-rw-rw-   0        0        0      766 2024-05-05 10:12:10.824345 pqsdk-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       85 2024-04-08 07:45:14.000000 pqsdk-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 10:12:10.702345 pqsdk-0.0.5/pqsdk/
--rw-rw-rw-   0        0        0      169 2024-04-12 13:30:06.000000 pqsdk-0.0.5/pqsdk/__init__.py
--rw-rw-rw-   0        0        0     4152 2024-04-10 00:51:13.000000 pqsdk-0.0.5/pqsdk/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:12:10.724345 pqsdk-0.0.5/pqsdk/api/
--rw-rw-rw-   0        0        0      547 2024-04-12 09:45:19.000000 pqsdk-0.0.5/pqsdk/api/__init__.py
--rw-rw-rw-   0        0        0     1155 2024-04-12 09:39:00.000000 pqsdk-0.0.5/pqsdk/api/main.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:12:10.762345 pqsdk-0.0.5/pqsdk/backtest/
--rw-rw-rw-   0        0        0     3196 2024-04-10 08:16:12.000000 pqsdk-0.0.5/pqsdk/backtest/__init__.py
--rw-rw-rw-   0        0        0     3419 2024-04-09 09:24:24.000000 pqsdk-0.0.5/pqsdk/backtest/analyzer.py
--rw-rw-rw-   0        0        0    35704 2024-04-10 03:08:27.000000 pqsdk-0.0.5/pqsdk/backtest/context.py
--rw-rw-rw-   0        0        0     3213 2024-04-10 03:08:27.000000 pqsdk-0.0.5/pqsdk/backtest/current_data.py
--rw-rw-rw-   0        0        0     6557 2024-04-10 03:08:27.000000 pqsdk-0.0.5/pqsdk/backtest/instrument.py
--rw-rw-rw-   0        0        0    14082 2024-04-20 12:07:11.000000 pqsdk-0.0.5/pqsdk/backtest/main.py
--rw-rw-rw-   0        0        0     3840 2024-04-09 09:28:17.000000 pqsdk-0.0.5/pqsdk/backtest/order.py
--rw-rw-rw-   0        0        0     2687 2024-04-10 03:08:27.000000 pqsdk-0.0.5/pqsdk/backtest/portfolio.py
--rw-rw-rw-   0        0        0     4500 2024-04-10 03:08:27.000000 pqsdk-0.0.5/pqsdk/backtest/position.py
--rw-rw-rw-   0        0        0     2021 2024-04-10 03:08:27.000000 pqsdk-0.0.5/pqsdk/backtest/run_info.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:12:10.766345 pqsdk-0.0.5/pqsdk/enums/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.5/pqsdk/enums/__init__.py
--rw-rw-rw-   0        0        0     1054 2024-04-09 09:33:02.000000 pqsdk-0.0.5/pqsdk/enums/orderStatus.py
--rw-rw-rw-   0        0        0     8669 2024-04-09 09:24:24.000000 pqsdk-0.0.5/pqsdk/faxconstant.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:12:10.801345 pqsdk-0.0.5/pqsdk/interface/
--rw-rw-rw-   0        0        0      589 2024-04-09 09:24:24.000000 pqsdk-0.0.5/pqsdk/interface/__init__.py
--rw-rw-rw-   0        0        0     3004 2024-04-09 09:24:24.000000 pqsdk-0.0.5/pqsdk/interface/abstractInstrument.py
--rw-rw-rw-   0        0        0     2341 2024-04-09 09:27:44.000000 pqsdk-0.0.5/pqsdk/interface/abstractOrder.py
--rw-rw-rw-   0        0        0     1347 2024-04-09 09:24:24.000000 pqsdk-0.0.5/pqsdk/interface/abstractPortfolio.py
--rw-rw-rw-   0        0        0     1677 2024-04-20 13:04:56.000000 pqsdk-0.0.5/pqsdk/interface/abstractPosition.py
--rw-rw-rw-   0        0        0     2652 2024-04-09 09:24:24.000000 pqsdk-0.0.5/pqsdk/interface/abstractRunInfo.py
--rw-rw-rw-   0        0        0    18860 2024-04-09 09:24:24.000000 pqsdk-0.0.5/pqsdk/interface/abstractStrategyContext.py
--rw-rw-rw-   0        0        0     2907 2024-04-09 09:24:24.000000 pqsdk-0.0.5/pqsdk/interface/abstractTrader.py
--rw-rw-rw-   0        0        0     2170 2024-04-09 09:32:55.000000 pqsdk-0.0.5/pqsdk/interface/constant.py
--rw-rw-rw-   0        0        0     5757 2024-05-05 10:11:04.000000 pqsdk-0.0.5/pqsdk/logger.py
--rw-rw-rw-   0        0        0     1650 2024-04-10 04:31:09.000000 pqsdk-0.0.5/pqsdk/main.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:12:10.819345 pqsdk-0.0.5/pqsdk/utils/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.5/pqsdk/utils/__init__.py
--rw-rw-rw-   0        0        0     3617 2024-04-09 09:24:24.000000 pqsdk-0.0.5/pqsdk/utils/dynamic_import.py
--rw-rw-rw-   0        0        0     1426 2024-04-09 09:24:24.000000 pqsdk-0.0.5/pqsdk/utils/file_util.py
--rw-rw-rw-   0        0        0      368 2024-04-09 09:24:24.000000 pqsdk-0.0.5/pqsdk/utils/import_global_modules.py
--rw-rw-rw-   0        0        0     5710 2024-04-10 03:08:27.000000 pqsdk-0.0.5/pqsdk/utils/timer_factory.py
--rw-rw-rw-   0        0        0      780 2024-04-09 09:24:24.000000 pqsdk-0.0.5/pqsdk/utils/value_type_util.py
--rw-rw-rw-   0        0        0      441 2024-05-05 10:11:04.000000 pqsdk-0.0.5/pqsdk/version.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:12:10.823344 pqsdk-0.0.5/pqsdk.egg-info/
--rw-rw-rw-   0        0        0      766 2024-05-05 10:12:10.000000 pqsdk-0.0.5/pqsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1193 2024-05-05 10:12:10.000000 pqsdk-0.0.5/pqsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 10:12:10.000000 pqsdk-0.0.5/pqsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-05 10:12:10.000000 pqsdk-0.0.5/pqsdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      183 2024-05-05 10:12:10.000000 pqsdk-0.0.5/pqsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-05 10:12:10.000000 pqsdk-0.0.5/pqsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 10:12:10.825346 pqsdk-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1599 2024-04-12 14:22:50.000000 pqsdk-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:12:10.823344 pqsdk-0.0.5/tests/
--rw-rw-rw-   0        0        0      472 2024-04-10 08:16:28.000000 pqsdk-0.0.5/tests/test_backtest.py
--rw-rw-rw-   0        0        0     2137 2024-05-05 08:03:23.000000 pqsdk-0.0.5/tests/test_pqsdk_api.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:09:20.011438 pqsdk-0.0.6/
+-rw-rw-rw-   0        0        0      766 2024-05-06 11:09:20.010438 pqsdk-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       85 2024-04-08 07:45:14.000000 pqsdk-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 11:09:19.885438 pqsdk-0.0.6/pqsdk/
+-rw-rw-rw-   0        0        0      190 2024-05-06 11:07:04.000000 pqsdk-0.0.6/pqsdk/__init__.py
+-rw-rw-rw-   0        0        0     4152 2024-04-10 00:51:13.000000 pqsdk-0.0.6/pqsdk/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:09:19.904438 pqsdk-0.0.6/pqsdk/api/
+-rw-rw-rw-   0        0        0      547 2024-04-12 09:45:19.000000 pqsdk-0.0.6/pqsdk/api/__init__.py
+-rw-rw-rw-   0        0        0     1155 2024-04-12 09:39:00.000000 pqsdk-0.0.6/pqsdk/api/main.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:09:19.945437 pqsdk-0.0.6/pqsdk/backtest/
+-rw-rw-rw-   0        0        0     3196 2024-04-10 08:16:12.000000 pqsdk-0.0.6/pqsdk/backtest/__init__.py
+-rw-rw-rw-   0        0        0     3419 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/backtest/analyzer.py
+-rw-rw-rw-   0        0        0    35704 2024-04-10 03:08:27.000000 pqsdk-0.0.6/pqsdk/backtest/context.py
+-rw-rw-rw-   0        0        0     3213 2024-04-10 03:08:27.000000 pqsdk-0.0.6/pqsdk/backtest/current_data.py
+-rw-rw-rw-   0        0        0     6557 2024-04-10 03:08:27.000000 pqsdk-0.0.6/pqsdk/backtest/instrument.py
+-rw-rw-rw-   0        0        0    14082 2024-04-20 12:07:11.000000 pqsdk-0.0.6/pqsdk/backtest/main.py
+-rw-rw-rw-   0        0        0     3840 2024-04-09 09:28:17.000000 pqsdk-0.0.6/pqsdk/backtest/order.py
+-rw-rw-rw-   0        0        0     2687 2024-04-10 03:08:27.000000 pqsdk-0.0.6/pqsdk/backtest/portfolio.py
+-rw-rw-rw-   0        0        0     4500 2024-04-10 03:08:27.000000 pqsdk-0.0.6/pqsdk/backtest/position.py
+-rw-rw-rw-   0        0        0     2021 2024-04-10 03:08:27.000000 pqsdk-0.0.6/pqsdk/backtest/run_info.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:09:19.948438 pqsdk-0.0.6/pqsdk/enums/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/enums/__init__.py
+-rw-rw-rw-   0        0        0     1054 2024-04-09 09:33:02.000000 pqsdk-0.0.6/pqsdk/enums/orderStatus.py
+-rw-rw-rw-   0        0        0     8669 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/faxconstant.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:09:19.984437 pqsdk-0.0.6/pqsdk/interface/
+-rw-rw-rw-   0        0        0      589 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/interface/__init__.py
+-rw-rw-rw-   0        0        0     3004 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/interface/abstractInstrument.py
+-rw-rw-rw-   0        0        0     2341 2024-04-09 09:27:44.000000 pqsdk-0.0.6/pqsdk/interface/abstractOrder.py
+-rw-rw-rw-   0        0        0     1347 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/interface/abstractPortfolio.py
+-rw-rw-rw-   0        0        0     1677 2024-04-20 13:04:56.000000 pqsdk-0.0.6/pqsdk/interface/abstractPosition.py
+-rw-rw-rw-   0        0        0     2652 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/interface/abstractRunInfo.py
+-rw-rw-rw-   0        0        0    18860 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/interface/abstractStrategyContext.py
+-rw-rw-rw-   0        0        0     2907 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/interface/abstractTrader.py
+-rw-rw-rw-   0        0        0     2170 2024-04-09 09:32:55.000000 pqsdk-0.0.6/pqsdk/interface/constant.py
+-rw-rw-rw-   0        0        0     5757 2024-05-05 10:11:04.000000 pqsdk-0.0.6/pqsdk/logger.py
+-rw-rw-rw-   0        0        0     1650 2024-04-10 04:31:09.000000 pqsdk-0.0.6/pqsdk/main.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:09:20.002437 pqsdk-0.0.6/pqsdk/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     3617 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/utils/dynamic_import.py
+-rw-rw-rw-   0        0        0     1426 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/utils/file_util.py
+-rw-rw-rw-   0        0        0      368 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/utils/import_global_modules.py
+-rw-rw-rw-   0        0        0     5710 2024-04-10 03:08:27.000000 pqsdk-0.0.6/pqsdk/utils/timer_factory.py
+-rw-rw-rw-   0        0        0      780 2024-04-09 09:24:24.000000 pqsdk-0.0.6/pqsdk/utils/value_type_util.py
+-rw-rw-rw-   0        0        0      441 2024-05-06 11:09:16.000000 pqsdk-0.0.6/pqsdk/version.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:09:20.010438 pqsdk-0.0.6/pqsdk.egg-info/
+-rw-rw-rw-   0        0        0      766 2024-05-06 11:09:19.000000 pqsdk-0.0.6/pqsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1193 2024-05-06 11:09:19.000000 pqsdk-0.0.6/pqsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 11:09:19.000000 pqsdk-0.0.6/pqsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-06 11:09:19.000000 pqsdk-0.0.6/pqsdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      183 2024-05-06 11:09:19.000000 pqsdk-0.0.6/pqsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-06 11:09:19.000000 pqsdk-0.0.6/pqsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 11:09:20.011438 pqsdk-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2024-04-12 14:22:50.000000 pqsdk-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:09:20.009438 pqsdk-0.0.6/tests/
+-rw-rw-rw-   0        0        0      472 2024-04-10 08:16:28.000000 pqsdk-0.0.6/tests/test_backtest.py
+-rw-rw-rw-   0        0        0     2137 2024-05-05 08:03:23.000000 pqsdk-0.0.6/tests/test_pqsdk_api.py
```

### Comparing `pqsdk-0.0.5/PKG-INFO` & `pqsdk-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqsdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: SDK for stock analysis and strategy backtest.
 Home-page: https://www.pinkquant.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 Platform: all
```

### Comparing `pqsdk-0.0.5/pqsdk/__main__.py` & `pqsdk-0.0.6/pqsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/api/__init__.py` & `pqsdk-0.0.6/pqsdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/api/main.py` & `pqsdk-0.0.6/pqsdk/api/main.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/backtest/__init__.py` & `pqsdk-0.0.6/pqsdk/backtest/__init__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/backtest/analyzer.py` & `pqsdk-0.0.6/pqsdk/backtest/analyzer.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/backtest/context.py` & `pqsdk-0.0.6/pqsdk/backtest/context.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/backtest/current_data.py` & `pqsdk-0.0.6/pqsdk/backtest/current_data.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/backtest/instrument.py` & `pqsdk-0.0.6/pqsdk/backtest/instrument.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/backtest/main.py` & `pqsdk-0.0.6/pqsdk/backtest/main.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/backtest/order.py` & `pqsdk-0.0.6/pqsdk/backtest/order.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/backtest/portfolio.py` & `pqsdk-0.0.6/pqsdk/backtest/portfolio.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/backtest/position.py` & `pqsdk-0.0.6/pqsdk/backtest/position.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/backtest/run_info.py` & `pqsdk-0.0.6/pqsdk/backtest/run_info.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/enums/orderStatus.py` & `pqsdk-0.0.6/pqsdk/enums/orderStatus.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/faxconstant.py` & `pqsdk-0.0.6/pqsdk/faxconstant.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/interface/__init__.py` & `pqsdk-0.0.6/pqsdk/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/interface/abstractInstrument.py` & `pqsdk-0.0.6/pqsdk/interface/abstractInstrument.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/interface/abstractOrder.py` & `pqsdk-0.0.6/pqsdk/interface/abstractOrder.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/interface/abstractPortfolio.py` & `pqsdk-0.0.6/pqsdk/interface/abstractPortfolio.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/interface/abstractPosition.py` & `pqsdk-0.0.6/pqsdk/interface/abstractPosition.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/interface/abstractRunInfo.py` & `pqsdk-0.0.6/pqsdk/interface/abstractRunInfo.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/interface/abstractStrategyContext.py` & `pqsdk-0.0.6/pqsdk/interface/abstractStrategyContext.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/interface/abstractTrader.py` & `pqsdk-0.0.6/pqsdk/interface/abstractTrader.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/interface/constant.py` & `pqsdk-0.0.6/pqsdk/interface/constant.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/logger.py` & `pqsdk-0.0.6/pqsdk/logger.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/main.py` & `pqsdk-0.0.6/pqsdk/main.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/utils/dynamic_import.py` & `pqsdk-0.0.6/pqsdk/utils/dynamic_import.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/utils/file_util.py` & `pqsdk-0.0.6/pqsdk/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/utils/timer_factory.py` & `pqsdk-0.0.6/pqsdk/utils/timer_factory.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk/utils/value_type_util.py` & `pqsdk-0.0.6/pqsdk/utils/value_type_util.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/pqsdk.egg-info/PKG-INFO` & `pqsdk-0.0.6/pqsdk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqsdk
-Version: 0.0.5
+Version: 0.0.6
 Summary: SDK for stock analysis and strategy backtest.
 Home-page: https://www.pinkquant.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 Platform: all
```

### Comparing `pqsdk-0.0.5/pqsdk.egg-info/SOURCES.txt` & `pqsdk-0.0.6/pqsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/setup.py` & `pqsdk-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.5/tests/test_pqsdk_api.py` & `pqsdk-0.0.6/tests/test_pqsdk_api.py`

 * *Files identical despite different names*

