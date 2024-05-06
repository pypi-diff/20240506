# Comparing `tmp/heaven-0.3.3.tar.gz` & `tmp/heaven-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaven-0.3.3.tar", max compression
+gzip compressed data, was "heaven-0.3.4.tar", max compression
```

## Comparing `heaven-0.3.3.tar` & `heaven-0.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-09-07 11:01:19.761432 heaven-0.3.3/LICENSE
--rw-r--r--   0        0        0     1300 2023-09-07 11:01:19.761530 heaven-0.3.3/README.md
--rw-r--r--   0        0        0      216 2024-04-01 15:46:30.995949 heaven-0.3.3/heaven/__init__.py
--rw-r--r--   0        0        0      787 2024-02-25 20:42:34.363535 heaven-0.3.3/heaven/constants.py
--rw-r--r--   0        0        0      261 2023-09-07 11:01:19.764194 heaven-0.3.3/heaven/context.py
--rw-r--r--   0        0        0      141 2023-09-07 11:01:19.764264 heaven-0.3.3/heaven/errors.py
--rw-r--r--   0        0        0      977 2023-09-07 11:01:19.764353 heaven-0.3.3/heaven/form.py
--rw-r--r--   0        0        0     2946 2023-09-07 11:01:19.764429 heaven-0.3.3/heaven/mocks.py
--rw-r--r--   0        0        0     4487 2024-04-01 15:42:37.904117 heaven-0.3.3/heaven/request.py
--rw-r--r--   0        0        0     5384 2024-01-20 00:20:05.299419 heaven-0.3.3/heaven/response.py
--rw-r--r--   0        0        0    24585 2024-03-27 15:30:32.380491 heaven-0.3.3/heaven/router.py
--rw-r--r--   0        0        0        0 2023-09-07 11:01:19.764867 heaven-0.3.3/heaven/server.py
--rw-r--r--   0        0        0     1504 2023-09-07 20:48:02.654119 heaven-0.3.3/heaven/tutorials.py
--rw-r--r--   0        0        0     1180 2023-09-20 10:40:19.499167 heaven-0.3.3/heaven/utils.py
--rw-r--r--   0        0        0      526 2024-04-01 15:46:05.750306 heaven-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2174 1970-01-01 00:00:00.000000 heaven-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-09-07 11:01:19.761432 heaven-0.3.4/LICENSE
+-rw-r--r--   0        0        0     1300 2023-09-07 11:01:19.761530 heaven-0.3.4/README.md
+-rw-r--r--   0        0        0      216 2024-05-06 12:52:19.398896 heaven-0.3.4/heaven/__init__.py
+-rw-r--r--   0        0        0      797 2024-05-06 12:52:03.442574 heaven-0.3.4/heaven/constants.py
+-rw-r--r--   0        0        0      261 2023-09-07 11:01:19.764194 heaven-0.3.4/heaven/context.py
+-rw-r--r--   0        0        0      141 2023-09-07 11:01:19.764264 heaven-0.3.4/heaven/errors.py
+-rw-r--r--   0        0        0      977 2023-09-07 11:01:19.764353 heaven-0.3.4/heaven/form.py
+-rw-r--r--   0        0        0     2946 2023-09-07 11:01:19.764429 heaven-0.3.4/heaven/mocks.py
+-rw-r--r--   0        0        0     4487 2024-04-01 15:42:37.904117 heaven-0.3.4/heaven/request.py
+-rw-r--r--   0        0        0     5384 2024-01-20 00:20:05.299419 heaven-0.3.4/heaven/response.py
+-rw-r--r--   0        0        0    24785 2024-05-06 12:51:20.757757 heaven-0.3.4/heaven/router.py
+-rw-r--r--   0        0        0        0 2023-09-07 11:01:19.764867 heaven-0.3.4/heaven/server.py
+-rw-r--r--   0        0        0     1504 2023-09-07 20:48:02.654119 heaven-0.3.4/heaven/tutorials.py
+-rw-r--r--   0        0        0     1180 2023-09-20 10:40:19.499167 heaven-0.3.4/heaven/utils.py
+-rw-r--r--   0        0        0      526 2024-05-06 12:52:36.874215 heaven-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2174 1970-01-01 00:00:00.000000 heaven-0.3.4/PKG-INFO
```

### Comparing `heaven-0.3.3/LICENSE` & `heaven-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `heaven-0.3.3/README.md` & `heaven-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `heaven-0.3.3/heaven/constants.py` & `heaven-0.3.4/heaven/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 METHOD_DELETE = DELETE = 'DELETE'
 METHOD_GET = GET = 'GET'
 METHOD_HEAD = HEAD = 'HEAD'
 METHOD_OPTIONS = OPTIONS = 'OPTIONS'
 METHOD_PATCH = PATCH = 'PATCH'
 METHOD_POST = POST = 'POST'
 METHOD_PUT = PUT = 'PUT'
