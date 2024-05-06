# Comparing `tmp/fhs-enyaq-data-0.1.3.tar.gz` & `tmp/fhs-enyaq-data-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhs-enyaq-data-0.1.3.tar", last modified: Tue Jun 14 20:50:47 2022, max compression
+gzip compressed data, was "fhs-enyaq-data-0.1.4.tar", last modified: Mon May  6 16:37:22 2024, max compression
```

## Comparing `fhs-enyaq-data-0.1.3.tar` & `fhs-enyaq-data-0.1.4.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-06-14 20:50:47.539127 fhs-enyaq-data-0.1.3/
--rw-r--r--   0 richard   (1000) richard   (1000)      119 2022-06-14 20:49:05.000000 fhs-enyaq-data-0.1.3/.bumpversion.cfg
--rw-r--r--   0 richard   (1000) richard   (1000)      379 2022-05-22 21:20:50.000000 fhs-enyaq-data-0.1.3/.gitignore
--rw-r--r--   0 richard   (1000) richard   (1000)      252 2022-06-14 20:49:38.000000 fhs-enyaq-data-0.1.3/CHANGELOG.md
--rw-r--r--   0 richard   (1000) richard   (1000)       25 2022-05-22 21:20:50.000000 fhs-enyaq-data-0.1.3/MANIFEST.in
--rw-r--r--   0 richard   (1000) richard   (1000)     1712 2022-06-14 20:50:47.535794 fhs-enyaq-data-0.1.3/PKG-INFO
--rw-r--r--   0 richard   (1000) richard   (1000)     1142 2022-06-14 20:47:40.000000 fhs-enyaq-data-0.1.3/README.rst
--rw-r--r--   0 richard   (1000) richard   (1000)     2228 2022-05-22 21:20:50.000000 fhs-enyaq-data-0.1.3/justfile
--rw-r--r--   0 richard   (1000) richard   (1000)       16 2022-05-22 21:20:50.000000 fhs-enyaq-data-0.1.3/requirements-dev.txt
--rw-r--r--   0 richard   (1000) richard   (1000)      174 2022-05-22 21:20:50.000000 fhs-enyaq-data-0.1.3/requirements-flake8.txt
--rw-r--r--   0 richard   (1000) richard   (1000)       70 2022-06-13 21:22:09.000000 fhs-enyaq-data-0.1.3/requirements.txt
--rw-r--r--   0 richard   (1000) richard   (1000)       38 2022-06-14 20:50:47.539127 fhs-enyaq-data-0.1.3/setup.cfg
--rw-r--r--   0 richard   (1000) richard   (1000)     1595 2022-05-29 20:00:01.000000 fhs-enyaq-data-0.1.3/setup.py
-drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-06-14 20:50:47.525794 fhs-enyaq-data-0.1.3/src/
-drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-06-14 20:50:47.532461 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/
--rw-r--r--   0 richard   (1000) richard   (1000)       66 2022-05-22 21:20:50.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/__init__.py
--rw-r--r--   0 richard   (1000) richard   (1000)      278 2022-06-14 20:49:05.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/__version__.py
-drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-06-14 20:50:47.535794 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/abrp/
--rw-r--r--   0 richard   (1000) richard   (1000)        0 2022-06-02 18:26:47.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/abrp/__init__.py
--rw-r--r--   0 richard   (1000) richard   (1000)     2310 2022-06-03 21:57:59.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/abrp/abrp_class.py
--rw-r--r--   0 richard   (1000) richard   (1000)      411 2022-06-03 21:47:25.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/abrp_list_cars.py
--rw-r--r--   0 richard   (1000) richard   (1000)      372 2022-06-03 22:02:51.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/abrp_send.py
--rw-r--r--   0 richard   (1000) richard   (1000)     1502 2022-06-03 21:51:31.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/cli.py
--rw-r--r--   0 richard   (1000) richard   (1000)      993 2022-06-02 21:20:09.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/config.py
--rw-r--r--   0 richard   (1000) richard   (1000)     1563 2022-06-03 13:14:04.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/fhs_enyaq_data.py
--rw-r--r--   0 richard   (1000) richard   (1000)     2085 2022-06-14 20:41:04.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/loop.py
--rw-r--r--   0 richard   (1000) richard   (1000)     1773 2022-06-14 20:48:14.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/mqtt.py
--rw-r--r--   0 richard   (1000) richard   (1000)      382 2022-06-03 16:24:08.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/output.py
-drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-06-14 20:50:47.535794 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/skoda_class/
--rw-r--r--   0 richard   (1000) richard   (1000)        9 2022-05-22 21:29:11.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/skoda_class/__init__.py
--rw-r--r--   0 richard   (1000) richard   (1000)     4856 2022-06-02 21:46:10.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/skoda_class/skoda_class.py
-drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-06-14 20:50:47.535794 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data.egg-info/
--rw-r--r--   0 richard   (1000) richard   (1000)     1712 2022-06-14 20:50:47.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data.egg-info/PKG-INFO
--rw-r--r--   0 richard   (1000) richard   (1000)      919 2022-06-14 20:50:47.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data.egg-info/SOURCES.txt
--rw-r--r--   0 richard   (1000) richard   (1000)        1 2022-06-14 20:50:47.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data.egg-info/dependency_links.txt
--rw-r--r--   0 richard   (1000) richard   (1000)       60 2022-06-14 20:50:47.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data.egg-info/entry_points.txt
--rw-r--r--   0 richard   (1000) richard   (1000)       70 2022-06-14 20:50:47.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data.egg-info/requires.txt
--rw-r--r--   0 richard   (1000) richard   (1000)       15 2022-06-14 20:50:47.000000 fhs-enyaq-data-0.1.3/src/fhs_enyaq_data.egg-info/top_level.txt
--rw-r--r--   0 richard   (1000) richard   (1000)      152 2022-05-22 21:20:50.000000 fhs-enyaq-data-0.1.3/template-version.txt
-drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2022-06-14 20:50:47.535794 fhs-enyaq-data-0.1.3/tests/
--rw-r--r--   0 richard   (1000) richard   (1000)       98 2022-05-22 21:20:50.000000 fhs-enyaq-data-0.1.3/tests/test_sample.py
--rw-r--r--   0 richard   (1000) richard   (1000)      599 2022-06-03 13:26:50.000000 fhs-enyaq-data-0.1.3/tox.ini
+drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2024-05-06 16:37:22.197794 fhs-enyaq-data-0.1.4/
+-rw-r--r--   0 richard   (1000) richard   (1000)      119 2024-05-05 19:20:36.000000 fhs-enyaq-data-0.1.4/.bumpversion.cfg
+-rw-r--r--   0 richard   (1000) richard   (1000)      379 2024-05-05 19:20:14.000000 fhs-enyaq-data-0.1.4/.dockerignore
+-rw-r--r--   0 richard   (1000) richard   (1000)      379 2022-05-22 21:20:50.000000 fhs-enyaq-data-0.1.4/.gitignore
+-rw-r--r--   0 richard   (1000) richard   (1000)      273 2024-05-05 19:21:16.000000 fhs-enyaq-data-0.1.4/CHANGELOG.md
+-rw-r--r--   0 richard   (1000) richard   (1000)       25 2022-05-22 21:20:50.000000 fhs-enyaq-data-0.1.4/MANIFEST.in
+-rw-r--r--   0 richard   (1000) richard   (1000)     1882 2024-05-06 16:37:22.197794 fhs-enyaq-data-0.1.4/PKG-INFO
+-rw-r--r--   0 richard   (1000) richard   (1000)     1142 2022-06-14 20:47:40.000000 fhs-enyaq-data-0.1.4/README.rst
+-rw-r--r--   0 richard   (1000) richard   (1000)     2228 2022-05-22 21:20:50.000000 fhs-enyaq-data-0.1.4/justfile
+-rw-r--r--   0 richard   (1000) richard   (1000)       16 2022-05-22 21:20:50.000000 fhs-enyaq-data-0.1.4/requirements-dev.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)      174 2022-05-22 21:20:50.000000 fhs-enyaq-data-0.1.4/requirements-flake8.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)       70 2022-06-13 21:22:09.000000 fhs-enyaq-data-0.1.4/requirements.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)       38 2024-05-06 16:37:22.197794 fhs-enyaq-data-0.1.4/setup.cfg
+-rw-r--r--   0 richard   (1000) richard   (1000)     1595 2022-05-29 20:00:01.000000 fhs-enyaq-data-0.1.4/setup.py
+drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2024-05-06 16:37:22.191127 fhs-enyaq-data-0.1.4/src/
+drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2024-05-06 16:37:22.194460 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/
+-rw-r--r--   0 richard   (1000) richard   (1000)       66 2022-05-22 21:20:50.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/__init__.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      278 2024-05-05 19:20:36.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/__version__.py
+drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2024-05-06 16:37:22.197794 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/abrp/
+-rw-r--r--   0 richard   (1000) richard   (1000)        0 2022-06-02 18:26:47.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/abrp/__init__.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     2309 2024-05-06 16:22:14.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/abrp/abrp_class.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      411 2022-06-03 21:47:25.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/abrp_list_cars.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      484 2024-05-06 16:23:55.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/abrp_send.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     1502 2022-06-03 21:51:31.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/cli.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      993 2022-06-02 21:20:09.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/config.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     1578 2024-05-06 15:46:12.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/fhs_enyaq_data.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     2300 2024-05-06 16:28:13.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/loop.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     1773 2024-05-06 15:45:34.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/mqtt.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      382 2022-06-03 16:24:08.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/output.py
+drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2024-05-06 16:37:22.197794 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/skoda_class/
+-rw-r--r--   0 richard   (1000) richard   (1000)        9 2022-05-22 21:29:11.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/skoda_class/__init__.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     5695 2024-05-06 16:25:56.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/skoda_class/skoda_class.py
+drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2024-05-06 16:37:22.197794 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data.egg-info/
+-rw-r--r--   0 richard   (1000) richard   (1000)     1882 2024-05-06 16:37:22.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data.egg-info/PKG-INFO
+-rw-r--r--   0 richard   (1000) richard   (1000)      933 2024-05-06 16:37:22.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data.egg-info/SOURCES.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)        1 2024-05-06 16:37:22.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data.egg-info/dependency_links.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)       59 2024-05-06 16:37:22.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data.egg-info/entry_points.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)       70 2024-05-06 16:37:22.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data.egg-info/requires.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)       15 2024-05-06 16:37:22.000000 fhs-enyaq-data-0.1.4/src/fhs_enyaq_data.egg-info/top_level.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)      152 2022-05-22 21:20:50.000000 fhs-enyaq-data-0.1.4/template-version.txt
+drwxr-xr-x   0 richard   (1000) richard   (1000)        0 2024-05-06 16:37:22.197794 fhs-enyaq-data-0.1.4/tests/
+-rw-r--r--   0 richard   (1000) richard   (1000)       98 2022-05-22 21:20:50.000000 fhs-enyaq-data-0.1.4/tests/test_sample.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      599 2022-06-03 13:26:50.000000 fhs-enyaq-data-0.1.4/tox.ini
```

### Comparing `fhs-enyaq-data-0.1.3/PKG-INFO` & `fhs-enyaq-data-0.1.4/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: fhs-enyaq-data
-Version: 0.1.3
-Summary: enyaq car data
-Home-page: https://github.com/foxhunt72/fhs-enyaq-data
-Author: Richard de Vos
-Author-email: rdevos72@gmail.com
-License: MIT license
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-
 fhs_enyaq_data
 ==============
 
 
 enyaq car data to external services for now
 abrp
 
