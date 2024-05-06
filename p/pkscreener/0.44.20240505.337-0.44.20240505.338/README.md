# Comparing `tmp/pkscreener-0.44.20240505.337.tar.gz` & `tmp/pkscreener-0.44.20240505.338.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240505.337.tar", last modified: Sun May  5 10:33:41 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240505.338.tar", last modified: Sun May  5 20:02:40 2024, max compression
```

## Comparing `pkscreener-0.44.20240505.337.tar` & `pkscreener-0.44.20240505.338.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 10:33:41.986603 pkscreener-0.44.20240505.337/
--rw-rw-rw-   0        0        0     1086 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-05 10:33:41.986603 pkscreener-0.44.20240505.337/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 10:33:41.970979 pkscreener-0.44.20240505.337/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:33:41.986603 pkscreener-0.44.20240505.337/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    26892 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7857 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    30385 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    11375 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    22090 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    21218 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18443 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   119213 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    52127 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    82261 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-05 10:33:33.000000 pkscreener-0.44.20240505.337/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   124696 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/globals.py
--rw-rw-rw-   0        0        0      867 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    44575 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    26476 2024-05-05 10:30:01.000000 pkscreener-0.44.20240505.337/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-05 10:33:41.970979 pkscreener-0.44.20240505.337/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-05 10:33:41.000000 pkscreener-0.44.20240505.337/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-05 10:33:41.000000 pkscreener-0.44.20240505.337/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 10:33:41.000000 pkscreener-0.44.20240505.337/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-05 10:33:41.000000 pkscreener-0.44.20240505.337/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-05 10:33:41.000000 pkscreener-0.44.20240505.337/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-05 10:33:41.000000 pkscreener-0.44.20240505.337/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-05 10:33:41.986603 pkscreener-0.44.20240505.337/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-05 10:30:02.000000 pkscreener-0.44.20240505.337/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 20:02:40.191307 pkscreener-0.44.20240505.338/
+-rw-rw-rw-   0        0        0     1086 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-05 20:02:40.191307 pkscreener-0.44.20240505.338/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 20:02:40.175711 pkscreener-0.44.20240505.338/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 20:02:40.191307 pkscreener-0.44.20240505.338/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    26892 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    10459 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    30557 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    11375 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    22090 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    21218 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18443 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   119323 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    52127 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    82533 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-05 20:02:28.000000 pkscreener-0.44.20240505.338/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   127151 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      867 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    46710 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    27495 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-05 20:02:40.175711 pkscreener-0.44.20240505.338/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-05 20:02:40.000000 pkscreener-0.44.20240505.338/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-05 20:02:40.000000 pkscreener-0.44.20240505.338/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 20:02:40.000000 pkscreener-0.44.20240505.338/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-05 20:02:40.000000 pkscreener-0.44.20240505.338/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-05 20:02:40.000000 pkscreener-0.44.20240505.338/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-05 20:02:40.000000 pkscreener-0.44.20240505.338/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-05 20:02:40.191307 pkscreener-0.44.20240505.338/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-05 19:58:25.000000 pkscreener-0.44.20240505.338/setup.py
```

### Comparing `pkscreener-0.44.20240505.337/LICENSE` & `pkscreener-0.44.20240505.338/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/LICENSE-Others` & `pkscreener-0.44.20240505.338/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/PKG-INFO` & `pkscreener-0.44.20240505.338/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240505.337
+Version: 0.44.20240505.338
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240505.337.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240505.338.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.337/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.337/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.337/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240505.337/README.md` & `pkscreener-0.44.20240505.338/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.337/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.337/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.337/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240505.337/pkscreener/__init__.py` & `pkscreener-0.44.20240505.338/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/MarketMonitor.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,20 +18,22 @@
     FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
     AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
     SOFTWARE.
 
 """
+import os
 import sys
 import pandas as pd
 import numpy as np
 from PKDevTools.classes.Singleton import SingletonType, SingletonMixin
 from PKDevTools.classes.OutputControls import OutputControls
 from PKDevTools.classes.ColorText import colorText
+from PKDevTools.classes import Archiver
 
 class MarketMonitor(SingletonMixin, metaclass=SingletonType):
     def __init__(self,monitors=[], maxNumResultsPerRow=3,maxNumColsInEachResult=6,maxNumRowsInEachResult=10,maxNumResultRowsInMonitor=2):
         super(MarketMonitor, self).__init__()
         if monitors is not None and len(monitors) > 0:
             
             self.monitors = monitors[:maxNumResultRowsInMonitor*maxNumResultsPerRow]
@@ -70,15 +72,15 @@
             self.monitorIndex += 1
             if self.monitorIndex > maxIndex:
                 self.monitorIndex = 0
         except:
             pass
         return option
 
-    def refresh(self, screen_df:pd.DataFrame=None, screenOptions=None, chosenMenu=None, dbTimestamp=""):
+    def refresh(self, screen_df:pd.DataFrame=None, screenOptions=None, chosenMenu=None, dbTimestamp="", telegram=False):
         highlightRows = []
         highlightCols = []
         if screen_df is None or screen_df.empty:
             return
 
         screen_monitor_df = screen_df.copy()
         screen_monitor_df.reset_index(inplace=True)
@@ -92,14 +94,38 @@
         screen_monitor_df.loc[:, "52Wk H"] = screen_monitor_df.loc[:, "52Wk H"].apply(
             lambda x: Utility.tools.roundOff(x,0)
         )
         screen_monitor_df.loc[:, "Volume"] = screen_monitor_df.loc[:, "Volume"].apply(
             lambda x: Utility.tools.roundOff(x,0)
         )
         screen_monitor_df.rename(columns={"%Chng": "Ch%","Volume":"Vol","52Wk H":"52WkH", "RSI":"RSI/i"}, inplace=True)
+        if telegram:
+            telegram_df = screen_monitor_df[["Stock", "LTP", "Ch%", "Vol"]]
+            try:
+                telegram_df.loc[:, "Stock"] = telegram_df.loc[:, "Stock"].apply(
+                    lambda x: x.split('\x1b')[3].replace('\\','') if 'http' in x else x
+                )
+                cols = ["LTP", "Ch%", "Vol"]
+                for col in cols:
+                    telegram_df.loc[:, col] = telegram_df.loc[:, col].apply(
+                        lambda x: x.replace(colorText.FAIL,"").replace(colorText.GREEN,"").replace(colorText.WARN,"").replace(colorText.BOLD,"").replace(colorText.END,"")
+                    )
+                telegram_df.loc[:, "LTP"] = telegram_df.loc[:, "LTP"].apply(
+                    lambda x: str(int(round(float(x),0)))
+                )
+                telegram_df.loc[:, "Ch%"] = telegram_df.loc[:, "Ch%"].apply(
+                    lambda x: f'{int(round(float(x.replace("%","")),0))}%'
+                )
+                telegram_df.loc[:, "Vol"] = telegram_df.loc[:, "Vol"].apply(
+                    lambda x: f'{int(round(float(x.replace("x","")),0))}x'
+                )
+                for col in telegram_df.columns:
+                    telegram_df[col] = telegram_df[col].astype(str)
+            except:
+                pass
         monitorPosition = self.monitorPositions.get(screenOptions)
         if monitorPosition is not None:
             startRowIndex, startColIndex = monitorPosition
             if not self.monitor_df.empty:
                 for _ in range(self.lines):
                     sys.stdout.write("\x1b[1A")  # cursor up one line
                     sys.stdout.write("\x1b[2K")  # delete the last line
@@ -127,25 +153,45 @@
                 rowIndex += 1
                 colIndex = 0
                 highlightRows.append(startRowIndex+1)
                 startRowIndex += 1
 
         self.monitor_df = self.monitor_df.replace(np.nan, "-", regex=True)
         # self.monitorNames[screenOptions] = f"(Dashboard) > {chosenMenu}"
-        latestScanMenuOption = f"[+] {dbTimestamp} (Dashboard) > " + f"{chosenMenu} [{screenOptions}]"
+        latestScanMenuOption = f"{dbTimestamp} (Dashboard) > " + f"{chosenMenu} [{screenOptions}]"
         OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
-            + latestScanMenuOption
+            + f"[+] {latestScanMenuOption}"
             + colorText.END
             , enableMultipleLineOutput=True
         )
         tabulated_results = colorText.miniTabulator().tabulate(
             self.monitor_df, tablefmt=colorText.No_Pad_GridFormat,
             highlightCharacter=colorText.HEAD+"="+colorText.END,
             showindex=False,
             highlightedRows=highlightRows,
             highlightedColumns=highlightCols,
             maxcolwidths=Utility.tools.getMaxColumnWidths(self.monitor_df)
         )
         self.lines = len(tabulated_results.splitlines()) + 1 # 1 for the progress bar at the bottom and 1 for the chosenMenu option
         OutputControls().printOutput(tabulated_results, enableMultipleLineOutput=True)
+        if telegram:
+            STD_ENCODING=sys.stdout.encoding if sys.stdout is not None else 'utf-8'
+            
+            telegram_df_tabulated = colorText.miniTabulator().tabulate(
+                            telegram_df,
+                            headers="keys",
+                            tablefmt=colorText.No_Pad_GridFormat,
+                            showindex=False,
+                            maxcolwidths=[None,None,4,3]
+                        ).encode("utf-8").decode(STD_ENCODING).replace("-K-----S-----C-----R","-K-----S----C---R").replace("%  ","% ").replace("=K=====S=====C=====R","=K=====S====C===R").replace("Vol  |","Vol|").replace("x  ","x")
+            telegram_df_tabulated = telegram_df_tabulated.replace("-E-----N-----E-----R","-E-----N----E---R").replace("=E=====N=====E=====R","=E=====N====E===R")
+            result_output = f"{latestScanMenuOption}\n<pre>{telegram_df_tabulated}</pre>"
+            try:
+                filePath = os.path.join(Archiver.get_user_outputs_dir(), "monitor_outputs.txt")
+                f = open(filePath, "w")
+                f.write(result_output)
+                f.close()
+            except:
+                pass
+
```

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/MenuOptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,20 @@
     "X": "Scanners",
     "M": "Monitor Intraday",
     "S": "Strategies",
     "B": "Backtests",
     "G": "Growth of 10k",
     "C": "Analyse morning vs close outcomes",
     "T": "~",
+    "D": "Download Daily OHLC Data for the Past Year",
+    "I": "Download Intraday OHLC Data for the Last Trading Day",
     "E": "Edit user configuration",
     "Y": "View your user configuration",
     "U": "Check for software update",
+    "L": "Collect Logs for Debugging",
     "H": "Help / About Developer",
     "Z": "Exit (Ctrl + C)",
 }
 level1_S_MenuDict = {
     "S": "Summary",
     "M": "Back to the Top/Main menu",
     "Z": "Exit (Ctrl + C)",
@@ -459,15 +462,15 @@
                 default_logger().debug(e, exc_info=True)
                 return None
         return None
 
     def renderLevel0Menus(self, asList=False, renderStyle=None, parent=None, skip=None):
         menuText = self.fromDictionary(
             level0MenuDict,
-            renderExceptionKeys=["T", "E", "U", "Z"],
+            renderExceptionKeys=["T", "E", "U", "Z", "L", "D"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
         ).render(asList=asList)
         if asList:
```

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/ScreeningStatistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -485,23 +485,27 @@
     def findHigherOpens(self, df):
         if df is None or len(df) == 0:
             return False
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         recent = data.head(2)
+        if len(recent) < 2:
+            return False
         return recent["Open"].iloc[0] > recent["Close"].iloc[1]
 
     def findHigherBullishOpens(self, df):
         if df is None or len(df) == 0:
             return False
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         recent = data.head(2)
+        if len(recent) < 2:
+            return False
         return recent["Open"].iloc[0] > recent["High"].iloc[1]
     
     def findNR4Day(self, df):
         if df is None or len(df) == 0:
             return False
         data = df.copy()
         # https://chartink.com/screener/nr4-daily-today
```

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/Utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -770,14 +770,15 @@
         cache_file = os.path.join(outputFolder, fileName)
         if not os.path.exists(cache_file) or forceSave or (loadCount >= 0 and len(stockDict) > (loadCount + 1)):
             try:
                 with open(cache_file, "wb") as f:
                     pickle.dump(stockDict.copy(), f, protocol=pickle.HIGHEST_PROTOCOL)
                     OutputControls().printOutput(colorText.BOLD + colorText.GREEN + "=> Done." + colorText.END)
                 if downloadOnly:
+                    OutputControls().printOutput(colorText.BOLD + colorText.GREEN + f"=> {cache_file}" + colorText.END)
                     Committer.execOSCommand(f"git add {cache_file} -f >/dev/null 2>&1")
             except pickle.PicklingError as e:  # pragma: no cover
                 default_logger().debug(e, exc_info=True)
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.FAIL
                     + "=> Error while Caching Stock Data."
@@ -785,14 +786,16 @@
                 )
             except Exception as e:  # pragma: no cover
                 default_logger().debug(e, exc_info=True)
         else:
             OutputControls().printOutput(
                 colorText.BOLD + colorText.GREEN + "=> Already Cached." + colorText.END
             )
+            if downloadOnly:
+                    OutputControls().printOutput(colorText.BOLD + colorText.GREEN + f"=> {cache_file}" + colorText.END)
 
     def downloadLatestData(stockDict,configManager,stockCodes=[],exchangeSuffix=".NS",downloadOnly=False):
         numStocksPerIteration = (int(len(stockCodes)/int(len(stockCodes)/10)) if len(stockCodes) >= 10 else len(stockCodes)) + 1
         queueCounter = 0
         iterations = int(len(stockCodes)/numStocksPerIteration) + 1
         tasksList = []
         while queueCounter < iterations:
```

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/classes/keys.py` & `pkscreener-0.44.20240505.338/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/courbd.ttf` & `pkscreener-0.44.20240505.338/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/globals.py` & `pkscreener-0.44.20240505.338/pkscreener/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -406,14 +406,20 @@
 def initExecution(menuOption=None):
     global selectedChoice
     Utility.tools.clearScreen()
 
     m0.renderForMenu(selectedMenu=None)
     try:
         if menuOption is None:
+            if "PKDevTools_Default_Log_Level" in os.environ.keys():
+                from PKDevTools.classes import Archiver
+                log_file_path = os.path.join(Archiver.get_user_outputs_dir(), "pkscreener-logs.txt")
+                OutputControls().printOutput(colorText.FAIL + "\n    [+] Logs will be written to:"+colorText.END)
+                OutputControls().printOutput(colorText.GREEN + f"    [+] {log_file_path}"+colorText.END)
+                OutputControls().printOutput(colorText.FAIL + "    [+] If you need to share,run through the menus that are causing problems. At the end, open this folder, zip the log file to share at https://github.com/pkjmesra/PKScreener/issues .\n" + colorText.END)
             menuOption = input(colorText.BOLD + colorText.FAIL + "[+] Select option: ")
             OutputControls().printOutput(colorText.END, end="")
         if menuOption == "" or menuOption is None:
             menuOption = "X"
         menuOption = menuOption.upper()
         selectedMenu = m0.find(menuOption)
         if selectedMenu is not None:
@@ -421,15 +427,15 @@
                 input(
                     colorText.BOLD
                     + colorText.FAIL
                     + "[+] Press <Enter> to Exit!"
                     + colorText.END
                 )
                 sys.exit(0)
-            elif selectedMenu.menuKey in ["B", "C", "G", "H", "U", "T", "S", "E", "X", "Y", "M"]:
+            elif selectedMenu.menuKey in ["B", "C", "G", "H", "U", "T", "S", "E", "X", "Y", "M", "D", "I", "L"]:
                 Utility.tools.clearScreen()
                 selectedChoice["0"] = selectedMenu.menuKey
                 return selectedMenu
     except KeyboardInterrupt:
         raise KeyboardInterrupt
     except Exception as e:  # pragma: no cover
         default_logger().debug(e, exc_info=True)
@@ -569,15 +575,15 @@
                 sortKey = ["FVDiff"]
                 ascending = [reversalOption in [9]]
         elif executeOption == 7:
             if reversalOption in [3]:
                 sortKey = ["Volume","MA-Signal"]
                 ascending = [False, False]
         elif executeOption == 23:
-            sortKey = ["bbands_ulr_ratio_max5"]
+            sortKey = ["bbands_ulr_ratio_max5"] if "bbands_ulr_ratio_max5" in screenResults.columns else ["Volume"]
             ascending = [False]
         try:
             try:
                 screenResults[sortKey] = screenResults[sortKey].replace("", np.nan).replace(np.inf, np.nan).replace(-np.inf, np.nan).astype(float)
             except:
                 pass
             try:
@@ -688,20 +694,33 @@
     screenResults, saveResults = PKScanRunner.initDataframes()
     options, menuOption, indexOption, executeOption = getTopLevelMenuChoices(
         startupoptions, testBuild, downloadOnly, defaultAnswer=defaultAnswer
     )
     # Print Level 1 menu options
     selectedMenu = initExecution(menuOption=menuOption)
     menuOption = selectedMenu.menuKey
-    if menuOption in ["M"]:
+    if menuOption in ["M", "D", "I", "L"]:
         launcher = sys.argv[0]
         launcher = f"python3.11 {launcher}" if launcher.endswith(".py") else launcher
-        print(f"{colorText.GREEN}Launching PKScreener in monitoring mode. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -m 'X'{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit monitoring mode.{colorText.END}")
-        sleep(2)
-        os.system(f"{launcher} -a Y -m 'X'")
+        if menuOption in ["M"]:
+            print(f"{colorText.GREEN}Launching PKScreener in monitoring mode. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -m 'X'{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit monitoring mode.{colorText.END}")
+            sleep(2)
+            os.system(f"{launcher} -a Y -m 'X'")
+        elif menuOption in ["D"]:
+            print(f"{colorText.GREEN}Launching PKScreener to Download daily OHLC data. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -e -d{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit at any time.{colorText.END}")
+            sleep(2)
+            os.system(f"{launcher} -a Y -e -d")
+        elif menuOption in ["I"]:
+            print(f"{colorText.GREEN}Launching PKScreener to Download intraday OHLC data. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -e -d -i 1m{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit at any time.{colorText.END}")
+            sleep(2)
+            os.system(f"{launcher} -a Y -e -d -i 1m")
+        elif menuOption in ["L"]:
+            print(f"{colorText.GREEN}Launching PKScreener to collect logs. If it does not launch, please try with the following:{colorText.END}\n{colorText.FAIL}{launcher} -a Y -l{colorText.END}\n{colorText.WARN}Press Ctrl + C to exit at any time.{colorText.END}")
+            sleep(2)
+            os.system(f"{launcher} -a Y -l")
         sys.exit(0)
     elif menuOption in ["X", "T", "E", "Y", "U", "H", "C"]:
         # Print Level 2 menu options
         menuOption, indexOption, executeOption, selectedChoice = getScannerMenuChoices(
             testBuild or testing,
             downloadOnly,
             startupoptions,
@@ -1838,15 +1857,15 @@
                         saveResultsTrimmed,
                         headers="keys",
                         tablefmt=colorText.No_Pad_GridFormat,
                         maxcolwidths=Utility.tools.getMaxColumnWidths(saveResultsTrimmed)
                     ).encode("utf-8").decode(STD_ENCODING)
                     caption_df = saveResultsTrimmed[['LTP','%Chng','Volume']].head(5)
                     caption_df.loc[:, "LTP"] = caption_df.loc[:, "LTP"].apply(
-                        lambda x: str(int(round(x,0)))
+                        lambda x: str(int(round(float(x),0)))
                     )
                     caption_df.loc[:, "%Chng"] = caption_df.loc[:, "%Chng"].apply(
                         lambda x: f'{int(round(float(x.replace("%","")),0))}%'
                     )
                     caption_df.loc[:, "Volume"] = caption_df.loc[:, "Volume"].apply(
                         lambda x: f'{int(round(float(x.replace("x","")),0))}x'
                     )
@@ -2166,14 +2185,21 @@
             + colorText.END
         )
         if not userPassedArgs.download:
             OutputControls().printOutput(colorText.WARN
                 + f"[+] Starting {'Stock' if menuOption not in ['C'] else 'Intraday'} {'Screening' if menuOption=='X' else ('Analysis' if menuOption == 'C' else 'Backtesting.')}. Press Ctrl+C to stop!"
                 + colorText.END
             )
+        else:
+            OutputControls().printOutput(
+                colorText.BOLD
+                + colorText.FAIL
+                + f"[+] Download ONLY mode (OHLCV for period:{configManager.period}, candle-duration:{configManager.duration} )! Stocks will not be screened!"
+                + colorText.END
+            )
         bar, spinner = Utility.tools.getProgressbarStyle()
         with alive_bar(numStocks, bar=bar, spinner=spinner) as progressbar:
             lstscreen = []
             lstsave = []
             result = None
             backtest_df = None
             start_time = time.time()
@@ -2183,15 +2209,15 @@
                 numStocks = processedCount
                 result = resultItem
                 backtest_df = processResults(menuOption, backtestPeriod, result, lstscreen, lstsave, result_df)
                 progressbar()
                 progressbar.text(
                     colorText.BOLD
                     + colorText.GREEN
-                    + f"{'Found' if menuOption in ['X'] else 'Analysed'} {len(lstscreen)} {'Stocks' if menuOption in ['X'] else 'Records'}"
+                    + f"{'Remaining' if userPassedArgs.download else ('Found' if menuOption in ['X'] else 'Analysed')} {len(lstscreen) if not userPassedArgs.download else processedCount} {'Stocks' if menuOption in ['X'] else 'Records'}"
                     + colorText.END
                 )
                 if keyboardInterruptEventFired:
                     return False, backtest_df
                 return not ((testing and len(lstscreen) >= 1) or len(lstscreen) >= max_allowed), backtest_df
             otherArgs = (menuOption, backtestPeriod, result, lstscreen, lstsave)
             backtest_df, result =PKScanRunner.runScan(userPassedArgs,testing,numStocks,iterations,items,numStocksPerIteration,tasks_queue,results_queue,originalNumberOfStocks,backtest_df,*otherArgs,resultsReceivedCb=processResultsCallback)
```

### Comparing `pkscreener-0.44.20240505.337/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240505.338/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240505.338/pkscreener/pkscreenerbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,29 +34,31 @@
 Then, the bot is started and runs until we press Ctrl-C on the command line.
 Usage:
 Example of a bot that uses inline keyboard that has multiple CallbackQueryHandlers arranged in a
 ConversationHandler.
 Send /start to initiate the conversation.
 Press Ctrl-C on the command line to stop the bot.
 """
