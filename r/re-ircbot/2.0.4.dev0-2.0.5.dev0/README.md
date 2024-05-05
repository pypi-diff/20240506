# Comparing `tmp/re_ircbot-2.0.4.dev0.tar.gz` & `tmp/re_ircbot-2.0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re_ircbot-2.0.4.dev0.tar", last modified: Sat May  4 23:48:39 2024, max compression
+gzip compressed data, was "re_ircbot-2.0.5.dev0.tar", last modified: Sun May  5 19:20:31 2024, max compression
```

## Comparing `re_ircbot-2.0.4.dev0.tar` & `re_ircbot-2.0.5.dev0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 23:48:39.752266 re_ircbot-2.0.4.dev0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-04 23:48:32.000000 re_ircbot-2.0.4.dev0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-04 23:48:39.752266 re_ircbot-2.0.4.dev0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13331 2024-05-04 23:48:32.000000 re_ircbot-2.0.4.dev0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 23:48:39.752266 re_ircbot-2.0.4.dev0/ircbot/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/ircbot/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    53399 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/ircbot/client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5384 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/ircbot/dcc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17845 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/ircbot/hooks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3039 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/ircbot/message.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/ircbot/shortest_prefix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11380 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/ircbot/sqlitedb.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1426 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/ircbot/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-04 23:48:39.752266 re_ircbot-2.0.4.dev0/re_ircbot.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-04 23:48:39.000000 re_ircbot-2.0.4.dev0/re_ircbot.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      335 2024-05-04 23:48:39.000000 re_ircbot-2.0.4.dev0/re_ircbot.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-04 23:48:39.000000 re_ircbot-2.0.4.dev0/re_ircbot.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2024-05-04 23:48:39.000000 re_ircbot-2.0.4.dev0/re_ircbot.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-04 23:48:39.000000 re_ircbot-2.0.4.dev0/re_ircbot.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-04 23:48:39.752266 re_ircbot-2.0.4.dev0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2024-05-04 23:48:33.000000 re_ircbot-2.0.4.dev0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 19:20:31.516736 re_ircbot-2.0.5.dev0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-05 19:20:31.516736 re_ircbot-2.0.5.dev0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13331 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 19:20:31.516736 re_ircbot-2.0.5.dev0/ircbot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    54808 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5384 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/dcc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5004 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/format.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18286 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/hooks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1822 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/message.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/shortest_prefix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11380 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/sqlitedb.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1426 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/ircbot/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-05 19:20:31.516736 re_ircbot-2.0.5.dev0/re_ircbot.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14099 2024-05-05 19:20:31.000000 re_ircbot-2.0.5.dev0/re_ircbot.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      352 2024-05-05 19:20:31.000000 re_ircbot-2.0.5.dev0/re_ircbot.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-05 19:20:31.000000 re_ircbot-2.0.5.dev0/re_ircbot.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2024-05-05 19:20:31.000000 re_ircbot-2.0.5.dev0/re_ircbot.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-05 19:20:31.000000 re_ircbot-2.0.5.dev0/re_ircbot.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-05 19:20:31.516736 re_ircbot-2.0.5.dev0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2024-05-05 19:20:24.000000 re_ircbot-2.0.5.dev0/setup.py
```

### Comparing `re_ircbot-2.0.4.dev0/LICENSE` & `re_ircbot-2.0.5.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.4.dev0/PKG-INFO` & `re_ircbot-2.0.5.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-ircbot
-Version: 2.0.4.dev0
+Version: 2.0.5.dev0
 Summary: A simple async irc bot framework with regex command definitions and data permanency
 Home-page: https://github.com/matheusfillipe/ircbot
 Author: Matheus Fillipe
 Author-email: mattf@tilde.club
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `re_ircbot-2.0.4.dev0/README.md` & `re_ircbot-2.0.5.dev0/README.md`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.4.dev0/ircbot/client.py` & `re_ircbot-2.0.5.dev0/ircbot/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from math import ceil
 from pathlib import Path
 from typing import Any, Awaitable, Callable
 
 from cachetools import TTLCache
 
 from ircbot import dcc, hooks
-from ircbot.message import Color, Message, RawMessage, ReplyIntent, Sendable
+from ircbot.message import Message, RawMessage, ReplyIntent, Sendable, Style
 from ircbot.sqlitedb import DB
 from ircbot.utils import debug, log, logger, validate_url
 
 Message = Message
 ReplyIntent = ReplyIntent
 RawMessage = RawMessage
 
@@ -298,32 +298,34 @@
         """Store anything you want in memory here."""
         return self._data
 
     @data.setter
     def data(self, value: Any):
         self._data = value
 
