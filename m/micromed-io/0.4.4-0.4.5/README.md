# Comparing `tmp/micromed_io-0.4.4.tar.gz` & `tmp/micromed_io-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micromed_io-0.4.4.tar", max compression
+gzip compressed data, was "micromed_io-0.4.5.tar", max compression
```

## Comparing `micromed_io-0.4.4.tar` & `micromed_io-0.4.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1534 2024-02-08 14:48:10.197272 micromed_io-0.4.4/LICENSE
--rw-r--r--   0        0        0       52 2024-05-02 07:42:39.386572 micromed_io-0.4.4/micromed_io/__init__.py
--rw-r--r--   0        0        0     3846 2024-02-08 14:48:13.835447 micromed_io-0.4.4/micromed_io/header.py
--rw-r--r--   0        0        0    24404 2024-05-02 07:31:49.684032 micromed_io-0.4.4/micromed_io/in_out.py
--rw-r--r--   0        0        0     8164 2024-02-08 14:48:13.836441 micromed_io-0.4.4/micromed_io/scripts/emulate_online_trc.py
--rw-r--r--   0        0        0     1453 2024-02-08 14:48:13.836441 micromed_io-0.4.4/micromed_io/scripts/rename_trc.py
--rw-r--r--   0        0        0    12576 2024-02-08 14:48:13.836441 micromed_io-0.4.4/micromed_io/scripts/tcp_to_lsl.py
--rw-r--r--   0        0        0     3650 2024-02-08 14:48:13.836441 micromed_io-0.4.4/micromed_io/tcp.py
--rw-r--r--   0        0        0     4070 2024-02-08 14:48:13.836441 micromed_io-0.4.4/micromed_io/to_mne.py
--rw-r--r--   0        0        0     3267 2024-02-08 14:48:13.837441 micromed_io-0.4.4/micromed_io/trc.py
--rw-r--r--   0        0        0      864 2024-05-02 07:42:33.597836 micromed_io-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     4911 2024-04-10 10:45:33.365380 micromed_io-0.4.4/README.rst
--rw-r--r--   0        0        0     5377 1970-01-01 00:00:00.000000 micromed_io-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1534 2024-02-08 14:48:10.197272 micromed_io-0.4.5/LICENSE
+-rw-r--r--   0        0        0       52 2024-05-06 14:57:45.038044 micromed_io-0.4.5/micromed_io/__init__.py
+-rw-r--r--   0        0        0     3846 2024-02-08 14:48:13.835447 micromed_io-0.4.5/micromed_io/header.py
+-rw-r--r--   0        0        0    24404 2024-05-02 07:31:49.684032 micromed_io-0.4.5/micromed_io/in_out.py
+-rw-r--r--   0        0        0     8164 2024-02-08 14:48:13.836441 micromed_io-0.4.5/micromed_io/scripts/emulate_online_trc.py
+-rw-r--r--   0        0        0     1453 2024-02-08 14:48:13.836441 micromed_io-0.4.5/micromed_io/scripts/rename_trc.py
+-rw-r--r--   0        0        0    12576 2024-02-08 14:48:13.836441 micromed_io-0.4.5/micromed_io/scripts/tcp_to_lsl.py
+-rw-r--r--   0        0        0     3650 2024-02-08 14:48:13.836441 micromed_io-0.4.5/micromed_io/tcp.py
+-rw-r--r--   0        0        0     4128 2024-05-06 14:55:35.381623 micromed_io-0.4.5/micromed_io/to_mne.py
+-rw-r--r--   0        0        0     3267 2024-02-08 14:48:13.837441 micromed_io-0.4.5/micromed_io/trc.py
+-rw-r--r--   0        0        0      864 2024-05-06 14:57:57.507584 micromed_io-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     4911 2024-04-10 10:45:33.365380 micromed_io-0.4.5/README.rst
+-rw-r--r--   0        0        0     5377 1970-01-01 00:00:00.000000 micromed_io-0.4.5/PKG-INFO
```

### Comparing `micromed_io-0.4.4/LICENSE` & `micromed_io-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `micromed_io-0.4.4/micromed_io/header.py` & `micromed_io-0.4.5/micromed_io/header.py`

 * *Files identical despite different names*

