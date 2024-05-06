# Comparing `tmp/ComplexJSON-1.1.0.tar.gz` & `tmp/ComplexJSON-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ComplexJSON-1.1.0.tar", last modified: Sat May  4 19:27:06 2024, max compression
+gzip compressed data, was "ComplexJSON-1.2.0.tar", last modified: Mon May  6 12:52:05 2024, max compression
```

## Comparing `ComplexJSON-1.1.0.tar` & `ComplexJSON-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 19:27:06.029583 ComplexJSON-1.1.0/
-drwxrwxrwx   0        0        0        0 2024-05-04 19:27:06.007908 ComplexJSON-1.1.0/ComplexJSON/
--rw-rw-rw-   0        0        0      173 2024-05-04 18:11:06.000000 ComplexJSON-1.1.0/ComplexJSON/__init__.py
--rw-rw-rw-   0        0        0     2166 2024-05-04 19:22:02.000000 ComplexJSON-1.1.0/ComplexJSON/complexJSONDecoder.py
--rw-rw-rw-   0        0        0      924 2024-05-04 19:22:02.000000 ComplexJSON-1.1.0/ComplexJSON/complexJSONEncoder.py
--rw-rw-rw-   0        0        0     3197 2024-05-04 19:24:51.000000 ComplexJSON-1.1.0/ComplexJSON/funcdef.py
--rw-rw-rw-   0        0        0       52 2024-05-01 20:24:25.000000 ComplexJSON-1.1.0/ComplexJSON/vardef.py
-drwxrwxrwx   0        0        0        0 2024-05-04 19:27:06.027582 ComplexJSON-1.1.0/ComplexJSON.egg-info/
--rw-rw-rw-   0        0        0     3950 2024-05-04 19:27:05.000000 ComplexJSON-1.1.0/ComplexJSON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2024-05-04 19:27:05.000000 ComplexJSON-1.1.0/ComplexJSON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 19:27:05.000000 ComplexJSON-1.1.0/ComplexJSON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-04 19:27:05.000000 ComplexJSON-1.1.0/ComplexJSON.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1063 2024-05-01 21:30:00.000000 ComplexJSON-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     3950 2024-05-04 19:27:06.029583 ComplexJSON-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3451 2024-05-04 19:22:02.000000 ComplexJSON-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 19:27:06.031606 ComplexJSON-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      728 2024-05-04 19:22:02.000000 ComplexJSON-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:52:05.653589 ComplexJSON-1.2.0/
+drwxrwxrwx   0        0        0        0 2024-05-06 12:52:05.631549 ComplexJSON-1.2.0/ComplexJSON/
+-rw-rw-rw-   0        0        0      173 2024-05-04 18:11:06.000000 ComplexJSON-1.2.0/ComplexJSON/__init__.py
+-rw-rw-rw-   0        0        0     3690 2024-05-06 12:38:59.000000 ComplexJSON-1.2.0/ComplexJSON/complexJSONDecoder.py
+-rw-rw-rw-   0        0        0     4326 2024-05-06 12:38:59.000000 ComplexJSON-1.2.0/ComplexJSON/complexJSONEncoder.py
+-rw-rw-rw-   0        0        0     4050 2024-05-06 12:39:27.000000 ComplexJSON-1.2.0/ComplexJSON/funcdef.py
+-rw-rw-rw-   0        0        0       77 2024-05-05 20:04:28.000000 ComplexJSON-1.2.0/ComplexJSON/vardef.py
+drwxrwxrwx   0        0        0        0 2024-05-06 12:52:05.652588 ComplexJSON-1.2.0/ComplexJSON.egg-info/
+-rw-rw-rw-   0        0        0     4430 2024-05-06 12:52:05.000000 ComplexJSON-1.2.0/ComplexJSON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-05-06 12:52:05.000000 ComplexJSON-1.2.0/ComplexJSON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 12:52:05.000000 ComplexJSON-1.2.0/ComplexJSON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-06 12:52:05.000000 ComplexJSON-1.2.0/ComplexJSON.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1063 2024-05-01 21:30:00.000000 ComplexJSON-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4430 2024-05-06 12:52:05.654589 ComplexJSON-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3931 2024-05-06 12:47:53.000000 ComplexJSON-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 12:52:05.656096 ComplexJSON-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      728 2024-05-06 12:47:53.000000 ComplexJSON-1.2.0/setup.py
```

### Comparing `ComplexJSON-1.1.0/ComplexJSON/funcdef.py` & `ComplexJSON-1.2.0/ComplexJSON/funcdef.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,50 +2,60 @@
 from . import ComplexJSONEncoder, ComplexJSONDecoder
 from json import dumps as __dumps, loads as __loads, dump as __dump, load as __load
 
 
 def dumps(obj, *args, skipkeys=False, ensure_ascii=True, check_circular=True,
           allow_nan=True, cls=ComplexJSONEncoder, indent=None, separators=None,
           default=None, sort_keys=False, localClassWord: str = None,
-          localModuleWord: str = None, **kwargs):
-    if localClassWord or localModuleWord:
-        encoder = ComplexJSONEncoder(localModuleWord=localModuleWord, localClassWord=localClassWord)
-        default = encoder.default
+          localModuleWord: str = None, localClassIdWord: str = None, useTypeAssociation: bool = False,
+          classStorage: Dict[str, Type] | List[Type] | None = None, **kwargs):
+    if localClassWord or localModuleWord or localClassIdWord or useTypeAssociation or classStorage:
+        cls = ComplexJSONEncoder
+        default = None
+        kwargs.update(dict(localModuleWord=localModuleWord, localClassWord=localClassWord,
+                           localClassIdWord=localClassIdWord, classStorage=classStorage,
+                           useTypeAssociation=useTypeAssociation))
     return __dumps(obj, *args, skipkeys=skipkeys, ensure_ascii=ensure_ascii, check_circular=check_circular,
                    allow_nan=allow_nan, cls=cls, indent=indent, separators=separators,
                    default=default, sort_keys=sort_keys, **kwargs)
 
 
 def loads(s, *args, cls=ComplexJSONDecoder, object_hook=None, parse_float=None,
           parse_int=None, parse_constant=None, object_pairs_hook=None,
           classStorage: Dict[str, Type] | List[Type] | None = None, localClassWord: str = None,
-          localModuleWord: str = None, **kwargs):
+          localModuleWord: str = None, localClassIdWord: str = None, **kwargs):
     if classStorage or localClassWord or localModuleWord:
