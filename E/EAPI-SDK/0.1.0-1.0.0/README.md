# Comparing `tmp/eapi_sdk-0.1.0.tar.gz` & `tmp/eapi_sdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eapi_sdk-0.1.0.tar", last modified: Sat Apr 27 16:52:02 2024, max compression
+gzip compressed data, was "eapi_sdk-1.0.0.tar", last modified: Mon May  6 07:09:48 2024, max compression
```

## Comparing `eapi_sdk-0.1.0.tar` & `eapi_sdk-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 16:52:02.862869 eapi_sdk-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-04-27 16:52:02.859869 eapi_sdk-0.1.0/EAPI_SDK.egg-info/
--rw-rw-rw-   0        0        0      322 2024-04-27 16:52:02.000000 eapi_sdk-0.1.0/EAPI_SDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-04-27 16:52:02.000000 eapi_sdk-0.1.0/EAPI_SDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 16:52:02.000000 eapi_sdk-0.1.0/EAPI_SDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-27 16:52:02.000000 eapi_sdk-0.1.0/EAPI_SDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-27 16:52:02.000000 eapi_sdk-0.1.0/EAPI_SDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      322 2024-04-27 16:52:02.860864 eapi_sdk-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-22 12:47:14.000000 eapi_sdk-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 16:52:02.857870 eapi_sdk-0.1.0/eapi-sdk/
--rw-rw-rw-   0        0        0      501 2024-04-26 04:15:10.000000 eapi_sdk-0.1.0/eapi-sdk/__init__.py
--rw-rw-rw-   0        0        0     3426 2024-04-26 06:06:46.000000 eapi_sdk-0.1.0/eapi-sdk/client.py
--rw-rw-rw-   0        0        0     1524 2024-04-22 13:32:59.000000 eapi_sdk-0.1.0/eapi-sdk/exceptions.py
--rw-rw-rw-   0        0        0      455 2024-04-26 06:03:37.000000 eapi_sdk-0.1.0/eapi-sdk/main.py
--rw-rw-rw-   0        0        0      974 2024-04-22 13:03:17.000000 eapi_sdk-0.1.0/eapi-sdk/models.py
--rw-rw-rw-   0        0        0     1225 2024-04-22 13:10:59.000000 eapi_sdk-0.1.0/eapi-sdk/utils.py
--rw-rw-rw-   0        0        0     1091 2024-04-27 08:12:45.000000 eapi_sdk-0.1.0/licence.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 16:52:02.862869 eapi_sdk-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      415 2024-04-27 16:39:19.000000 eapi_sdk-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:09:48.093708 eapi_sdk-1.0.0/
+drwxrwxrwx   0        0        0        0 2024-05-06 07:09:48.090719 eapi_sdk-1.0.0/EAPI_SDK.egg-info/
+-rw-rw-rw-   0        0        0      322 2024-05-06 07:09:47.000000 eapi_sdk-1.0.0/EAPI_SDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-05-06 07:09:47.000000 eapi_sdk-1.0.0/EAPI_SDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 07:09:47.000000 eapi_sdk-1.0.0/EAPI_SDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-06 07:09:47.000000 eapi_sdk-1.0.0/EAPI_SDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-06 07:09:47.000000 eapi_sdk-1.0.0/EAPI_SDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      322 2024-05-06 07:09:48.092712 eapi_sdk-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:47:14.000000 eapi_sdk-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 07:09:48.089722 eapi_sdk-1.0.0/eapi-sdk/
+-rw-rw-rw-   0        0        0      501 2024-04-26 04:15:10.000000 eapi_sdk-1.0.0/eapi-sdk/__init__.py
+-rw-rw-rw-   0        0        0     3303 2024-05-06 06:52:14.000000 eapi_sdk-1.0.0/eapi-sdk/client.py
+-rw-rw-rw-   0        0        0     1524 2024-04-22 13:32:59.000000 eapi_sdk-1.0.0/eapi-sdk/exceptions.py
+-rw-rw-rw-   0        0        0      434 2024-05-06 06:35:41.000000 eapi_sdk-1.0.0/eapi-sdk/main.py
+-rw-rw-rw-   0        0        0      974 2024-04-22 13:03:17.000000 eapi_sdk-1.0.0/eapi-sdk/models.py
+-rw-rw-rw-   0        0        0     1225 2024-04-22 13:10:59.000000 eapi_sdk-1.0.0/eapi-sdk/utils.py
+-rw-rw-rw-   0        0        0     1091 2024-04-27 08:12:45.000000 eapi_sdk-1.0.0/licence.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 07:09:48.093708 eapi_sdk-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      415 2024-05-06 06:55:31.000000 eapi_sdk-1.0.0/setup.py
```

### Comparing `eapi_sdk-0.1.0/eapi-sdk/client.py` & `eapi_sdk-1.0.0/eapi-sdk/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from requests.auth import HTTPBasicAuth
 from typing import Dict, Any
 import hashlib
 import time
 
 
 class EAPIClient:
-    def __init__(self, access_key: str, secret_key: str, base_url='http://192.168.3.5:8090/api/interfaceInfo/invoke'):
+    def __init__(self, access_key: str, secret_key: str, base_url='http://121.40.232.157:8090/api/interfaceInfo/invoke'):
         """
         初始化OpenAPI客户端
         :param access_key: OpenAPI平台的Access Key
         :param secret_key: OpenAPI平台的Secret Key
         :param base_url: OpenAPI平台的基础URL，默认值为'部署后的url'
         """
         self.access_key = access_key
@@ -50,30 +50,27 @@
         }
         json_finload = {
             'id': id,
             'userRequestParams': json_payload
         }
         if json_payload is not None:
             response = requests.post(self.base_url, json=json_finload, headers=headers, verify=False)
-            answer = json.loads(response.text)
-            print(answer.get('data'))
-            return answer.get('data')
+            return response.json().get("data")
         else:
             response = requests.request(method, self.base_url, auth=self.auth, headers=headers)
             return response
     def call_api(self, params: Dict[str, Any], interfaceInfoId: int, method: str = 'POST'):
         """
         根据接口名称调用OpenAPI接口
         :param interfaceInfoId: 接口id
         :param interfaceInfoId:
         :param params: JSON格式的请求参数
         :param method: HTTP请求方法，默认为'POST'
         :return: 响应的JSON数据
         """
         # 假设接口路径是固定的，可以根据实际情况调整
         # 替换为实际的接口版本和接口路径
-        print(method, params, interfaceInfoId)
         return self._make_request(method, interfaceInfoId, params)
 
 # 示例：调用名为'get_user_info'的接口
 # client = OpenAPIClient('your_access_key', 'your_secret_key')
 # user_info = client.call_api('get_user_info', {'user_id': '123'})
```

### Comparing `eapi_sdk-0.1.0/eapi-sdk/exceptions.py` & `eapi_sdk-1.0.0/eapi-sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `eapi_sdk-0.1.0/eapi-sdk/models.py` & `eapi_sdk-1.0.0/eapi-sdk/models.py`

 * *Files identical despite different names*

### Comparing `eapi_sdk-0.1.0/eapi-sdk/utils.py` & `eapi_sdk-1.0.0/eapi-sdk/utils.py`

 * *Files identical despite different names*

### Comparing `eapi_sdk-0.1.0/licence.txt` & `eapi_sdk-1.0.0/licence.txt`

 * *Files identical despite different names*

