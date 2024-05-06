# Comparing `tmp/wxhook-0.0.2.tar.gz` & `tmp/wxhook-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxhook-0.0.2.tar", last modified: Sun May  5 02:59:56 2024, max compression
+gzip compressed data, was "wxhook-0.0.3.tar", last modified: Sun May  5 09:03:32 2024, max compression
```

## Comparing `wxhook-0.0.2.tar` & `wxhook-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 02:59:56.320611 wxhook-0.0.2/
--rw-rw-rw-   0        0        0     1077 2024-05-02 11:25:01.000000 wxhook-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       51 2024-05-04 13:53:50.000000 wxhook-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7199 2024-05-05 02:59:56.319610 wxhook-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6455 2024-05-05 02:40:41.000000 wxhook-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 02:59:56.320611 wxhook-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     3928 2024-05-05 02:59:54.000000 wxhook-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 02:59:56.304133 wxhook-0.0.2/wxhook/
--rw-rw-rw-   0        0        0       44 2024-05-05 02:59:54.000000 wxhook-0.0.2/wxhook/__init__.py
--rw-rw-rw-   0        0        0    16091 2024-05-05 02:58:29.000000 wxhook-0.0.2/wxhook/core.py
--rw-rw-rw-   0        0        0      630 2024-05-03 14:07:48.000000 wxhook-0.0.2/wxhook/events.py
--rw-rw-rw-   0        0        0      273 2024-05-04 13:12:46.000000 wxhook-0.0.2/wxhook/logger.py
--rw-rw-rw-   0        0        0     3826 2024-05-04 13:09:16.000000 wxhook-0.0.2/wxhook/model.py
-drwxrwxrwx   0        0        0        0 2024-05-05 02:59:56.317609 wxhook-0.0.2/wxhook/tools/
--rw-rw-rw-   0        0        0       22 2024-05-05 02:55:57.000000 wxhook-0.0.2/wxhook/tools/config.ini
--rwxrwxrwx   0        0        0   270336 2024-05-01 02:42:10.000000 wxhook-0.0.2/wxhook/tools/faker.exe
--rwxrwxrwx   0        0        0   911872 2024-05-02 10:39:06.000000 wxhook-0.0.2/wxhook/tools/start-wechat.exe
--rw-rw-rw-   0        0        0   592384 2024-04-30 08:39:12.000000 wxhook-0.0.2/wxhook/tools/wxhook.dll
--rw-rw-rw-   0        0        0      103 2024-05-05 02:55:57.000000 wxhook-0.0.2/wxhook/tools/wxhook.json
--rw-rw-rw-   0        0        0     3304 2024-05-04 13:12:46.000000 wxhook-0.0.2/wxhook/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-05 02:59:56.318609 wxhook-0.0.2/wxhook.egg-info/
--rw-rw-rw-   0        0        0     7199 2024-05-05 02:59:56.000000 wxhook-0.0.2/wxhook.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-05 02:59:56.000000 wxhook-0.0.2/wxhook.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 02:59:56.000000 wxhook-0.0.2/wxhook.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-05 02:59:56.000000 wxhook-0.0.2/wxhook.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-05 02:59:56.000000 wxhook-0.0.2/wxhook.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 09:03:32.742483 wxhook-0.0.3/
+-rw-rw-rw-   0        0        0     1077 2024-05-02 11:25:01.000000 wxhook-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-05-04 13:53:50.000000 wxhook-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7199 2024-05-05 09:03:32.742483 wxhook-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6455 2024-05-05 02:40:41.000000 wxhook-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 09:03:32.743483 wxhook-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     3928 2024-05-05 09:00:07.000000 wxhook-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 09:03:32.730401 wxhook-0.0.3/wxhook/
+-rw-rw-rw-   0        0        0       44 2024-05-05 09:00:07.000000 wxhook-0.0.3/wxhook/__init__.py
+-rw-rw-rw-   0        0        0    16124 2024-05-05 08:58:11.000000 wxhook-0.0.3/wxhook/core.py
+-rw-rw-rw-   0        0        0      630 2024-05-03 14:07:48.000000 wxhook-0.0.3/wxhook/events.py
+-rw-rw-rw-   0        0        0      273 2024-05-04 13:12:46.000000 wxhook-0.0.3/wxhook/logger.py
+-rw-rw-rw-   0        0        0     4146 2024-05-05 08:57:27.000000 wxhook-0.0.3/wxhook/model.py
+drwxrwxrwx   0        0        0        0 2024-05-05 09:03:32.739483 wxhook-0.0.3/wxhook/tools/
+-rwxrwxrwx   0        0        0   270336 2024-05-01 02:42:10.000000 wxhook-0.0.3/wxhook/tools/faker.exe
+-rwxrwxrwx   0        0        0   911872 2024-05-02 10:39:06.000000 wxhook-0.0.3/wxhook/tools/start-wechat.exe
+-rw-rw-rw-   0        0        0   592384 2024-04-30 08:39:12.000000 wxhook-0.0.3/wxhook/tools/wxhook.dll
+-rw-rw-rw-   0        0        0     3304 2024-05-04 13:12:46.000000 wxhook-0.0.3/wxhook/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-05 09:03:32.741483 wxhook-0.0.3/wxhook.egg-info/
+-rw-rw-rw-   0        0        0     7199 2024-05-05 09:03:32.000000 wxhook-0.0.3/wxhook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2024-05-05 09:03:32.000000 wxhook-0.0.3/wxhook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 09:03:32.000000 wxhook-0.0.3/wxhook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-05 09:03:32.000000 wxhook-0.0.3/wxhook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-05 09:03:32.000000 wxhook-0.0.3/wxhook.egg-info/top_level.txt
```

### Comparing `wxhook-0.0.2/LICENSE` & `wxhook-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.2/PKG-INFO` & `wxhook-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhook
-Version: 0.0.2
+Version: 0.0.3
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhook
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `wxhook-0.0.2/README.md` & `wxhook-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.2/setup.py` & `wxhook-0.0.3/setup.py`

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
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'loguru',
     'psutil',
     'pyee',
     'requests',
