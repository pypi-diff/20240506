# Comparing `tmp/blueshed_gust-0.0.3.tar.gz` & `tmp/blueshed_gust-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueshed_gust-0.0.3.tar", last modified: Mon May  6 14:03:36 2024, max compression
+gzip compressed data, was "blueshed_gust-0.0.4.tar", last modified: Mon May  6 16:43:10 2024, max compression
```

## Comparing `blueshed_gust-0.0.3.tar` & `blueshed_gust-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 14:03:36.460554 blueshed_gust-0.0.3/
--rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-06 14:03:36.460379 blueshed_gust-0.0.3/PKG-INFO
--rw-r--r--   0 peterb     (501) staff       (20)      320 2024-05-06 13:29:02.000000 blueshed_gust-0.0.3/README.md
--rw-r--r--   0 peterb     (501) staff       (20)     1879 2024-05-06 14:03:33.000000 blueshed_gust-0.0.3/pyproject.toml
--rw-r--r--   0 peterb     (501) staff       (20)       38 2024-05-06 14:03:36.460588 blueshed_gust-0.0.3/setup.cfg
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 14:03:36.457898 blueshed_gust-0.0.3/src/
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 14:03:36.457839 blueshed_gust-0.0.3/src/blueshed/
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 14:03:36.459246 blueshed_gust-0.0.3/src/blueshed/gust/
--rw-r--r--   0 peterb     (501) staff       (20)      145 2024-05-06 14:03:33.000000 blueshed_gust-0.0.3/src/blueshed/gust/__init__.py
--rw-r--r--   0 peterb     (501) staff       (20)      754 2024-05-06 10:00:21.000000 blueshed_gust-0.0.3/src/blueshed/gust/configs.py
--rw-r--r--   0 peterb     (501) staff       (20)      590 2024-05-06 10:00:21.000000 blueshed_gust-0.0.3/src/blueshed/gust/context.py
--rw-r--r--   0 peterb     (501) staff       (20)     1416 2024-05-06 10:00:21.000000 blueshed_gust-0.0.3/src/blueshed/gust/json_utils.py
--rw-r--r--   0 peterb     (501) staff       (20)     2494 2024-05-06 13:33:43.000000 blueshed_gust-0.0.3/src/blueshed/gust/main.py
--rw-r--r--   0 peterb     (501) staff       (20)     3829 2024-05-06 13:33:43.000000 blueshed_gust-0.0.3/src/blueshed/gust/routes.py
--rw-r--r--   0 peterb     (501) staff       (20)      919 2024-05-06 10:00:21.000000 blueshed_gust-0.0.3/src/blueshed/gust/static_file_handler.py
--rw-r--r--   0 peterb     (501) staff       (20)     2599 2024-05-06 13:33:43.000000 blueshed_gust-0.0.3/src/blueshed/gust/utils.py
--rw-r--r--   0 peterb     (501) staff       (20)       67 2024-05-06 13:33:43.000000 blueshed_gust-0.0.3/src/blueshed/gust/web.py
--rw-r--r--   0 peterb     (501) staff       (20)     2263 2024-05-06 10:00:21.000000 blueshed_gust-0.0.3/src/blueshed/gust/web_handler.py
--rw-r--r--   0 peterb     (501) staff       (20)     5670 2024-05-06 10:28:00.000000 blueshed_gust-0.0.3/src/blueshed/gust/websocket.py
-drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 14:03:36.459881 blueshed_gust-0.0.3/src/blueshed_gust.egg-info/
--rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-06 14:03:36.000000 blueshed_gust-0.0.3/src/blueshed_gust.egg-info/PKG-INFO
--rw-r--r--   0 peterb     (501) staff       (20)      559 2024-05-06 14:03:36.000000 blueshed_gust-0.0.3/src/blueshed_gust.egg-info/SOURCES.txt
--rw-r--r--   0 peterb     (501) staff       (20)        1 2024-05-06 14:03:36.000000 blueshed_gust-0.0.3/src/blueshed_gust.egg-info/dependency_links.txt
--rw-r--r--   0 peterb     (501) staff       (20)      124 2024-05-06 14:03:36.000000 blueshed_gust-0.0.3/src/blueshed_gust.egg-info/requires.txt
--rw-r--r--   0 peterb     (501) staff       (20)        9 2024-05-06 14:03:36.000000 blueshed_gust-0.0.3/src/blueshed_gust.egg-info/top_level.txt
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:43:10.485919 blueshed_gust-0.0.4/
+-rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-06 16:43:10.485739 blueshed_gust-0.0.4/PKG-INFO
+-rw-r--r--   0 peterb     (501) staff       (20)      320 2024-05-06 13:29:02.000000 blueshed_gust-0.0.4/README.md
+-rw-r--r--   0 peterb     (501) staff       (20)     1879 2024-05-06 16:43:04.000000 blueshed_gust-0.0.4/pyproject.toml
+-rw-r--r--   0 peterb     (501) staff       (20)       38 2024-05-06 16:43:10.485955 blueshed_gust-0.0.4/setup.cfg
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:43:10.483008 blueshed_gust-0.0.4/src/
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:43:10.482949 blueshed_gust-0.0.4/src/blueshed/
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:43:10.484519 blueshed_gust-0.0.4/src/blueshed/gust/
+-rw-r--r--   0 peterb     (501) staff       (20)      145 2024-05-06 16:43:04.000000 blueshed_gust-0.0.4/src/blueshed/gust/__init__.py
+-rw-r--r--   0 peterb     (501) staff       (20)      754 2024-05-06 10:00:21.000000 blueshed_gust-0.0.4/src/blueshed/gust/configs.py
+-rw-r--r--   0 peterb     (501) staff       (20)      590 2024-05-06 10:00:21.000000 blueshed_gust-0.0.4/src/blueshed/gust/context.py
+-rw-r--r--   0 peterb     (501) staff       (20)     1416 2024-05-06 10:00:21.000000 blueshed_gust-0.0.4/src/blueshed/gust/json_utils.py
+-rw-r--r--   0 peterb     (501) staff       (20)     2474 2024-05-06 16:40:48.000000 blueshed_gust-0.0.4/src/blueshed/gust/main.py
+-rw-r--r--   0 peterb     (501) staff       (20)     3829 2024-05-06 14:08:50.000000 blueshed_gust-0.0.4/src/blueshed/gust/routes.py
+-rw-r--r--   0 peterb     (501) staff       (20)      919 2024-05-06 10:00:21.000000 blueshed_gust-0.0.4/src/blueshed/gust/static_file_handler.py
+-rw-r--r--   0 peterb     (501) staff       (20)     2599 2024-05-06 13:33:43.000000 blueshed_gust-0.0.4/src/blueshed/gust/utils.py
+-rw-r--r--   0 peterb     (501) staff       (20)       67 2024-05-06 13:33:43.000000 blueshed_gust-0.0.4/src/blueshed/gust/web.py
+-rw-r--r--   0 peterb     (501) staff       (20)     2263 2024-05-06 10:00:21.000000 blueshed_gust-0.0.4/src/blueshed/gust/web_handler.py
+-rw-r--r--   0 peterb     (501) staff       (20)     5670 2024-05-06 10:28:00.000000 blueshed_gust-0.0.4/src/blueshed/gust/websocket.py
+drwxr-xr-x   0 peterb     (501) staff       (20)        0 2024-05-06 16:43:10.485216 blueshed_gust-0.0.4/src/blueshed_gust.egg-info/
+-rw-r--r--   0 peterb     (501) staff       (20)     1027 2024-05-06 16:43:10.000000 blueshed_gust-0.0.4/src/blueshed_gust.egg-info/PKG-INFO
+-rw-r--r--   0 peterb     (501) staff       (20)      559 2024-05-06 16:43:10.000000 blueshed_gust-0.0.4/src/blueshed_gust.egg-info/SOURCES.txt
+-rw-r--r--   0 peterb     (501) staff       (20)        1 2024-05-06 16:43:10.000000 blueshed_gust-0.0.4/src/blueshed_gust.egg-info/dependency_links.txt
+-rw-r--r--   0 peterb     (501) staff       (20)      124 2024-05-06 16:43:10.000000 blueshed_gust-0.0.4/src/blueshed_gust.egg-info/requires.txt
+-rw-r--r--   0 peterb     (501) staff       (20)        9 2024-05-06 16:43:10.000000 blueshed_gust-0.0.4/src/blueshed_gust.egg-info/top_level.txt
```

### Comparing `blueshed_gust-0.0.3/PKG-INFO` & `blueshed_gust-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueshed-gust
-Version: 0.0.3
+Version: 0.0.4
 Summary: a library.
 Author-email: Peter Bunyan <pete@blueshed.co.uk>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
