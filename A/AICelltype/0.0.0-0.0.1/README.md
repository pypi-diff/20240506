# Comparing `tmp/aicelltype-0.0.0.tar.gz` & `tmp/aicelltype-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicelltype-0.0.0.tar", last modified: Sun May  5 14:31:33 2024, max compression
+gzip compressed data, was "aicelltype-0.0.1.tar", last modified: Sun May  5 16:41:25 2024, max compression
```

## Comparing `aicelltype-0.0.0.tar` & `aicelltype-0.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 14:31:33.178573 aicelltype-0.0.0/
--rw-rw-rw-   0        0        0        0 2024-02-03 13:10:46.000000 aicelltype-0.0.0/LICENSE
--rw-rw-rw-   0        0        0        0 2024-02-03 13:12:25.000000 aicelltype-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      722 2024-05-05 14:31:33.178573 aicelltype-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      115 2024-05-04 15:12:43.000000 aicelltype-0.0.0/README.md
--rw-rw-rw-   0        0        0      684 2024-05-04 15:24:16.000000 aicelltype-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-05 14:31:33.178573 aicelltype-0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-05 14:31:33.163036 aicelltype-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-05 14:31:33.163036 aicelltype-0.0.0/src/AICelltype/
--rw-rw-rw-   0        0        0     4905 2024-05-05 14:28:30.000000 aicelltype-0.0.0/src/AICelltype/__init__.py
--rw-rw-rw-   0        0        0       21 2024-05-05 04:52:48.000000 aicelltype-0.0.0/src/AICelltype/aicelltype.py
-drwxrwxrwx   0        0        0        0 2024-05-05 14:31:33.178573 aicelltype-0.0.0/src/AICelltype.egg-info/
--rw-rw-rw-   0        0        0      722 2024-05-05 14:31:33.000000 aicelltype-0.0.0/src/AICelltype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-05 14:31:33.000000 aicelltype-0.0.0/src/AICelltype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 14:31:33.000000 aicelltype-0.0.0/src/AICelltype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-05 14:31:33.000000 aicelltype-0.0.0/src/AICelltype.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-05 14:31:33.000000 aicelltype-0.0.0/src/AICelltype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      490 2024-02-03 13:12:00.000000 aicelltype-0.0.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 16:41:25.697567 aicelltype-0.0.1/
+-rw-rw-rw-   0        0        0        0 2024-02-03 13:10:46.000000 aicelltype-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0        0 2024-02-03 13:12:25.000000 aicelltype-0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      727 2024-05-05 16:41:25.697567 aicelltype-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2024-05-05 16:01:16.000000 aicelltype-0.0.1/README.md
+-rw-rw-rw-   0        0        0      684 2024-05-05 14:34:53.000000 aicelltype-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-05 16:41:25.697567 aicelltype-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 16:41:25.675433 aicelltype-0.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-05 16:41:25.675433 aicelltype-0.0.1/src/AICelltype/
+-rw-rw-rw-   0        0        0     5009 2024-05-05 16:41:08.000000 aicelltype-0.0.1/src/AICelltype/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-05-05 04:52:48.000000 aicelltype-0.0.1/src/AICelltype/aicelltype.py
+drwxrwxrwx   0        0        0        0 2024-05-05 16:41:25.697567 aicelltype-0.0.1/src/AICelltype.egg-info/
+-rw-rw-rw-   0        0        0      727 2024-05-05 16:41:25.000000 aicelltype-0.0.1/src/AICelltype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-05 16:41:25.000000 aicelltype-0.0.1/src/AICelltype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 16:41:25.000000 aicelltype-0.0.1/src/AICelltype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-05 16:41:25.000000 aicelltype-0.0.1/src/AICelltype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-05 16:41:25.000000 aicelltype-0.0.1/src/AICelltype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      490 2024-02-03 13:12:00.000000 aicelltype-0.0.1/src/__init__.py
```

### Comparing `aicelltype-0.0.0/PKG-INFO` & `aicelltype-0.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: AICelltype
-Version: 0.0.0
+Version: 0.0.1
 Summary: AICelltype: Annotate cell type through AI/LLM/GPT
 Author-email: renzhg <rzgedu@163.com>
 Project-URL: Homepage, https://github.com/renzhonggan/AICelltype
 Project-URL: Bug Tracker, https://github.com/renzhonggan/AICelltype/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dashscope==1.17.1
 Requires-Dist: requests==2.31.0
 
