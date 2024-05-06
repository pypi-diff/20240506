# Comparing `tmp/lunar_interceptor-0.3.3.tar.gz` & `tmp/lunar_interceptor-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunar_interceptor-0.3.3.tar", last modified: Wed Apr 17 11:43:27 2024, max compression
+gzip compressed data, was "lunar_interceptor-0.3.4.tar", last modified: Mon May  6 10:49:08 2024, max compression
```

## Comparing `lunar_interceptor-0.3.3.tar` & `lunar_interceptor-0.3.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:43:27.407835 lunar_interceptor-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-17 11:43:27.407835 lunar_interceptor-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)    48047 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-17 11:43:27.407835 lunar_interceptor-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:43:27.399835 lunar_interceptor-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:43:27.403835 lunar_interceptor-0.3.3/src/lunar_interceptor/
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:43:27.403835 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/fail_safe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:43:27.407835 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/traffic_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/src/lunar_interceptor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:43:27.407835 lunar_interceptor-0.3.3/src/lunar_interceptor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-17 11:43:27.000000 lunar_interceptor-0.3.3/src/lunar_interceptor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-17 11:43:27.000000 lunar_interceptor-0.3.3/src/lunar_interceptor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:43:27.000000 lunar_interceptor-0.3.3/src/lunar_interceptor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 11:43:27.000000 lunar_interceptor-0.3.3/src/lunar_interceptor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 11:43:27.000000 lunar_interceptor-0.3.3/src/lunar_interceptor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:43:27.407835 lunar_interceptor-0.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/test/fail_safe_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/test/helpers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/test/interceptor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-04-17 11:43:13.000000 lunar_interceptor-0.3.3/test/traffic_filter_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:49:08.493501 lunar_interceptor-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-06 10:49:08.493501 lunar_interceptor-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)    48047 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-06 10:49:08.493501 lunar_interceptor-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:49:08.485501 lunar_interceptor-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:49:08.489501 lunar_interceptor-0.3.4/src/lunar_interceptor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/src/lunar_interceptor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:49:08.493501 lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/fail_safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:49:08.493501 lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/hooks/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/hooks/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/hooks/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7347 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/hooks/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/traffic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/src/lunar_interceptor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:49:08.493501 lunar_interceptor-0.3.4/src/lunar_interceptor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-06 10:49:08.000000 lunar_interceptor-0.3.4/src/lunar_interceptor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-06 10:49:08.000000 lunar_interceptor-0.3.4/src/lunar_interceptor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:49:08.000000 lunar_interceptor-0.3.4/src/lunar_interceptor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 10:49:08.000000 lunar_interceptor-0.3.4/src/lunar_interceptor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 10:49:08.000000 lunar_interceptor-0.3.4/src/lunar_interceptor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:49:08.493501 lunar_interceptor-0.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/test/fail_safe_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/test/helpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/test/interceptor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-05-06 10:48:52.000000 lunar_interceptor-0.3.4/test/traffic_filter_test.py
```

### Comparing `lunar_interceptor-0.3.3/Pipfile.lock` & `lunar_interceptor-0.3.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `lunar_interceptor-0.3.3/src/lunar_interceptor/__init__.py` & `lunar_interceptor-0.3.4/src/lunar_interceptor/__init__.py`

 * *Files identical despite different names*

### Comparing `lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/configuration.py` & `lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/configuration.py`

 * *Files identical despite different names*

### Comparing `lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/fail_safe.py` & `lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/fail_safe.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 from time import time
-
+import traceback as tb
 from types import TracebackType
 from typing import Optional, Tuple, Type, Any, Mapping
-import traceback as tb
+
+from lunar_interceptor.interceptor.hooks.const import LUNAR_PROXY_ERROR_TRANSLATOR
 
 # Default values
 _DEFAULT_MAX_ERROR_ALLOWED = 5
 _DEFAULT_FAILSAFE_COOLDOWN_SEC = 10
 
 _HEADER_ERROR_KEY = "x-lunar-error"
 
@@ -57,17 +58,19 @@
         traceback: TracebackType,
     ) -> bool:
         if exc_type is not None and issubclass(exc_type, self._handle_on):
             self._on_error()
             self._logger.warning(
                 f"FailSafe::Error communicating with Lunar Proxy, Error: {exc_value}"
             )
