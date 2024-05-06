# Comparing `tmp/pycrdt_websocket-0.13.2.tar.gz` & `tmp/pycrdt_websocket-0.13.3.tar.gz`

## Comparing `pycrdt_websocket-0.13.2.tar` & `pycrdt_websocket-0.13.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/pycrdt_websocket/__init__.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/pycrdt_websocket/asgi_server.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/pycrdt_websocket/awareness.py
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/pycrdt_websocket/django_channels_consumer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/pycrdt_websocket/py.typed
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/pycrdt_websocket/websocket.py
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/pycrdt_websocket/websocket_provider.py
--rw-r--r--   0        0        0     8412 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/pycrdt_websocket/websocket_server.py
--rw-r--r--   0        0        0    10700 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/pycrdt_websocket/yroom.py
--rw-r--r--   0        0        0    16368 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/pycrdt_websocket/ystore.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/pycrdt_websocket/yutils.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/tests/conftest.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/tests/package.json
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/tests/test_asgi.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/tests/test_pycrdt_yjs.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/tests/test_server.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/tests/test_yroom.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/tests/test_ystore.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/tests/utils.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/tests/yjs_client_0.js
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/tests/yjs_client_1.js
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/LICENSE
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/README.md
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/pyproject.toml
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.2/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/__init__.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/asgi_server.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/awareness.py
+-rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/django_channels_consumer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/py.typed
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/websocket.py
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/websocket_provider.py
+-rw-r--r--   0        0        0     8412 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/websocket_server.py
+-rw-r--r--   0        0        0    10700 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/yroom.py
+-rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/ystore.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pycrdt_websocket/yutils.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/conftest.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/package.json
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/test_asgi.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/test_pycrdt_yjs.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/test_server.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/test_yroom.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/test_ystore.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/utils.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/yjs_client_0.js
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/tests/yjs_client_1.js
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/LICENSE
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/README.md
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/pyproject.toml
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.3/PKG-INFO
```

### Comparing `pycrdt_websocket-0.13.2/pycrdt_websocket/asgi_server.py` & `pycrdt_websocket-0.13.3/pycrdt_websocket/asgi_server.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/pycrdt_websocket/awareness.py` & `pycrdt_websocket-0.13.3/pycrdt_websocket/awareness.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/pycrdt_websocket/django_channels_consumer.py` & `pycrdt_websocket-0.13.3/pycrdt_websocket/django_channels_consumer.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/pycrdt_websocket/websocket.py` & `pycrdt_websocket-0.13.3/pycrdt_websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/pycrdt_websocket/websocket_provider.py` & `pycrdt_websocket-0.13.3/pycrdt_websocket/websocket_provider.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/pycrdt_websocket/websocket_server.py` & `pycrdt_websocket-0.13.3/pycrdt_websocket/websocket_server.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/pycrdt_websocket/yroom.py` & `pycrdt_websocket-0.13.3/pycrdt_websocket/yroom.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/pycrdt_websocket/ystore.py` & `pycrdt_websocket-0.13.3/pycrdt_websocket/ystore.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     pass
 
 
 class BaseYStore(ABC):
     metadata_callback: Callable[[], Awaitable[bytes] | bytes] | None = None
     version = 2
     _started: Event | None = None
+    _stopped: Event | None = None
     _task_group: TaskGroup | None = None
     __start_lock: Lock | None = None
 
     @abstractmethod
     def __init__(
         self, path: str, metadata_callback: Callable[[], Awaitable[bytes] | bytes] | None = None
     ): ...
@@ -47,14 +48,20 @@
     @property
     def started(self) -> Event:
         if self._started is None:
             self._started = Event()
         return self._started
 
     @property
+    def stopped(self) -> Event:
+        if self._stopped is None:
+            self._stopped = Event()
+        return self._stopped
+
+    @property
     def _start_lock(self) -> Lock:
         if self.__start_lock is None:
             self.__start_lock = Lock()
         return self.__start_lock
 
     async def __aenter__(self) -> BaseYStore:
         async with self._start_lock:
@@ -92,20 +99,22 @@
         async with self._start_lock:
             if self._task_group is not None:
                 raise RuntimeError("YStore already running")
 
             async with create_task_group() as self._task_group:
                 task_status.started()
                 self.started.set()
+                await self.stopped.wait()
 
     async def stop(self) -> None:
         """Stop the store."""
         if self._task_group is None:
             raise RuntimeError("YStore not running")
 
+        self.stopped.set()
         self._task_group.cancel_scope.cancel()
         self._task_group = None
 
     async def get_metadata(self) -> bytes:
         """
         Returns:
             The metadata.
@@ -305,15 +314,15 @@
     db_path: str = "ystore.db"
     # Determines the "time to live" for all documents, i.e. how recent the
     # latest update of a document must be before purging document history.
     # Defaults to never purging document history (None).
     document_ttl: int | None = None
     path: str
     lock: Lock
-    db_initialized: Event
+    db_initialized: Event | None
     _db: Connection
 
     def __init__(
         self,
         path: str,
         metadata_callback: Callable[[], Awaitable[bytes] | bytes] | None = None,
         log: Logger | None = None,
@@ -325,14 +334,15 @@
             metadata_callback: An optional callback to call to get the metadata.
             log: An optional logger.
         """
         self.path = path
         self.metadata_callback = metadata_callback
         self.log = log or getLogger(__name__)
         self.lock = Lock()
