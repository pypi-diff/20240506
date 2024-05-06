# Comparing `tmp/new_natnet_client-4.1.2b0.tar.gz` & `tmp/new_natnet_client-4.1.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_natnet_client-4.1.2b0.tar", max compression
+gzip compressed data, was "new_natnet_client-4.1.2b1.tar", max compression
```

## Comparing `new_natnet_client-4.1.2b0.tar` & `new_natnet_client-4.1.2b1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      958 2024-05-03 00:35:37.958385 new_natnet_client-4.1.2b0/LICENSE
--rw-r--r--   0        0        0      632 2024-05-03 00:10:07.988386 new_natnet_client-4.1.2b0/README.md
--rw-r--r--   0        0        0    15156 2024-05-06 17:11:06.228822 new_natnet_client-4.1.2b0/new_natnet_client/Client.py
--rw-r--r--   0        0        0     8503 2024-05-03 19:22:30.032709 new_natnet_client-4.1.2b0/new_natnet_client/NatNetTypes.py
--rw-r--r--   0        0        0    26344 2024-05-06 17:10:29.068824 new_natnet_client-4.1.2b0/new_natnet_client/Unpackers.py
--rw-r--r--   0        0        0        0 2024-05-03 00:03:07.918385 new_natnet_client-4.1.2b0/new_natnet_client/__init__.py
--rw-r--r--   0        0        0      467 2024-05-06 17:17:17.548785 new_natnet_client-4.1.2b0/pyproject.toml
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 new_natnet_client-4.1.2b0/PKG-INFO
+-rw-r--r--   0        0        0      958 2024-05-03 00:35:37.958385 new_natnet_client-4.1.2b1/LICENSE
+-rw-r--r--   0        0        0      632 2024-05-03 00:10:07.988386 new_natnet_client-4.1.2b1/README.md
+-rw-r--r--   0        0        0    15156 2024-05-06 17:11:06.228822 new_natnet_client-4.1.2b1/new_natnet_client/Client.py
+-rw-r--r--   0        0        0     8498 2024-05-06 18:27:28.019509 new_natnet_client-4.1.2b1/new_natnet_client/NatNetTypes.py
+-rw-r--r--   0        0        0    26344 2024-05-06 17:10:29.068824 new_natnet_client-4.1.2b1/new_natnet_client/Unpackers.py
+-rw-r--r--   0        0        0        0 2024-05-03 00:03:07.918385 new_natnet_client-4.1.2b1/new_natnet_client/__init__.py
+-rw-r--r--   0        0        0      468 2024-05-06 18:28:08.769527 new_natnet_client-4.1.2b1/pyproject.toml
+-rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 new_natnet_client-4.1.2b1/PKG-INFO
```

### Comparing `new_natnet_client-4.1.2b0/LICENSE` & `new_natnet_client-4.1.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.1.2b0/README.md` & `new_natnet_client-4.1.2b1/README.md`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.1.2b0/new_natnet_client/Client.py` & `new_natnet_client-4.1.2b1/new_natnet_client/Client.py`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.1.2b0/new_natnet_client/NatNetTypes.py` & `new_natnet_client-4.1.2b1/new_natnet_client/NatNetTypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
 @dataclass(frozen=True)
 class Device_data(MoCapData):
   num_devices: int
   devices: Tuple[Device, ...]
   devices_d: Dict[int, Device] = field(init=False)
   
   def __post_init__(self):
-    object.__setattr__(self, "rigid_bodies_d", { instance.id : instance for instance in self.devices})
+    object.__setattr__(self, "devices_d", { instance.id : instance for instance in self.devices})
 
 @dataclass(frozen=True)
 class Frame_suffix:
   time_code: int
   time_code_sub: int
   timestamp: float
   camera_mid_exposure: int
```

### Comparing `new_natnet_client-4.1.2b0/new_natnet_client/Unpackers.py` & `new_natnet_client-4.1.2b1/new_natnet_client/Unpackers.py`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.1.2b0/PKG-INFO` & `new_natnet_client-4.1.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: new-natnet-client
-Version: 4.1.2b0
+Version: 4.1.2b1
 Summary: natnet client for motive application for python
 Home-page: https://optitrack.com/
 License: GLWTPL
 Author: Ignacio de la Torre Arias
 Author-email: ignaciodlta@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

