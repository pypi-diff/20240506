# Comparing `tmp/new_natnet_client-4.1.1.tar.gz` & `tmp/new_natnet_client-4.1.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_natnet_client-4.1.1.tar", max compression
+gzip compressed data, was "new_natnet_client-4.1.2b0.tar", max compression
```

## Comparing `new_natnet_client-4.1.1.tar` & `new_natnet_client-4.1.2b0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      958 2024-05-03 00:35:37.958385 new_natnet_client-4.1.1/LICENSE
--rw-r--r--   0        0        0      632 2024-05-03 00:10:07.988386 new_natnet_client-4.1.1/README.md
--rw-r--r--   0        0        0    14899 2024-05-03 18:56:14.035147 new_natnet_client-4.1.1/new_natnet_client/Client.py
--rw-r--r--   0        0        0     8503 2024-05-03 19:22:30.032709 new_natnet_client-4.1.1/new_natnet_client/NatNetTypes.py
--rw-r--r--   0        0        0    26364 2024-05-03 00:54:50.418386 new_natnet_client-4.1.1/new_natnet_client/Unpackers.py
--rw-r--r--   0        0        0        0 2024-05-03 00:03:07.918385 new_natnet_client-4.1.1/new_natnet_client/__init__.py
--rw-r--r--   0        0        0      463 2024-05-03 19:31:15.406787 new_natnet_client-4.1.1/pyproject.toml
--rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 new_natnet_client-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0      958 2024-05-03 00:35:37.958385 new_natnet_client-4.1.2b0/LICENSE
+-rw-r--r--   0        0        0      632 2024-05-03 00:10:07.988386 new_natnet_client-4.1.2b0/README.md
+-rw-r--r--   0        0        0    15156 2024-05-06 17:11:06.228822 new_natnet_client-4.1.2b0/new_natnet_client/Client.py
+-rw-r--r--   0        0        0     8503 2024-05-03 19:22:30.032709 new_natnet_client-4.1.2b0/new_natnet_client/NatNetTypes.py
+-rw-r--r--   0        0        0    26344 2024-05-06 17:10:29.068824 new_natnet_client-4.1.2b0/new_natnet_client/Unpackers.py
+-rw-r--r--   0        0        0        0 2024-05-03 00:03:07.918385 new_natnet_client-4.1.2b0/new_natnet_client/__init__.py
+-rw-r--r--   0        0        0      467 2024-05-06 17:17:17.548785 new_natnet_client-4.1.2b0/pyproject.toml
+-rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 new_natnet_client-4.1.2b0/PKG-INFO
```

### Comparing `new_natnet_client-4.1.1/LICENSE` & `new_natnet_client-4.1.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.1.1/README.md` & `new_natnet_client-4.1.2b0/README.md`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.1.1/new_natnet_client/Client.py` & `new_natnet_client-4.1.2b0/new_natnet_client/Client.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   server_address: str = "127.0.0.1"
   local_ip_address: str = "127.0.0.1"
   use_multicast: bool = True
   multicast_address: str ="239.255.42.99"
   command_port: int = 1510
   data_port: int = 1511
   max_buffer_size: InitVar[int] = 255
-  mocap: MoCap | None = field(init=False, default=None)
+  __mocap_bytes: bytes | None = field(init=False, default=None)
   __can_change_bitstream: bool = field(init=False, default=False)
   __running: bool = field(init=False, default=False)
   __command_socket: socket.socket | None = field(init=False, repr=False, default=None)
   __data_socket: socket.socket | None = field(init=False, repr=False, default=None)
   __freeze: bool = field(init=False, repr=False, default=False)
 
   # TODO: Add bitstream change support
@@ -43,14 +43,20 @@
 
   @property
   def server_info(self) -> Server_info:
     with self.__server_info_lock:
       return copy(self.__server_info)
 
   @property
+  def MoCap(self) -> MoCap | None:
+    with self.__mocap_bytes_lock:
+      if self.__mocap_bytes is None: return None
+      return self.__unpacker.unpack_mocap_data(self.__mocap_bytes)
+
+  @property
   def server_responses(self) -> deque[int | str]:
     with self.__server_responses_lock:
       return self.__server_responses.copy()
 
   @property
   def server_messages(self) -> deque[str]:
     with self.__server_messages_lock:
@@ -123,14 +129,15 @@
 
   def __post_init__(self, max_buffer_size):
     self.__running_lock = Lock()
     self.__command_socket_lock = Lock()
     self.__server_info_lock = Lock()
     self.__server_responses_lock = Lock()
     self.__server_messages_lock = Lock()
+    self.__mocap_bytes_lock = Lock()
 
     self.__max_buffer_size = max_buffer_size
     # Buffer for server responses
     self.__server_responses: deque[int | str] = deque(maxlen=self.__max_buffer_size)
     # Buffer for server messages
     self.__server_messages: deque[str] = deque(maxlen=self.__max_buffer_size)
 
@@ -242,16 +249,17 @@
       NAT_Data.FORCE_PLATE: self.__unpacker.unpack_force_plate_description,
       NAT_Data.DEVICE: self.__unpacker.unpack_device_description,
       NAT_Data.CAMERA: self.__unpacker.unpack_camera_description,
       NAT_Data.ASSET: self.__unpacker.unpack_asset_description
     }
 
   def __unpack_mocap_data(self, data:bytes, packet_size:int):
-    self.mocap, offset = self.__unpacker.unpack_mocap_data(data)
-    return offset
+    with self.__mocap_bytes_lock:
+      self.__mocap_bytes = data
+    return packet_size
 
   def __unpack_data_descriptions(self, data:bytes, packet_size:int):
     offset = 0
     dataset_count = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     for i in range(dataset_count):
       t = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
       if self.__unpacker == DataUnpackerV4_1:
```

