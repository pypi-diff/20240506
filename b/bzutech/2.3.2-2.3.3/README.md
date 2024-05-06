# Comparing `tmp/bzutech-2.3.2.tar.gz` & `tmp/bzutech-2.3.3.tar.gz`

## Comparing `bzutech-2.3.2.tar` & `bzutech-2.3.3.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 bzutech-2.3.2/setup.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 bzutech-2.3.2/test.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bzutech-2.3.2/build/lib/bzutech/__init__.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bzutech-2.3.2/bzutech/__init__.py
--rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 bzutech-2.3.2/bzutech/bzutechapi/BzuTechAPI.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 bzutech-2.3.2/bzutech/bzutechapi/__init__.py
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 bzutech-2.3.2/bzutech/device/Device.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bzutech-2.3.2/bzutech/device/__init__.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 bzutech-2.3.2/bzutech/sensor/Sensor.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bzutech-2.3.2/bzutech/sensor/__init__.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 bzutech-2.3.2/bzutech.egg-info/PKG-INFO
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 bzutech-2.3.2/bzutech.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 bzutech-2.3.2/bzutech.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bzutech-2.3.2/bzutech.egg-info/requires.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bzutech-2.3.2/bzutech.egg-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bzutech-2.3.2/tests/main.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 bzutech-2.3.2/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 bzutech-2.3.2/pyproject.toml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bzutech-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 bzutech-2.3.3/setup.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 bzutech-2.3.3/test.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bzutech-2.3.3/build/lib/bzutech/__init__.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bzutech-2.3.3/bzutech/__init__.py
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 bzutech-2.3.3/bzutech/bzutechapi/BzuTechAPI.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 bzutech-2.3.3/bzutech/bzutechapi/__init__.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 bzutech-2.3.3/bzutech/device/Device.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bzutech-2.3.3/bzutech/device/__init__.py
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 bzutech-2.3.3/bzutech/sensor/Sensor.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bzutech-2.3.3/bzutech/sensor/__init__.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 bzutech-2.3.3/bzutech.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 bzutech-2.3.3/bzutech.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 bzutech-2.3.3/bzutech.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bzutech-2.3.3/bzutech.egg-info/requires.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bzutech-2.3.3/bzutech.egg-info/top_level.txt
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 bzutech-2.3.3/README.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 bzutech-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bzutech-2.3.3/PKG-INFO
```

### Comparing `bzutech-2.3.2/bzutech/bzutechapi/BzuTechAPI.py` & `bzutech-2.3.3/bzutech/bzutechapi/BzuTechAPI.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,13 +94,17 @@
     
     def get_reading(self, chipid: str, sensorname:str):
         return self.dispositivos[chipid].get_readings(sensorname.upper())
 
     async def send_reading(self, sensoref:str, DeviceID: str, reading: float, date: str):
         url = "https://back-dev.bzutech.com.br/logs/home_assistence/"
         data = '{"bci":"'+DeviceID+'", "date":"'+ date +'", "data":\"[{\'ref\':\''+ sensoref +'\',\'med\':'+ str(reading) +'}]\"}'
+        print(data)
         data = json.loads(data)
         client = ClientSession()
-        async with client.post(url, json=data, headers = self.httpheaders) as resp:
+        async with client.post(url, json=data) as resp:
             await client.close()
-            return resp.text != "[]"
-        
+            print(resp.text)
+            return (data, resp.text)
+
+    def get_apiversion(self):
+        return "2.3.3"
```

### Comparing `bzutech-2.3.2/bzutech/device/Device.py` & `bzutech-2.3.3/bzutech/device/Device.py`

 * *Files identical despite different names*

### Comparing `bzutech-2.3.2/bzutech/sensor/Sensor.py` & `bzutech-2.3.3/bzutech/sensor/Sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,8 +113,9 @@
         )
         client = ClientSession( )
         async with client.get(url, headers = self.httpheaders) as resp:
             resposta = await resp.json()
             await client.close()
             if("medicao" in resposta):
                 self.last_reading = int(resposta["medicao"]) / 1000000
+            print(resposta)
             return self.last_reading
```

### Comparing `bzutech-2.3.2/bzutech.egg-info/PKG-INFO` & `bzutech-2.3.3/bzutech.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `bzutech-2.3.2/PKG-INFO` & `bzutech-2.3.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.3
 Name: bzutech
-Version: 2.3.2
+Version: 2.3.3
 Summary: Integration package for bzutech services
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Author-email: Ênio Ferreira <e.nioferreira@hotmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: aiohttp
-Requires-Dist: paho-mqtt
 Description-Content-Type: text/markdown
 
 # BZUTech API
```