+        self.db_initialized = None
 
     async def start(
         self,
         *,
         task_status: TaskStatus[None] = TASK_STATUS_IGNORED,
         from_context_manager: bool = False,
     ):
@@ -352,18 +362,19 @@
         async with self._start_lock:
             if self._task_group is not None:
                 raise RuntimeError("YStore already running")
             async with create_task_group() as self._task_group:
                 self._task_group.start_soon(self._init_db)
                 task_status.started()
                 self.started.set()
+                await self.stopped.wait()
 
     async def stop(self) -> None:
         """Stop the store."""
-        if hasattr(self, "db_initialized") and self.db_initialized.is_set():
+        if self.db_initialized is not None and self.db_initialized.is_set():
             await self._db.close()
         await super().stop()
 
     async def _init_db(self):
         create_db = False
         move_db = False
         if not await anyio.Path(self.db_path).exists():
@@ -401,24 +412,25 @@
                 await cursor.execute(
                     "CREATE INDEX idx_yupdates_path_timestamp ON yupdates (path, timestamp)"
                 )
                 await cursor.execute(f"PRAGMA user_version = {self.version}")
                 await db.commit()
                 await db.close()
         self._db = await connect(self.db_path)
+        assert self.db_initialized is not None
         self.db_initialized.set()
 
     async def read(self) -> AsyncIterator[tuple[bytes, bytes, float]]:
         """Async iterator for reading the store content.
 
         Returns:
             A tuple of (update, metadata, timestamp) for each update.
         """
-        if not hasattr(self, "db_initialized"):
-            raise RuntimeError("ystore is not started")
+        if self.db_initialized is None:
+            raise RuntimeError("YStore not started")
         await self.db_initialized.wait()
         try:
             async with self.lock:
                 cursor = await self._db.cursor()
                 await cursor.execute(
                     "SELECT yupdate, metadata, timestamp FROM yupdates WHERE path = ?",
                     (self.path,),
@@ -434,16 +446,16 @@
 
     async def write(self, data: bytes) -> None:
         """Store an update.
 
         Arguments:
             data: The update to store.
         """
-        if not hasattr(self, "db_initialized"):
-            raise RuntimeError("ystore is not started")
+        if self.db_initialized is None:
+            raise RuntimeError("YStore not started")
         await self.db_initialized.wait()
         async with self.lock:
             # first, determine time elapsed since last update
             cursor = await self._db.cursor()
             await cursor.execute(
                 "SELECT timestamp FROM yupdates WHERE path = ? ORDER BY timestamp DESC LIMIT 1",
                 (self.path,),
```

### Comparing `pycrdt_websocket-0.13.2/pycrdt_websocket/yutils.py` & `pycrdt_websocket-0.13.3/pycrdt_websocket/yutils.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/tests/conftest.py` & `pycrdt_websocket-0.13.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/tests/test_asgi.py` & `pycrdt_websocket-0.13.3/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/tests/test_pycrdt_yjs.py` & `pycrdt_websocket-0.13.3/tests/test_pycrdt_yjs.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/tests/test_server.py` & `pycrdt_websocket-0.13.3/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/tests/test_yroom.py` & `pycrdt_websocket-0.13.3/tests/test_yroom.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/tests/test_ystore.py` & `pycrdt_websocket-0.13.3/tests/test_ystore.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/tests/utils.py` & `pycrdt_websocket-0.13.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/tests/yjs_client_0.js` & `pycrdt_websocket-0.13.3/tests/yjs_client_0.js`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/tests/yjs_client_1.js` & `pycrdt_websocket-0.13.3/tests/yjs_client_1.js`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/.gitignore` & `pycrdt_websocket-0.13.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/LICENSE` & `pycrdt_websocket-0.13.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/README.md` & `pycrdt_websocket-0.13.3/README.md`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/pyproject.toml` & `pycrdt_websocket-0.13.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.2/PKG-INFO` & `pycrdt_websocket-0.13.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pycrdt-websocket
-Version: 0.13.2
+Version: 0.13.3
 Summary: WebSocket connector for pycrdt
 Project-URL: Homepage, https://github.com/jupyter-server/pycrdt-websocket
 Project-URL: Source, https://github.com/jupyter-server/pycrdt-websocket
 Project-URL: Issues, https://github.com/jupyter-server/pycrdt-websocket/issues
 Project-URL: Pypi, https://pypi.org/project/pycrdt-websocket
 Author-email: David Brochart <david.brochart@gmail.com>
 License: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: pycrdt-websocket Version: 0.13.2 Summary: WebSocket
+Metadata-Version: 2.3 Name: pycrdt-websocket Version: 0.13.3 Summary: WebSocket
 connector for pycrdt Project-URL: Homepage, https://github.com/jupyter-server/
 pycrdt-websocket Project-URL: Source, https://github.com/jupyter-server/pycrdt-
 websocket Project-URL: Issues, https://github.com/jupyter-server/pycrdt-
 websocket/issues Project-URL: Pypi, https://pypi.org/project/pycrdt-websocket
 Author-email: David Brochart
 gmail.com> License: MIT License Copyright (c) 2022 David Brochart Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
```

