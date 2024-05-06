# Comparing `tmp/tsugu-api-python-0.1.1.tar.gz` & `tmp/tsugu-api-python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-api-python-0.1.1.tar", last modified: Wed Apr 24 09:28:16 2024, max compression
+gzip compressed data, was "tsugu-api-python-0.2.0.tar", last modified: Mon May  6 07:59:17 2024, max compression
```

## Comparing `tsugu-api-python-0.1.1.tar` & `tsugu-api-python-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:28:16.328532 tsugu-api-python-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-04-24 09:28:16.328532 tsugu-api-python-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 09:28:16.328532 tsugu-api-python-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:28:16.324532 tsugu-api-python-0.1.1/tsugu_api/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:28:16.324532 tsugu-api-python-0.1.1/tsugu_api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api/v1/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api/v1/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api/v1/_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:28:16.324532 tsugu-api-python-0.1.1/tsugu_api/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api/v2/_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:28:16.324532 tsugu-api-python-0.1.1/tsugu_api_async/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api_async/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api_async/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api_async/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api_async/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api_async/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:28:16.324532 tsugu-api-python-0.1.1/tsugu_api_async/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api_async/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api_async/v1/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10973 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api_async/v1/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api_async/v1/_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:28:16.324532 tsugu-api-python-0.1.1/tsugu_api_async/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api_async/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-04-24 09:28:02.000000 tsugu-api-python-0.1.1/tsugu_api_async/v2/_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:28:16.324532 tsugu-api-python-0.1.1/tsugu_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-04-24 09:28:15.000000 tsugu-api-python-0.1.1/tsugu_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-24 09:28:16.000000 tsugu-api-python-0.1.1/tsugu_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:28:15.000000 tsugu-api-python-0.1.1/tsugu_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 09:28:15.000000 tsugu-api-python-0.1.1/tsugu_api_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/tsugu_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/tsugu_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/v1/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/v1/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/v1/_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/tsugu_api/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api/v2/_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/tsugu_api_async/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/tsugu_api_async/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/v1/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/v1/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/v1/_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/tsugu_api_async/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-06 07:59:07.000000 tsugu-api-python-0.2.0/tsugu_api_async/v2/_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 07:59:17.382037 tsugu-api-python-0.2.0/tsugu_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-06 07:59:17.000000 tsugu-api-python-0.2.0/tsugu_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-06 07:59:17.000000 tsugu-api-python-0.2.0/tsugu_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 07:59:17.000000 tsugu-api-python-0.2.0/tsugu_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 07:59:17.000000 tsugu-api-python-0.2.0/tsugu_api_python.egg-info/top_level.txt
```

### Comparing `tsugu-api-python-0.1.1/LICENSE` & `tsugu-api-python-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.1.1/PKG-INFO` & `tsugu-api-python-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 0.1.1
+Version: 0.2.0
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 0.1.1 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 0.2.0 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-0.1.1/README.md` & `tsugu-api-python-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.1.1/setup.py` & `tsugu-api-python-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu-api-python',
-    version='0.1.1',
+    version='0.2.0',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Tsugu BanGDream Bot 的功能 API 统合包',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/tsugu-api-python',
     include_package_data=False,
```

### Comparing `tsugu-api-python-0.1.1/tsugu_api/_network.py` & `tsugu-api-python-0.2.0/tsugu_api/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.1.1/tsugu_api/_typing.py` & `tsugu-api-python-0.2.0/tsugu_api/_typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 class _QueryResult(TypedDict):
     '''`/station/queryAllRoom` 响应结果'''
     status: _Status
     data: Union[str, list[_CarData]]
 
 class _SubmitResult(TypedDict):
-    '''`submit_room_number` 响应结果'''
+    '''`/station/submitRoomNumber` 响应结果'''
     status: _Status
     data: Union[str, list[_CarData]]
 
 class _ServerData(TypedDict):
     '''服务器数据'''
     playerId: int
     bindingStatus: int
```

### Comparing `tsugu-api-python-0.1.1/tsugu_api/settings.py` & `tsugu-api-python-0.2.0/tsugu_api/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.1.1/tsugu_api/utils.py` & `tsugu-api-python-0.2.0/tsugu_api/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.1.1/tsugu_api/v1/__init__.py` & `tsugu-api-python-0.2.0/tsugu_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.1.1/tsugu_api/v1/_bandoristation.py` & `tsugu-api-python-0.2.0/tsugu_api/v1/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.1.1/tsugu_api/v1/_tsugu.py` & `tsugu-api-python-0.2.0/tsugu_api/v1/_tsugu.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,15 @@
     _SubmitResult
 )
 
 def get_card_illustration(card_id: int) -> _Response:
     '''获取卡面
 
     参数:
-        platform (str): 平台名称
-        user_id (str): 用户 ID
+        card_id (int): 卡片 ID
 
     返回:
         _Response: 响应信息
     '''
     
     # 构建 URL
     url = settings.backend_url + '/getCardIllustration'