-    def _install_hooks(self):
+    def install_hooks(self):
+        """Installs or reinstalls this bot's hooks."""
         self.custom_handlers.update(self.custom_handlers)
         if self.arg_commands_with_message:
             new_commands = deepcopy(self._defined_command_dict)
             new_commands.update(self.arg_commands_with_message)
             self.set_commands(new_commands, prefix=self.command_prefix)
 
     async def hot_reload(self):
         """Reload the handlers."""
+        log("Hot reloading...\n\n")
         self._hot_reload()
         self.custom_handlers.update(self.custom_handlers)
         if self.arg_commands_with_message:
             new_commands = deepcopy(self._defined_command_dict)
             new_commands.update(self.arg_commands_with_message)
             self.set_commands(new_commands, prefix=self.command_prefix)
 
     async def _mainloop(self, async_callback: AsyncCallback | None):
-        self._install_hooks()
+        self.install_hooks()
         self.is_running_with_callback = bool(async_callback)
         self.async_callback = async_callback
         while True:
             try:
                 await self._main_task()
             except (BotConnectionError, socket.gaierror):
                 log(f"Attempting to reconnect in {self.ping_delay / 2}...")
@@ -544,28 +546,56 @@
 
         if isinstance(channel, list):
             for chan in channel:
                 await self._send_message(message, chan)
         else:
             await self._send_message(message, channel)
 
+    def format_reply_message(self, reply_to: Message, message: str) -> str:
+        """Define how a reply message should look be formatted."""
+        return f"{reply_to.sender_nick}: {message}"
+
+    def _format_reply_message(self, reply_to: Message, message: Sendable) -> Sendable:
+        if isinstance(message, str):
+            return self.format_reply_message(reply_to, message)
+        elif isinstance(message, Style):
+            return self.format_reply_message(reply_to, message.str)
+        elif isinstance(message, list):
+            msgs = []
+            for msg in message:
+                msgs.append(self._format_reply_message(reply_to, msg))
+            return msgs
+        elif isinstance(message, Message):
+            return self.format_reply_message(reply_to, message.message)
+        else:
+            raise ValueError("Message must be a str, a list of str, a Message object or a Style object")
+
+    async def reply(self, reply_to: Message, message: Sendable):
+        """Replies to a message prepending it with the sender's nick.
+
+        :param message: Can be a str, a list of str or a IrcBot.Message object.
+        :param msg: Any sendable message object.
+        """
+        sendable = self._format_reply_message(reply_to, message)
+        await self.send_message(sendable, reply_to.channel)
+
     async def _send_message(self, message: Sendable, channel: str):
         if isinstance(message, str):
             message = message.replace("\n", "    ")
             message = message.replace("\r", "")
             await self._enqueue_message((str("PRIVMSG " + channel) + " :" + message + " \r\n"))
-        elif isinstance(message, Color):
+        elif isinstance(message, Style):
             await self._send_message(message.str, channel)
         elif isinstance(message, list):
             for msg in message:
                 await self._send_message(msg, channel)
         elif isinstance(message, Message):
             await self._send_message(message.message, message.channel)
         else:
-            raise ValueError("Message must be a str, a list of str, a Message object or a Color object")
+            raise ValueError("Message must be a str, a list of str, a Message object or a Style object")
 
     async def message_task_loop(self):
         while True:
             try:
                 msg = await self.message_queue.get()
                 await self._send_data(msg)
                 self.message_queue.task_done()
```

### Comparing `re_ircbot-2.0.4.dev0/ircbot/dcc.py` & `re_ircbot-2.0.5.dev0/ircbot/dcc.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.4.dev0/ircbot/hooks.py` & `re_ircbot-2.0.5.dev0/ircbot/hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from functools import wraps
 from typing import Awaitable, Literal, TypeAlias, get_args
 
 from typing_extensions import Self
 
 from ircbot.message import Message, Sendable
 from ircbot.shortest_prefix import find_shortest_prefix
-from ircbot.utils import log
+from ircbot.utils import debug, log
 
 
 def md5_file(file):
     import hashlib
 
     with open(file, "rb") as f:
         return hashlib.md5(f.read()).hexdigest()
@@ -189,25 +189,33 @@
         self,
         command: str,
         help: str = "",
         command_help: str = "",
         acccept_pms: bool = True,
         pass_data: bool = False,
         simplify: bool | None = None,
+        alias: str | list[str] | None = None,
         **kwargs,
     ):
         """Wrapper for setCommands.
 
         :param command: Command
         :param acccept_pms: bool. Should this command work with private messages?.
         param: simplify: Uses shortest prefixes for each command. If True the shortest differentiatable prefixes for the commands will work. Like if there is start and stop, !sta will call start and !sto will call stop. Instead of passing a function  directly you can pass in a dict like:
         param: help: Message to display on help command.
         param: command_help: Message to display on help command with this command's name as argument.
+        alias: str or list of strings with aliases for this command
         """
 