-# spSAM
+# AICelltype
 
 Please refer to the 
 [AICelltype](https://github.com/renzhonggan/AICelltype) for detailed tutorial.
```

### Comparing `aicelltype-0.0.0/pyproject.toml` & `aicelltype-0.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "AICelltype"
-version = "0.0.0"
+version = "0.0.1"
 authors = [
   { name = "renzhg", email = "rzgedu@163.com" },
 ]
 dependencies = ['dashscope==1.17.1', 'requests==2.31.0']
 description = "AICelltype: Annotate cell type through AI/LLM/GPT"
 readme = "README.md"
 requires-python = ">=3.10.0"
```

### Comparing `aicelltype-0.0.0/src/AICelltype/__init__.py` & `aicelltype-0.0.1/src/AICelltype/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """AICelltype: Annotate cell type through AI/LLM/GPT"""
 
 import requests
 import re
 import json
+import os
 
 from http import HTTPStatus
 from dashscope import Generation
 import dashscope
-global_variables_dt = globals()
-dashscope.api_key = global_variables_dt.get('qwen_key', '')
-API_KEY = global_variables_dt.get('API_KEY', '')
-SECRET_KEY = global_variables_dt.get('SECRET_KEY', '')
+
+dashscope.api_key = os.environ.get('QWEN_KEY', '')
+API_KEY = os.environ.get('API_KEY', '')
+SECRET_KEY = os.environ.get('SECRET_KEY', '')
 
 
 def aicelltype(issue_name, gene_list, model='gpt4'):
     if model == 'gpt4':
         cell_lt = gpt4(issue_name, gene_list)
     elif model == 'qwen-max':
-        print(dashscope.api_key)
+        # print(dashscope.api_key)
         cell_lt = qwen(issue_name, gene_list)
     elif model == 'ERNIE-4.0':
+        # print(API_KEY, SECRET_KEY)
         cell_lt = ernie(issue_name, gene_list)
     else:
         print(f'error:model {model} no found, choose one from ["gpt4", "qwen-max", "ERNIE-4.0"]')
         return
     return cell_lt
 
 
@@ -81,17 +83,16 @@
         return [''] * len(gene_list)
 
 
 def ernie(issue_name, gene_list):
     gene_str = '\n'.join([','.join(i) for i in gene_list])
     input_msg = f'Identify cell types of {issue_name} cells using the following markers. Identify one cell type for each row. Only provide the cell type name and nothing else. Some could be a mixture of multiple cell types. Some could be unknown cell types.\n{gene_str}'
     # print(input_msg)
-
+    # print('token', get_access_token())
     url = "https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/ernie-4.0-8k-preview?access_token=" + get_access_token()
-
     payload = json.dumps({
         "messages": [
             {
                 "role": "user",
                 "content": input_msg
             },
         ],
@@ -100,26 +101,27 @@
     })
     headers = {
         'Content-Type': 'application/json'
     }
 
     response = requests.request("POST", url, headers=headers, data=payload)
     if response.status_code == 200:
-        # print(response.text)
+        # print('response', response.text)
         # print('\n')
         res_js = response.json()
         cell_lt = res_js['result'].split('\n')[:len(gene_list)]
         return cell_lt
     else:
         print(f"failed:{response.status_code}")
         return [''] * len(gene_list)
 
 
 def get_access_token():
     """
     use AK, SK generate(Access Token)
     :return: access_token or None(if wrong)
     """
+    # print('API_KEY:', API_KEY, 'SECRET_KEY:', SECRET_KEY)
     url = "https://aip.baidubce.com/oauth/2.0/token"
     params = {"grant_type": "client_credentials", "client_id": API_KEY, "client_secret": SECRET_KEY}
     return str(requests.post(url, params=params).json().get("access_token"))
```

### Comparing `aicelltype-0.0.0/src/AICelltype.egg-info/PKG-INFO` & `aicelltype-0.0.1/src/AICelltype.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: AICelltype
-Version: 0.0.0
+Version: 0.0.1
 Summary: AICelltype: Annotate cell type through AI/LLM/GPT
 Author-email: renzhg <rzgedu@163.com>
 Project-URL: Homepage, https://github.com/renzhonggan/AICelltype
 Project-URL: Bug Tracker, https://github.com/renzhonggan/AICelltype/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dashscope==1.17.1
 Requires-Dist: requests==2.31.0
 
-# spSAM
+# AICelltype
 
 Please refer to the 
 [AICelltype](https://github.com/renzhonggan/AICelltype) for detailed tutorial.
```