### Comparing `micromed_io-0.4.4/micromed_io/in_out.py` & `micromed_io-0.4.5/micromed_io/in_out.py`

 * *Files identical despite different names*

### Comparing `micromed_io-0.4.4/micromed_io/scripts/emulate_online_trc.py` & `micromed_io-0.4.5/micromed_io/scripts/emulate_online_trc.py`

 * *Files identical despite different names*

### Comparing `micromed_io-0.4.4/micromed_io/scripts/rename_trc.py` & `micromed_io-0.4.5/micromed_io/scripts/rename_trc.py`

 * *Files identical despite different names*

### Comparing `micromed_io-0.4.4/micromed_io/scripts/tcp_to_lsl.py` & `micromed_io-0.4.5/micromed_io/scripts/tcp_to_lsl.py`

 * *Files identical despite different names*

### Comparing `micromed_io-0.4.4/micromed_io/tcp.py` & `micromed_io-0.4.5/micromed_io/tcp.py`

 * *Files identical despite different names*

### Comparing `micromed_io-0.4.4/micromed_io/to_mne.py` & `micromed_io-0.4.5/micromed_io/to_mne.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Micromed module to load and transform data from Micromed recordings to mne format"""
+
 from datetime import timedelta, timezone
 from pathlib import Path
 from typing import List, Union
 
 import mne
 import numpy as np
 
@@ -39,20 +40,22 @@
     Returns
     -------
     mne.io.RawArray
         A mne Raw instance containing the requested channels.
 
     Notes
     -----
+    Data is returned in volts.
+
     Some info are hardcoded, such as:
 
     - `device_info` type: Micromed
     - `device_info` site: Unknown
 
-    Update the code if needed.
+    Please update the code if needed.
 
     Examples
     --------
     >>> from micromed_io.to_mne import create_mne_from_micromed_recording
     >>> mne_raw = create_mne_from_micromed_recording("path/to/file.TRC", start_time=10.0, stop_time=20.0) #doctest: +SKIP
 
     """
@@ -60,15 +63,15 @@
 
     if sub_channels is None:
         sub_channels = micromed_trc.micromed_header.ch_names
     sfreq = micromed_trc.get_sfreq()
     start_sample = int(start_time * sfreq)
     stop_sample = int(stop_time * sfreq) if stop_time is not None else None
     sub_eegs = micromed_trc.get_data(
-        picks=sub_channels, start=start_sample, stop=stop_sample
+        picks=sub_channels, start=start_sample, stop=stop_sample, use_volt=True
     )
 
     info = mne.create_info(
         ch_names=sub_channels,
         sfreq=micromed_trc.sfreq,
         ch_types=ch_types,
     )
```

### Comparing `micromed_io-0.4.4/micromed_io/trc.py` & `micromed_io-0.4.5/micromed_io/trc.py`

 * *Files identical despite different names*

### Comparing `micromed_io-0.4.4/pyproject.toml` & `micromed_io-0.4.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micromed-io"
-version = "0.4.4"
+version = "0.4.5"
 description = "A library to read, emulate, and forward Micromed data in standard formats"
 authors = ["Etienne de MONTALIVET <etienne.demontalivet@protonmail.com>"]
 readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 mne = "^1.0.0"
```

### Comparing `micromed_io-0.4.4/README.rst` & `micromed_io-0.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `micromed_io-0.4.4/PKG-INFO` & `micromed_io-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micromed-io
-Version: 0.4.4
+Version: 0.4.5
 Summary: A library to read, emulate, and forward Micromed data in standard formats
 Author: Etienne de MONTALIVET
 Author-email: etienne.demontalivet@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

