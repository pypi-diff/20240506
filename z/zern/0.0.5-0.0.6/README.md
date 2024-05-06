# Comparing `tmp/zern-0.0.5.tar.gz` & `tmp/zern-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zern-0.0.5.tar", last modified: Thu May  2 19:53:11 2024, max compression
+gzip compressed data, was "zern-0.0.6.tar", last modified: Mon May  6 05:07:01 2024, max compression
```

## Comparing `zern-0.0.5.tar` & `zern-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:53:11.553616 zern-0.0.5/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     1071 2024-05-02 15:26:31.000000 zern-0.0.5/LICENSE
--rw-r--r--   0 harsha    (1000) harsha    (1000)     6347 2024-05-02 19:53:11.553616 zern-0.0.5/PKG-INFO
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     5716 2024-05-02 15:26:53.000000 zern-0.0.5/README.md
--rw-rw-r--   0 harsha    (1000) harsha    (1000)      772 2024-05-02 19:52:26.000000 zern-0.0.5/pyproject.toml
--rw-rw-r--   0 harsha    (1000) harsha    (1000)       38 2024-05-02 19:53:11.553616 zern-0.0.5/setup.cfg
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:53:11.549616 zern-0.0.5/src/
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:53:11.553616 zern-0.0.5/src/zern/
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:53:11.553616 zern-0.0.5/src/zern/Core/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     3798 2024-05-02 06:23:51.000000 zern-0.0.5/src/zern/Core/session.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     4646 2024-05-02 19:27:04.000000 zern-0.0.5/src/zern/Core/trader.py
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:53:11.553616 zern-0.0.5/src/zern/Core/websocket_connection/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     3534 2024-05-02 07:34:58.000000 zern-0.0.5/src/zern/Core/websocket_connection/ticker.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)       61 2024-04-24 18:27:30.000000 zern-0.0.5/src/zern/__init__.py
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:53:11.553616 zern-0.0.5/src/zern/utils/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     1861 2024-04-21 19:33:12.000000 zern-0.0.5/src/zern/utils/OrderedList.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     2280 2024-05-02 05:29:49.000000 zern-0.0.5/src/zern/utils/Types.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     6314 2024-05-02 05:36:04.000000 zern-0.0.5/src/zern/utils/parsing.py
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:53:11.553616 zern-0.0.5/src/zern.egg-info/
--rw-r--r--   0 harsha    (1000) harsha    (1000)     6347 2024-05-02 19:53:11.000000 zern-0.0.5/src/zern.egg-info/PKG-INFO
--rw-rw-r--   0 harsha    (1000) harsha    (1000)      386 2024-05-02 19:53:11.000000 zern-0.0.5/src/zern.egg-info/SOURCES.txt
--rw-rw-r--   0 harsha    (1000) harsha    (1000)        1 2024-05-02 19:53:11.000000 zern-0.0.5/src/zern.egg-info/dependency_links.txt
--rw-rw-r--   0 harsha    (1000) harsha    (1000)       32 2024-05-02 19:53:11.000000 zern-0.0.5/src/zern.egg-info/requires.txt
--rw-rw-r--   0 harsha    (1000) harsha    (1000)        5 2024-05-02 19:53:11.000000 zern-0.0.5/src/zern.egg-info/top_level.txt
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 05:07:01.684773 zern-0.0.6/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     1071 2024-05-02 15:26:31.000000 zern-0.0.6/LICENSE
+-rw-r--r--   0 harsha    (1000) harsha    (1000)     6419 2024-05-06 05:07:01.684773 zern-0.0.6/PKG-INFO
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     5788 2024-05-06 04:59:34.000000 zern-0.0.6/README.md
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)      772 2024-05-06 05:06:43.000000 zern-0.0.6/pyproject.toml
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)       38 2024-05-06 05:07:01.684773 zern-0.0.6/setup.cfg
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 05:07:01.680773 zern-0.0.6/src/
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 05:07:01.680773 zern-0.0.6/src/zern/
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 05:07:01.684773 zern-0.0.6/src/zern/Core/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     3798 2024-05-02 06:23:51.000000 zern-0.0.6/src/zern/Core/session.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     4646 2024-05-02 19:27:04.000000 zern-0.0.6/src/zern/Core/trader.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 05:07:01.684773 zern-0.0.6/src/zern/Core/websocket/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     3521 2024-05-06 05:05:18.000000 zern-0.0.6/src/zern/Core/websocket/ticker.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 05:07:01.684773 zern-0.0.6/src/zern/Core/websocket_connection/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     3534 2024-05-02 07:34:58.000000 zern-0.0.6/src/zern/Core/websocket_connection/ticker.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)       61 2024-04-24 18:27:30.000000 zern-0.0.6/src/zern/__init__.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 05:07:01.684773 zern-0.0.6/src/zern/utils/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     1861 2024-04-21 19:33:12.000000 zern-0.0.6/src/zern/utils/OrderedList.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     2280 2024-05-02 05:29:49.000000 zern-0.0.6/src/zern/utils/Types.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     6314 2024-05-02 05:36:04.000000 zern-0.0.6/src/zern/utils/parsing.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 05:07:01.684773 zern-0.0.6/src/zern.egg-info/
+-rw-r--r--   0 harsha    (1000) harsha    (1000)     6419 2024-05-06 05:07:01.000000 zern-0.0.6/src/zern.egg-info/PKG-INFO
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)      420 2024-05-06 05:07:01.000000 zern-0.0.6/src/zern.egg-info/SOURCES.txt
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)        1 2024-05-06 05:07:01.000000 zern-0.0.6/src/zern.egg-info/dependency_links.txt
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)       32 2024-05-06 05:07:01.000000 zern-0.0.6/src/zern.egg-info/requires.txt
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)        5 2024-05-06 05:07:01.000000 zern-0.0.6/src/zern.egg-info/top_level.txt
```

### Comparing `zern-0.0.5/LICENSE` & `zern-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zern-0.0.5/PKG-INFO` & `zern-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zern
-Version: 0.0.5
+Version: 0.0.6
 Summary: An unofficial client library using Zerodha web api for live data and historical data
 Author-email: Harsha Avapati <harshaavapati@gmail.com>
 Project-URL: Homepage, https://github.com/ExBlacklight/Zern
 Project-URL: Issues, https://github.com/ExBlacklight/Zern/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,16 @@
 License-File: LICENSE
 Requires-Dist: websocket-client
 Requires-Dist: pyotp
 Requires-Dist: requests
 
 # Zern Class Documentation
 
