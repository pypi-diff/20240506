# Comparing `tmp/requests_sse-0.3.1.tar.gz` & `tmp/requests_sse-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_sse-0.3.1.tar", max compression
+gzip compressed data, was "requests_sse-0.3.2.tar", max compression
```

## Comparing `requests_sse-0.3.1.tar` & `requests_sse-0.3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11374 2023-12-13 16:04:55.936736 requests_sse-0.3.1/LICENSE
--rw-r--r--   0        0        0     1547 2023-12-13 16:04:55.936736 requests_sse-0.3.1/README.rst
--rw-r--r--   0        0        0     1382 2023-12-13 16:04:55.936736 requests_sse-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       45 2023-12-13 16:04:55.936736 requests_sse-0.3.1/requests_sse/__init__.py
--rw-r--r--   0        0        0    13424 2023-12-13 16:04:55.936736 requests_sse-0.3.1/requests_sse/client.py
--rw-r--r--   0        0        0     3141 1970-01-01 00:00:00.000000 requests_sse-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11374 2024-05-06 12:09:17.855239 requests_sse-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1546 2024-05-06 12:09:17.855239 requests_sse-0.3.2/README.rst
+-rw-r--r--   0        0        0     1382 2024-05-06 12:09:17.859239 requests_sse-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-05-06 12:09:17.859239 requests_sse-0.3.2/requests_sse/__init__.py
+-rw-r--r--   0        0        0    13440 2024-05-06 12:09:17.859239 requests_sse-0.3.2/requests_sse/client.py
+-rw-r--r--   0        0        0     3140 1970-01-01 00:00:00.000000 requests_sse-0.3.2/PKG-INFO
```

### Comparing `requests_sse-0.3.1/LICENSE` & `requests_sse-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `requests_sse-0.3.1/README.rst` & `requests_sse-0.3.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 .. image:: https://img.shields.io/github/actions/workflow/status/overcat/requests-sse/test-deploy.yml?branch=main
     :alt: GitHub Workflow Status
     :target: https://github.com/overcat/requests-sse/actions
 .. image:: https://img.shields.io/pypi/v/requests-sse.svg
     :alt: PyPI
     :target: https://pypi.python.org/pypi/requests-sse
-.. image:: https://img.shields.io/badge/python-%3E%3D3.8-blue
+.. image:: https://img.shields.io/badge/python-%3E%3D37-blue
     :alt: Python - Version
     :target: https://pypi.python.org/pypi/stellar-sdk
 
 A Server-Sent Events python client based on requests, provides a simple interface to process `Server-Sent Events <https://www.w3.org/TR/eventsource>`_.
 
 Installation
 ------------
```

### Comparing `requests_sse-0.3.1/pyproject.toml` & `requests_sse-0.3.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "requests-sse"
-version = "0.3.1"
+version = "0.3.2"
 description = "server-sent events python client library based on requests"
 authors = ["overcat <4catcode@gmail.com>"]
 maintainers = ["overcat <4catcode@gmail.com>"]
 readme = "README.rst"
 homepage = "https://github.com/overcat/requests-sse"
 repository = "https://github.com/overcat/requests-sse"
 documentation = "https://github.com/overcat/requests-sse"
```

### Comparing `requests_sse-0.3.1/requests_sse/client.py` & `requests_sse-0.3.2/requests_sse/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "InvalidStatusCodeError",
     "InvalidContentTypeError",
 ]
 
 DEFAULT_RECONNECTION_TIME = timedelta(seconds=5)
 DEFAULT_MAX_CONNECT_RETRY = 5
 _CONTENT_TYPE_EVENT_STREAM = "text/event-stream"
-_CONTENT_TYPE_EVENT_STREAM_UTF_8 = "text/event-stream; charset=utf-8"
+_CONTENT_TYPE_EVENT_STREAM_UTF_8 = "text/event-stream;charset=utf-8"
 _LOGGER = logging.getLogger(__name__)
 
 
 class InvalidStatusCodeError(requests.RequestException):
     """Invalid status code error."""
 
     def __init__(self, status_code: int, *args, **kwargs):
@@ -275,15 +275,15 @@
             _LOGGER.error(error_message)
             self._fail_connect()
             raise InvalidStatusCodeError(
                 response.status_code, error_message, response=response
             )
 
         content_type = response.headers.get("Content-Type")
-        if not content_type or content_type.lower() not in (
+        if not content_type or content_type.lower().replace(" ", "") not in (
             _CONTENT_TYPE_EVENT_STREAM,
             _CONTENT_TYPE_EVENT_STREAM_UTF_8,
         ):
             error_message = "fetch {} failed with wrong Content-Type: {}".format(
                 self._url, response.headers.get("Content-Type")
             )
             _LOGGER.error(error_message)
```

### Comparing `requests_sse-0.3.1/PKG-INFO` & `requests_sse-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-sse
-Version: 0.3.1
+Version: 0.3.2
 Summary: server-sent events python client library based on requests
 Home-page: https://github.com/overcat/requests-sse
 License: Apache-2.0
 Keywords: server-sent events,sse,stream,requests
 Author: overcat
 Author-email: 4catcode@gmail.com
 Maintainer: overcat
@@ -40,15 +40,15 @@
 
 .. image:: https://img.shields.io/github/actions/workflow/status/overcat/requests-sse/test-deploy.yml?branch=main
     :alt: GitHub Workflow Status
     :target: https://github.com/overcat/requests-sse/actions
 .. image:: https://img.shields.io/pypi/v/requests-sse.svg
     :alt: PyPI
     :target: https://pypi.python.org/pypi/requests-sse
-.. image:: https://img.shields.io/badge/python-%3E%3D3.8-blue
+.. image:: https://img.shields.io/badge/python-%3E%3D37-blue
     :alt: Python - Version
     :target: https://pypi.python.org/pypi/stellar-sdk
 
 A Server-Sent Events python client based on requests, provides a simple interface to process `Server-Sent Events <https://www.w3.org/TR/eventsource>`_.
 
 Installation
 ------------
```