```

### Comparing `blueshed_gust-0.0.3/pyproject.toml` & `blueshed_gust-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,14 @@
 
 [tool.coverage.run]
 data_file = ".venv/cache/.coverage"
 [tool.coverage.report]
 data_file = ".venv/cache/.coverage"
 
 [tool.bumpversion]
-current_version = "0.0.3"
+current_version = "0.0.4"
 commit = false
 tag = true
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "src/blueshed/gust/__init__.py"
```

### Comparing `blueshed_gust-0.0.3/src/blueshed/gust/configs.py` & `blueshed_gust-0.0.4/src/blueshed/gust/configs.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.3/src/blueshed/gust/context.py` & `blueshed_gust-0.0.4/src/blueshed/gust/context.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.3/src/blueshed/gust/json_utils.py` & `blueshed_gust-0.0.4/src/blueshed/gust/json_utils.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.3/src/blueshed/gust/main.py` & `blueshed_gust-0.0.4/src/blueshed/gust/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 """main gust module"""
 
 import asyncio
 import functools
 import inspect
 import logging
-from typing import Any, List
+import os
+from typing import Any, List, Optional, Callable
 
+from tornado.options import define, options
 from tornado.web import Application
 
 from . import context
 from .configs import WebConfig
 from .web import web
 from .web_handler import WebHandler
 from .websocket import Websocket
 
 log = logging.getLogger(__name__)
 
