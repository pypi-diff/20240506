# Comparing `tmp/PKNSETools-0.1.20240505.96.tar.gz` & `tmp/PKNSETools-0.1.20240506.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKNSETools-0.1.20240505.96.tar", last modified: Sun May  5 06:18:50 2024, max compression
+gzip compressed data, was "PKNSETools-0.1.20240506.97.tar", last modified: Mon May  6 08:40:21 2024, max compression
```

## Comparing `PKNSETools-0.1.20240505.96.tar` & `PKNSETools-0.1.20240506.97.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 06:18:50.313278 PKNSETools-0.1.20240505.96/
--rw-rw-rw-   0        0        0     2661 2024-05-05 06:18:50.313278 PKNSETools-0.1.20240505.96/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-05 06:18:50.297650 PKNSETools-0.1.20240505.96/PKNSETools/
-drwxrwxrwx   0        0        0        0 2024-05-05 06:18:50.297650 PKNSETools-0.1.20240505.96/PKNSETools/Benny/
--rw-rw-rw-   0        0        0    34274 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/Benny/NSE.py
--rw-rw-rw-   0        0        0     1198 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/Benny/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 06:18:50.297650 PKNSETools-0.1.20240505.96/PKNSETools/Nasdaq/
--rw-rw-rw-   0        0        0     3386 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/Nasdaq/PKNasdaqIndex.py
--rw-rw-rw-   0        0        0     1225 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/Nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4806 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/PKAllStocks.py
--rw-rw-rw-   0        0        0    10032 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/PKCompanyGeneral.py
--rw-rw-rw-   0        0        0     3303 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/PKCompanyStock.py
--rw-rw-rw-   0        0        0     2223 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/PKConstants.py
--rw-rw-rw-   0        0        0     5168 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/PKIntraDay.py
--rw-rw-rw-   0        0        0     6446 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    12688 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/PKNSEStockDataFetcher.py
--rw-rw-rw-   0        0        0       30 2024-05-05 06:18:45.000000 PKNSETools-0.1.20240505.96/PKNSETools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 06:18:50.313278 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/
--rw-rw-rw-   0        0        0     1830 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/NSEStockDB.py
--rw-rw-rw-   0        0        0     1848 2024-05-05 06:16:43.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/NSEStockFairValueDB.py
--rw-rw-rw-   0        0        0     1836 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/NSEStockMFIDB.py
--rw-rw-rw-   0        0        0    61961 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
--rw-rw-rw-   0        0        0     1378 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/__init__.py
--rw-rw-rw-   0        0        0     2000 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/error.py
--rw-rw-rw-   0        0        0    40060 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/funds.py
--rw-rw-rw-   0        0        0    22038 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/search.py
--rw-rw-rw-   0        0        0    13495 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/security.py
--rw-rw-rw-   0        0        0    29916 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/stock.py
--rw-rw-rw-   0        0        0    23246 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-05 06:18:50.297650 PKNSETools-0.1.20240505.96/PKNSETools.egg-info/
--rw-rw-rw-   0        0        0     2661 2024-05-05 06:18:50.000000 PKNSETools-0.1.20240505.96/PKNSETools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1041 2024-05-05 06:18:50.000000 PKNSETools-0.1.20240505.96/PKNSETools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 06:18:50.000000 PKNSETools-0.1.20240505.96/PKNSETools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-05 06:18:43.000000 PKNSETools-0.1.20240505.96/PKNSETools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       79 2024-05-05 06:18:50.000000 PKNSETools-0.1.20240505.96/PKNSETools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-05 06:18:50.000000 PKNSETools-0.1.20240505.96/PKNSETools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1884 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/README.md
--rw-rw-rw-   0        0        0       86 2024-05-05 06:18:50.313278 PKNSETools-0.1.20240505.96/setup.cfg
--rw-rw-rw-   0        0        0     3832 2024-05-05 06:16:44.000000 PKNSETools-0.1.20240505.96/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:40:21.440579 PKNSETools-0.1.20240506.97/
+-rw-rw-rw-   0        0        0     2661 2024-05-06 08:40:21.440579 PKNSETools-0.1.20240506.97/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 08:40:21.424947 PKNSETools-0.1.20240506.97/PKNSETools/
+drwxrwxrwx   0        0        0        0 2024-05-06 08:40:21.424947 PKNSETools-0.1.20240506.97/PKNSETools/Benny/
+-rw-rw-rw-   0        0        0    34274 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/Benny/NSE.py
+-rw-rw-rw-   0        0        0     1198 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/Benny/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:40:21.424947 PKNSETools-0.1.20240506.97/PKNSETools/Nasdaq/
+-rw-rw-rw-   0        0        0     3386 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/Nasdaq/PKNasdaqIndex.py
+-rw-rw-rw-   0        0        0     1225 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/Nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4806 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/PKAllStocks.py
+-rw-rw-rw-   0        0        0    10032 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/PKCompanyGeneral.py
+-rw-rw-rw-   0        0        0     3303 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/PKCompanyStock.py
+-rw-rw-rw-   0        0        0     2223 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/PKConstants.py
+-rw-rw-rw-   0        0        0     5168 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/PKIntraDay.py
+-rw-rw-rw-   0        0        0     6446 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    13318 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/PKNSEStockDataFetcher.py
+-rw-rw-rw-   0        0        0       30 2024-05-06 08:40:17.000000 PKNSETools-0.1.20240506.97/PKNSETools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:40:21.440579 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/
+-rw-rw-rw-   0        0        0     1830 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/NSEStockDB.py
+-rw-rw-rw-   0        0        0     1848 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/NSEStockFairValueDB.py
+-rw-rw-rw-   0        0        0     1836 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/NSEStockMFIDB.py
+-rw-rw-rw-   0        0        0    61961 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
+-rw-rw-rw-   0        0        0     1378 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/__init__.py
+-rw-rw-rw-   0        0        0     2000 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/error.py
+-rw-rw-rw-   0        0        0    40060 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/funds.py
+-rw-rw-rw-   0        0        0    22038 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/search.py
+-rw-rw-rw-   0        0        0    13495 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/security.py
+-rw-rw-rw-   0        0        0    29916 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/stock.py
+-rw-rw-rw-   0        0        0    23246 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:40:21.424947 PKNSETools-0.1.20240506.97/PKNSETools.egg-info/
+-rw-rw-rw-   0        0        0     2661 2024-05-06 08:40:21.000000 PKNSETools-0.1.20240506.97/PKNSETools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1041 2024-05-06 08:40:21.000000 PKNSETools-0.1.20240506.97/PKNSETools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 08:40:21.000000 PKNSETools-0.1.20240506.97/PKNSETools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-06 08:40:15.000000 PKNSETools-0.1.20240506.97/PKNSETools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       79 2024-05-06 08:40:21.000000 PKNSETools-0.1.20240506.97/PKNSETools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-06 08:40:21.000000 PKNSETools-0.1.20240506.97/PKNSETools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1884 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-06 08:40:21.440579 PKNSETools-0.1.20240506.97/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/setup.py
```

### Comparing `PKNSETools-0.1.20240505.96/PKG-INFO` & `PKNSETools-0.1.20240506.97/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240505.96
+Version: 0.1.20240506.97
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240505.96.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240506.97.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/Benny/NSE.py` & `PKNSETools-0.1.20240506.97/PKNSETools/Benny/NSE.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/Benny/__init__.py` & `PKNSETools-0.1.20240506.97/PKNSETools/Benny/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/Nasdaq/PKNasdaqIndex.py` & `PKNSETools-0.1.20240506.97/PKNSETools/Nasdaq/PKNasdaqIndex.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/Nasdaq/__init__.py` & `PKNSETools-0.1.20240506.97/PKNSETools/Nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/PKAllStocks.py` & `PKNSETools-0.1.20240506.97/PKNSETools/PKAllStocks.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/PKCompanyGeneral.py` & `PKNSETools-0.1.20240506.97/PKNSETools/PKCompanyGeneral.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/PKCompanyStock.py` & `PKNSETools-0.1.20240506.97/PKNSETools/PKCompanyStock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/PKConstants.py` & `PKNSETools-0.1.20240506.97/PKNSETools/PKConstants.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/PKIntraDay.py` & `PKNSETools-0.1.20240506.97/PKNSETools/PKIntraDay.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/PKMultiProcessorClient.py` & `PKNSETools-0.1.20240506.97/PKNSETools/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/PKNSEStockDataFetcher.py` & `PKNSETools-0.1.20240506.97/PKNSETools/PKNSEStockDataFetcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -218,38 +218,56 @@
         cm_holidays.extend(cm_lastyear)
         raw["CM"] = cm_holidays
         return cm_holidays, raw
 
     def capitalMarketStatus(self, exchange="^NSEI"):
         # nse  = NSE(Archiver.get_user_outputs_dir())
         ticker = yf.Ticker(exchange) # ^IXIC
