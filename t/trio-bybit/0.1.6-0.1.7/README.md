# Comparing `tmp/trio_bybit-0.1.6.tar.gz` & `tmp/trio_bybit-0.1.7.tar.gz`

## Comparing `trio_bybit-0.1.6.tar` & `trio_bybit-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/pytest.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/tests/test_async_client.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/tests/test_streams.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/trio_bybit/__init__.py
--rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/trio_bybit/client.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/trio_bybit/enums.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/trio_bybit/exceptions.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/trio_bybit/helpers.py
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/trio_bybit/streams.py
--rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/LICENSE
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/README.md
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 trio_bybit-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/pytest.ini
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/tests/test_async_client.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/tests/test_streams.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/trio_bybit/__init__.py
+-rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/trio_bybit/client.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/trio_bybit/enums.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/trio_bybit/exceptions.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/trio_bybit/helpers.py
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/trio_bybit/streams.py
+-rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/LICENSE
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/README.md
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 trio_bybit-0.1.7/PKG-INFO
```

### Comparing `trio_bybit-0.1.6/tests/test_async_client.py` & `trio_bybit-0.1.7/tests/test_async_client.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.6/tests/test_streams.py` & `trio_bybit-0.1.7/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.6/trio_bybit/client.py` & `trio_bybit-0.1.7/trio_bybit/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     def _get_request(self, method, uri, signed: bool, **kwargs) -> httpx.Request:
         timestamp = int(time.time() * 1000 + self.timestamp_offset)
         headers = self._get_headers(timestamp, signed)
         if method.lower() == "get":
             req = self.session.build_request(method, uri, headers=headers, params=kwargs)
         else:
-            req = self.session.build_request(method, uri, headers=headers, data=kwargs)
+            req = self.session.build_request(method, uri, headers=headers, json=kwargs)
         if signed:
             req.headers["X-BAPI-SIGN"] = self._generate_signature(req, timestamp)
             req.headers["X-BAPI-SIGN-TYPE"] = "2"
         return req
 
 
 class AsyncClient(BaseClient):
```

### Comparing `trio_bybit-0.1.6/trio_bybit/exceptions.py` & `trio_bybit-0.1.7/trio_bybit/exceptions.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.6/trio_bybit/helpers.py` & `trio_bybit-0.1.7/trio_bybit/helpers.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.6/trio_bybit/streams.py` & `trio_bybit-0.1.7/trio_bybit/streams.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.6/.gitignore` & `trio_bybit-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.6/LICENSE` & `trio_bybit-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.6/README.md` & `trio_bybit-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.1.6/pyproject.toml` & `trio_bybit-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "trio-bybit"
-version = "0.1.6"
+version = "0.1.7"
 description = "Python bybit async SDK based on trio."
 authors = [
     { name = "Shu Wang", email = "halfelf.ronin@gmail.com" }
 ]
 dependencies = [
     "trio>=0.25.0",
     "httpx[http2]>=0.27.0",
```

### Comparing `trio_bybit-0.1.6/PKG-INFO` & `trio_bybit-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: trio-bybit
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python bybit async SDK based on trio.
 Project-URL: Repository, https://github.com/halfelf/trio-bybit
 Author-email: Shu Wang <halfelf.ronin@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Shu Wang <halfelf.ronin@gmail.com>
```

