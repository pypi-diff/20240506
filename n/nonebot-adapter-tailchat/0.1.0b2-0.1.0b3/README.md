# Comparing `tmp/nonebot_adapter_tailchat-0.1.0b2.tar.gz` & `tmp/nonebot_adapter_tailchat-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_tailchat-0.1.0b2.tar", max compression
+gzip compressed data, was "nonebot_adapter_tailchat-0.1.0b3.tar", max compression
```

## Comparing `nonebot_adapter_tailchat-0.1.0b2.tar` & `nonebot_adapter_tailchat-0.1.0b3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    11335 2024-05-03 11:48:15.148531 nonebot_adapter_tailchat-0.1.0b2/LICENSE
--rw-r--r--   0        0        0     1189 2024-05-03 11:48:15.148531 nonebot_adapter_tailchat-0.1.0b2/README.md
--rw-r--r--   0        0        0      260 2024-05-03 11:48:15.148531 nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/__init__.py
--rw-r--r--   0        0        0     6259 2024-05-03 11:48:15.148531 nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/adapter.py
--rw-r--r--   0        0        0     6659 2024-05-03 11:48:15.148531 nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/bbcode.py
--rw-r--r--   0        0        0    24667 2024-05-03 11:48:15.148531 nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/bot.py
--rw-r--r--   0        0        0      675 2024-05-03 11:48:15.148531 nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/config.py
--rw-r--r--   0        0        0       26 2024-05-03 11:48:15.148531 nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/const.py
--rw-r--r--   0        0        0     6092 2024-05-03 11:48:15.148531 nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/event.py
--rw-r--r--   0        0        0      761 2024-05-03 11:48:15.148531 nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/exception.py
--rw-r--r--   0        0        0     8557 2024-05-03 11:48:15.148531 nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/message.py
--rw-r--r--   0        0        0     4505 2024-05-03 11:48:15.148531 nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/model.py
--rw-r--r--   0        0        0      374 2024-05-03 11:48:15.148531 nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/permission.py
--rw-r--r--   0        0        0      203 2024-05-03 11:48:15.148531 nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/rule.py
--rw-r--r--   0        0        0     1697 2024-05-03 11:48:15.148531 nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/util.py
--rw-r--r--   0        0        0     1128 2024-05-03 11:48:15.148531 nonebot_adapter_tailchat-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 nonebot_adapter_tailchat-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0    11335 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/LICENSE
+-rw-r--r--   0        0        0     1189 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/README.md
+-rw-r--r--   0        0        0      260 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/__init__.py
+-rw-r--r--   0        0        0     6259 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/adapter.py
+-rw-r--r--   0        0        0    21563 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/api.py
+-rw-r--r--   0        0        0     6659 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/bbcode.py
+-rw-r--r--   0        0        0     3759 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/bot.py
+-rw-r--r--   0        0        0      675 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/config.py
+-rw-r--r--   0        0        0       26 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/const.py
+-rw-r--r--   0        0        0     6135 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/event.py
+-rw-r--r--   0        0        0      761 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/exception.py
+-rw-r--r--   0        0        0     8711 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/message.py
+-rw-r--r--   0        0        0     4505 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/model.py
+-rw-r--r--   0        0        0      374 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/permission.py
+-rw-r--r--   0        0        0      203 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/rule.py
+-rw-r--r--   0        0        0     1697 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/util.py
+-rw-r--r--   0        0        0     1146 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 nonebot_adapter_tailchat-0.1.0b3/PKG-INFO
```

### Comparing `nonebot_adapter_tailchat-0.1.0b2/LICENSE` & `nonebot_adapter_tailchat-0.1.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b2/README.md` & `nonebot_adapter_tailchat-0.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/adapter.py` & `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/bbcode.py` & `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/bbcode.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/bot.py` & `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,158 +1,34 @@
-from base64 import urlsafe_b64decode
-from hashlib import md5
-from json import loads
-from time import time
-from typing import TYPE_CHECKING, Any, Literal, Optional, Union
+from abc import ABC
+from typing import Any, Literal, Optional, Union
 
 from nonebot.adapters import Bot as BaseBot
-from nonebot.message import handle_event
 from pydantic import TypeAdapter
-from socketio import AsyncClient as AsyncSocketClient
-from typing_extensions import override
 
