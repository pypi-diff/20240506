# Comparing `tmp/olist_loafer-6.0.0a2.tar.gz` & `tmp/olist_loafer-6.0.0a3.tar.gz`

## Comparing `olist_loafer-6.0.0a2.tar` & `olist_loafer-6.0.0a3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/.editorconfig
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/CHANGES.rst
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/CONTRIBUTORS.rst
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/MANIFEST.in
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/Makefile
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/env.local
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/__init__.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/compat.py
--rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/dispatchers.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/exceptions.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/managers.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/message_translators.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/providers.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/routes.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/runners.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/ext/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/ext/sentry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/ext/aws/__init__.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/ext/aws/bases.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/ext/aws/handlers.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/ext/aws/message_translators.py
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/ext/aws/providers.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/src/loafer/ext/aws/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/tests/__init__.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/tests/conftest.py
--rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/tests/test_dispatchers.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/tests/test_managers.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/tests/test_message_translator.py
--rw-r--r--   0        0        0     6089 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/tests/test_routes.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/tests/test_runners.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/tests/ext/__init__.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/tests/ext/test_sentry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/tests/ext/aws/__init__.py
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/tests/ext/aws/conftest.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/tests/ext/aws/test_bases.py
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/tests/ext/aws/test_handlers.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/tests/ext/aws/test_message_translators.py
--rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/tests/ext/aws/test_providers.py
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/tests/ext/aws/test_routes.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/LICENSE
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/README.md
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/hatch.toml
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/.editorconfig
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/CHANGES.rst
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/CONTRIBUTORS.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/MANIFEST.in
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/Makefile
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/env.local
+-rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/ruff_defaults.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/compat.py
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/dispatchers.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/exceptions.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/managers.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/message_translators.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/providers.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/routes.py
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/runners.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/ext/__init__.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/ext/sentry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/ext/aws/__init__.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/ext/aws/bases.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/ext/aws/handlers.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/ext/aws/message_translators.py
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/ext/aws/providers.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/src/loafer/ext/aws/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/tests/__init__.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/tests/conftest.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/tests/test_dispatchers.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/tests/test_managers.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/tests/test_message_translator.py
+-rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/tests/test_routes.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/tests/test_runners.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/tests/ext/__init__.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/tests/ext/test_sentry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/tests/ext/aws/__init__.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/tests/ext/aws/conftest.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/tests/ext/aws/test_bases.py
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/tests/ext/aws/test_handlers.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/tests/ext/aws/test_message_translators.py
+-rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/tests/ext/aws/test_providers.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/tests/ext/aws/test_routes.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/LICENSE
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/README.md
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 olist_loafer-6.0.0a3/PKG-INFO
```

### Comparing `olist_loafer-6.0.0a2/.pre-commit-config.yaml` & `olist_loafer-6.0.0a3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `olist_loafer-6.0.0a2/CHANGES.rst` & `olist_loafer-6.0.0a3/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `olist_loafer-6.0.0a2/Makefile` & `olist_loafer-6.0.0a3/Makefile`

 * *Files identical despite different names*

### Comparing `olist_loafer-6.0.0a2/src/loafer/compat.py` & `olist_loafer-6.0.0a3/src/loafer/compat.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-6.0.0a2/src/loafer/dispatchers.py` & `olist_loafer-6.0.0a3/src/loafer/dispatchers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,49 @@
+from __future__ import annotations
+
 import asyncio
 import logging
 import sys
-from typing import Any, Optional, Sequence
+from typing import TYPE_CHECKING, Any, Sequence
 
 from .compat import TaskGroup
 from .exceptions import DeleteMessage
-from .routes import Route
+
+if TYPE_CHECKING:
+    from .routes import Route
 
 logger = logging.getLogger(__name__)
 
 
 class LoaferDispatcher:
     def __init__(
         self,
         routes: Sequence[Route],
-        max_concurrency: Optional[int] = None,
+        max_concurrency: int | None = None,
     ) -> None:
         self.routes = routes
-        self.max_concurrency = max_concurrency if max_concurrency is not None else len(routes) * 10
+        self.max_concurrency = max_concurrency if max_concurrency is not None else max(len(routes), 5)
 
     async def dispatch_message(self, message: Any, route: Route) -> bool:
-        logger.debug(f"dispatching message to route={route}")
+        logger.debug("dispatching message to route=%s", route)
         confirm_message = False
         if not message:
-            logger.warning(f"message will be ignored:\n{message!r}\n")
+            logger.warning("message will be ignored:\n%r\n", message)
             return confirm_message
 
         try:
             confirm_message = await route.deliver(message)
         except DeleteMessage:
-            logger.info(f"explicit message deletion\n{message}\n")
+            logger.info("explicit message deletion\n%s\n", message)
             confirm_message = True
         except asyncio.CancelledError:
             msg = '"{!r}" was cancelled, the message will not be acknowledged:\n{}\n'
             logger.warning(msg.format(route.handler, message))
         except Exception as exc:
-            logger.exception(f"{exc!r}")
+            logger.exception("%r", exc)  # noqa: TRY401
             exc_info = sys.exc_info()
             confirm_message = await route.error_handler(exc_info, message)
 
         return confirm_message
 
     async def _process_message(self, message: Any, route: Route) -> bool:
         confirmation = await self.dispatch_message(message, route)
@@ -50,28 +54,28 @@
             await provider.message_not_processed(message)
         return confirmation
 
     async def _fetch_messages(
         self,
         processing_queue: asyncio.Queue,
         tg: TaskGroup,
-        forever: bool = True,
+        forever: bool = True,  # noqa: FBT001, FBT002
     ) -> None:
-        routes = [route for route in self.routes]
+        routes = list(self.routes)
         tasks = [tg.create_task(route.provider.fetch_messages()) for route in routes]
 
         while routes or tasks:
             await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
 
             new_routes = []
             new_tasks = []
             for task, route in zip(tasks, routes):
                 if task.done():
-                    if task.exception():
-                        raise task.exception()
+                    if exc := task.exception():
+                        raise exc
 
                     for message in task.result():
                         await processing_queue.put((message, route))
 
                     if forever:
                         new_routes.append(route)
                         new_tasks.append(tg.create_task(route.provider.fetch_messages()))
@@ -85,15 +89,15 @@
     async def _consume_messages(self, processing_queue: asyncio.Queue) -> None:
         while True:
             message, route = await processing_queue.get()
 
             await self._process_message(message, route)
             processing_queue.task_done()
 
