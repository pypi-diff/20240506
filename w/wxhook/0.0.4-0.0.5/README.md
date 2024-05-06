# Comparing `tmp/wxhook-0.0.4.tar.gz` & `tmp/wxhook-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxhook-0.0.4.tar", last modified: Mon May  6 08:26:04 2024, max compression
+gzip compressed data, was "wxhook-0.0.5.tar", last modified: Mon May  6 10:02:26 2024, max compression
```

## Comparing `wxhook-0.0.4.tar` & `wxhook-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 08:26:04.649679 wxhook-0.0.4/
--rw-rw-rw-   0        0        0     1077 2024-05-06 06:49:40.000000 wxhook-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       51 2024-05-06 06:49:40.000000 wxhook-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6695 2024-05-06 08:26:04.648677 wxhook-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5951 2024-05-06 07:42:05.000000 wxhook-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-06 08:26:04.649679 wxhook-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     3928 2024-05-06 07:49:01.000000 wxhook-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:26:04.631300 wxhook-0.0.4/wxhook/
--rw-rw-rw-   0        0        0       44 2024-05-06 07:49:01.000000 wxhook-0.0.4/wxhook/__init__.py
--rw-rw-rw-   0        0        0    16187 2024-05-06 08:10:05.000000 wxhook-0.0.4/wxhook/core.py
--rw-rw-rw-   0        0        0      630 2024-05-06 06:49:40.000000 wxhook-0.0.4/wxhook/events.py
--rw-rw-rw-   0        0        0      273 2024-05-06 06:49:40.000000 wxhook-0.0.4/wxhook/logger.py
--rw-rw-rw-   0        0        0     3930 2024-05-06 07:14:37.000000 wxhook-0.0.4/wxhook/model.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:26:04.644541 wxhook-0.0.4/wxhook/tools/
--rwxrwxrwx   0        0        0   270336 2024-05-06 06:49:40.000000 wxhook-0.0.4/wxhook/tools/faker.exe
--rwxrwxrwx   0        0        0   911872 2024-05-06 06:49:40.000000 wxhook-0.0.4/wxhook/tools/start-wechat.exe
--rw-rw-rw-   0        0        0   592384 2024-05-06 06:49:40.000000 wxhook-0.0.4/wxhook/tools/wxhook.dll
--rw-rw-rw-   0        0        0     3566 2024-05-06 08:06:43.000000 wxhook-0.0.4/wxhook/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-06 08:26:04.640473 wxhook-0.0.4/wxhook.egg-info/
--rw-rw-rw-   0        0        0     6695 2024-05-06 08:26:04.000000 wxhook-0.0.4/wxhook.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2024-05-06 08:26:04.000000 wxhook-0.0.4/wxhook.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 08:26:04.000000 wxhook-0.0.4/wxhook.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-06 08:26:04.000000 wxhook-0.0.4/wxhook.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-06 08:26:04.000000 wxhook-0.0.4/wxhook.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 10:02:26.369561 wxhook-0.0.5/
+-rw-rw-rw-   0        0        0     1077 2024-05-06 06:49:40.000000 wxhook-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-05-06 09:07:02.000000 wxhook-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6719 2024-05-06 10:02:26.368558 wxhook-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5975 2024-05-06 10:02:18.000000 wxhook-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 10:02:26.369561 wxhook-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     3928 2024-05-06 09:15:12.000000 wxhook-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:02:26.346001 wxhook-0.0.5/wxhook/
+-rw-rw-rw-   0        0        0       44 2024-05-06 08:41:27.000000 wxhook-0.0.5/wxhook/__init__.py
+-rw-rw-rw-   0        0        0    16255 2024-05-06 08:41:27.000000 wxhook-0.0.5/wxhook/core.py
+-rw-rw-rw-   0        0        0      630 2024-05-06 06:49:40.000000 wxhook-0.0.5/wxhook/events.py
+-rw-rw-rw-   0        0        0      310 2024-05-06 08:37:49.000000 wxhook-0.0.5/wxhook/logger.py
+-rw-rw-rw-   0        0        0     3930 2024-05-06 07:14:37.000000 wxhook-0.0.5/wxhook/model.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:02:26.364486 wxhook-0.0.5/wxhook/tools/
+-rwxrwxrwx   0        0        0   270336 2024-05-06 06:49:40.000000 wxhook-0.0.5/wxhook/tools/faker.exe
+-rwxrwxrwx   0        0        0   911872 2024-05-06 06:49:40.000000 wxhook-0.0.5/wxhook/tools/start-wechat.exe
+-rw-rw-rw-   0        0        0   592384 2024-05-06 06:49:40.000000 wxhook-0.0.5/wxhook/tools/wxhook.dll
+-rw-rw-rw-   0        0        0     3749 2024-05-06 08:35:25.000000 wxhook-0.0.5/wxhook/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 10:02:26.360423 wxhook-0.0.5/wxhook.egg-info/
+-rw-rw-rw-   0        0        0     6719 2024-05-06 10:02:26.000000 wxhook-0.0.5/wxhook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2024-05-06 10:02:26.000000 wxhook-0.0.5/wxhook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 10:02:26.000000 wxhook-0.0.5/wxhook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-06 10:02:26.000000 wxhook-0.0.5/wxhook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-06 10:02:26.000000 wxhook-0.0.5/wxhook.egg-info/top_level.txt
```

### Comparing `wxhook-0.0.4/LICENSE` & `wxhook-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.4/PKG-INFO` & `wxhook-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhook
-Version: 0.0.4
+Version: 0.0.5
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhook
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -80,20 +80,21 @@
 
 ## 使用示例
 
 消息事件处理例子
 ```python
 # import os
 # os.environ["WXHOOK_LOG_LEVEL"] = "INFO" # 修改日志输出级别
+# os.environ["WXHOOK_LOG_FORMAT"] = "INFO" # 修改日志输出格式
 from wxhook import Bot
 from wxhook import events
 from wxhook.model import Event
 
 
-def on_login(bot: Bot):
+def on_login(bot: Bot, event: Event):
     print("登录成功之后会触发这个函数")
 
 
 def on_start(bot: Bot):
     print("微信客户端打开之后会触发这个函数")
 
 
@@ -135,19 +136,17 @@
 import os
 import json
 
 from wxhook import Bot
 from wxhook import events
 from wxhook.model import Event
 
-# faked_version="3.9.10.19"解除微信低版本登录限制
 bot = Bot()
 
-msgid_list = []
-
+msg_id_list = []
 
 @bot.handle(events.TEXT_MESSAGE)
 def on_text_message(bot: Bot, event: Event):
     self_id = bot.info.wxid
     content = event.content
     sender = event.fromUser
     msg_id = event.msgId
@@ -184,17 +183,17 @@
             bot.send_room_at(sender, ["<wxid1>", "<wxid2>"], "这是一条at群成员的消息")
         elif content.find("发送群聊拍一拍") != -1:
             bot.send_pat(sender, "wxid_vqj81fdula0x22")
         elif content.find("发送私聊拍一拍") != -1:
             bot.send_pat(sender, sender)
         elif content.find("置顶消息") != -1:
             bot.top_msg(msg_id)
-            msgid_list.append(msg_id)
+            msg_id_list.append(msg_id)
         elif content.find("取消置顶的消息") != -1:
-            bot.remove_top_msg(sender, msgid_list.pop())
+            bot.remove_top_msg(sender, msg_id_list.pop())
         elif content.find("获取联系人列表") != -1:
             bot.send_text(sender, json.dumps(bot.get_contacts()))
         elif content.find("获取联系人详情") != -1:
             bot.send_text(sender, json.dumps(bot.get_contact("<wxid>")))
         elif content.find("获取群详情") != -1:
             print(bot.get_room("<chatroomid>"))
         elif content.find("收藏消息") != -1:
```

