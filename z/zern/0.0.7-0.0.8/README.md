# Comparing `tmp/zern-0.0.7.tar.gz` & `tmp/zern-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zern-0.0.7.tar", last modified: Mon May  6 05:13:31 2024, max compression
+gzip compressed data, was "zern-0.0.8.tar", last modified: Mon May  6 07:58:27 2024, max compression
```

## Comparing `zern-0.0.7.tar` & `zern-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 05:13:31.264776 zern-0.0.7/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     1071 2024-05-02 15:26:31.000000 zern-0.0.7/LICENSE
--rw-r--r--   0 harsha    (1000) harsha    (1000)     6442 2024-05-06 05:13:31.264776 zern-0.0.7/PKG-INFO
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     5788 2024-05-06 04:59:34.000000 zern-0.0.7/README.md
--rw-rw-r--   0 harsha    (1000) harsha    (1000)      702 2024-05-06 05:13:26.000000 zern-0.0.7/pyproject.toml
--rw-rw-r--   0 harsha    (1000) harsha    (1000)       38 2024-05-06 05:13:31.264776 zern-0.0.7/setup.cfg
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 05:13:31.260776 zern-0.0.7/src/
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 05:13:31.264776 zern-0.0.7/src/zern/
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 05:13:31.264776 zern-0.0.7/src/zern/Core/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     3798 2024-05-02 06:23:51.000000 zern-0.0.7/src/zern/Core/session.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     4646 2024-05-02 19:27:04.000000 zern-0.0.7/src/zern/Core/trader.py
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 05:13:31.264776 zern-0.0.7/src/zern/Core/websocket/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     3521 2024-05-06 05:05:18.000000 zern-0.0.7/src/zern/Core/websocket/ticker.py
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 05:13:31.264776 zern-0.0.7/src/zern/Core/websocket_connection/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     3534 2024-05-02 07:34:58.000000 zern-0.0.7/src/zern/Core/websocket_connection/ticker.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)       61 2024-04-24 18:27:30.000000 zern-0.0.7/src/zern/__init__.py
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 05:13:31.264776 zern-0.0.7/src/zern/utils/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     1861 2024-04-21 19:33:12.000000 zern-0.0.7/src/zern/utils/OrderedList.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     2280 2024-05-02 05:29:49.000000 zern-0.0.7/src/zern/utils/Types.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     6314 2024-05-02 05:36:04.000000 zern-0.0.7/src/zern/utils/parsing.py
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 05:13:31.264776 zern-0.0.7/src/zern.egg-info/
--rw-r--r--   0 harsha    (1000) harsha    (1000)     6442 2024-05-06 05:13:31.000000 zern-0.0.7/src/zern.egg-info/PKG-INFO
--rw-rw-r--   0 harsha    (1000) harsha    (1000)      420 2024-05-06 05:13:31.000000 zern-0.0.7/src/zern.egg-info/SOURCES.txt
--rw-rw-r--   0 harsha    (1000) harsha    (1000)        1 2024-05-06 05:13:31.000000 zern-0.0.7/src/zern.egg-info/dependency_links.txt
--rw-rw-r--   0 harsha    (1000) harsha    (1000)       40 2024-05-06 05:13:31.000000 zern-0.0.7/src/zern.egg-info/requires.txt
--rw-rw-r--   0 harsha    (1000) harsha    (1000)        5 2024-05-06 05:13:31.000000 zern-0.0.7/src/zern.egg-info/top_level.txt
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 07:58:27.600166 zern-0.0.8/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     1071 2024-05-02 15:26:31.000000 zern-0.0.8/LICENSE
+-rw-r--r--   0 harsha    (1000) harsha    (1000)     6442 2024-05-06 07:58:27.596166 zern-0.0.8/PKG-INFO
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     5788 2024-05-06 04:59:34.000000 zern-0.0.8/README.md
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)      702 2024-05-06 07:54:46.000000 zern-0.0.8/pyproject.toml
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)       38 2024-05-06 07:58:27.600166 zern-0.0.8/setup.cfg
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 07:58:27.596166 zern-0.0.8/src/
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 07:58:27.596166 zern-0.0.8/src/zern/
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 07:58:27.596166 zern-0.0.8/src/zern/Core/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     3798 2024-05-06 07:56:14.000000 zern-0.0.8/src/zern/Core/session.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     4646 2024-05-02 19:27:04.000000 zern-0.0.8/src/zern/Core/trader.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 07:58:27.596166 zern-0.0.8/src/zern/Core/websocket_connection/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     3604 2024-05-06 07:57:44.000000 zern-0.0.8/src/zern/Core/websocket_connection/ticker.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)       61 2024-04-24 18:27:30.000000 zern-0.0.8/src/zern/__init__.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 07:58:27.596166 zern-0.0.8/src/zern/utils/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     1861 2024-04-21 19:33:12.000000 zern-0.0.8/src/zern/utils/OrderedList.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     2280 2024-05-02 05:29:49.000000 zern-0.0.8/src/zern/utils/Types.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     6314 2024-05-02 05:36:04.000000 zern-0.0.8/src/zern/utils/parsing.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 07:58:27.596166 zern-0.0.8/src/zern.egg-info/
+-rw-r--r--   0 harsha    (1000) harsha    (1000)     6442 2024-05-06 07:58:27.000000 zern-0.0.8/src/zern.egg-info/PKG-INFO
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)      386 2024-05-06 07:58:27.000000 zern-0.0.8/src/zern.egg-info/SOURCES.txt
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)        1 2024-05-06 07:58:27.000000 zern-0.0.8/src/zern.egg-info/dependency_links.txt
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)       40 2024-05-06 07:58:27.000000 zern-0.0.8/src/zern.egg-info/requires.txt
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)        5 2024-05-06 07:58:27.000000 zern-0.0.8/src/zern.egg-info/top_level.txt
```

### Comparing `zern-0.0.7/LICENSE` & `zern-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zern-0.0.7/PKG-INFO` & `zern-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zern
-Version: 0.0.7
+Version: 0.0.8
 Summary: An unofficial client library using Zerodha web api for live data and historical data
 Author-email: Harsha Avapati <harshaavapati@gmail.com>
 Project-URL: Homepage, https://github.com/ExBlacklight/Zern
 Project-URL: Issues, https://github.com/ExBlacklight/Zern/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `zern-0.0.7/README.md` & `zern-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `zern-0.0.7/pyproject.toml` & `zern-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zern"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Harsha Avapati", email="harshaavapati@gmail.com" },
 ]
 description = "An unofficial client library using Zerodha web api for live data and historical data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `zern-0.0.7/src/zern/Core/session.py` & `zern-0.0.8/src/zern/Core/session.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.7/src/zern/Core/trader.py` & `zern-0.0.8/src/zern/Core/trader.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.7/src/zern/Core/websocket/ticker.py` & `zern-0.0.8/src/zern/Core/websocket_connection/ticker.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import websocket
 import json
 from datetime import datetime
 import threading
 from zern.utils.parsing import encodeURIComponent,parse_binary
 from zern.utils.Types import MODE_STRING,KEYS
 from typing import Union, List
