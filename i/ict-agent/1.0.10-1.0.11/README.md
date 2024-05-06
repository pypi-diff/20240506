# Comparing `tmp/ict_agent-1.0.10.tar.gz` & `tmp/ict_agent-1.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ict_agent-1.0.10.tar", last modified: Thu Mar 21 14:24:50 2024, max compression
+gzip compressed data, was "ict_agent-1.0.11.tar", last modified: Mon May  6 05:35:42 2024, max compression
```

## Comparing `ict_agent-1.0.10.tar` & `ict_agent-1.0.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 14:24:50.019618 ict_agent-1.0.10/
--rw-rw-rw-   0        0        0      134 2024-03-21 14:24:50.018618 ict_agent-1.0.10/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-01-18 13:15:16.000000 ict_agent-1.0.10/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 14:24:50.010619 ict_agent-1.0.10/ict_agent/
--rw-rw-rw-   0        0        0    13586 2024-03-21 14:09:02.000000 ict_agent-1.0.10/ict_agent/DigitalHuman.py
--rw-rw-rw-   0        0        0     7969 2024-02-07 05:48:44.000000 ict_agent-1.0.10/ict_agent/Math.py
--rw-rw-rw-   0        0        0     4749 2024-03-21 14:09:03.000000 ict_agent-1.0.10/ict_agent/Public.py
--rw-rw-rw-   0        0        0     5961 2024-03-21 14:09:02.000000 ict_agent-1.0.10/ict_agent/Robot.py
--rw-rw-rw-   0        0        0    18432 2024-03-21 14:09:02.000000 ict_agent-1.0.10/ict_agent/UAV.py
--rw-rw-rw-   0        0        0       29 2024-01-18 13:16:31.000000 ict_agent-1.0.10/ict_agent/__init__.py
--rw-rw-rw-   0        0        0     4713 2024-02-04 09:51:43.000000 ict_agent-1.0.10/ict_agent/core.py
-drwxrwxrwx   0        0        0        0 2024-03-21 14:24:50.017618 ict_agent-1.0.10/ict_agent.egg-info/
--rw-rw-rw-   0        0        0      134 2024-03-21 14:24:49.000000 ict_agent-1.0.10/ict_agent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2024-03-21 14:24:49.000000 ict_agent-1.0.10/ict_agent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 14:24:49.000000 ict_agent-1.0.10/ict_agent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-03-21 14:24:49.000000 ict_agent-1.0.10/ict_agent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-21 14:24:49.000000 ict_agent-1.0.10/ict_agent.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-21 14:24:50.019618 ict_agent-1.0.10/setup.cfg
--rw-rw-rw-   0        0        0      287 2024-03-21 14:24:05.000000 ict_agent-1.0.10/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 05:35:42.513338 ict_agent-1.0.11/
+-rw-rw-rw-   0        0        0      134 2024-05-06 05:35:42.511338 ict_agent-1.0.11/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-01-18 13:15:16.000000 ict_agent-1.0.11/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 05:35:42.502338 ict_agent-1.0.11/ict_agent/
+-rw-rw-rw-   0        0        0    14002 2024-05-06 05:22:30.000000 ict_agent-1.0.11/ict_agent/DigitalHuman.py
+-rw-rw-rw-   0        0        0     7969 2024-02-07 05:48:44.000000 ict_agent-1.0.11/ict_agent/Math.py
+-rw-rw-rw-   0        0        0     4749 2024-03-21 14:09:03.000000 ict_agent-1.0.11/ict_agent/Public.py
+-rw-rw-rw-   0        0        0     5976 2024-05-06 05:29:21.000000 ict_agent-1.0.11/ict_agent/Robot.py
+-rw-rw-rw-   0        0        0    18432 2024-03-21 14:09:02.000000 ict_agent-1.0.11/ict_agent/UAV.py
+-rw-rw-rw-   0        0        0       29 2024-01-18 13:16:31.000000 ict_agent-1.0.11/ict_agent/__init__.py
+-rw-rw-rw-   0        0        0     4713 2024-02-04 09:51:43.000000 ict_agent-1.0.11/ict_agent/core.py
+drwxrwxrwx   0        0        0        0 2024-05-06 05:35:42.510338 ict_agent-1.0.11/ict_agent.egg-info/
+-rw-rw-rw-   0        0        0      134 2024-05-06 05:35:42.000000 ict_agent-1.0.11/ict_agent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2024-05-06 05:35:42.000000 ict_agent-1.0.11/ict_agent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 05:35:42.000000 ict_agent-1.0.11/ict_agent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-06 05:35:42.000000 ict_agent-1.0.11/ict_agent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-06 05:35:42.000000 ict_agent-1.0.11/ict_agent.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 05:35:42.513338 ict_agent-1.0.11/setup.cfg
+-rw-rw-rw-   0        0        0      287 2024-05-06 05:29:58.000000 ict_agent-1.0.11/setup.py
```

### Comparing `ict_agent-1.0.10/ict_agent/DigitalHuman.py` & `ict_agent-1.0.11/ict_agent/DigitalHuman.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 import ict_agent.core
 from ict_agent.core import MyWS
 
 # 数字人
 class DigtalHuman():
     name = '安琪拉'
     age = 18
