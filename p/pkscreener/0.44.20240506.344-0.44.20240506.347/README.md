# Comparing `tmp/pkscreener-0.44.20240506.344.tar.gz` & `tmp/pkscreener-0.44.20240506.347.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240506.344.tar", last modified: Mon May  6 10:15:33 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240506.347.tar", last modified: Mon May  6 11:54:06 2024, max compression
```

## Comparing `pkscreener-0.44.20240506.344.tar` & `pkscreener-0.44.20240506.347.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 10:15:33.650649 pkscreener-0.44.20240506.344/
--rw-rw-rw-   0        0        0     1086 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-06 10:15:33.650649 pkscreener-0.44.20240506.344/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 10:15:33.635025 pkscreener-0.44.20240506.344/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 10:15:33.650649 pkscreener-0.44.20240506.344/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    26892 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    10662 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    30557 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    11375 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    22090 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    21218 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18443 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   119323 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    52127 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82533 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-06 10:15:25.000000 pkscreener-0.44.20240506.344/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   127151 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/globals.py
--rw-rw-rw-   0        0        0      867 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47432 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    27495 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-06 10:15:33.635025 pkscreener-0.44.20240506.344/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-06 10:15:33.000000 pkscreener-0.44.20240506.344/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-06 10:15:33.000000 pkscreener-0.44.20240506.344/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 10:15:33.000000 pkscreener-0.44.20240506.344/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-06 10:15:33.000000 pkscreener-0.44.20240506.344/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-06 10:15:33.000000 pkscreener-0.44.20240506.344/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-06 10:15:33.000000 pkscreener-0.44.20240506.344/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-06 10:15:33.650649 pkscreener-0.44.20240506.344/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-06 10:09:33.000000 pkscreener-0.44.20240506.344/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:54:06.932648 pkscreener-0.44.20240506.347/
+-rw-rw-rw-   0        0        0     1086 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-06 11:54:06.932648 pkscreener-0.44.20240506.347/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 11:54:06.917050 pkscreener-0.44.20240506.347/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:54:06.932648 pkscreener-0.44.20240506.347/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    26892 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    10662 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    30557 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    11375 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    22090 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    21218 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18443 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   119323 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    52127 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82533 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-06 11:53:59.000000 pkscreener-0.44.20240506.347/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   127151 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      867 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    48085 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    28426 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:54:06.917050 pkscreener-0.44.20240506.347/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-06 11:54:06.000000 pkscreener-0.44.20240506.347/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-06 11:54:06.000000 pkscreener-0.44.20240506.347/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 11:54:06.000000 pkscreener-0.44.20240506.347/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-06 11:54:06.000000 pkscreener-0.44.20240506.347/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-06 11:54:06.000000 pkscreener-0.44.20240506.347/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-06 11:54:06.000000 pkscreener-0.44.20240506.347/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-06 11:54:06.932648 pkscreener-0.44.20240506.347/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-06 11:49:32.000000 pkscreener-0.44.20240506.347/setup.py
```

### Comparing `pkscreener-0.44.20240506.344/LICENSE` & `pkscreener-0.44.20240506.347/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/LICENSE-Others` & `pkscreener-0.44.20240506.347/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/PKG-INFO` & `pkscreener-0.44.20240506.347/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240506.344
+Version: 0.44.20240506.347
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240506.344.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240506.347.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.343/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.344/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.343/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.344/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.343/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.344/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240506.344/README.md` & `pkscreener-0.44.20240506.347/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.343/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.344/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.343/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.344/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.343/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.344/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240506.344/pkscreener/__init__.py` & `pkscreener-0.44.20240506.347/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/ConfigManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         self.generalTimeout = 2
         self.defaultIndex = 12
         self.longTimeout = 4
         self.maxNetworkRetryCount = 10
         self.backtestPeriod = 120
         self.maxBacktestWindow = 30
         self.minVolume = 10000
-        self.morninganalysiscandlenumber = 43 # 9:58am IST, since market opens at 9:15am IST
+        self.morninganalysiscandlenumber = 25 # 9:40am IST, since market opens at 9:15am IST
         self.morninganalysiscandleduration = '1m'
         self.logger = None
         self.showPastStrategyData = False
         # This determines how many days apart the backtest calculations are run.
         # For example, for weekly backtest calculations, set this to 5 (5 days = 1 week)
         # For fortnightly, set this to 10 and so on (10 trading sessions = 2 weeks)
         self.backtestPeriodFactor = 1
