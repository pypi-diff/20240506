# Comparing `tmp/fastapi_user_limiter-1.0.0.tar.gz` & `tmp/fastapi_user_limiter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_user_limiter-1.0.0.tar", last modified: Thu May  2 13:00:33 2024, max compression
+gzip compressed data, was "fastapi_user_limiter-1.1.0.tar", last modified: Mon May  6 12:04:45 2024, max compression
```

## Comparing `fastapi_user_limiter-1.0.0.tar` & `fastapi_user_limiter-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:00:33.796290 fastapi_user_limiter-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-02 13:00:33.796290 fastapi_user_limiter-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-02 13:00:26.000000 fastapi_user_limiter-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-02 13:00:26.000000 fastapi_user_limiter-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:00:33.796290 fastapi_user_limiter-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:00:33.796290 fastapi_user_limiter-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:00:33.796290 fastapi_user_limiter-1.0.0/src/fastapi_user_limiter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:00:26.000000 fastapi_user_limiter-1.0.0/src/fastapi_user_limiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-02 13:00:26.000000 fastapi_user_limiter-1.0.0/src/fastapi_user_limiter/limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:00:33.796290 fastapi_user_limiter-1.0.0/src/fastapi_user_limiter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-02 13:00:33.000000 fastapi_user_limiter-1.0.0/src/fastapi_user_limiter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-02 13:00:33.000000 fastapi_user_limiter-1.0.0/src/fastapi_user_limiter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:00:33.000000 fastapi_user_limiter-1.0.0/src/fastapi_user_limiter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 13:00:33.000000 fastapi_user_limiter-1.0.0/src/fastapi_user_limiter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 13:00:33.000000 fastapi_user_limiter-1.0.0/src/fastapi_user_limiter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:04:45.537661 fastapi_user_limiter-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-06 12:04:45.537661 fastapi_user_limiter-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-06 12:04:29.000000 fastapi_user_limiter-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-06 12:04:29.000000 fastapi_user_limiter-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 12:04:45.537661 fastapi_user_limiter-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:04:45.537661 fastapi_user_limiter-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:04:45.537661 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:04:29.000000 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-06 12:04:29.000000 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter/limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:04:45.537661 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-06 12:04:45.000000 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-06 12:04:45.000000 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 12:04:45.000000 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 12:04:45.000000 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 12:04:45.000000 fastapi_user_limiter-1.1.0/src/fastapi_user_limiter.egg-info/top_level.txt
```

### Comparing `fastapi_user_limiter-1.0.0/PKG-INFO` & `fastapi_user_limiter-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_user_limiter
-Version: 1.0.0
+Version: 1.1.0
 Summary: Rate-limiter for FastAPI with the possibility of user-based rate limits
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/fastapi-user-limiter
 Project-URL: Bug Tracker, https://github.com/epflgraph/fastapi-user-limiter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -101,18 +101,18 @@
 ```python
 from fastapi_user_limiter.limiter import rate_limiter
 from fastapi import Depends, FastAPI
 
 app = FastAPI()
 
 
-def get_user(headers):
+def get_user(headers, url):
     # The username is assumed to be a bearer token,
     # contained in the 'authorization' header.
-    username = headers['authorization'].strip('Bearer ')
+    username = headers['authorization'].replace('Bearer ', '')
     return username
 
 # 3 requests max per 20 seconds, per user
 @app.post("/auth",
           dependencies=[Depends(rate_limiter(3, 20,
                                              user=get_user))])
 async def read_with_auth(data: dict):
```

### Comparing `fastapi_user_limiter-1.0.0/README.md` & `fastapi_user_limiter-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -86,18 +86,18 @@
 ```python
 from fastapi_user_limiter.limiter import rate_limiter
 from fastapi import Depends, FastAPI
 
 app = FastAPI()
 
 
-def get_user(headers):
+def get_user(headers, url):
     # The username is assumed to be a bearer token,
     # contained in the 'authorization' header.
-    username = headers['authorization'].strip('Bearer ')
+    username = headers['authorization'].replace('Bearer ', '')
     return username
 
 # 3 requests max per 20 seconds, per user
 @app.post("/auth",
           dependencies=[Depends(rate_limiter(3, 20,
                                              user=get_user))])
 async def read_with_auth(data: dict):
```

