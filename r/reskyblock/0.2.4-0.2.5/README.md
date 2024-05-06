# Comparing `tmp/reskyblock-0.2.4.tar.gz` & `tmp/reskyblock-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reskyblock-0.2.4.tar", last modified: Sun May  5 03:41:07 2024, max compression
+gzip compressed data, was "reskyblock-0.2.5.tar", last modified: Mon May  6 16:06:50 2024, max compression
```

## Comparing `reskyblock-0.2.4.tar` & `reskyblock-0.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1072 2024-05-05 03:40:49.117972 reskyblock-0.2.4/LICENSE
--rw-r--r--   0        0        0       13 2024-05-05 03:40:49.117972 reskyblock-0.2.4/README.md
--rw-r--r--   0        0        0     2689 2024-05-05 03:41:07.022198 reskyblock-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      441 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/__init__.py
--rw-r--r--   0        0        0        0 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/__main__.py
--rw-r--r--   0        0        0     9808 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/client.py
--rw-r--r--   0        0        0      212 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/http/__init__.py
--rw-r--r--   0        0        0     2130 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/http/http_adapter.py
--rw-r--r--   0        0        0      387 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/models/__init__.py
--rw-r--r--   0        0        0     1353 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/models/auctions.py
--rw-r--r--   0        0        0      666 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/models/auctions_ended.py
--rw-r--r--   0        0        0      716 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/models/bazaar.py
--rw-r--r--   0        0        0       73 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/nbt/__init__.py
--rw-r--r--   0        0        0     3357 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/nbt/decoder.py
--rw-r--r--   0        0        0        0 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/py.typed
--rw-r--r--   0        0        0      131 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/serialization/__init__.py
--rw-r--r--   0        0        0      992 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/serialization/json.py
--rw-r--r--   0        0        0      575 2024-05-05 03:40:49.117972 reskyblock-0.2.4/src/reskyblock/urls.py
--rw-r--r--   0        0        0        0 2024-05-05 03:40:49.117972 reskyblock-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0  2018239 2024-05-05 03:40:49.129973 reskyblock-0.2.4/tests/data/auctions.json
--rw-r--r--   0        0        0  2039142 2024-05-05 03:40:49.141973 reskyblock-0.2.4/tests/data/auctions2.json
--rw-r--r--   0        0        0   315276 2024-05-05 03:40:49.141973 reskyblock-0.2.4/tests/data/auctions_ended.json
--rw-r--r--   0        0        0  2264250 2024-05-05 03:40:49.149973 reskyblock-0.2.4/tests/data/bazaar.json
--rw-r--r--   0        0        0    89195 2024-05-05 03:40:49.149973 reskyblock-0.2.4/tests/data/item_bytes.txt
--rw-r--r--   0        0        0     3204 2024-05-05 03:40:49.149973 reskyblock-0.2.4/tests/test_client.py
--rw-r--r--   0        0        0      692 2024-05-05 03:40:49.149973 reskyblock-0.2.4/tests/test_httpx_client.py
--rw-r--r--   0        0        0     1992 2024-05-05 03:40:49.149973 reskyblock-0.2.4/tests/test_mock_client.py
--rw-r--r--   0        0        0     8497 2024-05-05 03:40:49.149973 reskyblock-0.2.4/tests/test_nbt.py
--rw-r--r--   0        0        0      819 2024-05-05 03:40:49.149973 reskyblock-0.2.4/tests/test_urls.py
--rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 reskyblock-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-06 16:06:29.642553 reskyblock-0.2.5/LICENSE
+-rw-r--r--   0        0        0       13 2024-05-06 16:06:29.642553 reskyblock-0.2.5/README.md
+-rw-r--r--   0        0        0     2689 2024-05-06 16:06:50.338622 reskyblock-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      514 2024-05-06 16:06:29.642553 reskyblock-0.2.5/src/reskyblock/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 16:06:29.642553 reskyblock-0.2.5/src/reskyblock/__main__.py
+-rw-r--r--   0        0        0     9808 2024-05-06 16:06:29.642553 reskyblock-0.2.5/src/reskyblock/client.py
+-rw-r--r--   0        0        0      212 2024-05-06 16:06:29.642553 reskyblock-0.2.5/src/reskyblock/http/__init__.py
+-rw-r--r--   0        0        0     2130 2024-05-06 16:06:29.642553 reskyblock-0.2.5/src/reskyblock/http/http_adapter.py
+-rw-r--r--   0        0        0      387 2024-05-06 16:06:29.642553 reskyblock-0.2.5/src/reskyblock/models/__init__.py
+-rw-r--r--   0        0        0     1353 2024-05-06 16:06:29.642553 reskyblock-0.2.5/src/reskyblock/models/auctions.py
+-rw-r--r--   0        0        0      666 2024-05-06 16:06:29.642553 reskyblock-0.2.5/src/reskyblock/models/auctions_ended.py
+-rw-r--r--   0        0        0      716 2024-05-06 16:06:29.642553 reskyblock-0.2.5/src/reskyblock/models/bazaar.py
+-rw-r--r--   0        0        0       73 2024-05-06 16:06:29.642553 reskyblock-0.2.5/src/reskyblock/nbt/__init__.py
+-rw-r--r--   0        0        0     3357 2024-05-06 16:06:29.642553 reskyblock-0.2.5/src/reskyblock/nbt/decoder.py
+-rw-r--r--   0        0        0        0 2024-05-06 16:06:29.642553 reskyblock-0.2.5/src/reskyblock/py.typed
+-rw-r--r--   0        0        0      131 2024-05-06 16:06:29.642553 reskyblock-0.2.5/src/reskyblock/serialization/__init__.py
+-rw-r--r--   0        0        0      992 2024-05-06 16:06:29.642553 reskyblock-0.2.5/src/reskyblock/serialization/json.py
+-rw-r--r--   0        0        0      575 2024-05-06 16:06:29.642553 reskyblock-0.2.5/src/reskyblock/urls.py
+-rw-r--r--   0        0        0        0 2024-05-06 16:06:29.642553 reskyblock-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0  2018239 2024-05-06 16:06:29.658553 reskyblock-0.2.5/tests/data/auctions.json
+-rw-r--r--   0        0        0  2039142 2024-05-06 16:06:29.670553 reskyblock-0.2.5/tests/data/auctions2.json
+-rw-r--r--   0        0        0   315276 2024-05-06 16:06:29.670553 reskyblock-0.2.5/tests/data/auctions_ended.json
+-rw-r--r--   0        0        0  2264250 2024-05-06 16:06:29.678553 reskyblock-0.2.5/tests/data/bazaar.json
+-rw-r--r--   0        0        0    89195 2024-05-06 16:06:29.678553 reskyblock-0.2.5/tests/data/item_bytes.txt
+-rw-r--r--   0        0        0     3204 2024-05-06 16:06:29.678553 reskyblock-0.2.5/tests/test_client.py
+-rw-r--r--   0        0        0      692 2024-05-06 16:06:29.678553 reskyblock-0.2.5/tests/test_httpx_client.py
+-rw-r--r--   0        0        0     1992 2024-05-06 16:06:29.678553 reskyblock-0.2.5/tests/test_mock_client.py
+-rw-r--r--   0        0        0     8497 2024-05-06 16:06:29.678553 reskyblock-0.2.5/tests/test_nbt.py
+-rw-r--r--   0        0        0      819 2024-05-06 16:06:29.678553 reskyblock-0.2.5/tests/test_urls.py
+-rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 reskyblock-0.2.5/PKG-INFO
```

### Comparing `reskyblock-0.2.4/LICENSE` & `reskyblock-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/pyproject.toml` & `reskyblock-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "reskyblock"
-version = "0.2.4"
+version = "0.2.5"
 description = "Python API wrapper for Hypixel SkyBlock"
 authors = [
     { name = "ch-iv", email = "alicesummer38@gmail.com" },
 ]
 dependencies = [
     "pyright>=1.1.350",
     "httpx>=0.26.0",
```

### Comparing `reskyblock-0.2.4/src/reskyblock/client.py` & `reskyblock-0.2.5/src/reskyblock/client.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/src/reskyblock/http/http_adapter.py` & `reskyblock-0.2.5/src/reskyblock/http/http_adapter.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/src/reskyblock/models/auctions.py` & `reskyblock-0.2.5/src/reskyblock/models/auctions.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/src/reskyblock/models/auctions_ended.py` & `reskyblock-0.2.5/src/reskyblock/models/auctions_ended.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/src/reskyblock/models/bazaar.py` & `reskyblock-0.2.5/src/reskyblock/models/bazaar.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/src/reskyblock/nbt/decoder.py` & `reskyblock-0.2.5/src/reskyblock/nbt/decoder.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/src/reskyblock/serialization/json.py` & `reskyblock-0.2.5/src/reskyblock/serialization/json.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/src/reskyblock/urls.py` & `reskyblock-0.2.5/src/reskyblock/urls.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/tests/data/auctions.json` & `reskyblock-0.2.5/tests/data/auctions.json`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/tests/data/auctions2.json` & `reskyblock-0.2.5/tests/data/auctions2.json`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/tests/data/auctions_ended.json` & `reskyblock-0.2.5/tests/data/auctions_ended.json`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/tests/data/bazaar.json` & `reskyblock-0.2.5/tests/data/bazaar.json`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/tests/data/item_bytes.txt` & `reskyblock-0.2.5/tests/data/item_bytes.txt`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/tests/test_client.py` & `reskyblock-0.2.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/tests/test_httpx_client.py` & `reskyblock-0.2.5/tests/test_httpx_client.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/tests/test_mock_client.py` & `reskyblock-0.2.5/tests/test_mock_client.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/tests/test_nbt.py` & `reskyblock-0.2.5/tests/test_nbt.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.4/tests/test_urls.py` & `reskyblock-0.2.5/tests/test_urls.py`

 * *Files identical despite different names*

