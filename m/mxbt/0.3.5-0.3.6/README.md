# Comparing `tmp/mxbt-0.3.5.tar.gz` & `tmp/mxbt-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxbt-0.3.5.tar", last modified: Fri Apr 26 15:43:47 2024, max compression
+gzip compressed data, was "mxbt-0.3.6.tar", last modified: Mon May  6 11:42:00 2024, max compression
```

## Comparing `mxbt-0.3.5.tar` & `mxbt-0.3.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-26 15:43:47.046463 mxbt-0.3.5/
--rw-r--r--   0 warlock   (1000) warlock   (1000)    35149 2024-04-26 15:33:21.000000 mxbt-0.3.5/LICENSE
--rw-r--r--   0 warlock   (1000) warlock   (1000)     3130 2024-04-26 15:43:47.046463 mxbt-0.3.5/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2383 2024-04-26 15:38:14.000000 mxbt-0.3.5/README.md
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-26 15:43:47.046463 mxbt-0.3.5/mxbt/
--rw-r--r--   0 warlock   (1000) warlock   (1000)      221 2024-04-26 15:42:57.000000 mxbt-0.3.5/mxbt/__init__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     5465 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/auth.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)    22720 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/bot.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     3395 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/callbacks.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     7431 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/context.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     9633 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/filters.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     7582 2024-04-26 15:37:31.000000 mxbt-0.3.5/mxbt/listener.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     3938 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/match.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2441 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/module.py
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-26 15:43:47.046463 mxbt-0.3.5/mxbt/types/
--rw-r--r--   0 warlock   (1000) warlock   (1000)       67 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/types/__init__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)      279 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/types/command.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)    10011 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/types/file.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)      178 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/types/msgtype.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)      281 2024-04-26 15:33:21.000000 mxbt-0.3.5/mxbt/utils.py
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-26 15:43:47.046463 mxbt-0.3.5/mxbt.egg-info/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     3130 2024-04-26 15:43:46.000000 mxbt-0.3.5/mxbt.egg-info/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)      403 2024-04-26 15:43:46.000000 mxbt-0.3.5/mxbt.egg-info/SOURCES.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-26 15:43:46.000000 mxbt-0.3.5/mxbt.egg-info/dependency_links.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       80 2024-04-26 15:43:46.000000 mxbt-0.3.5/mxbt.egg-info/requires.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        5 2024-04-26 15:43:46.000000 mxbt-0.3.5/mxbt.egg-info/top_level.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-26 15:43:47.046463 mxbt-0.3.5/setup.cfg
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1032 2024-04-26 15:33:21.000000 mxbt-0.3.5/setup.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-05-06 11:42:00.590811 mxbt-0.3.6/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)    35149 2024-04-26 15:33:21.000000 mxbt-0.3.6/LICENSE
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     3386 2024-05-06 11:42:00.590811 mxbt-0.3.6/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2632 2024-05-06 11:36:38.000000 mxbt-0.3.6/README.md
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-05-06 11:42:00.590811 mxbt-0.3.6/mxbt/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      243 2024-05-06 11:28:58.000000 mxbt-0.3.6/mxbt/__init__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     6865 2024-05-06 11:25:51.000000 mxbt-0.3.6/mxbt/auth.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)    22786 2024-05-06 11:28:30.000000 mxbt-0.3.6/mxbt/bot.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     9193 2024-05-06 10:36:37.000000 mxbt-0.3.6/mxbt/callbacks.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1158 2024-05-06 09:53:42.000000 mxbt-0.3.6/mxbt/config.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     7431 2024-04-26 15:33:21.000000 mxbt-0.3.6/mxbt/context.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     9633 2024-04-26 15:33:21.000000 mxbt-0.3.6/mxbt/filters.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     7596 2024-05-06 09:11:28.000000 mxbt-0.3.6/mxbt/listener.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     3938 2024-04-26 15:33:21.000000 mxbt-0.3.6/mxbt/match.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2441 2024-04-26 15:33:21.000000 mxbt-0.3.6/mxbt/module.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-05-06 11:42:00.590811 mxbt-0.3.6/mxbt/types/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       67 2024-04-26 15:33:21.000000 mxbt-0.3.6/mxbt/types/__init__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      279 2024-04-26 15:33:21.000000 mxbt-0.3.6/mxbt/types/command.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)    10011 2024-04-26 15:33:21.000000 mxbt-0.3.6/mxbt/types/file.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      178 2024-04-26 15:33:21.000000 mxbt-0.3.6/mxbt/types/msgtype.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      281 2024-05-06 09:12:27.000000 mxbt-0.3.6/mxbt/utils.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-05-06 11:42:00.590811 mxbt-0.3.6/mxbt.egg-info/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     3386 2024-05-06 11:42:00.000000 mxbt-0.3.6/mxbt.egg-info/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      418 2024-05-06 11:42:00.000000 mxbt-0.3.6/mxbt.egg-info/SOURCES.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-05-06 11:42:00.000000 mxbt-0.3.6/mxbt.egg-info/dependency_links.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       72 2024-05-06 11:42:00.000000 mxbt-0.3.6/mxbt.egg-info/requires.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        5 2024-05-06 11:42:00.000000 mxbt-0.3.6/mxbt.egg-info/top_level.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-05-06 11:42:00.590811 mxbt-0.3.6/setup.cfg
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1027 2024-05-06 11:18:12.000000 mxbt-0.3.6/setup.py
```

### Comparing `mxbt-0.3.5/LICENSE` & `mxbt-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mxbt-0.3.5/PKG-INFO` & `mxbt-0.3.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxbt
-Version: 0.3.5
+Version: 0.3.6
 Summary: Yet another Matrix bot library.
 Home-page: https://codeberg.org/librehub/mxbt
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,matrix-nio,matrix,bot,api
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -13,17 +13,18 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matrix-nio
 Requires-Dist: pillow
 Requires-Dist: markdown