-METHOD_WEBSOCKET = WEBSOCKET = 'WEBSOCKET'
+METHOD_SOCKET = METHOD_WEBSOCKET = SOCKET = 'SOCKET'
 METHOD_TRACE = TRACE = 'TRACE'
 METHODS = [GET, HEAD, POST, PUT, PATCH, CONNECT, TRACE, DELETE, OPTIONS]
 
 MESSAGE_NOT_FOUND = 'Not found'
 
 SHUTDOWN = 'shutdown'
 STARTUP = 'startup'
```

### Comparing `heaven-0.3.3/heaven/form.py` & `heaven-0.3.4/heaven/form.py`

 * *Files identical despite different names*

### Comparing `heaven-0.3.3/heaven/mocks.py` & `heaven-0.3.4/heaven/mocks.py`

 * *Files identical despite different names*

### Comparing `heaven-0.3.3/heaven/request.py` & `heaven-0.3.4/heaven/request.py`

 * *Files identical despite different names*

### Comparing `heaven-0.3.3/heaven/response.py` & `heaven-0.3.4/heaven/response.py`

 * *Files identical despite different names*

### Comparing `heaven-0.3.3/heaven/router.py` & `heaven-0.3.4/heaven/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,14 +421,19 @@
         if not route.startswith('/'): raise UrlError(f'{route} is not a valid route - must start with /')
         handler = _string_to_function_handler(handler)
         engine = self.subdomains.get(subdomain)
         if not isinstance(engine, Routes):
             raise SubdomainError
         engine.add(method, route, handler, router or self)
 
+    def call(self, handler: str, *args, **kwargs):
+        if isinstance(handler, str): handler = _string_to_function_handler(handler)
+        handler(self, *args, **kwargs)
+        return self
+
     @property
     def daemons(self):
         return self.__daemons
 
     @daemons.setter
     def daemons(self, afunction):
         @wraps(afunction)
```

### Comparing `heaven-0.3.3/heaven/tutorials.py` & `heaven-0.3.4/heaven/tutorials.py`

 * *Files identical despite different names*

### Comparing `heaven-0.3.3/heaven/utils.py` & `heaven-0.3.4/heaven/utils.py`

 * *Files identical despite different names*

### Comparing `heaven-0.3.3/pyproject.toml` & `heaven-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heaven"
-version = "0.3.3"
+version = "0.3.4"
 description = "Extremely Stupid Simple, Blazing Fast, Get Out of your way immediately Microframework for building Python Web Applications."
 authors = ["Raymond Ortserga <ortserga@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.6"
```

### Comparing `heaven-0.3.3/PKG-INFO` & `heaven-0.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaven
-Version: 0.3.3
+Version: 0.3.4
 Summary: Extremely Stupid Simple, Blazing Fast, Get Out of your way immediately Microframework for building Python Web Applications.
 License: MIT
 Author: Raymond Ortserga
 Author-email: ortserga@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