### Comparing `fastapi_user_limiter-1.0.0/pyproject.toml` & `fastapi_user_limiter-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastapi_user_limiter"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Ramtin Yazdanian", email="ramtin.yazdanian@epfl.ch" }
 ]
 description = "Rate-limiter for FastAPI with the possibility of user-based rate limits"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `fastapi_user_limiter-1.0.0/src/fastapi_user_limiter/limiter.py` & `fastapi_user_limiter-1.1.0/src/fastapi_user_limiter/limiter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import redis.asyncio as redis
 from fastapi import Request, HTTPException, status
+from starlette.datastructures import Headers, URL
 import time
 import random
 from typing import Union, Callable
 
 
 DEFAULT_REDIS_URL = 'redis://localhost:6379/1'
 
@@ -62,15 +63,16 @@
 
 def get_rate_limited_message(max_requests, window):
     return (f"Too many requests, no more than {max_requests} requests "
             f"are allowed every {window} seconds.")
 
 
 def rate_limiter(max_requests: Union[int, None] = 10, window: Union[int, None] = 1,
-                 path: Union[str, None] = None, user: Union[Callable, None] = None,
+                 path: Union[str, None] = None,
+                 user: Union[Callable[[Headers, URL], Union[str, dict]], None] = None,
                  redis_url: Union[str, None] = None):
     """
     Rate limiter dependency for FastAPI
     :param max_requests: Max # of requests in given time window
     :param window: Time window in seconds
     :param path: Custom path.
                  Can be used for a router-wide (or even API-wide) rate limit that applies to all
@@ -82,34 +84,47 @@
                  Can be used with a custom callable that extracts the username from request header
                  in order to have a per-user rate-limit, rather than per-IP.
                  If None, the host of the client is used as the username.
     :param redis_url: URL for Redis server
     :return: Rate limiting async callable to be used as FastAPI dependency
     """
     async def _rate_limit(request: Request):
-        rlc = RateLimiterConnection(redis_url)
         # Providing a None value for either window or max_requests disables rate limiting
         if max_requests is None or window is None:
             return
+        n_max_requests = max_requests
+        window_size = window
+        rlc = RateLimiterConnection(redis_url)
         # Checking to see if a custom callable has been provided for the username
         if user is None:
             user_name = request.client.host
         else:
-            user_name = await user(request.headers)
+            user_output = await user(request.headers, request.url)
+            if isinstance(user_output, str):
+                user_name = user_output
+            else:
+                assert 'username' in user_output.keys()
+                user_name = user_output['username']
+                n_max_requests = user_output.get('max_requests', n_max_requests)
+                window_size = user_output.get('window', window_size)
+                # Here we check again because the values may have been overridden
+                if n_max_requests is None or window_size is None:
+                    return
+
         # Checking to see if a custom path has been provided
         if path is None:
             path_name = request.url.path
         else:
             path_name = path
         # Generating the redis key
-        key = f"rate_limit:{path_name}:{window}:{max_requests}:{user_name}"
-        if await rlc.is_rate_limited(key, max_requests, window):
+        key = f"rate_limit:{path_name}:{window_size}:{n_max_requests}:{user_name}"
+        if await rlc.is_rate_limited(key, n_max_requests, window_size):
             raise HTTPException(
                 status_code=status.HTTP_429_TOO_MANY_REQUESTS,
-                detail=get_rate_limited_message(max_requests, window)
+                detail=get_rate_limited_message(n_max_requests, window_size)
             )
     return _rate_limit
 
 
 def dummy_rate_limiter():
     """
     Dummy rate limiter for pytest dependency override
```

### Comparing `fastapi_user_limiter-1.0.0/src/fastapi_user_limiter.egg-info/PKG-INFO` & `fastapi_user_limiter-1.1.0/src/fastapi_user_limiter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_user_limiter
-Version: 1.0.0
+Version: 1.1.0
 Summary: Rate-limiter for FastAPI with the possibility of user-based rate limits
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/fastapi-user-limiter
 Project-URL: Bug Tracker, https://github.com/epflgraph/fastapi-user-limiter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -101,18 +101,18 @@
 ```python
 from fastapi_user_limiter.limiter import rate_limiter
 from fastapi import Depends, FastAPI
 
 app = FastAPI()
 
 
-def get_user(headers):
+def get_user(headers, url):
     # The username is assumed to be a bearer token,
     # contained in the 'authorization' header.
-    username = headers['authorization'].strip('Bearer ')
+    username = headers['authorization'].replace('Bearer ', '')
     return username
 
 # 3 requests max per 20 seconds, per user
 @app.post("/auth",
           dependencies=[Depends(rate_limiter(3, 20,
                                              user=get_user))])
 async def read_with_auth(data: dict):
```

