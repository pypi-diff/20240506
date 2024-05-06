# Comparing `tmp/pyany2json-0.1.2.tar.gz` & `tmp/pyany2json-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyany2json-0.1.2.tar", max compression
+gzip compressed data, was "pyany2json-0.1.3.tar", max compression
```

## Comparing `pyany2json-0.1.2.tar` & `pyany2json-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2024-04-07 14:39:29.855166 pyany2json-0.1.2/LICENSE
--rw-r--r--   0        0        0     2829 2024-04-30 09:13:55.496675 pyany2json-0.1.2/README.md
--rw-r--r--   0        0        0   101192 2024-04-25 08:52:53.877970 pyany2json-0.1.2/libs/xelem-3.1.jar
--rw-r--r--   0        0        0      107 2024-04-06 04:06:45.433805 pyany2json-0.1.2/pyany2json/__init__.py
--rw-r--r--   0        0        0     2878 2024-04-30 07:32:28.086864 pyany2json-0.1.2/pyany2json/document_factory.py
--rw-r--r--   0        0        0      312 2024-04-07 09:29:48.489269 pyany2json-0.1.2/pyany2json/layex_table_parser.py
--rw-r--r--   0        0        0     1085 2024-04-07 09:16:49.923104 pyany2json-0.1.2/pyany2json/model.py
--rw-r--r--   0        0        0     1590 2024-05-01 07:34:58.231191 pyany2json-0.1.2/pyany2json/setup.py
--rw-r--r--   0        0        0      658 2024-04-07 09:19:08.905143 pyany2json-0.1.2/pyany2json/types.py
--rw-r--r--   0        0        0      427 2024-05-01 07:49:25.954228 pyany2json-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 pyany2json-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-07 14:39:29.855166 pyany2json-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2829 2024-04-30 09:13:55.496675 pyany2json-0.1.3/README.md
+-rw-r--r--   0        0        0   101192 2024-04-25 08:52:53.877970 pyany2json-0.1.3/libs/xelem-3.1.jar
+-rw-r--r--   0        0        0      934 2024-05-06 07:49:29.871385 pyany2json-0.1.3/pyany2json/__init__.py
+-rw-r--r--   0        0        0     2878 2024-04-30 07:32:28.086864 pyany2json-0.1.3/pyany2json/document_factory.py
+-rw-r--r--   0        0        0      312 2024-04-07 09:29:48.489269 pyany2json-0.1.3/pyany2json/layex_table_parser.py
+-rw-r--r--   0        0        0     1263 2024-05-06 07:39:18.566710 pyany2json-0.1.3/pyany2json/model.py
+-rw-r--r--   0        0        0     1590 2024-05-01 07:34:58.231191 pyany2json-0.1.3/pyany2json/setup.py
+-rw-r--r--   0        0        0      902 2024-05-06 07:44:26.814007 pyany2json-0.1.3/pyany2json/types.py
+-rw-r--r--   0        0        0      427 2024-05-06 08:04:32.210245 pyany2json-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 pyany2json-0.1.3/PKG-INFO
```

### Comparing `pyany2json-0.1.2/LICENSE` & `pyany2json-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyany2json-0.1.2/README.md` & `pyany2json-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyany2json-0.1.2/libs/xelem-3.1.jar` & `pyany2json-0.1.3/libs/xelem-3.1.jar`

 * *Files identical despite different names*

### Comparing `pyany2json-0.1.2/pyany2json/document_factory.py` & `pyany2json-0.1.3/pyany2json/document_factory.py`

 * *Files identical despite different names*

### Comparing `pyany2json-0.1.2/pyany2json/model.py` & `pyany2json-0.1.3/pyany2json/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     """createInstance"""
 
 
 class ModelBuilder:
     def __init__(self):
         """createInstance"""
         
+    def fromPath(self, path: str) -> ModelBuilder:
+        """Toto"""
+        
     def fromURI(self, uri: str) -> ModelBuilder:
         """Toto"""
         
     def fromJSON(self, data: str) -> ModelBuilder:
         """Toto"""
 
     def getEntityList(self) -> list:
@@ -40,13 +43,16 @@
         """Toto"""
         
     def setPatternMap(self, patterns: dict) -> ModelBuilder:
         """Toto"""
 
     def setTableParser(self, parser: TableParser) -> ModelBuilder:
         """Toto"""
+        
+    def setTagClassifier(self, tagger: TagClassifier) -> ModelBuilder:
+        """Toto"""
 
     def build(self) -> Model:
         """Toto"""
 
 
 ModelBuilder = ModelBuilder_
```

### Comparing `pyany2json-0.1.2/pyany2json/setup.py` & `pyany2json-0.1.3/pyany2json/setup.py`

 * *Files identical despite different names*

### Comparing `pyany2json-0.1.2/pyany2json/types.py` & `pyany2json-0.1.3/pyany2json/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 import jpype
 import jpype.imports
 
+from java.nio.file import Path as Path_  # type: ignore
+from java.nio.file import Paths as Paths_  # type: ignore 
 from java.util import List as List_  # type: ignore
 from java.util import EnumSet as EnumSet_  # type: ignore
 from com.github.romualdrousseau.shuju.json import JSON as JSON_  # type: ignore
 
 
+@jpype._jcustomizer.JConversion("java.nio.file.Path", instanceof=str)
+def _JPathConvert(jcls, obj):
+    return Paths_.get(obj)
+
+
 @jpype._jcustomizer.JConversion("java.util.List", instanceof=list)
 def _JListConvert(jcls, obj):
     return List_.of(obj)
 
 
 @jpype._jcustomizer.JConversion(
     "com.github.romualdrousseau.shuju.json.JSONObject", instanceof=str
```

### Comparing `pyany2json-0.1.2/PKG-INFO` & `pyany2json-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyany2json
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python binding to Any2Json
 Author: Romuald Rousseau
 Author-email: romuald.rousseau@servier.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

