# Comparing `tmp/defillama-2.2.0.tar.gz` & `tmp/defillama-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defillama-2.2.0.tar", last modified: Sat Apr 27 16:49:34 2024, max compression
+gzip compressed data, was "defillama-2.2.1.tar", last modified: Mon May  6 10:09:41 2024, max compression
```

## Comparing `defillama-2.2.0.tar` & `defillama-2.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:49:34.920696 defillama-2.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:49:34.920696 defillama-2.2.0/DeFiLlama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-27 16:49:34.000000 defillama-2.2.0/DeFiLlama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-27 16:49:34.000000 defillama-2.2.0/DeFiLlama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:49:34.000000 defillama-2.2.0/DeFiLlama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-27 16:49:34.000000 defillama-2.2.0/DeFiLlama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 16:49:34.000000 defillama-2.2.0/DeFiLlama.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-27 16:49:24.000000 defillama-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-27 16:49:34.920696 defillama-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-27 16:49:24.000000 defillama-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:49:34.916696 defillama-2.2.0/defillama/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-27 16:49:24.000000 defillama-2.2.0/defillama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-27 16:49:24.000000 defillama-2.2.0/defillama/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-04-27 16:49:24.000000 defillama-2.2.0/defillama/defillama.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 16:49:34.920696 defillama-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-27 16:49:24.000000 defillama-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:49:34.920696 defillama-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-27 16:49:24.000000 defillama-2.2.0/tests/test_defillama.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:09:41.485442 defillama-2.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:09:41.481442 defillama-2.2.1/DeFiLlama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-06 10:09:41.000000 defillama-2.2.1/DeFiLlama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-06 10:09:41.000000 defillama-2.2.1/DeFiLlama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:09:41.000000 defillama-2.2.1/DeFiLlama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 10:09:41.000000 defillama-2.2.1/DeFiLlama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 10:09:41.000000 defillama-2.2.1/DeFiLlama.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 10:09:33.000000 defillama-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-06 10:09:41.485442 defillama-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-06 10:09:33.000000 defillama-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:09:41.481442 defillama-2.2.1/defillama/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-06 10:09:33.000000 defillama-2.2.1/defillama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-06 10:09:33.000000 defillama-2.2.1/defillama/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-05-06 10:09:33.000000 defillama-2.2.1/defillama/defillama.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 10:09:41.485442 defillama-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-06 10:09:33.000000 defillama-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:09:41.481442 defillama-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-06 10:09:33.000000 defillama-2.2.1/tests/test_defillama.py
```

### Comparing `defillama-2.2.0/DeFiLlama.egg-info/PKG-INFO` & `defillama-2.2.1/DeFiLlama.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeFiLlama
-Version: 2.2.0
+Version: 2.2.1
 Summary: Unofficial DeFi Llama API client.
 Home-page: https://github.com/itzmestar/DeFiLlama
 Author: Tarique Anwer
 Author-email: itzmetariq@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `defillama-2.2.0/LICENSE` & `defillama-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `defillama-2.2.0/PKG-INFO` & `defillama-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeFiLlama
-Version: 2.2.0
+Version: 2.2.1
 Summary: Unofficial DeFi Llama API client.
 Home-page: https://github.com/itzmestar/DeFiLlama
 Author: Tarique Anwer
 Author-email: itzmetariq@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `defillama-2.2.0/README.md` & `defillama-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `defillama-2.2.0/defillama/defillama.py` & `defillama-2.2.1/defillama/defillama.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         path = f'/tvl/{protocol}'
 
         return self._get(path)
 
     def get_chains_current_tvl(self):
         """
         Returns list of current TVL of all chains.
-        
+
         :return: JSON response
         """
         path = f'/v2/chains'
 
         return self._get(path)
 
     # ##### Coins EPs ###### #
@@ -330,13 +330,13 @@
 
         return self._get(path, params=params)
 
     def get_fees_protocol(self, protocol, dataType='dailyFees'):
         """
             Get summary of protocol fees and revenue with historical data
         """
-        path = f'/overview/fees/{protocol}'
+        path = f'/summary/fees/{protocol}'
         params = {
             'dataType': dataType
         }
 
         return self._get(path, params=params)
```

### Comparing `defillama-2.2.0/setup.py` & `defillama-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `defillama-2.2.0/tests/test_defillama.py` & `defillama-2.2.1/tests/test_defillama.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from unittest import TestCase
-
 import pytest
 
 
 @pytest.mark.usefixtures('llama')
 class TestDefiLlama:
     """
     Test class for DefiLlama
```