-            self._logger.debug(
-                f"Exception: {str(exc_type)}, Traceback: {tb.format_tb(traceback)}"
-            )
+            if exc_type is not ProxyErrorException:
+                self._logger.debug(
+                    f"Exception: {str(exc_type)}, Traceback: {tb.format_tb(traceback)}"
+                )
+
             return True  # Handle the exception for the caller
 
         elif exc_type is not None:
             return False  # Dont handle the exception for the caller
 
         self._error_counter = 0
         return True
@@ -99,14 +102,26 @@
 
         Raises:
             ProxyErrorException: if the error header exists.
         """
         if _HEADER_ERROR_KEY not in headers:
             return
 
+        errorCode = headers[_HEADER_ERROR_KEY]
+        errorMsg = LUNAR_PROXY_ERROR_TRANSLATOR.get(
+            errorCode,
+            "Unknown error, Please check the Proxy logs for more information.",
+        )
+
+        self._logger.warning(
+            "FailSafe::Error communicating with Lunar Proxy,"
+            f"Error: {errorCode}"
+            f"Message: {errorMsg}"
+        )
+
         raise ProxyErrorException("An error occurs on the Proxy side")
 
     def _on_error(self):
         """
         Increase the counter and break the circuit if needed.
         """
         self._error_counter += 1
```

### Comparing `lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/helpers.py` & `lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/helpers.py`

 * *Files identical despite different names*

### Comparing `lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/aiohttp.py` & `lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/hooks/aiohttp.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,112 +90,132 @@
         async def _request(
             client_session: "aiohttp.ClientSession",
             method: str,
             url: "StrOrURL",
             *args: List[Any],
             **kwargs: Dict[str, Any],
         ) -> "aiohttp.client.ClientResponse":
-            url_object = client_session._build_url(url)  # type: ignore [reportPrivateUsage]
+            lunar_req_id = generate_request_id()
+            url_obj = client_session._build_url(url)  # type: ignore [reportPrivateUsage]
             original_headers = kwargs.pop(HEADERS_KWARGS_KEY, {}).copy()
 
             with self._fail_safe:
                 if self._fail_safe.state_ok and self._traffic_filter.is_allowed(
-                    str(url_object.host), original_headers
+                    str(url_obj.host), original_headers
                 ):
                     return await self._make_request(
                         client_session=client_session,
                         method=method,
-                        url_object=url_object,
+                        url_object=url_obj,
                         original_headers=original_headers,
+                        lunar_req_id=lunar_req_id,
                         sequence_id=None,
                         *args,
                         **kwargs,
                     )
 
             kwargs[HEADERS_KWARGS_KEY] = original_headers
+            self._logger.debug(
+                f"Request {lunar_req_id} - Will send {url_obj} without using Lunar Proxy"
+            )
             return await self._original_function(  # type: ignore [reportOptionalCall]
                 client_session, method, url, *args, **kwargs
             )
 
         return _request
 
     async def _make_request(
         self,
         client_session: "aiohttp.ClientSession",
         method: str,
         url_object: URL,
         original_headers: Dict[str, Any],
+        lunar_req_id: str,
         sequence_id: Optional[str] = None,
         *args: List[Any],
         **kwargs: Dict[str, Any],
     ) -> "aiohttp.client.ClientResponse":
         manipulated_headers = generate_modified_headers(
             original_url=url_object,
             original_headers=original_headers,
             sequence_id=sequence_id,
+            lunar_req_id=lunar_req_id,
             lunar_tenant_id=self._connection_config.tenant_id,
             traffic_filter=self._traffic_filter,
         )
 
+        modified_url: URL = generate_modified_url(
+            self._connection_config.proxy_scheme,
+            self._connection_config.proxy_host_with_port,
+            url_object,
+        )
+
+        self._logger.debug(
+            f"Request {lunar_req_id} - Forwarding the request to {modified_url} using Lunar Proxy"
+        )
+
         response = await self._original_function(  # type: ignore [reportOptionalCall]
             self=client_session,
             method=method,
-            str_or_url=generate_modified_url(
-                self._connection_config.proxy_scheme,
-                self._connection_config.proxy_host_with_port,
-                url_object,
-            ),
+            str_or_url=modified_url,
             headers=manipulated_headers,
             *args,
             **kwargs,
         )
 
         self._fail_safe.validate_headers(response.headers)
 
-        retry_sequence_id = await self._prepare_for_retry(response.headers)
+        retry_sequence_id = await self._prepare_for_retry(
+            response.headers, lunar_req_id
+        )
         if retry_sequence_id is not None:
             response = await self._make_request(
                 client_session=client_session,
                 method=method,
                 url_object=url_object,
                 original_headers=original_headers,
+                lunar_req_id=lunar_req_id,
                 sequence_id=retry_sequence_id,
                 *args,
                 **kwargs,
             )
 
         modified_response_headers = self._generate_modified_response_headers(
             response.headers
         )
         response._cache[CACHE_HEADERS_KEY] = modified_response_headers  # type: ignore [reportPrivateUsage]
 
         return response
 
-    async def _prepare_for_retry(self, headers: CIMultiDictProxy[str]) -> Optional[str]:
+    async def _prepare_for_retry(
+        self, headers: CIMultiDictProxy[str], lunar_req_id: str
+    ) -> Optional[str]:
         raw_retry_after = headers.get(LUNAR_RETRY_AFTER_HEADER_KEY)
         if raw_retry_after is None:
             return None
 
         sequence_id = headers.get(LUNAR_SEQ_ID_HEADER_KEY)
         if sequence_id is None:
             self._logger.debug(
-                f"Retry required, but {LUNAR_SEQ_ID_HEADER_KEY} is missing!"
+                f"Request {lunar_req_id} - Retry required, but {LUNAR_SEQ_ID_HEADER_KEY} is missing!"
             )
             return None
 
         try:
             retry_after = float(raw_retry_after)
         except ValueError:
             self._logger.debug(
-                f"Retry required, but parsing header {LUNAR_RETRY_AFTER_HEADER_KEY}"
+                f"Request {lunar_req_id} - Retry required, but parsing header {LUNAR_RETRY_AFTER_HEADER_KEY}"
                 + f"as float failed ({raw_retry_after})"
             )
             return None
 
-        self._logger.debug(f"Retry required, will retry in {retry_after} seconds...")
+        self._logger.debug(
+            f"Request {lunar_req_id} - Retry required, will retry in {retry_after} seconds..."
+        )
         await sleep(retry_after)
         return sequence_id
 
     def _generate_modified_response_headers(
         self, original_headers: CIMultiDictProxy[str]
     ) -> CIMultiDictProxy[str]:
         if LUNAR_SEQ_ID_HEADER_KEY not in original_headers:
```

### Comparing `lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/const.py` & `lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/hooks/const.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,18 +2,27 @@
 
 HTTP_SCHEME = "http"
 HTTPS_SCHEME = "https"
 X_LUNAR_HOST_HEADER_KEY = "x-lunar-host"
 X_LUNAR_SCHEME_HEADER_KEY = "x-lunar-scheme"
 X_LUNAR_INTERCEPTOR_HEADER_KEY = "x-lunar-interceptor"
 X_LUNAR_TENANT_ID_HEADER_KEY = "x-lunar-tenant-id"
+X_LUNAR_REQ_ID_HEADER_KEY = "x-lunar-req-id"
 INTERCEPTOR_TYPE_VALUE = "lunar-py-interceptor"
 VERSION = get_package_version("lunar-interceptor")
 INTERCEPTOR_HEADER_DELIMITER = "/"
 LUNAR_INTERCEPTOR_HEADER_VALUE = (
     f"{INTERCEPTOR_TYPE_VALUE}{INTERCEPTOR_HEADER_DELIMITER}{VERSION}"
 )
 
 HEADERS_KWARGS_KEY = "headers"
 CACHE_HEADERS_KEY = "headers"
 LUNAR_SEQ_ID_HEADER_KEY = "x-lunar-sequence-id"
 LUNAR_RETRY_AFTER_HEADER_KEY = "x-lunar-retry-after"
+
+LUNAR_PROXY_ERROR_TRANSLATOR = {
+    "1": "Wrong request, Lunar Proxy could not find header `x-lunar-host` and Proxy was not set to use query params.",
+    "2": "The endpoint cannot be reached",
+    "3": "Gateway timeout",
+    "4": "Lunar Proxy could not find the endpoint",
+    "5": "Lunar Proxy could not resolve host",
+}
```

### Comparing `lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/helpers.py` & `lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/hooks/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 from typing import Dict, Optional
 
 from yarl import URL
 
 from .const import *
 from lunar_interceptor.interceptor.traffic_filter import TrafficFilter
+import uuid
+
+
+def generate_request_id() -> str:
+    """
+    Generate a Request Identifier.
+
+    Returns:
+        str: A string representation of the generated ID.
+    """
+    return str(uuid.uuid4())
 
 
 def generate_modified_headers(
     original_url: URL,
     original_headers: Optional[Dict[str, str]],
     sequence_id: Optional[str],
     traffic_filter: TrafficFilter,
     lunar_tenant_id: str,
+    lunar_req_id: str,
 ) -> Dict[str, str]:
     """
     Generate the headers to support the proxy work flow.
 
     Args:
         original_url (yarl.URL):The url object converted by the original url passed to the request.
         original_headers (Dict[str ,str]): The dictionary of the original request headers.
