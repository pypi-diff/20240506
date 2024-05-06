# Comparing `tmp/py_ce_forms_api-0.0.6.tar.gz` & `tmp/py_ce_forms_api-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ce_forms_api-0.0.6.tar", last modified: Mon Apr 22 11:12:17 2024, max compression
+gzip compressed data, was "py_ce_forms_api-0.0.7.tar", last modified: Mon May  6 12:39:33 2024, max compression
```

## Comparing `py_ce_forms_api-0.0.6.tar` & `py_ce_forms_api-0.0.7.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 jeanpul    (501) staff       (20)        0 2024-04-22 11:12:17.100582 py_ce_forms_api-0.0.6/
--rw-r--r--   0 jeanpul    (501) staff       (20)    11339 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/LICENSE
--rw-r--r--   0 jeanpul    (501) staff       (20)     1923 2024-04-22 11:12:17.100475 py_ce_forms_api-0.0.6/PKG-INFO
--rw-r--r--   0 jeanpul    (501) staff       (20)     1160 2024-04-22 10:25:59.000000 py_ce_forms_api-0.0.6/README.md
-drwxr-xr-x   0 jeanpul    (501) staff       (20)        0 2024-04-22 11:12:17.095589 py_ce_forms_api-0.0.6/py_ce_forms_api/
--rw-r--r--   0 jeanpul    (501) staff       (20)      265 2024-04-22 11:05:23.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/__init__.py
-drwxr-xr-x   0 jeanpul    (501) staff       (20)        0 2024-04-22 11:12:17.096564 py_ce_forms_api-0.0.6/py_ce_forms_api/accounts/
--rw-r--r--   0 jeanpul    (501) staff       (20)       30 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/accounts/__init__.py
--rw-r--r--   0 jeanpul    (501) staff       (20)      529 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/accounts/accounts.py
-drwxr-xr-x   0 jeanpul    (501) staff       (20)        0 2024-04-22 11:12:17.097936 py_ce_forms_api-0.0.6/py_ce_forms_api/api/
--rw-r--r--   0 jeanpul    (501) staff       (20)       85 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/api/__init__.py
--rw-r--r--   0 jeanpul    (501) staff       (20)      220 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/api/bearer_auth.py
--rw-r--r--   0 jeanpul    (501) staff       (20)     3138 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/api/client.py
--rw-r--r--   0 jeanpul    (501) staff       (20)       72 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/api/exceptions.py
--rw-r--r--   0 jeanpul    (501) staff       (20)       58 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/api/modules.py
-drwxr-xr-x   0 jeanpul    (501) staff       (20)        0 2024-04-22 11:12:17.098201 py_ce_forms_api-0.0.6/py_ce_forms_api/assets/
--rw-r--r--   0 jeanpul    (501) staff       (20)       26 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/assets/__init__.py
--rw-r--r--   0 jeanpul    (501) staff       (20)     1303 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/assets/assets.py
--rw-r--r--   0 jeanpul    (501) staff       (20)      977 2024-04-22 11:05:47.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/client.py
-drwxr-xr-x   0 jeanpul    (501) staff       (20)        0 2024-04-22 11:12:17.098462 py_ce_forms_api-0.0.6/py_ce_forms_api/form/
--rw-r--r--   0 jeanpul    (501) staff       (20)       23 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/form/__init__.py
--rw-r--r--   0 jeanpul    (501) staff       (20)      331 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/form/form.py
-drwxr-xr-x   0 jeanpul    (501) staff       (20)        0 2024-04-22 11:12:17.099018 py_ce_forms_api-0.0.6/py_ce_forms_api/processing/
--rw-r--r--   0 jeanpul    (501) staff       (20)       89 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/processing/__init__.py
--rw-r--r--   0 jeanpul    (501) staff       (20)     1610 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/processing/processing.py
--rw-r--r--   0 jeanpul    (501) staff       (20)     1605 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/processing/task.py
--rw-r--r--   0 jeanpul    (501) staff       (20)     1710 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/processing/task_pool.py
-drwxr-xr-x   0 jeanpul    (501) staff       (20)        0 2024-04-22 11:12:17.100303 py_ce_forms_api-0.0.6/py_ce_forms_api/query/
--rw-r--r--   0 jeanpul    (501) staff       (20)       72 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/query/__init__.py
--rw-r--r--   0 jeanpul    (501) staff       (20)      478 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/query/form_mutate.py
--rw-r--r--   0 jeanpul    (501) staff       (20)     2077 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/query/forms_query.py
--rw-r--r--   0 jeanpul    (501) staff       (20)      149 2024-04-22 09:22:59.000000 py_ce_forms_api-0.0.6/py_ce_forms_api/query/forms_res.py
-drwxr-xr-x   0 jeanpul    (501) staff       (20)        0 2024-04-22 11:12:17.096212 py_ce_forms_api-0.0.6/py_ce_forms_api.egg-info/
--rw-r--r--   0 jeanpul    (501) staff       (20)     1923 2024-04-22 11:12:17.000000 py_ce_forms_api-0.0.6/py_ce_forms_api.egg-info/PKG-INFO
--rw-r--r--   0 jeanpul    (501) staff       (20)      938 2024-04-22 11:12:17.000000 py_ce_forms_api-0.0.6/py_ce_forms_api.egg-info/SOURCES.txt
--rw-r--r--   0 jeanpul    (501) staff       (20)        1 2024-04-22 11:12:17.000000 py_ce_forms_api-0.0.6/py_ce_forms_api.egg-info/dependency_links.txt
--rw-r--r--   0 jeanpul    (501) staff       (20)       25 2024-04-22 11:12:17.000000 py_ce_forms_api-0.0.6/py_ce_forms_api.egg-info/requires.txt
--rw-r--r--   0 jeanpul    (501) staff       (20)       16 2024-04-22 11:12:17.000000 py_ce_forms_api-0.0.6/py_ce_forms_api.egg-info/top_level.txt
--rw-r--r--   0 jeanpul    (501) staff       (20)       38 2024-04-22 11:12:17.100628 py_ce_forms_api-0.0.6/setup.cfg
--rw-r--r--   0 jeanpul    (501) staff       (20)     1144 2024-04-22 11:12:05.000000 py_ce_forms_api-0.0.6/setup.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2024-05-06 12:39:33.697522 py_ce_forms_api-0.0.7/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)    11339 2023-11-24 13:30:41.000000 py_ce_forms_api-0.0.7/LICENSE
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1923 2024-05-06 12:39:33.697522 py_ce_forms_api-0.0.7/PKG-INFO
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1160 2024-04-30 08:25:12.000000 py_ce_forms_api-0.0.7/README.md
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2024-05-06 12:39:33.693522 py_ce_forms_api-0.0.7/py_ce_forms_api/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      286 2024-04-30 13:26:36.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/__init__.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2024-05-06 12:39:33.697522 py_ce_forms_api-0.0.7/py_ce_forms_api/accounts/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       30 2024-04-30 08:25:12.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/accounts/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      529 2024-04-30 08:25:12.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/accounts/accounts.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2024-05-06 12:39:33.697522 py_ce_forms_api-0.0.7/py_ce_forms_api/api/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       85 2024-04-30 08:25:12.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/api/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      220 2024-04-30 08:25:12.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/api/bearer_auth.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     3415 2024-05-02 12:53:21.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/api/client.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       72 2024-04-30 08:25:12.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/api/exceptions.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       58 2024-04-30 08:25:12.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/api/modules.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2024-05-06 12:39:33.697522 py_ce_forms_api-0.0.7/py_ce_forms_api/assets/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       26 2024-04-30 08:25:12.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/assets/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1303 2024-04-30 08:25:12.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/assets/assets.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     2376 2024-05-02 13:23:50.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/client.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2024-05-06 12:39:33.697522 py_ce_forms_api-0.0.7/py_ce_forms_api/form/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       57 2024-04-30 13:21:30.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/form/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1139 2024-04-30 13:25:22.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/form/form.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1670 2024-04-30 13:19:58.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/form/form_block.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2024-05-06 12:39:33.697522 py_ce_forms_api-0.0.7/py_ce_forms_api/processing/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       89 2024-04-30 08:25:12.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/processing/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1610 2024-04-30 08:25:12.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/processing/processing.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1605 2024-04-30 08:25:12.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/processing/task.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1710 2024-04-30 08:25:12.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/processing/task_pool.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2024-05-06 12:39:33.697522 py_ce_forms_api-0.0.7/py_ce_forms_api/query/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      105 2024-04-30 08:40:40.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/query/__init__.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      478 2024-04-30 08:25:12.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/query/form_mutate.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     2119 2024-04-30 08:41:22.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/query/forms_query.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      591 2024-04-30 09:29:30.000000 py_ce_forms_api-0.0.7/py_ce_forms_api/query/forms_res.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2024-05-06 12:39:33.693522 py_ce_forms_api-0.0.7/py_ce_forms_api.egg-info/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1923 2024-05-06 12:39:33.000000 py_ce_forms_api-0.0.7/py_ce_forms_api.egg-info/PKG-INFO
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      973 2024-05-06 12:39:33.000000 py_ce_forms_api-0.0.7/py_ce_forms_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)        1 2024-05-06 12:39:33.000000 py_ce_forms_api-0.0.7/py_ce_forms_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       25 2024-05-06 12:39:33.000000 py_ce_forms_api-0.0.7/py_ce_forms_api.egg-info/requires.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       16 2024-05-06 12:39:33.000000 py_ce_forms_api-0.0.7/py_ce_forms_api.egg-info/top_level.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       38 2024-05-06 12:39:33.697522 py_ce_forms_api-0.0.7/setup.cfg
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1144 2024-05-06 12:35:51.000000 py_ce_forms_api-0.0.7/setup.py
```

### Comparing `py_ce_forms_api-0.0.6/LICENSE` & `py_ce_forms_api-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ce_forms_api-0.0.6/PKG-INFO` & `py_ce_forms_api-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_ce_forms_api
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python library for the CeForms API.
 Home-page: UNKNOWN
 Author: codeffekt
 Author-email: contact@codeffekt.com
 License: UNKNOWN
 Keywords: python,ceforms,api
 Platform: UNKNOWN