-from .config import BotInfo
-from .event import Event, MessageEvent
-from .message import Message, MessageSegment
+from .message import Message
 from .model import (
     Ack,
-    BaseBotInfo,
     ClientConfig,
     ConverseInfo,
     FileInfo,
     GroupInfo,
     Health,
     InviteCodeInfo,
-    JwtPayload,
     LastMessages,
     MessageRet,
     Panel,
     TokenInfo,
     UserInfo,
     Whoami,
 )
 
-if TYPE_CHECKING:
-    from .adapter import Adapter
-
-
-class Bot(BaseBot):
-    def __str__(self):
-        return f"{self.info.nickname}-{self.self_id}" if self.info else self.self_id
-
-    async def connect(self):
-        return await self.sio.connect(
-            url=self.url,
-            auth={"token": self.base_info.jwt},
-            transports=["websocket"],
-        )
-
-    async def handle_event(self, event: Event) -> None:
-        await handle_event(self, event)
-
-    @staticmethod
-    def md5(text: str) -> str:
-        return md5(text.encode()).hexdigest()
-
-    @staticmethod
-    def decode_jwt(jwt: str) -> tuple[dict, JwtPayload, str]:
-        segments = jwt.split(".")
-        if len(segments) != 3:
-            raise ValueError("Invalid JWT format.")
-
-        return (
-            loads(urlsafe_b64decode(segments[0] + "===").decode("utf-8")),
-            JwtPayload.model_validate(loads(urlsafe_b64decode(segments[1] + "===").decode("utf-8"))),
-            segments[2],
-        )
-
-    @classmethod
-    async def build(cls, adapter: "Adapter", base_info: BotInfo):
-        bot = Bot(adapter, base_info.appId, base_info)
-        await bot.login(base_info.jwt)
-        return bot
-
-    async def update_info(self, jwt: Optional[str]):
-        jwt = jwt or self.base_info.jwt
-        self.info = await self.resolveToken(token=jwt)
-        self.base_info.jwt = jwt
-        self.self_id = self.info.userId
-
-    @override
-    def __init__(self, adapter: "Adapter", self_id: str, base_info: BotInfo):
-        super().__init__(adapter, self_id)
-        self.url = str(base_info.url)
-        self.base_info = base_info
-        self.sio = AsyncSocketClient(serializer="msgpack")
-        self.info: Optional[TokenInfo] = None
-
-    @override
-    async def send(
-        self,
-        event: Event,
-        message: Union[str, Message, MessageSegment],
-        encode: bool = False,
-        **kwargs,
-    ) -> Any:
-        if not isinstance(event, MessageEvent):
-            raise ValueError("event must be MessageEvent")
-        return await self.sendMessage(
-            content=(Message(message).decode() if encode else message) if isinstance(message, str) else message.decode(),
-            converseId=event.get_converse_id(),
-            groupId=event.get_group_id(),
-            meta=kwargs.get("meta"),
-            plain=kwargs.get("plain"),
-        )
-
-    async def resolveToken(self, *, token: str) -> TokenInfo:
-        """获取token信息"""
-        return TypeAdapter(TokenInfo).validate_python(await self.call_api("user.resolveToken", token=token))
-
-    async def loginBot(self, *, appId: str, appSecret: str) -> BaseBotInfo:
-        return TypeAdapter(BaseBotInfo).validate_python(
-            await self.call_api(
-                "openapi.bot.login", token=self.md5(appId + appSecret), appId=appId, use_http_=True, use_sio_=False
-            )
-        )
-
-    async def login(self, jwt: Optional[str] = None):
-        if jwt:
-            jwt_data = self.decode_jwt(jwt)[1]
-            if jwt_data.exp.timestamp() > time():
-                self.base_info.jwt = jwt
-                return
-        if self.base_info.appId and self.base_info.appSecret:
-            data = await self.loginBot(appId=self.base_info.appId, appSecret=self.base_info.appSecret)
-            self.base_info.jwt = data.jwt
-            return
-        raise ValueError("必须提供jwt或appId和appSecret")
-
-    async def sendMessage(
-        self,
-        *,
-        content: str,
-        converseId: str,
-        meta: Optional[dict] = None,
-        plain: Optional[str] = None,
-        groupId: Optional[str] = None,
-    ) -> MessageRet:
-        """发送消息"""
-        return TypeAdapter(MessageRet).validate_python(
-            await self.call_api(
-                "chat.message.sendMessage",
-                meta=meta,
-                plain=plain,
-                content=content,
-                groupId=groupId,
-                converseId=converseId,
-            )
-        )
 