@@ -33,14 +45,15 @@
         if destination_port is not None
         else original_url.host
     )
 
     modified_headers: Dict[str, str] = original_headers if original_headers else {}
 
     modified_headers[X_LUNAR_HOST_HEADER_KEY] = host
+    modified_headers[X_LUNAR_REQ_ID_HEADER_KEY] = lunar_req_id
     modified_headers[X_LUNAR_SCHEME_HEADER_KEY] = original_url.scheme
     modified_headers[X_LUNAR_INTERCEPTOR_HEADER_KEY] = LUNAR_INTERCEPTOR_HEADER_VALUE
     if traffic_filter.managed:
         modified_headers[X_LUNAR_TENANT_ID_HEADER_KEY] = lunar_tenant_id
 
     if sequence_id is not None:
         modified_headers[LUNAR_SEQ_ID_HEADER_KEY] = sequence_id
```

### Comparing `lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/hooks/requests.py` & `lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/hooks/requests.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,120 +69,133 @@
         def _request(
             client_session: "requests.sessions.Session",
             method: str,
             url: str,
             *args: List[Any],
             **kwargs: Dict[str, Any],
         ) -> "requests.Response":
+            lunar_req_id = generate_request_id()
             url_obj = URL(url)
             original_headers = kwargs.pop(HEADERS_KWARGS_KEY, {})
 
             with self._fail_safe:
                 if self._fail_safe.state_ok and self._traffic_filter.is_allowed(
                     str(url_obj.host), original_headers
                 ):
                     return self._make_request(
                         client_session=client_session,
                         method=method,
                         url_object=url_obj,
                         original_headers=original_headers,
+                        lunar_req_id=lunar_req_id,
                         sequence_id=None,
                         *args,
                         **kwargs,
                     )
 
             kwargs[HEADERS_KWARGS_KEY] = original_headers