-        info = ticker.info
-        md = ticker.get_history_metadata()
-        ltd = md["regularMarketTime"]
-        ctp = md["currentTradingPeriod"]
-        tzName = md["exchangeTimezoneName"]
-        lastTradeDate = pd.to_datetime(ltd, unit='s', utc=True).tz_convert(tzName)
-        basicInfo = ticker.get_fast_info()
-        todayClose = pd.to_datetime(ctp["regular"]["end"], unit='s', utc=True).tz_convert(tzName)
-        todayOpen = pd.to_datetime(ctp["regular"]["start"], unit='s', utc=True).tz_convert(tzName)
+        try:
+            info = ticker.info
+        except:
+            info = {"longName":exchange}
+            pass
+        try:
+            md = ticker.get_history_metadata()
+            ltd = md["regularMarketTime"]
+            ctp = md["currentTradingPeriod"]
+            tzName = md["exchangeTimezoneName"]
+            lastTradeDate = pd.to_datetime(ltd, unit='s', utc=True).tz_convert(tzName)
+        except:
+            tzName = "Asia/Kolkata"
+            lastTradeDate = PKDateUtilities.currentDateTime()
+            pass
+        try:
+            basicInfo = ticker.get_fast_info()
+        except:
+            basicInfo = {"last_price":0,"regular_market_previous_close":0}
+            pass
+        try:
+            todayClose = pd.to_datetime(ctp["regular"]["end"], unit='s', utc=True).tz_convert(tzName)
+            todayOpen = pd.to_datetime(ctp["regular"]["start"], unit='s', utc=True).tz_convert(tzName)
+        except:
+            todayClose = PKDateUtilities.currentDateTime()
+            todayOpen = PKDateUtilities.currentDateTime()
+            pass
         now = PKDateUtilities.currentDateTime().astimezone(tz=pytz.timezone(tzName))
         ts = datetime.datetime.timestamp(now)
         now = pd.to_datetime(ts, unit='s', utc=True).tz_convert(tzName)
         # isClosed = now < todayOpen and now < todayClose
         isOpen = now >= todayOpen and todayClose >= now
         status = "Open" if isOpen else "Closed"
         lastPrice = round(basicInfo["last_price"],2)
         prevClose = round(basicInfo["regular_market_previous_close"],2)
         change = round(lastPrice - prevClose,2)
         pctChange = round(100*change/prevClose,2)
         tradeDate = lastTradeDate.strftime("%Y-%m-%d")
         
         if len(status) > 0:
-            change = ((colorText.GREEN +"▲")if change >=0 else colorText.FAIL+"▼") + str(change) + colorText.END
-            pctChange = (colorText.GREEN if pctChange >=0 else colorText.FAIL) + str(pctChange) + colorText.END
+            change = ((colorText.GREEN +"▲")if change >=0 else colorText.FAIL+"▼") + str(change if pd.notna(change) else "?") + colorText.END
+            pctChange = (colorText.GREEN if pctChange >=0 else colorText.FAIL) + str(pctChange if pd.notna(pctChange) else "?") + colorText.END
             marketStatusLong = f'{info["longName"]} | {status} | {tradeDate} | {lastPrice} | {change} ({pctChange}%)'
         return status, marketStatusLong,tradeDate
 
 # f = nseStockDataFetcher()
 # f.capitalMarketStatus(exchange="^NSEI")
```

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/NSEStockDB.py` & `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/NSEStockDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/NSEStockFairValueDB.py` & `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/NSEStockFairValueDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/NSEStockMFIDB.py` & `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/NSEStockMFIDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/PKMorningstarDataFetcher.py` & `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/PKMorningstarDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/__init__.py` & `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/error.py` & `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/error.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/funds.py` & `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/funds.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/search.py` & `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/search.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/security.py` & `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/security.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/stock.py` & `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/stock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools/morningstartools/utils.py` & `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/utils.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools.egg-info/PKG-INFO` & `PKNSETools-0.1.20240506.97/PKNSETools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240505.96
+Version: 0.1.20240506.97
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240505.96.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240506.97.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240505.96/PKNSETools.egg-info/SOURCES.txt` & `PKNSETools-0.1.20240506.97/PKNSETools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/README.md` & `PKNSETools-0.1.20240506.97/README.md`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240505.96/setup.py` & `PKNSETools-0.1.20240506.97/setup.py`

 * *Files identical despite different names*

