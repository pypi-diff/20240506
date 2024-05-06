# Comparing `tmp/rlsdk_python-0.4.0.tar.gz` & `tmp/rlsdk_python-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlsdk_python-0.4.0.tar", max compression
+gzip compressed data, was "rlsdk_python-0.4.1.tar", max compression
```

## Comparing `rlsdk_python-0.4.0.tar` & `rlsdk_python-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      357 2024-04-28 21:04:45.985727 rlsdk_python-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1640 2024-04-21 20:56:20.206780 rlsdk_python-0.4.0/README.md
--rw-r--r--   0        0        0      121 2024-04-28 17:35:36.468385 rlsdk_python-0.4.0/rlsdk_python/__init__.py
--rw-r--r--   0        0        0     1812 2024-04-18 23:00:20.787805 rlsdk_python-0.4.0/rlsdk_python/event_handling.py
--rw-r--r--   0        0        0     1814 2024-04-18 21:23:06.061748 rlsdk_python-0.4.0/rlsdk_python/events.py
--rw-r--r--   0        0        0     4065 2024-04-26 18:56:51.985326 rlsdk_python-0.4.0/rlsdk_python/frida_script.py
--rw-r--r--   0        0        0    30557 2024-04-26 15:34:23.035361 rlsdk_python-0.4.0/rlsdk_python/game_objects.py
--rw-r--r--   0        0        0    21863 2024-04-28 17:23:29.111823 rlsdk_python-0.4.0/rlsdk_python/sdk.py
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 rlsdk_python-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      357 2024-05-06 00:06:42.498308 rlsdk_python-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1640 2024-04-21 20:56:20.206780 rlsdk_python-0.4.1/README.md
+-rw-r--r--   0        0        0      121 2024-04-28 17:35:36.468385 rlsdk_python-0.4.1/rlsdk_python/__init__.py
+-rw-r--r--   0        0        0     1812 2024-04-18 23:00:20.787805 rlsdk_python-0.4.1/rlsdk_python/event_handling.py
+-rw-r--r--   0        0        0     1814 2024-04-18 21:23:06.061748 rlsdk_python-0.4.1/rlsdk_python/events.py
+-rw-r--r--   0        0        0     4065 2024-04-26 18:56:51.985326 rlsdk_python-0.4.1/rlsdk_python/frida_script.py
+-rw-r--r--   0        0        0    31126 2024-05-06 00:07:22.328055 rlsdk_python-0.4.1/rlsdk_python/game_objects.py
+-rw-r--r--   0        0        0    22610 2024-05-06 00:07:22.328055 rlsdk_python-0.4.1/rlsdk_python/sdk.py
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 rlsdk_python-0.4.1/PKG-INFO
```

### Comparing `rlsdk_python-0.4.0/README.md` & `rlsdk_python-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.4.0/rlsdk_python/event_handling.py` & `rlsdk_python-0.4.1/rlsdk_python/event_handling.py`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.4.0/rlsdk_python/events.py` & `rlsdk_python-0.4.1/rlsdk_python/events.py`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.4.0/rlsdk_python/frida_script.py` & `rlsdk_python-0.4.1/rlsdk_python/frida_script.py`

 * *Files identical despite different names*

### Comparing `rlsdk_python-0.4.0/rlsdk_python/game_objects.py` & `rlsdk_python-0.4.1/rlsdk_python/game_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import ctypes
 from typing import Tuple
 import time
 
 
 class Pointer:
-  def __init__(self, address, *, sdk=None):
-
+    def __repr__(self):
+        return f"<{self.__class__.__name__} at 0x{self.address:X}>"
+    
+    def __init__(self, address, *, sdk=None):
         if(address == None):
            raise ValueError("Address is None")
 
         self.address = address
         self.sdk = sdk
 
 class UObject(Pointer):
@@ -226,23 +228,37 @@
         return TArray(goals_tarray_address, Goal, sdk=self.sdk).get_items()
 
     def get_local_players(self):
         local_players_tarray_address = self.address + 0x0360
         return TArray(local_players_tarray_address, PlayerController, sdk=self.sdk).get_items()
 
 class TArray(Pointer):
-
     size = 0x10
 
     def __init__(self, address, class_type, sdk=None):
         super().__init__(address, sdk=sdk)
         self.class_type = class_type
 
-    def get_count(self):
+    def __len__(self):
         return self.sdk.pm.read_int(self.address + 0x8)