-            self._logger.debug(f"Will send {url_obj} without using Lunar Proxy")
+            self._logger.debug(
+                f"Request {lunar_req_id} - Will send {url_obj} without using Lunar Proxy"
+            )
             return self._original_function(
                 self=client_session, method=method, url=url, *args, **kwargs
             )
 
         return _request
 
     def _make_request(
         self,
         client_session: "requests.sessions.Session",
         method: str,
         url_object: URL,
         original_headers: Dict[str, Any],
+        lunar_req_id: str,
         sequence_id: Optional[str] = None,
         *args: List[Any],
         **kwargs: Dict[str, Any],
     ) -> "requests.Response":
         manipulated_headers = generate_modified_headers(
             original_url=url_object,
             original_headers=original_headers,
             sequence_id=sequence_id,
             lunar_tenant_id=self._connection_config.tenant_id,
             traffic_filter=self._traffic_filter,
+            lunar_req_id=lunar_req_id,
         )
         modified_url = str(
             generate_modified_url(
                 self._connection_config.proxy_scheme,
                 self._connection_config.proxy_host_with_port,
                 url_object,
             ),
         )
         self._logger.debug(
-            f"Forwarding the request to {modified_url} using Lunar Proxy"
+            f"Request {lunar_req_id} - Forwarding the request to {modified_url} using Lunar Proxy"
         )
         response = self._original_function(
             self=client_session,
             method=method,
             url=modified_url,
             headers=manipulated_headers,
             *args,
             **kwargs,
         )
 
         self._fail_safe.validate_headers(response.headers)
 
