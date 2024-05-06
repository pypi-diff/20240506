# Comparing `tmp/pkscreener-0.44.20240506.342.tar.gz` & `tmp/pkscreener-0.44.20240506.343.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240506.342.tar", last modified: Mon May  6 06:07:57 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240506.343.tar", last modified: Mon May  6 09:44:00 2024, max compression
```

## Comparing `pkscreener-0.44.20240506.342.tar` & `pkscreener-0.44.20240506.343.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 06:07:57.635634 pkscreener-0.44.20240506.342/
--rw-rw-rw-   0        0        0     1086 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-06 06:07:57.635634 pkscreener-0.44.20240506.342/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 06:07:57.620036 pkscreener-0.44.20240506.342/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:07:57.635634 pkscreener-0.44.20240506.342/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    26892 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    10459 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    30557 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    11375 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    22090 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    21218 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18443 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   119323 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    52127 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82533 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-06 06:07:47.000000 pkscreener-0.44.20240506.342/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   127151 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/globals.py
--rw-rw-rw-   0        0        0      867 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47310 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    27495 2024-05-06 06:02:45.000000 pkscreener-0.44.20240506.342/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:07:57.620036 pkscreener-0.44.20240506.342/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-06 06:07:57.000000 pkscreener-0.44.20240506.342/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-06 06:07:57.000000 pkscreener-0.44.20240506.342/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 06:07:57.000000 pkscreener-0.44.20240506.342/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-06 06:07:57.000000 pkscreener-0.44.20240506.342/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-06 06:07:57.000000 pkscreener-0.44.20240506.342/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-06 06:07:57.000000 pkscreener-0.44.20240506.342/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-06 06:07:57.635634 pkscreener-0.44.20240506.342/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-06 06:02:46.000000 pkscreener-0.44.20240506.342/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:44:00.694445 pkscreener-0.44.20240506.343/
+-rw-rw-rw-   0        0        0     1086 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-06 09:44:00.694445 pkscreener-0.44.20240506.343/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 09:44:00.678846 pkscreener-0.44.20240506.343/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:44:00.694445 pkscreener-0.44.20240506.343/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    26892 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    10611 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    30557 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    11375 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    22090 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    21218 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18443 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   119323 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    52127 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82533 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-06 09:43:48.000000 pkscreener-0.44.20240506.343/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   127151 2024-05-06 09:39:57.000000 pkscreener-0.44.20240506.343/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      867 2024-05-06 09:39:58.000000 pkscreener-0.44.20240506.343/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47310 2024-05-06 09:39:58.000000 pkscreener-0.44.20240506.343/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    27495 2024-05-06 09:39:58.000000 pkscreener-0.44.20240506.343/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-06 09:44:00.694445 pkscreener-0.44.20240506.343/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-06 09:44:00.000000 pkscreener-0.44.20240506.343/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-06 09:44:00.000000 pkscreener-0.44.20240506.343/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 09:44:00.000000 pkscreener-0.44.20240506.343/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-06 09:44:00.000000 pkscreener-0.44.20240506.343/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-06 09:44:00.000000 pkscreener-0.44.20240506.343/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-06 09:44:00.000000 pkscreener-0.44.20240506.343/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-06 09:44:00.710068 pkscreener-0.44.20240506.343/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-06 09:39:58.000000 pkscreener-0.44.20240506.343/setup.py
```

### Comparing `pkscreener-0.44.20240506.342/LICENSE` & `pkscreener-0.44.20240506.343/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/LICENSE-Others` & `pkscreener-0.44.20240506.343/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/PKG-INFO` & `pkscreener-0.44.20240506.343/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240506.342
+Version: 0.44.20240506.343
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240506.342.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240506.343.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.341/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.342/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.341/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.342/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.341/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.342/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240506.342/README.md` & `pkscreener-0.44.20240506.343/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.341/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.342/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.341/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.342/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.341/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.342/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240506.342/pkscreener/__init__.py` & `pkscreener-0.44.20240506.343/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/MarketMonitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 import sys
 import pandas as pd
 import numpy as np
 from PKDevTools.classes.Singleton import SingletonType, SingletonMixin
 from PKDevTools.classes.OutputControls import OutputControls
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes import Archiver
+from PKDevTools.classes.SuppressOutput import SuppressOutput
 
 class MarketMonitor(SingletonMixin, metaclass=SingletonType):
     def __init__(self,monitors=[], maxNumResultsPerRow=3,maxNumColsInEachResult=6,maxNumRowsInEachResult=10,maxNumResultRowsInMonitor=2):
         super(MarketMonitor, self).__init__()
         if monitors is not None and len(monitors) > 0:
             
             self.monitors = monitors[:maxNumResultRowsInMonitor*maxNumResultsPerRow]
@@ -114,16 +115,17 @@
                 )
                 telegram_df.loc[:, "Ch%"] = telegram_df.loc[:, "Ch%"].apply(
                     lambda x: f'{int(round(float(x.replace("%","")),0))}%'
                 )
                 telegram_df.loc[:, "Vol"] = telegram_df.loc[:, "Vol"].apply(
                     lambda x: f'{int(round(float(x.replace("x","")),0))}x'
                 )
-                for col in telegram_df.columns:
-                    telegram_df[col] = telegram_df[col].astype(str)
+                with SuppressOutput(suppress_stderr=True, suppress_stdout=True):
+                    for col in telegram_df.columns:
+                        telegram_df[col] = telegram_df[col].astype(str)
             except:
                 pass
         monitorPosition = self.monitorPositions.get(screenOptions)
         if monitorPosition is not None:
             startRowIndex, startColIndex = monitorPosition
             if not self.monitor_df.empty:
                 for _ in range(self.lines):
```

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/classes/keys.py` & `pkscreener-0.44.20240506.343/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/courbd.ttf` & `pkscreener-0.44.20240506.343/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/globals.py` & `pkscreener-0.44.20240506.343/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240506.343/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240506.343/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240506.343/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240506.343/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240506.342
+Version: 0.44.20240506.343
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240506.342.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240506.343.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.341/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.342/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.341/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.342/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.341/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240506.342/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240506.342/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240506.343/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240506.342/setup.py` & `pkscreener-0.44.20240506.343/setup.py`

 * *Files identical despite different names*