+        
+    def __iter__(self):
+        data_address = self.get_data_address()
+        for i in range(len(self)):
+            item_address = self.sdk.pm.read_ulonglong(data_address + i * 0x8)
+            yield self.class_type(item_address, sdk=self.sdk)
+            
+    def __contains__(self, item):
+        for x in self:
+            if x == item:
+                return True
+        return False
+
+    def get_count(self):
+        return self.__len__()
     
     def get_max(self):
         return self.sdk.pm.read_int(self.address + 0xC)
 
     def get_data_address(self):
         return self.sdk.pm.read_ulonglong(self.address)
     
@@ -256,14 +272,15 @@
         return items
     
     def get_item(self, index):
         data_address = self.get_data_address()
         item_address = self.sdk.pm.read_ulonglong(data_address + index * 0x8)
         return self.class_type(item_address, sdk=self.sdk)
 
+
 class FVector(Pointer):
     size = 0x0C
 
     def get_x(self):
         return self.sdk.pm.read_float(self.address)
     
     def get_y(self):
```

### Comparing `rlsdk_python-0.4.0/rlsdk_python/sdk.py` & `rlsdk_python-0.4.1/rlsdk_python/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,19 +104,28 @@
 
         self.static_classes = {}
         self.static_functions = {}
 
         self.scan_result = []
         self.scan_response_received_event = threading.Event()
 
-        
+
         try:
             self.load_gnames()
             self.map_objects()
+<<<<<<< HEAD
+            
+            if len(self.gnames) == 0 or len(self.static_classes) == 0 or len(self.static_functions) == 0:
+                raise Exception("GNames or mapping objects not found")
+
         except:
+=======
+        except Exception as e:
+            print(e)
+>>>>>>> 73a68b8087e8c6619bb5f63edb3518798878b70c
             print(Fore.RED + "Error while loading GNames and mapping objects. Trying to resolve offsets" + END)
            # If an error occurs, offset may be wrong, try to resolve them again
             try:
                 self.resolve_offsets()
                 self.load_gnames()
                 self.map_objects()
                 
@@ -276,41 +285,53 @@
     
     
         
     def load_gnames(self):
 
         print(Fore.YELLOW + "Loading GNames..." + END)
         gnames_entries_tarray = self.get_gnames_entries_tarray()
-        print(Fore.GREEN + "GNames count: " + Fore.BLUE + str(gnames_entries_tarray.get_count()) + END)
+        print(Fore.GREEN + "GNames count: " + Fore.BLUE + str(len(gnames_entries_tarray)) + END)
         
         
-        for gname_entry in tqdm(gnames_entries_tarray.get_items()):
+        for gname_entry in tqdm(gnames_entries_tarray):
 
             if not gname_entry.address:
                 continue
 
             self.gnames[gname_entry.get_index()] = gname_entry.get_name()
             
 
         print(Fore.GREEN + "GNames loaded" + END)
 
     def map_objects(self):
         print(Fore.YELLOW + "Mapping objects..." + END)
         gobjects_tarray = self.get_gobjects_tarray()
+<<<<<<< HEAD
         for gobject in tqdm(gobjects_tarray.get_items()):
+            try:
+                if not gobject.address:
+                    continue
+                # if full_name content "Class " then it's a UClass
+=======
+        print(Fore.GREEN + "GObjects count: " + Fore.BLUE + str(len(gobjects_tarray)) + END)
+        
+        for gobject in tqdm(gobjects_tarray):
             if not gobject.address:
                 continue
             # if full_name content "Class " then it's a UClass
+>>>>>>> 73a68b8087e8c6619bb5f63edb3518798878b70c
 
-            full_name = gobject.get_full_name() 
-            
-            if "Class " in full_name:
-                self.static_classes[full_name] = UClass(gobject.address, sdk=self)
-            elif "Function " in full_name:
-                self.static_functions[full_name] = UFunction(gobject.address, sdk=self)
+                full_name = gobject.get_full_name() 
+                
+                if "Class " in full_name:
+                    self.static_classes[full_name] = UClass(gobject.address, sdk=self)
+                elif "Function " in full_name:
+                    self.static_functions[full_name] = UFunction(gobject.address, sdk=self)
+            except:
+                continue
         
         
         print(Fore.GREEN + "UClasses: " + Fore.BLUE + str(len(self.static_classes)) + END)
         print(Fore.GREEN + "UFunctions: " + Fore.BLUE + str(len(self.static_functions)) + END)
     
     # ==========================================================
     # ================ INTERNAL EVENT HANDLING =================
```

### Comparing `rlsdk_python-0.4.0/PKG-INFO` & `rlsdk_python-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlsdk_python
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: MarlburroW
 Author-email: nik0o@hotmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

