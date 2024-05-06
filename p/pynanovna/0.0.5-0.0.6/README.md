# Comparing `tmp/pynanovna-0.0.5.tar.gz` & `tmp/pynanovna-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynanovna-0.0.5.tar", last modified: Sat May  4 14:42:23 2024, max compression
+gzip compressed data, was "pynanovna-0.0.6.tar", last modified: Mon May  6 16:31:42 2024, max compression
```

## Comparing `pynanovna-0.0.5.tar` & `pynanovna-0.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-04 14:42:23.060435 pynanovna-0.0.5/
--rw-r--r--   0 teo        (501) staff       (20)      895 2024-04-25 07:30:24.000000 pynanovna-0.0.5/LICENCE
--rw-r--r--   0 teo        (501) staff       (20)     1333 2024-05-04 14:42:23.059227 pynanovna-0.0.5/PKG-INFO
--rw-r--r--   0 teo        (501) staff       (20)      676 2024-05-04 14:41:16.000000 pynanovna-0.0.5/README.md
--rw-r--r--   0 teo        (501) staff       (20)      637 2024-05-04 14:21:36.000000 pynanovna-0.0.5/pyproject.toml
--rw-r--r--   0 teo        (501) staff       (20)       38 2024-05-04 14:42:23.060787 pynanovna-0.0.5/setup.cfg
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-04 14:42:23.035294 pynanovna-0.0.5/src/
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-04 14:42:23.043606 pynanovna-0.0.5/src/pynanovna/
--rw-r--r--   0 teo        (501) staff       (20)    16095 2024-05-04 11:44:22.000000 pynanovna-0.0.5/src/pynanovna/Calibration.py
--rw-r--r--   0 teo        (501) staff       (20)     8952 2024-05-04 11:44:22.000000 pynanovna-0.0.5/src/pynanovna/CalibrationGuide.py
--rw-r--r--   0 teo        (501) staff       (20)     4526 2024-04-25 06:16:41.000000 pynanovna-0.0.5/src/pynanovna/RFTools.py
--rw-r--r--   0 teo        (501) staff       (20)     5697 2024-04-25 06:16:34.000000 pynanovna-0.0.5/src/pynanovna/SITools.py
--rw-r--r--   0 teo        (501) staff       (20)     4626 2024-04-25 06:12:36.000000 pynanovna-0.0.5/src/pynanovna/Sweep.py
--rw-r--r--   0 teo        (501) staff       (20)    11096 2024-05-04 13:32:02.000000 pynanovna-0.0.5/src/pynanovna/SweepWorker.py
--rw-r--r--   0 teo        (501) staff       (20)     8824 2024-05-04 11:44:22.000000 pynanovna-0.0.5/src/pynanovna/Touchstone.py
--rw-r--r--   0 teo        (501) staff       (20)      101 2024-05-04 14:14:44.000000 pynanovna-0.0.5/src/pynanovna/__init__.py
--rw-r--r--   0 teo        (501) staff       (20)      653 2024-05-04 14:20:41.000000 pynanovna-0.0.5/src/pynanovna/example.py
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-04 14:42:23.057460 pynanovna-0.0.5/src/pynanovna/hardware/
--rw-r--r--   0 teo        (501) staff       (20)      579 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/AVNA.py
--rw-r--r--   0 teo        (501) staff       (20)     5641 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/Hardware.py
--rw-r--r--   0 teo        (501) staff       (20)      541 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/JNCRadio_VNA_3G.py
--rw-r--r--   0 teo        (501) staff       (20)     4118 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/NanoVNA.py
--rw-r--r--   0 teo        (501) staff       (20)      270 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/NanoVNA_F.py
--rw-r--r--   0 teo        (501) staff       (20)      273 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/NanoVNA_F_V2.py
--rw-r--r--   0 teo        (501) staff       (20)      225 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/NanoVNA_H.py
--rw-r--r--   0 teo        (501) staff       (20)      453 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/NanoVNA_H4.py
--rw-r--r--   0 teo        (501) staff       (20)     9852 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/NanoVNA_V2.py
--rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/SV4401A.py
--rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/SV6301A.py
--rw-r--r--   0 teo        (501) staff       (20)      966 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/Serial.py
--rw-r--r--   0 teo        (501) staff       (20)     3369 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/TinySA.py
--rw-r--r--   0 teo        (501) staff       (20)     6482 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/VNA.py
--rw-r--r--   0 teo        (501) staff       (20)      743 2024-04-25 05:48:01.000000 pynanovna-0.0.5/src/pynanovna/hardware/Version.py
--rw-r--r--   0 teo        (501) staff       (20)    10060 2024-05-04 13:34:06.000000 pynanovna-0.0.5/src/pynanovna/pynanovna.py
--rw-r--r--   0 teo        (501) staff       (20)     3973 2024-05-04 14:02:01.000000 pynanovna-0.0.5/src/pynanovna/vis.py
-drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-04 14:42:23.058238 pynanovna-0.0.5/src/pynanovna.egg-info/
--rw-r--r--   0 teo        (501) staff       (20)     1333 2024-05-04 14:42:23.000000 pynanovna-0.0.5/src/pynanovna.egg-info/PKG-INFO
--rw-r--r--   0 teo        (501) staff       (20)     1033 2024-05-04 14:42:23.000000 pynanovna-0.0.5/src/pynanovna.egg-info/SOURCES.txt
--rw-r--r--   0 teo        (501) staff       (20)        1 2024-05-04 14:42:23.000000 pynanovna-0.0.5/src/pynanovna.egg-info/dependency_links.txt
--rw-r--r--   0 teo        (501) staff       (20)       60 2024-05-04 14:42:23.000000 pynanovna-0.0.5/src/pynanovna.egg-info/requires.txt
--rw-r--r--   0 teo        (501) staff       (20)       10 2024-05-04 14:42:23.000000 pynanovna-0.0.5/src/pynanovna.egg-info/top_level.txt
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-06 16:31:42.725478 pynanovna-0.0.6/
+-rw-r--r--   0 teo        (501) staff       (20)      895 2024-04-25 07:30:24.000000 pynanovna-0.0.6/LICENCE
+-rw-r--r--   0 teo        (501) staff       (20)     1325 2024-05-06 16:31:42.724672 pynanovna-0.0.6/PKG-INFO
+-rw-r--r--   0 teo        (501) staff       (20)      668 2024-05-04 14:44:35.000000 pynanovna-0.0.6/README.md
+-rw-r--r--   0 teo        (501) staff       (20)      637 2024-05-06 16:31:13.000000 pynanovna-0.0.6/pyproject.toml
+-rw-r--r--   0 teo        (501) staff       (20)       38 2024-05-06 16:31:42.725646 pynanovna-0.0.6/setup.cfg
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-06 16:31:42.671632 pynanovna-0.0.6/src/
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-06 16:31:42.691628 pynanovna-0.0.6/src/pynanovna/
+-rw-r--r--   0 teo        (501) staff       (20)    16095 2024-05-04 11:44:22.000000 pynanovna-0.0.6/src/pynanovna/Calibration.py
+-rw-r--r--   0 teo        (501) staff       (20)     8952 2024-05-04 11:44:22.000000 pynanovna-0.0.6/src/pynanovna/CalibrationGuide.py
+-rw-r--r--   0 teo        (501) staff       (20)     4526 2024-04-25 06:16:41.000000 pynanovna-0.0.6/src/pynanovna/RFTools.py
+-rw-r--r--   0 teo        (501) staff       (20)     5697 2024-04-25 06:16:34.000000 pynanovna-0.0.6/src/pynanovna/SITools.py
+-rw-r--r--   0 teo        (501) staff       (20)     4626 2024-04-25 06:12:36.000000 pynanovna-0.0.6/src/pynanovna/Sweep.py
+-rw-r--r--   0 teo        (501) staff       (20)    11095 2024-05-06 16:28:01.000000 pynanovna-0.0.6/src/pynanovna/SweepWorker.py
+-rw-r--r--   0 teo        (501) staff       (20)     8824 2024-05-04 11:44:22.000000 pynanovna-0.0.6/src/pynanovna/Touchstone.py
+-rw-r--r--   0 teo        (501) staff       (20)      101 2024-05-04 14:14:44.000000 pynanovna-0.0.6/src/pynanovna/__init__.py
+-rw-r--r--   0 teo        (501) staff       (20)      653 2024-05-04 14:20:41.000000 pynanovna-0.0.6/src/pynanovna/example.py
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-06 16:31:42.719961 pynanovna-0.0.6/src/pynanovna/hardware/
+-rw-r--r--   0 teo        (501) staff       (20)      579 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/AVNA.py
+-rw-r--r--   0 teo        (501) staff       (20)     5641 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/Hardware.py
+-rw-r--r--   0 teo        (501) staff       (20)      541 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/JNCRadio_VNA_3G.py
+-rw-r--r--   0 teo        (501) staff       (20)     4134 2024-05-06 16:27:53.000000 pynanovna-0.0.6/src/pynanovna/hardware/NanoVNA.py
+-rw-r--r--   0 teo        (501) staff       (20)      270 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/NanoVNA_F.py
+-rw-r--r--   0 teo        (501) staff       (20)      273 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/NanoVNA_F_V2.py
+-rw-r--r--   0 teo        (501) staff       (20)      225 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/NanoVNA_H.py
+-rw-r--r--   0 teo        (501) staff       (20)      453 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/NanoVNA_H4.py
+-rw-r--r--   0 teo        (501) staff       (20)     9852 2024-05-06 15:57:18.000000 pynanovna-0.0.6/src/pynanovna/hardware/NanoVNA_V2.py
+-rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/SV4401A.py
+-rw-r--r--   0 teo        (501) staff       (20)      525 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/SV6301A.py
+-rw-r--r--   0 teo        (501) staff       (20)      966 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/Serial.py
+-rw-r--r--   0 teo        (501) staff       (20)     3369 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/TinySA.py
+-rw-r--r--   0 teo        (501) staff       (20)     6490 2024-05-06 16:28:00.000000 pynanovna-0.0.6/src/pynanovna/hardware/VNA.py
+-rw-r--r--   0 teo        (501) staff       (20)      743 2024-04-25 05:48:01.000000 pynanovna-0.0.6/src/pynanovna/hardware/Version.py
+-rw-r--r--   0 teo        (501) staff       (20)    10177 2024-05-06 16:24:11.000000 pynanovna-0.0.6/src/pynanovna/pynanovna.py
+-rw-r--r--   0 teo        (501) staff       (20)     3973 2024-05-04 14:02:01.000000 pynanovna-0.0.6/src/pynanovna/vis.py
+drwxr-xr-x   0 teo        (501) staff       (20)        0 2024-05-06 16:31:42.722318 pynanovna-0.0.6/src/pynanovna.egg-info/
+-rw-r--r--   0 teo        (501) staff       (20)     1325 2024-05-06 16:31:42.000000 pynanovna-0.0.6/src/pynanovna.egg-info/PKG-INFO
+-rw-r--r--   0 teo        (501) staff       (20)     1033 2024-05-06 16:31:42.000000 pynanovna-0.0.6/src/pynanovna.egg-info/SOURCES.txt
+-rw-r--r--   0 teo        (501) staff       (20)        1 2024-05-06 16:31:42.000000 pynanovna-0.0.6/src/pynanovna.egg-info/dependency_links.txt
+-rw-r--r--   0 teo        (501) staff       (20)       60 2024-05-06 16:31:42.000000 pynanovna-0.0.6/src/pynanovna.egg-info/requires.txt
+-rw-r--r--   0 teo        (501) staff       (20)       10 2024-05-06 16:31:42.000000 pynanovna-0.0.6/src/pynanovna.egg-info/top_level.txt
```

### Comparing `pynanovna-0.0.5/LICENCE` & `pynanovna-0.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/PKG-INFO` & `pynanovna-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynanovna
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package to use a NanoVNA
 Author-email: Teo Bergkvist <bergkvist.teo@protonmail.com>
 Project-URL: Homepage, https://github.com/PICC-Group/pynanovna
 Project-URL: Issues, https://github.com/PICC-Group/pynanovna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 Install with `pip install pynanovna` or `pip3 install pynanovna`.
 
 ## Example
 ```
 import pynanovna
 
 worker = pynanovna.NanoVNAWorker()
-stream = worker.stream_data(datafile)
+stream = worker.stream_data()
 for sweep in stream:
     print(sweep)
 ```
 
 See `src/pynanovna/example.py` for a more detailed example on some use cases of the project.
