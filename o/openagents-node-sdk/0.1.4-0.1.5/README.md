# Comparing `tmp/openagents_node_sdk-0.1.4.tar.gz` & `tmp/openagents_node_sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openagents_node_sdk-0.1.4.tar", last modified: Sat May  4 12:24:22 2024, max compression
+gzip compressed data, was "openagents_node_sdk-0.1.5.tar", last modified: Mon May  6 15:52:11 2024, max compression
```

## Comparing `openagents_node_sdk-0.1.4.tar` & `openagents_node_sdk-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:24:22.133051 openagents_node_sdk-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-04 12:24:17.000000 openagents_node_sdk-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 12:24:17.000000 openagents_node_sdk-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-04 12:24:22.133051 openagents_node_sdk-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-04 12:24:17.000000 openagents_node_sdk-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 12:24:17.000000 openagents_node_sdk-0.1.4/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:24:22.133051 openagents_node_sdk-0.1.4/openagents/
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-04 12:24:17.000000 openagents_node_sdk-0.1.4/openagents/Disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-04 12:24:17.000000 openagents_node_sdk-0.1.4/openagents/DiskReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-04 12:24:17.000000 openagents_node_sdk-0.1.4/openagents/DiskWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8845 2024-05-04 12:24:17.000000 openagents_node_sdk-0.1.4/openagents/JobRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-04 12:24:17.000000 openagents_node_sdk-0.1.4/openagents/Logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-04 12:24:17.000000 openagents_node_sdk-0.1.4/openagents/NodeConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-05-04 12:24:17.000000 openagents_node_sdk-0.1.4/openagents/OpenAgentsNode.py
--rw-r--r--   0 runner    (1001) docker     (127)    16104 2024-05-04 12:24:17.000000 openagents_node_sdk-0.1.4/openagents/RunnerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-04 12:24:17.000000 openagents_node_sdk-0.1.4/openagents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 12:24:22.133051 openagents_node_sdk-0.1.4/openagents_node_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-04 12:24:22.000000 openagents_node_sdk-0.1.4/openagents_node_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-04 12:24:22.000000 openagents_node_sdk-0.1.4/openagents_node_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 12:24:22.000000 openagents_node_sdk-0.1.4/openagents_node_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-04 12:24:22.000000 openagents_node_sdk-0.1.4/openagents_node_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-04 12:24:22.000000 openagents_node_sdk-0.1.4/openagents_node_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 12:24:22.133051 openagents_node_sdk-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-04 12:24:17.000000 openagents_node_sdk-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:52:11.541254 openagents_node_sdk-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-06 15:52:11.541254 openagents_node_sdk-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:52:11.541254 openagents_node_sdk-0.1.5/openagents/
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/Disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/DiskReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/DiskWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8845 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/JobRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/NodeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/OpenAgentsNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16537 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/RunnerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/openagents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:52:11.541254 openagents_node_sdk-0.1.5/openagents_node_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-06 15:52:11.000000 openagents_node_sdk-0.1.5/openagents_node_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-06 15:52:11.000000 openagents_node_sdk-0.1.5/openagents_node_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:52:11.000000 openagents_node_sdk-0.1.5/openagents_node_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-06 15:52:11.000000 openagents_node_sdk-0.1.5/openagents_node_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 15:52:11.000000 openagents_node_sdk-0.1.5/openagents_node_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:52:11.541254 openagents_node_sdk-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-06 15:52:07.000000 openagents_node_sdk-0.1.5/setup.py
```

### Comparing `openagents_node_sdk-0.1.4/LICENSE` & `openagents_node_sdk-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.4/openagents/Disk.py` & `openagents_node_sdk-0.1.5/openagents/Disk.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.4/openagents/DiskReader.py` & `openagents_node_sdk-0.1.5/openagents/DiskReader.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.4/openagents/DiskWriter.py` & `openagents_node_sdk-0.1.5/openagents/DiskWriter.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.4/openagents/JobRunner.py` & `openagents_node_sdk-0.1.5/openagents/JobRunner.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.4/openagents/Logger.py` & `openagents_node_sdk-0.1.5/openagents/Logger.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.4/openagents/NodeConfig.py` & `openagents_node_sdk-0.1.5/openagents/NodeConfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,24 @@
     """
     The configuration of an OpenAgents Node.
     Can be configured also with environment variables:
     - NODE_NAME: The name of the node.
     - NODE_DESCRIPTION: The description of the node.
     - NODE_VERSION: The version of the node.
     """
-    def __init__(self):
+    def __init__(self, meta:dict=None):
         self._meta={
             "name": "OpenAgents Node",
             "description": "An new OpenAgents Node",
             "about": "An new OpenAgents Node",
             "version": "0.0.1",
         }
+        if meta:
+            for k,v in meta.items():
+                self._meta[k]=v
 
     def getMeta(self):
         self._meta["name"] = os.getenv('NODE_NAME', self._meta["name"])
         self._meta["description"] = os.getenv('NODE_DESCRIPTION', self._meta["description"])
         self._meta["about"] = os.getenv('NODE_DESCRIPTION', self._meta["about"])
         self._meta["description"] = os.getenv('NODE_DESCRIPTION', self._meta["description"])
         self._meta["version"] = os.getenv('NODE_VERSION', self._meta["version"])
```

### Comparing `openagents_node_sdk-0.1.4/openagents/OpenAgentsNode.py` & `openagents_node_sdk-0.1.5/openagents/OpenAgentsNode.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.1.4/openagents/RunnerConfig.py` & `openagents_node_sdk-0.1.5/openagents/RunnerConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,15 +359,15 @@
         """
         return self._econfig
 
 class RunnerConfig:
     """
     A class to build an event (meta, template, socket schema, filters).
     """
-    def __init__(self):
+    def __init__(self, meta:dict=None, filters:list[dict]=None, template:str=None, sockets:dict=None):
         self._meta={
             "kind": 5003,
             "name": "An event template",
             "about": "",
             "description": "",
             "tos": "",
             "privacy": "",
@@ -376,14 +376,31 @@
             "picture": "",
             "tags": []
         }
         self._filters=[]
         self._template=""
         self._sockets={}
 
+        if template:
+            self._template=template
+
+        if meta:
+            for k,v in meta.items():
+                self._meta[k]=v
+        
+        if sockets:
+            for k,v in sockets.items():
+                self._sockets[k]=v
+
+        if filters:    
+            for f in filters:
+                self._filters.append(f)
+        
+
+
     def getMeta(self) -> dict:
         """
         Get the meta data of the event.
         Returns:
             dict: The meta data of the event.
         """
         return self._meta
```

### Comparing `openagents_node_sdk-0.1.4/setup.py` & `openagents_node_sdk-0.1.5/setup.py`

 * *Files identical despite different names*

