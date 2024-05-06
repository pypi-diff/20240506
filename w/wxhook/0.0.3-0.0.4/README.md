# Comparing `tmp/wxhook-0.0.3.tar.gz` & `tmp/wxhook-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxhook-0.0.3.tar", last modified: Sun May  5 09:03:32 2024, max compression
+gzip compressed data, was "wxhook-0.0.4.tar", last modified: Mon May  6 08:26:04 2024, max compression
```

## Comparing `wxhook-0.0.3.tar` & `wxhook-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 09:03:32.742483 wxhook-0.0.3/
--rw-rw-rw-   0        0        0     1077 2024-05-02 11:25:01.000000 wxhook-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       51 2024-05-04 13:53:50.000000 wxhook-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     7199 2024-05-05 09:03:32.742483 wxhook-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6455 2024-05-05 02:40:41.000000 wxhook-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 09:03:32.743483 wxhook-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     3928 2024-05-05 09:00:07.000000 wxhook-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 09:03:32.730401 wxhook-0.0.3/wxhook/
--rw-rw-rw-   0        0        0       44 2024-05-05 09:00:07.000000 wxhook-0.0.3/wxhook/__init__.py
--rw-rw-rw-   0        0        0    16124 2024-05-05 08:58:11.000000 wxhook-0.0.3/wxhook/core.py
--rw-rw-rw-   0        0        0      630 2024-05-03 14:07:48.000000 wxhook-0.0.3/wxhook/events.py
--rw-rw-rw-   0        0        0      273 2024-05-04 13:12:46.000000 wxhook-0.0.3/wxhook/logger.py
--rw-rw-rw-   0        0        0     4146 2024-05-05 08:57:27.000000 wxhook-0.0.3/wxhook/model.py
-drwxrwxrwx   0        0        0        0 2024-05-05 09:03:32.739483 wxhook-0.0.3/wxhook/tools/
--rwxrwxrwx   0        0        0   270336 2024-05-01 02:42:10.000000 wxhook-0.0.3/wxhook/tools/faker.exe
--rwxrwxrwx   0        0        0   911872 2024-05-02 10:39:06.000000 wxhook-0.0.3/wxhook/tools/start-wechat.exe
--rw-rw-rw-   0        0        0   592384 2024-04-30 08:39:12.000000 wxhook-0.0.3/wxhook/tools/wxhook.dll
--rw-rw-rw-   0        0        0     3304 2024-05-04 13:12:46.000000 wxhook-0.0.3/wxhook/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-05 09:03:32.741483 wxhook-0.0.3/wxhook.egg-info/
--rw-rw-rw-   0        0        0     7199 2024-05-05 09:03:32.000000 wxhook-0.0.3/wxhook.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2024-05-05 09:03:32.000000 wxhook-0.0.3/wxhook.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 09:03:32.000000 wxhook-0.0.3/wxhook.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-05 09:03:32.000000 wxhook-0.0.3/wxhook.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-05 09:03:32.000000 wxhook-0.0.3/wxhook.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 08:26:04.649679 wxhook-0.0.4/
+-rw-rw-rw-   0        0        0     1077 2024-05-06 06:49:40.000000 wxhook-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-05-06 06:49:40.000000 wxhook-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6695 2024-05-06 08:26:04.648677 wxhook-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5951 2024-05-06 07:42:05.000000 wxhook-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 08:26:04.649679 wxhook-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     3928 2024-05-06 07:49:01.000000 wxhook-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:26:04.631300 wxhook-0.0.4/wxhook/
+-rw-rw-rw-   0        0        0       44 2024-05-06 07:49:01.000000 wxhook-0.0.4/wxhook/__init__.py
+-rw-rw-rw-   0        0        0    16187 2024-05-06 08:10:05.000000 wxhook-0.0.4/wxhook/core.py
+-rw-rw-rw-   0        0        0      630 2024-05-06 06:49:40.000000 wxhook-0.0.4/wxhook/events.py
+-rw-rw-rw-   0        0        0      273 2024-05-06 06:49:40.000000 wxhook-0.0.4/wxhook/logger.py
+-rw-rw-rw-   0        0        0     3930 2024-05-06 07:14:37.000000 wxhook-0.0.4/wxhook/model.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:26:04.644541 wxhook-0.0.4/wxhook/tools/
+-rwxrwxrwx   0        0        0   270336 2024-05-06 06:49:40.000000 wxhook-0.0.4/wxhook/tools/faker.exe
+-rwxrwxrwx   0        0        0   911872 2024-05-06 06:49:40.000000 wxhook-0.0.4/wxhook/tools/start-wechat.exe
+-rw-rw-rw-   0        0        0   592384 2024-05-06 06:49:40.000000 wxhook-0.0.4/wxhook/tools/wxhook.dll
+-rw-rw-rw-   0        0        0     3566 2024-05-06 08:06:43.000000 wxhook-0.0.4/wxhook/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:26:04.640473 wxhook-0.0.4/wxhook.egg-info/
+-rw-rw-rw-   0        0        0     6695 2024-05-06 08:26:04.000000 wxhook-0.0.4/wxhook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2024-05-06 08:26:04.000000 wxhook-0.0.4/wxhook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 08:26:04.000000 wxhook-0.0.4/wxhook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-06 08:26:04.000000 wxhook-0.0.4/wxhook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-06 08:26:04.000000 wxhook-0.0.4/wxhook.egg-info/top_level.txt
```

### Comparing `wxhook-0.0.3/LICENSE` & `wxhook-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.3/PKG-INFO` & `wxhook-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhook
-Version: 0.0.3
+Version: 0.0.4
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhook
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -80,64 +80,55 @@
 
 ## 使用示例
 
 消息事件处理例子
 ```python
 # import os
 # os.environ["WXHOOK_LOG_LEVEL"] = "INFO" # 修改日志输出级别
-import time
-
 from wxhook import Bot
 from wxhook import events
 from wxhook.model import Event
 
 
 def on_login(bot: Bot):
-    bot.send_text("filehelper", "登录成功之后会触发这个函数")
+    print("登录成功之后会触发这个函数")
 
 
 def on_start(bot: Bot):
     print("微信客户端打开之后会触发这个函数")
 
 
 def on_stop(bot: Bot):
-    bot.send_text("filehelper", "关闭微信客户端之前会触发这个函数")
-    time.sleep(1)  # 防止客户端关闭太快导致消息发送失败
+    print("关闭微信客户端之前会触发这个函数")
+
+
+def on_before_message(bot: Bot, event: Event):
+    print("消息事件处理之前")
+
+
+def on_after_message(bot: Bot, event: Event):
+    print("消息事件处理之后")
 
 
 bot = Bot(
+    # faked_version="3.9.10.19", # 解除微信低版本限制
     on_login=on_login,
     on_start=on_start,
-    on_stop=on_stop
+    on_stop=on_stop,
+    on_before_message=on_before_message,
+    on_after_message=on_after_message
 )
 
 
 # 消息回调地址
 # bot.set_webhook_url("http://127.0.0.1:8000")
 
-@bot.handle(events.TEXT_MESSAGE, once=True)
-def on_message(bot: Bot, event: Event):
-    bot.send_text("filehelper", "这条消息只会发送一次哦")
-
-
 @bot.handle(events.TEXT_MESSAGE)
 def on_message(bot: Bot, event: Event):
-    if event.fromUser != bot.info.wxid:
-        bot.send_text(event.fromUser, event.content)
-
-
-@bot.handle([events.IMAGE_MESSAGE, events.EMOJI_MESSAGE, events.VIDEO_MESSAGE])
-def on_message(bot: Bot, event: Event):
-    if event.fromUser != bot.info.wxid:
-        if event.type == events.IMAGE_MESSAGE:
-            bot.send_text(event.fromUser, "图片消息")
-        elif event.type == events.EMOJI_MESSAGE:
-            bot.send_text(event.fromUser, "表情消息")
-        elif event.type == events.VIDEO_MESSAGE:
-            bot.send_text(event.fromUser, "视频消息")
+    bot.send_text("filehelper", "hello world!")
 
 
 bot.run()
 ```
 
 接口使用例子
 ```python
```

