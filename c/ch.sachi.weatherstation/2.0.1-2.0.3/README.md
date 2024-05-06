# Comparing `tmp/ch_sachi_weatherstation-2.0.1.tar.gz` & `tmp/ch_sachi_weatherstation-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ch_sachi_weatherstation-2.0.1.tar", max compression
+gzip compressed data, was "ch_sachi_weatherstation-2.0.3.tar", max compression
```

## Comparing `ch_sachi_weatherstation-2.0.1.tar` & `ch_sachi_weatherstation-2.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1068 2024-02-02 15:23:51.241839 ch_sachi_weatherstation-2.0.1/LICENSE
--rw-r--r--   0        0        0      245 2024-02-02 15:23:51.241839 ch_sachi_weatherstation-2.0.1/README.md
--rw-r--r--   0        0        0        0 2024-02-02 15:23:51.241839 ch_sachi_weatherstation-2.0.1/ch/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 15:23:51.241839 ch_sachi_weatherstation-2.0.1/ch/sachi/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 15:23:51.241839 ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/__init__.py
--rw-r--r--   0        0        0     2706 2024-02-02 15:23:51.241839 ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/config.py
--rw-r--r--   0        0        0      280 2024-02-02 15:23:51.241839 ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/domain.py
--rw-r--r--   0        0        0      314 2024-02-02 15:23:51.241839 ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/logging.py
--rw-r--r--   0        0        0     4307 2024-02-02 15:23:51.241839 ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/measureRepository.py
--rw-r--r--   0        0        0     1730 2024-02-02 15:23:51.245839 ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/publishMeasures.py
--rw-r--r--   0        0        0     3253 2024-02-02 15:23:51.245839 ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/publishPictures.py
--rw-r--r--   0        0        0     2609 2024-02-02 15:23:51.245839 ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/restServiceMeasures.py
--rw-r--r--   0        0        0     4879 2024-02-02 15:23:51.245839 ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/restServicePictures.py
--rw-r--r--   0        0        0      980 2024-02-02 15:23:51.245839 ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/saveMeasures.py
--rw-r--r--   0        0        0     1645 2024-02-02 15:23:51.245839 ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/sensorService.py
--rw-r--r--   0        0        0      878 2024-02-02 15:24:46.697416 ch_sachi_weatherstation-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 ch_sachi_weatherstation-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-06 11:57:02.838692 ch_sachi_weatherstation-2.0.3/LICENSE
+-rw-r--r--   0        0        0      245 2024-05-06 11:57:02.838692 ch_sachi_weatherstation-2.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:57:02.838692 ch_sachi_weatherstation-2.0.3/ch/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:57:02.838692 ch_sachi_weatherstation-2.0.3/ch/sachi/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:57:02.838692 ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/__init__.py
+-rw-r--r--   0        0        0     2706 2024-05-06 11:57:02.838692 ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/config.py
+-rw-r--r--   0        0        0      540 2024-05-06 11:57:02.838692 ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/domain.py
+-rw-r--r--   0        0        0      314 2024-05-06 11:57:02.842692 ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/logging.py
+-rw-r--r--   0        0        0     4307 2024-05-06 11:57:02.842692 ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/measureRepository.py
+-rw-r--r--   0        0        0     1929 2024-05-06 11:57:02.842692 ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/publishMeasures.py
+-rw-r--r--   0        0        0     3253 2024-05-06 11:57:02.842692 ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/publishPictures.py
+-rw-r--r--   0        0        0     2546 2024-05-06 11:57:02.842692 ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/restServiceMeasures.py
+-rw-r--r--   0        0        0     4879 2024-05-06 11:57:02.842692 ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/restServicePictures.py
+-rw-r--r--   0        0        0      980 2024-05-06 11:57:02.842692 ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/saveMeasures.py
+-rw-r--r--   0        0        0     1645 2024-05-06 11:57:02.842692 ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/sensorService.py
+-rw-r--r--   0        0        0      878 2024-05-06 11:58:56.335397 ch_sachi_weatherstation-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 ch_sachi_weatherstation-2.0.3/PKG-INFO
```

### Comparing `ch_sachi_weatherstation-2.0.1/LICENSE` & `ch_sachi_weatherstation-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/config.py` & `ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/config.py`

 * *Files identical despite different names*

### Comparing `ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/measureRepository.py` & `ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/measureRepository.py`

 * *Files identical despite different names*

### Comparing `ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/publishMeasures.py` & `ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/publishMeasures.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,19 @@
                 sensor_id = sensor['id']
                 sensor_name = sensor['name']
                 last = self.service.get_last_timestamp(sensor_id)
                 measures_to_post = self.repo.get_measures_after(sensor_name, last)
                 measures_per_sensor = len(measures_to_post)
                 if len(measures_to_post) > 0:
                     logging.info('Posting ' + str(measures_per_sensor) + " for sensor '" + sensor['name'] + "'")
