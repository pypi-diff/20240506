# Comparing `tmp/mh_z19-3.1.3.tar.gz` & `tmp/mh_z19-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mh_z19-3.1.3.tar", last modified: Fri Feb 25 01:38:56 2022, max compression
+gzip compressed data, was "dist/mh_z19-3.1.5.tar", last modified: Mon May  6 08:24:40 2024, max compression
```

## Comparing `mh_z19-3.1.3.tar` & `mh_z19-3.1.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-02-25 01:38:56.000000 mh_z19-3.1.3/
--rw-r--r--   0 pi        (1000) pi        (1000)    13265 2022-02-25 01:35:38.000000 mh_z19-3.1.3/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-02-25 01:38:56.000000 mh_z19-3.1.3/mh_z19.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      215 2022-02-25 01:38:42.000000 mh_z19-3.1.3/mh_z19.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       48 2022-02-25 01:38:42.000000 mh_z19-3.1.3/mh_z19.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2022-02-25 01:38:42.000000 mh_z19-3.1.3/mh_z19.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)    15184 2022-02-25 01:38:42.000000 mh_z19-3.1.3/mh_z19.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)        7 2022-02-25 01:38:42.000000 mh_z19-3.1.3/mh_z19.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       79 2022-02-25 01:38:56.000000 mh_z19-3.1.3/setup.cfg
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-02-25 01:38:55.000000 mh_z19-3.1.3/mh_z19/
--rw-r--r--   0 pi        (1000) pi        (1000)     7411 2022-02-25 01:31:58.000000 mh_z19-3.1.3/mh_z19/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4426 2022-01-22 04:06:56.000000 mh_z19-3.1.3/mh_z19/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1052 2022-02-25 01:36:22.000000 mh_z19-3.1.3/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)    15184 2022-02-25 01:38:56.000000 mh_z19-3.1.3/PKG-INFO
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-06 08:24:39.000000 mh_z19-3.1.5/
+-rw-r--r--   0 pi        (1000) pi        (1000)    15325 2024-05-06 08:24:39.000000 mh_z19-3.1.5/PKG-INFO
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-06 08:24:39.000000 mh_z19-3.1.5/mh_z19/
+-rw-r--r--   0 pi        (1000) pi        (1000)     7534 2024-05-06 05:33:49.000000 mh_z19-3.1.5/mh_z19/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4426 2024-05-06 05:33:49.000000 mh_z19-3.1.5/mh_z19/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3009 2024-05-06 05:33:49.000000 mh_z19-3.1.5/mh_z19/pwm.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-06 08:24:39.000000 mh_z19-3.1.5/mh_z19.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)    15325 2024-05-06 08:24:38.000000 mh_z19-3.1.5/mh_z19.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)        7 2024-05-06 08:24:38.000000 mh_z19-3.1.5/mh_z19.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       63 2024-05-06 08:24:38.000000 mh_z19-3.1.5/mh_z19.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-05-06 08:24:38.000000 mh_z19-3.1.5/mh_z19.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      229 2024-05-06 08:24:38.000000 mh_z19-3.1.5/mh_z19.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)    13398 2024-05-06 05:33:49.000000 mh_z19-3.1.5/README.md
+-rw-r--r--   0 pi        (1000) pi        (1000)       79 2024-05-06 08:24:39.000000 mh_z19-3.1.5/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)     1081 2024-05-06 08:24:18.000000 mh_z19-3.1.5/setup.py
```

### Comparing `mh_z19-3.1.3/README.md` & `mh_z19-3.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -172,8 +172,9 @@
 - 3.0.2 2021.03.25 Fix to support RPi4 correctly as [issue#29](https://github.com/UedaTakeyuki/mh-z19/issues/29). Thanks [iperniaf](https://github.com/iperniaf)!
 - 3.0.3 2021.11.08 Fix [issue#35](https://github.com/UedaTakeyuki/mh-z19/issues/35). Thanks [false](https://github.com/false-git)!
 - 3.0.4 2011.11.11 Fix [issue#36](https://github.com/UedaTakeyuki/mh-z19/issues/36). Thanks [David Bock](https://github.com/DavidBock)
 - 3.0.5 2022.01.01 Fix [issue#38](https://github.com/UedaTakeyuki/mh-z19/issues/38). Thanks [kzehnter](https://github.com/kzehnter)!
 - 3.1.0 2022.01.22 add ``--co2valueonly`` option by merging [issue#39](https://github.com/UedaTakeyuki/mh-z19/issues/39) and [issue#40](https://github.com/UedaTakeyuki/mh-z19/issues/40). Thanks [jonesthefox](https://github.com/jonesthefox)!
 - 3.1.1 2022.01.23 remove code clone.
 - 3.1.2 2022.01.31 Fix [issue#41](https://github.com/UedaTakeyuki/mh-z19/issues/41). Thanks [Christopher M. Pierce](https://github.com/electronsandstuff)!
-- 3.1.3 2022.02.25 Fix [issue#43](https://github.com/UedaTakeyuki/mh-z19/issues/43). Thanks [Jannis Möller](https://github.com/jannismoeller)!
+- 3.1.3 2022.02.25 Fix [issue#43](https://github.com/UedaTakeyuki/mh-z19/issues/43). Thanks [Jannis Möller](https://github.com/jannismoeller)!
+- 3.1.5 2024.05.06 FIx [issue#53](https://github.com/UedaTakeyuki/mh-z19/issues/53). Thanks [Tats Shibata](https://github.com/rewse)
```

### Comparing `mh_z19-3.1.3/mh_z19.egg-info/PKG-INFO` & `mh_z19-3.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mh-z19
-Version: 3.1.3
+Name: mh_z19
+Version: 3.1.5
 Summary: mh-z19 CO2 concentration sensor library for All models of Raspberry Pi
 Home-page: https://github.com/UedaTakeyuki/mh-z19
 Author: Takeyuki UEDA
 Author-email: gde00107@nifty.com
 License: MIT
 Description: # mh-z19
         Read CO2 concentration from mh-z19 sensor
@@ -181,13 +181,14 @@
         - 3.0.3 2021.11.08 Fix [issue#35](https://github.com/UedaTakeyuki/mh-z19/issues/35). Thanks [false](https://github.com/false-git)!
         - 3.0.4 2011.11.11 Fix [issue#36](https://github.com/UedaTakeyuki/mh-z19/issues/36). Thanks [David Bock](https://github.com/DavidBock)
         - 3.0.5 2022.01.01 Fix [issue#38](https://github.com/UedaTakeyuki/mh-z19/issues/38). Thanks [kzehnter](https://github.com/kzehnter)!
         - 3.1.0 2022.01.22 add ``--co2valueonly`` option by merging [issue#39](https://github.com/UedaTakeyuki/mh-z19/issues/39) and [issue#40](https://github.com/UedaTakeyuki/mh-z19/issues/40). Thanks [jonesthefox](https://github.com/jonesthefox)!
         - 3.1.1 2022.01.23 remove code clone.
         - 3.1.2 2022.01.31 Fix [issue#41](https://github.com/UedaTakeyuki/mh-z19/issues/41). Thanks [Christopher M. Pierce](https://github.com/electronsandstuff)!
         - 3.1.3 2022.02.25 Fix [issue#43](https://github.com/UedaTakeyuki/mh-z19/issues/43). Thanks [Jannis Möller](https://github.com/jannismoeller)!
+        - 3.1.5 2024.05.06 FIx [issue#53](https://github.com/UedaTakeyuki/mh-z19/issues/53). Thanks [Tats Shibata](https://github.com/rewse)
 Keywords: sensor,IoT,Raspberry Pi,mh-z19,CO2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Topic :: Terminals
 Description-Content-Type: text/markdown
```

### Comparing `mh_z19-3.1.3/mh_z19/__init__.py` & `mh_z19-3.1.5/mh_z19/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 # -*- coding: utf-8 -*-
 # original: https://raw.githubusercontent.com/UedaTakeyuki/slider/master/mh_z19.py
 #
 # © Takeyuki UEDA 2015 -
 
 import serial
-import time
 import subprocess
 import traceback
 import getrpimodel
 import struct
 import platform
 import os.path
 
-import RPi.GPIO as GPIO
+# import RPi.GPIO as GPIO
+import mh_z19.pwm as pwm
 
 # setting
-version = "3.1.3"
+version = "3.1.5"
 pimodel        = getrpimodel.model()
 pimodel_strict = getrpimodel.model_strict()
 retry_count    = 3
 
-# exception
-class GPIO_Edge_Timeout(Exception):
-  pass
-
 if os.path.exists('/dev/serial0'):
   partial_serial_dev = 'serial0'
 elif pimodel == "3 Model B" or pimodel == "4 Model B" or pimodel_strict == "Zero W":
   partial_serial_dev = 'ttyS0'
 else:
   partial_serial_dev = 'ttyAMA0'
   
@@ -211,14 +207,19 @@
   request = b"\xff\x01\x99\x00\x00\x00\x07\xd0\x8F"
   result = ser.write(request)
   ser.close()
   if not serial_console_untouched:
     start_getty()
 
 def read_from_pwm(gpio=12, range=5000):
+#  if pimodel == "5":
+    return pwm.read_from_pwm_with_gpiozero(gpio=12, range=5000)
+#  else:
+#    return pwm.read_from_pwm_with_gpio(gpio=12, range=5000)
+'''
   CYCLE_START_HIGHT_TIME = 2
   TIMEOUT = 2000 # must be larger than PWM cycle time.
 
   GPIO.setmode(GPIO.BCM)
   GPIO.setup(gpio,GPIO.IN)
 
   # wait falling ¯¯|_ to see end of last cycle
@@ -237,14 +238,15 @@
   channel = GPIO.wait_for_edge(gpio, GPIO.FALLING, timeout=TIMEOUT)
   if channel is None:
     raise GPIO_Edge_Timeout("gpio {} edge timeout".format(gpio))
   else:
     falling = time.time() * 1000
 
   return {'co2': int(falling -rising - CYCLE_START_HIGHT_TIME) / 2 *(range/500)}
+'''
 
 def checksum(array):
   if p_ver == '2' and isinstance(array, str):
     array = [ord(c) for c in array]
   csum = sum(array) % 0x100
   if csum == 0:
     return struct.pack('B', 0)
```

### Comparing `mh_z19-3.1.3/mh_z19/__main__.py` & `mh_z19-3.1.5/mh_z19/__main__.py`

 * *Files identical despite different names*

### Comparing `mh_z19-3.1.3/setup.py` & `mh_z19-3.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 else:
   with open("README.md", encoding='utf8') as f:
     long_description = f.read()
 
 setup(
   name = 'mh_z19',
   packages = ['mh_z19'], # this must be the same as the name above
-  version = '3.1.3',
+  version = '3.1.5',
   description = 'mh-z19 CO2 concentration sensor library for All models of Raspberry Pi',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author = 'Takeyuki UEDA',
   author_email = 'gde00107@nifty.com',
   license='MIT',
   url = 'https://github.com/UedaTakeyuki/mh-z19', # use the URL to the github repo
@@ -25,10 +25,12 @@
                  'Topic :: Terminals'
   ],
   install_requires=[
     'getrpimodel',
     'pyserial',
     'requests',
     'argparse',
-    'RPi.GPIO'
+    'RPi.GPIO',
+    'gpiozero',
+    'lgpio'
   ]
 )
```

### Comparing `mh_z19-3.1.3/PKG-INFO` & `mh_z19-3.1.5/mh_z19.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mh_z19
-Version: 3.1.3
+Name: mh-z19
+Version: 3.1.5
 Summary: mh-z19 CO2 concentration sensor library for All models of Raspberry Pi
 Home-page: https://github.com/UedaTakeyuki/mh-z19
 Author: Takeyuki UEDA
 Author-email: gde00107@nifty.com
 License: MIT
 Description: # mh-z19
         Read CO2 concentration from mh-z19 sensor
@@ -181,13 +181,14 @@
         - 3.0.3 2021.11.08 Fix [issue#35](https://github.com/UedaTakeyuki/mh-z19/issues/35). Thanks [false](https://github.com/false-git)!
         - 3.0.4 2011.11.11 Fix [issue#36](https://github.com/UedaTakeyuki/mh-z19/issues/36). Thanks [David Bock](https://github.com/DavidBock)
         - 3.0.5 2022.01.01 Fix [issue#38](https://github.com/UedaTakeyuki/mh-z19/issues/38). Thanks [kzehnter](https://github.com/kzehnter)!
         - 3.1.0 2022.01.22 add ``--co2valueonly`` option by merging [issue#39](https://github.com/UedaTakeyuki/mh-z19/issues/39) and [issue#40](https://github.com/UedaTakeyuki/mh-z19/issues/40). Thanks [jonesthefox](https://github.com/jonesthefox)!
         - 3.1.1 2022.01.23 remove code clone.
         - 3.1.2 2022.01.31 Fix [issue#41](https://github.com/UedaTakeyuki/mh-z19/issues/41). Thanks [Christopher M. Pierce](https://github.com/electronsandstuff)!
         - 3.1.3 2022.02.25 Fix [issue#43](https://github.com/UedaTakeyuki/mh-z19/issues/43). Thanks [Jannis Möller](https://github.com/jannismoeller)!
+        - 3.1.5 2024.05.06 FIx [issue#53](https://github.com/UedaTakeyuki/mh-z19/issues/53). Thanks [Tats Shibata](https://github.com/rewse)
 Keywords: sensor,IoT,Raspberry Pi,mh-z19,CO2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Topic :: Terminals
 Description-Content-Type: text/markdown
```