### Comparing `wxhook-0.0.4/README.md` & `wxhook-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -56,20 +56,21 @@
 
 ## 使用示例
 
 消息事件处理例子
 ```python
 # import os
 # os.environ["WXHOOK_LOG_LEVEL"] = "INFO" # 修改日志输出级别
+# os.environ["WXHOOK_LOG_FORMAT"] = "INFO" # 修改日志输出格式
 from wxhook import Bot
 from wxhook import events
 from wxhook.model import Event
 
 
-def on_login(bot: Bot):
+def on_login(bot: Bot, event: Event):
     print("登录成功之后会触发这个函数")
 
 
 def on_start(bot: Bot):
     print("微信客户端打开之后会触发这个函数")
 
 
@@ -111,19 +112,17 @@
 import os
 import json
 
 from wxhook import Bot
 from wxhook import events
 from wxhook.model import Event
 
-# faked_version="3.9.10.19"解除微信低版本登录限制
 bot = Bot()
 
-msgid_list = []
-
+msg_id_list = []
 
 @bot.handle(events.TEXT_MESSAGE)
 def on_text_message(bot: Bot, event: Event):
     self_id = bot.info.wxid
     content = event.content
     sender = event.fromUser
     msg_id = event.msgId
@@ -160,17 +159,17 @@
             bot.send_room_at(sender, ["<wxid1>", "<wxid2>"], "这是一条at群成员的消息")
         elif content.find("发送群聊拍一拍") != -1:
             bot.send_pat(sender, "wxid_vqj81fdula0x22")
         elif content.find("发送私聊拍一拍") != -1:
             bot.send_pat(sender, sender)
         elif content.find("置顶消息") != -1:
             bot.top_msg(msg_id)
-            msgid_list.append(msg_id)
+            msg_id_list.append(msg_id)
         elif content.find("取消置顶的消息") != -1:
-            bot.remove_top_msg(sender, msgid_list.pop())
+            bot.remove_top_msg(sender, msg_id_list.pop())
         elif content.find("获取联系人列表") != -1:
             bot.send_text(sender, json.dumps(bot.get_contacts()))
         elif content.find("获取联系人详情") != -1:
             bot.send_text(sender, json.dumps(bot.get_contact("<wxid>")))
         elif content.find("获取群详情") != -1:
             print(bot.get_room("<chatroomid>"))
         elif content.find("收藏消息") != -1:
```