### Comparing `wxhook-0.0.3/README.md` & `wxhook-0.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -56,64 +56,55 @@
 
 ## 使用示例
 
 消息事件处理例子
 ```python
 # import os
 # os.environ["WXHOOK_LOG_LEVEL"] = "INFO" # 修改日志输出级别
-import time
-
 from wxhook import Bot
 from wxhook import events
 from wxhook.model import Event
 
 
 def on_login(bot: Bot):
-    bot.send_text("filehelper", "登录成功之后会触发这个函数")
+    print("登录成功之后会触发这个函数")
 
 
 def on_start(bot: Bot):
     print("微信客户端打开之后会触发这个函数")
 
 
 def on_stop(bot: Bot):
-    bot.send_text("filehelper", "关闭微信客户端之前会触发这个函数")
-    time.sleep(1)  # 防止客户端关闭太快导致消息发送失败
+    print("关闭微信客户端之前会触发这个函数")
+
+
+def on_before_message(bot: Bot, event: Event):
+    print("消息事件处理之前")
+
+
+def on_after_message(bot: Bot, event: Event):
+    print("消息事件处理之后")
 
 
 bot = Bot(
+    # faked_version="3.9.10.19", # 解除微信低版本限制
     on_login=on_login,
     on_start=on_start,
-    on_stop=on_stop
+    on_stop=on_stop,
+    on_before_message=on_before_message,
+    on_after_message=on_after_message
 )
 
 
 # 消息回调地址
 # bot.set_webhook_url("http://127.0.0.1:8000")
 
-@bot.handle(events.TEXT_MESSAGE, once=True)
-def on_message(bot: Bot, event: Event):
-    bot.send_text("filehelper", "这条消息只会发送一次哦")
-
-
 @bot.handle(events.TEXT_MESSAGE)
 def on_message(bot: Bot, event: Event):
-    if event.fromUser != bot.info.wxid:
-        bot.send_text(event.fromUser, event.content)
-
-
-@bot.handle([events.IMAGE_MESSAGE, events.EMOJI_MESSAGE, events.VIDEO_MESSAGE])
-def on_message(bot: Bot, event: Event):
-    if event.fromUser != bot.info.wxid:
-        if event.type == events.IMAGE_MESSAGE:
-            bot.send_text(event.fromUser, "图片消息")
-        elif event.type == events.EMOJI_MESSAGE:
-            bot.send_text(event.fromUser, "表情消息")
-        elif event.type == events.VIDEO_MESSAGE:
-            bot.send_text(event.fromUser, "视频消息")
+    bot.send_text("filehelper", "hello world!")
 
 
 bot.run()
 ```
 
 接口使用例子
 ```python
```