-    async def dispatch_providers(self, forever: bool = True) -> None:
+    async def dispatch_providers(self, forever: bool = True) -> None:  # noqa: FBT001, FBT002
         processing_queue = asyncio.Queue(self.max_concurrency)
 
         async with TaskGroup() as tg:
             provider_task = tg.create_task(self._fetch_messages(processing_queue, tg, forever))
 
             consumer_tasks = [
                 tg.create_task(self._consume_messages(processing_queue)) for _ in range(self.max_concurrency)
@@ -102,12 +106,14 @@
             async def join():
                 await provider_task
                 await processing_queue.join()
 
                 for consumer_task in consumer_tasks:
                     consumer_task.cancel()
 
+                await asyncio.gather(*consumer_tasks, return_exceptions=True)
+
             tg.create_task(join())
 
     def stop(self) -> None:
         for route in self.routes:
             route.stop()
```

### Comparing `olist_loafer-6.0.0a2/src/loafer/managers.py` & `olist_loafer-6.0.0a3/src/loafer/managers.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             self.runner = LoaferRunner(on_stop_callback=self.on_loop__stop)
         else:
             self.runner = runner
 
         self.routes = routes
         self.dispatcher = LoaferDispatcher(self.routes, max_concurrency)
 
-    def run(self, forever=True, debug=False):
+    def run(self, forever=True, debug=False):  # noqa: FBT002
         loop = self.runner.loop
         self._future = asyncio.ensure_future(
             self.dispatcher.dispatch_providers(forever=forever),
             loop=loop,
         )
 
         self._future.add_done_callback(self.on_future__errors)
@@ -40,17 +40,19 @@
     def on_future__errors(self, future):
         if future.cancelled():
             return self.runner.prepare_stop()
 
         exc = future.exception()
         # Unhandled errors crashes the event loop execution
         if isinstance(exc, BaseException):
-            logger.critical(f"fatal error caught: {exc!r}")
+            logger.critical("fatal error caught: %r", exc)
             self.runner.prepare_stop()
+            return None
+        return None
 
-    def on_loop__stop(self, *args, **kwargs):
+    def on_loop__stop(self):
         logger.info("cancel dispatcher operations ...")
 
         if hasattr(self, "_future"):
             self._future.cancel()
 
         self.dispatcher.stop()
```

### Comparing `olist_loafer-6.0.0a2/src/loafer/message_translators.py` & `olist_loafer-6.0.0a3/src/loafer/message_translators.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,9 +14,9 @@
         The `content` should contain the translated message and, `metadata` a
         dictionary with translation metadata or an empty `dict`.
         """
 
 
 class StringMessageTranslator(AbstractMessageTranslator):
     def translate(self, message):
-        logger.debug(f"{type(self).__name__!r} will translate {message!r}")
+        logger.debug("%r will translate %r", type(self).__name__, message)
         return {"content": str(message), "metadata": {}}
```

### Comparing `olist_loafer-6.0.0a2/src/loafer/providers.py` & `olist_loafer-6.0.0a3/src/loafer/providers.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 
         After the message confirmation we should not receive the same message again.
         This usually means we need to delete the message in the provider.
         """
 
     async def message_not_processed(self, message):
         """Perform actions when a message was not processed."""
-        pass
 
     def stop(self):
         """Stop the provider.
 
         If needed, the provider should perform clean-up actions.
         This method is called whenever we need to shutdown the provider.
         """
-        pass
```

### Comparing `olist_loafer-6.0.0a2/src/loafer/routes.py` & `olist_loafer-6.0.0a3/src/loafer/routes.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,72 +8,71 @@
 
 
 class Route:
     def __init__(self, provider, handler, name="default", message_translator=None, error_handler=None):
         self.name = name
 
         if not isinstance(provider, AbstractProvider):
-            raise TypeError(f"invalid provider instance: {provider!r}")
+            msg = f"invalid provider instance: {provider!r}"
+            raise TypeError(msg)
 
         self.provider = provider
 
-        if message_translator:
-            if not isinstance(message_translator, AbstractMessageTranslator):
-                raise TypeError(f"invalid message translator instance: {message_translator!r}")
+        if message_translator and not isinstance(message_translator, AbstractMessageTranslator):
+            msg = f"invalid message translator instance: {message_translator!r}"
+            raise TypeError(msg)
 
         self.message_translator = message_translator
 
-        if error_handler:
-            if not callable(error_handler):
-                raise TypeError(f"error_handler must be a callable object: {error_handler!r}")
+        if error_handler and not callable(error_handler):
+            msg = f"error_handler must be a callable object: {error_handler!r}"
+            raise TypeError(msg)
 
         self._error_handler = error_handler
 
         if callable(handler):
             self.handler = handler
             self._handler_instance = None
         else:
             self.handler = getattr(handler, "handle", None)
             self._handler_instance = handler
 
         if not self.handler:
-            raise ValueError(
-                f"handler must be a callable object or implement `handle` method: {self.handler!r}"
-            )
+            msg = f"handler must be a callable object or implement `handle` method: {self.handler!r}"
+            raise ValueError(msg)
 
     def __str__(self):
-        return "<{}(name={} provider={!r} handler={!r})>".format(
-            type(self).__name__, self.name, self.provider, self.handler
-        )
+        return f"<{type(self).__name__}(name={self.name} provider={self.provider!r} handler={self.handler!r})>"
 
     def apply_message_translator(self, message):
         processed_message = {"content": message, "metadata": {}}
         if not self.message_translator:
             return processed_message
 
         translated = self.message_translator.translate(processed_message["content"])
         processed_message["metadata"].update(translated.get("metadata", {}))
         processed_message["content"] = translated["content"]
         if not processed_message["content"]:
-            raise ValueError(f"{self.message_translator} failed to translate message={message}")
+            msg = f"{self.message_translator} failed to translate message={message}"
+            raise ValueError(msg)
 
         return processed_message
 
     async def deliver(self, raw_message):
         message = self.apply_message_translator(raw_message)
-        logger.info(f"delivering message route={self}, message={message!r}")
+        logger.info("delivering message route=%s, message=%r", self, message)
         return await ensure_coroutinefunction(self.handler, message["content"], message["metadata"])
 
     async def error_handler(self, exc_info, message):
-        logger.info(f"error handler process originated by message={message}")
+        logger.info("error handler process originated by message=%s", message)
 
         if self._error_handler is not None:
             return await ensure_coroutinefunction(self._error_handler, exc_info, message)
 
         return False
 
     def stop(self):
-        logger.info(f"stopping route {self}")
+        logger.info("stopping route %s", self)
         self.provider.stop()
         # only for class-based handlers
         if hasattr(self._handler_instance, "stop"):
             self._handler_instance.stop()
```

### Comparing `olist_loafer-6.0.0a2/src/loafer/runners.py` & `olist_loafer-6.0.0a3/src/loafer/runners.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,30 +11,30 @@
     def __init__(self, on_stop_callback=None):
         self._on_stop_callback = on_stop_callback
 
     @property
     def loop(self):
         return asyncio.get_event_loop()
 
-    def start(self, debug=False):
+    def start(self, debug=False):  # noqa: FBT002
         if debug:
             self.loop.set_debug(enabled=debug)
 
         self.loop.add_signal_handler(signal.SIGINT, self.prepare_stop)
         self.loop.add_signal_handler(signal.SIGTERM, self.prepare_stop)
 
         try:
             self.loop.run_forever()
         finally:
             self.stop()
             self.loop.close()
-            logger.debug(f"loop.is_running={self.loop.is_running()}")
-            logger.debug(f"loop.is_closed={self.loop.is_closed()}")
+            logger.debug("loop.is_running=%s", self.loop.is_running())
+            logger.debug("loop.is_closed=%s", self.loop.is_closed())
 
-    def prepare_stop(self, *args):
+    def prepare_stop(self, *args):  # noqa: ARG002
         if self.loop.is_running():
             # signals loop.run_forever to exit in the next iteration
             self.loop.stop()
 
     def _cancel_all_tasks(self):
         to_cancel = asyncio.all_tasks(self.loop)
         if not to_cancel:
@@ -51,15 +51,15 @@
                     {
                         "message": "unhandled exception during asyncio.run() shutdown",
                         "exception": task.exception(),
                         "task": task,
                     }
                 )
 
-    def stop(self, *args, **kwargs):
+    def stop(self):
         logger.info("stopping Loafer ...")
         if callable(self._on_stop_callback):
             self._on_stop_callback()
 
         logger.info("cancel schedulled operations ...")
         with suppress(CancelledError, RuntimeError):
             self._cancel_all_tasks()
```

### Comparing `olist_loafer-6.0.0a2/src/loafer/ext/aws/bases.py` & `olist_loafer-6.0.0a3/src/loafer/ext/aws/bases.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     boto_service_name = "sqs"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._cached_queue_urls = {}
 
     async def get_queue_url(self, queue):