### Comparing `new_natnet_client-4.1.1/new_natnet_client/NatNetTypes.py` & `new_natnet_client-4.1.2b0/new_natnet_client/NatNetTypes.py`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.1.1/new_natnet_client/Unpackers.py` & `new_natnet_client-4.1.2b0/new_natnet_client/Unpackers.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
     template['stamp_transmit'] = int.from_bytes(data[offset:(offset:=offset+8)], byteorder='little', signed=True)
     param = unpack( 'h', data[offset:(offset:=offset+2)])[0]
     template['recording'] = bool(param & 0x01)
     template['tracked_models_changed'] = bool(param & 0x02)
     return NatNetTypes.Frame_suffix(**template), offset
 
   @classmethod
-  def unpack_mocap_data(cls, data:bytes) -> Tuple[NatNetTypes.MoCap, int]:
+  def unpack_mocap_data(cls, data:bytes) -> NatNetTypes.MoCap:
     offset = 0
     tmp_offset = 0
     template = {}
 
     template['prefix_data'], tmp_offset = cls.unpack_frame_prefix_data(data[offset:])
     offset += tmp_offset
 
@@ -244,15 +244,15 @@
 
     template['device_data'], tmp_offset = cls.unpack_device_data(data[offset:])
     offset += tmp_offset
 
     template['suffix_data'], tmp_offset = cls.unpack_frame_suffix_data(data[offset:])
     offset += tmp_offset
 
-    return NatNetTypes.MoCap(**template), offset
+    return NatNetTypes.MoCap(**template)
 
   @classmethod
   def unpack_marker_set_description(cls, data:bytes) -> Tuple[Dict[str, NatNetTypes.Marker_set_description], int]:
     offset = 0
     template = {}
     name, _, _ = data[offset:].partition(b'\0')
     offset += len(name) + 1
```

### Comparing `new_natnet_client-4.1.1/PKG-INFO` & `new_natnet_client-4.1.2b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: new-natnet-client
-Version: 4.1.1
+Version: 4.1.2b0
 Summary: natnet client for motive application for python
 Home-page: https://optitrack.com/
 License: GLWTPL
 Author: Ignacio de la Torre Arias
 Author-email: ignaciodlta@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