### Comparing `wxhook-0.0.3/setup.py` & `wxhook-0.0.4/setup.py`

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
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'loguru',
     'psutil',
     'pyee',
     'requests',
```

### Comparing `wxhook-0.0.3/wxhook/core.py` & `wxhook-0.0.4/wxhook/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import socketserver
 from functools import lru_cache
 
 import psutil
 import pyee
 import requests
 
-from .events import ALL_MESSAGE, SYSTEM_MESSAGE
+from .events import ALL_MESSAGE
 from .logger import logger
-from .model import RawData, Event, Account, Contact, ContactDetail, Room, RoomMembers, Table, DB, Response
-from .utils import WeChatManager, start_wechat_with_inject, fake_wechat_version, parse_event
+from .model import Event, Account, Contact, ContactDetail, Room, RoomMembers, Table, DB, Response
+from .utils import WeChatManager, start_wechat_with_inject, fake_wechat_version, get_pid, parse_event
 
 
 class RequestHandler(socketserver.BaseRequestHandler):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def handle(self):
@@ -64,45 +64,47 @@
         self.webhook_url = None
         self.DATA_SAVE_PATH = None
         self.WXHELPER_PATH = None
         self.FILE_SAVE_PATH = None
         self.IMAGE_SAVE_PATH = None
         self.VIDEO_SAVE_PATH = None
 
