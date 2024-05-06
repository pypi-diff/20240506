# Comparing `tmp/mikrotik-bt5-0.0.2b4.tar.gz` & `tmp/mikrotik-bt5-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikrotik-bt5-0.0.2b4.tar", last modified: Sat May  4 16:10:49 2024, max compression
+gzip compressed data, was "mikrotik-bt5-1.0.0.tar", last modified: Mon May  6 07:27:58 2024, max compression
```

## Comparing `mikrotik-bt5-0.0.2b4.tar` & `mikrotik-bt5-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-04 16:10:49.536380 mikrotik-bt5-0.0.2b4/
--rw-r--r--   0 pi        (1000) pi        (1000)      868 2024-05-04 16:10:49.532380 mikrotik-bt5-0.0.2b4/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      501 2024-05-03 08:43:20.000000 mikrotik-bt5-0.0.2b4/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-04 16:10:49.512380 mikrotik-bt5-0.0.2b4/mikrotik_bt5/
--rw-r--r--   0 pi        (1000) pi        (1000)       90 2024-05-04 05:52:43.000000 mikrotik-bt5-0.0.2b4/mikrotik_bt5/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3861 2024-05-04 16:10:04.000000 mikrotik-bt5-0.0.2b4/mikrotik_bt5/beacon.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1880 2024-05-04 05:49:06.000000 mikrotik-bt5-0.0.2b4/mikrotik_bt5/client.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-04 16:10:49.528380 mikrotik-bt5-0.0.2b4/mikrotik_bt5.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      868 2024-05-04 16:10:48.000000 mikrotik-bt5-0.0.2b4/mikrotik_bt5.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      315 2024-05-04 16:10:49.000000 mikrotik-bt5-0.0.2b4/mikrotik_bt5.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-05-04 16:10:48.000000 mikrotik-bt5-0.0.2b4/mikrotik_bt5.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        6 2024-05-04 16:10:48.000000 mikrotik-bt5-0.0.2b4/mikrotik_bt5.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       19 2024-05-04 16:10:48.000000 mikrotik-bt5-0.0.2b4/mikrotik_bt5.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2024-05-04 16:10:49.536380 mikrotik-bt5-0.0.2b4/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      639 2024-05-04 16:06:58.000000 mikrotik-bt5-0.0.2b4/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-04 16:10:49.532380 mikrotik-bt5-0.0.2b4/tests/
--rw-r--r--   0 pi        (1000) pi        (1000)       44 2024-05-04 15:30:02.000000 mikrotik-bt5-0.0.2b4/tests/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2767 2024-05-04 16:06:16.000000 mikrotik-bt5-0.0.2b4/tests/test_advertisements.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-06 07:27:58.537194 mikrotik-bt5-1.0.0/
+-rw-r--r--   0 pi        (1000) pi        (1000)      866 2024-05-06 07:27:58.533194 mikrotik-bt5-1.0.0/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      501 2024-05-03 08:43:20.000000 mikrotik-bt5-1.0.0/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-06 07:27:58.513194 mikrotik-bt5-1.0.0/mikrotik_bt5/
+-rw-r--r--   0 pi        (1000) pi        (1000)       90 2024-05-04 05:52:43.000000 mikrotik-bt5-1.0.0/mikrotik_bt5/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3470 2024-05-05 07:24:14.000000 mikrotik-bt5-1.0.0/mikrotik_bt5/beacon.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1880 2024-05-04 05:49:06.000000 mikrotik-bt5-1.0.0/mikrotik_bt5/client.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-06 07:27:58.525194 mikrotik-bt5-1.0.0/mikrotik_bt5.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)      866 2024-05-06 07:27:57.000000 mikrotik-bt5-1.0.0/mikrotik_bt5.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      315 2024-05-06 07:27:58.000000 mikrotik-bt5-1.0.0/mikrotik_bt5.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-05-06 07:27:57.000000 mikrotik-bt5-1.0.0/mikrotik_bt5.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        6 2024-05-06 07:27:57.000000 mikrotik-bt5-1.0.0/mikrotik_bt5.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       19 2024-05-06 07:27:57.000000 mikrotik-bt5-1.0.0/mikrotik_bt5.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2024-05-06 07:27:58.537194 mikrotik-bt5-1.0.0/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      637 2024-05-06 07:26:52.000000 mikrotik-bt5-1.0.0/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-06 07:27:58.529194 mikrotik-bt5-1.0.0/tests/
+-rw-r--r--   0 pi        (1000) pi        (1000)       44 2024-05-05 07:27:22.000000 mikrotik-bt5-1.0.0/tests/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2767 2024-05-05 07:27:22.000000 mikrotik-bt5-1.0.0/tests/test_advertisements.py
```

### Comparing `mikrotik-bt5-0.0.2b4/PKG-INFO` & `mikrotik-bt5-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikrotik-bt5
-Version: 0.0.2b4
+Version: 1.0.0
 Summary: MikroTik BT5 scanner
 Home-page: https://github.com/Anrijs/MikroTik-BT5-Python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `mikrotik-bt5-0.0.2b4/mikrotik_bt5/beacon.py` & `mikrotik-bt5-1.0.0/mikrotik_bt5/beacon.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,24 +31,22 @@
             zz = self.z * self.z
 
             ms = math.sqrt(xx + yy + zz)
             return ms
 
     name: str = "MikroTik BT5"
     address: str | None = None