```

### Comparing `py_ce_forms_api-0.0.6/README.md` & `py_ce_forms_api-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `py_ce_forms_api-0.0.6/py_ce_forms_api/accounts/accounts.py` & `py_ce_forms_api-0.0.7/py_ce_forms_api/accounts/accounts.py`

 * *Files identical despite different names*

### Comparing `py_ce_forms_api-0.0.6/py_ce_forms_api/api/client.py` & `py_ce_forms_api-0.0.7/py_ce_forms_api/api/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,35 +2,42 @@
 import requests
 from .bearer_auth import BearerAuth
 from .modules import *
 from .exceptions import *
 
 class APIClient():
     """
-    A low-level client for the CeForms API.
+    A low-level client for the CeForms API.    
     
     Example:
     
         >>> import ce_forms
-        >>> client = ce_forms.APIClient(base_url='', token='')        
+        >>> client = ce_forms.APIClient(base_url='', token='')
+        
+    Args:
+        base_url (str): URL to the CeForms API server.
+        token (str): API token provided by a CeForms backend.
     
     """
     
     def __init__(self, base_url=None, token=None):
         super().__init__()
         
         if base_url is None:
             self.base_url = os.environ.get("CE_FORMS_BASE_URL")
         else:     
             self.base_url = base_url
             
         if token is None:
             self.token = os.environ.get("CE_FORMS_TOKEN")
         else:    