+class API(BaseBot, ABC):
     async def ackAll(self) -> list[Ack]:
-        """获取所有会话的最后一条消息的ID(不确定)"""
+        """获取所有会话的最后一条消息的ID"""
         return TypeAdapter(list[Ack]).validate_python(await self.call_api("chat.ack.all"))
 
     async def allApp(self):
         """获取当前账号全部openapi app信息"""
         return await self.call_api("openapi.app.all")
 
     async def getApp(self, *, appId: str):
@@ -160,29 +36,25 @@
         return await self.call_api("openapi.app.get", appId=appId)
 
     async def whoami(self) -> Whoami:
         """获取当前账户信息"""
         return TypeAdapter(Whoami).validate_python(await self.call_api("user.whoami"))
 
     async def getFile(self, *, objectName: str):
+        """获取文件url (但是参数不知道填啥)"""
         return await self.call_api("file.get", objectName=objectName)
 
-    async def upload(self, *, file: bytes) -> FileInfo:
-        """上传文件"""
-        return TypeAdapter(FileInfo).validate_python(
-            await self.call_api("upload", file=file, use_api_=False, use_http_=True, use_sio_=False)
-        )
-
     async def ackInbox(self, *, inboxItemIds: list[str]):
         return await self.call_api("chat.inbox.ack", inboxItemIds=inboxItemIds)
 
     async def allInbox(self):
         return await self.call_api("chat.inbox.all")
 
     async def isMember(self, *, groupId: str):