-    mac: bytearray | None = None
     version: int | None = None
     udata: int | None = None
     salt: int | None = None
     acceleration: Acceleration | None = None
     temperature: float | None = None
     uptime: int | None = None
     flags: int | None = None
     battery: int | None = None
-    voltage: int | None = None
     rssi: int | None = None
 
     def __init__(self, device = None, ad_data = None):
         super().__init__(BeaconType.MIKROTIK.value)
 
         if device and ad_data and MikrotikBeacon.MIKROTIK_ID in ad_data.manufacturer_data:
             if device.name:
@@ -62,16 +60,14 @@
             version = int(raw_bytes[0])
             value_fmt = None
 
             if version == 0:
                 value_fmt = "<BBHhhhbIBB"
             elif version == 1:
                 value_fmt = "<BBHhhhhIBB"
-            elif version == 2:
-                value_fmt = "<BBIhhBBBBBB"
             else:
                 self.version = None
                 return
                 # invalid/unknown version
 
             if value_fmt:
                 value = struct.unpack(value_fmt, raw_bytes)
@@ -104,32 +100,24 @@
         if value[6] != -32768:
             self.temperature = value[6] / 256.0
 
         self.uptime = value[7]
         self.flags = value[8]
         self.battery = value[9]
 
-    def decode_v2(self, value: tuple):
-        if value[1] == 0:
-            self.temperature = value[4] / 256.0
-        else:
-            self.temperature = value[4] / 128.0
-        self.uptime = value[2]
-        self.voltage = value[3]
-        self.mac = bytearray(value[5:11])
-
     def decode(self, value: tuple):
         self.version = value[0]
 
         if self.version == 0:
             self.decode_v0(value)
         elif self.version == 1:
             self.decode_v1(value)
-        elif self.version == 2:
-            self.decode_v2(value)
+
+    def hasTemperature(self):
+        return self.temperature and self.temperature != -128.0
 
     def toDict(self):
         return {
             "version": self.version,
             "acceleration": {
                 "x": self.acceleration.x,
                 "y": self.acceleration.y,
```

### Comparing `mikrotik-bt5-0.0.2b4/mikrotik_bt5/client.py` & `mikrotik-bt5-1.0.0/mikrotik_bt5/client.py`

 * *Files identical despite different names*

### Comparing `mikrotik-bt5-0.0.2b4/mikrotik_bt5.egg-info/PKG-INFO` & `mikrotik-bt5-1.0.0/mikrotik_bt5.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikrotik-bt5
-Version: 0.0.2b4
+Version: 1.0.0
 Summary: MikroTik BT5 scanner
 Home-page: https://github.com/Anrijs/MikroTik-BT5-Python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `mikrotik-bt5-0.0.2b4/setup.py` & `mikrotik-bt5-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mikrotik-bt5",
-    version="0.0.2b4",
+    version="1.0.0",
     description="MikroTik BT5 scanner",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Anrijs/MikroTik-BT5-Python",
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python',
```

### Comparing `mikrotik-bt5-0.0.2b4/tests/test_advertisements.py` & `mikrotik-bt5-1.0.0/tests/test_advertisements.py`

 * *Files identical despite different names*

