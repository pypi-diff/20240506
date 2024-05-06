# Comparing `tmp/HandyLLM-0.6.3.tar.gz` & `tmp/handyllm-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HandyLLM-0.6.3.tar", last modified: Sat Apr 13 11:22:26 2024, max compression
+gzip compressed data, was "handyllm-0.7.0.tar", last modified: Mon May  6 20:05:43 2024, max compression
```

## Comparing `HandyLLM-0.6.3.tar` & `handyllm-0.7.0.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:22:26.556732 HandyLLM-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-04-13 11:22:26.556732 HandyLLM-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 11:22:26.556732 HandyLLM-0.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:22:26.552732 HandyLLM-0.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:22:26.556732 HandyLLM-0.6.3/src/HandyLLM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-04-13 11:22:26.000000 HandyLLM-0.6.3/src/HandyLLM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-13 11:22:26.000000 HandyLLM-0.6.3/src/HandyLLM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 11:22:26.000000 HandyLLM-0.6.3/src/HandyLLM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 11:22:26.000000 HandyLLM-0.6.3/src/HandyLLM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 11:22:26.000000 HandyLLM-0.6.3/src/HandyLLM.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:22:26.556732 HandyLLM-0.6.3/src/handyllm/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:22:26.556732 HandyLLM-0.6.3/src/handyllm/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/deprecated/api_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/deprecated/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/endpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15434 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/openai_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/prompt_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/requestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/src/handyllm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:22:26.556732 HandyLLM-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/tests/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/tests/test_client_async_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/tests/test_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-13 11:22:22.000000 HandyLLM-0.6.3/tests/test_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:05:43.546211 handyllm-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-06 20:05:43.546211 handyllm-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-06 20:05:39.000000 handyllm-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-06 20:05:39.000000 handyllm-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:05:43.546211 handyllm-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:05:43.542211 handyllm-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:05:43.546211 handyllm-0.7.0/src/HandyLLM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-06 20:05:43.000000 handyllm-0.7.0/src/HandyLLM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-06 20:05:43.000000 handyllm-0.7.0/src/HandyLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:05:43.000000 handyllm-0.7.0/src/HandyLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 20:05:43.000000 handyllm-0.7.0/src/HandyLLM.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-06 20:05:43.000000 handyllm-0.7.0/src/HandyLLM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 20:05:43.000000 handyllm-0.7.0/src/HandyLLM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:05:43.546211 handyllm-0.7.0/src/handyllm/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-06 20:05:39.000000 handyllm-0.7.0/src/handyllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-06 20:05:39.000000 handyllm-0.7.0/src/handyllm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-06 20:05:39.000000 handyllm-0.7.0/src/handyllm/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-06 20:05:39.000000 handyllm-0.7.0/src/handyllm/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-06 20:05:39.000000 handyllm-0.7.0/src/handyllm/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:05:43.546211 handyllm-0.7.0/src/handyllm/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-06 20:05:39.000000 handyllm-0.7.0/src/handyllm/deprecated/api_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-05-06 20:05:39.000000 handyllm-0.7.0/src/handyllm/deprecated/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-06 20:05:39.000000 handyllm-0.7.0/src/handyllm/endpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31633 2024-05-06 20:05:39.000000 handyllm-0.7.0/src/handyllm/hprompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-06 20:05:39.000000 handyllm-0.7.0/src/handyllm/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15434 2024-05-06 20:05:39.000000 handyllm-0.7.0/src/handyllm/openai_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-06 20:05:39.000000 handyllm-0.7.0/src/handyllm/prompt_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-05-06 20:05:39.000000 handyllm-0.7.0/src/handyllm/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-06 20:05:39.000000 handyllm-0.7.0/src/handyllm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:05:43.546211 handyllm-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-06 20:05:39.000000 handyllm-0.7.0/tests/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-06 20:05:39.000000 handyllm-0.7.0/tests/test_client_async_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-06 20:05:39.000000 handyllm-0.7.0/tests/test_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-06 20:05:39.000000 handyllm-0.7.0/tests/test_hprompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-06 20:05:39.000000 handyllm-0.7.0/tests/test_prompt.py
```

### Comparing `HandyLLM-0.6.3/src/HandyLLM.egg-info/SOURCES.txt` & `handyllm-0.7.0/src/HandyLLM.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 README.md
 pyproject.toml
 src/HandyLLM.egg-info/PKG-INFO
 src/HandyLLM.egg-info/SOURCES.txt
 src/HandyLLM.egg-info/dependency_links.txt
+src/HandyLLM.egg-info/entry_points.txt
 src/HandyLLM.egg-info/requires.txt
 src/HandyLLM.egg-info/top_level.txt
 src/handyllm/__init__.py
+src/handyllm/__main__.py
 src/handyllm/_constants.py
 src/handyllm/_utils.py
+src/handyllm/cli.py
 src/handyllm/endpoint_manager.py
+src/handyllm/hprompt.py
 src/handyllm/openai_api.py
 src/handyllm/openai_client.py
 src/handyllm/prompt_converter.py
 src/handyllm/requestor.py
 src/handyllm/utils.py
 src/handyllm/deprecated/api_request.py
 src/handyllm/deprecated/openai_api.py
 tests/test_azure.py
 tests/test_client_async_sync.py
 tests/test_endpoint.py
+tests/test_hprompt.py
 tests/test_prompt.py
```

### Comparing `HandyLLM-0.6.3/src/handyllm/_utils.py` & `handyllm-0.7.0/src/handyllm/_utils.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.3/src/handyllm/deprecated/api_request.py` & `handyllm-0.7.0/src/handyllm/deprecated/api_request.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.3/src/handyllm/deprecated/openai_api.py` & `handyllm-0.7.0/src/handyllm/deprecated/openai_api.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.3/src/handyllm/endpoint_manager.py` & `handyllm-0.7.0/src/handyllm/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.3/src/handyllm/openai_api.py` & `handyllm-0.7.0/src/handyllm/openai_api.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.3/src/handyllm/openai_client.py` & `handyllm-0.7.0/src/handyllm/openai_client.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.3/src/handyllm/prompt_converter.py` & `handyllm-0.7.0/src/handyllm/prompt_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,20 @@
         self.substitute_map = {}
 
     @property
     def split_pattern(self):
         # build a regex pattern to split the prompt by role keys
         return r'^\$(' + '|'.join(self.role_keys) + r')\$$'
 
+    def detect(self, raw_prompt: str):
+        # detect the role keys in the prompt
+        if re.search(self.split_pattern, raw_prompt, flags=re.MULTILINE):
+            return True
+        return False
+
     def read_substitute_content(self, path: str):
         # 从文本文件读取所有prompt中需要替换的内容
         with open(path, 'r', encoding='utf-8') as fin:
             content = fin.read()
     
         self.substitute_map = {}
         blocks = re.split(r'(%\w+%)', content)
```

### Comparing `HandyLLM-0.6.3/src/handyllm/requestor.py` & `handyllm-0.7.0/src/handyllm/requestor.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.3/src/handyllm/utils.py` & `handyllm-0.7.0/src/handyllm/utils.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.3/tests/test_azure.py` & `handyllm-0.7.0/tests/test_azure.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.3/tests/test_client_async_sync.py` & `handyllm-0.7.0/tests/test_client_async_sync.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.3/tests/test_endpoint.py` & `handyllm-0.7.0/tests/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.3/tests/test_prompt.py` & `handyllm-0.7.0/tests/test_prompt.py`

 * *Files identical despite different names*

