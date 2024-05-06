# Comparing `tmp/PKNSETools-0.1.20240506.97.tar.gz` & `tmp/PKNSETools-0.1.20240506.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKNSETools-0.1.20240506.97.tar", last modified: Mon May  6 08:40:21 2024, max compression
+gzip compressed data, was "PKNSETools-0.1.20240506.98.tar", last modified: Mon May  6 11:33:31 2024, max compression
```

## Comparing `PKNSETools-0.1.20240506.97.tar` & `PKNSETools-0.1.20240506.98.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 08:40:21.440579 PKNSETools-0.1.20240506.97/
--rw-rw-rw-   0        0        0     2661 2024-05-06 08:40:21.440579 PKNSETools-0.1.20240506.97/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 08:40:21.424947 PKNSETools-0.1.20240506.97/PKNSETools/
-drwxrwxrwx   0        0        0        0 2024-05-06 08:40:21.424947 PKNSETools-0.1.20240506.97/PKNSETools/Benny/
--rw-rw-rw-   0        0        0    34274 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/Benny/NSE.py
--rw-rw-rw-   0        0        0     1198 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/Benny/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:40:21.424947 PKNSETools-0.1.20240506.97/PKNSETools/Nasdaq/
--rw-rw-rw-   0        0        0     3386 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/Nasdaq/PKNasdaqIndex.py
--rw-rw-rw-   0        0        0     1225 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/Nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4806 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/PKAllStocks.py
--rw-rw-rw-   0        0        0    10032 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/PKCompanyGeneral.py
--rw-rw-rw-   0        0        0     3303 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/PKCompanyStock.py
--rw-rw-rw-   0        0        0     2223 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/PKConstants.py
--rw-rw-rw-   0        0        0     5168 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/PKIntraDay.py
--rw-rw-rw-   0        0        0     6446 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    13318 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/PKNSEStockDataFetcher.py
--rw-rw-rw-   0        0        0       30 2024-05-06 08:40:17.000000 PKNSETools-0.1.20240506.97/PKNSETools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:40:21.440579 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/
--rw-rw-rw-   0        0        0     1830 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/NSEStockDB.py
--rw-rw-rw-   0        0        0     1848 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/NSEStockFairValueDB.py
--rw-rw-rw-   0        0        0     1836 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/NSEStockMFIDB.py
--rw-rw-rw-   0        0        0    61961 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
--rw-rw-rw-   0        0        0     1378 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/__init__.py
--rw-rw-rw-   0        0        0     2000 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/error.py
--rw-rw-rw-   0        0        0    40060 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/funds.py
--rw-rw-rw-   0        0        0    22038 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/search.py
--rw-rw-rw-   0        0        0    13495 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/security.py
--rw-rw-rw-   0        0        0    29916 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/stock.py
--rw-rw-rw-   0        0        0    23246 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:40:21.424947 PKNSETools-0.1.20240506.97/PKNSETools.egg-info/
--rw-rw-rw-   0        0        0     2661 2024-05-06 08:40:21.000000 PKNSETools-0.1.20240506.97/PKNSETools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1041 2024-05-06 08:40:21.000000 PKNSETools-0.1.20240506.97/PKNSETools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 08:40:21.000000 PKNSETools-0.1.20240506.97/PKNSETools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-06 08:40:15.000000 PKNSETools-0.1.20240506.97/PKNSETools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       79 2024-05-06 08:40:21.000000 PKNSETools-0.1.20240506.97/PKNSETools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-06 08:40:21.000000 PKNSETools-0.1.20240506.97/PKNSETools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1884 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/README.md
--rw-rw-rw-   0        0        0       86 2024-05-06 08:40:21.440579 PKNSETools-0.1.20240506.97/setup.cfg
--rw-rw-rw-   0        0        0     3832 2024-05-06 08:37:55.000000 PKNSETools-0.1.20240506.97/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:33:31.993979 PKNSETools-0.1.20240506.98/
+-rw-rw-rw-   0        0        0     2661 2024-05-06 11:33:31.993979 PKNSETools-0.1.20240506.98/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 11:33:31.978358 PKNSETools-0.1.20240506.98/PKNSETools/
+drwxrwxrwx   0        0        0        0 2024-05-06 11:33:31.978358 PKNSETools-0.1.20240506.98/PKNSETools/Benny/
+-rw-rw-rw-   0        0        0    34274 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/Benny/NSE.py
+-rw-rw-rw-   0        0        0     1198 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/Benny/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:33:31.993979 PKNSETools-0.1.20240506.98/PKNSETools/Nasdaq/
+-rw-rw-rw-   0        0        0     3386 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/Nasdaq/PKNasdaqIndex.py
+-rw-rw-rw-   0        0        0     1225 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/Nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4806 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/PKAllStocks.py
+-rw-rw-rw-   0        0        0    10032 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/PKCompanyGeneral.py
+-rw-rw-rw-   0        0        0     3303 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/PKCompanyStock.py
+-rw-rw-rw-   0        0        0     2223 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/PKConstants.py
+-rw-rw-rw-   0        0        0     5168 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/PKIntraDay.py
+-rw-rw-rw-   0        0        0    13318 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/PKNSEStockDataFetcher.py
+-rw-rw-rw-   0        0        0       30 2024-05-06 11:33:26.000000 PKNSETools-0.1.20240506.98/PKNSETools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:33:31.993979 PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/
+-rw-rw-rw-   0        0        0     1830 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/NSEStockDB.py
+-rw-rw-rw-   0        0        0     1848 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/NSEStockFairValueDB.py
+-rw-rw-rw-   0        0        0     1836 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/NSEStockMFIDB.py
+-rw-rw-rw-   0        0        0    61961 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
+-rw-rw-rw-   0        0        0     1378 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/__init__.py
+-rw-rw-rw-   0        0        0     2000 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/error.py
+-rw-rw-rw-   0        0        0    40060 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/funds.py
+-rw-rw-rw-   0        0        0    22038 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/search.py
+-rw-rw-rw-   0        0        0    13495 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/security.py
+-rw-rw-rw-   0        0        0    29916 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/stock.py
+-rw-rw-rw-   0        0        0    23246 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:33:31.978358 PKNSETools-0.1.20240506.98/PKNSETools.egg-info/
+-rw-rw-rw-   0        0        0     2661 2024-05-06 11:33:31.000000 PKNSETools-0.1.20240506.98/PKNSETools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2024-05-06 11:33:31.000000 PKNSETools-0.1.20240506.98/PKNSETools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 11:33:31.000000 PKNSETools-0.1.20240506.98/PKNSETools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-06 11:33:24.000000 PKNSETools-0.1.20240506.98/PKNSETools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       79 2024-05-06 11:33:31.000000 PKNSETools-0.1.20240506.98/PKNSETools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-06 11:33:31.000000 PKNSETools-0.1.20240506.98/PKNSETools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1884 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-06 11:33:31.993979 PKNSETools-0.1.20240506.98/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2024-05-06 11:31:10.000000 PKNSETools-0.1.20240506.98/setup.py
```

### Comparing `PKNSETools-0.1.20240506.97/PKG-INFO` & `PKNSETools-0.1.20240506.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240506.97
+Version: 0.1.20240506.98
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240506.97.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240506.98.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/Benny/NSE.py` & `PKNSETools-0.1.20240506.98/PKNSETools/Benny/NSE.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/Benny/__init__.py` & `PKNSETools-0.1.20240506.98/PKNSETools/Benny/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/Nasdaq/PKNasdaqIndex.py` & `PKNSETools-0.1.20240506.98/PKNSETools/Nasdaq/PKNasdaqIndex.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/Nasdaq/__init__.py` & `PKNSETools-0.1.20240506.98/PKNSETools/Nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/PKAllStocks.py` & `PKNSETools-0.1.20240506.98/PKNSETools/PKAllStocks.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/PKCompanyGeneral.py` & `PKNSETools-0.1.20240506.98/PKNSETools/PKCompanyGeneral.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/PKCompanyStock.py` & `PKNSETools-0.1.20240506.98/PKNSETools/PKCompanyStock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/PKConstants.py` & `PKNSETools-0.1.20240506.98/PKNSETools/PKConstants.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/PKIntraDay.py` & `PKNSETools-0.1.20240506.98/PKNSETools/PKIntraDay.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/PKNSEStockDataFetcher.py` & `PKNSETools-0.1.20240506.98/PKNSETools/PKNSEStockDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/NSEStockDB.py` & `PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/NSEStockDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/NSEStockFairValueDB.py` & `PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/NSEStockFairValueDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/NSEStockMFIDB.py` & `PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/NSEStockMFIDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/PKMorningstarDataFetcher.py` & `PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/PKMorningstarDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/__init__.py` & `PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/error.py` & `PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/error.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/funds.py` & `PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/funds.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/search.py` & `PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/search.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/security.py` & `PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/security.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/stock.py` & `PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/stock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools/morningstartools/utils.py` & `PKNSETools-0.1.20240506.98/PKNSETools/morningstartools/utils.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools.egg-info/PKG-INFO` & `PKNSETools-0.1.20240506.98/PKNSETools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240506.97
+Version: 0.1.20240506.98
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240506.97.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240506.98.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240506.97/PKNSETools.egg-info/SOURCES.txt` & `PKNSETools-0.1.20240506.98/PKNSETools.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 setup.cfg
 setup.py
 PKNSETools/PKAllStocks.py
 PKNSETools/PKCompanyGeneral.py
 PKNSETools/PKCompanyStock.py
 PKNSETools/PKConstants.py
 PKNSETools/PKIntraDay.py
-PKNSETools/PKMultiProcessorClient.py
 PKNSETools/PKNSEStockDataFetcher.py
 PKNSETools/__init__.py
 PKNSETools.egg-info/PKG-INFO
 PKNSETools.egg-info/SOURCES.txt
 PKNSETools.egg-info/dependency_links.txt
 PKNSETools.egg-info/not-zip-safe
 PKNSETools.egg-info/requires.txt
```

### Comparing `PKNSETools-0.1.20240506.97/README.md` & `PKNSETools-0.1.20240506.98/README.md`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240506.97/setup.py` & `PKNSETools-0.1.20240506.98/setup.py`

 * *Files identical despite different names*