+This is a free library. This doesn't require any subscription to use. 
+
 ## Documentation
 
 ```python
 from zern import Trader
 trader = Trader(user_name=YOUR_USERNAME,password=YOUR_PASSWORD,totp_key=YOUR_TOTP_KEY)
 ```
```

### Comparing `zern-0.0.5/README.md` & `zern-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Zern Class Documentation
 
+This is a free library. This doesn't require any subscription to use. 
+
 ## Documentation
 
 ```python
 from zern import Trader
 trader = Trader(user_name=YOUR_USERNAME,password=YOUR_PASSWORD,totp_key=YOUR_TOTP_KEY)
 ```
```

### Comparing `zern-0.0.5/pyproject.toml` & `zern-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zern"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Harsha Avapati", email="harshaavapati@gmail.com" },
 ]
 description = "An unofficial client library using Zerodha web api for live data and historical data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `zern-0.0.5/src/zern/Core/session.py` & `zern-0.0.6/src/zern/Core/session.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.5/src/zern/Core/trader.py` & `zern-0.0.6/src/zern/Core/trader.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.5/src/zern/Core/websocket_connection/ticker.py` & `zern-0.0.6/src/zern/Core/websocket_connection/ticker.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.5/src/zern/utils/OrderedList.py` & `zern-0.0.6/src/zern/utils/OrderedList.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.5/src/zern/utils/Types.py` & `zern-0.0.6/src/zern/utils/Types.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.5/src/zern/utils/parsing.py` & `zern-0.0.6/src/zern/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.5/src/zern.egg-info/PKG-INFO` & `zern-0.0.6/src/zern.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zern
-Version: 0.0.5
+Version: 0.0.6
 Summary: An unofficial client library using Zerodha web api for live data and historical data
 Author-email: Harsha Avapati <harshaavapati@gmail.com>
 Project-URL: Homepage, https://github.com/ExBlacklight/Zern
 Project-URL: Issues, https://github.com/ExBlacklight/Zern/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,16 @@
 License-File: LICENSE
 Requires-Dist: websocket-client
 Requires-Dist: pyotp
 Requires-Dist: requests
 
 # Zern Class Documentation
 
+This is a free library. This doesn't require any subscription to use. 
+
 ## Documentation
 
 ```python
 from zern import Trader
 trader = Trader(user_name=YOUR_USERNAME,password=YOUR_PASSWORD,totp_key=YOUR_TOTP_KEY)
 ```
```

