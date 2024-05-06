# Comparing `tmp/migoapiclient-1.1.8.tar.gz` & `tmp/migoapiclient-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migoapiclient-1.1.8.tar", last modified: Thu Apr 18 11:00:18 2024, max compression
+gzip compressed data, was "migoapiclient-1.1.9.tar", last modified: Sun May  5 10:06:58 2024, max compression
```

## Comparing `migoapiclient-1.1.8.tar` & `migoapiclient-1.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 11:00:18.141918 migoapiclient-1.1.8/
--rw-rw-rw-   0        0        0     3900 2024-04-18 11:00:18.141918 migoapiclient-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 11:00:18.133909 migoapiclient-1.1.8/migoapiclient/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.1.8/migoapiclient/__init__.py
--rw-rw-rw-   0        0        0    12320 2024-04-18 10:59:25.000000 migoapiclient-1.1.8/migoapiclient/api_client.py
--rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.1.8/migoapiclient/file_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:00:18.140919 migoapiclient-1.1.8/migoapiclient.egg-info/
--rw-rw-rw-   0        0        0     3900 2024-04-18 11:00:18.000000 migoapiclient-1.1.8/migoapiclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-18 11:00:18.000000 migoapiclient-1.1.8/migoapiclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 11:00:18.000000 migoapiclient-1.1.8/migoapiclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-18 11:00:18.000000 migoapiclient-1.1.8/migoapiclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 11:00:18.141918 migoapiclient-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     3898 2024-04-18 10:59:25.000000 migoapiclient-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:00:18.140919 migoapiclient-1.1.8/src/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.1.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 10:06:58.355706 migoapiclient-1.1.9/
+-rw-rw-rw-   0        0        0     3900 2024-05-05 10:06:58.355706 migoapiclient-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 10:06:58.351705 migoapiclient-1.1.9/migoapiclient/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.1.9/migoapiclient/__init__.py
+-rw-rw-rw-   0        0        0    12638 2024-05-05 10:04:36.000000 migoapiclient-1.1.9/migoapiclient/api_client.py
+-rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.1.9/migoapiclient/file_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-05 10:06:58.354705 migoapiclient-1.1.9/migoapiclient.egg-info/
+-rw-rw-rw-   0        0        0     3900 2024-05-05 10:06:58.000000 migoapiclient-1.1.9/migoapiclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-05-05 10:06:58.000000 migoapiclient-1.1.9/migoapiclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 10:06:58.000000 migoapiclient-1.1.9/migoapiclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-05 10:06:58.000000 migoapiclient-1.1.9/migoapiclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 10:06:58.355706 migoapiclient-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     3898 2024-05-05 10:06:52.000000 migoapiclient-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 10:06:58.354705 migoapiclient-1.1.9/src/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.1.9/src/__init__.py
```

### Comparing `migoapiclient-1.1.8/PKG-INFO` & `migoapiclient-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.1.8
+Version: 1.1.9
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.1.8/README.md` & `migoapiclient-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.1.8/migoapiclient/api_client.py` & `migoapiclient-1.1.9/migoapiclient/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,14 +300,22 @@
         post_data = {
             'sourceStrings': column_list,
             'queryString': json.dumps(es_query),
             'indexName': table_name
         }
         return self.migo_try_post(self.host + uri, 0, '获取节点信息', 0, json=post_data)
 
+    def get_third_party_auths(self, auth_id: int):
+        """
+        获取第三方平台授权信息
+        :param auth_id
+        """
+        uri = f'/data-collection-service/node/thirdpartyauths/{auth_id}'
+        return self.migo_try_get(self.host + uri, auth_id, '获取第三方平台授权信息')
+
     def post_schedule_log(self, msg: str, shop_id: str, definition_info: dict, log_params: dict = None):
         """
         上传日志
         :param msg 信息
         :param shop_id 店铺ID
         :param definition_info 策略信息
         :param log_params 其他信息
```

### Comparing `migoapiclient-1.1.8/migoapiclient/file_manager.py` & `migoapiclient-1.1.9/migoapiclient/file_manager.py`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.1.8/migoapiclient.egg-info/PKG-INFO` & `migoapiclient-1.1.9/migoapiclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.1.8
+Version: 1.1.9
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.1.8/setup.py` & `migoapiclient-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'migoapiclient'
 DESCRIPTION = '米果请求API客户端'
 URL = 'https://github.com/me/myproject'
 EMAIL = '2920167524@qq.com'
 AUTHOR = 'pykira'
 REQUIRES_PYTHON = '>=3.5.0'
-VERSION = '1.1.8'
+VERSION = '1.1.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