### Comparing `wxhook-0.0.4/setup.py` & `wxhook-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'wxhook'
 DESCRIPTION = 'wechat robot framework.'
 URL = 'https://github.com/miloira/wxhook'
 EMAIL = '690126048@qq.com'
 AUTHOR = 'Msky'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'loguru',
     'psutil',
     'pyee',
     'requests',
```

### Comparing `wxhook-0.0.4/wxhook/core.py` & `wxhook-0.0.5/wxhook/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import socketserver
 from functools import lru_cache
 
 import psutil
 import pyee
 import requests
 
-from .events import ALL_MESSAGE
 from .logger import logger
+from .events import ALL_MESSAGE
 from .model import Event, Account, Contact, ContactDetail, Room, RoomMembers, Table, DB, Response
 from .utils import WeChatManager, start_wechat_with_inject, fake_wechat_version, get_pid, parse_event
 
 
 class RequestHandler(socketserver.BaseRequestHandler):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -425,44 +425,44 @@
         """测试"""
         return Response(**self.call_api("/api/test"))
 
     @property
     def info(self) -> Account:
         return self.get_self_info()
 
-    def on_event(self, raw_data: bytes):
+    def on_event(self, raw_data: bytes) -> None:
         try:
             data = json.loads(raw_data)
             event = Event(**parse_event(data))
             logger.debug(event)
             self.call_hook_func(self.on_before_message, self, event)
             self.event_emitter.emit(str(ALL_MESSAGE), self, event)
             self.event_emitter.emit(str(event.type), self, event)
             self.call_hook_func(self.on_after_message, self, event)
             self.webhook(data)
         except Exception:
             logger.error(traceback.format_exc())
             logger.error(raw_data)
 
