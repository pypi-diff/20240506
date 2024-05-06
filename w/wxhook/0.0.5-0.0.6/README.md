# Comparing `tmp/wxhook-0.0.5.tar.gz` & `tmp/wxhook-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxhook-0.0.5.tar", last modified: Mon May  6 10:02:26 2024, max compression
+gzip compressed data, was "wxhook-0.0.6.tar", last modified: Mon May  6 11:41:26 2024, max compression
```

## Comparing `wxhook-0.0.5.tar` & `wxhook-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 10:02:26.369561 wxhook-0.0.5/
--rw-rw-rw-   0        0        0     1077 2024-05-06 06:49:40.000000 wxhook-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       51 2024-05-06 09:07:02.000000 wxhook-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6719 2024-05-06 10:02:26.368558 wxhook-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5975 2024-05-06 10:02:18.000000 wxhook-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-06 10:02:26.369561 wxhook-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     3928 2024-05-06 09:15:12.000000 wxhook-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 10:02:26.346001 wxhook-0.0.5/wxhook/
--rw-rw-rw-   0        0        0       44 2024-05-06 08:41:27.000000 wxhook-0.0.5/wxhook/__init__.py
--rw-rw-rw-   0        0        0    16255 2024-05-06 08:41:27.000000 wxhook-0.0.5/wxhook/core.py
--rw-rw-rw-   0        0        0      630 2024-05-06 06:49:40.000000 wxhook-0.0.5/wxhook/events.py
--rw-rw-rw-   0        0        0      310 2024-05-06 08:37:49.000000 wxhook-0.0.5/wxhook/logger.py
--rw-rw-rw-   0        0        0     3930 2024-05-06 07:14:37.000000 wxhook-0.0.5/wxhook/model.py
-drwxrwxrwx   0        0        0        0 2024-05-06 10:02:26.364486 wxhook-0.0.5/wxhook/tools/
--rwxrwxrwx   0        0        0   270336 2024-05-06 06:49:40.000000 wxhook-0.0.5/wxhook/tools/faker.exe
--rwxrwxrwx   0        0        0   911872 2024-05-06 06:49:40.000000 wxhook-0.0.5/wxhook/tools/start-wechat.exe
--rw-rw-rw-   0        0        0   592384 2024-05-06 06:49:40.000000 wxhook-0.0.5/wxhook/tools/wxhook.dll
--rw-rw-rw-   0        0        0     3749 2024-05-06 08:35:25.000000 wxhook-0.0.5/wxhook/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-06 10:02:26.360423 wxhook-0.0.5/wxhook.egg-info/
--rw-rw-rw-   0        0        0     6719 2024-05-06 10:02:26.000000 wxhook-0.0.5/wxhook.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2024-05-06 10:02:26.000000 wxhook-0.0.5/wxhook.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 10:02:26.000000 wxhook-0.0.5/wxhook.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-06 10:02:26.000000 wxhook-0.0.5/wxhook.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-06 10:02:26.000000 wxhook-0.0.5/wxhook.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 11:41:26.092171 wxhook-0.0.6/
+-rw-rw-rw-   0        0        0     1077 2024-05-06 06:49:40.000000 wxhook-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-05-06 09:07:02.000000 wxhook-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3397 2024-05-06 11:41:26.092171 wxhook-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2653 2024-05-06 10:56:59.000000 wxhook-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 11:41:26.093174 wxhook-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     3928 2024-05-06 11:41:17.000000 wxhook-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:41:26.067622 wxhook-0.0.6/wxhook/
+-rw-rw-rw-   0        0        0       44 2024-05-06 11:41:17.000000 wxhook-0.0.6/wxhook/__init__.py
+-rw-rw-rw-   0        0        0    16311 2024-05-06 11:32:10.000000 wxhook-0.0.6/wxhook/core.py
+-rw-rw-rw-   0        0        0      630 2024-05-06 06:49:40.000000 wxhook-0.0.6/wxhook/events.py
+-rw-rw-rw-   0        0        0      310 2024-05-06 08:37:49.000000 wxhook-0.0.6/wxhook/logger.py
+-rw-rw-rw-   0        0        0     3930 2024-05-06 07:14:37.000000 wxhook-0.0.6/wxhook/model.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:41:26.090011 wxhook-0.0.6/wxhook/tools/
+-rwxrwxrwx   0        0        0   270336 2024-05-06 06:49:40.000000 wxhook-0.0.6/wxhook/tools/faker.exe
+-rwxrwxrwx   0        0        0   911872 2024-05-06 06:49:40.000000 wxhook-0.0.6/wxhook/tools/start-wechat.exe
+-rw-rw-rw-   0        0        0   592384 2024-05-06 06:49:40.000000 wxhook-0.0.6/wxhook/tools/wxhook.dll
+-rw-rw-rw-   0        0        0     3763 2024-05-06 11:32:10.000000 wxhook-0.0.6/wxhook/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:41:26.086893 wxhook-0.0.6/wxhook.egg-info/
+-rw-rw-rw-   0        0        0     3397 2024-05-06 11:41:26.000000 wxhook-0.0.6/wxhook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2024-05-06 11:41:26.000000 wxhook-0.0.6/wxhook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 11:41:26.000000 wxhook-0.0.6/wxhook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-06 11:41:26.000000 wxhook-0.0.6/wxhook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-06 11:41:26.000000 wxhook-0.0.6/wxhook.egg-info/top_level.txt
```

### Comparing `wxhook-0.0.5/LICENSE` & `wxhook-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.5/setup.py` & `wxhook-0.0.6/setup.py`

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
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'loguru',
     'psutil',
     'pyee',
     'requests',
```

