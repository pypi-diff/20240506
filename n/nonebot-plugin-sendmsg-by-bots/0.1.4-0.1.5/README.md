# Comparing `tmp/nonebot-plugin-sendmsg-by-bots-0.1.4.tar.gz` & `tmp/nonebot-plugin-sendmsg-by-bots-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-sendmsg-by-bots-0.1.4.tar", last modified: Thu Apr 18 11:17:53 2024, max compression
+gzip compressed data, was "nonebot-plugin-sendmsg-by-bots-0.1.5.tar", last modified: Mon May  6 02:28:28 2024, max compression
```

## Comparing `nonebot-plugin-sendmsg-by-bots-0.1.4.tar` & `nonebot-plugin-sendmsg-by-bots-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2800 2024-04-18 11:17:50.264318 nonebot-plugin-sendmsg-by-bots-0.1.4/README.md
--rw-r--r--   0        0        0     1976 2024-04-18 11:17:50.264318 nonebot-plugin-sendmsg-by-bots-0.1.4/nonebot_plugin_sendmsg_by_bots/__init__.py
--rw-r--r--   0        0        0      336 2024-04-18 11:17:50.264318 nonebot-plugin-sendmsg-by-bots-0.1.4/nonebot_plugin_sendmsg_by_bots/config.py
--rw-r--r--   0        0        0     9007 2024-04-18 11:17:50.264318 nonebot-plugin-sendmsg-by-bots-0.1.4/nonebot_plugin_sendmsg_by_bots/tools.py
--rw-r--r--   0        0        0      575 2024-04-18 11:17:50.264318 nonebot-plugin-sendmsg-by-bots-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3181 1970-01-01 00:00:00.000000 nonebot-plugin-sendmsg-by-bots-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2800 2024-05-06 02:28:25.864006 nonebot-plugin-sendmsg-by-bots-0.1.5/README.md
+-rw-r--r--   0        0        0     1976 2024-05-06 02:28:25.864006 nonebot-plugin-sendmsg-by-bots-0.1.5/nonebot_plugin_sendmsg_by_bots/__init__.py
+-rw-r--r--   0        0        0      336 2024-05-06 02:28:25.864006 nonebot-plugin-sendmsg-by-bots-0.1.5/nonebot_plugin_sendmsg_by_bots/config.py
+-rw-r--r--   0        0        0     9508 2024-05-06 02:28:25.864006 nonebot-plugin-sendmsg-by-bots-0.1.5/nonebot_plugin_sendmsg_by_bots/tools.py
+-rw-r--r--   0        0        0      575 2024-05-06 02:28:25.864006 nonebot-plugin-sendmsg-by-bots-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3181 1970-01-01 00:00:00.000000 nonebot-plugin-sendmsg-by-bots-0.1.5/PKG-INFO
```

### Comparing `nonebot-plugin-sendmsg-by-bots-0.1.4/README.md` & `nonebot-plugin-sendmsg-by-bots-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sendmsg-by-bots-0.1.4/nonebot_plugin_sendmsg_by_bots/__init__.py` & `nonebot-plugin-sendmsg-by-bots-0.1.5/nonebot_plugin_sendmsg_by_bots/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sendmsg-by-bots-0.1.4/nonebot_plugin_sendmsg_by_bots/tools.py` & `nonebot-plugin-sendmsg-by-bots-0.1.5/nonebot_plugin_sendmsg_by_bots/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,39 +89,58 @@
     status = False
     for bot in bots:
         if await is_in_friend(bots[bot],int(user_id)):
             await send_forward_msg(bots[bot],int(user_id),node_msg,msg_type="private")
             status = True
     return status
 
-async def send_group_forward_msg_by_bots_once(group_id:int,node_msg:list) -> bool:
+async def send_group_forward_msg_by_bots_once(group_id:int,node_msg:list,bot_id: Optional[str] = None) -> bool:
     '''group_id：尝试发送到的群号\n
     msg：尝试发送的node列表\n
     不在bot群列表的群不会尝试发送'''
     bots = nonebot.get_adapter(Adapter).bots
     status = False
+    
+    if bot_id:
+        try:
+            await send_forward_msg(bots[bot_id],int(group_id),node_msg)
+            status = True
+            return status
+        except Exception as e:
+            pass
+        
     for bot in bots:
         if await is_in_group(bots[bot],int(group_id)):
             await send_forward_msg(bots[bot],int(group_id),node_msg)
             status = True
             return status
     return status
         
-async def send_private_forward_msg_by_bots_once(user_id:int,node_msg:list) -> bool:
+async def send_private_forward_msg_by_bots_once(user_id:int,node_msg:list,bot_id: Optional[str] = None) -> bool:
     '''user_id：尝试发送到的好友qq号\n
     msg：尝试发送的node列表\n
     不在bot好友列表的qq不会尝试发送'''
     bots = nonebot.get_adapter(Adapter).bots
     status = False
+    
+    if bot_id:
+        try:
+            await send_forward_msg(bots[bot_id],int(user_id),node_msg,msg_type="private")
+            status = True
+            return status
+        except Exception as e:
+            pass
+    
     for bot in bots:
         if await is_in_friend(bots[bot],int(user_id)):
             await send_forward_msg(bots[bot],int(user_id),node_msg,msg_type="private")
             status = True
             return status
     return status            
+
 async def send_group_msg_by_bots(group_id:int,msg:Message|MessageSegment|str) -> bool:
     '''group_id：尝试发送到的群号\n
     msg：尝试发送的消息\n
     不在bot群列表的群不会尝试发送'''
     bots = nonebot.get_adapter(Adapter).bots
     status = False
     for bot in bots:
```

### Comparing `nonebot-plugin-sendmsg-by-bots-0.1.4/pyproject.toml` & `nonebot-plugin-sendmsg-by-bots-0.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-sendmsg-by-bots"
-version = "0.1.4"
+version = "0.1.5"
 description = "a send msg tools"
 authors = [
     { name = "nek0us", email = "nekouss@gmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.3",
```

### Comparing `nonebot-plugin-sendmsg-by-bots-0.1.4/PKG-INFO` & `nonebot-plugin-sendmsg-by-bots-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sendmsg-by-bots
-Version: 0.1.4
+Version: 0.1.5
 Summary: a send msg tools
 License: MIT
 Author-email: nek0us <nekouss@gmail.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/nek0us/nonebot-plugin-sendmsg-by-bots
 Project-URL: Repository, https://github.com/nek0us/nonebot-plugin-sendmsg-by-bots
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sendmsg-by-bots Version: 0.1.4
+Metadata-Version: 2.1 Name: nonebot-plugin-sendmsg-by-bots Version: 0.1.5
 Summary: a send msg tools License: MIT Author-email: nek0us
 gmail.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 nek0us/nonebot-plugin-sendmsg-by-bots Project-URL: Repository, https://
 github.com/nek0us/nonebot-plugin-sendmsg-by-bots Description-Content-Type:
 text/markdown
                              x_[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
```