-        if queue and (queue.startswith("http://") or queue.startswith("https://")):
+        if queue and (queue.startswith(("http://", "https://"))):
             name = queue.split("/")[-1]
             self._cached_queue_urls[name] = queue
             queue = name
 
         if queue not in self._cached_queue_urls:
             async with self.get_client() as client:
                 response = await client.get_queue_url(QueueName=queue)
```

### Comparing `olist_loafer-6.0.0a2/src/loafer/ext/aws/handlers.py` & `olist_loafer-6.0.0a3/src/loafer/ext/aws/handlers.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,26 +14,27 @@
         super().__init__(**kwargs)
 
     def __str__(self):
         return f"<{type(self).__name__}: {self.queue_name}>"
 
     async def publish(self, message, encoder=json.dumps):
         if not self.queue_name:
-            raise ValueError(f"{type(self).__name__}: missing queue_name attribute")
+            msg = f"{type(self).__name__}: missing queue_name attribute"
+            raise ValueError(msg)
 
         if encoder:
             message = encoder(message)
 
-        logger.debug(f"publishing, queue={self.queue_name}, message={message}")
+        logger.debug("publishing, queue=%s, message=%s", self.queue_name, message)
 
         queue_url = await self.get_queue_url(self.queue_name)
         async with self.get_client() as client:
             return await client.send_message(QueueUrl=queue_url, MessageBody=message)
 
-    async def handle(self, message, *args):
+    async def handle(self, message, *args):  # noqa: ARG002
         return await self.publish(message)
 
 
 class SNSHandler(BaseSNSClient):
     topic = None
 
     def __init__(self, topic=None, **kwargs):
@@ -41,21 +42,22 @@
         super().__init__(**kwargs)
 
     def __str__(self):
         return f"<{type(self).__name__}: {self.topic}>"
 
     async def publish(self, message, encoder=json.dumps):
         if not self.topic:
-            raise ValueError(f"{type(self).__name__}: missing topic attribute")
+            msg = f"{type(self).__name__}: missing topic attribute"
+            raise ValueError(msg)
 
         if encoder:
             message = encoder(message)
 
         topic_arn = await self.get_topic_arn(self.topic)
-        logger.debug(f"publishing, topic={topic_arn}, message={message}")
+        logger.debug("publishing, topic=%s, message=%s", topic_arn, message)
 
         msg = json.dumps({"default": message})
         async with self.get_client() as client:
             return await client.publish(TopicArn=topic_arn, MessageStructure="json", Message=msg)
 
-    async def handle(self, message, *args):
+    async def handle(self, message, *args):  # noqa: ARG002
         return await self.publish(message)
```

### Comparing `olist_loafer-6.0.0a2/src/loafer/ext/aws/message_translators.py` & `olist_loafer-6.0.0a3/src/loafer/ext/aws/message_translators.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,47 +8,44 @@
 
 class SQSMessageTranslator(AbstractMessageTranslator):
     def translate(self, message):
         translated = {"content": None, "metadata": {}}
         try:
             body = message["Body"]
         except (KeyError, TypeError):
-            logger.error(
-                "missing Body key in SQS message. It really came from SQS ?" "\nmessage={!r}".format(message)
-            )
+            logger.exception("missing Body key in SQS message. It really came from SQS ?\nmessage=%r", message)
             return translated
 
         try:
             translated["content"] = json.loads(body)
         except json.decoder.JSONDecodeError as exc:
-            logger.error(f"error={exc!r}, message={message!r}")
+            logger.exception("error=%r, message=%r", exc, message)  # noqa: TRY401
             return translated
 
         message.pop("Body")
         translated["metadata"].update(message)
         return translated
 
 
 class SNSMessageTranslator(AbstractMessageTranslator):
     def translate(self, message):
         translated = {"content": None, "metadata": {}}
         try:
             body = json.loads(message["Body"])
             message_body = body.pop("Message")
         except (KeyError, TypeError):