```

### Comparing `pynanovna-0.0.5/README.md` & `pynanovna-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Install with `pip install pynanovna` or `pip3 install pynanovna`.
 
 ## Example
 ```
 import pynanovna
 
 worker = pynanovna.NanoVNAWorker()
-stream = worker.stream_data(datafile)
+stream = worker.stream_data()
 for sweep in stream:
     print(sweep)
 ```
 
 See `src/pynanovna/example.py` for a more detailed example on some use cases of the project.
```

### Comparing `pynanovna-0.0.5/pyproject.toml` & `pynanovna-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pynanovna"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name = "Teo Bergkvist", email = "bergkvist.teo@protonmail.com" },
 ]
 description = "A package to use a NanoVNA"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
```

### Comparing `pynanovna-0.0.5/src/pynanovna/Calibration.py` & `pynanovna-0.0.6/src/pynanovna/Calibration.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/src/pynanovna/CalibrationGuide.py` & `pynanovna-0.0.6/src/pynanovna/CalibrationGuide.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/src/pynanovna/RFTools.py` & `pynanovna-0.0.6/src/pynanovna/RFTools.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/src/pynanovna/SITools.py` & `pynanovna-0.0.6/src/pynanovna/SITools.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/src/pynanovna/Sweep.py` & `pynanovna-0.0.6/src/pynanovna/Sweep.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/src/pynanovna/SweepWorker.py` & `pynanovna-0.0.6/src/pynanovna/SweepWorker.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,14 @@
             print("Init data length: ", len(self.data11))
 
     def updateData(self, frequencies, values11, values21, index):
         # Update the data from (i*101) to (i+1)*101
         if self.verbose:
             print(f"Calculating data and inserting in existing data at index {index}")
         offset = self.sweep.points * index
