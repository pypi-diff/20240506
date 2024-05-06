# Comparing `tmp/androidtvremote2-0.0.9.tar.gz` & `tmp/androidtvremote2-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "androidtvremote2-0.0.9.tar", last modified: Sat May 27 00:09:13 2023, max compression
+gzip compressed data, was "androidtvremote2-0.1.0.tar", last modified: Mon May  6 07:37:05 2024, max compression
```

## Comparing `androidtvremote2-0.0.9.tar` & `androidtvremote2-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:09:13.197309 androidtvremote2-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-27 00:09:13.197309 androidtvremote2-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-27 00:09:13.197309 androidtvremote2-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:09:13.193309 androidtvremote2-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:09:13.193309 androidtvremote2-0.0.9/src/androidtvremote2/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/androidtv_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/certificate_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/pairing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/polo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    19528 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/androidtvremote2/remotemessage_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:09:13.197309 androidtvremote2-0.0.9/src/androidtvremote2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-27 00:09:13.000000 androidtvremote2-0.0.9/src/androidtvremote2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-27 00:09:13.000000 androidtvremote2-0.0.9/src/androidtvremote2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 00:09:13.000000 androidtvremote2-0.0.9/src/androidtvremote2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-27 00:09:13.000000 androidtvremote2-0.0.9/src/androidtvremote2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 00:09:13.000000 androidtvremote2-0.0.9/src/androidtvremote2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/src/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 00:09:13.197309 androidtvremote2-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-27 00:08:54.000000 androidtvremote2-0.0.9/tests/test_androidtv_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:37:05.812653 androidtvremote2-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 07:37:01.000000 androidtvremote2-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-06 07:37:05.812653 androidtvremote2-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-06 07:37:01.000000 androidtvremote2-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-06 07:37:01.000000 androidtvremote2-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-06 07:37:05.812653 androidtvremote2-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:37:05.808653 androidtvremote2-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:37:05.808653 androidtvremote2-0.1.0/src/androidtvremote2/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-06 07:37:01.000000 androidtvremote2-0.1.0/src/androidtvremote2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17048 2024-05-06 07:37:01.000000 androidtvremote2-0.1.0/src/androidtvremote2/androidtv_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-06 07:37:01.000000 androidtvremote2-0.1.0/src/androidtvremote2/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-06 07:37:01.000000 androidtvremote2-0.1.0/src/androidtvremote2/certificate_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-06 07:37:01.000000 androidtvremote2-0.1.0/src/androidtvremote2/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-06 07:37:01.000000 androidtvremote2-0.1.0/src/androidtvremote2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-06 07:37:01.000000 androidtvremote2-0.1.0/src/androidtvremote2/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-06 07:37:01.000000 androidtvremote2-0.1.0/src/androidtvremote2/polo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12537 2024-05-06 07:37:01.000000 androidtvremote2-0.1.0/src/androidtvremote2/polo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8599 2024-05-06 07:37:01.000000 androidtvremote2-0.1.0/src/androidtvremote2/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20147 2024-05-06 07:37:01.000000 androidtvremote2-0.1.0/src/androidtvremote2/remotemessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86069 2024-05-06 07:37:01.000000 androidtvremote2-0.1.0/src/androidtvremote2/remotemessage_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:37:05.812653 androidtvremote2-0.1.0/src/androidtvremote2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-06 07:37:05.000000 androidtvremote2-0.1.0/src/androidtvremote2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-06 07:37:05.000000 androidtvremote2-0.1.0/src/androidtvremote2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 07:37:05.000000 androidtvremote2-0.1.0/src/androidtvremote2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 07:37:05.000000 androidtvremote2-0.1.0/src/androidtvremote2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 07:37:05.000000 androidtvremote2-0.1.0/src/androidtvremote2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-05-06 07:37:01.000000 androidtvremote2-0.1.0/src/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:37:05.808653 androidtvremote2-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-06 07:37:01.000000 androidtvremote2-0.1.0/tests/test_androidtv_remote.py
```

### Comparing `androidtvremote2-0.0.9/LICENSE` & `androidtvremote2-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `androidtvremote2-0.0.9/pyproject.toml` & `androidtvremote2-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "androidtvremote2"
-version = "0.0.9"
+version = "0.1.0"
 license = {text = "Apache-2.0"}
 authors = [
     { name="tronikos", email="tronikos@gmail.com" },
 ]
 description = "A Python library for interacting with Android TV using the Android TV Remote protocol v2"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 dependencies = [
     "aiofiles>=0.8",
     "cryptography>=3",
     "protobuf>=4.21",
 ]
 
 [project.urls]
```

### Comparing `androidtvremote2-0.0.9/src/androidtvremote2/androidtv_remote.py` & `androidtvremote2-0.1.0/src/androidtvremote2/androidtv_remote.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,55 +26,59 @@
         client_name: str,
         certfile: str,
         keyfile: str,
         host: str,
         api_port: int = 6466,
         pair_port: int = 6467,
         loop: asyncio.AbstractEventLoop | None = None,
+        enable_ime: bool = True,
     ) -> None:
         """Initialize.
 
         :param client_name: client name. Will be shown on the Android TV during pairing.
         :param certfile: filename that contains the client certificate in PEM format.
         :param keyfile: filename that contains the public key in PEM format.
         :param host: IP address of the Android TV.
         :param api_port: port for connecting and sending commands.
         :param pair_port: port for pairing.
         :param loop: event loop. Used for connections and futures.
+        :param enable_ime: Needed for getting current_app.
+               Disable for devices that show 'Use keyboard on mobile device screen'.
         """
         self._client_name = client_name
         self._certfile = certfile
         self._keyfile = keyfile
         self.host = host
         self._api_port = api_port
         self._pair_port = pair_port
         self._loop = loop or asyncio.get_running_loop()
-        self._transport = None
+        self._enable_ime = enable_ime
+        self._transport: asyncio.Transport | None = None
         self._remote_message_protocol: RemoteProtocol | None = None
         self._pairing_message_protocol: PairingProtocol | None = None
         self._reconnect_task: asyncio.Task | None = None
         self._ssl_context: ssl.SSLContext | None = None
         self._is_on_updated_callbacks: list[Callable] = []
         self._current_app_updated_callbacks: list[Callable] = []
         self._volume_info_updated_callbacks: list[Callable] = []
         self._is_available_updated_callbacks: list[Callable] = []
 
-        def is_on_updated(is_on: bool):
+        def is_on_updated(is_on: bool) -> None:
             for callback in self._is_on_updated_callbacks:
                 callback(is_on)
 
-        def current_app_updated(current_app: str):
+        def current_app_updated(current_app: str) -> None:
             for callback in self._current_app_updated_callbacks:
                 callback(current_app)
 
-        def volume_info_updated(volume_info: dict[str, str | bool]):
+        def volume_info_updated(volume_info: dict[str, str | bool]) -> None:
             for callback in self._volume_info_updated_callbacks:
                 callback(volume_info)
 
-        def is_available_updated(is_available: bool):
+        def is_available_updated(is_available: bool) -> None:
             for callback in self._is_available_updated_callbacks:
                 callback(is_available)
 
         self._on_is_on_updated = is_on_updated
         self._on_current_app_updated = current_app_updated
         self._on_volume_info_updated = volume_info_updated
         self._on_is_available_updated = is_available_updated
@@ -97,15 +101,15 @@
     def device_info(self) -> dict[str, str] | None:
         """Device info (manufacturer, model, sw_version)."""
         if not self._remote_message_protocol:
             return None
         return self._remote_message_protocol.device_info
 
     @property
-    def volume_info(self) -> dict[str, str | bool] | None:
+    def volume_info(self) -> dict[str, str | bool | int] | None:
         """Volume info (level, max, muted)."""
         if not self._remote_message_protocol:
             return None
         return self._remote_message_protocol.volume_info
 
     def add_is_on_updated_callback(self, callback: Callable) -> None:
         """Add a callback for when is_on is updated."""
@@ -161,51 +165,63 @@
         cert_pem, key_pem = generate_selfsigned_cert(self._client_name)
         async with aiofiles.open(self._certfile, "w", encoding="utf-8") as out:
             await out.write(cert_pem.decode("utf-8"))
         async with aiofiles.open(self._keyfile, "w", encoding="utf-8") as out:
             await out.write(key_pem.decode("utf-8"))
         return True
 
-    async def async_connect(self):
+    def _create_ssl_context(self) -> ssl.SSLContext:
+        if self._ssl_context:
+            return self._ssl_context
+        ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+        ssl_context.check_hostname = False
+        ssl_context.verify_mode = ssl.VerifyMode.CERT_NONE
+        try:
+            ssl_context.load_cert_chain(self._certfile, self._keyfile)
+        except FileNotFoundError as exc:
+            LOGGER.debug("Missing certificate. Error: %s", exc)
+            raise InvalidAuth from exc
+        ssl_context.load_cert_chain(self._certfile, self._keyfile)
+        self._ssl_context = ssl_context
+        return self._ssl_context
+
+    async def async_connect(self) -> None:
         """Connect to an Android TV.
 
         :raises CannotConnect: if couldn't connect, e.g. invalid IP address.
         :raises ConnectionClosed: if connection was lost while waiting for the remote to start.
         :raises InvalidAuth: if pairing is needed first.
         """
-        if self._ssl_context is None:
-            self._ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS)
-            try:
-                self._ssl_context.load_cert_chain(self._certfile, self._keyfile)
-            except FileNotFoundError as exc:
-                LOGGER.debug("Missing certificate. Error: %s", exc)
-                raise InvalidAuth from exc
+        ssl_context = self._create_ssl_context()
         on_con_lost = self._loop.create_future()
         on_remote_started = self._loop.create_future()
         try:
             (
                 self._transport,
                 self._remote_message_protocol,
             ) = await self._loop.create_connection(
                 lambda: RemoteProtocol(
                     on_con_lost,
                     on_remote_started,
                     self._on_is_on_updated,
                     self._on_current_app_updated,
                     self._on_volume_info_updated,
                     self._loop,
+                    self._enable_ime,
                 ),
                 self.host,
                 self._api_port,
-                ssl=self._ssl_context,
+                ssl=ssl_context,
             )
         except OSError as exc:
             LOGGER.debug(
                 "Couldn't connect to %s:%s. Error: %s", self.host, self._api_port, exc
             )
+            if isinstance(exc, ssl.SSLError):
+                raise InvalidAuth("Need to pair") from exc
             raise CannotConnect(
                 f"Couldn't connect to {self.host}:{self._api_port}"
             ) from exc
 
         await asyncio.wait(
             (on_con_lost, on_remote_started), return_when=asyncio.FIRST_COMPLETED
         )
@@ -234,15 +250,15 @@
             )
             while self._remote_message_protocol:
                 await asyncio.sleep(delay_seconds)
                 try:
                     await self.async_connect()
                     self._on_is_available_updated(True)
                     break