-            logger.error(
-                "Missing Body or Message key in SQS message. It really came from SNS ?"
-                "\nmessage={!r}".format(message)
+            logger.exception(
+                "Missing Body or Message key in SQS message. It really came from SNS ?\nmessage=%r", message
             )
             return translated
 
         translated["metadata"].update(message)
         translated["metadata"].pop("Body")
 
         try:
             translated["content"] = json.loads(message_body)
         except (json.decoder.JSONDecodeError, TypeError) as exc:
-            logger.error(f"error={exc!r}, message={message!r}")
+            logger.exception("error=%r, message=%r", exc, message)  # noqa: TRY401
             return translated
 
         translated["metadata"].update(body)
         return translated
```

### Comparing `olist_loafer-6.0.0a2/src/loafer/ext/aws/providers.py` & `olist_loafer-6.0.0a3/src/loafer/ext/aws/providers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import logging
+from http import HTTPStatus
 
 import botocore.exceptions
 
-from .bases import BaseSQSClient
 from loafer.exceptions import ProviderError
 from loafer.providers import AbstractProvider
 from loafer.utils import calculate_backoff_multiplier
 
+from .bases import BaseSQSClient
+
 logger = logging.getLogger(__name__)
 
 
 class SQSProvider(AbstractProvider, BaseSQSClient):
     def __init__(self, queue_name, options=None, **kwargs):
         self.queue_name = queue_name
         self._options = options or {}
@@ -24,58 +26,59 @@
         super().__init__(**kwargs)
 
     def __str__(self):
         return f"<{type(self).__name__}: {self.queue_name}>"
 
     async def confirm_message(self, message):
         receipt = message["ReceiptHandle"]
-        logger.info(f"confirm message (ack/deletion), receipt={receipt!r}")
+        logger.info("confirm message (ack/deletion), receipt=%r", receipt)
 
         queue_url = await self.get_queue_url(self.queue_name)
         try:
             async with self.get_client() as client:
                 return await client.delete_message(QueueUrl=queue_url, ReceiptHandle=receipt)
         except botocore.exceptions.ClientError as exc:
-            if exc.response["ResponseMetadata"]["HTTPStatusCode"] == 404:
+            if exc.response["ResponseMetadata"]["HTTPStatusCode"] == HTTPStatus.NOT_FOUND:
                 return True
 
             raise
 
     async def message_not_processed(self, message):
         receipt = message["ReceiptHandle"]
         if self._backoff_factor:
             backoff_multiplier = calculate_backoff_multiplier(
                 int(message["Attributes"]["ApproximateReceiveCount"]),
                 self._backoff_factor,
             )
 
             custom_visibility_timeout = round(backoff_multiplier * self._options.get("VisibilityTimeout", 30))
             logger.info(
-                f"message not processed, receipt={receipt!r}, "
-                f"custom_visibility_timeout={custom_visibility_timeout!r}"
+                "message not processed, receipt=%r, custom_visibility_timeout=%r", receipt, custom_visibility_timeout
             )
             queue_url = await self.get_queue_url(self.queue_name)
             try:
                 async with self.get_client() as client:
                     return await client.change_message_visibility(
                         QueueUrl=queue_url,
                         ReceiptHandle=receipt,
                         VisibilityTimeout=custom_visibility_timeout,
                     )
             except botocore.exceptions.ClientError as exc:
                 if "InvalidParameterValue" not in str(exc):
                     raise
+        return None
 
     async def fetch_messages(self):
-        logger.debug(f"fetching messages on {self.queue_name}")
+        logger.debug("fetching messages on %s", self.queue_name)
         try:
             queue_url = await self.get_queue_url(self.queue_name)
             async with self.get_client() as client:
                 response = await client.receive_message(QueueUrl=queue_url, **self._options)
         except (botocore.exceptions.BotoCoreError, botocore.exceptions.ClientError) as exc:
-            raise ProviderError(f"error fetching messages from queue={self.queue_name}: {str(exc)}") from exc
+            msg = f"error fetching messages from queue={self.queue_name}: {exc!s}"
+            raise ProviderError(msg) from exc
 
         return response.get("Messages", [])
 
     def stop(self):
-        logger.info(f"stopping {self}")
+        logger.info("stopping %s", self)
         return super().stop()
```

### Comparing `olist_loafer-6.0.0a2/src/loafer/ext/aws/routes.py` & `olist_loafer-6.0.0a3/src/loafer/ext/aws/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from ...routes import Route
+from loafer.routes import Route
+
 from .message_translators import SNSMessageTranslator, SQSMessageTranslator
 from .providers import SQSProvider
 
 
 class SQSRoute(Route):
     def __init__(self, provider_queue, provider_options=None, *args, **kwargs):
         provider_options = provider_options or {}
```

### Comparing `olist_loafer-6.0.0a2/tests/conftest.py` & `olist_loafer-6.0.0a3/tests/conftest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import pytest
 
 from loafer.providers import AbstractProvider
 
 
 @pytest.fixture
 def dummy_handler():
-    def handler(message, *args):
-        raise AssertionError("I should not be called")
+    def handler(message, *args):  # noqa: ARG001
+        msg = "I should not be called"
+        raise AssertionError(msg)
 
     return handler
 
 
 @pytest.fixture
 def dummy_provider():
     class Dummy(AbstractProvider):
         async def fetch_messages(self):
-            raise AssertionError("I should not be called")
+            msg = "I should not be called"
+            raise AssertionError(msg)
 
         async def confirm_message(self):
-            raise AssertionError("I should not be called")
+            msg = "I should not be called"
+            raise AssertionError(msg)
 
         async def message_not_processed(self):
-            raise AssertionError("I should not be called")
+            msg = "I should not be called"
+            raise AssertionError(msg)
 
         def stop(self):
-            raise AssertionError("I should not be called")
+            msg = "I should not be called"
+            raise AssertionError(msg)
 
     return Dummy()
```

### Comparing `olist_loafer-6.0.0a2/tests/test_dispatchers.py` & `olist_loafer-6.0.0a3/tests/test_dispatchers.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,21 @@
 def create_mock_route(messages):
     provider = mock.AsyncMock(
         fetch_messages=mock.AsyncMock(side_effect=[messages]),
         confirm_message=mock.AsyncMock(),
         message_not_processed=mock.AsyncMock(),
     )
 
-    message_translator = mock.Mock(
-        translate=mock.Mock(side_effect=[{"content": message} for message in messages])
-    )
-    route = mock.AsyncMock(
+    message_translator = mock.Mock(translate=mock.Mock(side_effect=[{"content": message} for message in messages]))
+    return mock.AsyncMock(
         provider=provider,
         handler=mock.AsyncMock(),
         message_translator=message_translator,
         spec=Route,
     )
-    return route
 
 
 @pytest.fixture
 def route():
     return create_mock_route(["message"])
```

### Comparing `olist_loafer-6.0.0a2/tests/test_managers.py` & `olist_loafer-6.0.0a3/tests/test_managers.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,12 +55,12 @@
     assert manager.runner.prepare_stop.called
     manager.runner.prepare_stop.assert_called_once_with()
 
 
 def test_on_loop__stop():
     manager = LoaferManager(routes=[])
     manager.dispatcher = mock.Mock()
-    manager._future = mock.Mock()
+    manager._future = mock.Mock()  # noqa: SLF001
     manager.on_loop__stop()
 
     assert manager.dispatcher.stop.called
-    assert manager._future.cancel.called
+    assert manager._future.cancel.called  # noqa: SLF001
```

### Comparing `olist_loafer-6.0.0a2/tests/test_routes.py` & `olist_loafer-6.0.0a3/tests/test_routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,18 +48,20 @@
     translator.translate.assert_called_once_with("message")
 
 
 def test_apply_message_translator_error(dummy_provider):
     translator = StringMessageTranslator()
     translator.translate = mock.Mock(return_value={"content": "", "metadata": {}})
     route = Route(dummy_provider, mock.Mock(), message_translator=translator)
-    with pytest.raises(ValueError):
+
+    with pytest.raises(ValueError, match="failed to translate"):
         route.apply_message_translator("message")
-        assert translator.translate.called
-        translator.translate.assert_called_once_with("message")
+
+    assert translator.translate.called
+    translator.translate.assert_called_once_with("message")
 
 
 @pytest.mark.asyncio
 async def test_error_handler_unset(dummy_provider):
     route = Route(dummy_provider, mock.Mock())
     exc = TypeError()
     exc_info = (type(exc), exc, None)
@@ -102,54 +104,54 @@
     assert result is True
     assert error_handler.called
     error_handler.assert_called_once_with(exc_info, "whatever")
 
 
 @pytest.mark.asyncio
 async def test_handler_class_based(dummy_provider):
-    class handler:
+    class Handler:
         async def handle(self, *args, **kwargs):
             pass
 
-    handler = handler()
+    handler = Handler()
     route = Route(dummy_provider, handler=handler)
     assert route.handler == handler.handle
 
 
 @pytest.mark.asyncio
 async def test_handler_class_based_invalid(dummy_provider):
-    class handler:
+    class Handler:
         pass
 
-    handler = handler()
-    with pytest.raises(ValueError):
+    handler = Handler()
+    with pytest.raises(ValueError, match="handler must be a callable object"):
         Route(dummy_provider, handler=handler)
 
 
 @pytest.mark.asyncio
 async def test_handler_invalid(dummy_provider):
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="handler must be a callable object"):
         Route(dummy_provider, "invalid-handler")
 
 
 def test_route_stop(dummy_provider):
     dummy_provider.stop = mock.Mock()
     route = Route(dummy_provider, handler=mock.Mock())
     route.stop()
 
     assert dummy_provider.stop.called
 
 
 def test_route_stop_with_handler_stop(dummy_provider):
-    class handler:
+    class Handler:
         def handle(self, *args):
             pass
 
     dummy_provider.stop = mock.Mock()
-    handler = handler()
+    handler = Handler()
     handler.stop = mock.Mock()
     route = Route(dummy_provider, handler)
     route.stop()
 
     assert dummy_provider.stop.called
     assert handler.stop.called
```

### Comparing `olist_loafer-6.0.0a2/tests/test_runners.py` & `olist_loafer-6.0.0a3/tests/test_runners.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,27 +55,26 @@
 
     runner.prepare_stop()
 
     loop.is_running.assert_called_once_with()
     assert loop.stop.called is False
 
 
-@mock.patch("loafer.runners.asyncio.get_event_loop")
-def test_runner_stop_with_callback(loop_mock):
+def test_runner_stop_with_callback():
     callback = mock.Mock()
     runner = LoaferRunner(on_stop_callback=callback)
 
     runner.stop()
 
     assert callback.called
 
 
 def test_runner_stop_dont_raise_cancelled_error():
     async def some_coro():
-        raise asyncio.CancelledError()
+        raise asyncio.CancelledError
 
     runner = LoaferRunner()
     loop = runner.loop
     task = loop.create_task(some_coro())
 
     assert task.done() is False
     assert task.cancelled() is False
```

### Comparing `olist_loafer-6.0.0a2/tests/ext/test_sentry.py` & `olist_loafer-6.0.0a3/tests/ext/test_sentry.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-6.0.0a2/tests/ext/aws/conftest.py` & `olist_loafer-6.0.0a3/tests/ext/aws/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,25 +59,21 @@
     mock_client.change_message_visibility = mock.AsyncMock()
     mock_client.close = mock.AsyncMock()
     return mock_client
 
 
 @pytest.fixture
 def mock_boto_session_sqs(boto_client_sqs):
-    return mock.patch(
-        "loafer.ext.aws.bases.session.create_client", return_value=ClientContextCreator(boto_client_sqs)
-    )
+    return mock.patch("loafer.ext.aws.bases.session.create_client", return_value=ClientContextCreator(boto_client_sqs))
 
 
 @pytest.fixture
-def boto_client_sns(sns_publish, sns_list_topics):
+def boto_client_sns(sns_publish):
     mock_client = mock.Mock()
     mock_client.publish = mock.AsyncMock(return_value=sns_publish)
     mock_client.close = mock.AsyncMock()
     return mock_client
 
 
 @pytest.fixture
 def mock_boto_session_sns(boto_client_sns):
-    return mock.patch(
-        "loafer.ext.aws.bases.session.create_client", return_value=ClientContextCreator(boto_client_sns)
-    )
+    return mock.patch("loafer.ext.aws.bases.session.create_client", return_value=ClientContextCreator(boto_client_sns))
```

### Comparing `olist_loafer-6.0.0a2/tests/ext/aws/test_bases.py` & `olist_loafer-6.0.0a3/tests/ext/aws/test_bases.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-6.0.0a2/tests/ext/aws/test_handlers.py` & `olist_loafer-6.0.0a3/tests/ext/aws/test_handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             QueueUrl=await handler.get_queue_url("queue-name"), MessageBody="message"
         )
 
 
 @pytest.mark.asyncio
 async def test_sqs_handler_publish_without_queue_name():
     handler = SQSHandler()
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="missing queue_name attribute"):
         await handler.publish("wrong")
 
 
 @pytest.mark.asyncio
 async def test_sqs_handler_hadle():
     handler = SQSHandler("foobar")
     handler.publish = mock.AsyncMock()