-            self.token = token
+            self.token = token            
+        
+        if self.base_url is None or self.token is None:
+            raise TypeError("Invalid base_url or token None value")
         
     def self(self):
         response = requests.get(f'{self.base_url}/self', auth=BearerAuth(self.token))
         return response.json()
     
     def call_module(self, func, params, module_name):
         return self.call(f'Public{module_name}', func_name=func, func_params=params)
```

### Comparing `py_ce_forms_api-0.0.6/py_ce_forms_api/assets/assets.py` & `py_ce_forms_api-0.0.7/py_ce_forms_api/assets/assets.py`

 * *Files identical despite different names*

### Comparing `py_ce_forms_api-0.0.6/py_ce_forms_api/client.py` & `py_ce_forms_api-0.0.7/py_ce_forms_api/form/form.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,32 @@
-from .api.client import APIClient
-from .query import FormsQuery, FormMutate
-from .accounts.accounts import Accounts
-from .assets.assets import Assets
-from .processing.processing import Processing
-class CeFormsClient:
+from datetime import datetime
+from .form_block import FormBlock
+class Form:
     """
-    A client form communication with a CeForms server.
-    
-    Example:
-    
-        >>> import py_ce_forms_api
-        >>> client = py_ce_forms_api.CeFormsClient()
-        >>> client.query().with_root('forms-account').with_sub_forms(False).with_limit(1).call()
+    An utility class to manipulate form properties
     """
-    def __init__(self, *args, **kwargs):
-        self.api = APIClient(*args, **kwargs)
+    def __init__(self, form) -> None:
+        self.form = form
     
-    def self(self):
-        return self.api.self()
+    def set_value(self, field: str, value):
+        self.get_block(field).set_value(value)
+        return self    
     