-    def handle(self, events: typing.Union[list[str], str, None] = None, once: bool = False):
+    def handle(self, events: typing.Union[list[str], str, None] = None, once: bool = False) -> typing.Callable[[typing.Callable], None]:
         def wrapper(func):
             listen = self.event_emitter.on if not once else self.event_emitter.once
             if not events:
                 listen(str(ALL_MESSAGE), func)
             else:
                 for event in events if isinstance(events, list) else [events]:
                     listen(str(event), func)
 
         return wrapper
 
-    def exit(self):
+    def exit(self) -> None:
         self.call_hook_func(self.on_stop, self)
         self.process.terminate()
 
-    def run(self):
+    def run(self) -> None:
         try:
             server = socketserver.ThreadingTCPServer((self.server_host, self.server_port), RequestHandler)
             server.bot = self
             logger.info(f"Listening Server at {self.server_host}:{self.server_port}")
             server.serve_forever()
         except (KeyboardInterrupt, SystemExit):
             self.exit()
```

### Comparing `wxhook-0.0.4/wxhook/events.py` & `wxhook-0.0.5/wxhook/events.py`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.4/wxhook/model.py` & `wxhook-0.0.5/wxhook/model.py`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.4/wxhook/tools/faker.exe` & `wxhook-0.0.5/wxhook/tools/faker.exe`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.4/wxhook/tools/start-wechat.exe` & `wxhook-0.0.5/wxhook/tools/start-wechat.exe`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.4/wxhook/tools/wxhook.dll` & `wxhook-0.0.5/wxhook/tools/wxhook.dll`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.4/wxhook/utils.py` & `wxhook-0.0.5/wxhook/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 import os
 import json
+import typing
 import pathlib
 import subprocess
 
 import psutil
 import xmltodict
 
 BASE_DIR = pathlib.Path(__file__).resolve().parent
 TOOLS = BASE_DIR / "tools"
 DLL = TOOLS / "wxhook.dll"
 START_WECHAT = TOOLS / "start-wechat.exe"
 FAKER = TOOLS / "faker.exe"
 
 
-def start_wechat_with_inject(port: int):
+def start_wechat_with_inject(port: int) -> typing.Tuple[int, str]:
     result = subprocess.run(f"{START_WECHAT} {DLL} {port}", capture_output=True, text=True)
     code, output = result.stdout.split(",")
     return int(code), output
 
 
-def fake_wechat_version(pid: int, old_version: str, new_version: str):
+def fake_wechat_version(pid: int, old_version: str, new_version: str) -> int:
     result = subprocess.run(f"{FAKER} {pid} {old_version} {new_version}", capture_output=True, text=True)
     return int(result.stdout)
 
 
-def get_processes(process_name: str):
+def get_processes(process_name: str) -> list[psutil.Process]:
     processes = []
     for process in psutil.process_iter():
         if process.name().lower() == process_name.lower():
             processes.append(process)
     return processes
 
 
-def get_pid(port: int):
+def get_pid(port: int) -> int:
     output = subprocess.run(f"netstat -ano | findStr \"{port}\"", capture_output=True, text=True, shell=True).stdout
     return int(output.split("\n")[0].split("LISTENING")[-1])
 
 
-def parse_xml(xml: str):
+def parse_xml(xml: str) -> dict:
     return xmltodict.parse(xml)
 
 
-def parse_event(event: dict, fields=None):
+def parse_event(event: dict, fields=None) -> dict:
     for field in fields or ["content", "signature"]:
         try:
             if field in event:
                 event[field] = parse_xml(event[field])
         except Exception:
             pass
     return event
@@ -59,59 +60,59 @@
         # http port:   38999 ~ 57997
         self.filename = BASE_DIR / "tools" / "wxhook.json"
         if not os.path.exists(self.filename):
             self.init_file()
         else:
             self.clean()
 
-    def init_file(self):
+    def init_file(self) -> None:
         with open(self.filename, "w", encoding="utf-8") as file:
             json.dump({
                 "increase_remote_port": 19000,
                 "wechat": []
             }, file)
 
-    def read(self):
+    def read(self) -> dict:
         with open(self.filename, "r", encoding="utf-8") as file:
             data = json.load(file)
         return data
 
-    def write(self, data: dict):
+    def write(self, data: dict) -> None:
         with open(self.filename, "w", encoding="utf-8") as file:
             json.dump(data, file)
 
-    def refresh(self, pid_list: list[int]):
+    def refresh(self, pid_list: list[int]) -> None:
         data = self.read()
         cleaned_data = []
         remote_port_list = [19000]
         for item in data["wechat"]:
             if item["pid"] in pid_list:
                 remote_port_list.append(item["remote_port"])
                 cleaned_data.append(item)
 
         data["increase_remote_port"] = max(remote_port_list)
         data["wechat"] = cleaned_data
         self.write(data)
 
-    def clean(self):
+    def clean(self) -> None:
         pid_list = [process.pid for process in get_processes("WeChat.exe")]
         self.refresh(pid_list)
 
-    def get_remote_port(self):
+    def get_remote_port(self) -> int:
         data = self.read()
         return data["increase_remote_port"] + 1
 
-    def get_listen_port(self, remote_port: int):
+    def get_listen_port(self, remote_port: int) -> int:
         return 19000 - (remote_port - 19000)
 
-    def get_port(self):
+    def get_port(self) -> typing.Tuple[int, int]:
         remote_port = self.get_remote_port()
         return remote_port, self.get_listen_port(remote_port)
 
-    def add(self, pid: int, remote_port: int, server_port: int):
+    def add(self, pid: int, remote_port: int, server_port: int) -> None:
         data = self.read()
         data["increase_remote_port"] = remote_port
         data["wechat"].append({
             "pid": pid,
             "remote_port": remote_port,
             "server_port": server_port
         })
```

