# Comparing `tmp/new_natnet_client-4.1.2b1.tar.gz` & `tmp/new_natnet_client-4.1.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_natnet_client-4.1.2b1.tar", max compression
+gzip compressed data, was "new_natnet_client-4.1.2b2.tar", max compression
```

## Comparing `new_natnet_client-4.1.2b1.tar` & `new_natnet_client-4.1.2b2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      958 2024-05-03 00:35:37.958385 new_natnet_client-4.1.2b1/LICENSE
--rw-r--r--   0        0        0      632 2024-05-03 00:10:07.988386 new_natnet_client-4.1.2b1/README.md
--rw-r--r--   0        0        0    15156 2024-05-06 17:11:06.228822 new_natnet_client-4.1.2b1/new_natnet_client/Client.py
--rw-r--r--   0        0        0     8498 2024-05-06 18:27:28.019509 new_natnet_client-4.1.2b1/new_natnet_client/NatNetTypes.py
--rw-r--r--   0        0        0    26344 2024-05-06 17:10:29.068824 new_natnet_client-4.1.2b1/new_natnet_client/Unpackers.py
--rw-r--r--   0        0        0        0 2024-05-03 00:03:07.918385 new_natnet_client-4.1.2b1/new_natnet_client/__init__.py
--rw-r--r--   0        0        0      468 2024-05-06 18:28:08.769527 new_natnet_client-4.1.2b1/pyproject.toml
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 new_natnet_client-4.1.2b1/PKG-INFO
+-rw-r--r--   0        0        0      958 2024-05-03 00:35:37.958385 new_natnet_client-4.1.2b2/LICENSE
+-rw-r--r--   0        0        0      632 2024-05-03 00:10:07.988386 new_natnet_client-4.1.2b2/README.md
+-rw-r--r--   0        0        0    15156 2024-05-06 17:11:06.228822 new_natnet_client-4.1.2b2/new_natnet_client/Client.py
+-rw-r--r--   0        0        0     8498 2024-05-06 18:27:28.019509 new_natnet_client-4.1.2b2/new_natnet_client/NatNetTypes.py
+-rw-r--r--   0        0        0    26325 2024-05-06 18:46:40.709526 new_natnet_client-4.1.2b2/new_natnet_client/Unpackers.py
+-rw-r--r--   0        0        0        0 2024-05-03 00:03:07.918385 new_natnet_client-4.1.2b2/new_natnet_client/__init__.py
+-rw-r--r--   0        0        0      468 2024-05-06 18:47:13.599526 new_natnet_client-4.1.2b2/pyproject.toml
+-rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 new_natnet_client-4.1.2b2/PKG-INFO
```

### Comparing `new_natnet_client-4.1.2b1/LICENSE` & `new_natnet_client-4.1.2b2/LICENSE`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.1.2b1/README.md` & `new_natnet_client-4.1.2b2/README.md`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.1.2b1/new_natnet_client/Client.py` & `new_natnet_client-4.1.2b2/new_natnet_client/Client.py`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.1.2b1/new_natnet_client/NatNetTypes.py` & `new_natnet_client-4.1.2b2/new_natnet_client/NatNetTypes.py`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.1.2b1/new_natnet_client/Unpackers.py` & `new_natnet_client-4.1.2b2/new_natnet_client/Unpackers.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,15 +494,15 @@
     template['precision_timestamp_frac_sec'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     param = unpack( 'h', data[offset:(offset:=offset+2)])[0]
     template['recording'] = bool(param & 0x01)
     template['tracked_models_changed'] = bool(param & 0x02)
     return NatNetTypes.Frame_suffix(**template), offset
 
   @classmethod
-  def unpack_mocap_data(cls, data:bytes) -> Tuple[NatNetTypes.MoCap,int]:
+  def unpack_mocap_data(cls, data:bytes) -> NatNetTypes.MoCap:
     offset = 0
     tmp_offset = 0
     template = {}
 
     template['prefix_data'], tmp_offset = cls.unpack_frame_prefix_data(data[offset:])
     offset += tmp_offset
 
@@ -529,15 +529,15 @@
 
     template['device_data'], tmp_offset = cls.unpack_device_data(data[offset:])
     offset += tmp_offset
 
     template['suffix_data'], tmp_offset = cls.unpack_frame_suffix_data(data[offset:])
     offset += tmp_offset
 
-    return NatNetTypes.MoCap(**template), offset
+    return NatNetTypes.MoCap(**template)
 
   @classmethod
   def unpack_rigid_body_description(cls, data: bytes) -> Tuple[Dict[int, NatNetTypes.Rigid_body_description], int]:
     d, offset = super().unpack_rigid_body_description(data)
     rb_desc = asdict(list(d.values())[0])
     markers = deque()
     for marker in rb_desc['markers']:
```

### Comparing `new_natnet_client-4.1.2b1/PKG-INFO` & `new_natnet_client-4.1.2b2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: new-natnet-client
-Version: 4.1.2b1
+Version: 4.1.2b2
 Summary: natnet client for motive application for python
 Home-page: https://optitrack.com/
 License: GLWTPL
 Author: Ignacio de la Torre Arias
 Author-email: ignaciodlta@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

