# Comparing `tmp/htagui-0.5.8.tar.gz` & `tmp/htagui-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagui-0.5.8.tar", max compression
+gzip compressed data, was "htagui-0.5.9.tar", max compression
```

## Comparing `htagui-0.5.8.tar` & `htagui-0.5.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1065 2024-05-02 07:49:39.894433 htagui-0.5.8/LICENSE
--rw-r--r--   0        0        0     8906 2024-05-02 07:49:39.894433 htagui-0.5.8/README.md
--rw-r--r--   0        0        0      330 2024-05-02 07:49:40.154432 htagui-0.5.8/htagui/__init__.py
--rw-r--r--   0        0        0      892 2024-05-02 07:49:39.894433 htagui-0.5.8/htagui/all.py
--rw-r--r--   0        0        0      750 2024-05-02 07:49:39.894433 htagui-0.5.8/htagui/basics/__init__.py
--rw-r--r--   0        0        0    11404 2024-05-02 07:49:39.894433 htagui-0.5.8/htagui/basics/bases.py
--rw-r--r--   0        0        0      771 2024-05-02 07:49:39.894433 htagui-0.5.8/htagui/bulma/__init__.py
--rw-r--r--   0        0        0   656501 2024-05-02 07:49:39.898433 htagui-0.5.8/htagui/bulma/bases.py
--rw-r--r--   0        0        0     4268 2024-05-02 07:49:39.898433 htagui-0.5.8/htagui/common.py
--rw-r--r--   0        0        0     3988 2024-05-02 07:49:39.898433 htagui-0.5.8/htagui/dialog.py
--rw-r--r--   0        0        0      648 2024-05-02 07:49:39.898433 htagui-0.5.8/htagui/fileupload.py
--rw-r--r--   0        0        0     1856 2024-05-02 07:49:39.898433 htagui-0.5.8/htagui/flex.py
--rw-r--r--   0        0        0      785 2024-05-02 07:49:39.898433 htagui-0.5.8/htagui/fluent/__init__.py
--rw-r--r--   0        0        0     8538 2024-05-02 07:49:39.898433 htagui-0.5.8/htagui/fluent/bases.py
--rw-r--r--   0        0        0      771 2024-05-02 07:49:39.898433 htagui-0.5.8/htagui/form.py
--rw-r--r--   0        0        0     3795 2024-05-02 07:49:39.898433 htagui-0.5.8/htagui/ifields.py
--rw-r--r--   0        0        0      922 2024-05-02 07:49:39.898433 htagui-0.5.8/htagui/md/__init__.py
--rw-r--r--   0        0        0    10945 2024-05-02 07:49:39.898433 htagui-0.5.8/htagui/md/bases.py
--rw-r--r--   0        0        0      774 2024-05-02 07:49:39.898433 htagui-0.5.8/htagui/shoelace/__init__.py
--rw-r--r--   0        0        0     8489 2024-05-02 07:49:39.898433 htagui-0.5.8/htagui/shoelace/bases.py
--rw-r--r--   0        0        0     9619 2024-05-02 07:49:39.898433 htagui-0.5.8/htagui/splitters.py
--rw-r--r--   0        0        0     1441 2024-05-02 07:49:39.898433 htagui-0.5.8/htagui/tabs.py
--rw-r--r--   0        0        0     1069 2024-05-02 07:49:40.154432 htagui-0.5.8/pyproject.toml
--rw-r--r--   0        0        0    10139 1970-01-01 00:00:00.000000 htagui-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-05 05:13:00.772400 htagui-0.5.9/LICENSE
+-rw-r--r--   0        0        0     8906 2024-05-05 05:13:00.772400 htagui-0.5.9/README.md
+-rw-r--r--   0        0        0      330 2024-05-05 05:13:01.028400 htagui-0.5.9/htagui/__init__.py
+-rw-r--r--   0        0        0      892 2024-05-05 05:13:00.772400 htagui-0.5.9/htagui/all.py
+-rw-r--r--   0        0        0      750 2024-05-05 05:13:00.772400 htagui-0.5.9/htagui/basics/__init__.py
+-rw-r--r--   0        0        0    11518 2024-05-05 05:13:00.772400 htagui-0.5.9/htagui/basics/bases.py
+-rw-r--r--   0        0        0      771 2024-05-05 05:13:00.772400 htagui-0.5.9/htagui/bulma/__init__.py
+-rw-r--r--   0        0        0   656501 2024-05-05 05:13:00.776400 htagui-0.5.9/htagui/bulma/bases.py
+-rw-r--r--   0        0        0     4268 2024-05-05 05:13:00.776400 htagui-0.5.9/htagui/common.py
+-rw-r--r--   0        0        0     3988 2024-05-05 05:13:00.776400 htagui-0.5.9/htagui/dialog.py
+-rw-r--r--   0        0        0      648 2024-05-05 05:13:00.776400 htagui-0.5.9/htagui/fileupload.py
+-rw-r--r--   0        0        0     1856 2024-05-05 05:13:00.776400 htagui-0.5.9/htagui/flex.py
+-rw-r--r--   0        0        0      785 2024-05-05 05:13:00.776400 htagui-0.5.9/htagui/fluent/__init__.py
+-rw-r--r--   0        0        0     8538 2024-05-05 05:13:00.776400 htagui-0.5.9/htagui/fluent/bases.py
+-rw-r--r--   0        0        0      771 2024-05-05 05:13:00.776400 htagui-0.5.9/htagui/form.py
+-rw-r--r--   0        0        0     3795 2024-05-05 05:13:00.776400 htagui-0.5.9/htagui/ifields.py
+-rw-r--r--   0        0        0      922 2024-05-05 05:13:00.776400 htagui-0.5.9/htagui/md/__init__.py
+-rw-r--r--   0        0        0    10945 2024-05-05 05:13:00.776400 htagui-0.5.9/htagui/md/bases.py
+-rw-r--r--   0        0        0      774 2024-05-05 05:13:00.776400 htagui-0.5.9/htagui/shoelace/__init__.py
+-rw-r--r--   0        0        0     8489 2024-05-05 05:13:00.776400 htagui-0.5.9/htagui/shoelace/bases.py
+-rw-r--r--   0        0        0     9619 2024-05-05 05:13:00.776400 htagui-0.5.9/htagui/splitters.py
+-rw-r--r--   0        0        0     1441 2024-05-05 05:13:00.776400 htagui-0.5.9/htagui/tabs.py
+-rw-r--r--   0        0        0     1069 2024-05-05 05:13:01.028400 htagui-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0    10139 1970-01-01 00:00:00.000000 htagui-0.5.9/PKG-INFO
```

### Comparing `htagui-0.5.8/LICENSE` & `htagui-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/README.md` & `htagui-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/all.py` & `htagui-0.5.9/htagui/all.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/basics/__init__.py` & `htagui-0.5.9/htagui/basics/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/basics/bases.py` & `htagui-0.5.9/htagui/basics/bases.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,64 +11,66 @@
 from ..form import Form
 from ..common import ensuredict,ListOrDict,autoclosemenu
 
 STATICS="""
 
 html,body {
     width:100%;
-    font-family: ubuntu;
+    font-family: ubuntu, 'Helvetica';
     padding:0px;
     margin:0px;
 }
 
 a {color: #0075ff;text-decoration:none}
 
 .button {
     border:1px solid #DDD;
     border-radius:6px;
     padding:10px;
     margin:1px;
     cursor:pointer;
-    font-family: ubuntu;
+    font-family: ubuntu, 'Helvetica';
 }
 
 .button:hover {
     filter: brightness(0.95);
 }
 
 .input[type="text"] {
-    font-family: ubuntu;
-    padding:4px;
+    font-family: ubuntu,'Helvetica';
+    font-size: 1em;
+    padding:6px;
     border-radius: 4px;
     border: 2px solid #EEE;
     width: calc(100% - 16px);
 }
 .input:focus {
     outline: none;
     border: 2px solid #0075ff !important;
 }
 
 
 .textarea {
-    font-family: ubuntu;
-    padding:4px;
+    font-family: ubuntu,'Helvetica';
+    font-size: 1em;
+    padding:6px;
     border-radius: 4px;
     border: 2px solid #EEE;
     width: calc(100% - 16px);
 }
 .textarea:focus {
     outline: none;
     border: 2px solid #0075ff !important;
 }
 
 .select {
     padding:4px;
     border-radius: 4px;
     border: 2px solid #EEE;
-    font-family: ubuntu;
+    font-family: ubuntu,'Helvetica';
 }
 
 .select:focus {
     border: 2px solid #0075ff !important;
 }
 
 .menu {}
@@ -84,15 +86,15 @@
 
 .tab {
     border:0px;
     cursor:pointer;
     margin:2px;
     background:white;
     padding:8px;
-    font-family: ubuntu;
+    font-family: ubuntu,'Helvetica';
 }
 .tab.selected {
     color:#0075ff;
     border-bottom: 1px solid #0075ff;
 }
```

### Comparing `htagui-0.5.8/htagui/bulma/__init__.py` & `htagui-0.5.9/htagui/bulma/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/bulma/bases.py` & `htagui-0.5.9/htagui/bulma/bases.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/common.py` & `htagui-0.5.9/htagui/common.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/dialog.py` & `htagui-0.5.9/htagui/dialog.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/fileupload.py` & `htagui-0.5.9/htagui/fileupload.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/flex.py` & `htagui-0.5.9/htagui/flex.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/fluent/__init__.py` & `htagui-0.5.9/htagui/fluent/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/fluent/bases.py` & `htagui-0.5.9/htagui/fluent/bases.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/form.py` & `htagui-0.5.9/htagui/form.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/ifields.py` & `htagui-0.5.9/htagui/ifields.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/md/__init__.py` & `htagui-0.5.9/htagui/md/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/md/bases.py` & `htagui-0.5.9/htagui/md/bases.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/shoelace/__init__.py` & `htagui-0.5.9/htagui/shoelace/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/shoelace/bases.py` & `htagui-0.5.9/htagui/shoelace/bases.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/splitters.py` & `htagui-0.5.9/htagui/splitters.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/htagui/tabs.py` & `htagui-0.5.9/htagui/tabs.py`

 * *Files identical despite different names*

### Comparing `htagui-0.5.8/pyproject.toml` & `htagui-0.5.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagui"
-version = "0.5.8" # auto-updated
+version = "0.5.9" # auto-updated
 description = "GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','gui', 'electron', "cef", "asyncio", "guy", "desktop", "web", "mobile", "http", "websocket", "html", "pyscript"]
 homepage = "https://github.com/manatlan/htagui"
 repository = "https://github.com/manatlan/htagui"
```

### Comparing `htagui-0.5.8/PKG-INFO` & `htagui-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagui
-Version: 0.5.8
+Version: 0.5.9
 Summary: GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase
 Home-page: https://github.com/manatlan/htagui
 License: MIT
 Keywords: htag,gui,electron,cef,asyncio,guy,desktop,web,mobile,http,websocket,html,pyscript
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.7,<4.0
```