### Comparing `wxhook-0.0.5/wxhook/core.py` & `wxhook-0.0.6/wxhook/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,15 @@
             "jsonParam": json_param,
             "headImgUrl": head_img_url,
             "mainImg": main_img,
             "indexPage": index_page
         }
         return Response(**self.call_api("/api/sendApplet", json=data))
 
-    def send_room_at(self, room_id: str, wxids: list[str], msg: str) -> Response:
+    def send_room_at(self, room_id: str, wxids: typing.List[str], msg: str) -> Response:
         """发送群@消息"""
         data = {
             "chatRoomId": room_id,
             "wxids": ",".join(wxids),
             "msg": msg
         }
         return Response(**self.call_api("/api/sendAtText", json=data))
@@ -223,26 +223,26 @@
         """发送拍一拍消息"""
         data = {
             "receiver": room_id,
             "wxid": wxid
         }
         return Response(**self.call_api("/api/sendPatMsg", json=data))
 
-    def get_contacts(self) -> list[Contact]:
+    def get_contacts(self) -> typing.List[Contact]:
         """获取联系人列表"""
         return [Contact(**item) for item in self.call_api("/api/getContactList")["data"]]
 
     def get_contact(self, wxid: str) -> ContactDetail:
         """获取联系人详情"""
         data = {
             "wxid": wxid
         }
         return ContactDetail(**self.call_api("/api/getContactProfile", json=data)["data"])
 
-    def create_room(self, member_ids: list[str]) -> Response:
+    def create_room(self, member_ids: typing.List[str]) -> Response:
         """创建群聊"""
         data = {
             "memberIds": ",".join(member_ids)
         }
         return Response(**self.call_api("/api/createChatRoom", json=data))
 
     def quit_room(self, room_id: str) -> Response:
@@ -262,31 +262,31 @@
     def get_room_members(self, room_id: str) -> RoomMembers:
         """获取群成员列表"""
         data = {
             "chatRoomId": room_id
         }
         return RoomMembers(**self.call_api("/api/getMemberFromChatRoom", json=data)["data"])
 
-    def add_room_member(self, room_id: str, member_ids: list[str]) -> Response:
+    def add_room_member(self, room_id: str, member_ids: typing.List[str]) -> Response:
         """添加群成员"""
         data = {
             "chatRoomId": room_id,
             "memberIds": ",".join(member_ids)
         }
         return Response(**self.call_api("/api/addMemberToChatRoom", json=data))
 