```

### Comparing `wxhook-0.0.2/wxhook/core.py` & `wxhook-0.0.3/wxhook/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     def __init__(
         self,
         on_login: typing.Callable = None,
         on_before_message: typing.Callable = None,
         on_after_message: typing.Callable = None,
         on_start: typing.Callable = None,
         on_stop: typing.Callable = None,
-        faked_version: typing.Union[str, None] = None
+        faked_version: typing.Optional[str] = None
     ):
         self.version = "3.9.5.81"
         self.server_host = "127.0.0.1"
         self.remote_host = "127.0.0.1"
         self.on_start = on_start
         self.on_login = on_login
         self.on_before_message = on_before_message
@@ -435,14 +435,15 @@
             self.call_hook_func(self.on_before_message, self, event)
             self.event_emitter.emit(str(ALL_MESSAGE), self, event)
             self.event_emitter.emit(str(event.type), self, event)
             self.call_hook_func(self.on_after_message, self, event)
             self.webhook(data)
         except Exception:
             logger.error(traceback.format_exc())
+            logger.error(raw_data)
 
     def handle(self, events: typing.Union[list[str], str, None] = None, once: bool = False):
         def wrapper(func):
             listen = self.event_emitter.on if not once else self.event_emitter.once
             if not events:
                 listen(str(ALL_MESSAGE), func)
             else:
```

### Comparing `wxhook-0.0.2/wxhook/events.py` & `wxhook-0.0.3/wxhook/events.py`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.2/wxhook/model.py` & `wxhook-0.0.3/wxhook/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -74,26 +74,27 @@
 
     __str__ = __repr__
 
 
 @dataclass
 class Event:
     """消息事件"""
-    content: typing.Any  # 消息内容，可能包含用户ID和冒号之后的文本内容
-    createTime: int  # 消息创建时间的UNIX时间戳
-    displayFullContent: str  # 完整的消息内容，如果有的话
-    fromUser: str  # 发送消息的用户或群组ID
-    msgId: int  # 消息的唯一标识符
-    msgSequence: int  # 消息序列号
-    pid: int  # 消息的PID
-    signature: str  # 消息签名，包含一系列的配置信息
-    toUser: str  # 消息接收者的用户ID
-    type: int  # 消息类型
-    rawData: RawData  # 原始数据
-    base64Img: typing.Union[str, None] = None  # 图片base64
+    content: typing.Optional[typing.Any] = None  # 消息内容，可能包含用户ID和冒号之后的文本内容
+    base64Img: typing.Optional[str] = None  # 图片base64
+    data: typing.Optional[list] = None  # 朋友圈数据
+    createTime: typing.Optional[int] = None  # 消息创建时间的UNIX时间戳
+    displayFullContent: typing.Optional[str] = None  # 完整的消息内容，如果有的话
+    fromUser: typing.Optional[str] = None  # 发送消息的用户或群组ID
+    msgId: typing.Optional[int] = None  # 消息的唯一标识符
+    msgSequence: typing.Optional[int] = None  # 消息序列号
+    pid: typing.Optional[int] = None  # 消息的PID
+    signature: typing.Optional[str] = None  # 消息签名，包含一系列的配置信息
+    toUser: typing.Optional[str] = None  # 消息接收者的用户ID
+    type: typing.Optional[int] = None  # 消息类型
+    rawData: typing.Optional[RawData] = None  # 原始数据
 
 
 @dataclass
 class Table:
     """表结构"""
     name: str  # 任务名称
     rootpage: str  # 根页面
```

### Comparing `wxhook-0.0.2/wxhook/tools/faker.exe` & `wxhook-0.0.3/wxhook/tools/faker.exe`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.2/wxhook/tools/start-wechat.exe` & `wxhook-0.0.3/wxhook/tools/start-wechat.exe`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.2/wxhook/tools/wxhook.dll` & `wxhook-0.0.3/wxhook/tools/wxhook.dll`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.2/wxhook/utils.py` & `wxhook-0.0.3/wxhook/utils.py`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.2/wxhook.egg-info/PKG-INFO` & `wxhook-0.0.3/wxhook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhook
-Version: 0.0.2
+Version: 0.0.3
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhook
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