-
         raw_data11 = [
             Datapoint(freq, values11[i][0], values11[i][1])
             for i, freq in enumerate(frequencies)
         ]
         raw_data21 = [
             Datapoint(freq, values21[i][0], values21[i][1])
             for i, freq in enumerate(frequencies)
```

### Comparing `pynanovna-0.0.5/src/pynanovna/Touchstone.py` & `pynanovna-0.0.6/src/pynanovna/Touchstone.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/src/pynanovna/example.py` & `pynanovna-0.0.6/src/pynanovna/example.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/src/pynanovna/hardware/AVNA.py` & `pynanovna-0.0.6/src/pynanovna/hardware/AVNA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/src/pynanovna/hardware/Hardware.py` & `pynanovna-0.0.6/src/pynanovna/hardware/Hardware.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/src/pynanovna/hardware/JNCRadio_VNA_3G.py` & `pynanovna-0.0.6/src/pynanovna/hardware/JNCRadio_VNA_3G.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/src/pynanovna/hardware/NanoVNA.py` & `pynanovna-0.0.6/src/pynanovna/hardware/NanoVNA.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,29 +87,29 @@
         if self.verbose:
             print("readFrequencies: %s", self.sweep_method)
         if self.sweep_method != "scan_mask":
             return super().readFrequencies()
         return [
             int(line)
             for line in self.exec_command(
-                f"scan {self.start} {self.stop} {self.datapoints} 0b001"
+                f"scan {self.start} {self.stop} {self.datapoints} 0b001", wait=0
             )
         ]
 
     def readValues(self, value) -> list[str]:
         if self.sweep_method != "scan_mask":
             return super().readValues(value)
         if self.verbose:
             print("readValue with scan mask (%s)", value)
         # Actually grab the data only when requesting channel 0.
         # The hardware will return all channels which we will store.
         if value == "data 0":
             self._sweepdata = []
             for line in self.exec_command(
-                f"scan {self.start} {self.stop} {self.datapoints} 0b110"
+                f"scan {self.start} {self.stop} {self.datapoints} 0b110", wait=0
             ):
                 data = line.split()
                 self._sweepdata.append((f"{data[0]} {data[1]}", f"{data[2]} {data[3]}"))
         if value == "data 0":
             return [x[0] for x in self._sweepdata]
         if value == "data 1":
             return [x[1] for x in self._sweepdata]
```

### Comparing `pynanovna-0.0.5/src/pynanovna/hardware/NanoVNA_V2.py` & `pynanovna-0.0.6/src/pynanovna/hardware/NanoVNA_V2.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/src/pynanovna/hardware/SV4401A.py` & `pynanovna-0.0.6/src/pynanovna/hardware/SV4401A.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/src/pynanovna/hardware/SV6301A.py` & `pynanovna-0.0.6/src/pynanovna/hardware/SV6301A.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/src/pynanovna/hardware/Serial.py` & `pynanovna-0.0.6/src/pynanovna/hardware/Serial.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/src/pynanovna/hardware/TinySA.py` & `pynanovna-0.0.6/src/pynanovna/hardware/TinySA.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/src/pynanovna/hardware/VNA.py` & `pynanovna-0.0.6/src/pynanovna/hardware/VNA.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         if self.verbose:
             print("result:\n%s", result)
         return result
 
     def readValues(self, value) -> list[str]:
         if self.verbose:
             print("VNA reading %s", value)
-        result = list(self.exec_command(value))
+        result = list(self.exec_command(value, wait=0))
         if self.verbose:
             print("VNA done reading %s (%d values)", value, len(result))
         return result
 
     def readVersion(self) -> "Version":
         result = list(self.exec_command("version"))
         if self.verbose:
```

### Comparing `pynanovna-0.0.5/src/pynanovna/hardware/Version.py` & `pynanovna-0.0.6/src/pynanovna/hardware/Version.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/src/pynanovna/pynanovna.py` & `pynanovna-0.0.6/src/pynanovna/pynanovna.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             self.CalibrationGuide = CalibrationGuide(
                 self.calibration, self.worker, verbose
             )
             if self.verbose:
                 print("VNA is connected: ", self.vna.connected())
                 print("Firmware: ", self.vna.readFirmware())
                 print("Features: ", self.vna.read_features())
+                print("Version", self.vna.name)
 
     def calibrate(self, savefile=None, load_file=False):
         """Run the calibration guide and calibrate the NanoVNA.
 
         Args:
             savefile (path): Path to save the calibration. Defaults to None.
             load_file (bool, optional): Path to existing calibration. Defaults to False.
@@ -69,14 +70,16 @@
             segments (int): Number of segments.
             points (int): Number of points.
         """
         if self.playback_mode:
             print("Cannot set sweep in playback mode. Connect NanoVNA and restart.")
             return
         self.worker.sweep.update(start, stop, segments, points)
+        self.worker.init_data()
+        self.vna.datapoints = points
         if self.verbose:
             print(
                 "Sweep set from "
                 + str(self.worker.sweep.start / 1e9)
                 + "e9"
                 + " to "
                 + str(self.worker.sweep.end / 1e9)
```

### Comparing `pynanovna-0.0.5/src/pynanovna/vis.py` & `pynanovna-0.0.6/src/pynanovna/vis.py`

 * *Files identical despite different names*

### Comparing `pynanovna-0.0.5/src/pynanovna.egg-info/PKG-INFO` & `pynanovna-0.0.6/src/pynanovna.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynanovna
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package to use a NanoVNA
 Author-email: Teo Bergkvist <bergkvist.teo@protonmail.com>
 Project-URL: Homepage, https://github.com/PICC-Group/pynanovna
 Project-URL: Issues, https://github.com/PICC-Group/pynanovna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 Install with `pip install pynanovna` or `pip3 install pynanovna`.
 
 ## Example
 ```
 import pynanovna
 
 worker = pynanovna.NanoVNAWorker()
-stream = worker.stream_data(datafile)
+stream = worker.stream_data()
 for sweep in stream:
     print(sweep)
 ```
 
 See `src/pynanovna/example.py` for a more detailed example on some use cases of the project.
```

### Comparing `pynanovna-0.0.5/src/pynanovna.egg-info/SOURCES.txt` & `pynanovna-0.0.6/src/pynanovna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