-        decoder = ComplexJSONDecoder(classStorage=classStorage, localClassWord=localClassWord,
-                                     localModuleWord=localModuleWord)
-        object_hook = decoder.object_hook
+        cls = ComplexJSONDecoder
+        object_hook = None
+        kwargs.update(dict(classStorage=classStorage, localClassWord=localClassWord,
+                           localModuleWord=localModuleWord, localClassIdWord=localClassIdWord))
     return __loads(s, *args, cls=cls, object_hook=object_hook, parse_float=parse_float,
                    parse_int=parse_int, parse_constant=parse_constant, object_pairs_hook=object_pairs_hook, **kwargs)
 
 
 def dump(obj, fp, *args, skipkeys=False, ensure_ascii=True, check_circular=True,
          allow_nan=True, cls=ComplexJSONEncoder, indent=None, separators=None,
          default=None, sort_keys=False, localClassWord: str = None,
-         localModuleWord: str = None, **kwargs):
-    if localClassWord or localModuleWord:
-        encoder = ComplexJSONEncoder(localModuleWord=localModuleWord, localClassWord=localClassWord)
-        default = encoder.default
+         localModuleWord: str = None, localClassIdWord: str = None, useTypeAssociation: bool = False,
+         classStorage: Dict[str, Type] | List[Type] | None = None, **kwargs):
+    if localClassWord or localModuleWord or localClassIdWord or useTypeAssociation or classStorage:
+        cls = ComplexJSONEncoder
+        default = None
+        kwargs.update(dict(localModuleWord=localModuleWord, localClassWord=localClassWord,
+                           localClassIdWord=localClassIdWord, classStorage=classStorage,
+                           useTypeAssociation=useTypeAssociation))
     return __dump(obj, fp, *args, skipkeys=skipkeys, ensure_ascii=ensure_ascii, check_circular=check_circular,
                   allow_nan=allow_nan, cls=cls, indent=indent, separators=separators,
                   default=default, sort_keys=sort_keys, **kwargs)
 
 
 def load(fp, *args, cls=ComplexJSONDecoder, object_hook=None, parse_float=None,
          parse_int=None, parse_constant=None, object_pairs_hook=None,
          classStorage: Dict[str, Type] | List[Type] | None = None, localClassWord: str = None,
-         localModuleWord: str = None, **kwargs):
+         localModuleWord: str = None, localClassIdWord: str = None, **kwargs):
     if classStorage or localClassWord or localModuleWord:
-        decoder = ComplexJSONDecoder(classStorage=classStorage, localClassWord=localClassWord,
-                                     localModuleWord=localModuleWord)
-        object_hook = decoder.object_hook
+        cls = ComplexJSONDecoder
+        object_hook = None
+        kwargs.update(dict(classStorage=classStorage, localClassWord=localClassWord,
+                           localModuleWord=localModuleWord, localClassIdWord=localClassIdWord))
     return __load(fp, *args, cls=cls, object_hook=object_hook, parse_float=parse_float,
                   parse_int=parse_int, parse_constant=parse_constant, object_pairs_hook=object_pairs_hook, **kwargs)
```

### Comparing `ComplexJSON-1.1.0/ComplexJSON.egg-info/PKG-INFO` & `ComplexJSON-1.2.0/ComplexJSON.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ComplexJSON
-Version: 1.1.0
+Version: 1.2.0
 Summary: This is the simplest module for serialize and deserialize python complex objects
 Home-page: https://github.com/dail45/ComplexJSON
 Author: dail45
 Keywords: json complexobject serialize
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -172,8 +172,28 @@
 ```python
 import ComplexJSON as json
 ...
 _json = json.dumps(obj, localClassWord="Type", localModuleWord="Module")
 new_obj = json.loads(_json, localClassWord="Type", localModuleWord="Module")
 ```
 
+#### Type Association (v1.2+) ####
+
+```python
+import ComplexJSON
+
+
+class A:
+    def __init__(self):
+        self.a = 1
+        self.b = 2
+
+
+rs = {1: A()}
+json_obj = ComplexJSON.dumps(rs, useTypeAssociation=True)
+print(json_obj)
+#>>> {"types": {".": {"useTA": true}, "0": {"__module__": "__main__", "__class__": "A"}}, "obj": {"1": {"a": 1, "b": 2, "__cid__": "0"}}}
+print(ComplexJSON.loads(json_obj))
+#>>> {'1': <__main__.A object at 0x00000154D6013490>}
+```
+
 ----------
```

### Comparing `ComplexJSON-1.1.0/LICENSE` & `ComplexJSON-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ComplexJSON-1.1.0/PKG-INFO` & `ComplexJSON-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ComplexJSON
-Version: 1.1.0
+Version: 1.2.0
 Summary: This is the simplest module for serialize and deserialize python complex objects
 Home-page: https://github.com/dail45/ComplexJSON
 Author: dail45
 Keywords: json complexobject serialize
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -172,8 +172,28 @@
 ```python
 import ComplexJSON as json
 ...
 _json = json.dumps(obj, localClassWord="Type", localModuleWord="Module")
 new_obj = json.loads(_json, localClassWord="Type", localModuleWord="Module")
 ```
 
+#### Type Association (v1.2+) ####
+
+```python
+import ComplexJSON
+
+
+class A:
+    def __init__(self):
+        self.a = 1
+        self.b = 2
+
+
+rs = {1: A()}
+json_obj = ComplexJSON.dumps(rs, useTypeAssociation=True)
+print(json_obj)
+#>>> {"types": {".": {"useTA": true}, "0": {"__module__": "__main__", "__class__": "A"}}, "obj": {"1": {"a": 1, "b": 2, "__cid__": "0"}}}
+print(ComplexJSON.loads(json_obj))
+#>>> {'1': <__main__.A object at 0x00000154D6013490>}
+```
+
 ----------
```

### Comparing `ComplexJSON-1.1.0/README.md` & `ComplexJSON-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -158,8 +158,28 @@
 ```python
 import ComplexJSON as json
 ...
 _json = json.dumps(obj, localClassWord="Type", localModuleWord="Module")
 new_obj = json.loads(_json, localClassWord="Type", localModuleWord="Module")
 ```
 
+#### Type Association (v1.2+) ####
+
+```python
+import ComplexJSON
+
+
+class A:
+    def __init__(self):
+        self.a = 1
+        self.b = 2
+
+
+rs = {1: A()}
+json_obj = ComplexJSON.dumps(rs, useTypeAssociation=True)
+print(json_obj)
+#>>> {"types": {".": {"useTA": true}, "0": {"__module__": "__main__", "__class__": "A"}}, "obj": {"1": {"a": 1, "b": 2, "__cid__": "0"}}}
+print(ComplexJSON.loads(json_obj))
+#>>> {'1': <__main__.A object at 0x00000154D6013490>}
+```
+
 ----------
```

### Comparing `ComplexJSON-1.1.0/setup.py` & `ComplexJSON-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='ComplexJSON',
-    version='1.1.0',
+    version='1.2.0',
     author='dail45',
     description='This is the simplest module for serialize and deserialize python complex objects',
     long_description=readme(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     url="https://github.com/dail45/ComplexJSON",
     classifiers=[
```