+import os
+import certifi
 
 class Ticker:
     def __init__(self,session):
         self.__private_session = session
         self.__private_input_message = None
         self.__private_websocket_connection = None
         self.connect_to_websocket()
@@ -24,14 +26,16 @@
             'enctoken': encodeURIComponent(self.__private_session._enc_token),
             'uid': f'{int(time.time() * 1000)}',
             'user-agent': 'kite3-web',
             'version': '3.0.0',
         }
         address = "wss://ws.zerodha.com/"
         url = self.params_to_url(address)
+        if os.environ.get('WEBSOCKET_CLIENT_CA_BUNDLE') is None:
+            os.environ['WEBSOCKET_CLIENT_CA_BUNDLE'] = certifi.where()
         ws = websocket.WebSocketApp(url, on_message=self.on_message,on_error=self.on_error,on_close=self.on_close)
         ws.on_open = self.on_open
         self.__private_websocket_connection = ws
         thread = threading.Thread(target=ws.run_forever,daemon=True)
         thread.start()
         print(f'connection successful')
 
@@ -45,16 +49,16 @@
         self.last_msg = parse_binary(message)
         self.last_msg_time = datetime.now()
         #print(parse_binary(message))
 
     def on_error(self,ws, error):
         print(error)
 
-    def on_close(self,ws,status_code,close_message):
-        print("websocket::CLOSED::status={}::{}".format(status_code,close_message))
+    def on_close(self,ws):
+        print("### closed ###")
     
     def on_open(self,ws):
         m1 = {"a": KEYS.subscribe ,"v":[256265,260105]}
         m2 = {"a": KEYS.mode,"v":[ MODE_STRING.modeLTPC ,[256265,260105]]}
         ws.send(json.dumps(m1))
         ws.send(json.dumps(m2))
```

### Comparing `zern-0.0.7/src/zern/utils/OrderedList.py` & `zern-0.0.8/src/zern/utils/OrderedList.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.7/src/zern/utils/Types.py` & `zern-0.0.8/src/zern/utils/Types.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.7/src/zern/utils/parsing.py` & `zern-0.0.8/src/zern/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.7/src/zern.egg-info/PKG-INFO` & `zern-0.0.8/src/zern.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zern
-Version: 0.0.7
+Version: 0.0.8
 Summary: An unofficial client library using Zerodha web api for live data and historical data
 Author-email: Harsha Avapati <harshaavapati@gmail.com>
 Project-URL: Homepage, https://github.com/ExBlacklight/Zern
 Project-URL: Issues, https://github.com/ExBlacklight/Zern/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