@@ -88,15 +88,15 @@
             Message=json.dumps({"default": "message"}),
         )
 
 
 @pytest.mark.asyncio
 async def test_sns_handler_publish_without_topic():
     handler = SNSHandler()
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="missing topic attribute"):
         await handler.publish("wrong")
 
 
 @pytest.mark.asyncio
 async def test_sns_handler_hadle():
     handler = SNSHandler("foobar")
     handler.publish = mock.AsyncMock()
```

### Comparing `olist_loafer-6.0.0a2/tests/ext/aws/test_message_translators.py` & `olist_loafer-6.0.0a3/tests/ext/aws/test_message_translators.py`

 * *Files identical despite different names*

### Comparing `olist_loafer-6.0.0a2/tests/ext/aws/test_providers.py` & `olist_loafer-6.0.0a3/tests/ext/aws/test_providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,34 +18,30 @@
         assert boto_client_sqs.delete_message.call_args == mock.call(
             QueueUrl=await provider.get_queue_url("queue-name"), ReceiptHandle="message-receipt-handle"
         )
 
 
 @pytest.mark.asyncio
 async def test_confirm_message_not_found(mock_boto_session_sqs, boto_client_sqs):
-    error = ClientError(
-        error_response={"ResponseMetadata": {"HTTPStatusCode": 404}}, operation_name="whatever"
-    )
+    error = ClientError(error_response={"ResponseMetadata": {"HTTPStatusCode": 404}}, operation_name="whatever")
     boto_client_sqs.delete_message.side_effect = error
     with mock_boto_session_sqs:
         provider = SQSProvider("queue-name")
         message = {"ReceiptHandle": "message-receipt-handle-not-found"}
         await provider.confirm_message(message)
 
         assert boto_client_sqs.delete_message.call_args == mock.call(
             QueueUrl=await provider.get_queue_url("queue-name"),
             ReceiptHandle="message-receipt-handle-not-found",
         )
 
 
 @pytest.mark.asyncio
 async def test_confirm_message_unknown_error(mock_boto_session_sqs, boto_client_sqs):
