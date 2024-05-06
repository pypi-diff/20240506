# Comparing `tmp/tokyo_stock_exchange-0.0.1.tar.gz` & `tmp/tokyo_stock_exchange-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokyo_stock_exchange-0.0.1.tar", last modified: Mon May  6 09:02:12 2024, max compression
+gzip compressed data, was "tokyo_stock_exchange-0.0.2.tar", last modified: Mon May  6 09:42:12 2024, max compression
```

## Comparing `tokyo_stock_exchange-0.0.1.tar` & `tokyo_stock_exchange-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxr-xr-x   0 penguin   (1000) penguin   (1000)        0 2024-05-06 09:02:12.655567 tokyo_stock_exchange-0.0.1/
--rw-r--r--   0 penguin   (1000) penguin   (1000)     1067 2024-05-06 08:41:22.000000 tokyo_stock_exchange-0.0.1/LICENSE
--rw-r--r--   0 penguin   (1000) penguin   (1000)       36 2024-05-06 05:16:16.000000 tokyo_stock_exchange-0.0.1/MANIFEST.in
--rw-r--r--   0 penguin   (1000) penguin   (1000)     6445 2024-05-06 09:02:12.655567 tokyo_stock_exchange-0.0.1/PKG-INFO
--rw-r--r--   0 penguin   (1000) penguin   (1000)     5881 2024-05-06 08:37:42.000000 tokyo_stock_exchange-0.0.1/README.md
--rw-r--r--   0 penguin   (1000) penguin   (1000)      531 2024-05-06 09:02:08.000000 tokyo_stock_exchange-0.0.1/pyproject.toml
--rw-r--r--   0 penguin   (1000) penguin   (1000)       38 2024-05-06 09:02:12.655567 tokyo_stock_exchange-0.0.1/setup.cfg
--rw-r--r--   0 penguin   (1000) penguin   (1000)      423 2024-05-06 08:42:28.000000 tokyo_stock_exchange-0.0.1/setup.py
-drwxr-xr-x   0 penguin   (1000) penguin   (1000)        0 2024-05-06 09:02:12.655567 tokyo_stock_exchange-0.0.1/tokyo_stock_exchange/
--rw-r--r--   0 penguin   (1000) penguin   (1000)        0 2024-05-06 04:07:24.000000 tokyo_stock_exchange-0.0.1/tokyo_stock_exchange/__init__.py
--rw-r--r--   0 penguin   (1000) penguin   (1000)   534694 2024-05-06 04:06:55.000000 tokyo_stock_exchange-0.0.1/tokyo_stock_exchange/tse.csv
--rw-r--r--   0 penguin   (1000) penguin   (1000)     6151 2024-05-06 08:06:00.000000 tokyo_stock_exchange-0.0.1/tokyo_stock_exchange/tse.py
--rw-r--r--   0 penguin   (1000) penguin   (1000)   533650 2024-05-06 06:58:35.000000 tokyo_stock_exchange-0.0.1/tokyo_stock_exchange/tse20240229.csv
-drwxr-xr-x   0 penguin   (1000) penguin   (1000)        0 2024-05-06 09:02:12.655567 tokyo_stock_exchange-0.0.1/tokyo_stock_exchange.egg-info/
--rw-r--r--   0 penguin   (1000) penguin   (1000)     6445 2024-05-06 09:02:12.000000 tokyo_stock_exchange-0.0.1/tokyo_stock_exchange.egg-info/PKG-INFO
--rw-r--r--   0 penguin   (1000) penguin   (1000)      356 2024-05-06 09:02:12.000000 tokyo_stock_exchange-0.0.1/tokyo_stock_exchange.egg-info/SOURCES.txt
--rw-r--r--   0 penguin   (1000) penguin   (1000)        1 2024-05-06 09:02:12.000000 tokyo_stock_exchange-0.0.1/tokyo_stock_exchange.egg-info/dependency_links.txt
--rw-r--r--   0 penguin   (1000) penguin   (1000)       21 2024-05-06 09:02:12.000000 tokyo_stock_exchange-0.0.1/tokyo_stock_exchange.egg-info/top_level.txt
+drwxr-xr-x   0 penguin   (1000) penguin   (1000)        0 2024-05-06 09:42:12.185507 tokyo_stock_exchange-0.0.2/
+-rw-r--r--   0 penguin   (1000) penguin   (1000)     1067 2024-05-06 08:41:22.000000 tokyo_stock_exchange-0.0.2/LICENSE
+-rw-r--r--   0 penguin   (1000) penguin   (1000)       36 2024-05-06 05:16:16.000000 tokyo_stock_exchange-0.0.2/MANIFEST.in
+-rw-r--r--   0 penguin   (1000) penguin   (1000)     6452 2024-05-06 09:42:12.185507 tokyo_stock_exchange-0.0.2/PKG-INFO
+-rw-r--r--   0 penguin   (1000) penguin   (1000)     5881 2024-05-06 08:37:42.000000 tokyo_stock_exchange-0.0.2/README.md
+-rw-r--r--   0 penguin   (1000) penguin   (1000)      705 2024-05-06 09:38:02.000000 tokyo_stock_exchange-0.0.2/pyproject.toml
+-rw-r--r--   0 penguin   (1000) penguin   (1000)       38 2024-05-06 09:42:12.185507 tokyo_stock_exchange-0.0.2/setup.cfg
+drwxr-xr-x   0 penguin   (1000) penguin   (1000)        0 2024-05-06 09:42:12.185507 tokyo_stock_exchange-0.0.2/tokyo_stock_exchange/
+drwxr-xr-x   0 penguin   (1000) penguin   (1000)        0 2024-05-06 09:42:12.185507 tokyo_stock_exchange-0.0.2/tokyo_stock_exchange/tokyo_stock_exchange.egg-info/
+-rw-r--r--   0 penguin   (1000) penguin   (1000)     6452 2024-05-06 09:42:12.000000 tokyo_stock_exchange-0.0.2/tokyo_stock_exchange/tokyo_stock_exchange.egg-info/PKG-INFO
+-rw-r--r--   0 penguin   (1000) penguin   (1000)      397 2024-05-06 09:42:12.000000 tokyo_stock_exchange-0.0.2/tokyo_stock_exchange/tokyo_stock_exchange.egg-info/SOURCES.txt
+-rw-r--r--   0 penguin   (1000) penguin   (1000)        1 2024-05-06 09:42:12.000000 tokyo_stock_exchange-0.0.2/tokyo_stock_exchange/tokyo_stock_exchange.egg-info/dependency_links.txt
+-rw-r--r--   0 penguin   (1000) penguin   (1000)        7 2024-05-06 09:42:12.000000 tokyo_stock_exchange-0.0.2/tokyo_stock_exchange/tokyo_stock_exchange.egg-info/requires.txt
+-rw-r--r--   0 penguin   (1000) penguin   (1000)        1 2024-05-06 09:42:12.000000 tokyo_stock_exchange-0.0.2/tokyo_stock_exchange/tokyo_stock_exchange.egg-info/top_level.txt
+-rw-r--r--   0 penguin   (1000) penguin   (1000)   534694 2024-05-06 04:06:55.000000 tokyo_stock_exchange-0.0.2/tokyo_stock_exchange/tse.csv
```

### Comparing `tokyo_stock_exchange-0.0.1/LICENSE` & `tokyo_stock_exchange-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tokyo_stock_exchange-0.0.1/PKG-INFO` & `tokyo_stock_exchange-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: tokyo-stock-exchange
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python library for accessing Tokyo Stock Exchange data.
-Author: AKB428
 Author-email: AKB428 <otoraru@gmail.com>
 Project-URL: Homepage, https://github.com/AKB428/tokyo-stock-exchange
 Project-URL: Issues, https://github.com/AKB428/tokyo-stock-exchange/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
 
 # Tokyo Stock Exchange Library
 
 `tokyo-stock-exchange`は東京証券取引所の証券コードを扱うPythonライブラリです。株式のコードや名称、分類情報に基づいて詳細なデータを照会する機能を提供します。
 
 ## 特徴
```

### Comparing `tokyo_stock_exchange-0.0.1/README.md` & `tokyo_stock_exchange-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tokyo_stock_exchange-0.0.1/tokyo_stock_exchange/tse.csv` & `tokyo_stock_exchange-0.0.2/tokyo_stock_exchange/tse.csv`

 * *Files identical despite different names*

### Comparing `tokyo_stock_exchange-0.0.1/tokyo_stock_exchange.egg-info/PKG-INFO` & `tokyo_stock_exchange-0.0.2/tokyo_stock_exchange/tokyo_stock_exchange.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: tokyo-stock-exchange
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python library for accessing Tokyo Stock Exchange data.
-Author: AKB428
 Author-email: AKB428 <otoraru@gmail.com>
 Project-URL: Homepage, https://github.com/AKB428/tokyo-stock-exchange
 Project-URL: Issues, https://github.com/AKB428/tokyo-stock-exchange/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
 
 # Tokyo Stock Exchange Library
 
 `tokyo-stock-exchange`は東京証券取引所の証券コードを扱うPythonライブラリです。株式のコードや名称、分類情報に基づいて詳細なデータを照会する機能を提供します。
 
 ## 特徴
```