### Comparing `wxhook-0.0.4/wxhook.egg-info/PKG-INFO` & `wxhook-0.0.5/wxhook.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhook
-Version: 0.0.4
+Version: 0.0.5
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhook
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -80,20 +80,21 @@
 
 ## 使用示例
 
 消息事件处理例子
 ```python
 # import os
 # os.environ["WXHOOK_LOG_LEVEL"] = "INFO" # 修改日志输出级别
+# os.environ["WXHOOK_LOG_FORMAT"] = "INFO" # 修改日志输出格式
 from wxhook import Bot
 from wxhook import events
 from wxhook.model import Event
 
 
-def on_login(bot: Bot):
+def on_login(bot: Bot, event: Event):
     print("登录成功之后会触发这个函数")
 
 
 def on_start(bot: Bot):
     print("微信客户端打开之后会触发这个函数")
 
 
@@ -135,19 +136,17 @@
 import os
 import json
 
 from wxhook import Bot
 from wxhook import events
 from wxhook.model import Event
 
-# faked_version="3.9.10.19"解除微信低版本登录限制
 bot = Bot()
 
-msgid_list = []
-
+msg_id_list = []
 
 @bot.handle(events.TEXT_MESSAGE)
 def on_text_message(bot: Bot, event: Event):
     self_id = bot.info.wxid
     content = event.content
     sender = event.fromUser
     msg_id = event.msgId
@@ -184,17 +183,17 @@
             bot.send_room_at(sender, ["<wxid1>", "<wxid2>"], "这是一条at群成员的消息")
         elif content.find("发送群聊拍一拍") != -1:
             bot.send_pat(sender, "wxid_vqj81fdula0x22")
         elif content.find("发送私聊拍一拍") != -1:
             bot.send_pat(sender, sender)
         elif content.find("置顶消息") != -1:
             bot.top_msg(msg_id)
-            msgid_list.append(msg_id)
+            msg_id_list.append(msg_id)
         elif content.find("取消置顶的消息") != -1:
-            bot.remove_top_msg(sender, msgid_list.pop())
+            bot.remove_top_msg(sender, msg_id_list.pop())
         elif content.find("获取联系人列表") != -1:
             bot.send_text(sender, json.dumps(bot.get_contacts()))
         elif content.find("获取联系人详情") != -1:
             bot.send_text(sender, json.dumps(bot.get_contact("<wxid>")))
         elif content.find("获取群详情") != -1:
             print(bot.get_room("<chatroomid>"))
         elif content.find("收藏消息") != -1:
```