-                    self.service.post_measures(sensor_id, measures_to_post)
-                    posted_measures += measures_per_sensor
+                    try:
+                        self.service.post_measures(sensor_id, measures_to_post)
+                        posted_measures += measures_per_sensor
+                    except Exception as postEx:
+                        logging.error("Error occurred when posting measures for " + sensor_name + ": " + str(postEx))
             elapsed_time = datetime.datetime.now() - start
             logging.info('Posted ' + str(posted_measures) + ' in ' + str(elapsed_time))
         except Exception as e:
             logging.error("Error occurred: " + str(e))
 
 
 def main():
```

### Comparing `ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/publishPictures.py` & `ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/publishPictures.py`

 * *Files identical despite different names*

### Comparing `ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/restServiceMeasures.py` & `ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/restServiceMeasures.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 import logging
 import sys
-from typing import Any
+from typing import Any, List
 
 import requests
 
+from ch.sachi.weatherstation.domain import Measure
+
 
 class RestServiceMeasures:
     def __init__(self, url: str, username: str, password: str):
         self.url = url
         self.auth = {'username': username, 'password': password}
         self.headers = {'User-Agent': 'python'}
         self.login()
@@ -49,19 +51,18 @@
             if str_response:
                 last = json.loads(str_response)
                 return last['measured_at']
             return '1970-01-01 00:00'
         else:
             response.raise_for_status()
 
-    def post_measures(self, sensor_id, measures) -> None:
+    def post_measures(self, sensor_id, measures: List[Measure]) -> None:
         measures_data = []
         for measure in measures:
-            data = {'sensor': sensor_id, 'measured_at': measure['measured_at'], 'temperature': measure['temperature'],
-                    'humidity': measure['humidity']}
+            data = measure.toJson()
             measures_data.append(data)
         logging.debug('Headers:')
         logging.debug(self.headers)
         response = requests.post(self.url + '/measures', data=json.dumps(measures_data), headers=self.headers,
                                  timeout=120)
         logging.debug(response)
         if not response.ok:
```

### Comparing `ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/restServicePictures.py` & `ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/restServicePictures.py`

 * *Files identical despite different names*

### Comparing `ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/saveMeasures.py` & `ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/saveMeasures.py`

 * *Files identical despite different names*

### Comparing `ch_sachi_weatherstation-2.0.1/ch/sachi/weatherstation/sensorService.py` & `ch_sachi_weatherstation-2.0.3/ch/sachi/weatherstation/sensorService.py`

 * *Files identical despite different names*

### Comparing `ch_sachi_weatherstation-2.0.1/pyproject.toml` & `ch_sachi_weatherstation-2.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ch.sachi.weatherstation"
-version = "2.0.1"
+version = "2.0.3"
 description = "Collects data from tinkerforge outdoor weather station and saves it to sqlite database."
 authors = ["Patrick Zbinden <patrick+dev@zbinden-online.ch>"]
 readme = "README.md"
 packages = [{include = "ch"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `ch_sachi_weatherstation-2.0.1/PKG-INFO` & `ch_sachi_weatherstation-2.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch.sachi.weatherstation
-Version: 2.0.1
+Version: 2.0.3
 Summary: Collects data from tinkerforge outdoor weather station and saves it to sqlite database.
 Author: Patrick Zbinden
 Author-email: patrick+dev@zbinden-online.ch
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