+define('debug', type=bool, default=False, help='auto reload')
+define('port', type=int, default=8080, help='port')
+
 
 class Gust(Application):
     """A minimal sub-class of tornado.web.Application"""
 
-    def __init__(self, routes: List = None, port: int = 8080, **kwargs):
-        self.port = port
-        # routes = routes if routes else []
-        # for path, cfg in web.route_map.items():
-        #     handler = (
-        #         WebHandler if isinstance(cfg, (WebConfig,)) else Websocket
-        #     )
-        #     routes.append((rf'{path}', handler, {'method_settings': cfg}))
-        # routes.sort(reverse=True)
-        # web.broadcaster = self
+    def __init__(
+        self,
+        routes: Optional[List] = None,
+        port: Optional[int] = None,
+        **kwargs,
+    ):
+        self.port = port if port else os.getenv('PORT', options.port)
         super().__init__(routes, **kwargs)
         web.install(self)
 
-    async def perform(self, user, func: callable, *args, **kwargs) -> Any:
+    async def perform(self, user, func: Callable, *args, **kwargs) -> Any:
         """await a function or call in a thread_pool, better yet call redis"""
         if inspect.iscoroutinefunction(func):
             log.debug('aperform: %s', func)
             with context.gust(self, user):
                 result = await func(*args, **kwargs)
         else:
             log.debug('perform: %s', func)
@@ -64,15 +66,19 @@
             log.info('listening on port: %s', self.port)
         else:
             log.warning("No 'port' in settings")
 
         if self.settings.get('debug') is True:
             log.info('running in debug mode')
 
+        await asyncio.Event().wait()
+
+    def run(self):  # pragma: no cover
         try:
-            await asyncio.Event().wait()
+            asyncio.run(self._run_())
         except (KeyboardInterrupt, SystemExit):
             # graceful shutdown
             pass
 
-    def run(self):  # pragma: no cover
-        asyncio.run(self._run_())
+
+if __name__ == "__main__":
+    Gust().run()
```

### Comparing `blueshed_gust-0.0.3/src/blueshed/gust/routes.py` & `blueshed_gust-0.0.4/src/blueshed/gust/routes.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.3/src/blueshed/gust/static_file_handler.py` & `blueshed_gust-0.0.4/src/blueshed/gust/static_file_handler.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.3/src/blueshed/gust/utils.py` & `blueshed_gust-0.0.4/src/blueshed/gust/utils.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.3/src/blueshed/gust/web_handler.py` & `blueshed_gust-0.0.4/src/blueshed/gust/web_handler.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.3/src/blueshed/gust/websocket.py` & `blueshed_gust-0.0.4/src/blueshed/gust/websocket.py`

 * *Files identical despite different names*

### Comparing `blueshed_gust-0.0.3/src/blueshed_gust.egg-info/PKG-INFO` & `blueshed_gust-0.0.4/src/blueshed_gust.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueshed-gust
-Version: 0.0.3
+Version: 0.0.4
 Summary: a library.
 Author-email: Peter Bunyan <pete@blueshed.co.uk>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
```

### Comparing `blueshed_gust-0.0.3/src/blueshed_gust.egg-info/SOURCES.txt` & `blueshed_gust-0.0.4/src/blueshed_gust.egg-info/SOURCES.txt`

 * *Files identical despite different names*