-    error = ClientError(
-        error_response={"ResponseMetadata": {"HTTPStatusCode": 400}}, operation_name="whatever"
-    )
+    error = ClientError(error_response={"ResponseMetadata": {"HTTPStatusCode": 400}}, operation_name="whatever")
     boto_client_sqs.delete_message.side_effect = error
     with mock_boto_session_sqs:
         provider = SQSProvider("queue-name")
         message = {"ReceiptHandle": "message-receipt-handle-not-found"}
         with pytest.raises(ClientError):
             await provider.confirm_message(message)
 
@@ -126,50 +122,48 @@
 
 @pytest.mark.asyncio
 async def test_backoff_factor_options(mock_boto_session_sqs, boto_client_sqs):
     options = {"WaitTimeSeconds": 5, "MaxNumberOfMessages": 10, "BackoffFactor": 1.5}
     with mock_boto_session_sqs:
         provider = SQSProvider("queue-name", options=options)
 
-        assert provider._backoff_factor == 1.5
+        assert provider._backoff_factor == 1.5  # noqa: SLF001
 
         await provider.fetch_messages()
 
         _, receive_message_kwargs = boto_client_sqs.receive_message.call_args
 
         assert "BackoffFactor" not in receive_message_kwargs
         assert "AttributeNames" in receive_message_kwargs
         assert "ApproximateReceiveCount" in receive_message_kwargs["AttributeNames"]
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
-    "options, expected",
+    ("options", "expected"),
     [
         ({}, ["ApproximateReceiveCount"]),
         ({"AttributeNames": []}, ["ApproximateReceiveCount"]),
         ({"AttributeNames": ["CreatedTimestamp"]}, ["ApproximateReceiveCount", "CreatedTimestamp"]),
         ({"AttributeNames": ["All"]}, ["All"]),
     ],
 )