+import os
 import html
 import json
 import logging
 import re
 import sys
 import traceback
 from datetime import datetime
-
+from time import sleep
 from telegram import __version__ as TG_VER
 from telegram.constants import ParseMode
 
 start_time = datetime.now()
 MINUTES_5_IN_SECONDS = 300
 
 from PKDevTools.classes.Telegram import get_secrets
+from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from PKDevTools.classes.ColorText import colorText
 from pkscreener.classes.MenuOptions import MenuRenderStyle, menu, menus
 from pkscreener.classes.WorkflowManager import run_workflow
 from pkscreener.globals import showSendConfigInfo, showSendHelpInfo
 
 try:
     from telegram import __version_info__
@@ -96,31 +98,31 @@
 ONE, TWO, THREE, FOUR = range(4)
 
 m0 = menus()
 m1 = menus()
 m2 = menus()
 m3 = menus()
 
-TOP_LEVEL_SCANNER_MENUS = ["X", "B"]
-TOP_LEVEL_SCANNER_SKIP_MENUS = ["M", "S", "G", "C", "T", "E", "U", "Z"]
+TOP_LEVEL_SCANNER_MENUS = ["X", "B", "MI"]
+TOP_LEVEL_SCANNER_SKIP_MENUS = ["M", "S", "G", "C", "T", "D", "I", "E", "U", "L", "Z"]
 INDEX_SKIP_MENUS = ["W","E","M","Z","0","2","3","4","6","7","9","10","13"]
 SCANNER_SKIP_MENUS_1_TO_6 = ["0","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_7_TO_12 = ["0","1","2","3","4","5","6","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_13_TO_18 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_19_TO_25 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","22","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_26_TO_31 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","29","30","42","M","Z"]
 SCANNER_MENUS_WITH_NO_SUBMENUS = ["1","2","3","10","11","12","13","14","15","16","17","18","19","20","21","23","24","25","26","27","28"]
 SCANNER_MENUS_WITH_SUBMENU_SUPPORT = ["6", "7", "21"]
 
 INDEX_COMMANDS_SKIP_MENUS_SCANNER = ["W", "E", "M", "Z"]
 INDEX_COMMANDS_SKIP_MENUS_BACKTEST = ["W", "E", "M", "Z", "N", "0", "15"]
 UNSUPPORTED_COMMAND_MENUS =["22","29","30","42","M","Z"]
 SUPPORTED_COMMAND_MENUS = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28"]
 
-async def start(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
+async def start(update: Update, context: ContextTypes.DEFAULT_TYPE, updatedResults=None) -> int:
     """Send message on `/start`."""
     updateCarrier = None
     if update is None:
         return
     else:
         if update.callback_query is not None:
             updateCarrier = update.callback_query
@@ -132,14 +134,16 @@
     user = updateCarrier.from_user
     logger.info("User %s started the conversation.", user.first_name)
     # Build InlineKeyboard where each button has a displayed text
     # and a string as callback_data
     # The keyboard is a list of button rows, where each row is in turn
     # a list (hence `[[...]]`).
     mns = m0.renderForMenu(asList=True)
+    if (PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]) or ("PKDevTools_Default_Log_Level" in os.environ.keys()):
+        mns.append(menu().create("MI", "Intraday Monitor", 2))
     inlineMenus = []
     for mnu in mns:
         if mnu.menuKey in TOP_LEVEL_SCANNER_MENUS:
             inlineMenus.append(
                 InlineKeyboardButton(
                     mnu.menuText.split("(")[0],
                     callback_data="C" + str(mnu.menuKey),
@@ -149,22 +153,25 @@
     reply_markup = InlineKeyboardMarkup(keyboard)
     cmds = m0.renderForMenu(
         selectedMenu=None,
         skip=TOP_LEVEL_SCANNER_SKIP_MENUS,
         asList=True,
         renderStyle=MenuRenderStyle.STANDALONE,
     )
-    cmdText = ""
-    for cmd in cmds:
-        cmdText = f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
-    menuText = f"Welcome {user.first_name}, {(user.username)}! Please choose a menu option by selecting a button from below.\n\nYou can also explore a wide variety of all other scanners by typing in \n{cmdText}\n\n OR just use the buttons below to choose."
+    if updatedResults is None:
+        cmdText = ""
+        for cmd in cmds:
+            cmdText = f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
+        menuText = f"Welcome {user.first_name}, {(user.username)}! Please choose a menu option by selecting a button from below.\n\nYou can also explore a wide variety of all other scanners by typing in \n{cmdText}\n\n OR just use the buttons below to choose."
+    else:
+        menuText = updatedResults
     # Send message with text and appended InlineKeyboard
     if update.callback_query is not None:
         await sendUpdatedMenu(
-            menuText=menuText, update=update, context=context, reply_markup=reply_markup
+            menuText=menuText, update=update, context=context, reply_markup=reply_markup, replaceWhiteSpaces=(updatedResults is None)
         )
     elif update.message is not None:
         await update.message.reply_text(
             menuText,
             reply_markup=reply_markup,
         )
     await context.bot.send_message(
@@ -175,17 +182,46 @@
     # Tell ConversationHandler that we're in state `FIRST` now
     return START_ROUTES
 
 
 async def XScanners(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
     """Show new choice of buttons"""
     query = update.callback_query
-    data = query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G")
+    data = query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G").replace("CMI", "MI")
     if data not in TOP_LEVEL_SCANNER_MENUS:
         return start(update, context)
+    if data == "MI":
+        # User wants an intraday monitor
+        launcher = "pkscreener" if "PKDevTools_Default_Log_Level" in os.environ.keys() else sys.argv[0]
+        launcher = f"python3.11 {launcher}" if launcher.endswith(".py") else launcher
+        try:
+            from subprocess import Popen
+            Popen([f"{launcher}","-a","Y","-p","-m","X","-p","--telegram",])
+            # os.system(f"{launcher} -a Y -m 'X' -p --telegram")
+            print(f"{launcher} -a Y -m 'X' -p --telegram launched")
+        except:
+            pass
+        try:
+            from PKDevTools.classes import Archiver
+            filePath = os.path.join(Archiver.get_user_outputs_dir(), "monitor_outputs.txt")
+            # if not os.path.exists(filePath):
+            #     sleep(5)
+            #     if not os.path.exists(filePath):
+            #         f = open(filePath, "w")
+            #         f.write("Please wait...")
+            #         f.close()
+            f = open(filePath, "r")
+            result_outputs = f.read()
+            f.close()
+            await start(update, context, updatedResults=result_outputs)
+            return START_ROUTES
+        except:
+            await start(update, context, updatedResults="No New update. Please try again in the next few seconds.")
+            return START_ROUTES
+
     midSkip = "1" if data == "X" else "N"
     skipMenus = [midSkip]
     skipMenus.extend(INDEX_SKIP_MENUS)
     menuText = (
         m1.renderForMenu(
             m0.find(data),
             skip=skipMenus,
@@ -400,21 +436,23 @@
                     )
                 )
     keyboard = [inlineMenus]
     reply_markup = InlineKeyboardMarkup(keyboard)
     return reply_markup
 
 
-async def sendUpdatedMenu(menuText, update: Update, context, reply_markup):
+async def sendUpdatedMenu(menuText, update: Update, context, reply_markup, replaceWhiteSpaces=True):
     try:
         await update.callback_query.edit_message_text(
-            text=menuText.replace("     ", "").replace("    ", "").replace("\t", "").replace(colorText.FAIL,"").replace(colorText.END,""),
+            text=menuText.replace("     ", "").replace("    ", "").replace("\t", "").replace(colorText.FAIL,"").replace(colorText.END,"") if replaceWhiteSpaces else menuText,
+            parse_mode="HTML",
             reply_markup=reply_markup,
         )
-    except Exception:# pragma: no cover
+    except Exception as e:# pragma: no cover
+        logger.log(e)
         await start(update, context)
 
 
 async def launchScreener(options, user, context, optionChoices, update):
     try:
         if str(optionChoices.upper()).startswith("B"):
             optionChoices = optionChoices.replace(" ", "").replace(">", "_").replace(":","_").replace("_D","")
@@ -972,17 +1010,19 @@
     # So ^ABC$ will only allow 'ABC'
     conv_handler = ConversationHandler(
         entry_points=[CommandHandler("start", start)],
         states={
             START_ROUTES: [
                 CallbackQueryHandler(XScanners, pattern="^" + str("CX") + "$"),
                 CallbackQueryHandler(XScanners, pattern="^" + str("CB") + "$"),
+                CallbackQueryHandler(XScanners, pattern="^" + str("CMI") + "$"),
                 # CallbackQueryHandler(XScanners, pattern="^" + str("CG") + "$"),
                 CallbackQueryHandler(Level2, pattern="^" + str("CX_")),
                 CallbackQueryHandler(Level2, pattern="^" + str("CB_")),
+                CallbackQueryHandler(Level2, pattern="^" + str("CMI_")),
                 # CallbackQueryHandler(Level2, pattern="^" + str("CG_")),
                 CallbackQueryHandler(end, pattern="^" + str("CZ") + "$"),
                 CallbackQueryHandler(start, pattern="^"),
             ],
             END_ROUTES: [],
         },
         fallbacks=[CommandHandler("start", start)],
```

### Comparing `pkscreener-0.44.20240505.337/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240505.338/pkscreener/pkscreenercli.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,20 @@
     "-t",
     "--testbuild",
     action="store_true",
     help="Run in test-build mode",
     required=False,
 )
 argParser.add_argument(
+    "--telegram",
+    action="store_true",
+    help="Run with an assumption that this instance is launched via telegram bot",
+    required=False,
+)
+argParser.add_argument(
     "-u",
     "--user",
     help="Telegram user ID to whom the results must be sent.",
     required=False,
 )
 argParser.add_argument(
     "-l",
@@ -234,14 +240,21 @@
 resultStocks = None
 plainResults = None
 start_time = None
 dbTimestamp = None
 elapsed_time = None
 configManager = ConfigManager.tools()
 
+def removeMonitorFile():
+    from PKDevTools.classes import Archiver
+    filePath = os.path.join(Archiver.get_user_outputs_dir(), "monitor_outputs.txt")
+    try:
+        os.remove(filePath)
+    except:
+        pass
 
 def logFilePath():
     try:
         from PKDevTools.classes import Archiver
 
         filePath = os.path.join(Archiver.get_user_outputs_dir(), "pkscreener-logs.txt")
         f = open(filePath, "w")
@@ -299,15 +312,15 @@
                 + colorText.FAIL
                 + "[+] Neither ta-lib nor pandas_ta was located. You need at least one of them to continue! \n[+] Please follow instructions from README file under PKScreener repo: https://github.com/pkjmesra/PKScreener"
                 + colorText.END
             )
             input("Press any key to try anyway...")
 
 def runApplication():
-    from pkscreener.globals import main, sendQuickScanResult, sendGlobalMarketBarometer, updateMenuChoiceHierarchy, isInterrupted, refreshStockData, closeWorkersAndExit
+    from pkscreener.globals import main, sendQuickScanResult,sendMessageToTelegramChannel, sendGlobalMarketBarometer, updateMenuChoiceHierarchy, isInterrupted, refreshStockData, closeWorkersAndExit
     # From a previous call to main with args, it may have been mutated.
     # Let's stock to the original args passed by user
     argsv = argParser.parse_known_args()
     args = argsv[0]
     if args.runintradayanalysis:
         from pkscreener.classes.MenuOptions import menus
         runOptions = menus.allMenus(topLevel="C", index=12)
@@ -404,30 +417,33 @@
             try: 
                 results = None
                 plainResults = None
                 resultStocks = None
                 results, plainResults = main(userArgs=args)
                 if isInterrupted():
                     closeWorkersAndExit()
+                    removeMonitorFile()
                     sys.exit(0)
                 while pipeResults(plainResults,args):
                     results, plainResults = main(userArgs=args)
             except SystemExit:
                 closeWorkersAndExit()
+                removeMonitorFile()
                 sys.exit(0)
             except Exception as e:
                 default_logger().debug(e, exc_info=True)
                 # Probably user cancelled an operation by choosing a cancel sub-menu somewhere
                 pass
             if plainResults is not None and not plainResults.empty:
                 plainResults = plainResults[~plainResults.index.duplicated(keep='first')]
                 results = results[~results.index.duplicated(keep='first')]
                 resultStocks = plainResults.index
             if results is not None and args.monitor and len(monitorOption_org) > 0:
-                MarketMonitor().refresh(screen_df=results,screenOptions=monitorOption_org, chosenMenu=updateMenuChoiceHierarchy(),dbTimestamp=f"{dbTimestamp} | CycleTime:{elapsed_time}s")
+                MarketMonitor().refresh(screen_df=results,screenOptions=monitorOption_org, chosenMenu=updateMenuChoiceHierarchy(),dbTimestamp=f"{dbTimestamp} | CycleTime:{elapsed_time}s",telegram=args.telegram)
+
 
 def pipeResults(prevOutput,args):
     nextOnes = args.options.split(";")
     if len(nextOnes) > 1:
         monitorOption = nextOnes[1]
         if len(monitorOption) == 0:
             return False
@@ -501,14 +517,22 @@
     if args.prodbuild:
         disableSysOut()
 
     if not configManager.checkConfigFile():
         configManager.setConfig(
             ConfigManager.parser, default=True, showFileCreatedText=False
         )
+    if args.telegram:
+        from PKDevTools.classes import Archiver
+        filePath = os.path.join(Archiver.get_user_outputs_dir(), "monitor_outputs.txt")
+        if os.path.exists(filePath):
+            # Since the file exists, it means, there is another instance running
+            sys.exit(0)
+        import atexit
+        atexit.register(removeMonitorFile)
     # Check and see if we're running only the telegram bot
     if args.bot:
         from pkscreener import pkscreenerbot
         pkscreenerbot.runpkscreenerbot()
         return
     
     if args.intraday:
@@ -541,14 +565,15 @@
             + colorText.END
         )
         if args.intraday is None:
             configManager.toggleConfig(candleDuration="1d", clearCache=False)
         runApplication()
         from pkscreener.globals import closeWorkersAndExit
         closeWorkersAndExit()
+        removeMonitorFile()
         sys.exit(0)
     else:
         runApplicationForScreening()
 
 def runLoopOnScheduleOrStdApplication(hasCronInterval):
     if hasCronInterval:
         scheduleNextRun()
@@ -565,31 +590,34 @@
             if shouldBreak:
                 break
             runLoopOnScheduleOrStdApplication(hasCronInterval)
         if args.v:
             disableSysOut(disable=False)
             return
         closeWorkersAndExit()
+        removeMonitorFile()
         sys.exit(0)
     except SystemExit:
         closeWorkersAndExit()
+        removeMonitorFile()
         sys.exit(0)
     except (RuntimeError, Exception) as e:  # pragma: no cover
         default_logger().debug(e, exc_info=True)
         if args.prodbuild:
             disableSysOut(disable=False)
         OutputControls().printOutput(
             f"{e}\n[+] An error occurred! Please run with '-l' option to collect the logs.\n[+] For example, 'pkscreener -l' and then contact the developer!"
         )
         if "RUNNER" in os.environ.keys() or ('PKDevTools_Default_Log_Level' in os.environ.keys() and os.environ["PKDevTools_Default_Log_Level"] != str(log.logging.NOTSET)):
             traceback.print_exc()
         if args.v:
             disableSysOut(disable=False)
             return
         closeWorkersAndExit()
+        removeMonitorFile()
         sys.exit(0)
 
 
 def scheduleNextRun():
     sleepUntilNextExecution = not PKDateUtilities.isTradingTime()
     while sleepUntilNextExecution:
         OutputControls().printOutput(
@@ -626,13 +654,12 @@
             end="\r",
             flush=True,
         )
         sleep(int(args.croninterval) if not args.testbuild else 3)
     runApplication()
     cron_runs += 1
 
-
 if __name__ == "__main__":
     try:
         pkscreenercli()
     except KeyboardInterrupt:
         sys.exit(0)
```

### Comparing `pkscreener-0.44.20240505.337/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240505.338/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240505.337
+Version: 0.44.20240505.338
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240505.337.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240505.338.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.337/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.337/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.336/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240505.337/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240505.337/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240505.338/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240505.337/setup.py` & `pkscreener-0.44.20240505.338/setup.py`

 * *Files identical despite different names*