-                except CannotConnect as exc:
+                except (CannotConnect, ConnectionClosed) as exc:
                     delay_seconds = min(2 * delay_seconds, 30)
                     LOGGER.debug(
                         "Couldn't reconnect to %s. Will retry in %s seconds. Error: %s",
                         self.host,
                         delay_seconds,
                         exc,
                     )
@@ -276,47 +292,51 @@
             self._pairing_message_protocol = None
 
     async def async_get_name_and_mac(self) -> tuple[str, str]:
         """Connect to the Android TV and get its name and MAC address from its certificate.
 
         :raises CannotConnect: if couldn't connect, e.g. invalid IP address.
         """
-        ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS)
+        ssl_context = self._create_ssl_context()
         try:
             _, writer = await asyncio.open_connection(
-                self.host, self._api_port, ssl=ssl_context
+                self.host, self._pair_port, ssl=ssl_context
             )
         except OSError as exc:
             LOGGER.debug(
-                "Couldn't connect to %s:%s. %s", self.host, self._api_port, exc
+                "Couldn't connect to %s:%s. %s", self.host, self._pair_port, exc
             )
             raise CannotConnect from exc
         server_cert_bytes = writer.transport.get_extra_info("ssl_object").getpeercert(
             True
         )
         writer.close()
         server_cert = x509.load_der_x509_certificate(server_cert_bytes)
-        server_cert_common_name = str(
-            server_cert.subject.get_attributes_for_oid(x509.oid.NameOID.COMMON_NAME)[
-                0
-            ].value
-        )
-        # Example: atvremote/darcy/darcy/SHIELD Android TV/XX:XX:XX:XX:XX:XX
-        parts = server_cert_common_name.split("/")
-        return parts[-2], parts[-1]
+        # NVIDIA SHIELD example:
+        # CN=atvremote/darcy/darcy/SHIELD Android TV/XX:XX:XX:XX:XX:XX
+        # Nexus Player example:
+        # dnQualifier=fugu/fugu/Nexus Player/CN=atvremote/XX:XX:XX:XX:XX:XX
+        common_name = server_cert.subject.get_attributes_for_oid(x509.OID_COMMON_NAME)
+        common_name_str = str(common_name[0].value) if common_name else ""
+        dn_qualifier = server_cert.subject.get_attributes_for_oid(x509.OID_DN_QUALIFIER)
+        dn_qualifier_str = str(dn_qualifier[0].value) if dn_qualifier else ""
+        common_name_parts = common_name_str.split("/")
+        dn_qualifier_parts = dn_qualifier_str.split("/")
+        name = dn_qualifier_parts[-1] if dn_qualifier_str else common_name_parts[-2]
+        mac = common_name_parts[-1]
+        return name, mac
 
-    async def async_start_pairing(self):
+    async def async_start_pairing(self) -> None:
         """Start the pairing process.
 
         :raises CannotConnect: if couldn't connect, e.g. invalid IP address.
         :raises ConnectionClosed: if connection was lost.
         """
         self.disconnect()