-    def query(self):
-        return FormsQuery(self.api)
+    def get_value(self, field: str):
+        return self.get_block(field).get_value()        
     
-    def mutation(self):
-        return FormMutate(self.api)
+    def get_block(self, field: str) -> FormBlock:
+        return FormBlock(self.form["content"][field])
     
-    def accounts(self):
-        return Accounts(self.api)
+    def id(self):
+        return self.form["id"]
     
-    def assets(self):
-        return Assets(self.api)
+    def __str__(self) -> str:
+        modified_at = f'modified at {self.mtime().isoformat(" ", "seconds")}' if self.form["mtime"] is not None else ''
+        return f'Form {self.form["id"]} from root {self.form["root"]} {modified_at} created at {self.ctime().isoformat(" ", "seconds")}'
     
-    def processing(self, task):
-        return Processing(self.api, task)
-
+    def ctime(self) -> datetime:
+        return datetime.fromtimestamp(self.form["ctime"] / 1000)
     
+    def mtime(self) -> datetime|None:
+        return datetime.fromtimestamp(self.form["mtime"] / 1000) if self.form["mtime"] is not None else None
```

### Comparing `py_ce_forms_api-0.0.6/py_ce_forms_api/processing/processing.py` & `py_ce_forms_api-0.0.7/py_ce_forms_api/processing/processing.py`

 * *Files identical despite different names*

### Comparing `py_ce_forms_api-0.0.6/py_ce_forms_api/processing/task.py` & `py_ce_forms_api-0.0.7/py_ce_forms_api/processing/task.py`

 * *Files identical despite different names*

### Comparing `py_ce_forms_api-0.0.6/py_ce_forms_api/processing/task_pool.py` & `py_ce_forms_api-0.0.7/py_ce_forms_api/processing/task_pool.py`

 * *Files identical despite different names*

### Comparing `py_ce_forms_api-0.0.6/py_ce_forms_api/query/forms_query.py` & `py_ce_forms_api-0.0.7/py_ce_forms_api/query/forms_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ..api.client import APIClient
 from ..api.modules import *
+from .forms_res import FormsRes
 
 class FormsQuery():
     """
     An utility class to query the forms dataset.
     """
     
     def __init__(self, client: APIClient) -> None:
@@ -55,20 +56,20 @@
         return self
     
     def _add_query_field(self, qf):
         self.query_fields.append(qf)
         return self
     
     def call(self):
-        return self.client.call_forms_query({
+        return FormsRes(self.client.call_forms_query({
                     "extMode": self.extMode,
                     "limit": self.limit,
                     "offset": self.offset,
                     "queryFields": self.query_fields
-                }, self.module_name)
+                }, self.module_name))
     
     def call_single(self, id: str):
         return self.client.call_form_query(id, {
                     "extMode": self.extMode,
                     "limit": self.limit,
                     "offset": self.offset,
                     "queryFields": self.query_fields
```

### Comparing `py_ce_forms_api-0.0.6/py_ce_forms_api.egg-info/PKG-INFO` & `py_ce_forms_api-0.0.7/py_ce_forms_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ce-forms-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python library for the CeForms API.
 Home-page: UNKNOWN
 Author: codeffekt
 Author-email: contact@codeffekt.com
 License: UNKNOWN
 Keywords: python,ceforms,api
 Platform: UNKNOWN
```

### Comparing `py_ce_forms_api-0.0.6/py_ce_forms_api.egg-info/SOURCES.txt` & `py_ce_forms_api-0.0.7/py_ce_forms_api.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 py_ce_forms_api/api/client.py
 py_ce_forms_api/api/exceptions.py
 py_ce_forms_api/api/modules.py
 py_ce_forms_api/assets/__init__.py
 py_ce_forms_api/assets/assets.py
 py_ce_forms_api/form/__init__.py
 py_ce_forms_api/form/form.py
+py_ce_forms_api/form/form_block.py
 py_ce_forms_api/processing/__init__.py
 py_ce_forms_api/processing/processing.py
 py_ce_forms_api/processing/task.py
 py_ce_forms_api/processing/task_pool.py
 py_ce_forms_api/query/__init__.py
 py_ce_forms_api/query/form_mutate.py
 py_ce_forms_api/query/forms_query.py
```

### Comparing `py_ce_forms_api-0.0.6/setup.py` & `py_ce_forms_api-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'A Python library for the CeForms API.'
 
 setup(
     name="py_ce_forms_api",
     version=VERSION,
     author='codeffekt',
     author_email='contact@codeffekt.com',
```