```

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/classes/keys.py` & `pkscreener-0.44.20240506.347/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/courbd.ttf` & `pkscreener-0.44.20240506.347/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/globals.py` & `pkscreener-0.44.20240506.347/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240506.347/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240506.347/pkscreener/pkscreenerbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     logger.info("User %s started the conversation.", user.first_name)
     # Build InlineKeyboard where each button has a displayed text
     # and a string as callback_data
     # The keyboard is a list of button rows, where each row is in turn
     # a list (hence `[[...]]`).
     mns = m0.renderForMenu(asList=True)
     if (PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]) or ("PKDevTools_Default_Log_Level" in os.environ.keys()):
-        mns.append(menu().create("MI", "Intraday Monitor", 2))
+        mns.append(menu().create("MI", "Int. Monitor", 2))
     inlineMenus = []
     for mnu in mns:
         if mnu.menuKey in TOP_LEVEL_SCANNER_MENUS:
             inlineMenus.append(
                 InlineKeyboardButton(
                     mnu.menuText.split("(")[0],
                     callback_data="C" + str(mnu.menuKey),
@@ -187,31 +187,44 @@
 async def XScanners(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
     """Show new choice of buttons"""
     query = update.callback_query
     data = query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G").replace("CMI", "MI")
     if data not in TOP_LEVEL_SCANNER_MENUS:
         return start(update, context)
     if data == "MI":
-        # User wants an intraday monitor
-        launcher = "/home/runner/work/PKScreener/PKScreener/pkscreenercli.bin" #if "PKDevTools_Default_Log_Level" in os.environ.keys() else sys.argv[0]
+        from PKDevTools.classes import Archiver
+        filePath = os.path.join(Archiver.get_user_outputs_dir(), "monitor_outputs.txt")
+        appLogsEnabled = ("PKDevTools_Default_Log_Level" in os.environ.keys())
+        # User wants an Int. Monitor
+        launcher = "/home/runner/work/PKScreener/PKScreener/pkscreenercli.bin" if "MONITORING_BOT_RUNNER" in os.environ.keys() else "pkscreener"
         launcher = f"python3.11 {launcher}" if launcher.endswith(".py") else launcher
         # print(f"launcher is {sys.argv[0]} -a Y -m 'X' -p --telegram")
         try:
             from subprocess import Popen
             global monitor_proc
             if monitor_proc is None or monitor_proc.poll() is not None: # Process finished from an earlier launch
-                monitor_proc = Popen([f"{launcher}","-a","Y","-p","-m","X","--telegram",])
-            logger.info(f"{launcher} -a Y -m 'X' -p --telegram launched")
+                if os.path.exists(filePath):
+                    # Let's remove the old file so that the new app can begin to run
+                    # If we don't remove, it might just exit assuming that there's another instance
+                    # already running.
+                    os.remove(filePath)
+                appArgs = [f"{launcher}","-a","Y","-m","X","--telegram",]
+                if appLogsEnabled:
+                    appArgs.append("-l")
+                else:
+                    appArgs.append("-p")
+                monitor_proc = Popen(appArgs)
+                logger.info(f"{launcher} -a Y -m 'X' -p --telegram launched")
+            else:
+                logger.info(f"{launcher} -a Y -m 'X' -p --telegram already running")
         except Exception as e:
             logger.info(f"{launcher} -a Y -m 'X' -p --telegram could not be launched")
             logger.info(e)
             pass
         try:
-            from PKDevTools.classes import Archiver
-            filePath = os.path.join(Archiver.get_user_outputs_dir(), "monitor_outputs.txt")
             # if not os.path.exists(filePath):
             #     sleep(5)
             #     if not os.path.exists(filePath):
             #         f = open(filePath, "w")
             #         f.write("Please wait...")
             #         f.close()
             if os.path.exists(filePath):
```

### Comparing `pkscreener-0.44.20240506.344/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240506.347/pkscreener/pkscreenercli.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,14 +329,18 @@
         import pandas as pd
         # Delete any existing data from the previous run.
         configManager.deleteFileWithPattern(pattern="stock_data_*.pkl")
         for runOption in runOptions:
             args.options = runOption
             try:
                 optionalFinalOutcome_df,_ = main(userArgs=args,optionalFinalOutcome_df=optionalFinalOutcome_df)
+                if "EoDDiff" not in optionalFinalOutcome_df.columns:
+                    # Somehow the file must have been corrupted. Let's re-download
+                    configManager.deleteFileWithPattern(pattern="stock_data_*.pkl")
+                    configManager.deleteFileWithPattern(pattern="intraday_stock_data_*.pkl")
                 if isInterrupted():
                     break
             except Exception as e:
                 OutputControls().printOutput(e)
                 if args.log:
                     traceback.print_exc()
         if optionalFinalOutcome_df is not None:
@@ -518,21 +522,28 @@
         disableSysOut()
 
     if not configManager.checkConfigFile():
         configManager.setConfig(
             ConfigManager.parser, default=True, showFileCreatedText=False
         )
     if args.telegram:
-        from PKDevTools.classes import Archiver
-        filePath = os.path.join(Archiver.get_user_outputs_dir(), "monitor_outputs.txt")
-        if os.path.exists(filePath):
-            # Since the file exists, it means, there is another instance running
+        # Launched by bot for intraday monitor?
+        if (PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]) or ("PKDevTools_Default_Log_Level" in os.environ.keys()):
+            from PKDevTools.classes import Archiver
+            filePath = os.path.join(Archiver.get_user_outputs_dir(), "monitor_outputs.txt")
+            if os.path.exists(filePath):
+                default_logger().info("monitor_outputs.txt already exists! This means an instance may already be running. Exiting now...")
+                # Since the file exists, it means, there is another instance running
+                sys.exit(0)
+            import atexit
+            atexit.register(removeMonitorFile)
+        else:
+            # It should have been launched only during the trading hours
+            default_logger().info("--telegram option must be launched ONLY during NSE trading hours. Exiting now...")
             sys.exit(0)
-        import atexit
-        atexit.register(removeMonitorFile)
     # Check and see if we're running only the telegram bot
     if args.bot:
         from pkscreener import pkscreenerbot
         pkscreenerbot.runpkscreenerbot()
         return
     
     if args.intraday:
```

### Comparing `pkscreener-0.44.20240506.344/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240506.347/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240506.344
+Version: 0.44.20240506.347
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240506.344.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240506.347.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.343/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.344/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.343/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.344/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.343/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.344/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240506.344/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240506.347/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.344/setup.py` & `pkscreener-0.44.20240506.347/setup.py`

 * *Files identical despite different names*