-        ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS)
-        ssl_context.load_cert_chain(self._certfile, self._keyfile)
+        ssl_context = self._create_ssl_context()
         on_con_lost = self._loop.create_future()
         try:
             (
                 _,
                 self._pairing_message_protocol,
             ) = await self._loop.create_connection(
                 lambda: PairingProtocol(
@@ -332,30 +352,30 @@
         except OSError as exc:
             LOGGER.debug(
                 "Couldn't connect to %s:%s. %s", self.host, self._pair_port, exc
             )
             raise CannotConnect from exc
         await self._pairing_message_protocol.async_start_pairing()
 
-    async def async_finish_pairing(self, pairing_code: str):
+    async def async_finish_pairing(self, pairing_code: str) -> None:
         """Finish the pairing process.
 
         :param pairing_code: pairing code shown on the Android TV.
         :raises ConnectionClosed: if connection was lost, e.g. user pressed cancel on the Android TV.
         :raises InvalidAuth: if pairing was unsuccessful.
         """
         if not self._pairing_message_protocol:
             LOGGER.debug("Called async_finish_pairing after disconnect")
             raise ConnectionClosed("Called async_finish_pairing after disconnect")
         await self._pairing_message_protocol.async_finish_pairing(pairing_code)
         self.disconnect()
 
     def send_key_command(
         self, key_code: int | str, direction: int | str = RemoteDirection.SHORT
-    ):
+    ) -> None:
         """Send a key press to Android TV.
 
         This does not block; it buffers the data and arranges for it to be sent out asynchronously.
 
         :param key_code: int (e.g. 26) or str (e.g. "KEYCODE_POWER" or just "POWER") from the enum
                          RemoteKeyCode in remotemessage.proto.
         :param direction: "SHORT" (default) or "START_LONG" or "END_LONG".
@@ -363,18 +383,21 @@
         :raises ConnectionClosed: if client is disconnected.
         """
         if not self._remote_message_protocol:
             LOGGER.debug("Called send_key_command after disconnect")
             raise ConnectionClosed("Called send_key_command after disconnect")
         self._remote_message_protocol.send_key_command(key_code, direction)
 
-    def send_launch_app_command(self, app_link: str):
+    def send_launch_app_command(self, app_link_or_app_id: str) -> None:
         """Launch an app on Android TV.
 
         This does not block; it buffers the data and arranges for it to be sent out asynchronously.
 
         :raises ConnectionClosed: if client is disconnected.
         """
         if not self._remote_message_protocol:
             LOGGER.debug("Called send_launch_app_command after disconnect")
             raise ConnectionClosed("Called send_launch_app_command after disconnect")
-        self._remote_message_protocol.send_launch_app_command(app_link)
+        prefix = "" if "://" in app_link_or_app_id else "market://launch?id="
+        self._remote_message_protocol.send_launch_app_command(
+            f"{prefix}{app_link_or_app_id}"
+        )
```

### Comparing `androidtvremote2-0.0.9/src/androidtvremote2/base.py` & `androidtvremote2-0.1.0/src/androidtvremote2/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from __future__ import annotations
 
 import asyncio
 from typing import cast
 
 from google.protobuf import text_format
-from google.protobuf.internal.decoder import _DecodeVarint
-from google.protobuf.internal.encoder import _EncodeVarint
+from google.protobuf.internal.decoder import _DecodeVarint  # type: ignore[attr-defined]
+from google.protobuf.internal.encoder import _EncodeVarint  # type: ignore[attr-defined]
 from google.protobuf.message import Message
 
 from .const import LOGGER
 
 
 class ProtobufProtocol(asyncio.Protocol):
     """Protocol for receiving and sending protobuf messages."""
```

### Comparing `androidtvremote2-0.0.9/src/androidtvremote2/certificate_generator.py` & `androidtvremote2-0.1.0/src/androidtvremote2/certificate_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,38 +11,38 @@
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
 from cryptography.x509.oid import NameOID
 
 
-def generate_selfsigned_cert(hostname: str):
+def generate_selfsigned_cert(hostname: str) -> tuple[bytes, bytes]:
     """Generate self signed certificate for a hostname.
 
     :return: self signed certificate and public key in PEM format
     """
     key = rsa.generate_private_key(
         public_exponent=65537,
         key_size=2048,
         backend=default_backend(),
     )
     name = x509.Name([x509.NameAttribute(NameOID.COMMON_NAME, hostname)])
     alt_names = [x509.DNSName(hostname)]
     san = x509.SubjectAlternativeName(alt_names)
-    basic_contraints = x509.BasicConstraints(ca=True, path_length=0)
+    basic_constraints = x509.BasicConstraints(ca=True, path_length=0)
     now = datetime.utcnow()
     cert = (
         x509.CertificateBuilder()
         .subject_name(name)
         .issuer_name(name)
         .public_key(key.public_key())
         .serial_number(1000)
         .not_valid_before(now)
         .not_valid_after(now + timedelta(days=10 * 365))
-        .add_extension(basic_contraints, False)
+        .add_extension(basic_constraints, False)
         .add_extension(san, False)
         .sign(key, hashes.SHA256(), default_backend())
     )
     cert_pem = cert.public_bytes(encoding=serialization.Encoding.PEM)
     key_pem = key.private_bytes(
         encoding=serialization.Encoding.PEM,
         format=serialization.PrivateFormat.TraditionalOpenSSL,
```

### Comparing `androidtvremote2-0.0.9/src/androidtvremote2/pairing.py` & `androidtvremote2-0.1.0/src/androidtvremote2/pairing.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 
 from .base import ProtobufProtocol
 from .const import LOGGER
 from .exceptions import ConnectionClosed, InvalidAuth
 from .polo_pb2 import Options, OuterMessage
 
 
-def _create_message():
+def _create_message() -> OuterMessage:
     """Create an OuterMessage with default values."""
     msg = OuterMessage()
     msg.protocol_version = 2
     msg.status = OuterMessage.Status.STATUS_OK
     return msg
 
 
-def _get_modulus_and_exponent(cert):
+def _get_modulus_and_exponent(cert: x509.Certificate) -> tuple[int, int]:
     """Extract modulus and exponent from a certificate."""
-    public_numbers = cert.public_key().public_numbers()
-    return public_numbers.n, public_numbers.e
+    public_numbers = cert.public_key().public_numbers()  # type: ignore[union-attr]
+    return public_numbers.n, public_numbers.e  # type: ignore[union-attr]
 
 
 class PairingProtocol(ProtobufProtocol):
     """Implement pairing protocol with an Android TV.
 
     Messages transmitted between client and server are of type OuterMessage, see polo.proto.
     Protocol is described in
@@ -61,15 +61,15 @@
         super().__init__(on_con_lost)
         self._client_name = client_name
         self._certfile = certfile
         self._loop = loop
         self._on_pairing_started: asyncio.Future | None = None
         self._on_pairing_finished: asyncio.Future | None = None
 
-    async def async_start_pairing(self):
+    async def async_start_pairing(self) -> None:
         """Start the pairing process.
 
         :raises ConnectionClosed: if connection was lost.
         """
         self._raise_if_not_connected()
         msg = _create_message()
         msg.pairing_request.client_name = self._client_name
@@ -77,15 +77,15 @@
         self._on_pairing_started = self._loop.create_future()
         self._send_message(msg)
         try:
             await self._async_wait_for_future_or_con_lost(self._on_pairing_started)
         finally:
             self._on_pairing_started = None
 
-    async def async_finish_pairing(self, pairing_code: str):
+    async def async_finish_pairing(self, pairing_code: str) -> None:
         """Finish the pairing process.
 
         :param pairing_code: pairing code shown on the Android TV.
         :raises ConnectionClosed: if connection was lost.
         :raises InvalidAuth: if pairing was unsuccessful.
         """
         self._raise_if_not_connected()
@@ -126,33 +126,33 @@
         self._on_pairing_finished = self._loop.create_future()
         self._send_message(msg)
         try:
             await self._async_wait_for_future_or_con_lost(self._on_pairing_finished)
         finally:
             self._on_pairing_finished = None
 
-    async def _async_wait_for_future_or_con_lost(self, future: asyncio.Future):
+    async def _async_wait_for_future_or_con_lost(self, future: asyncio.Future) -> None:
         """Wait for future to finish or connection to be lost."""
         await asyncio.wait(
             (self.on_con_lost, future), return_when=asyncio.FIRST_COMPLETED
         )
         if future.done():
             if future.exception():
                 raise ConnectionClosed(future.exception())
             if future.result():
                 return
         self._raise_if_not_connected()
 
-    def _raise_if_not_connected(self):
+    def _raise_if_not_connected(self) -> None:
         """Raise ConnectionClosed if not connected."""
         if self.transport is None or self.transport.is_closing():
             LOGGER.debug("Connection has been lost, cannot pair")
             raise ConnectionClosed("Connection has been lost")
 
-    def _handle_message(self, raw_msg: bytes):
+    def _handle_message(self, raw_msg: bytes) -> None:
         """Handle a message from the server."""
         msg = OuterMessage()
         try:
             msg.ParseFromString(raw_msg)
         except DecodeError as exc:
             LOGGER.debug("Couldn't parse as OuterMessage. %s", exc)
             self._handle_error(exc)
@@ -198,14 +198,15 @@
                     f"Unhandled msg: {text_format.MessageToString(msg, as_one_line=True)}"
                 )
             )
             return
 
         self._send_message(new_msg)
 
-    def _handle_error(self, exception):
+    def _handle_error(self, exception: Exception) -> None:
         """Handle errors during _handle_message."""
         if self._on_pairing_started and not self._on_pairing_started.done():
             self._on_pairing_started.set_exception(exception)
         if self._on_pairing_finished and not self._on_pairing_finished.done():
             self._on_pairing_finished.set_exception(exception)
-        self.transport.close()
+        if self.transport:
+            self.transport.close()
```

### Comparing `androidtvremote2-0.0.9/src/androidtvremote2/polo_pb2.py` & `androidtvremote2-0.1.0/src/androidtvremote2/polo_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: polo.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\npolo.proto\x12\x12polo.wire.protobuf\"\xd1\x04\n\x0cOuterMessage\x12\x1b\n\x10protocol_version\x18\x01 \x02(\r:\x01\x31\x12\x37\n\x06status\x18\x02 \x02(\x0e\x32\'.polo.wire.protobuf.OuterMessage.Status\x12;\n\x0fpairing_request\x18\n \x01(\x0b\x32\".polo.wire.protobuf.PairingRequest\x12\x42\n\x13pairing_request_ack\x18\x0b \x01(\x0b\x32%.polo.wire.protobuf.PairingRequestAck\x12,\n\x07options\x18\x14 \x01(\x0b\x32\x1b.polo.wire.protobuf.Options\x12\x38\n\rconfiguration\x18\x1e \x01(\x0b\x32!.polo.wire.protobuf.Configuration\x12?\n\x11\x63onfiguration_ack\x18\x1f \x01(\x0b\x32$.polo.wire.protobuf.ConfigurationAck\x12*\n\x06secret\x18( \x01(\x0b\x32\x1a.polo.wire.protobuf.Secret\x12\x31\n\nsecret_ack\x18) \x01(\x0b\x32\x1d.polo.wire.protobuf.SecretAck\"b\n\x06Status\x12\x0e\n\tSTATUS_OK\x10\xc8\x01\x12\x11\n\x0cSTATUS_ERROR\x10\x90\x03\x12\x1d\n\x18STATUS_BAD_CONFIGURATION\x10\x91\x03\x12\x16\n\x11STATUS_BAD_SECRET\x10\x92\x03\";\n\x0ePairingRequest\x12\x14\n\x0cservice_name\x18\x01 \x02(\t\x12\x13\n\x0b\x63lient_name\x18\x02 \x01(\t\"(\n\x11PairingRequestAck\x12\x13\n\x0bserver_name\x18\x01 \x01(\t\"\x99\x04\n\x07Options\x12=\n\x0finput_encodings\x18\x01 \x03(\x0b\x32$.polo.wire.protobuf.Options.Encoding\x12>\n\x10output_encodings\x18\x02 \x03(\x0b\x32$.polo.wire.protobuf.Options.Encoding\x12<\n\x0epreferred_role\x18\x03 \x01(\x0e\x32$.polo.wire.protobuf.Options.RoleType\x1a\x82\x02\n\x08\x45ncoding\x12?\n\x04type\x18\x01 \x02(\x0e\x32\x31.polo.wire.protobuf.Options.Encoding.EncodingType\x12\x15\n\rsymbol_length\x18\x02 \x02(\r\"\x9d\x01\n\x0c\x45ncodingType\x12\x19\n\x15\x45NCODING_TYPE_UNKNOWN\x10\x00\x12\x1e\n\x1a\x45NCODING_TYPE_ALPHANUMERIC\x10\x01\x12\x19\n\x15\x45NCODING_TYPE_NUMERIC\x10\x02\x12\x1d\n\x19\x45NCODING_TYPE_HEXADECIMAL\x10\x03\x12\x18\n\x14\x45NCODING_TYPE_QRCODE\x10\x04\"L\n\x08RoleType\x12\x15\n\x11ROLE_TYPE_UNKNOWN\x10\x00\x12\x13\n\x0fROLE_TYPE_INPUT\x10\x01\x12\x14\n\x10ROLE_TYPE_OUTPUT\x10\x02\"\x82\x01\n\rConfiguration\x12\x36\n\x08\x65ncoding\x18\x01 \x02(\x0b\x32$.polo.wire.protobuf.Options.Encoding\x12\x39\n\x0b\x63lient_role\x18\x02 \x02(\x0e\x32$.polo.wire.protobuf.Options.RoleType\"\x12\n\x10\x43onfigurationAck\"\x18\n\x06Secret\x12\x0e\n\x06secret\x18\x01 \x02(\x0c\"\x1b\n\tSecretAck\x12\x0e\n\x06secret\x18\x01 \x02(\x0c\x42,\n\x1d\x63om.google.polo.wire.protobufB\tPoloProtoH\x03')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'polo_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'polo_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\035com.google.polo.wire.protobufB\tPoloProtoH\003'
-  _OUTERMESSAGE._serialized_start=35
-  _OUTERMESSAGE._serialized_end=628
-  _OUTERMESSAGE_STATUS._serialized_start=530
-  _OUTERMESSAGE_STATUS._serialized_end=628
-  _PAIRINGREQUEST._serialized_start=630
-  _PAIRINGREQUEST._serialized_end=689
-  _PAIRINGREQUESTACK._serialized_start=691
-  _PAIRINGREQUESTACK._serialized_end=731
-  _OPTIONS._serialized_start=734
-  _OPTIONS._serialized_end=1271
-  _OPTIONS_ENCODING._serialized_start=935
-  _OPTIONS_ENCODING._serialized_end=1193
-  _OPTIONS_ENCODING_ENCODINGTYPE._serialized_start=1036
-  _OPTIONS_ENCODING_ENCODINGTYPE._serialized_end=1193
-  _OPTIONS_ROLETYPE._serialized_start=1195
-  _OPTIONS_ROLETYPE._serialized_end=1271
-  _CONFIGURATION._serialized_start=1274
-  _CONFIGURATION._serialized_end=1404
-  _CONFIGURATIONACK._serialized_start=1406
-  _CONFIGURATIONACK._serialized_end=1424
-  _SECRET._serialized_start=1426
-  _SECRET._serialized_end=1450
-  _SECRETACK._serialized_start=1452
-  _SECRETACK._serialized_end=1479
+  _globals['_OUTERMESSAGE']._serialized_start=35
+  _globals['_OUTERMESSAGE']._serialized_end=628
+  _globals['_OUTERMESSAGE_STATUS']._serialized_start=530
+  _globals['_OUTERMESSAGE_STATUS']._serialized_end=628
+  _globals['_PAIRINGREQUEST']._serialized_start=630
+  _globals['_PAIRINGREQUEST']._serialized_end=689
+  _globals['_PAIRINGREQUESTACK']._serialized_start=691
+  _globals['_PAIRINGREQUESTACK']._serialized_end=731
+  _globals['_OPTIONS']._serialized_start=734
+  _globals['_OPTIONS']._serialized_end=1271
+  _globals['_OPTIONS_ENCODING']._serialized_start=935
+  _globals['_OPTIONS_ENCODING']._serialized_end=1193
+  _globals['_OPTIONS_ENCODING_ENCODINGTYPE']._serialized_start=1036
+  _globals['_OPTIONS_ENCODING_ENCODINGTYPE']._serialized_end=1193
+  _globals['_OPTIONS_ROLETYPE']._serialized_start=1195
+  _globals['_OPTIONS_ROLETYPE']._serialized_end=1271
+  _globals['_CONFIGURATION']._serialized_start=1274
+  _globals['_CONFIGURATION']._serialized_end=1404
+  _globals['_CONFIGURATIONACK']._serialized_start=1406
+  _globals['_CONFIGURATIONACK']._serialized_end=1424
+  _globals['_SECRET']._serialized_start=1426
+  _globals['_SECRET']._serialized_end=1450
+  _globals['_SECRETACK']._serialized_start=1452
+  _globals['_SECRETACK']._serialized_end=1479
 # @@protoc_insertion_point(module_scope)
```

### Comparing `androidtvremote2-0.0.9/src/androidtvremote2/remote.py` & `androidtvremote2-0.1.0/src/androidtvremote2/remote.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,68 +4,95 @@
 # https://github.com/louis49/androidtv-remote/tree/main/src/remote
 # https://github.com/farshid616/Android-TV-Remote-Controller-Python/blob/main/sending_keys.py
 
 from __future__ import annotations
 
 import asyncio
 from collections.abc import Callable
+from enum import IntFlag
 
 from google.protobuf import text_format
 from google.protobuf.message import DecodeError
 
 from .base import ProtobufProtocol
 from .const import LOGGER
 from .remotemessage_pb2 import RemoteDirection, RemoteKeyCode, RemoteMessage
 
 LOG_PING_REQUESTS = False
+ERROR_SUGGESTION_MSG = (
+    "Try clearing the storage of the Android TV Remove Service system app. "
+    "On the Android TV device, go to Settings > Apps > See all apps > Show system apps. "
+    "Then, select Android TV Remote Service > Storage > Clear data/storage."
+)
+
+
+class Feature(IntFlag):
+    """Supported features."""
+
+    PING = 2**0
+    KEY = 2**1
+    IME = 2**2
+    POWER = 2**5
+    VOLUME = 2**6
+    APP_LINK = 2**9
 
 
 class RemoteProtocol(ProtobufProtocol):
     """Implement remote protocol with an Android TV.
 
-    Messages transmitted between client and server are of type RemoteMessage, see remotegmessage.proto.
+    Messages transmitted between client and server are of type RemoteMessage, see remotemessage.proto.
     Protocol is described in
     https://github.com/Aymkdn/assistant-freebox-cloud/wiki/Google-TV-(aka-Android-TV)-Remote-Control-(v2)
     """
 
     def __init__(
         self,
         on_con_lost: asyncio.Future,
         on_remote_started: asyncio.Future,
         on_is_on_updated: Callable,
         on_current_app_updated: Callable,
         on_volume_info_updated: Callable,
         loop: asyncio.AbstractEventLoop,
+        enable_ime: bool,
     ) -> None:
         """Initialize.
 
         :param on_con_lost: callback for when the connection is lost or closed.
         :param on_remote_started: callback for when the Android TV is ready to receive commands.
         :param on_is_on_updated: callback for when is_on is updated.
         :param on_current_app_updated: callback for when current_app is updated.
         :param on_volume_info_updated: callback for when volume_info is updated.
         :param loop: event loop.
+        :param enable_ime: Needed for getting current_app.
+               Disable for devices that show 'Use keyboard on mobile device screen'.
         """
         super().__init__(on_con_lost)
         self._on_remote_started = on_remote_started
         self._on_is_on_updated = on_is_on_updated
         self._on_current_app_updated = on_current_app_updated
         self._on_volume_info_updated = on_volume_info_updated
-        self._active_mask = 622
+        self._active_features = (
+            Feature.PING
+            | Feature.KEY
+            | Feature.POWER
+            | Feature.VOLUME
+            | Feature.APP_LINK
+            | (Feature.IME if enable_ime else 0)
+        )
         self.is_on = False
         self.current_app = ""
         self.device_info: dict[str, str] = {}
-        self.volume_info: dict[str, str | bool] = {}
+        self.volume_info: dict[str, str | bool | int] = {}
         self._loop = loop
         self._idle_disconnect_task: asyncio.Task | None = None
         self._reset_idle_disconnect_task()
 
     def send_key_command(
         self, key_code: int | str, direction: int | str = RemoteDirection.SHORT
-    ):
+    ) -> None:
         """Send a key press to Android TV.
 
         This does not block; it buffers the data and arranges for it to be sent out asynchronously.
 
         :param key_code: int (e.g. 26) or str (e.g. KEYCODE_POWER or just "POWER") from the enum
                          RemoteKeyCode in remotemessage.proto.
         :param direction: "SHORT" (default) or "START_LONG" or "END_LONG".
@@ -75,29 +102,29 @@
         msg = RemoteMessage()
         if isinstance(key_code, str):
             if not key_code.startswith("KEYCODE_"):
                 key_code = "KEYCODE_" + key_code
             key_code = RemoteKeyCode.Value(key_code)
         if isinstance(direction, str):
             direction = RemoteDirection.Value(direction)
-        msg.remote_key_inject.key_code = key_code
-        msg.remote_key_inject.direction = direction
+        msg.remote_key_inject.key_code = key_code  # type: ignore[assignment]
+        msg.remote_key_inject.direction = direction  # type: ignore[assignment]
         self._send_message(msg)
 
-    def send_launch_app_command(self, app_link: str):
+    def send_launch_app_command(self, app_link: str) -> None:
         """Launch an app on Android TV.
 
         This does not block; it buffers the data and arranges for it to be sent out asynchronously.
         """
         self._reset_idle_disconnect_task()
         msg = RemoteMessage()
         msg.remote_app_link_launch_request.app_link = app_link
         self._send_message(msg)
 
-    def _handle_message(self, raw_msg):
+    def _handle_message(self, raw_msg: bytes) -> None:
         """Handle a message from the server."""
         self._reset_idle_disconnect_task()
         msg = RemoteMessage()
         try:
             msg.ParseFromString(raw_msg)
         except DecodeError as exc:
             LOGGER.debug("Couldn't parse as RemoteMessage. %s", exc)
@@ -113,23 +140,32 @@
         if msg.HasField("remote_configure"):
             cfg = msg.remote_configure
             self.device_info = {
                 "manufacturer": cfg.device_info.vendor,
                 "model": cfg.device_info.model,
                 "sw_version": cfg.device_info.app_version,
             }
-            if cfg.code1:
-                self._active_mask = cfg.code1
-            new_msg.remote_configure.code1 = self._active_mask
+            supported_features = Feature(cfg.code1)
+            LOGGER.debug("Device supports: %s", [supported_features])
+            if Feature.KEY not in supported_features:
+                LOGGER.error(
+                    "Device doesn't support sending keys. %s", ERROR_SUGGESTION_MSG
+                )
+            if Feature.APP_LINK not in supported_features:
+                LOGGER.error(
+                    "Device doesn't support sending app links. %s", ERROR_SUGGESTION_MSG
+                )
+            self._active_features &= supported_features
+            new_msg.remote_configure.code1 = self._active_features.value
             new_msg.remote_configure.device_info.unknown1 = 1
             new_msg.remote_configure.device_info.unknown2 = "1"
             new_msg.remote_configure.device_info.package_name = "atvremote"
             new_msg.remote_configure.device_info.app_version = "1.0.0"
         elif msg.HasField("remote_set_active"):
-            new_msg.remote_set_active.active = self._active_mask
+            new_msg.remote_set_active.active = self._active_features
         elif msg.HasField("remote_ime_key_inject"):
             self.current_app = msg.remote_ime_key_inject.app_info.app_package
             self._on_current_app_updated(self.current_app)
         elif msg.HasField("remote_set_volume_level"):
             self.volume_info = {
                 "level": msg.remote_set_volume_level.volume_level,
                 "max": msg.remote_set_volume_level.volume_max,
@@ -148,24 +184,25 @@
             LOGGER.debug(
                 "Unhandled: %s", text_format.MessageToString(msg, as_one_line=True)
             )
 
         if new_msg != RemoteMessage():
             self._send_message(new_msg, log_send)
 
-    def _reset_idle_disconnect_task(self):
+    def _reset_idle_disconnect_task(self) -> None:
         if self._idle_disconnect_task is not None:
             self._idle_disconnect_task.cancel()
         self._idle_disconnect_task = self._loop.create_task(
             self._async_idle_disconnect()
         )
 
-    async def _async_idle_disconnect(self):
+    async def _async_idle_disconnect(self) -> None:
         # Disconnect if there is no message from the server or client within
         # 16 seconds. Server pings every 5 seconds if there is no command sent.
         # This is similar to the server behavior that closes connections after 3
         # unanswered pings.
         await asyncio.sleep(16)
         LOGGER.debug("Closing idle connection")
-        self.transport.close()
+        if self.transport and not self.transport.is_closing():
+            self.transport.close()
         if not self.on_con_lost.done():
             self.on_con_lost.set_result(Exception("Closed idle connection"))
```

### Comparing `androidtvremote2-0.0.9/src/androidtvremote2/remotemessage_pb2.py` & `androidtvremote2-0.1.0/src/androidtvremote2/remotemessage_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: remotemessage.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13remotemessage.proto\x12\x06remote\".\n\x1aRemoteAppLinkLaunchRequest\x12\x10\n\x08\x61pp_link\x18\x01 \x01(\t\"!\n\x1fRemoteResetPreferredAudioDevice\"\x1f\n\x1dRemoteSetPreferredAudioDevice\"\x19\n\x17RemoteAdjustVolumeLevel\"\xb4\x01\n\x14RemoteSetVolumeLevel\x12\x10\n\x08unknown1\x18\x01 \x01(\r\x12\x10\n\x08unknown2\x18\x02 \x01(\r\x12\x14\n\x0cplayer_model\x18\x03 \x01(\t\x12\x10\n\x08unknown4\x18\x04 \x01(\r\x12\x10\n\x08unknown5\x18\x05 \x01(\r\x12\x12\n\nvolume_max\x18\x06 \x01(\r\x12\x14\n\x0cvolume_level\x18\x07 \x01(\r\x12\x14\n\x0cvolume_muted\x18\x08 \x01(\x08\"\x1e\n\x0bRemoteStart\x12\x0f\n\x07started\x18\x01 \x01(\x08\"\x10\n\x0eRemoteVoiceEnd\"\x14\n\x12RemoteVoicePayload\"\x12\n\x10RemoteVoiceBegin\"v\n\x15RemoteTextFieldStatus\x12\x15\n\rcounter_field\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t\x12\r\n\x05start\x18\x03 \x01(\x05\x12\x0b\n\x03\x65nd\x18\x04 \x01(\x05\x12\x0c\n\x04int5\x18\x05 \x01(\x05\x12\r\n\x05label\x18\x06 \x01(\t\"W\n\x14RemoteImeShowRequest\x12?\n\x18remote_text_field_status\x18\x02 \x01(\x0b\x32\x1d.remote.RemoteTextFieldStatus\" \n\x0eRemoteEditInfo\x12\x0e\n\x06insert\x18\x02 \x01(\x05\"k\n\x12RemoteImeBatchEdit\x12\x13\n\x0bime_counter\x18\x01 \x01(\x05\x12\x15\n\rfield_counter\x18\x02 \x01(\x05\x12)\n\tedit_info\x18\x03 \x01(\x0b\x32\x16.remote.RemoteEditInfo\"\x99\x01\n\rRemoteAppInfo\x12\x0f\n\x07\x63ounter\x18\x01 \x01(\x05\x12\x0c\n\x04int2\x18\x02 \x01(\x05\x12\x0c\n\x04int3\x18\x03 \x01(\x05\x12\x0c\n\x04int4\x18\x04 \x01(\t\x12\x0c\n\x04int7\x18\x07 \x01(\x05\x12\x0c\n\x04int8\x18\x08 \x01(\x05\x12\r\n\x05label\x18\n \x01(\t\x12\x13\n\x0b\x61pp_package\x18\x0c \x01(\t\x12\r\n\x05int13\x18\r \x01(\x05\"w\n\x12RemoteImeKeyInject\x12\'\n\x08\x61pp_info\x18\x01 \x01(\x0b\x32\x15.remote.RemoteAppInfo\x12\x38\n\x11text_field_status\x18\x02 \x01(\x0b\x32\x1d.remote.RemoteTextFieldStatus\"f\n\x0fRemoteKeyInject\x12\'\n\x08key_code\x18\x01 \x01(\x0e\x32\x15.remote.RemoteKeyCode\x12*\n\tdirection\x18\x02 \x01(\x0e\x32\x17.remote.RemoteDirection\"\"\n\x12RemotePingResponse\x12\x0c\n\x04val1\x18\x01 \x01(\x05\"/\n\x11RemotePingRequest\x12\x0c\n\x04val1\x18\x01 \x01(\x05\x12\x0c\n\x04val2\x18\x02 \x01(\x05\"!\n\x0fRemoteSetActive\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\x05\"\x80\x01\n\x10RemoteDeviceInfo\x12\r\n\x05model\x18\x01 \x01(\t\x12\x0e\n\x06vendor\x18\x02 \x01(\t\x12\x10\n\x08unknown1\x18\x03 \x01(\x05\x12\x10\n\x08unknown2\x18\x04 \x01(\t\x12\x14\n\x0cpackage_name\x18\x05 \x01(\t\x12\x13\n\x0b\x61pp_version\x18\x06 \x01(\t\"O\n\x0fRemoteConfigure\x12\r\n\x05\x63ode1\x18\x01 \x01(\x05\x12-\n\x0b\x64\x65vice_info\x18\x02 \x01(\x0b\x32\x18.remote.RemoteDeviceInfo\"D\n\x0bRemoteError\x12\r\n\x05value\x18\x01 \x01(\x08\x12&\n\x07message\x18\x02 \x01(\x0b\x32\x15.remote.RemoteMessage\"\xc1\x08\n\rRemoteMessage\x12\x31\n\x10remote_configure\x18\x01 \x01(\x0b\x32\x17.remote.RemoteConfigure\x12\x32\n\x11remote_set_active\x18\x02 \x01(\x0b\x32\x17.remote.RemoteSetActive\x12)\n\x0cremote_error\x18\x03 \x01(\x0b\x32\x13.remote.RemoteError\x12\x36\n\x13remote_ping_request\x18\x08 \x01(\x0b\x32\x19.remote.RemotePingRequest\x12\x38\n\x14remote_ping_response\x18\t \x01(\x0b\x32\x1a.remote.RemotePingResponse\x12\x32\n\x11remote_key_inject\x18\n \x01(\x0b\x32\x17.remote.RemoteKeyInject\x12\x39\n\x15remote_ime_key_inject\x18\x14 \x01(\x0b\x32\x1a.remote.RemoteImeKeyInject\x12\x39\n\x15remote_ime_batch_edit\x18\x15 \x01(\x0b\x32\x1a.remote.RemoteImeBatchEdit\x12=\n\x17remote_ime_show_request\x18\x16 \x01(\x0b\x32\x1c.remote.RemoteImeShowRequest\x12\x34\n\x12remote_voice_begin\x18\x1e \x01(\x0b\x32\x18.remote.RemoteVoiceBegin\x12\x38\n\x14remote_voice_payload\x18\x1f \x01(\x0b\x32\x1a.remote.RemoteVoicePayload\x12\x30\n\x10remote_voice_end\x18  \x01(\x0b\x32\x16.remote.RemoteVoiceEnd\x12)\n\x0cremote_start\x18( \x01(\x0b\x32\x13.remote.RemoteStart\x12=\n\x17remote_set_volume_level\x18\x32 \x01(\x0b\x32\x1c.remote.RemoteSetVolumeLevel\x12\x43\n\x1aremote_adjust_volume_level\x18\x33 \x01(\x0b\x32\x1f.remote.RemoteAdjustVolumeLevel\x12P\n!remote_set_preferred_audio_device\x18< \x01(\x0b\x32%.remote.RemoteSetPreferredAudioDevice\x12T\n#remote_reset_preferred_audio_device\x18= \x01(\x0b\x32\'.remote.RemoteResetPreferredAudioDevice\x12J\n\x1eremote_app_link_launch_request\x18Z \x01(\x0b\x32\".remote.RemoteAppLinkLaunchRequest*\xe7\x37\n\rRemoteKeyCode\x12\x13\n\x0fKEYCODE_UNKNOWN\x10\x00\x12\x15\n\x11KEYCODE_SOFT_LEFT\x10\x01\x12\x16\n\x12KEYCODE_SOFT_RIGHT\x10\x02\x12\x10\n\x0cKEYCODE_HOME\x10\x03\x12\x10\n\x0cKEYCODE_BACK\x10\x04\x12\x10\n\x0cKEYCODE_CALL\x10\x05\x12\x13\n\x0fKEYCODE_ENDCALL\x10\x06\x12\r\n\tKEYCODE_0\x10\x07\x12\r\n\tKEYCODE_1\x10\x08\x12\r\n\tKEYCODE_2\x10\t\x12\r\n\tKEYCODE_3\x10\n\x12\r\n\tKEYCODE_4\x10\x0b\x12\r\n\tKEYCODE_5\x10\x0c\x12\r\n\tKEYCODE_6\x10\r\x12\r\n\tKEYCODE_7\x10\x0e\x12\r\n\tKEYCODE_8\x10\x0f\x12\r\n\tKEYCODE_9\x10\x10\x12\x10\n\x0cKEYCODE_STAR\x10\x11\x12\x11\n\rKEYCODE_POUND\x10\x12\x12\x13\n\x0fKEYCODE_DPAD_UP\x10\x13\x12\x15\n\x11KEYCODE_DPAD_DOWN\x10\x14\x12\x15\n\x11KEYCODE_DPAD_LEFT\x10\x15\x12\x16\n\x12KEYCODE_DPAD_RIGHT\x10\x16\x12\x17\n\x13KEYCODE_DPAD_CENTER\x10\x17\x12\x15\n\x11KEYCODE_VOLUME_UP\x10\x18\x12\x17\n\x13KEYCODE_VOLUME_DOWN\x10\x19\x12\x11\n\rKEYCODE_POWER\x10\x1a\x12\x12\n\x0eKEYCODE_CAMERA\x10\x1b\x12\x11\n\rKEYCODE_CLEAR\x10\x1c\x12\r\n\tKEYCODE_A\x10\x1d\x12\r\n\tKEYCODE_B\x10\x1e\x12\r\n\tKEYCODE_C\x10\x1f\x12\r\n\tKEYCODE_D\x10 \x12\r\n\tKEYCODE_E\x10!\x12\r\n\tKEYCODE_F\x10\"\x12\r\n\tKEYCODE_G\x10#\x12\r\n\tKEYCODE_H\x10$\x12\r\n\tKEYCODE_I\x10%\x12\r\n\tKEYCODE_J\x10&\x12\r\n\tKEYCODE_K\x10\'\x12\r\n\tKEYCODE_L\x10(\x12\r\n\tKEYCODE_M\x10)\x12\r\n\tKEYCODE_N\x10*\x12\r\n\tKEYCODE_O\x10+\x12\r\n\tKEYCODE_P\x10,\x12\r\n\tKEYCODE_Q\x10-\x12\r\n\tKEYCODE_R\x10.\x12\r\n\tKEYCODE_S\x10/\x12\r\n\tKEYCODE_T\x10\x30\x12\r\n\tKEYCODE_U\x10\x31\x12\r\n\tKEYCODE_V\x10\x32\x12\r\n\tKEYCODE_W\x10\x33\x12\r\n\tKEYCODE_X\x10\x34\x12\r\n\tKEYCODE_Y\x10\x35\x12\r\n\tKEYCODE_Z\x10\x36\x12\x11\n\rKEYCODE_COMMA\x10\x37\x12\x12\n\x0eKEYCODE_PERIOD\x10\x38\x12\x14\n\x10KEYCODE_ALT_LEFT\x10\x39\x12\x15\n\x11KEYCODE_ALT_RIGHT\x10:\x12\x16\n\x12KEYCODE_SHIFT_LEFT\x10;\x12\x17\n\x13KEYCODE_SHIFT_RIGHT\x10<\x12\x0f\n\x0bKEYCODE_TAB\x10=\x12\x11\n\rKEYCODE_SPACE\x10>\x12\x0f\n\x0bKEYCODE_SYM\x10?\x12\x14\n\x10KEYCODE_EXPLORER\x10@\x12\x14\n\x10KEYCODE_ENVELOPE\x10\x41\x12\x11\n\rKEYCODE_ENTER\x10\x42\x12\x0f\n\x0bKEYCODE_DEL\x10\x43\x12\x11\n\rKEYCODE_GRAVE\x10\x44\x12\x11\n\rKEYCODE_MINUS\x10\x45\x12\x12\n\x0eKEYCODE_EQUALS\x10\x46\x12\x18\n\x14KEYCODE_LEFT_BRACKET\x10G\x12\x19\n\x15KEYCODE_RIGHT_BRACKET\x10H\x12\x15\n\x11KEYCODE_BACKSLASH\x10I\x12\x15\n\x11KEYCODE_SEMICOLON\x10J\x12\x16\n\x12KEYCODE_APOSTROPHE\x10K\x12\x11\n\rKEYCODE_SLASH\x10L\x12\x0e\n\nKEYCODE_AT\x10M\x12\x0f\n\x0bKEYCODE_NUM\x10N\x12\x17\n\x13KEYCODE_HEADSETHOOK\x10O\x12\x11\n\rKEYCODE_FOCUS\x10P\x12\x10\n\x0cKEYCODE_PLUS\x10Q\x12\x10\n\x0cKEYCODE_MENU\x10R\x12\x18\n\x14KEYCODE_NOTIFICATION\x10S\x12\x12\n\x0eKEYCODE_SEARCH\x10T\x12\x1c\n\x18KEYCODE_MEDIA_PLAY_PAUSE\x10U\x12\x16\n\x12KEYCODE_MEDIA_STOP\x10V\x12\x16\n\x12KEYCODE_MEDIA_NEXT\x10W\x12\x1a\n\x16KEYCODE_MEDIA_PREVIOUS\x10X\x12\x18\n\x14KEYCODE_MEDIA_REWIND\x10Y\x12\x1e\n\x1aKEYCODE_MEDIA_FAST_FORWARD\x10Z\x12\x10\n\x0cKEYCODE_MUTE\x10[\x12\x13\n\x0fKEYCODE_PAGE_UP\x10\\\x12\x15\n\x11KEYCODE_PAGE_DOWN\x10]\x12\x17\n\x13KEYCODE_PICTSYMBOLS\x10^\x12\x1a\n\x16KEYCODE_SWITCH_CHARSET\x10_\x12\x14\n\x10KEYCODE_BUTTON_A\x10`\x12\x14\n\x10KEYCODE_BUTTON_B\x10\x61\x12\x14\n\x10KEYCODE_BUTTON_C\x10\x62\x12\x14\n\x10KEYCODE_BUTTON_X\x10\x63\x12\x14\n\x10KEYCODE_BUTTON_Y\x10\x64\x12\x14\n\x10KEYCODE_BUTTON_Z\x10\x65\x12\x15\n\x11KEYCODE_BUTTON_L1\x10\x66\x12\x15\n\x11KEYCODE_BUTTON_R1\x10g\x12\x15\n\x11KEYCODE_BUTTON_L2\x10h\x12\x15\n\x11KEYCODE_BUTTON_R2\x10i\x12\x19\n\x15KEYCODE_BUTTON_THUMBL\x10j\x12\x19\n\x15KEYCODE_BUTTON_THUMBR\x10k\x12\x18\n\x14KEYCODE_BUTTON_START\x10l\x12\x19\n\x15KEYCODE_BUTTON_SELECT\x10m\x12\x17\n\x13KEYCODE_BUTTON_MODE\x10n\x12\x12\n\x0eKEYCODE_ESCAPE\x10o\x12\x17\n\x13KEYCODE_FORWARD_DEL\x10p\x12\x15\n\x11KEYCODE_CTRL_LEFT\x10q\x12\x16\n\x12KEYCODE_CTRL_RIGHT\x10r\x12\x15\n\x11KEYCODE_CAPS_LOCK\x10s\x12\x17\n\x13KEYCODE_SCROLL_LOCK\x10t\x12\x15\n\x11KEYCODE_META_LEFT\x10u\x12\x16\n\x12KEYCODE_META_RIGHT\x10v\x12\x14\n\x10KEYCODE_FUNCTION\x10w\x12\x11\n\rKEYCODE_SYSRQ\x10x\x12\x11\n\rKEYCODE_BREAK\x10y\x12\x15\n\x11KEYCODE_MOVE_HOME\x10z\x12\x14\n\x10KEYCODE_MOVE_END\x10{\x12\x12\n\x0eKEYCODE_INSERT\x10|\x12\x13\n\x0fKEYCODE_FORWARD\x10}\x12\x16\n\x12KEYCODE_MEDIA_PLAY\x10~\x12\x17\n\x13KEYCODE_MEDIA_PAUSE\x10\x7f\x12\x18\n\x13KEYCODE_MEDIA_CLOSE\x10\x80\x01\x12\x18\n\x13KEYCODE_MEDIA_EJECT\x10\x81\x01\x12\x19\n\x14KEYCODE_MEDIA_RECORD\x10\x82\x01\x12\x0f\n\nKEYCODE_F1\x10\x83\x01\x12\x0f\n\nKEYCODE_F2\x10\x84\x01\x12\x0f\n\nKEYCODE_F3\x10\x85\x01\x12\x0f\n\nKEYCODE_F4\x10\x86\x01\x12\x0f\n\nKEYCODE_F5\x10\x87\x01\x12\x0f\n\nKEYCODE_F6\x10\x88\x01\x12\x0f\n\nKEYCODE_F7\x10\x89\x01\x12\x0f\n\nKEYCODE_F8\x10\x8a\x01\x12\x0f\n\nKEYCODE_F9\x10\x8b\x01\x12\x10\n\x0bKEYCODE_F10\x10\x8c\x01\x12\x10\n\x0bKEYCODE_F11\x10\x8d\x01\x12\x10\n\x0bKEYCODE_F12\x10\x8e\x01\x12\x15\n\x10KEYCODE_NUM_LOCK\x10\x8f\x01\x12\x15\n\x10KEYCODE_NUMPAD_0\x10\x90\x01\x12\x15\n\x10KEYCODE_NUMPAD_1\x10\x91\x01\x12\x15\n\x10KEYCODE_NUMPAD_2\x10\x92\x01\x12\x15\n\x10KEYCODE_NUMPAD_3\x10\x93\x01\x12\x15\n\x10KEYCODE_NUMPAD_4\x10\x94\x01\x12\x15\n\x10KEYCODE_NUMPAD_5\x10\x95\x01\x12\x15\n\x10KEYCODE_NUMPAD_6\x10\x96\x01\x12\x15\n\x10KEYCODE_NUMPAD_7\x10\x97\x01\x12\x15\n\x10KEYCODE_NUMPAD_8\x10\x98\x01\x12\x15\n\x10KEYCODE_NUMPAD_9\x10\x99\x01\x12\x1a\n\x15KEYCODE_NUMPAD_DIVIDE\x10\x9a\x01\x12\x1c\n\x17KEYCODE_NUMPAD_MULTIPLY\x10\x9b\x01\x12\x1c\n\x17KEYCODE_NUMPAD_SUBTRACT\x10\x9c\x01\x12\x17\n\x12KEYCODE_NUMPAD_ADD\x10\x9d\x01\x12\x17\n\x12KEYCODE_NUMPAD_DOT\x10\x9e\x01\x12\x19\n\x14KEYCODE_NUMPAD_COMMA\x10\x9f\x01\x12\x19\n\x14KEYCODE_NUMPAD_ENTER\x10\xa0\x01\x12\x1a\n\x15KEYCODE_NUMPAD_EQUALS\x10\xa1\x01\x12\x1e\n\x19KEYCODE_NUMPAD_LEFT_PAREN\x10\xa2\x01\x12\x1f\n\x1aKEYCODE_NUMPAD_RIGHT_PAREN\x10\xa3\x01\x12\x18\n\x13KEYCODE_VOLUME_MUTE\x10\xa4\x01\x12\x11\n\x0cKEYCODE_INFO\x10\xa5\x01\x12\x17\n\x12KEYCODE_CHANNEL_UP\x10\xa6\x01\x12\x19\n\x14KEYCODE_CHANNEL_DOWN\x10\xa7\x01\x12\x14\n\x0fKEYCODE_ZOOM_IN\x10\xa8\x01\x12\x15\n\x10KEYCODE_ZOOM_OUT\x10\xa9\x01\x12\x0f\n\nKEYCODE_TV\x10\xaa\x01\x12\x13\n\x0eKEYCODE_WINDOW\x10\xab\x01\x12\x12\n\rKEYCODE_GUIDE\x10\xac\x01\x12\x10\n\x0bKEYCODE_DVR\x10\xad\x01\x12\x15\n\x10KEYCODE_BOOKMARK\x10\xae\x01\x12\x15\n\x10KEYCODE_CAPTIONS\x10\xaf\x01\x12\x15\n\x10KEYCODE_SETTINGS\x10\xb0\x01\x12\x15\n\x10KEYCODE_TV_POWER\x10\xb1\x01\x12\x15\n\x10KEYCODE_TV_INPUT\x10\xb2\x01\x12\x16\n\x11KEYCODE_STB_POWER\x10\xb3\x01\x12\x16\n\x11KEYCODE_STB_INPUT\x10\xb4\x01\x12\x16\n\x11KEYCODE_AVR_POWER\x10\xb5\x01\x12\x16\n\x11KEYCODE_AVR_INPUT\x10\xb6\x01\x12\x15\n\x10KEYCODE_PROG_RED\x10\xb7\x01\x12\x17\n\x12KEYCODE_PROG_GREEN\x10\xb8\x01\x12\x18\n\x13KEYCODE_PROG_YELLOW\x10\xb9\x01\x12\x16\n\x11KEYCODE_PROG_BLUE\x10\xba\x01\x12\x17\n\x12KEYCODE_APP_SWITCH\x10\xbb\x01\x12\x15\n\x10KEYCODE_BUTTON_1\x10\xbc\x01\x12\x15\n\x10KEYCODE_BUTTON_2\x10\xbd\x01\x12\x15\n\x10KEYCODE_BUTTON_3\x10\xbe\x01\x12\x15\n\x10KEYCODE_BUTTON_4\x10\xbf\x01\x12\x15\n\x10KEYCODE_BUTTON_5\x10\xc0\x01\x12\x15\n\x10KEYCODE_BUTTON_6\x10\xc1\x01\x12\x15\n\x10KEYCODE_BUTTON_7\x10\xc2\x01\x12\x15\n\x10KEYCODE_BUTTON_8\x10\xc3\x01\x12\x15\n\x10KEYCODE_BUTTON_9\x10\xc4\x01\x12\x16\n\x11KEYCODE_BUTTON_10\x10\xc5\x01\x12\x16\n\x11KEYCODE_BUTTON_11\x10\xc6\x01\x12\x16\n\x11KEYCODE_BUTTON_12\x10\xc7\x01\x12\x16\n\x11KEYCODE_BUTTON_13\x10\xc8\x01\x12\x16\n\x11KEYCODE_BUTTON_14\x10\xc9\x01\x12\x16\n\x11KEYCODE_BUTTON_15\x10\xca\x01\x12\x16\n\x11KEYCODE_BUTTON_16\x10\xcb\x01\x12\x1c\n\x17KEYCODE_LANGUAGE_SWITCH\x10\xcc\x01\x12\x18\n\x13KEYCODE_MANNER_MODE\x10\xcd\x01\x12\x14\n\x0fKEYCODE_3D_MODE\x10\xce\x01\x12\x15\n\x10KEYCODE_CONTACTS\x10\xcf\x01\x12\x15\n\x10KEYCODE_CALENDAR\x10\xd0\x01\x12\x12\n\rKEYCODE_MUSIC\x10\xd1\x01\x12\x17\n\x12KEYCODE_CALCULATOR\x10\xd2\x01\x12\x1c\n\x17KEYCODE_ZENKAKU_HANKAKU\x10\xd3\x01\x12\x11\n\x0cKEYCODE_EISU\x10\xd4\x01\x12\x15\n\x10KEYCODE_MUHENKAN\x10\xd5\x01\x12\x13\n\x0eKEYCODE_HENKAN\x10\xd6\x01\x12\x1e\n\x19KEYCODE_KATAKANA_HIRAGANA\x10\xd7\x01\x12\x10\n\x0bKEYCODE_YEN\x10\xd8\x01\x12\x0f\n\nKEYCODE_RO\x10\xd9\x01\x12\x11\n\x0cKEYCODE_KANA\x10\xda\x01\x12\x13\n\x0eKEYCODE_ASSIST\x10\xdb\x01\x12\x1c\n\x17KEYCODE_BRIGHTNESS_DOWN\x10\xdc\x01\x12\x1a\n\x15KEYCODE_BRIGHTNESS_UP\x10\xdd\x01\x12\x1e\n\x19KEYCODE_MEDIA_AUDIO_TRACK\x10\xde\x01\x12\x12\n\rKEYCODE_SLEEP\x10\xdf\x01\x12\x13\n\x0eKEYCODE_WAKEUP\x10\xe0\x01\x12\x14\n\x0fKEYCODE_PAIRING\x10\xe1\x01\x12\x1b\n\x16KEYCODE_MEDIA_TOP_MENU\x10\xe2\x01\x12\x0f\n\nKEYCODE_11\x10\xe3\x01\x12\x0f\n\nKEYCODE_12\x10\xe4\x01\x12\x19\n\x14KEYCODE_LAST_CHANNEL\x10\xe5\x01\x12\x1c\n\x17KEYCODE_TV_DATA_SERVICE\x10\xe6\x01\x12\x19\n\x14KEYCODE_VOICE_ASSIST\x10\xe7\x01\x12\x1d\n\x18KEYCODE_TV_RADIO_SERVICE\x10\xe8\x01\x12\x18\n\x13KEYCODE_TV_TELETEXT\x10\xe9\x01\x12\x1c\n\x17KEYCODE_TV_NUMBER_ENTRY\x10\xea\x01\x12\"\n\x1dKEYCODE_TV_TERRESTRIAL_ANALOG\x10\xeb\x01\x12#\n\x1eKEYCODE_TV_TERRESTRIAL_DIGITAL\x10\xec\x01\x12\x19\n\x14KEYCODE_TV_SATELLITE\x10\xed\x01\x12\x1c\n\x17KEYCODE_TV_SATELLITE_BS\x10\xee\x01\x12\x1c\n\x17KEYCODE_TV_SATELLITE_CS\x10\xef\x01\x12!\n\x1cKEYCODE_TV_SATELLITE_SERVICE\x10\xf0\x01\x12\x17\n\x12KEYCODE_TV_NETWORK\x10\xf1\x01\x12\x1d\n\x18KEYCODE_TV_ANTENNA_CABLE\x10\xf2\x01\x12\x1c\n\x17KEYCODE_TV_INPUT_HDMI_1\x10\xf3\x01\x12\x1c\n\x17KEYCODE_TV_INPUT_HDMI_2\x10\xf4\x01\x12\x1c\n\x17KEYCODE_TV_INPUT_HDMI_3\x10\xf5\x01\x12\x1c\n\x17KEYCODE_TV_INPUT_HDMI_4\x10\xf6\x01\x12!\n\x1cKEYCODE_TV_INPUT_COMPOSITE_1\x10\xf7\x01\x12!\n\x1cKEYCODE_TV_INPUT_COMPOSITE_2\x10\xf8\x01\x12!\n\x1cKEYCODE_TV_INPUT_COMPONENT_1\x10\xf9\x01\x12!\n\x1cKEYCODE_TV_INPUT_COMPONENT_2\x10\xfa\x01\x12\x1b\n\x16KEYCODE_TV_INPUT_VGA_1\x10\xfb\x01\x12!\n\x1cKEYCODE_TV_AUDIO_DESCRIPTION\x10\xfc\x01\x12(\n#KEYCODE_TV_AUDIO_DESCRIPTION_MIX_UP\x10\xfd\x01\x12*\n%KEYCODE_TV_AUDIO_DESCRIPTION_MIX_DOWN\x10\xfe\x01\x12\x19\n\x14KEYCODE_TV_ZOOM_MODE\x10\xff\x01\x12\x1d\n\x18KEYCODE_TV_CONTENTS_MENU\x10\x80\x02\x12\"\n\x1dKEYCODE_TV_MEDIA_CONTEXT_MENU\x10\x81\x02\x12!\n\x1cKEYCODE_TV_TIMER_PROGRAMMING\x10\x82\x02\x12\x11\n\x0cKEYCODE_HELP\x10\x83\x02\x12\x1e\n\x19KEYCODE_NAVIGATE_PREVIOUS\x10\x84\x02\x12\x1a\n\x15KEYCODE_NAVIGATE_NEXT\x10\x85\x02\x12\x18\n\x13KEYCODE_NAVIGATE_IN\x10\x86\x02\x12\x19\n\x14KEYCODE_NAVIGATE_OUT\x10\x87\x02\x12\x19\n\x14KEYCODE_STEM_PRIMARY\x10\x88\x02\x12\x13\n\x0eKEYCODE_STEM_1\x10\x89\x02\x12\x13\n\x0eKEYCODE_STEM_2\x10\x8a\x02\x12\x13\n\x0eKEYCODE_STEM_3\x10\x8b\x02\x12\x19\n\x14KEYCODE_DPAD_UP_LEFT\x10\x8c\x02\x12\x1b\n\x16KEYCODE_DPAD_DOWN_LEFT\x10\x8d\x02\x12\x1a\n\x15KEYCODE_DPAD_UP_RIGHT\x10\x8e\x02\x12\x1c\n\x17KEYCODE_DPAD_DOWN_RIGHT\x10\x8f\x02\x12\x1f\n\x1aKEYCODE_MEDIA_SKIP_FORWARD\x10\x90\x02\x12 \n\x1bKEYCODE_MEDIA_SKIP_BACKWARD\x10\x91\x02\x12\x1f\n\x1aKEYCODE_MEDIA_STEP_FORWARD\x10\x92\x02\x12 \n\x1bKEYCODE_MEDIA_STEP_BACKWARD\x10\x93\x02\x12\x17\n\x12KEYCODE_SOFT_SLEEP\x10\x94\x02\x12\x10\n\x0bKEYCODE_CUT\x10\x95\x02\x12\x11\n\x0cKEYCODE_COPY\x10\x96\x02\x12\x12\n\rKEYCODE_PASTE\x10\x97\x02\x12!\n\x1cKEYCODE_SYSTEM_NAVIGATION_UP\x10\x98\x02\x12#\n\x1eKEYCODE_SYSTEM_NAVIGATION_DOWN\x10\x99\x02\x12#\n\x1eKEYCODE_SYSTEM_NAVIGATION_LEFT\x10\x9a\x02\x12$\n\x1fKEYCODE_SYSTEM_NAVIGATION_RIGHT\x10\x9b\x02\x12\x15\n\x10KEYCODE_ALL_APPS\x10\x9c\x02\x12\x14\n\x0fKEYCODE_REFRESH\x10\x9d\x02\x12\x16\n\x11KEYCODE_THUMBS_UP\x10\x9e\x02\x12\x18\n\x13KEYCODE_THUMBS_DOWN\x10\x9f\x02\x12\x1b\n\x16KEYCODE_PROFILE_SWITCH\x10\xa0\x02\x12\x18\n\x13KEYCODE_VIDEO_APP_1\x10\xa1\x02\x12\x18\n\x13KEYCODE_VIDEO_APP_2\x10\xa2\x02\x12\x18\n\x13KEYCODE_VIDEO_APP_3\x10\xa3\x02\x12\x18\n\x13KEYCODE_VIDEO_APP_4\x10\xa4\x02\x12\x18\n\x13KEYCODE_VIDEO_APP_5\x10\xa5\x02\x12\x18\n\x13KEYCODE_VIDEO_APP_6\x10\xa6\x02\x12\x18\n\x13KEYCODE_VIDEO_APP_7\x10\xa7\x02\x12\x18\n\x13KEYCODE_VIDEO_APP_8\x10\xa8\x02\x12\x1b\n\x16KEYCODE_FEATURED_APP_1\x10\xa9\x02\x12\x1b\n\x16KEYCODE_FEATURED_APP_2\x10\xaa\x02\x12\x1b\n\x16KEYCODE_FEATURED_APP_3\x10\xab\x02\x12\x1b\n\x16KEYCODE_FEATURED_APP_4\x10\xac\x02\x12\x17\n\x12KEYCODE_DEMO_APP_1\x10\xad\x02\x12\x17\n\x12KEYCODE_DEMO_APP_2\x10\xae\x02\x12\x17\n\x12KEYCODE_DEMO_APP_3\x10\xaf\x02\x12\x17\n\x12KEYCODE_DEMO_APP_4\x10\xb0\x02*Q\n\x0fRemoteDirection\x12\x15\n\x11UNKNOWN_DIRECTION\x10\x00\x12\x0e\n\nSTART_LONG\x10\x01\x12\x0c\n\x08\x45ND_LONG\x10\x02\x12\t\n\x05SHORT\x10\x03\x62\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'remotemessage_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'remotemessage_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _REMOTEKEYCODE._serialized_start=2677
-  _REMOTEKEYCODE._serialized_end=9820
-  _REMOTEDIRECTION._serialized_start=9822
-  _REMOTEDIRECTION._serialized_end=9903
-  _REMOTEAPPLINKLAUNCHREQUEST._serialized_start=31
-  _REMOTEAPPLINKLAUNCHREQUEST._serialized_end=77
-  _REMOTERESETPREFERREDAUDIODEVICE._serialized_start=79
-  _REMOTERESETPREFERREDAUDIODEVICE._serialized_end=112
-  _REMOTESETPREFERREDAUDIODEVICE._serialized_start=114
-  _REMOTESETPREFERREDAUDIODEVICE._serialized_end=145
-  _REMOTEADJUSTVOLUMELEVEL._serialized_start=147
-  _REMOTEADJUSTVOLUMELEVEL._serialized_end=172
-  _REMOTESETVOLUMELEVEL._serialized_start=175
-  _REMOTESETVOLUMELEVEL._serialized_end=355
-  _REMOTESTART._serialized_start=357
-  _REMOTESTART._serialized_end=387
-  _REMOTEVOICEEND._serialized_start=389
-  _REMOTEVOICEEND._serialized_end=405
-  _REMOTEVOICEPAYLOAD._serialized_start=407
-  _REMOTEVOICEPAYLOAD._serialized_end=427
-  _REMOTEVOICEBEGIN._serialized_start=429
-  _REMOTEVOICEBEGIN._serialized_end=447
-  _REMOTETEXTFIELDSTATUS._serialized_start=449
-  _REMOTETEXTFIELDSTATUS._serialized_end=567
-  _REMOTEIMESHOWREQUEST._serialized_start=569
-  _REMOTEIMESHOWREQUEST._serialized_end=656
-  _REMOTEEDITINFO._serialized_start=658
-  _REMOTEEDITINFO._serialized_end=690
-  _REMOTEIMEBATCHEDIT._serialized_start=692
-  _REMOTEIMEBATCHEDIT._serialized_end=799
-  _REMOTEAPPINFO._serialized_start=802
-  _REMOTEAPPINFO._serialized_end=955
-  _REMOTEIMEKEYINJECT._serialized_start=957
-  _REMOTEIMEKEYINJECT._serialized_end=1076
-  _REMOTEKEYINJECT._serialized_start=1078
-  _REMOTEKEYINJECT._serialized_end=1180
-  _REMOTEPINGRESPONSE._serialized_start=1182
-  _REMOTEPINGRESPONSE._serialized_end=1216
-  _REMOTEPINGREQUEST._serialized_start=1218
-  _REMOTEPINGREQUEST._serialized_end=1265
-  _REMOTESETACTIVE._serialized_start=1267
-  _REMOTESETACTIVE._serialized_end=1300
-  _REMOTEDEVICEINFO._serialized_start=1303
-  _REMOTEDEVICEINFO._serialized_end=1431
-  _REMOTECONFIGURE._serialized_start=1433
-  _REMOTECONFIGURE._serialized_end=1512
-  _REMOTEERROR._serialized_start=1514
-  _REMOTEERROR._serialized_end=1582
-  _REMOTEMESSAGE._serialized_start=1585
-  _REMOTEMESSAGE._serialized_end=2674
+  _globals['_REMOTEKEYCODE']._serialized_start=2677
+  _globals['_REMOTEKEYCODE']._serialized_end=9820
+  _globals['_REMOTEDIRECTION']._serialized_start=9822
+  _globals['_REMOTEDIRECTION']._serialized_end=9903
+  _globals['_REMOTEAPPLINKLAUNCHREQUEST']._serialized_start=31
+  _globals['_REMOTEAPPLINKLAUNCHREQUEST']._serialized_end=77
+  _globals['_REMOTERESETPREFERREDAUDIODEVICE']._serialized_start=79
+  _globals['_REMOTERESETPREFERREDAUDIODEVICE']._serialized_end=112
+  _globals['_REMOTESETPREFERREDAUDIODEVICE']._serialized_start=114
+  _globals['_REMOTESETPREFERREDAUDIODEVICE']._serialized_end=145
+  _globals['_REMOTEADJUSTVOLUMELEVEL']._serialized_start=147
+  _globals['_REMOTEADJUSTVOLUMELEVEL']._serialized_end=172
+  _globals['_REMOTESETVOLUMELEVEL']._serialized_start=175
+  _globals['_REMOTESETVOLUMELEVEL']._serialized_end=355
+  _globals['_REMOTESTART']._serialized_start=357
+  _globals['_REMOTESTART']._serialized_end=387
+  _globals['_REMOTEVOICEEND']._serialized_start=389
+  _globals['_REMOTEVOICEEND']._serialized_end=405
+  _globals['_REMOTEVOICEPAYLOAD']._serialized_start=407
+  _globals['_REMOTEVOICEPAYLOAD']._serialized_end=427
+  _globals['_REMOTEVOICEBEGIN']._serialized_start=429
+  _globals['_REMOTEVOICEBEGIN']._serialized_end=447
+  _globals['_REMOTETEXTFIELDSTATUS']._serialized_start=449
+  _globals['_REMOTETEXTFIELDSTATUS']._serialized_end=567
+  _globals['_REMOTEIMESHOWREQUEST']._serialized_start=569
+  _globals['_REMOTEIMESHOWREQUEST']._serialized_end=656
+  _globals['_REMOTEEDITINFO']._serialized_start=658
+  _globals['_REMOTEEDITINFO']._serialized_end=690
+  _globals['_REMOTEIMEBATCHEDIT']._serialized_start=692
+  _globals['_REMOTEIMEBATCHEDIT']._serialized_end=799
+  _globals['_REMOTEAPPINFO']._serialized_start=802
+  _globals['_REMOTEAPPINFO']._serialized_end=955
+  _globals['_REMOTEIMEKEYINJECT']._serialized_start=957
+  _globals['_REMOTEIMEKEYINJECT']._serialized_end=1076
+  _globals['_REMOTEKEYINJECT']._serialized_start=1078
+  _globals['_REMOTEKEYINJECT']._serialized_end=1180
+  _globals['_REMOTEPINGRESPONSE']._serialized_start=1182
+  _globals['_REMOTEPINGRESPONSE']._serialized_end=1216
+  _globals['_REMOTEPINGREQUEST']._serialized_start=1218
+  _globals['_REMOTEPINGREQUEST']._serialized_end=1265
+  _globals['_REMOTESETACTIVE']._serialized_start=1267
+  _globals['_REMOTESETACTIVE']._serialized_end=1300
+  _globals['_REMOTEDEVICEINFO']._serialized_start=1303
+  _globals['_REMOTEDEVICEINFO']._serialized_end=1431
+  _globals['_REMOTECONFIGURE']._serialized_start=1433
+  _globals['_REMOTECONFIGURE']._serialized_end=1512
+  _globals['_REMOTEERROR']._serialized_start=1514
+  _globals['_REMOTEERROR']._serialized_end=1582
+  _globals['_REMOTEMESSAGE']._serialized_start=1585
+  _globals['_REMOTEMESSAGE']._serialized_end=2674
 # @@protoc_insertion_point(module_scope)
```

### Comparing `androidtvremote2-0.0.9/src/androidtvremote2.egg-info/SOURCES.txt` & `androidtvremote2-0.1.0/src/androidtvremote2.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 src/androidtvremote2/androidtv_remote.py
 src/androidtvremote2/base.py
 src/androidtvremote2/certificate_generator.py
 src/androidtvremote2/const.py
 src/androidtvremote2/exceptions.py
 src/androidtvremote2/pairing.py
 src/androidtvremote2/polo_pb2.py
+src/androidtvremote2/polo_pb2.pyi
 src/androidtvremote2/remote.py
 src/androidtvremote2/remotemessage_pb2.py
+src/androidtvremote2/remotemessage_pb2.pyi
 src/androidtvremote2.egg-info/PKG-INFO
 src/androidtvremote2.egg-info/SOURCES.txt
 src/androidtvremote2.egg-info/dependency_links.txt
 src/androidtvremote2.egg-info/requires.txt
 src/androidtvremote2.egg-info/top_level.txt
 tests/test_androidtv_remote.py
```

### Comparing `androidtvremote2-0.0.9/src/demo.py` & `androidtvremote2-0.1.0/src/demo.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,29 +15,30 @@
     ConnectionClosed,
     InvalidAuth,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
-async def _bind_keyboard(remote: AndroidTVRemote):
+async def _bind_keyboard(remote: AndroidTVRemote) -> None:
     print(
         "\n\nYou can control the connected Android TV with:"
         "\n- arrow keys: move selected item"
         "\n- enter: run selected item"
         "\n- space: play/pause"
         "\n- home: go to the home screen"
         "\n- backspace or esc: go back"
-        "\n- delete: power off/one"
+        "\n- delete: power off/on"
         "\n- +/-: volume up/down"
         "\n- 'm': mute"
         "\n- 'y': YouTube"
         "\n- 'n': Netflix"
         "\n- 'd': Disney+"
         "\n- 'a': Amazon Prime Video"
+        "\n- 'k': Kodi"
         "\n- 'q': quit\n\n"
     )
     key_mappings = {
         keyboard.Key.up: "DPAD_UP",
         keyboard.Key.down: "DPAD_DOWN",
         keyboard.Key.left: "DPAD_LEFT",
         keyboard.Key.right: "DPAD_RIGHT",
@@ -45,19 +46,19 @@
         keyboard.Key.space: "MEDIA_PLAY_PAUSE",
         keyboard.Key.home: "HOME",
         keyboard.Key.backspace: "BACK",
         keyboard.Key.esc: "BACK",
         keyboard.Key.delete: "POWER",
     }
 
-    def transmit_keys():
-        queue = asyncio.Queue()
+    def transmit_keys() -> asyncio.Queue:
+        queue: asyncio.Queue = asyncio.Queue()
         loop = asyncio.get_event_loop()
 
-        def on_press(key):
+        def on_press(key: keyboard.Key | keyboard.KeyCode | None) -> None:
             loop.call_soon_threadsafe(queue.put_nowait, key)
 
         keyboard.Listener(on_press=on_press).start()
         return queue
 
     key_queue = transmit_keys()
     while True:
@@ -73,73 +74,75 @@
             elif key.char == "+":
                 remote.send_key_command("VOLUME_UP")
             elif key.char == "-":
                 remote.send_key_command("VOLUME_DOWN")
             elif key.char == "y":
                 remote.send_launch_app_command("https://www.youtube.com")
             elif key.char == "n":
-                remote.send_launch_app_command("https://www.netflix.com/title")
+                remote.send_launch_app_command("com.netflix.ninja")
             elif key.char == "d":
-                remote.send_launch_app_command("https://www.disneyplus.com")
+                remote.send_launch_app_command("com.disney.disneyplus")
             elif key.char == "a":
-                remote.send_launch_app_command("https://app.primevideo.com")
+                remote.send_launch_app_command("com.amazon.amazonvideo.livingroom")
+            elif key.char == "k":
+                remote.send_launch_app_command("org.xbmc.kodi")
 
 
 async def _host_from_zeroconf(timeout: float) -> str:
     def _async_on_service_state_change(
         zeroconf: Zeroconf,
         service_type: str,
         name: str,
         state_change: ServiceStateChange,
     ) -> None:
         if state_change is not ServiceStateChange.Added:
             return
-        _ = asyncio.ensure_future(
+        _ = asyncio.ensure_future(  # noqa: RUF006
             async_display_service_info(zeroconf, service_type, name)
         )
 
     async def async_display_service_info(
         zeroconf: Zeroconf, service_type: str, name: str
     ) -> None:
         info = AsyncServiceInfo(service_type, name)
         await info.async_request(zeroconf, 3000)
         if info:
             addresses = [
                 "%s:%d" % (addr, cast(int, info.port))
                 for addr in info.parsed_scoped_addresses()
             ]
-            print("  Name: %s" % name)
-            print("  Addresses: %s" % ", ".join(addresses))
+            print(f"  Name: {name}")
+            print(f"  Addresses: {", ".join(addresses)}")
             if info.properties:
                 print("  Properties:")
                 for key, value in info.properties.items():
-                    print(f"    {key}: {value}")
+                    print(f"    {key!r}: {value!r}")
             else:
                 print("  No properties")
         else:
             print("  No info")
         print()
 
-    aiozc = AsyncZeroconf()
+    zc = AsyncZeroconf()
     services = ["_androidtvremote2._tcp.local."]
     print(
         f"\nBrowsing {services} service(s) for {timeout} seconds, press Ctrl-C to exit...\n"
     )
-    aiobrowser = AsyncServiceBrowser(
-        aiozc.zeroconf, services, handlers=[_async_on_service_state_change]
+    browser = AsyncServiceBrowser(
+        zc.zeroconf, services, handlers=[_async_on_service_state_change]
     )
     await asyncio.sleep(timeout)
 
-    await aiobrowser.async_cancel()
-    await aiozc.async_close()
+    await browser.async_cancel()
+    await zc.async_close()
 
     return input("Enter IP address of Android TV to connect to: ").split(":")[0]
 
 
-async def _pair(remote: AndroidTVRemote):
+async def _pair(remote: AndroidTVRemote) -> None:
     name, mac = await remote.async_get_name_and_mac()
     if (
         input(
             f"Do you want to pair with {remote.host} {name} {mac}"
             " (this will turn on the Android TV)? y/n: "
         )
         != "y"
@@ -154,15 +157,15 @@
             _LOGGER.error("Invalid pairing code. Error: %s", exc)
             continue
         except ConnectionClosed as exc:
             _LOGGER.error("Initialize pair again. Error: %s", exc)
             return await _pair(remote)
 
 
-async def _main():
+async def _main() -> None:
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", help="IP address of Android TV to connect to")
     parser.add_argument(
         "--certfile",
         help="filename that contains the client certificate in PEM format",
         default="cert.pem",
     )
@@ -211,24 +214,24 @@
     remote.keep_reconnecting()
 
     _LOGGER.info("device_info: %s", remote.device_info)
     _LOGGER.info("is_on: %s", remote.is_on)
     _LOGGER.info("current_app: %s", remote.current_app)
     _LOGGER.info("volume_info: %s", remote.volume_info)
 
-    def is_on_updated(is_on):
+    def is_on_updated(is_on: bool) -> None:
         _LOGGER.info("Notified that is_on: %s", is_on)
 
-    def current_app_updated(current_app):
+    def current_app_updated(current_app: str) -> None:
         _LOGGER.info("Notified that current_app: %s", current_app)
 
-    def volume_info_updated(volume_info):
+    def volume_info_updated(volume_info: dict[str, str | bool]) -> None:
         _LOGGER.info("Notified that volume_info: %s", volume_info)
 
-    def is_available_updated(is_available):
+    def is_available_updated(is_available: bool) -> None:
         _LOGGER.info("Notified that is_available: %s", is_available)
 
     remote.add_is_on_updated_callback(is_on_updated)
     remote.add_current_app_updated_callback(current_app_updated)
     remote.add_volume_info_updated_callback(volume_info_updated)
     remote.add_is_available_updated_callback(is_available_updated)
```