+        """是否为指定群的成员"""
         return await self.call_api("group.isMember", groupId=groupId)
 
     async def register(
         self,
         *,
         password: str,
         email: Optional[str] = None,
@@ -203,28 +75,35 @@
 
     async def saveFile(self):
         return await self.call_api("file.save")
 
     async def statFile(self, *, objectName: str):
         return await self.call_api("file.stat", objectName=objectName)
 
+    async def upload(self, *, file: bytes) -> FileInfo:
+        """上传文件"""
+        return TypeAdapter(FileInfo).validate_python(
+            await self.call_api("upload", file=file, use_api_=False, use_http_=True, use_sio_=False)
+        )
+
     async def authToken(self, *, appId: str, token: str, capability: Optional[list[str]] = None):
         """验证token"""
         return await self.call_api("openapi.app.authToken", appId=appId, token=token, capability=capability)
 
     async def createApp(self, *, appDesc: str, appIcon: str, appName: str):
         return await self.call_api("openapi.app.create", appDesc=appDesc, appIcon=appIcon, appName=appName)
 
     async def deleteApp(self, *, appId: str):
         return await self.call_api("openapi.app.delete", appId=appId)
 
     async def loginUser(self, *, password: str, email: Optional[str] = None, username: Optional[str] = None):
         return await self.call_api("user.login", email=email, password=password, username=username)
 
     async def quitGroup(self, *, groupId: str):
+        """退群"""
         return await self.call_api("group.quitGroup", groupId=groupId)
 
     async def updateAck(self, *, converseId: str, lastMessageId: str):
         return await self.call_api("chat.ack.update", converseId=converseId, lastMessageId=lastMessageId)
 
     async def addBotUser(self, *, appId: str, groupId: str):
         return await self.call_api("openapi.integration.addBotUser", appId=appId, groupId=groupId)
@@ -245,25 +124,50 @@
         return await self.call_api("user.dmlist.addConverse", converseId=converseId)
 
     async def addReaction(self, *, emoji: str, messageId: str):
         """添加消息表情"""
         return await self.call_api("chat.message.addReaction", emoji=emoji, messageId=messageId)
 
     async def applyInvite(self, *, code: str):
+        """通过邀请码加群"""
         return await self.call_api("group.invite.applyInvite", code=code)
 
     async def createGroup(self, *, name: str, panels: list[Union[Panel, dict]]) -> GroupInfo:
         """创建群组"""
-        return TypeAdapter(GroupInfo).validate_python(await self.call_api("group.createGroup", name=name, panels=panels))
+        return TypeAdapter(GroupInfo).validate_python(
+            await self.call_api("group.createGroup", name=name, panels=panels)
+        )
 
     async def denyRequest(self, *, requestId: str):
         return await self.call_api("friend.request.deny", requestId=requestId)
 
-    async def getUserInfo(self, *, userId: str):
-        return await self.call_api("user.getUserInfo", userId=userId)
+    async def getUserInfo(self, *, userId: str) -> UserInfo:
+        """获取用户信息"""
+        return TypeAdapter(UserInfo).validate_python(await self.call_api("user.getUserInfo", userId=userId))
+
+    async def sendMessage(
+        self,
+        *,
+        content: str,
+        converseId: str,
+        meta: Optional[dict] = None,
+        plain: Optional[str] = None,
+        groupId: Optional[str] = None,
+    ) -> MessageRet:
+        """发送消息"""
+        return TypeAdapter(MessageRet).validate_python(
+            await self.call_api(
+                "chat.message.sendMessage",
+                meta=meta,
+                plain=plain,
+                content=content,
+                groupId=groupId,
+                converseId=converseId,
+            )
+        )
 
     async def verifyEmail(self, *, email: str):
         return await self.call_api("user.verifyEmail", email=email)
 
     async def configClient(self) -> ClientConfig:
         """获取客户端配置"""
         return TypeAdapter(ClientConfig).validate_python(await self.call_api("config.client"))
@@ -284,14 +188,18 @@
 
     async def listRegistry(self):
         return await self.call_api("plugin.registry.list")
 
     async def removeFriend(self, *, friendUserId: str):
         return await self.call_api("friend.removeFriend", friendUserId=friendUserId)
 
+    async def resolveToken(self, *, token: str) -> TokenInfo:
+        """获取token信息"""
+        return TypeAdapter(TokenInfo).validate_python(await self.call_api("user.resolveToken", token=token))
+
     async def acceptRequest(self, *, requestId: str):
         return await self.call_api("friend.request.accept", requestId=requestId)
 
     async def cancelRequest(self, *, requestId: str):
         return await self.call_api("friend.request.cancel", requestId=requestId)
 
     async def checkIsFriend(self, *, targetId: str):
@@ -446,16 +354,18 @@
 
     async def findConverseInfo(self, *, converseId: str) -> ConverseInfo:
         """获取会话信息"""
         return TypeAdapter(ConverseInfo).validate_python(
             await self.call_api("chat.converse.findConverseInfo", converseId=converseId)
         )
 
-    async def findInviteByCode(self, *, code: str):
-        return await self.call_api("group.invite.findInviteByCode", code=code)
+    async def findInviteByCode(self, *, code: str) -> Optional[InviteCodeInfo]:
+        return TypeAdapter(Optional[InviteCodeInfo]).validate_python(
+            await self.call_api("group.invite.findInviteByCode", code=code)
+        )
 
     async def findOpenapiBotId(self, *, email: str):
         return await self.call_api("user.findOpenapiBotId", email=email)
 
     async def modifyGroupPanel(
         self,
         *,
@@ -483,15 +393,17 @@
         )
 
     async def setAppCapability(self, *, appId: str, capability: list[str]):
         return await self.call_api("openapi.app.setAppCapability", appId=appId, capability=capability)
 
     async def updateGroupField(self, *, groupId: str, fieldName: str, fieldValue: Any):
         """更新群组字段"""
-        return await self.call_api("group.updateGroupField", groupId=groupId, fieldName=fieldName, fieldValue=fieldValue)
+        return await self.call_api(
+            "group.updateGroupField", groupId=groupId, fieldName=fieldName, fieldValue=fieldValue
+        )
 
     async def createGroupInvite(self, *, groupId: str, inviteType: Literal["normal", "permanent"]) -> InviteCodeInfo:
         """创建群组邀请码"""
         return TypeAdapter(InviteCodeInfo).validate_python(
             await self.call_api("group.invite.createGroupInvite", groupId=groupId, inviteType=inviteType)
         )
 
@@ -527,14 +439,15 @@
         return TypeAdapter(list[Message]).validate_python(
             await self.call_api(
                 "chat.message.fetchNearbyMessage", groupId=groupId, messageId=messageId, converseId=converseId
             )
         )
 
     async def verifyEmailWithOTP(self, *, emailOTP: str):
+        """验证邮箱"""
         return await self.call_api("user.verifyEmailWithOTP", emailOTP=emailOTP)
 
     async def buildFriendRelation(self, *, user1: str, user2: str):
         return await self.call_api("friend.buildFriendRelation", user1=user1, user2=user2)
 
     async def createTemporaryUser(self, *, nickname: str):
         return await self.call_api("user.createTemporaryUser", nickname=nickname)
```

### Comparing `nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/config.py` & `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/event.py` & `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,37 +156,37 @@
     createdAt: datetime
     updatedAt: datetime
 
     groupId: Optional[str] = Field(default=None)
 
     @property
     def replay(self) -> Optional[Replay]:
-        return self.meta.replay
+        return self.meta.replay if self.meta else None
 
     @override
     def get_message(self) -> Message:
         return self.content
 
     @override
     def get_user_id(self) -> str:
         return self.author
 
     @override
     def get_session_id(self) -> str:
         return self.converseId
 
     def _is_tome(self) -> bool:
-        return not self.is_group() or self.self_id in self.meta.mentions
+        return not self.is_group() or (self.meta and self.self_id in self.meta.mentions)
 
     @override
     def get_event_description(self) -> str:
         return (
             f"Message {self.id} from {self.author}"
             + (f"@[群:{self.groupId}]" if self.groupId else "")
-            + f" {str(self.content)}"
+            + f" {self.content.show()}"
         )
 
     def is_group(self) -> bool:
         return not not self.groupId
 
 
 class AtEvent(Event):
@@ -229,15 +229,15 @@
         return self.payload.messageAuthor
 
     @override
     def get_event_description(self) -> str:
         return (
             f"AtMessage {self.payload.messageId} from {self.payload.messageAuthor}"
             + (f"@[群:{self.get_group_id()}]" if self.payload.groupId else "")
-            + f" {str(self.payload.messageSnippet)}"
+            + f" {self.payload.messageSnippet.show()}"
         )
 
 
 @register_event_class
 class MessageAddEvent(DefaultMessageEvent):
     event_name: Literal["notify:chat.message.add"]
```

### Comparing `nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/exception.py` & `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/message.py` & `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,16 +70,18 @@
     def text(self) -> str:
         return self.box["text"]
 
     @property
     def head(self) -> str:
         return (
             "["
-            + (f"{self.tag}={self.main}" if self.main else self.tag)
-            + " ".join(f"{k}={v}" for k, v in self.items() if k in self.keys_)
+            + (
+                (f"{self.tag}={self.main} " if self.main else self.tag)
+                + " ".join(f"{k}={v}" for k, v in self.items() if k in self.keys_ and k not in self.tags)
+            ).rstrip(" ")
             + "]"
         )
 
     @property
     def tail(self) -> str:
         return f"[/{self.tag}]"
 
@@ -331,7 +333,10 @@
 
     @override
     def extract_plain_text(self) -> str:
         return "".join(seg.data["text"] for seg in self if seg.is_text())
 
     def decode(self) -> str:
         return "".join(seg.decode() for seg in self)
+
+    def show(self) -> str:
+        return " ".join(seg.decode() for seg in self)
```

### Comparing `nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/model.py` & `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b2/nonebot_adapter_tailchat/util.py` & `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b2/pyproject.toml` & `nonebot_adapter_tailchat-0.1.0b3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-tailchat"
-version = "0.1.0b2"
+version = "0.1.0b3"
 description = "NoneBot2 Tailchat 适配器 / Tailchat adapter for nonebot2"
 authors = ["eya46 <61458340+eya46@users.noreply.github.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "nonebot_adapter_tailchat" }]
 
 [tool.poetry.dependencies]
@@ -14,21 +14,22 @@
 python-socketio = { extras = ["asyncio-client"], version = "^5.11.2" }
 msgpack = "^1.0.8"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.4.2"
 nonebot2 = { extras = ["httpx"], version = "^2.3.0" }
+pyyaml = "^6.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
-line-length = 121
+line-length = 120
 target-version = "py39"
 
 [tool.ruff.lint]
 select = ["E", "W", "F", "UP", "C", "T", "PYI", "PT", "Q", "I"]
 ignore = [
     "E402", # 导包位置
     "E722", # 空except
```

### Comparing `nonebot_adapter_tailchat-0.1.0b2/PKG-INFO` & `nonebot_adapter_tailchat-0.1.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-tailchat
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: NoneBot2 Tailchat 适配器 / Tailchat adapter for nonebot2
 License: Apache-2.0
 Author: eya46
 Author-email: 61458340+eya46@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-tailchat Version: 0.1.0b2 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-tailchat Version: 0.1.0b3 Summary:
 NoneBot2 Tailchat ééå¨ / Tailchat adapter for nonebot2 License: Apache-2.0
 Author: eya46 Author-email: 61458340+eya46@users.noreply.github.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: msgpack (>=1.0.8,<2.0.0) Requires-
```

