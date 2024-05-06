# Comparing `tmp/marketorestpython-0.5.8.tar.gz` & `tmp/marketorestpython-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\marketorestpython-0.5.8.tar", last modified: Thu Dec 24 01:23:07 2020, max compression
+gzip compressed data, was "dist\marketorestpython-0.5.9.tar", last modified: Sun May  9 18:48:05 2021, max compression
```

## Comparing `marketorestpython-0.5.8.tar` & `marketorestpython-0.5.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2020-12-24 01:23:07.000000 marketorestpython-0.5.8/
-drwxrwxrwx   0        0        0        0 2020-12-24 01:23:07.000000 marketorestpython-0.5.8/marketorestpython/
--rw-rw-rw-   0        0        0   221377 2020-12-24 01:16:26.000000 marketorestpython-0.5.8/marketorestpython/client.py
-drwxrwxrwx   0        0        0        0 2020-12-24 01:23:07.000000 marketorestpython-0.5.8/marketorestpython/helper/
--rw-rw-rw-   0        0        0      314 2018-03-30 21:48:54.000000 marketorestpython-0.5.8/marketorestpython/helper/exceptions.py
--rw-rw-rw-   0        0        0     4015 2020-12-19 19:36:16.000000 marketorestpython-0.5.8/marketorestpython/helper/http_lib.py
--rw-rw-rw-   0        0        0        0 2018-03-30 21:48:54.000000 marketorestpython-0.5.8/marketorestpython/helper/__init__.py
--rw-rw-rw-   0        0        0        0 2018-03-30 21:48:54.000000 marketorestpython-0.5.8/marketorestpython/__init__.py
-drwxrwxrwx   0        0        0        0 2020-12-24 01:23:07.000000 marketorestpython-0.5.8/marketorestpython.egg-info/
--rw-rw-rw-   0        0        0        1 2020-12-24 01:23:06.000000 marketorestpython-0.5.8/marketorestpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      512 2020-12-24 01:23:06.000000 marketorestpython-0.5.8/marketorestpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       22 2020-12-24 01:23:06.000000 marketorestpython-0.5.8/marketorestpython.egg-info/requires.txt
--rw-rw-rw-   0        0        0      400 2020-12-24 01:23:07.000000 marketorestpython-0.5.8/marketorestpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       18 2020-12-24 01:23:06.000000 marketorestpython-0.5.8/marketorestpython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      512 2020-12-24 01:23:07.000000 marketorestpython-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0      121 2018-03-30 21:48:54.000000 marketorestpython-0.5.8/README
--rw-rw-rw-   0        0        0       86 2020-12-24 01:23:07.000000 marketorestpython-0.5.8/setup.cfg
--rw-rw-rw-   0        0        0     1180 2020-12-24 01:20:27.000000 marketorestpython-0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-05-09 18:48:05.000000 marketorestpython-0.5.9/
+drwxrwxrwx   0        0        0        0 2021-05-09 18:48:04.000000 marketorestpython-0.5.9/marketorestpython/
+-rw-rw-rw-   0        0        0   225400 2021-05-09 18:43:46.000000 marketorestpython-0.5.9/marketorestpython/client.py
+drwxrwxrwx   0        0        0        0 2021-05-09 18:48:05.000000 marketorestpython-0.5.9/marketorestpython/helper/
+-rw-rw-rw-   0        0        0      314 2018-03-30 21:48:54.000000 marketorestpython-0.5.9/marketorestpython/helper/exceptions.py
+-rw-rw-rw-   0        0        0     4015 2020-12-19 19:36:16.000000 marketorestpython-0.5.9/marketorestpython/helper/http_lib.py
+-rw-rw-rw-   0        0        0        0 2018-03-30 21:48:54.000000 marketorestpython-0.5.9/marketorestpython/helper/__init__.py
+-rw-rw-rw-   0        0        0        0 2018-03-30 21:48:54.000000 marketorestpython-0.5.9/marketorestpython/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-09 18:48:05.000000 marketorestpython-0.5.9/marketorestpython.egg-info/
+-rw-rw-rw-   0        0        0        1 2021-05-09 18:48:04.000000 marketorestpython-0.5.9/marketorestpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      512 2021-05-09 18:48:04.000000 marketorestpython-0.5.9/marketorestpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2021-05-09 18:48:04.000000 marketorestpython-0.5.9/marketorestpython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      400 2021-05-09 18:48:04.000000 marketorestpython-0.5.9/marketorestpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       18 2021-05-09 18:48:04.000000 marketorestpython-0.5.9/marketorestpython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      512 2021-05-09 18:48:05.000000 marketorestpython-0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0      121 2018-03-30 21:48:54.000000 marketorestpython-0.5.9/README
+-rw-rw-rw-   0        0        0       86 2021-05-09 18:48:05.000000 marketorestpython-0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     1180 2021-05-09 18:45:16.000000 marketorestpython-0.5.9/setup.py
```

### Comparing `marketorestpython-0.5.8/marketorestpython/client.py` & `marketorestpython-0.5.9/marketorestpython/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,14 +231,21 @@
                     'approve_program': self.approve_program,
                     'unapprove_program': self.unapprove_program,
                     'get_smart_list_by_program_id': self.get_smart_list_by_program_id,
                     'get_channels': self.get_channels,
                     'get_channel_by_name': self.get_channel_by_name,
                     'get_tags': self.get_tags,
                     'get_tag_by_name': self.get_tag_by_name,