@@ -83,9 +66,7 @@
 -------
 MIT
 
 Authors
 -------
 
 `fhs_enyaq_data` was written by `Richard de Vos <rdevos72@gmail.com>`_.
-
-
```

### Comparing `fhs-enyaq-data-0.1.3/justfile` & `fhs-enyaq-data-0.1.4/justfile`

 * *Files identical despite different names*

### Comparing `fhs-enyaq-data-0.1.3/setup.py` & `fhs-enyaq-data-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/abrp/abrp_class.py` & `fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/abrp/abrp_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #      "Skoda;ENYAQ iV;80 (alpha)": "skoda:enyaq:21:77:meb"
 #      "Skoda;ENYAQ iV;80x (alpha)": "skoda:enyaq:21:77:meb:x"
 #      "Skoda;ENYAQ iV;RS (alpha)": "skoda:enyaq:21:77:meb:rs"
 #      "Skoda;ENYAQ iV;portline (alpha)": "skoda:enyaq:21:77:meb:sportline"
 
 
 class abrp_class:
-    def __init__(self, token, api_key='c626070c-1c8d-4003-bc76-6de223b44679', url='https://api.iternio.com/1/', car_type='skoda:enyaq:21:77:meb', debug_output=None):
+    def __init__(self, token, api_key='c626070c-1c8d-4003-bc76-6de223b44679', url='https://api.iternio.com/1', car_type='skoda:enyaq:21:77:meb', debug_output=None):
         self.token = token
         self.api_key = api_key
         self.url = url
         self.car_type = car_type
         self.debug_output = debug_output
         self.fail_output = print
 
