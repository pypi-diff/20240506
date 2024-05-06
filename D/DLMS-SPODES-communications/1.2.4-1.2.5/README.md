# Comparing `tmp/DLMS_SPODES_communications-1.2.4.tar.gz` & `tmp/DLMS_SPODES_communications-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLMS_SPODES_communications-1.2.4.tar", last modified: Wed Apr 10 06:46:47 2024, max compression
+gzip compressed data, was "DLMS_SPODES_communications-1.2.5.tar", last modified: Mon May  6 06:45:46 2024, max compression
```

## Comparing `DLMS_SPODES_communications-1.2.4.tar` & `DLMS_SPODES_communications-1.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 06:46:47.809666 DLMS_SPODES_communications-1.2.4/
--rw-rw-rw-   0        0        0      527 2024-04-10 06:46:47.808664 DLMS_SPODES_communications-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       61 2024-01-18 10:40:20.000000 DLMS_SPODES_communications-1.2.4/README.md
--rw-rw-rw-   0        0        0      851 2024-04-10 06:41:28.000000 DLMS_SPODES_communications-1.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 06:46:47.810667 DLMS_SPODES_communications-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0       43 2024-01-19 07:53:50.000000 DLMS_SPODES_communications-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 06:46:47.770662 DLMS_SPODES_communications-1.2.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-10 06:46:47.788663 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/
--rw-rw-rw-   0        0        0      572 2024-02-14 09:26:43.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/__init__.py
--rw-rw-rw-   0        0        0     2769 2024-04-10 06:04:37.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/base.py
--rw-rw-rw-   0        0        0    11579 2024-01-19 05:28:12.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/ble.py
--rw-rw-rw-   0        0        0     3094 2024-02-14 09:17:34.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/network.py
--rw-rw-rw-   0        0        0     4366 2024-04-10 06:11:51.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/serial_port.py
-drwxrwxrwx   0        0        0        0 2024-04-10 06:46:47.802665 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/
--rw-rw-rw-   0        0        0      527 2024-04-10 06:46:47.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      608 2024-04-10 06:46:47.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 06:46:47.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-04-10 06:46:47.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       65 2024-04-10 06:46:47.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-04-10 06:46:47.000000 DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 06:46:47.806663 DLMS_SPODES_communications-1.2.4/test/
--rw-rw-rw-   0        0        0     1035 2024-02-14 09:19:03.000000 DLMS_SPODES_communications-1.2.4/test/test_Network.py
--rw-rw-rw-   0        0        0     1695 2024-04-10 06:09:40.000000 DLMS_SPODES_communications-1.2.4/test/test_Serial.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:45:46.807830 DLMS_SPODES_communications-1.2.5/
+-rw-rw-rw-   0        0        0      527 2024-05-06 06:45:46.806862 DLMS_SPODES_communications-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       61 2024-01-18 10:40:20.000000 DLMS_SPODES_communications-1.2.5/README.md
+-rw-rw-rw-   0        0        0      851 2024-05-06 06:45:19.000000 DLMS_SPODES_communications-1.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 06:45:46.807830 DLMS_SPODES_communications-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0       43 2024-01-19 07:53:50.000000 DLMS_SPODES_communications-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:45:46.768826 DLMS_SPODES_communications-1.2.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 06:45:46.786826 DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications/
+-rw-rw-rw-   0        0        0      572 2024-02-14 09:26:43.000000 DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications/__init__.py
+-rw-rw-rw-   0        0        0     2769 2024-04-10 06:04:37.000000 DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications/base.py
+-rw-rw-rw-   0        0        0    11552 2024-05-06 06:44:34.000000 DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications/ble.py
+-rw-rw-rw-   0        0        0     3168 2024-05-06 06:32:17.000000 DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications/network.py
+-rw-rw-rw-   0        0        0     4439 2024-05-06 06:44:34.000000 DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications/serial_port.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:45:46.799827 DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications.egg-info/
+-rw-rw-rw-   0        0        0      527 2024-05-06 06:45:46.000000 DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      608 2024-05-06 06:45:46.000000 DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 06:45:46.000000 DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-06 06:45:46.000000 DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       65 2024-05-06 06:45:46.000000 DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-06 06:45:46.000000 DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 06:45:46.804829 DLMS_SPODES_communications-1.2.5/test/
+-rw-rw-rw-   0        0        0     1035 2024-02-14 09:19:03.000000 DLMS_SPODES_communications-1.2.5/test/test_Network.py
+-rw-rw-rw-   0        0        0     1695 2024-04-10 06:09:40.000000 DLMS_SPODES_communications-1.2.5/test/test_Serial.py
```

### Comparing `DLMS_SPODES_communications-1.2.4/PKG-INFO` & `DLMS_SPODES_communications-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS_SPODES_communications
-Version: 1.2.4
+Version: 1.2.5
 Summary: dlms-spodes
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/DLMSSPODEScommunication_prj
 Keywords: dlms,drivers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DLMS_SPODES_communications-1.2.4/pyproject.toml` & `DLMS_SPODES_communications-1.2.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [project]
 name = "DLMS_SPODES_communications"
-version = "1.2.4"
+version = "1.2.5"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 dependencies = [
     "bleak==0.20.2",
     "netaddr>=0.8.0",
     "pyserial>=3.5",
```

### Comparing `DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/__init__.py` & `DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/base.py` & `DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications/base.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/ble.py` & `DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications/ble.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         if self.discovery_timeout != self.DISCOVERY_TIMEOUT_DEFAULT:
             params.append(F"discovery_timeout={self.discovery_timeout}")
         if self.octet_timeout != self.OCTET_TIMEOUT_DEFAULT:
             params.append(F"octet_timeout={self.octet_timeout}")
         return F"{self.__class__.__name__}({', '.join(params)})"
 
     def __str__(self):
-        return F"{self.__class__.__name__}: {self.__client.address}"
+        return F"{self.__client.address}"
 
     @property
     def client(self) -> bleak.BleakClient:
         return self.__client
 
     def addListener(self, listener):
         raise NotImplementedError()
```

### Comparing `DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/network.py` & `DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications/network.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,7 +92,10 @@
         return F"{self.__class__.__name__}({', '.join(params)})"
 
     async def open(self):
         """ coroutine start """
         self.reader, self.writer = await asyncio.open_connection(
             host=self.host_name,
             port=self.port)
+
+    def __str__(self):
+        return F"{self.host_name}:{self.port}"
```

### Comparing `DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications/serial_port.py` & `DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications/serial_port.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,7 +132,10 @@
         self.reader, self.writer = await open_serial_connection(
             url=self.port,
             baudrate=self.baudrate)
 
     async def close(self):
         await asyncio.sleep(.1)  # need delay before close writer
         await super(AsyncSerial, self).close()
+
+    def __str__(self):
+        return F"{self.port},{self.baudrate}"
```

### Comparing `DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/PKG-INFO` & `DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS-SPODES-communications
-Version: 1.2.4
+Version: 1.2.5
 Summary: dlms-spodes
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/DLMSSPODEScommunication_prj
 Keywords: dlms,drivers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DLMS_SPODES_communications-1.2.4/src/DLMS_SPODES_communications.egg-info/SOURCES.txt` & `DLMS_SPODES_communications-1.2.5/src/DLMS_SPODES_communications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_communications-1.2.4/test/test_Network.py` & `DLMS_SPODES_communications-1.2.5/test/test_Network.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_communications-1.2.4/test/test_Serial.py` & `DLMS_SPODES_communications-1.2.5/test/test_Serial.py`

 * *Files identical despite different names*