-async def test_backoff_factor_options_with_attributes_names(
-    mock_boto_session_sqs, boto_client_sqs, options, expected
-):
+async def test_backoff_factor_options_with_attributes_names(mock_boto_session_sqs, boto_client_sqs, options, expected):
     with mock_boto_session_sqs:
         provider = SQSProvider("queue-name", options={"BackoffFactor": 1.5, **options})
         await provider.fetch_messages()
 
     _, receive_message_kwargs = boto_client_sqs.receive_message.call_args
     assert set(receive_message_kwargs["AttributeNames"]) == set(expected)
     assert len(receive_message_kwargs["AttributeNames"]) == len(expected)
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
-    "visibility, backoff_multiplier, expected",
+    ("visibility", "backoff_multiplier", "expected"),
     [
         (30, 1.5, 45),
         (30, 1.75, 52),
         (60, 1.5, 90),
     ],
 )
 async def test_fetch_messages_using_backoff_factor(
@@ -198,20 +192,18 @@
             ReceiptHandle="message-receipt-handle",
             VisibilityTimeout=expected,
         )
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
-    "error,expectation",
+    ("error", "expectation"),
     [
         (
-            ClientError(
-                error_response={"Error": {"Code": "InvalidParameterValue"}}, operation_name="whatever"
-            ),
+            ClientError(error_response={"Error": {"Code": "InvalidParameterValue"}}, operation_name="whatever"),
             does_not_raise(),
         ),
         (
             ClientError(error_response={"Error": {"Code": "Other"}}, operation_name="whatever"),
             pytest.raises(ClientError),
         ),
     ],
```

### Comparing `olist_loafer-6.0.0a2/tests/ext/aws/test_routes.py` & `olist_loafer-6.0.0a3/tests/ext/aws/test_routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 def test_sqs_route_keep_name(dummy_handler):
     route = SQSRoute("what", handler=dummy_handler, name="foobar")
     assert route.name == "foobar"
 
 
 def test_sqs_route_provider_options(dummy_handler):
     route = SQSRoute("what", {"use_ssl": False}, handler=dummy_handler, name="foobar")
-    assert "use_ssl" in route.provider._client_options
-    assert route.provider._client_options["use_ssl"] is False
+    assert "use_ssl" in route.provider._client_options  # noqa: SLF001
+    assert route.provider._client_options["use_ssl"] is False  # noqa: SLF001
 
 
 def test_sns_queue_route(dummy_handler):
     route = SNSQueueRoute("what", handler=dummy_handler)
     assert isinstance(route.message_translator, SNSMessageTranslator)
     assert isinstance(route.provider, SQSProvider)
     assert route.name == "what"
@@ -44,12 +44,10 @@
 
 def test_sns_queue_route_keep_name(dummy_handler):
     route = SNSQueueRoute("what", handler=dummy_handler, name="foobar")
     assert route.name == "foobar"
 
 
 def test_sns_queue_route_provider_options(dummy_handler):
-    route = SNSQueueRoute(
-        "what", provider_options={"region_name": "sa-east-1"}, handler=dummy_handler, name="foobar"
-    )
-    assert "region_name" in route.provider._client_options
-    assert route.provider._client_options["region_name"] == "sa-east-1"
+    route = SNSQueueRoute("what", provider_options={"region_name": "sa-east-1"}, handler=dummy_handler, name="foobar")
+    assert "region_name" in route.provider._client_options  # noqa: SLF001
+    assert route.provider._client_options["region_name"] == "sa-east-1"  # noqa: SLF001
```

### Comparing `olist_loafer-6.0.0a2/.gitignore` & `olist_loafer-6.0.0a3/.gitignore`

 * *Files identical despite different names*

### Comparing `olist_loafer-6.0.0a2/LICENSE` & `olist_loafer-6.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `olist_loafer-6.0.0a2/README.md` & `olist_loafer-6.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `olist_loafer-6.0.0a2/PKG-INFO` & `olist_loafer-6.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: olist-loafer
-Version: 6.0.0a2
+Version: 6.0.0a3
 Summary: Asynchronous message dispatcher for concurrent tasks processing
 Project-URL: Download, https://github.com/olist/olist-loafer/releases
 Project-URL: Repository, https://github.com/olist/olist-loafer/
 Author-email: Olist <developers@olist.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 George Kussumoto
```