-        code, output = start_wechat_with_inject(self.remote_port)
-        if code == 1:
-            raise Exception(output)
+        try:
+            code, output = start_wechat_with_inject(self.remote_port)
+            if code == 1:
+                raise Exception(output)
+        except Exception:
+            output = get_pid(self.remote_port)
 
         self.process = psutil.Process(int(output))
 
         if self.faked_version is not None:
             if fake_wechat_version(self.process.pid, self.version, faked_version) == 0:
-                logger.info(f"wechat version faked: {self.version} -> {faked_version}")
+                logger.success(f"wechat version faked: {self.version} -> {faked_version}")
             else:
-                logger.info(f"wechat version fake failed.")
+                logger.error(f"wechat version fake failed.")
 
+        logger.info(f"API Server at 0.0.0.0:{self.remote_port}")
         self.wechat_manager.add(self.process.pid, self.remote_port, self.server_port)
-
         self.call_hook_func(self.on_start, self)
-        self.handle(SYSTEM_MESSAGE, once=True)(self.init_bot)
+        self.handle(ALL_MESSAGE, once=True)(self.init_bot)
         self.hook_sync_msg(self.server_host, self.server_port)
 
     @staticmethod
     def call_hook_func(func: typing.Callable, *args, **kwargs) -> typing.Any:
         if callable(func):
             return func(*args, **kwargs)
 
     def init_bot(self, bot: "Bot", event: Event) -> None:
-        if event.content["sysmsg"]["@type"] == "SafeModuleCfg":
-            self.DATA_SAVE_PATH = bot.info.dataSavePath
-            self.WXHELPER_PATH = os.path.join(self.DATA_SAVE_PATH, "wxhelper")
-            self.FILE_SAVE_PATH = os.path.join(self.WXHELPER_PATH, "file")
-            self.IMAGE_SAVE_PATH = os.path.join(self.WXHELPER_PATH, "image")
-            self.VIDEO_SAVE_PATH = os.path.join(self.WXHELPER_PATH, "video")
-            self.call_hook_func(self.on_login, bot)
+        self.DATA_SAVE_PATH = bot.info.dataSavePath
+        self.WXHELPER_PATH = os.path.join(self.DATA_SAVE_PATH, "wxhelper")
+        self.FILE_SAVE_PATH = os.path.join(self.WXHELPER_PATH, "file")
+        self.IMAGE_SAVE_PATH = os.path.join(self.WXHELPER_PATH, "image")
+        self.VIDEO_SAVE_PATH = os.path.join(self.WXHELPER_PATH, "video")
+        self.call_hook_func(self.on_login, bot, event)
 
     def set_webhook_url(self, webhook_url: str) -> None:
         self.webhook_url = webhook_url
 
     def webhook(self, event: dict) -> None:
         if self.webhook_url is not None:
             try:
@@ -405,15 +407,15 @@
             "imagePath": image_path
         }
         return Response(**self.call_api("/api/ocr", json=data))
 
     def get_db_info(self) -> list[DB]:
         """获取数据库句柄"""
         return [DB(databaseName=item["databaseName"], handle=item["handle"],
-                   tables=[Table(**subitem) for subitem in item["tables"]]) for item in self.call_api("/api/getDBInfo")]
+                   tables=[Table(**sub_item) for sub_item in item["tables"]]) for item in self.call_api("/api/getDBInfo")]
 
     def exec_sql(self, db_handle: int, sql: str) -> Response:
         """执行SQL命令"""
         data = {
             "dbHandle": db_handle,
             "sql": sql
         }
@@ -426,15 +428,15 @@
     @property
     def info(self) -> Account:
         return self.get_self_info()
 
     def on_event(self, raw_data: bytes):
         try:
             data = json.loads(raw_data)
-            event = Event(**parse_event(data), rawData=RawData(raw_data))
+            event = Event(**parse_event(data))
             logger.debug(event)
             self.call_hook_func(self.on_before_message, self, event)
             self.event_emitter.emit(str(ALL_MESSAGE), self, event)
             self.event_emitter.emit(str(event.type), self, event)
             self.call_hook_func(self.on_after_message, self, event)
             self.webhook(data)
         except Exception:
@@ -456,11 +458,11 @@
         self.call_hook_func(self.on_stop, self)
         self.process.terminate()
 
     def run(self):
         try:
             server = socketserver.ThreadingTCPServer((self.server_host, self.server_port), RequestHandler)
             server.bot = self
-            logger.info(f"{self.server_host}:{self.server_port}")
+            logger.info(f"Listening Server at {self.server_host}:{self.server_port}")
             server.serve_forever()
         except (KeyboardInterrupt, SystemExit):
             self.exit()
```

### Comparing `wxhook-0.0.3/wxhook/events.py` & `wxhook-0.0.4/wxhook/events.py`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.3/wxhook/model.py` & `wxhook-0.0.4/wxhook/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,40 +61,28 @@
     adminNickname: str  # 聊天室管理员的昵称
     chatRoomId: str  # 聊天室的ID
     memberNickname: str  # 正在提及的成员昵称，可能包含特殊字符作为昵称的一部分
     members: str  # 聊天室成员的微信ID列表，各ID之间使用特定字符分隔
 
 
 @dataclass
-class RawData:
-    """原始数据"""
-    data: bytes
-
-    def __repr__(self):
-        return "<RawData>"
-
-    __str__ = __repr__
-
-
-@dataclass
 class Event:
     """消息事件"""
     content: typing.Optional[typing.Any] = None  # 消息内容，可能包含用户ID和冒号之后的文本内容
     base64Img: typing.Optional[str] = None  # 图片base64
     data: typing.Optional[list] = None  # 朋友圈数据
     createTime: typing.Optional[int] = None  # 消息创建时间的UNIX时间戳
     displayFullContent: typing.Optional[str] = None  # 完整的消息内容，如果有的话
     fromUser: typing.Optional[str] = None  # 发送消息的用户或群组ID
     msgId: typing.Optional[int] = None  # 消息的唯一标识符
     msgSequence: typing.Optional[int] = None  # 消息序列号
     pid: typing.Optional[int] = None  # 消息的PID
     signature: typing.Optional[str] = None  # 消息签名，包含一系列的配置信息
     toUser: typing.Optional[str] = None  # 消息接收者的用户ID
     type: typing.Optional[int] = None  # 消息类型
-    rawData: typing.Optional[RawData] = None  # 原始数据
 
 
 @dataclass
 class Table:
     """表结构"""
     name: str  # 任务名称
     rootpage: str  # 根页面
```

### Comparing `wxhook-0.0.3/wxhook/tools/faker.exe` & `wxhook-0.0.4/wxhook/tools/faker.exe`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.3/wxhook/tools/start-wechat.exe` & `wxhook-0.0.4/wxhook/tools/start-wechat.exe`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.3/wxhook/tools/wxhook.dll` & `wxhook-0.0.4/wxhook/tools/wxhook.dll`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.3/wxhook/utils.py` & `wxhook-0.0.4/wxhook/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,27 +20,32 @@
 
 
 def fake_wechat_version(pid: int, old_version: str, new_version: str):
     result = subprocess.run(f"{FAKER} {pid} {old_version} {new_version}", capture_output=True, text=True)
     return int(result.stdout)
 
 
-def get_processes(process_name):
+def get_processes(process_name: str):
     processes = []
     for process in psutil.process_iter():
         if process.name().lower() == process_name.lower():
             processes.append(process)
     return processes
 
 
-def parse_xml(xml):
+def get_pid(port: int):
+    output = subprocess.run(f"netstat -ano | findStr \"{port}\"", capture_output=True, text=True, shell=True).stdout
+    return int(output.split("\n")[0].split("LISTENING")[-1])
+
+
+def parse_xml(xml: str):
     return xmltodict.parse(xml)
 
 
-def parse_event(event, fields=None):
+def parse_event(event: dict, fields=None):
     for field in fields or ["content", "signature"]:
         try:
             if field in event:
                 event[field] = parse_xml(event[field])
         except Exception:
             pass
     return event
@@ -66,19 +71,19 @@
             }, file)
 
     def read(self):
         with open(self.filename, "r", encoding="utf-8") as file:
             data = json.load(file)
         return data
 