-        retry_sequence_id = self._prepare_requests_for_retry(response.headers)
+        retry_sequence_id = self._prepare_requests_for_retry(
+            response.headers, lunar_req_id
+        )
         if retry_sequence_id is not None:
             response = self._make_request(
                 client_session=client_session,
                 method=method,
                 url_object=url_object,
                 original_headers=original_headers,
+                lunar_req_id=lunar_req_id,
                 sequence_id=retry_sequence_id,
                 *args,
                 **kwargs,
             )
 
         modified_response_headers = self._generate_modified_response_headers(
             response.headers
         )
         response.headers = modified_response_headers  # type: ignore [reportPrivateUsage]
 
         return response
 
     def _prepare_requests_for_retry(
-        self, headers: "requests.models.CaseInsensitiveDict[str]"
+        self,
+        headers: "requests.models.CaseInsensitiveDict[str]",
+        lunar_req_id: str,
     ) -> Optional[str]:
         raw_retry_after = headers.get(LUNAR_RETRY_AFTER_HEADER_KEY)
         if raw_retry_after is None:
             return None
 
         sequence_id = headers.get(LUNAR_SEQ_ID_HEADER_KEY)
         if sequence_id is None:
             self._logger.debug(
-                f"Retry required, but {LUNAR_SEQ_ID_HEADER_KEY} is missing!"
+                f"Request {lunar_req_id} - Retry required, but {LUNAR_SEQ_ID_HEADER_KEY} is missing!"
             )
             return None
 
         try:
             retry_after = float(raw_retry_after)
         except ValueError:
             self._logger.debug(
-                f"Retry required, but parsing header {LUNAR_RETRY_AFTER_HEADER_KEY}"
+                f"Request {lunar_req_id} - Retry required, but parsing header {LUNAR_RETRY_AFTER_HEADER_KEY}"
                 + f"as float failed ({raw_retry_after})"
             )
             return None
 
-        self._logger.debug(f"Retry required, will retry in {retry_after} seconds...")
+        self._logger.debug(
+            f"Request {lunar_req_id} - Retry required, will retry in {retry_after} seconds..."
+        )
         sleep(retry_after)
         return sequence_id
 
     def _generate_modified_response_headers(
         self, original_headers: "requests.models.CaseInsensitiveDict[str]"
     ) -> "requests.models.CaseInsensitiveDict[str]":
         if LUNAR_SEQ_ID_HEADER_KEY not in original_headers:
```

### Comparing `lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/interceptor.py` & `lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/interceptor.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,14 @@
                 f" please make sure that Lunar Proxy is running and port '{self._connection_config.handshake_port}'"
                 f" is set as the handshake port.\n"
                 f" For more information please refer to:"
                 f" http://docs.lunar.dev/installation-configuration/configuration#lunar-interceptor-configuration"
             )
             return
 
-        print(res)
         for hook in self._lunar_hooks:
             hook.init_hooks()
 
         self._logger.info(
             "[ⓥ] Successfully communicate with Lunar Proxy"
             "Lunar Interceptor is ENABLED!"
         )
```

### Comparing `lunar_interceptor-0.3.3/src/lunar_interceptor/interceptor/traffic_filter.py` & `lunar_interceptor-0.3.4/src/lunar_interceptor/interceptor/traffic_filter.py`

 * *Files identical despite different names*

### Comparing `lunar_interceptor-0.3.3/src/lunar_interceptor.egg-info/SOURCES.txt` & `lunar_interceptor-0.3.4/src/lunar_interceptor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lunar_interceptor-0.3.3/test/fail_safe_test.py` & `lunar_interceptor-0.3.4/test/fail_safe_test.py`

 * *Files identical despite different names*

### Comparing `lunar_interceptor-0.3.3/test/interceptor_test.py` & `lunar_interceptor-0.3.4/test/interceptor_test.py`

 * *Files identical despite different names*

### Comparing `lunar_interceptor-0.3.3/test/traffic_filter_test.py` & `lunar_interceptor-0.3.4/test/traffic_filter_test.py`

 * *Files identical despite different names*