@@ -61,15 +63,16 @@
     def get_sex(self):
         """
         获取数字人性别
         :return:返回性别
         """
         result = MyWS.do_wait_return({'type': 'szr', 'commond': 'get_sex'})
         if result['result'] == ict_agent.core.SUCCESS:
-            return result['msg']
+            j=json.loads(result['msg'])
+            return j
 
     def set_sex(self, sex: str):
         """
         设置数字人性别
         :param sex:性别Male，Female
         :return: bool返回操作成功或失败
         """
@@ -80,15 +83,16 @@
     def get_somatotype(self):
         """
         获取体型列表
         :return:
         """
         result = MyWS.do_wait_return({'type': 'szr', 'commond': 'get_somatotype'})
         if result['result'] == ict_agent.core.SUCCESS:
-            return result['msg']
+            j=json.loads(result['msg'])
+            return j
 
     def set_somatotype(self, somatotype: str):
         """
         设置体型
         :param somatotype:体型
         :return:
         """
@@ -143,15 +147,16 @@
     def get_hairstyle(self):
         """
         获取发型列表
         :return:
         """
         result = MyWS.do_wait_return({'type': 'szr', 'commond': 'get_hairstyle'})
         if result['result'] == ict_agent.core.SUCCESS:
-            return result['msg']
+            j=json.loads(result['msg'])
+            return j
 
     def set_hairstyle(self, hairstyle: str):
         """
         设置发型
         :param hairstyle: 发型
         :return:
         """
@@ -161,15 +166,16 @@
     def get_face(self):
         """
         获取脸型列表
         :return:
         """
         result = MyWS.do_wait_return({'type': 'szr', 'commond': 'get_face'})
         if result['result'] == ict_agent.core.SUCCESS:
-            return result['msg']
+            j=json.loads(result['msg'])
+            return j
 
     def set_face(self, face: str):
         """
         设置脸型
         :return: face: 脸型
         """
         result = MyWS.do_wait_return(self.__handle_result('set_face', {'face': face}))
@@ -178,15 +184,16 @@
     def get_glasses(self):
         """
         获取眼镜列表
         :return:
         """
         result = MyWS.do_wait_return({'type': 'szr', 'commond': 'get_glasses'})
         if result['result'] == ict_agent.core.SUCCESS:
-            return result['msg']
+            j=json.loads(result['msg'])
+            return j
 
     def set_glasses(self, glasses: str):
         """
         设置眼镜
         :return: glasses : 眼镜
         """
         result = MyWS.do_wait_return(self.__handle_result('set_glasses', {'glasses': glasses}))
@@ -199,51 +206,56 @@
     def get_head_action(self):
         """
         获取头部动作列表
         :return:
         """
         result = MyWS.do_wait_return({'type': 'szr', 'commond': 'get_head_action'})
         if result['result'] == ict_agent.core.SUCCESS:
-            return result['msg']
+            j=json.loads(result['msg'])
+            return j
 
     def get_hand_action(self):
             """
             获取手部动作列表
             :return:
             """
             result = MyWS.do_wait_return({'type': 'szr', 'commond': 'get_hand_action'})
             if result['result'] == ict_agent.core.SUCCESS:
-                return result['msg']
+                j = json.loads(result['msg'])
+                return j
 
     def get_legs_action(self):
             """
             获取腿部动作列表
             :return:
             """
             result = MyWS.do_wait_return({'type': 'szr', 'commond': 'get_legs_action'})
             if result['result'] == ict_agent.core.SUCCESS:
-                return result['msg']
+                j = json.loads(result['msg'])
+                return j
 
     def get_torso_action(self):
             """
             获取躯干动作列表
             :return:
             """
             result = MyWS.do_wait_return({'type': 'szr', 'commond': 'get_torso_action'})
             if result['result'] == ict_agent.core.SUCCESS:
-                return result['msg']
+                j = json.loads(result['msg'])
+                return j
 
     def get_emote_action(self):
             """
             获取表情动作列表
             :return:
             """
             result = MyWS.do_wait_return({'type': 'szr', 'commond': 'get_emote_action'})
             if result['result'] == ict_agent.core.SUCCESS:
-                return result['msg']
+                j = json.loads(result['msg'])
+                return j
 
     def set_head_action(self, action: [str], loop_times: int):
         """
         设置头部动作
         :param action:
         :return:
         """
@@ -281,15 +293,16 @@
     def get_skincolor(self):
         """
         获取肤色列表
         :return:
         """
         result = MyWS.do_wait_return({'type': 'szr', 'commond': 'get_skincolor'})
         if result['result'] == ict_agent.core.SUCCESS:
-            return result['msg']
+            j=json.loads(result['msg'])
+            return j
 
     def set_skincolor(self, skincolor: str):
         """
         设置肤色
         :return:
         """
         result = MyWS.do_wait_return(self.__handle_result('set_skincolor', {'skincolor': skincolor}))
@@ -298,15 +311,16 @@
     def get_timbre(self):
         """
         获取音色列表
         :return:
         """
         result = MyWS.do_wait_return({'type': 'szr', 'commond': 'get_timbre'})
         if result['result'] == ict_agent.core.SUCCESS:
-            return result['msg']
+            j=json.loads(result['msg'])
+            return j
 
     def set_timbre(self, timbre: str):
         """
         设置音色
         :return:
         """
         result = MyWS.do_wait_return(self.__handle_result('set_timbre', {'timbre': timbre}))
@@ -416,15 +430,16 @@
     def get_text_asset(self):
         """
 
         :return:
         """
         result = MyWS.do_wait_return({'type': 'szr', 'commond': 'get_text_asset'})
         if result['result'] == ict_agent.core.SUCCESS:
-            return result['msg']
+            j=json.loads(result['msg'])
+            return j
 
     def set_text_asset(self, text_asset: str):
         """
 
         :return:
         """
         result = MyWS.do_wait_return(self.__handle_result('set_text_asset', {'text_asset': text_asset}))
```

### Comparing `ict_agent-1.0.10/ict_agent/Math.py` & `ict_agent-1.0.11/ict_agent/Math.py`

 * *Files identical despite different names*

### Comparing `ict_agent-1.0.10/ict_agent/Public.py` & `ict_agent-1.0.11/ict_agent/Public.py`

 * *Files identical despite different names*

### Comparing `ict_agent-1.0.10/ict_agent/Robot.py` & `ict_agent-1.0.11/ict_agent/Robot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 import ict_agent
 from ict_agent.core import MyWS
 
 Number = 0
 
 
 # 机器人
```

### Comparing `ict_agent-1.0.10/ict_agent/UAV.py` & `ict_agent-1.0.11/ict_agent/UAV.py`

 * *Files identical despite different names*

### Comparing `ict_agent-1.0.10/ict_agent/core.py` & `ict_agent-1.0.11/ict_agent/core.py`

 * *Files identical despite different names*