+                    'create_update_custom_object_type': self.create_update_custom_object_type,
+                    'delete_custom_object_type': self.delete_custom_object_type,
+                    'approve_custom_object_type': self.approve_custom_object_type,                    
+                    'discard_custom_object_type': self.discard_custom_object_type,
+                    'get_list_of_custom_object_types': self.get_list_of_custom_object_types,
+                    'describe_custom_object_type': self.describe_custom_object_type,
+                    'add_field_custom_object_type': self.add_field_custom_object_type,
                     'get_list_of_custom_objects': self.get_list_of_custom_objects,
                     'describe_custom_object': self.describe_custom_object,
                     'create_update_custom_objects': self.create_update_custom_objects,
                     'delete_custom_objects': self.delete_custom_objects,
                     'get_custom_objects': self.get_custom_objects,
                     'describe_opportunity': self.describe_opportunity,
                     'create_update_opportunities': self.create_update_opportunities,
@@ -4462,14 +4469,108 @@
         }
         result = self._api_call(
             'get', self.host + "/rest/asset/v1/tagType/byName.json", args)
         if result is None:
             raise Exception("Empty Response")
         return result['result']
 
+    # --------- CUSTOM OBJECT TYPES ---------
+
+    def create_update_custom_object_type(self, apiName, action='createOrUpdate', displayName, pluralName=None,
+            description=None, showInLeadDetail=None):
+        self.authenticate()      
+        args = {
+            'access_token': self.token
+        }
+        data = {
+            'action': action,
+            'apiName': apiName,
+            'displayName': displayName
+        }
+        if pluralName is not None:
+            data['pluralName'] = pluralName
+        if description is not None:
+            data['description'] = description
+        if showInLeadDetail is not None:
+            data['showInLeadDetail'] = showInLeadDetail
+        result = self._api_call(
+            'post', self.host + "/rest/v1/customobjects/schema.json", args, data)
+        if result is None:
+            raise Exception("Empty Response")
+        return result['result']
+
+    def delete_custom_object_type(self, apiName):
+        self.authenticate()
+        args = {
+            'access_token': self.token
+        }
+        result = self._api_call(
+            'post', self.host + "/rest/v1/customobjects/schema/"+ str(apiName) +"/delete.json", args)
+        if result is None:
+            raise Exception("Empty Response")
+        return result['result']
+
+    def approve_custom_object_type(self, apiName):
+        self.authenticate()      
+        args = {
+            'access_token': self.token
+        }
+        result = self._api_call(
+            'post', self.host + "/rest/v1/customobjects/schema/"+ str(apiName) +"/approve.json", args)
+        if result is None:
+            raise Exception("Empty Response")
+        return result['result']
+
+    def discard_custom_object_type(self, apiName):
+        self.authenticate()
+        args = {
+            'access_token': self.token
+        }
+        result = self._api_call(
+            'post', self.host + "/rest/v1/customobjects/schema/"+ str(apiName) +"/discardDraft.json", args)
+        if result is None:
+            raise Exception("Empty Response")
+        return result['result']
+
+    def add_field_custom_object_type(self, apiName, fields):
+        self.authenticate()
+        args = {
+            'access_token': self.token
+        }
+        data = {
+            'input': fields
+        }
+        result = self._api_call(
+            'post', self.host + "/rest/v1/customobjects/schema/" + str(apiName) + "/addField.json", args, data)
+        if result is None:
+            raise Exception("Empty Response")
+        return result['result']
+
+    def get_list_of_custom_object_types(self):
+        self.authenticate()
+        args = {
+            'access_token': self.token
+        }
+        result = self._api_call(
+            'get', self.host + "/rest/v1/customobjects/schema.json", args)
+        if result is None:
+            raise Exception("Empty Response")
+        return result['result']
+
+    def describe_custom_object_type(self, apiName):
+        self.authenticate()
+        args = {
+            'access_token': self.token
+        }
+        result = self._api_call(
+            'get', self.host + "/rest/v1/customobjects/schema/" + str(apiName) + "/describe.json", args)
+        if result is None:
+            raise Exception("Empty Response")
+        return result['result']
+
     # --------- CUSTOM OBJECTS ---------
 
     def get_list_of_custom_objects(self, names=None):
         self.authenticate()
         args = {
             'access_token': self.token
         }
```

### Comparing `marketorestpython-0.5.8/marketorestpython/helper/http_lib.py` & `marketorestpython-0.5.9/marketorestpython/helper/http_lib.py`

 * *Files identical despite different names*

### Comparing `marketorestpython-0.5.8/marketorestpython.egg-info/PKG-INFO` & `marketorestpython-0.5.9/marketorestpython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: marketorestpython
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python Client for the Marketo REST API
 Home-page: https://github.com/jepcastelein/marketo-rest-python
 Author: Jep Castelein
 Author-email: jep@castelein.net
 License: MIT License
 Description: 
         Marketo Python REST is a Python client that wraps the Marketo Rest API.
```

### Comparing `marketorestpython-0.5.8/PKG-INFO` & `marketorestpython-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: marketorestpython
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python Client for the Marketo REST API
 Home-page: https://github.com/jepcastelein/marketo-rest-python
 Author: Jep Castelein
 Author-email: jep@castelein.net
 License: MIT License
 Description: 
         Marketo Python REST is a Python client that wraps the Marketo Rest API.
```

### Comparing `marketorestpython-0.5.8/setup.py` & `marketorestpython-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 long_description = '''
 Marketo Python REST is a Python client that wraps the Marketo Rest API.
 Originally developed by asamat with contributions from sandipsinha and osamakhn
 '''
 
 setup(
     name='marketorestpython',
-    version= '0.5.8',
+    version= '0.5.9',
     url='https://github.com/jepcastelein/marketo-rest-python',
     author='Jep Castelein',
     author_email='jep@castelein.net',
     packages=['marketorestpython', 'marketorestpython.helper'],
     license='MIT License',
     install_requires=[
         'backoff',
```