-    def delete_room_member(self, room_id: str, member_ids: list[str]) -> Response:
+    def delete_room_member(self, room_id: str, member_ids: typing.List[str]) -> Response:
         """删除群成员"""
         data = {
             "chatRoomId": room_id,
             "memberIds": ",".join(member_ids)
         }
         return Response(**self.call_api("/api/delMemberFromChatRoom", json=data))
 
-    def invite_room_member(self, room_id: str, member_ids: list[str]) -> Response:
+    def invite_room_member(self, room_id: str, member_ids: typing.List[str]) -> Response:
         """邀请群成员"""
         data = {
             "chatRoomId": room_id,
             "memberIds": ",".join(member_ids)
         }
         return Response(**self.call_api("/api/InviteMemberToChatRoom", json=data))
 
@@ -404,15 +404,15 @@
     def ocr(self, image_path: str) -> Response:
         """图片文本识别"""
         data = {
             "imagePath": image_path
         }
         return Response(**self.call_api("/api/ocr", json=data))
 
-    def get_db_info(self) -> list[DB]:
+    def get_db_info(self) -> typing.List[DB]:
         """获取数据库句柄"""
         return [DB(databaseName=item["databaseName"], handle=item["handle"],
                    tables=[Table(**sub_item) for sub_item in item["tables"]]) for item in self.call_api("/api/getDBInfo")]
 
     def exec_sql(self, db_handle: int, sql: str) -> Response:
         """执行SQL命令"""
         data = {
@@ -439,15 +439,15 @@
             self.event_emitter.emit(str(event.type), self, event)
             self.call_hook_func(self.on_after_message, self, event)
             self.webhook(data)
         except Exception:
             logger.error(traceback.format_exc())
             logger.error(raw_data)
 
-    def handle(self, events: typing.Union[list[str], str, None] = None, once: bool = False) -> typing.Callable[[typing.Callable], None]:
+    def handle(self, events: typing.Union[typing.List[str], str, None] = None, once: bool = False) -> typing.Callable[[typing.Callable], None]:
         def wrapper(func):
             listen = self.event_emitter.on if not once else self.event_emitter.once
             if not events:
                 listen(str(ALL_MESSAGE), func)
             else:
                 for event in events if isinstance(events, list) else [events]:
                     listen(str(event), func)
```

### Comparing `wxhook-0.0.5/wxhook/events.py` & `wxhook-0.0.6/wxhook/events.py`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.5/wxhook/model.py` & `wxhook-0.0.6/wxhook/model.py`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.5/wxhook/tools/faker.exe` & `wxhook-0.0.6/wxhook/tools/faker.exe`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.5/wxhook/tools/start-wechat.exe` & `wxhook-0.0.6/wxhook/tools/start-wechat.exe`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.5/wxhook/tools/wxhook.dll` & `wxhook-0.0.6/wxhook/tools/wxhook.dll`

 * *Files identical despite different names*

### Comparing `wxhook-0.0.5/wxhook/utils.py` & `wxhook-0.0.6/wxhook/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 def fake_wechat_version(pid: int, old_version: str, new_version: str) -> int:
     result = subprocess.run(f"{FAKER} {pid} {old_version} {new_version}", capture_output=True, text=True)
     return int(result.stdout)
 
 
-def get_processes(process_name: str) -> list[psutil.Process]:
+def get_processes(process_name: str) -> typing.List[psutil.Process]:
     processes = []
     for process in psutil.process_iter():
         if process.name().lower() == process_name.lower():
             processes.append(process)
     return processes
 
 
@@ -76,15 +76,15 @@
             data = json.load(file)
         return data
 
     def write(self, data: dict) -> None:
         with open(self.filename, "w", encoding="utf-8") as file:
             json.dump(data, file)
 
-    def refresh(self, pid_list: list[int]) -> None:
+    def refresh(self, pid_list: typing.List[int]) -> None:
         data = self.read()
         cleaned_data = []
         remote_port_list = [19000]
         for item in data["wechat"]:
             if item["pid"] in pid_list:
                 remote_port_list.append(item["remote_port"])
                 cleaned_data.append(item)
```

