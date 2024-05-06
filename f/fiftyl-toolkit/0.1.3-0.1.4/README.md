# Comparing `tmp/fiftyl_toolkit-0.1.3.tar.gz` & `tmp/fiftyl_toolkit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiftyl_toolkit-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fiftyl_toolkit-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fiftyl_toolkit-0.1.3.tar` & `fiftyl_toolkit-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      583 2023-10-23 15:57:30.490862 fiftyl_toolkit-0.1.3/README.md
--rw-r--r--   0        0        0     1289 2024-05-04 11:01:59.636333 fiftyl_toolkit-0.1.3/fiftyl_toolkit/ChannelMaps.py
--rw-r--r--   0        0        0       21 2023-10-23 14:43:57.802838 fiftyl_toolkit-0.1.3/fiftyl_toolkit/__init__.py
--rw-r--r--   0        0        0       28 2023-10-23 14:43:57.849504 fiftyl_toolkit-0.1.3/fiftyl_toolkit/io/__init__.py
--rw-r--r--   0        0        0     5583 2024-05-04 11:11:04.980463 fiftyl_toolkit-0.1.3/fiftyl_toolkit/io/extractor.py
--rw-r--r--   0        0        0      670 2024-05-04 11:12:01.583522 fiftyl_toolkit-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 fiftyl_toolkit-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-10-23 15:57:30.490862 fiftyl_toolkit-0.1.4/README.md
+-rw-r--r--   0        0        0     1289 2024-05-04 11:01:59.636333 fiftyl_toolkit-0.1.4/fiftyl_toolkit/ChannelMaps.py
+-rw-r--r--   0        0        0       21 2023-10-23 14:43:57.802838 fiftyl_toolkit-0.1.4/fiftyl_toolkit/__init__.py
+-rw-r--r--   0        0        0       28 2023-10-23 14:43:57.849504 fiftyl_toolkit-0.1.4/fiftyl_toolkit/io/__init__.py
+-rw-r--r--   0        0        0     5593 2024-05-06 09:24:55.957444 fiftyl_toolkit-0.1.4/fiftyl_toolkit/io/extractor.py
+-rw-r--r--   0        0        0      670 2024-05-06 09:25:20.763952 fiftyl_toolkit-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 fiftyl_toolkit-0.1.4/PKG-INFO
```

### Comparing `fiftyl_toolkit-0.1.3/README.md` & `fiftyl_toolkit-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fiftyl_toolkit-0.1.3/fiftyl_toolkit/ChannelMaps.py` & `fiftyl_toolkit-0.1.4/fiftyl_toolkit/ChannelMaps.py`

 * *Files identical despite different names*

### Comparing `fiftyl_toolkit-0.1.3/fiftyl_toolkit/io/extractor.py` & `fiftyl_toolkit-0.1.4/fiftyl_toolkit/io/extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self.sub_run_id = int(self._filename.split('/')[-1].split('_')[2])
         self.set_channel_map(map_version)
 
     def set_channel_map(self, map_version: int=0) -> None:
         """
         Set the channel map version.
         """
-        self._channel_map = CHANNEL_MAPS[map_version]
+        self._channel_map = np.array(CHANNEL_MAPS[map_version])
         return
 
     def get_run_id(self) -> int:
         """
         Return the run ID integer.
         """
         return self.run_id
```

### Comparing `fiftyl_toolkit-0.1.3/pyproject.toml` & `fiftyl_toolkit-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "fiftyl_toolkit"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
 	{ name = "Alejandro Oranday", email = "alejandro@oran.day" }
 ]
 description = "50L data toolkit"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `fiftyl_toolkit-0.1.3/PKG-INFO` & `fiftyl_toolkit-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyl_toolkit
-Version: 0.1.3
+Version: 0.1.4
 Summary: 50L data toolkit
 Author-email: Alejandro Oranday <alejandro@oran.day>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