-    def write(self, data):
+    def write(self, data: dict):
         with open(self.filename, "w", encoding="utf-8") as file:
             json.dump(data, file)
 
-    def refresh(self, pid_list):
+    def refresh(self, pid_list: list[int]):
         data = self.read()
         cleaned_data = []
         remote_port_list = [19000]
         for item in data["wechat"]:
             if item["pid"] in pid_list:
                 remote_port_list.append(item["remote_port"])
                 cleaned_data.append(item)
@@ -91,22 +96,22 @@
         pid_list = [process.pid for process in get_processes("WeChat.exe")]
         self.refresh(pid_list)
 
     def get_remote_port(self):
         data = self.read()
         return data["increase_remote_port"] + 1
 
-    def get_listen_port(self, remote_port):
+    def get_listen_port(self, remote_port: int):
         return 19000 - (remote_port - 19000)
 
     def get_port(self):
         remote_port = self.get_remote_port()
         return remote_port, self.get_listen_port(remote_port)
 
-    def add(self, pid, remote_port, server_port):
+    def add(self, pid: int, remote_port: int, server_port: int):
         data = self.read()
         data["increase_remote_port"] = remote_port
         data["wechat"].append({
             "pid": pid,
             "remote_port": remote_port,
             "server_port": server_port
         })
```

### Comparing `wxhook-0.0.3/wxhook.egg-info/PKG-INFO` & `wxhook-0.0.4/wxhook.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhook
-Version: 0.0.3
+Version: 0.0.4
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhook
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -80,64 +80,55 @@
 
 ## 使用示例
 
 消息事件处理例子
 ```python
 # import os
 # os.environ["WXHOOK_LOG_LEVEL"] = "INFO" # 修改日志输出级别
-import time
-
 from wxhook import Bot
 from wxhook import events
 from wxhook.model import Event
 
 
 def on_login(bot: Bot):
-    bot.send_text("filehelper", "登录成功之后会触发这个函数")
+    print("登录成功之后会触发这个函数")
 
 
 def on_start(bot: Bot):
     print("微信客户端打开之后会触发这个函数")
 
 
 def on_stop(bot: Bot):
-    bot.send_text("filehelper", "关闭微信客户端之前会触发这个函数")
-    time.sleep(1)  # 防止客户端关闭太快导致消息发送失败
+    print("关闭微信客户端之前会触发这个函数")
+
+
+def on_before_message(bot: Bot, event: Event):
+    print("消息事件处理之前")
+
+
+def on_after_message(bot: Bot, event: Event):
+    print("消息事件处理之后")
 
 
 bot = Bot(
+    # faked_version="3.9.10.19", # 解除微信低版本限制
     on_login=on_login,
     on_start=on_start,
-    on_stop=on_stop
+    on_stop=on_stop,
+    on_before_message=on_before_message,
+    on_after_message=on_after_message
 )
 
 
 # 消息回调地址
 # bot.set_webhook_url("http://127.0.0.1:8000")
 
-@bot.handle(events.TEXT_MESSAGE, once=True)
-def on_message(bot: Bot, event: Event):
-    bot.send_text("filehelper", "这条消息只会发送一次哦")
-
-
 @bot.handle(events.TEXT_MESSAGE)
 def on_message(bot: Bot, event: Event):
-    if event.fromUser != bot.info.wxid:
-        bot.send_text(event.fromUser, event.content)
-
-
-@bot.handle([events.IMAGE_MESSAGE, events.EMOJI_MESSAGE, events.VIDEO_MESSAGE])
-def on_message(bot: Bot, event: Event):
-    if event.fromUser != bot.info.wxid:
-        if event.type == events.IMAGE_MESSAGE:
-            bot.send_text(event.fromUser, "图片消息")
-        elif event.type == events.EMOJI_MESSAGE:
-            bot.send_text(event.fromUser, "表情消息")
-        elif event.type == events.VIDEO_MESSAGE:
-            bot.send_text(event.fromUser, "视频消息")
+    bot.send_text("filehelper", "hello world!")
 
 
 bot.run()
 ```
 
 接口使用例子
 ```python
```