@@ -31,15 +31,15 @@
     def create_data(self, input_data):
         output_data = {}
         output_data['utc'] = int(time.time())
         output_data['soc'] = input_data['Battery level'] 
         output_data['car_model'] = self.car_type
         output_data['is_charging'] = input_data['Charging']
         output_data['est_battery_range'] = input_data['Electric range']
-        output_data['power'] = int(input_data['Charging power'] / -1000)
+        output_data['power'] = int(input_data['Charging Power'] / -1000)
         self.debug(str(output_data))
         return output_data
 
     def send(self, output_data):
         try:
             headers = {"Authorization": f"APIKEY {self.api_key}"}
             data = {"tlm": output_data}
```

### Comparing `fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/cli.py` & `fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/cli.py`

 * *Files identical despite different names*

### Comparing `fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/config.py` & `fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/config.py`

 * *Files identical despite different names*

### Comparing `fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/fhs_enyaq_data.py` & `fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/fhs_enyaq_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Main module."""
 
 from fhs_enyaq_data.skoda_class.skoda_class import skoda_class
 import signal
 
 def main(config):
     """ Skoda. """
-    skoda = skoda_class(config=config['skoda'])
+    skoda = skoda_class(config=config['skoda'], verbose=False)
     skoda.list_cars()
 
 
 def get_vehicle_data(config):
     if 'vehicle_vin' not in config['skoda'] or config['skoda']['vehicle_vin'] == '':
         vehicle_vin = None
     else:
```

### Comparing `fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/loop.py` & `fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/loop.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,19 @@
         mqtt = None
 
     while True:
         # run
         output('get instruments information from skoda connect.')
         instruments = get_instruments_with_timeout(config)
         if instruments is not None:
+            # pprint(instruments)
+            if 'Battery level' not in instruments:
+                output('no battery level returned, sleeping 30 seconds.')
+                time.sleep(30)
+                continue
             output(f"battery level: {instruments['Battery level']}   charging: {instruments['Charging']}")
             send_abrp(config, instruments, output=output)
             if mqtt is not None:
                 mqtt_publish_instruments(mqtt, config['mqtt']['topic'], instruments)
                 #pprint(instruments)
             sleep_time = idle_wait * 60
             if last_km is None:
```

### Comparing `fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/mqtt.py` & `fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/mqtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,14 @@
 def mqtt_publish(client, topic, value):
     result = client.publish(topic, value)
 
 
 def mqtt_publish_instruments(client, topic, instruments):
     mqtt_publish(client, f"{topic}/battery_level", instruments['Battery level'])
     mqtt_publish(client, f"{topic}/charging", instruments['Charging'])
-    mqtt_publish(client, f"{topic}/charging_power", instruments['Charging power'])
+    mqtt_publish(client, f"{topic}/charging_power", instruments['Charging Power'])
     mqtt_publish(client, f"{topic}/charging_rate", instruments['Charging rate'])
     mqtt_publish(client, f"{topic}/climatisation_target_temperature", instruments['Climatisation target temperature'])
     mqtt_publish(client, f"{topic}/electric_range", instruments['Electric range'])
     mqtt_publish(client, f"{topic}/minimum_charge_level", instruments['Minimum charge level'])
```

### Comparing `fhs-enyaq-data-0.1.3/src/fhs_enyaq_data/skoda_class/skoda_class.py` & `fhs-enyaq-data-0.1.4/src/fhs_enyaq_data/skoda_class/skoda_class.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python3
-from pprint import pprint
 import asyncio
 import inspect
 import time
 import sys
 import os
 import yaml
 from aiohttp import ClientSession
@@ -37,35 +36,41 @@
             with open(self.config_file, "r") as file:
                 self.state = yaml.load(file, Loader=yaml.FullLoader)
         except Exception as e:
             print(f"can't open config file: {self.config_file}  {e}")
 
     async def login_and_get_vehicles(self):
         """Main method."""
+        if self.state.get("verbose"):
+            print("function: login_and_get_vehicles")
         session = ClientSession(headers={"Connection": "keep-alive"})
         if self.state.get("verbose"):
             print(
                 f"Initiating new session to Skoda Connect with {self.state['username']} as username"
             )
         connection = Connection(
             session, self.state["username"], self.state["password"], False
         )
+        self.conn = connection
         if self.state.get("verbose"):
             print("Attempting to login to the Skoda Connect service")
             print(datetime.now())
         if await connection.doLogin():
             if self.state.get("verbose"):
                 print("Login success!")
                 print(datetime.now())
                 print("Fetching vehicles associated with account.")
             await connection.get_vehicles()
+            await connection.update_all()
             return (session, connection.vehicles)
         return (session, None)
 
     async def async_get_vehicle(self, vehicle_vin):
+        if self.state.get("verbose"):
+            print("function: async_get_vehicle")
         (session, vehicles) = await self.login_and_get_vehicles()
         if vehicles == None:
             print("no vehicle found to set temp.")
             await session.close()
             return (None, None)
         if vehicle_vin == None:
             if len(vehicles) > 1:
@@ -77,27 +82,31 @@
             if vehicle_vin == vehicle.vin:
                 return (session, vehicle)
         await session.close()
         return (None, None)
 
     async def async_get_instruments(self, vehicle_vin):
         """Async airco."""
+        if self.state.get("verbose"):
+            print("function: async_get_instruments")
         (session, vehicle) = await self.async_get_vehicle(vehicle_vin)
         if vehicle == None:
             print("no vehicle found.")
             await session.close()
             return None
         dashboard = vehicle.dashboard()
         instruments = dashboard.instruments
         await session.close()
         return instruments
 
 
     async def async_print_instruments(self, vehicle_vin):
         # Battery level
+        if self.state.get("verbose"):
+            print("function: aync_print_instruments")
         instruments = await self.async_get_instruments(vehicle_vin)
         if instruments == None:
             print('no instruments')
         for i in instruments:
             print(f"{i.name} = {i.state}")
         return None
 
@@ -105,45 +114,55 @@
         return self.loop.run_until_complete(
             self.async_print_instruments(vehicle_vin)
         )
 
 
     async def async_get_battery_level(self, vehicle_vin):
         # Battery level
+        if self.state.get("verbose"):
+            print("function: async_get_battery_level")
         instruments = await self.async_get_instruments(vehicle_vin)
         if instruments == None:
             return None
         for i in instruments:
             if i.name == "Battery level":
                 return int(i.state)
         return None
 
 
     def get_battery_level(self, vehicle_vin=None):
+        if self.state.get("verbose"):
+            print("function: get_battery_level")
         return self.loop.run_until_complete(
             self.async_get_battery_level(vehicle_vin)
         )
 
     def get_instruments(self, vehicle_vin=None):
+        if self.state.get("verbose"):
+            print("function: get_instruments")
         result = self.loop.run_until_complete(
             self.async_get_instruments(vehicle_vin)
         )
         instruments={}
         for i in result:
             instruments[i.name] = i.state
         return instruments
 
     async def async_list_cars(self):
         """Async airco."""
+        if self.state.get("verbose"):
+            print("function: async_list_cars")
         (session, vehicles) = await self.login_and_get_vehicles()
         if vehicles == None:
             print("no vehicle found.")
             await session.close()
             return False
         for vehicle in vehicles:
             print(f"VIN: {vehicle.vin}\t: {vehicle.model}")
         await session.close()
 
 
     def list_cars(self):
+        if self.state.get("verbose"):
+            print("function: list_cars") 
         print(f"listing cars")
         return self.loop.run_until_complete(self.async_list_cars())
```

### Comparing `fhs-enyaq-data-0.1.3/src/fhs_enyaq_data.egg-info/PKG-INFO` & `fhs-enyaq-data-0.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 Metadata-Version: 2.1
 Name: fhs-enyaq-data
-Version: 0.1.3
+Version: 0.1.4
 Summary: enyaq car data
 Home-page: https://github.com/foxhunt72/fhs-enyaq-data
 Author: Richard de Vos
 Author-email: rdevos72@gmail.com
 License: MIT license
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: skodaconnect
+Requires-Dist: typer[all]
+Requires-Dist: pyyaml
+Requires-Dist: appdirs
+Requires-Dist: requests
+Requires-Dist: pyyaml
+Requires-Dist: rich
+Requires-Dist: paho-mqtt
 
 fhs_enyaq_data
 ==============
 
 
 enyaq car data to external services for now
 abrp
@@ -83,9 +90,7 @@
 -------
 MIT
 
 Authors
 -------
 
 `fhs_enyaq_data` was written by `Richard de Vos <rdevos72@gmail.com>`_.
-
-
```

### Comparing `fhs-enyaq-data-0.1.3/src/fhs_enyaq_data.egg-info/SOURCES.txt` & `fhs-enyaq-data-0.1.4/src/fhs_enyaq_data.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .bumpversion.cfg
+.dockerignore
 .gitignore
 CHANGELOG.md
 MANIFEST.in
 README.rst
 justfile
 requirements-dev.txt
 requirements-flake8.txt
```

### Comparing `fhs-enyaq-data-0.1.3/tox.ini` & `fhs-enyaq-data-0.1.4/tox.ini`

 * *Files identical despite different names*