-Requires-Dist: python-cryptography-fernet-wrapper
+Requires-Dist: cryptography
 Requires-Dist: filetype
 Requires-Dist: aiofiles
+Requires-Dist: python-dotenv
 
 # mxbt 
 
 Yet another Matrix bot library, built on [matrix-nio](https://github.com/matrix-nio/matrix-nio).
 
 ## Feauters
 
@@ -36,15 +37,15 @@
     - [x] External files
     - [x] Internal files
 - [x] Native mentions
 - [x] Access to `matrix-nio` features
 - [x] Event filters
 - [x] Bot modules support
 - [ ] Wait for event system
-- [ ] Full e2ee support
+- [x] E2EE support (check [docs](docs/encryption.md) before)
 
 ## Installation
 
 **With pip:**
 
 ```sh
 $ pip install mxbt
@@ -59,39 +60,41 @@
 ```
 
 ## Getting started
 
 More examples [here](examples/) or in [docs](https://librehub.codeberg.page/mxbt/).
 
 ```python
-from mxbt import Bot, Context, Creds, Filter, Listener
+from mxbt import Bot, Context, Creds, Config, Filter, Listener
 import asyncio
 
 bot = Bot(
-    prefix="!",          # Standart command prefix, commands can setup it own prefix
-    creds=Creds.from_json_file("credits.json")
+    creds=Creds.from_env(               # You also can use Creds.from_json and just Creds() 
+        homeserver="MATRIX_HOMESERVER",
+        username="MATRIX_USERNAME",
+        password="MATRIX_PASSWORD"
+    ),                               
+    config=Config()                     # Config has many options for bot, like prefix, selfbot, encryption, etc...
 )
 lr = Listener(bot)
 
 @lr.on_command(prefix="?", aliases=["test", "t"])
 @Filter.from_users(['@username:homeserver'])    # Event works only with this senders
 async def ctx_echo(ctx: Context) -> None:       # Context object contains main info about event
     await ctx.reply(ctx.body)                   # Reply message to event room
 
 if __name__ == "__main__":
     asyncio.run(lr.start_polling())
 ```
 
-**credits.json** structure
-```json
-{
-    "homeserver" : "https://matrix.org",
-    "user_id" : "user",
-    "password" : "password"
-}
+**.env** structure
+```env
+MATRIX_HOMESERVER=https://matrix.org/
+MATRIX_USERNAME=user
+MATRIX_PASSWORD=password
 ```
 
 ## Built with mxbt
 
 | Project                                               | Description                       |
 | :---                                                  | :---                              |
 | [sofie](https://codeberg.org/librehub/sofie)          | A simple selfbot                  |
```

### Comparing `mxbt-0.3.5/README.md` & `mxbt-0.3.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     - [x] External files
     - [x] Internal files
 - [x] Native mentions
 - [x] Access to `matrix-nio` features
 - [x] Event filters
 - [x] Bot modules support
 - [ ] Wait for event system
-- [ ] Full e2ee support
+- [x] E2EE support (check [docs](docs/encryption.md) before)
 
 ## Installation
 
 **With pip:**
 
 ```sh
 $ pip install mxbt
@@ -36,39 +36,41 @@
 ```
 
 ## Getting started
 
 More examples [here](examples/) or in [docs](https://librehub.codeberg.page/mxbt/).
 
 ```python
-from mxbt import Bot, Context, Creds, Filter, Listener
+from mxbt import Bot, Context, Creds, Config, Filter, Listener
 import asyncio
 
 bot = Bot(
-    prefix="!",          # Standart command prefix, commands can setup it own prefix
-    creds=Creds.from_json_file("credits.json")
+    creds=Creds.from_env(               # You also can use Creds.from_json and just Creds() 
+        homeserver="MATRIX_HOMESERVER",
+        username="MATRIX_USERNAME",
+        password="MATRIX_PASSWORD"
+    ),                               
+    config=Config()                     # Config has many options for bot, like prefix, selfbot, encryption, etc...
 )
 lr = Listener(bot)
 
 @lr.on_command(prefix="?", aliases=["test", "t"])
 @Filter.from_users(['@username:homeserver'])    # Event works only with this senders
 async def ctx_echo(ctx: Context) -> None:       # Context object contains main info about event
     await ctx.reply(ctx.body)                   # Reply message to event room
 
 if __name__ == "__main__":
     asyncio.run(lr.start_polling())
 ```
 
-**credits.json** structure
-```json
-{
-    "homeserver" : "https://matrix.org",
-    "user_id" : "user",
-    "password" : "password"
-}
+**.env** structure
+```env
+MATRIX_HOMESERVER=https://matrix.org/
+MATRIX_USERNAME=user
+MATRIX_PASSWORD=password
 ```
 
 ## Built with mxbt
 
 | Project                                               | Description                       |
 | :---                                                  | :---                              |
 | [sofie](https://codeberg.org/librehub/sofie)          | A simple selfbot                  |
```

### Comparing `mxbt-0.3.5/mxbt/auth.py` & `mxbt-0.3.6/mxbt/auth.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,21 @@
-from fernet_wrapper import Wrapper as fw
-import json
-
 """
-Implementation from: 
+Partly implementation from: 
 https://codeberg.org/imbev/simplematrixbotlib/src/branch/master/simplematrixbotlib/auth.py
 """
 
+from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import hashes
+from cryptography.fernet import Fernet
+import dotenv
+import base64
+import json
+import os
+
 class Creds:
     """
     A class to store and handle login credentials.
 
     ...
 
     Attributes
@@ -66,29 +72,64 @@
         self.login_token = login_token
         self.access_token = access_token
         self._session_stored_file = session_stored_file
         self.device_name = device_name
         self.device_id = ""
 
         if self.password:
-            self._key = fw.key_from_pass(self.password)
+            self._key = self.fernet_key_from_pass(self.password)
         elif self.login_token:
-            self._key = fw.key_from_pass(self.login_token)
+            self._key = self.fernet_key_from_pass(self.login_token)
         elif self.access_token:
-            self._key = fw.key_from_pass(self.access_token)
+            self._key = self.fernet_key_from_pass(self.access_token)
         else:
             raise ValueError(
                 "password or login_token or access_token is required")
 
-    @staticmethod 
-    def from_json_file(filepath: str):
+    def fernet_key_from_pass(self, value: str, unique: bool=False) -> bytes:
+        password = bytes(value, 'utf-8')
+        if unique:
+            salt = os.urandom(16)
+        else:
+            salt = b'0\xc03T\xb8\x9a\xf9\xcb\xf4\xf8\xc7\x00a\xd6\xa7M'
+        kdf = PBKDF2HMAC(
+            algorithm=hashes.SHA256(),
+            length=32,
+            salt=salt,
+            iterations=100000,
+            backend=default_backend()
+        )
+        return base64.urlsafe_b64encode(kdf.derive(password))
+
+    def fernet_decrypt(self, token, key):
+        f = Fernet(key)
+        data = str(f.decrypt(token))
+        if data[0:2] == "b'":
+            data = data[2:-1]
+        return data
+
+    @classmethod
+    def from_env(cls, filepath: str=".env", **kwargs):
+        """
+        Initialize class using .env file.
+        You can provide any custom options with format:
+            name = ENV_VAR_NAME
+        """
+        dotenv.load_dotenv(filepath)
+        data = dict()
+        for key, value in kwargs.items():
+            data[key] = os.environ.get(value)
+        return cls(**data)
+
+    @classmethod
+    def from_json(cls, filepath: str):
         data = json.load(open(filepath, "r"))
-        return Creds(
+        return cls(
             data['homeserver'],
-            data['user_id'],
+            data['username'],
             data['password']
         )
 
     def session_read_file(self):
         """
         Reads and decrypts the device_id and access_token from file
 
@@ -99,15 +140,15 @@
                     encrypted_session_data = bytes(f.read()[2:-1], 'utf-8')
                     file_exists = True
 
             except FileNotFoundError:
                 file_exists = False
 
             if file_exists:
-                decrypted_session_data = fw.decrypt(
+                decrypted_session_data = self.fernet_decrypt(
                     encrypted_session_data,
                     self._key)[3:-2].replace('\'', '').replace(' ',
                                                                '').split(",")
 
                 self.device_id = decrypted_session_data[0]
                 self.access_token = decrypted_session_data[1]
 
@@ -140,12 +181,16 @@
         elif (self.device_id == "") or (self.access_token == ""):
             raise ValueError(
                 f"Can't save credentials: empty device ID '{self.device_id}' or access token '{self.access_token}'"
             )
 
         session_data = str([self.device_id, self.access_token])
 
-        encrypted_session_data = fw.encrypt(session_data, self._key)
+        encrypted_session_data = Fernet(
+            self._key
+        ).encrypt(
+            session_data.encode()
+        )
 
         with open(self._session_stored_file, 'w') as f:
             f.write(str(encrypted_session_data))
```

### Comparing `mxbt-0.3.5/mxbt/bot.py` & `mxbt-0.3.6/mxbt/bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from nio import (AsyncClient, Event, MatrixRoom,
                  OlmUnverifiedDeviceError,
                  AsyncClientConfig,
                  RoomGetEventResponse,
                  RoomMessageFile, RoomMessageImage,
                  RoomMessageText, RoomMessageVideo,
                  RoomSendResponse, SyncResponse)
-from nio.crypto import ENCRYPTION_ENABLED
-from typing import List, Union, Tuple 
-import cryptography
+from cryptography.fernet import InvalidToken
+from typing import List, Union, Tuple
 import markdown
 import aiohttp
 import json
 import nio
 import re
 import os
 
 from .types.file import File, FileUrl
 from .callbacks import Callbacks
 from .utils import info, error
+from .config import Config
 
 def split_mxid(mxid: str) -> Union[Tuple[str, str], Tuple[None, None]]:
     # s = mxid.split(':')
     # if len(s) != 2 or s[0][0] != '@':
     #     return None, None
     # s[0] = s[0][1:]
     match = re.match(
@@ -29,17 +29,17 @@
         mxid)
     if match is None:
         return None, None
     return match.group('localpart'), match.group('hostname')
 
 class Bot:
 
-    def __init__(self, creds, prefix: str="!", selfbot: bool=False, config: dict=dict()) -> None:
-        self.prefix = prefix
-        self.selfbot = selfbot
+    def __init__(self, creds, config: Config) -> None:
+        self.prefix = config.prefix
+        self.selfbot = config.selfbot
         self.creds = creds 
         self.config = config
         self.user_emotes = dict()
         self.room_emotes = dict()
 
         self.async_client: AsyncClient | None = None
         self.callbacks: Callbacks | None = None
@@ -51,15 +51,15 @@
         Can be runed with mxbt.Bot.run method or with asyncio.run(bot.connect())
 
         Implementation from:
         https://codeberg.org/imbev/simplematrixbotlib/src/branch/master/simplematrixbotlib/bot.py
         """
         try:
             self.creds.session_read_file()
-        except cryptography.fernet.InvalidToken:
+        except InvalidToken:
             print("Invalid Stored Token")
             print("Regenerating token from provided credentials")
             os.remove(self.creds._session_stored_file)
             self.creds.session_read_file()
 
         await self.login()
 
@@ -68,15 +68,15 @@
 
         resp = await self.async_client.sync(full_state=True)  #Ignore prior messages
 
         if isinstance(resp, SyncResponse):
             info(
                 f"Connected to {self.async_client.homeserver} as {self.async_client.user_id} ({self.async_client.device_id})"
             )
-            if ENCRYPTION_ENABLED:
+            if self.config.encryption_enabled:
                 if self.async_client.olm is None:
                     raise Exception("AsyncClient doesn't have olm module")
                 key = self.async_client.olm.account.identity_keys['ed25519']
                 info(
                     f"This bot's public fingerprint (\"Session key\") for one-sided verification is: "
                     f"{' '.join([key[i:i+4] for i in range(0, len(key), 4)])}")
 
@@ -136,15 +136,15 @@
                 "Either password, login token or access token must be provided"
             )
 
         client_config = AsyncClientConfig(
             max_limit_exceeded=0,
             max_timeouts=0,
             store_sync_tokens=True,
-            encryption_enabled=ENCRYPTION_ENABLED)
+            encryption_enabled=self.config.encryption_enabled)
         store_path = "./store"
         os.makedirs(store_path, mode=0o750, exist_ok=True)
         self.async_client = AsyncClient(homeserver=self.creds.homeserver,
                                         user=self.creds.username,
                                         device_id=self.creds.device_id,
                                         store_path=store_path,
                                         config=client_config)
@@ -261,15 +261,15 @@
             raise Exception("AsyncClient is None!")
 
         try:
             res = await self.async_client.room_send(
                 room_id=room_id,
                 message_type=message_type,
                 content=content,
-                ignore_unverified_devices=ignore_unverified_devices)
+                ignore_unverified_devices=ignore_unverified_devices or self.config.ignore_unverified_devices)
             if isinstance(res, RoomSendResponse):
                 res = await self.async_client.room_get_event(res.room_id, res.event_id)
                 if isinstance(res, RoomGetEventResponse):
                     return res.event
         except OlmUnverifiedDeviceError:
             # print(str(e))
             error(
@@ -290,15 +290,15 @@
                 if len(unverified) > 0:
                     info(f"\tUser {user}: {', '.join(unverified)}")
 
             res = await self.async_client.room_send(
                 room_id=room_id,
                 message_type=message_type,
                 content=content,
-                ignore_unverified_devices=ignore_unverified_devices)
+                ignore_unverified_devices=ignore_unverified_devices or self.config.ignore_unverified_devices)
             if isinstance(res, RoomSendResponse):
                 res = await self.async_client.room_get_event(res.room_id, res.event_id)
                 if isinstance(res, RoomGetEventResponse):
                     return res.event
 
     async def __send(self, room_id: str, body: str | File | FileUrl,
                      use_html: bool, reply_to: str="", edit_id: str="",
```

### Comparing `mxbt-0.3.5/mxbt/context.py` & `mxbt-0.3.6/mxbt/context.py`

 * *Files identical despite different names*

### Comparing `mxbt-0.3.5/mxbt/filters.py` & `mxbt-0.3.6/mxbt/filters.py`

 * *Files identical despite different names*

### Comparing `mxbt-0.3.5/mxbt/listener.py` & `mxbt-0.3.6/mxbt/listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         self._commands.append(Command(prefix, aliases))
 
     def _reg_event(self, func, event) -> None:
         self._registry.append([func, event])
 
     def _get_command_prefix(self, **kwargs) -> str:
         if not 'prefix' in kwargs.keys():
-            return self._bot.prefix
+            return self._bot.config.prefix
         else:
             return kwargs['prefix']
 
     def _get_command_name(self, prefix: str, body: str) -> str:
         return body.split(" ")[0].replace(prefix, "")
 
     def get_commands(self) -> list:
@@ -151,15 +151,15 @@
             async def command_func(room, event: RoomMessageText) -> None:
                 if not event.body.startswith(prefix):
                     return
 
                 match = Match(room, event, self._bot)
                 name = self._get_command_name(prefix, event.body)
                 if name in kwargs['aliases']:
-                    if self._bot.selfbot:
+                    if self._bot.config.selfbot:
                         if not match.is_from_self():
                             return
                     else:
                         if match.is_from_self():
                             return
                     await func(Context.from_command(self._bot, room, event, prefix, kwargs['aliases']))
             self._reg_event(command_func, RoomMessageText)
```

### Comparing `mxbt-0.3.5/mxbt/match.py` & `mxbt-0.3.6/mxbt/match.py`

 * *Files identical despite different names*

### Comparing `mxbt-0.3.5/mxbt/module.py` & `mxbt-0.3.6/mxbt/module.py`

 * *Files identical despite different names*

### Comparing `mxbt-0.3.5/mxbt/types/file.py` & `mxbt-0.3.6/mxbt/types/file.py`

 * *Files identical despite different names*

### Comparing `mxbt-0.3.5/mxbt.egg-info/PKG-INFO` & `mxbt-0.3.6/mxbt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxbt
-Version: 0.3.5
+Version: 0.3.6
 Summary: Yet another Matrix bot library.
 Home-page: https://codeberg.org/librehub/mxbt
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,matrix-nio,matrix,bot,api
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -13,17 +13,18 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matrix-nio
 Requires-Dist: pillow
 Requires-Dist: markdown
-Requires-Dist: python-cryptography-fernet-wrapper
+Requires-Dist: cryptography
 Requires-Dist: filetype
 Requires-Dist: aiofiles
+Requires-Dist: python-dotenv
 
 # mxbt 
 
 Yet another Matrix bot library, built on [matrix-nio](https://github.com/matrix-nio/matrix-nio).
 
 ## Feauters
 
@@ -36,15 +37,15 @@
     - [x] External files
     - [x] Internal files
 - [x] Native mentions
 - [x] Access to `matrix-nio` features
 - [x] Event filters
 - [x] Bot modules support
 - [ ] Wait for event system
-- [ ] Full e2ee support
+- [x] E2EE support (check [docs](docs/encryption.md) before)
 
 ## Installation
 
 **With pip:**
 
 ```sh
 $ pip install mxbt
@@ -59,39 +60,41 @@
 ```
 
 ## Getting started
 
 More examples [here](examples/) or in [docs](https://librehub.codeberg.page/mxbt/).
 
 ```python
-from mxbt import Bot, Context, Creds, Filter, Listener
+from mxbt import Bot, Context, Creds, Config, Filter, Listener
 import asyncio
 
 bot = Bot(
-    prefix="!",          # Standart command prefix, commands can setup it own prefix
-    creds=Creds.from_json_file("credits.json")
+    creds=Creds.from_env(               # You also can use Creds.from_json and just Creds() 
+        homeserver="MATRIX_HOMESERVER",
+        username="MATRIX_USERNAME",
+        password="MATRIX_PASSWORD"
+    ),                               
+    config=Config()                     # Config has many options for bot, like prefix, selfbot, encryption, etc...
 )
 lr = Listener(bot)
 
 @lr.on_command(prefix="?", aliases=["test", "t"])
 @Filter.from_users(['@username:homeserver'])    # Event works only with this senders
 async def ctx_echo(ctx: Context) -> None:       # Context object contains main info about event
     await ctx.reply(ctx.body)                   # Reply message to event room
 
 if __name__ == "__main__":
     asyncio.run(lr.start_polling())
 ```
 
-**credits.json** structure
-```json
-{
-    "homeserver" : "https://matrix.org",
-    "user_id" : "user",
-    "password" : "password"
-}
+**.env** structure
+```env
+MATRIX_HOMESERVER=https://matrix.org/
+MATRIX_USERNAME=user
+MATRIX_PASSWORD=password
 ```
 
 ## Built with mxbt
 
 | Project                                               | Description                       |
 | :---                                                  | :---                              |
 | [sofie](https://codeberg.org/librehub/sofie)          | A simple selfbot                  |
```

### Comparing `mxbt-0.3.5/setup.py` & `mxbt-0.3.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     version=VERSION,
     author="loliconshik3",
     author_email="loliconshik3@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=packages,
-    install_requires=['matrix-nio', 'pillow', 'markdown', 'python-cryptography-fernet-wrapper', 'filetype', 'aiofiles'],
+    install_requires=['matrix-nio', 'pillow', 'markdown', 'cryptography', 'filetype', 'aiofiles', 'python-dotenv'],
     keywords=['python', 'matrix-nio', 'matrix', 'bot', 'api'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