+        aliases = []
+        if isinstance(alias, str):
+            aliases = [alias]
+        elif alias is None:
+            aliases = []
+
         if simplify is None:
             simplify = self.simplify_arg_commands
 
         def wrap_cmd(func: ArgCommandCallback):
             @wraps(func)
             def wrapped(*a, **bb):
                 return func(*a, **bb)
@@ -218,14 +226,18 @@
                 "acccept_pms": acccept_pms,
                 "pass_data": pass_data,
                 "help": help,
                 "command_help": command_help,
                 "simplify": simplify,
             }
 
+            for a in aliases:
+                debug(f"Adding alias {a} for {command}")
+                self.arg_commands_with_message[a] = self.arg_commands_with_message[command]
+
             return wrapped
 
         return wrap_cmd
 
     help_msg_header: list[str] = []
     help_msg: dict[str, str] = {}
     help_msg_bottom: list[str] = []
```

### Comparing `re_ircbot-2.0.4.dev0/ircbot/message.py` & `re_ircbot-2.0.5.dev0/ircbot/message.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,10 @@
-import random
 from typing import TypeAlias
 
-
-class Color(object):
-    """Colorcodes enum."""
-
-    esc = "\003"
-    white = "00"
-    black = "01"
-    navy = "02"
-    green = "03"
-    red = "04"
-    maroon = "05"
-    purple = "06"
-    orange = "07"
-    yellow = "08"
-    light_green = "09"
-    teal = "10"
-    cyan = "11"
-    blue = "12"
-    magenta = "13"
-    gray = "14"
-    light_gray = "15"
-
-    COLORS = [
-        "00",
-        "01",
-        "02",
-        "03",
-        "04",
-        "05",
-        "06",
-        "07",
-        "08",
-        "09",
-        "10",
-        "11",
-        "12",
-        "13",
-        "14",
-        "15",
-    ]
-
-    def __init__(self, text, fg=white, bg=None):
-        if bg is not None:
-            self.text = "{}{},{}{}".format(self.esc, fg, bg, text)
-        else:
-            self.text = "{}{}{}".format(self.esc, fg, text)
-        self.str = self.text + Color.esc
-
-    @classmethod
-    def random(cls):
-        return random.choice(cls.COLORS)
-
-    @classmethod
-    def colors(cls):
-        """Returns the color names."""
-        return [
-            k
-            for k in Color.__dict__
-            if not (k.startswith("_") or k in ["esc", "COLORS", "colors", "getcolors", "random"])
-        ]
-
-    def __str__(self):
-        return self.str
+from ircbot.format import Style
 
 
 class RawMessage:
     def __init__(self, message):
         self.message = message
 
     def __str__(self):
@@ -100,8 +37,8 @@
         """__init__.
 
         :param message: Message to send. You can use a message object if you want to change channel or make it a pm.  :param func: Function to call passing the received full message string that the user will reply with. This is useful for building dialogs. This function must either return None, a message to send back (str or IrcBot.Message) or another ReplyIntent. It must receive one argument."""
         self.func = func
         self.message = message
 
 
-Sendable: TypeAlias = str | Message | Color | list[str] | list[Message] | list[Color] | ReplyIntent
+Sendable: TypeAlias = str | Message | Style | list[str] | list[Message] | list[Style] | ReplyIntent
```

### Comparing `re_ircbot-2.0.4.dev0/ircbot/shortest_prefix.py` & `re_ircbot-2.0.5.dev0/ircbot/shortest_prefix.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.4.dev0/ircbot/sqlitedb.py` & `re_ircbot-2.0.5.dev0/ircbot/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.4.dev0/ircbot/utils.py` & `re_ircbot-2.0.5.dev0/ircbot/utils.py`

 * *Files identical despite different names*

### Comparing `re_ircbot-2.0.4.dev0/re_ircbot.egg-info/PKG-INFO` & `re_ircbot-2.0.5.dev0/re_ircbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-ircbot
-Version: 2.0.4.dev0
+Version: 2.0.5.dev0
 Summary: A simple async irc bot framework with regex command definitions and data permanency
 Home-page: https://github.com/matheusfillipe/ircbot
 Author: Matheus Fillipe
 Author-email: mattf@tilde.club
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `re_ircbot-2.0.4.dev0/setup.py` & `re_ircbot-2.0.5.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import subprocess
 
 import setuptools
 
-VERSION = "2.0.4-dev"
+VERSION = "2.0.5-dev"
 BRANCH = "v2"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 def requirements():
```