@@ -149,14 +148,45 @@
     
     # 发送请求
     return Api(
         url,
         proxy=settings.backend_proxy,
         data=data
     ).post().json()
+
+def event_stage(server: _Server, meta: bool = False, event_id: Optional[int] = None) -> _Response:
+    '''查询团队 LIVE 佳节活动舞台数据
+
+    参数:
+        server (_Server): 服务器
+        meta (bool): 是否携带歌曲分数表
+        event_id (int): 活动 ID
+
+    返回:
+        _Response: 响应信息
+    '''
+    
+    # 构建 URL
+    url = settings.backend_url + '/eventStage'
+    
+    # 构建数据
+    data = {
+        'server': server,
+        'meta': meta,
+        'compress': settings.compress
+    }
+    if event_id:
+        data['eventId'] = event_id
+    
+    # 发送请求
+    return Api(
+        url,
+        proxy=settings.backend_proxy,
+        data=data
+    ).post().json()
 
 def search_song(default_servers: list[_Server], text: str) -> _Response:
     '''查询歌曲
 
     参数:
         default_servers (list[_Server]): 默认服务器
         text (str): 查询参数
```

### Comparing `tsugu-api-python-0.1.1/tsugu_api/v1/_user.py` & `tsugu-api-python-0.2.0/tsugu_api/v1/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.1.1/tsugu_api/v2/__init__.py` & `tsugu-api-python-0.2.0/tsugu_api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.1.1/tsugu_api/v2/_api.py` & `tsugu-api-python-0.2.0/tsugu_api/v2/_api.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.1.1/tsugu_api_async/_network.py` & `tsugu-api-python-0.2.0/tsugu_api_async/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.1.1/tsugu_api_async/_typing.py` & `tsugu-api-python-0.2.0/tsugu_api_async/_typing.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.1.1/tsugu_api_async/settings.py` & `tsugu-api-python-0.2.0/tsugu_api_async/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.1.1/tsugu_api_async/utils.py` & `tsugu-api-python-0.2.0/tsugu_api_async/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.1.1/tsugu_api_async/v1/__init__.py` & `tsugu-api-python-0.2.0/tsugu_api_async/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.1.1/tsugu_api_async/v1/_bandoristation.py` & `tsugu-api-python-0.2.0/tsugu_api_async/v1/_bandoristation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from httpx import Response
+
 from tsugu_api_async import settings
 from tsugu_api_async._network import Api
 from tsugu_api_async.exception import RoomSubmitFailure
 
 BANDORI_STATION_URL = 'https://api.bandoristation.com/index.php'
 
 async def submit_room_number(number: int, user_id: str, raw_message: str, source: str, token: str) -> None:
@@ -22,16 +24,16 @@
         'user_id': user_id,
         'raw_message': raw_message,
         'source': source,
         'token': token
     }
     
     # 发送请求
-    response = await (
-        await Api(
+    response = await Api(
             BANDORI_STATION_URL,
             proxy=settings.backend_proxy,
             params=params
-        ).get()
-    ).json()
+    ).get()
+    if isinstance(response, Response): response = response.json()
+    else: response = await response.json()
     if response['status'] == 'failure':
         raise RoomSubmitFailure(response['response'])
```

### Comparing `tsugu-api-python-0.1.1/tsugu_api_async/v1/_user.py` & `tsugu-api-python-0.2.0/tsugu_api_async/v1/_user.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from httpx import HTTPStatusError
+from httpx import Response, HTTPStatusError
 
 from tsugu_api_async import settings
 from tsugu_api_async._network import Api
 from tsugu_api_async._typing import (
     _Result,
     _Server,
     _BindResponse,
@@ -26,21 +26,21 @@
     # 构建数据
     data = {
         'platform': platform,
         'user_id': user_id
     }
     
     # 发送请求
-    return await (
-        await Api(
-            url,
-            proxy=settings.userdata_backend_proxy,
-            data=data
-        ).post()
-    ).json()
+    response = await Api(
+        url,
+        proxy=settings.userdata_backend_proxy,
+        data=data
+    ).post()
+    if isinstance(response, Response): return response.json()
+    return await response.json()
 
 async def bind_player_request(
     platform: str,
     user_id: str,
     server: _Server,
     bind_type: bool
 ) -> _BindResponse:
@@ -65,21 +65,21 @@
         'user_id': user_id,
         'server': server,
         'bindType': bind_type
     }
     
     # 发送请求
     try:
-        return await (
-            await Api(
-                url,
-                proxy=settings.userdata_backend_proxy,
-                data=data
-            ).post()
-        ).json()
+        response = await Api(
+            url,
+            proxy=settings.userdata_backend_proxy,
+            data=data
+        ).post()
+        if isinstance(response, Response): return response.json()
+        return await response.json()
     except HTTPStatusError as exception:
         if exception.response.status_code == 400:
             return exception.response.json()
         else:
             raise exception
 
 async def bind_player_verification(
@@ -112,21 +112,21 @@
         'playerId': player_id,
         'server': server,
         'bindType': bind_type
     }
     
     # 发送请求
     try:
-        return await (
-            await Api(
-                url,
-                proxy=settings.userdata_backend_proxy,
-                data=data
-            ).post()
-        ).json()
+        response = await Api(
+            url,
+            proxy=settings.userdata_backend_proxy,
+            data=data
+        ).post()
+        if isinstance(response, Response): return response.json()
+        return await response.json()
     except HTTPStatusError as exception:
         if exception.response.status_code == 400:
             return exception.response.json()
         else:
             raise exception
 
 async def set_car_forwarding(platform: str, user_id: str, status: bool) -> _Result:
@@ -149,21 +149,21 @@
         'platform': platform,
         'user_id': user_id,
         'status': status
     }
     
     # 发送请求
     try:
-        return await (
-            await Api(
-                url,
-                proxy=settings.userdata_backend_proxy,
-                data=data
-            ).post()
-        ).json()
+        response = await Api(
+            url,
+            proxy=settings.userdata_backend_proxy,
+            data=data
+        ).post()
+        if isinstance(response, Response): return response.json()
+        return await response.json()
     except HTTPStatusError as exception:
         if exception.response.status_code == 400:
             return exception.response.json()
         else:
             raise exception
 
 async def set_default_server(platform: str, user_id: str, text: str) -> _Result:
@@ -186,21 +186,21 @@
         'platform': platform,
         'user_id': user_id,
         'text': text
     }
     
     # 发送请求
     try:
-        return await (
-            await Api(
-                url,
-                proxy=settings.userdata_backend_proxy,
-                data=data
-            ).post()
-        ).json()
+        response = await Api(
+            url,
+            proxy=settings.userdata_backend_proxy,
+            data=data
+        ).post()
+        if isinstance(response, Response): return response.json()
+        return await response.json()
     except HTTPStatusError as exception:
         if exception.response.status_code == 400:
             return exception.response.json()
         else:
             raise exception
 
 async def set_server_mode(platform: str, user_id: str, text: str) -> _Result:
@@ -223,19 +223,19 @@
         'platform': platform,
         'user_id': user_id,
         'text': text
     }
     
     # 发送请求
     try:
-        return await (
-            await Api(
-                url,
-                proxy=settings.userdata_backend_proxy,
-                data=data
-            ).post()
-        ).json()
+        response = await Api(
+            url,
+            proxy=settings.userdata_backend_proxy,
+            data=data
+        ).post()
+        if isinstance(response, Response): return response.json()
+        return await response.json()
     except HTTPStatusError as exception:
         if exception.response.status_code == 400:
             return exception.response.json()
         else:
             raise exception
```

### Comparing `tsugu-api-python-0.1.1/tsugu_api_async/v2/__init__.py` & `tsugu-api-python-0.2.0/tsugu_api_async/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-0.1.1/tsugu_api_async/v2/_api.py` & `tsugu-api-python-0.2.0/tsugu_api_async/v2/_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from httpx import Response
+
 from tsugu_api_async import settings
 from tsugu_api_async._network import Api
 from tsugu_api_async._typing import _Server, _Response
 
 async def _v2_post_request(
     api: str,
     text: str,
@@ -29,21 +31,21 @@
         'default_server': default_server,
         'server': server,
         'useEasyBG': settings.use_easy_bg,
         'compress': settings.compress
     }
     
     # 发送请求
-    return await (
-        await Api(
-            url,
-            proxy=settings.backend_proxy,
-            data=data
-        ).post()
-    ).json()
+    response = await Api(
+        url,
+        proxy=settings.backend_proxy,
+        data=data
+    ).post()
+    if isinstance(response, Response): return response.json()
+    return await response.json()
 
 async def card_illustration(
     text: str
 ) -> _Response:
     '''卡片插图
 
     参数:
```

### Comparing `tsugu-api-python-0.1.1/tsugu_api_python.egg-info/PKG-INFO` & `tsugu-api-python-0.2.0/tsugu_api_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 0.1.1
+Version: 0.2.0
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 0.1.1 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 0.2.0 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-0.1.1/tsugu_api_python.egg-info/SOURCES.txt` & `tsugu-api-python-0.2.0/tsugu_api_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

