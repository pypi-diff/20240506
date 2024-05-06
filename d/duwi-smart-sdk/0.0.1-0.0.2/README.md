# Comparing `tmp/duwi_smart_sdk-0.0.1.tar.gz` & `tmp/duwi_smart_sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smart_sdk-0.0.1.tar", last modified: Sun May  5 02:47:41 2024, max compression
+gzip compressed data, was "duwi_smart_sdk-0.0.2.tar", last modified: Mon May  6 08:42:00 2024, max compression
```

## Comparing `duwi_smart_sdk-0.0.1.tar` & `duwi_smart_sdk-0.0.2.tar`

### file list

```diff
@@ -1,56 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 02:47:41.914260 duwi_smart_sdk-0.0.1/
--rw-rw-rw-   0        0        0      532 2024-05-05 02:47:41.913726 duwi_smart_sdk-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-05 02:03:11.000000 duwi_smart_sdk-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 02:47:41.885004 duwi_smart_sdk-0.0.1/duwi_smart_sdk/
--rw-rw-rw-   0        0        0        0 2024-05-05 02:15:40.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 02:47:41.894004 duwi_smart_sdk-0.0.1/duwi_smart_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-05-04 11:19:01.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     1361 2024-05-05 02:19:48.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/api/control.py
--rw-rw-rw-   0        0        0     2597 2024-05-05 02:19:48.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/api/discover.py
--rw-rw-rw-   0        0        0     2188 2024-05-05 02:19:48.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/api/house.py
--rw-rw-rw-   0        0        0     1723 2024-05-05 02:19:48.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/api/login.py
--rw-rw-rw-   0        0        0     1534 2024-05-05 02:19:48.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/api/refresh_token.py
--rw-rw-rw-   0        0        0     4746 2024-05-05 02:19:48.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-05 02:47:41.896004 duwi_smart_sdk-0.0.1/duwi_smart_sdk/const/
--rw-rw-rw-   0        0        0        0 2024-05-04 11:19:01.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/const/__init__.py
--rw-rw-rw-   0        0        0      216 2024-05-04 04:59:17.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/const/const.py
--rw-rw-rw-   0        0        0      274 2024-05-04 12:18:23.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/const/status.py
--rw-rw-rw-   0        0        0     1194 2024-05-02 06:54:28.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-05 02:47:41.897004 duwi_smart_sdk-0.0.1/duwi_smart_sdk/model/
--rw-rw-rw-   0        0        0        0 2024-05-04 11:19:01.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 02:47:41.898005 duwi_smart_sdk-0.0.1/duwi_smart_sdk/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-04 11:19:01.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/model/req/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-02 06:54:28.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-05 02:47:41.902144 duwi_smart_sdk-0.0.1/duwi_smart_sdk/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-04 11:19:01.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-04 06:02:22.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-04 14:15:21.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/model/resp/control.py
--rw-rw-rw-   0        0        0     2767 2024-05-04 14:58:19.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/model/resp/device.py
--rw-rw-rw-   0        0        0     1113 2024-05-04 06:01:22.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/model/resp/house.py
-drwxrwxrwx   0        0        0        0 2024-05-05 02:47:41.904654 duwi_smart_sdk-0.0.1/duwi_smart_sdk/util/
--rw-rw-rw-   0        0        0        0 2024-05-04 11:19:01.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-04 06:19:55.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/util/http.py
--rw-rw-rw-   0        0        0      906 2024-05-02 06:54:28.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-02 06:54:28.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-05 02:47:41.912652 duwi_smart_sdk-0.0.1/duwi_smart_sdk.egg-info/
--rw-rw-rw-   0        0        0      532 2024-05-05 02:47:41.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1256 2024-05-05 02:47:41.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 02:47:41.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-05 02:47:41.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-05 02:47:41.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-05 02:47:41.000000 duwi_smart_sdk-0.0.1/duwi_smart_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 02:47:41.914260 duwi_smart_sdk-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      908 2024-05-05 02:31:41.000000 duwi_smart_sdk-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 02:47:41.905653 duwi_smart_sdk-0.0.1/test/
--rw-rw-rw-   0        0        0        0 2024-05-04 06:46:08.000000 duwi_smart_sdk-0.0.1/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 02:47:41.910653 duwi_smart_sdk-0.0.1/test/api/
--rw-rw-rw-   0        0        0        0 2024-05-04 06:46:08.000000 duwi_smart_sdk-0.0.1/test/api/__init__.py
--rw-rw-rw-   0        0        0      627 2024-05-05 02:19:48.000000 duwi_smart_sdk-0.0.1/test/api/test_control.py
--rw-rw-rw-   0        0        0      459 2024-05-05 02:15:57.000000 duwi_smart_sdk-0.0.1/test/api/test_discover.py
--rw-rw-rw-   0        0        0      410 2024-05-05 02:15:57.000000 duwi_smart_sdk-0.0.1/test/api/test_house.py
--rw-rw-rw-   0        0        0      330 2024-05-05 02:42:26.000000 duwi_smart_sdk-0.0.1/test/api/test_login.py
--rw-rw-rw-   0        0        0      423 2024-05-05 02:15:57.000000 duwi_smart_sdk-0.0.1/test/api/test_refresh_token.py
--rw-rw-rw-   0        0        0      715 2024-05-05 02:15:57.000000 duwi_smart_sdk-0.0.1/test/api/test_ws.py
-drwxrwxrwx   0        0        0        0 2024-05-05 02:47:41.911652 duwi_smart_sdk-0.0.1/test/util/
--rw-rw-rw-   0        0        0        0 2024-05-04 06:46:08.000000 duwi_smart_sdk-0.0.1/test/util/__init__.py
--rw-rw-rw-   0        0        0     1192 2024-05-04 06:46:08.000000 duwi_smart_sdk-0.0.1/test/util/test_http.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.645693 duwi_smart_sdk-0.0.2/
+-rw-rw-rw-   0        0        0      543 2024-05-06 08:42:00.644716 duwi_smart_sdk-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.579125 duwi_smart_sdk-0.0.2/duwi_smart_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.608585 duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     1361 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/control.py
+-rw-rw-rw-   0        0        0     2597 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/discover.py
+-rw-rw-rw-   0        0        0     2188 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/house.py
+-rw-rw-rw-   0        0        0     1723 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/login.py
+-rw-rw-rw-   0        0        0     1534 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/refresh_token.py
+-rw-rw-rw-   0        0        0     4752 2024-05-06 08:41:25.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.617373 duwi_smart_sdk-0.0.2/duwi_smart_sdk/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/const/const.py
+-rw-rw-rw-   0        0        0      274 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/const/status.py
+-rw-rw-rw-   0        0        0     1194 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.619326 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.622256 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/req/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.630068 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/control.py
+-rw-rw-rw-   0        0        0     2767 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/device.py
+-rw-rw-rw-   0        0        0     1113 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/house.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.637887 duwi_smart_sdk-0.0.2/duwi_smart_sdk/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/util/http.py
+-rw-rw-rw-   0        0        0      906 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.592973 duwi_smart_sdk-0.0.2/duwi_smart_sdk.egg-info/
+-rw-rw-rw-   0        0        0      543 2024-05-06 08:42:00.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1087 2024-05-06 08:42:00.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 08:42:00.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-06 08:42:00.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-06 08:42:00.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-06 08:42:00.000000 duwi_smart_sdk-0.0.2/duwi_smart_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 08:42:00.645693 duwi_smart_sdk-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      908 2024-05-06 08:41:33.000000 duwi_smart_sdk-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.639833 duwi_smart_sdk-0.0.2/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:42:00.642763 duwi_smart_sdk-0.0.2/test/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/test/util/__init__.py
+-rw-rw-rw-   0        0        0     1192 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.0.2/test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.0.1/PKG-INFO` & `duwi_smart_sdk-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: duwi_smart_sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
-Requires-Dist: websockets
-Requires-Dist: aiohttp
+
+install sdk
+```shell
+pip install duwi-smart-sdk
+```
+
+
```

### Comparing `duwi_smart_sdk-0.0.1/duwi_smart_sdk/api/control.py` & `duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.1/duwi_smart_sdk/api/discover.py` & `duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.1/duwi_smart_sdk/api/house.py` & `duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.1/duwi_smart_sdk/api/login.py` & `duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/login.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.1/duwi_smart_sdk/api/refresh_token.py` & `duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.1/duwi_smart_sdk/api/ws.py` & `duwi_smart_sdk-0.0.2/duwi_smart_sdk/api/ws.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     async def process_messages(self):
         async for message in self._connection:
             try:
                 if message == "KEEPALIVE":
                     continue
                 _LOGGER.info(f"ws接受消息:{message}")
                 message = str.replace(message, "&excision&", "")
