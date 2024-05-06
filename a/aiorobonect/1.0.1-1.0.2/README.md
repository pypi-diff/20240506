# Comparing `tmp/aiorobonect-1.0.1.tar.gz` & `tmp/aiorobonect-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorobonect-1.0.1.tar", last modified: Mon Dec 11 16:53:52 2023, max compression
+gzip compressed data, was "aiorobonect-1.0.2.tar", last modified: Mon May  6 11:02:45 2024, max compression
```

## Comparing `aiorobonect-1.0.1.tar` & `aiorobonect-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:53:52.744487 aiorobonect-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-11 16:53:28.000000 aiorobonect-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2023-12-11 16:53:52.744487 aiorobonect-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2023-12-11 16:53:28.000000 aiorobonect-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:53:52.744487 aiorobonect-1.0.1/aiorobonect/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-11 16:53:28.000000 aiorobonect-1.0.1/aiorobonect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5716 2023-12-11 16:53:28.000000 aiorobonect-1.0.1/aiorobonect/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-12-11 16:53:28.000000 aiorobonect-1.0.1/aiorobonect/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-11 16:53:28.000000 aiorobonect-1.0.1/aiorobonect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 16:53:52.744487 aiorobonect-1.0.1/aiorobonect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2023-12-11 16:53:52.000000 aiorobonect-1.0.1/aiorobonect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-12-11 16:53:52.000000 aiorobonect-1.0.1/aiorobonect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 16:53:52.000000 aiorobonect-1.0.1/aiorobonect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-11 16:53:52.000000 aiorobonect-1.0.1/aiorobonect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-11 16:53:52.000000 aiorobonect-1.0.1/aiorobonect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-12-11 16:53:52.744487 aiorobonect-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-12-11 16:53:31.000000 aiorobonect-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:02:45.426974 aiorobonect-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-06 11:02:15.000000 aiorobonect-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-06 11:02:45.430974 aiorobonect-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-06 11:02:15.000000 aiorobonect-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:02:45.426974 aiorobonect-1.0.2/aiorobonect/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 11:02:15.000000 aiorobonect-1.0.2/aiorobonect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-06 11:02:15.000000 aiorobonect-1.0.2/aiorobonect/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 11:02:15.000000 aiorobonect-1.0.2/aiorobonect/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-06 11:02:15.000000 aiorobonect-1.0.2/aiorobonect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:02:45.426974 aiorobonect-1.0.2/aiorobonect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-06 11:02:45.000000 aiorobonect-1.0.2/aiorobonect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-06 11:02:45.000000 aiorobonect-1.0.2/aiorobonect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:02:45.000000 aiorobonect-1.0.2/aiorobonect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-06 11:02:45.000000 aiorobonect-1.0.2/aiorobonect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 11:02:45.000000 aiorobonect-1.0.2/aiorobonect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-06 11:02:45.430974 aiorobonect-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-06 11:02:21.000000 aiorobonect-1.0.2/setup.py
```

### Comparing `aiorobonect-1.0.1/LICENSE` & `aiorobonect-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiorobonect-1.0.1/PKG-INFO` & `aiorobonect-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 1.0.1
+Version: 1.0.2
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,15 +13,15 @@
 License-File: LICENSE
 
 # aiorobonect
 
 Asynchronous library to communicate with the Robonect API
 
 [![maintainer](https://img.shields.io/badge/maintainer-Geert%20Meersman-green?style=for-the-badge&logo=github)](https://github.com/geertmeersman)
-[![buyme_coffee](https://img.shields.io/badge/Buy%20me%20a%20Duvel-donate-yellow?style=for-the-badge&logo=buymeacoffee)](https://www.buymeacoffee.com/geertmeersman)
+[![buyme_coffee](https://img.shields.io/badge/Buy%20me%20an%20Omer-donate-yellow?style=for-the-badge&logo=buymeacoffee)](https://www.buymeacoffee.com/geertmeersman)
 [![discord](https://img.shields.io/discord/1094198226493636638?style=for-the-badge&logo=discord)](https://discord.gg/f6qxuMA4)
 
 [![MIT License](https://img.shields.io/github/license/geertmeersman/miwa?style=flat-square)](https://github.com/geertmeersman/miwa/blob/master/LICENSE)
 
 [![GitHub issues](https://img.shields.io/github/issues/geertmeersman/aiorobonect)](https://github.com/geertmeersman/aiorobonect/issues)
 [![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/geertmeersman/aiorobonect.svg)](http://isitmaintained.com/project/geertmeersman/aiorobonect)
 [![Percentage of issues still open](http://isitmaintained.com/badge/open/geertmeersman/aiorobonect.svg)](http://isitmaintained.com/project/geertmeersman/aiorobonect)
@@ -31,24 +31,23 @@
 
 [![github release](https://img.shields.io/github/v/release/geertmeersman/aiorobonect?logo=github)](https://github.com/geertmeersman/aiorobonect/releases)
 [![github release date](https://img.shields.io/github/release-date/geertmeersman/aiorobonect)](https://github.com/geertmeersman/aiorobonect/releases)
 [![github last-commit](https://img.shields.io/github/last-commit/geertmeersman/aiorobonect)](https://github.com/geertmeersman/aiorobonect/commits)
 [![github contributors](https://img.shields.io/github/contributors/geertmeersman/aiorobonect)](https://github.com/geertmeersman/aiorobonect/graphs/contributors)
 [![github commit activity](https://img.shields.io/github/commit-activity/y/geertmeersman/aiorobonect?logo=github)](https://github.com/geertmeersman/aiorobonect/commits/main)
 
-
 ## API Example
 
 ```python
 """Test for aiorobonect."""
 from aiorobonect import RobonectClient
 
 import asyncio
 import json
-import aiohttp
+import httpx
 
 async def main():
     host = "10.0.0.99"        ## The Robonect mower IP
     username = "USERNAME"    ## Your Robonect username
     password = "xxxxxxxx"    ## Your Robonect password
     tracking = [             ## Commands to query
                 "battery",
@@ -61,13 +60,13 @@
     client = RobonectClient(host, username, password)
     try:
         status = await client.async_cmd("status")
         print(status)
         tracking = await client.async_cmds(tracking)
         print(json.dumps(tracking, indent=2))
     except Exception as exception:
-        if isinstance(exception, aiohttp.ClientResponseError):
+        if isinstance(exception, httpx.HTTPStatusError):
             print(exception)
     await client.session_close()
 
 asyncio.run(main())
 ```
```

### Comparing `aiorobonect-1.0.1/README.md` & `aiorobonect-1.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # aiorobonect
 
 Asynchronous library to communicate with the Robonect API
 
 [![maintainer](https://img.shields.io/badge/maintainer-Geert%20Meersman-green?style=for-the-badge&logo=github)](https://github.com/geertmeersman)
-[![buyme_coffee](https://img.shields.io/badge/Buy%20me%20a%20Duvel-donate-yellow?style=for-the-badge&logo=buymeacoffee)](https://www.buymeacoffee.com/geertmeersman)
+[![buyme_coffee](https://img.shields.io/badge/Buy%20me%20an%20Omer-donate-yellow?style=for-the-badge&logo=buymeacoffee)](https://www.buymeacoffee.com/geertmeersman)
 [![discord](https://img.shields.io/discord/1094198226493636638?style=for-the-badge&logo=discord)](https://discord.gg/f6qxuMA4)
 
 [![MIT License](https://img.shields.io/github/license/geertmeersman/miwa?style=flat-square)](https://github.com/geertmeersman/miwa/blob/master/LICENSE)
 
 [![GitHub issues](https://img.shields.io/github/issues/geertmeersman/aiorobonect)](https://github.com/geertmeersman/aiorobonect/issues)
 [![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/geertmeersman/aiorobonect.svg)](http://isitmaintained.com/project/geertmeersman/aiorobonect)
 [![Percentage of issues still open](http://isitmaintained.com/badge/open/geertmeersman/aiorobonect.svg)](http://isitmaintained.com/project/geertmeersman/aiorobonect)
@@ -17,24 +17,23 @@
 
 [![github release](https://img.shields.io/github/v/release/geertmeersman/aiorobonect?logo=github)](https://github.com/geertmeersman/aiorobonect/releases)
 [![github release date](https://img.shields.io/github/release-date/geertmeersman/aiorobonect)](https://github.com/geertmeersman/aiorobonect/releases)
 [![github last-commit](https://img.shields.io/github/last-commit/geertmeersman/aiorobonect)](https://github.com/geertmeersman/aiorobonect/commits)
 [![github contributors](https://img.shields.io/github/contributors/geertmeersman/aiorobonect)](https://github.com/geertmeersman/aiorobonect/graphs/contributors)
 [![github commit activity](https://img.shields.io/github/commit-activity/y/geertmeersman/aiorobonect?logo=github)](https://github.com/geertmeersman/aiorobonect/commits/main)
 
-
 ## API Example
 
 ```python
 """Test for aiorobonect."""
 from aiorobonect import RobonectClient
 
 import asyncio
 import json
-import aiohttp
+import httpx
 
 async def main():
     host = "10.0.0.99"        ## The Robonect mower IP
     username = "USERNAME"    ## Your Robonect username
     password = "xxxxxxxx"    ## Your Robonect password
     tracking = [             ## Commands to query
                 "battery",
@@ -47,13 +46,13 @@
     client = RobonectClient(host, username, password)
     try:
         status = await client.async_cmd("status")
         print(status)
         tracking = await client.async_cmds(tracking)
         print(json.dumps(tracking, indent=2))
     except Exception as exception:
-        if isinstance(exception, aiohttp.ClientResponseError):
+        if isinstance(exception, httpx.HTTPStatusError):
             print(exception)
     await client.session_close()
 
 asyncio.run(main())
 ```
```

### Comparing `aiorobonect-1.0.1/aiorobonect/client.py` & `aiorobonect-1.0.2/aiorobonect/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 from datetime import datetime
 import json
 import logging
 import urllib.parse
 
-import aiohttp
+import httpx
 
 from .const import TIMEOUT
 from .utils import transform_json_to_single_depth
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -52,97 +52,84 @@
 
     def __init__(self, host, username, password, transform_json=False) -> None:
         """Initialize the Communication API to get data."""
         self.auth = None
         self.host = host
         self.username = username
         self.password = password
-        self.session = None
+        self.client = None
         self.sleeping = None
         self.transform_json = transform_json
         if username is not None and password is not None:
-            self.auth = aiohttp.BasicAuth(login=username, password=password)
+            self.auth = (username, password)
 
-    def session_start(self):
-        """Start the aiohttp session."""
-        if self.session:
-            return True
-        if self.username is not None and self.password is not None:
-            self.session = aiohttp.ClientSession(read_timeout=TIMEOUT, auth=self.auth)
-            return True
-        return False
-
-    async def session_close(self):
-        """Close the session."""
-        if self.session:
-            await self.session.close()
-        self.session = None
+    async def client_start(self):
+        """Start the httpx client."""
+        if not self.client:
+            self.client = httpx.AsyncClient(timeout=TIMEOUT, auth=self.auth)
+
+    async def client_close(self):
+        """Close the httpx client."""
+        if self.client:
+            await self.client.aclose()
+            self.client = None
 
     async def async_cmd(self, command=None, params={}) -> list[dict]:
         """Send command to mower."""
         if command is None:
             return False
         if params is None:
             params = ""
         else:
             params = urllib.parse.urlencode(params)
 
         if command == "job":
             _LOGGER.debug(f"Job params: {params}")
             return
 
-        result = None
-        self.session_start()
-        try:
-            _LOGGER.debug(f"Calling http://{self.host}/json?cmd={command}&{params}")
-            async with self.session.get(
-                f"http://{self.host}/json?cmd={command}&{params}"
-            ) as response:
-                if response.status == 200:
-                    result_text = await response.text(encoding="iso-8859-15")
-                    _LOGGER.debug(f"Rest API call result for {command}: {result_text}")
-                    # Load JSON data from response text
-                    result_json = json.loads(result_text)
-                    # Add the epoch timestamp to the JSON result
-                    result_json["sync_time"] = datetime.now()
-                if response.status >= 400:
-                    await self.session_close()
-                    response.raise_for_status()
-            await self.session_close()
-            if self.transform_json:
-                return transform_json_to_single_depth(result_json)
-            return result_json
-        except json.JSONDecodeError as exception:
-            await self.session_close()
-            raise RobonectException(command, exception, result)
-        except Exception as exception:
-            await self.session_close()
-            raise exception
+        result_json = None
+        await self.client_start()
+        url = f"http://{self.host}/json?cmd={command}&{params}"
+        _LOGGER.debug(f"Calling {url}")
+        response = await self.client.get(url)
+        if response.status_code == 200:
+            result_text = response.text
+            _LOGGER.debug(f"Rest API call result for {command}: {result_text}")
+            result_json = json.loads(result_text)
+            result_json["sync_time"] = datetime.now()
+        elif response.status_code >= 400:
+            response.raise_for_status()
+        await self.client_close()
+
+        if self.transform_json:
+            return transform_json_to_single_depth(result_json)
+
+        return result_json
 
     async def async_cmds(self, commands=None, bypass_sleeping=False) -> dict:
         """Send command to mower."""
-        self.session_start()
+        await self.client_start()
         result = await self.state()
         if result:
             result = {"status": result}
             if not self.sleeping or bypass_sleeping:
                 for cmd in commands:
                     json_res = await self.async_cmd(cmd)
                     if json_res:
                         result.update({cmd: json_res})
-            await self.session_close()
+            await self.client_close()
         return result
 
     async def state(self) -> dict:
         """Send status command to mower."""
-        self.session_start()
+        await self.client_start()
         result = await self.async_cmd("status")
         if result:
             self.sleeping = result.get("status").get("status") == 17
-            await self.session_close()
+            await self.client_close()
         return result
 
     async def async_start(self) -> bool:
         """Start the mower."""
         result = await self.async_cmd("start")
         return result
```

### Comparing `aiorobonect-1.0.1/aiorobonect.egg-info/PKG-INFO` & `aiorobonect-1.0.2/aiorobonect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 1.0.1
+Version: 1.0.2
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,15 +13,15 @@
 License-File: LICENSE
 
 # aiorobonect
 
 Asynchronous library to communicate with the Robonect API
 
 [![maintainer](https://img.shields.io/badge/maintainer-Geert%20Meersman-green?style=for-the-badge&logo=github)](https://github.com/geertmeersman)
-[![buyme_coffee](https://img.shields.io/badge/Buy%20me%20a%20Duvel-donate-yellow?style=for-the-badge&logo=buymeacoffee)](https://www.buymeacoffee.com/geertmeersman)
+[![buyme_coffee](https://img.shields.io/badge/Buy%20me%20an%20Omer-donate-yellow?style=for-the-badge&logo=buymeacoffee)](https://www.buymeacoffee.com/geertmeersman)
 [![discord](https://img.shields.io/discord/1094198226493636638?style=for-the-badge&logo=discord)](https://discord.gg/f6qxuMA4)
 
 [![MIT License](https://img.shields.io/github/license/geertmeersman/miwa?style=flat-square)](https://github.com/geertmeersman/miwa/blob/master/LICENSE)
 
 [![GitHub issues](https://img.shields.io/github/issues/geertmeersman/aiorobonect)](https://github.com/geertmeersman/aiorobonect/issues)
 [![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/geertmeersman/aiorobonect.svg)](http://isitmaintained.com/project/geertmeersman/aiorobonect)
 [![Percentage of issues still open](http://isitmaintained.com/badge/open/geertmeersman/aiorobonect.svg)](http://isitmaintained.com/project/geertmeersman/aiorobonect)
@@ -31,24 +31,23 @@
 
 [![github release](https://img.shields.io/github/v/release/geertmeersman/aiorobonect?logo=github)](https://github.com/geertmeersman/aiorobonect/releases)
 [![github release date](https://img.shields.io/github/release-date/geertmeersman/aiorobonect)](https://github.com/geertmeersman/aiorobonect/releases)
 [![github last-commit](https://img.shields.io/github/last-commit/geertmeersman/aiorobonect)](https://github.com/geertmeersman/aiorobonect/commits)
 [![github contributors](https://img.shields.io/github/contributors/geertmeersman/aiorobonect)](https://github.com/geertmeersman/aiorobonect/graphs/contributors)
 [![github commit activity](https://img.shields.io/github/commit-activity/y/geertmeersman/aiorobonect?logo=github)](https://github.com/geertmeersman/aiorobonect/commits/main)
 
-
 ## API Example
 
 ```python
 """Test for aiorobonect."""
 from aiorobonect import RobonectClient
 
 import asyncio
 import json
-import aiohttp
+import httpx
 
 async def main():
     host = "10.0.0.99"        ## The Robonect mower IP
     username = "USERNAME"    ## Your Robonect username
     password = "xxxxxxxx"    ## Your Robonect password
     tracking = [             ## Commands to query
                 "battery",
@@ -61,13 +60,13 @@
     client = RobonectClient(host, username, password)
     try:
         status = await client.async_cmd("status")
         print(status)
         tracking = await client.async_cmds(tracking)
         print(json.dumps(tracking, indent=2))
     except Exception as exception:
-        if isinstance(exception, aiohttp.ClientResponseError):
+        if isinstance(exception, httpx.HTTPStatusError):
             print(exception)
     await client.session_close()
 
 asyncio.run(main())
 ```
```

### Comparing `aiorobonect-1.0.1/setup.cfg` & `aiorobonect-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `aiorobonect-1.0.1/setup.py` & `aiorobonect-1.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[val.strip() for val in open("requirements.txt")],
-    version="v1.0.1",
+    version="v1.0.2",
 )
```