-                self._on_callback(message)
+                await self._on_callback(message)
             except Exception as e:
                 _LOGGER.error(f"ws接受消息出现异常:{e}")
                 _LOGGER.error(f"error message detail: \n{traceback.format_exc()}")
 
             # try:
             #     if message == "KEEPALIVE":
             #         continue
```

### Comparing `duwi_smart_sdk-0.0.1/duwi_smart_sdk/const/type_map.py` & `duwi_smart_sdk-0.0.2/duwi_smart_sdk/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.1/duwi_smart_sdk/model/req/device_control.py` & `duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.1/duwi_smart_sdk/model/resp/auth.py` & `duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.1/duwi_smart_sdk/model/resp/device.py` & `duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.1/duwi_smart_sdk/model/resp/house.py` & `duwi_smart_sdk-0.0.2/duwi_smart_sdk/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.1/duwi_smart_sdk/util/http.py` & `duwi_smart_sdk-0.0.2/duwi_smart_sdk/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.1/duwi_smart_sdk/util/sign.py` & `duwi_smart_sdk-0.0.2/duwi_smart_sdk/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.0.1/duwi_smart_sdk.egg-info/PKG-INFO` & `duwi_smart_sdk-0.0.2/duwi_smart_sdk.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
-Name: duwi_smart_sdk
-Version: 0.0.1
+Name: duwi-smart-sdk
+Version: 0.0.2
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
-Requires-Dist: websockets
-Requires-Dist: aiohttp
+
+install sdk
+```shell
+pip install duwi-smart-sdk
+```
+
+
```

### Comparing `duwi_smart_sdk-0.0.1/setup.py` & `duwi_smart_sdk-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smart_sdk",
     version=VERSION,
     author="ledger",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smart_sdk-0.0.1/test/util/test_http.py` & `duwi_smart_sdk-0.0.2/test/util/test_http.py`

 * *Files identical despite different names*

