# Comparing `tmp/openweatherapi_sdk-0.2.tar.gz` & `tmp/openweatherapi_sdk-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\openweatherapi_sdk-0.2.tar", last modified: Mon May  6 12:50:47 2024, max compression
+gzip compressed data, was "dist\openweatherapi_sdk-0.3.tar", last modified: Mon May  6 13:10:45 2024, max compression
```

## Comparing `openweatherapi_sdk-0.2.tar` & `openweatherapi_sdk-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 12:50:47.128352 openweatherapi_sdk-0.2/
--rw-rw-rw-   0        0        0     1088 2024-05-05 09:09:40.000000 openweatherapi_sdk-0.2/LICENSE
--rw-rw-rw-   0        0        0     1689 2024-05-06 12:50:47.128352 openweatherapi_sdk-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1273 2024-05-05 19:55:42.000000 openweatherapi_sdk-0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-06 12:50:47.128352 openweatherapi_sdk-0.2/setup.cfg
--rw-rw-rw-   0        0        0      760 2024-05-06 12:47:30.000000 openweatherapi_sdk-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 12:50:47.077298 openweatherapi_sdk-0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 12:50:47.124226 openweatherapi_sdk-0.2/src/openweatherapi_sdk.egg-info/
--rw-rw-rw-   0        0        0     1689 2024-05-06 12:50:46.000000 openweatherapi_sdk-0.2/src/openweatherapi_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-05-06 12:50:46.000000 openweatherapi_sdk-0.2/src/openweatherapi_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 12:50:46.000000 openweatherapi_sdk-0.2/src/openweatherapi_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-06 12:50:46.000000 openweatherapi_sdk-0.2/src/openweatherapi_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 12:50:46.000000 openweatherapi_sdk-0.2/src/openweatherapi_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 13:10:45.956721 openweatherapi_sdk-0.3/
+-rw-rw-rw-   0        0        0     1088 2024-05-05 09:09:40.000000 openweatherapi_sdk-0.3/LICENSE
+-rw-rw-rw-   0        0        0     1281 2024-05-06 13:10:45.952376 openweatherapi_sdk-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2024-05-05 07:03:35.000000 openweatherapi_sdk-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-06 13:10:45.956721 openweatherapi_sdk-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      760 2024-05-06 13:09:32.000000 openweatherapi_sdk-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:10:45.929839 openweatherapi_sdk-0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 13:10:45.952376 openweatherapi_sdk-0.3/src/openweatherapi_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1281 2024-05-06 13:10:45.000000 openweatherapi_sdk-0.3/src/openweatherapi_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-05-06 13:10:45.000000 openweatherapi_sdk-0.3/src/openweatherapi_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 13:10:45.000000 openweatherapi_sdk-0.3/src/openweatherapi_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-06 13:10:45.000000 openweatherapi_sdk-0.3/src/openweatherapi_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 13:10:45.000000 openweatherapi_sdk-0.3/src/openweatherapi_sdk.egg-info/top_level.txt
```

### Comparing `openweatherapi_sdk-0.2/LICENSE` & `openweatherapi_sdk-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openweatherapi_sdk-0.2/PKG-INFO` & `openweatherapi_sdk-0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openweatherapi-sdk
-Version: 0.2
+Version: 0.3
 Summary: A simple SDK for interacting with the OpenWeatherMap API
 Author: Snehal Palve
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -15,20 +15,20 @@
 
 A simple SDK for interacting with the OpenWeatherMap API.
 
 ## Installation
 
 You can install the package using pip:
 
-pip install openweatherapi_sdk
+pip install weather_sdk
 
 
 # Usage
 * First, initialize the SDK with your OpenWeatherMap API key:
-from openweatherapi_sdk.sdk import WeatherSDK
+from weather_sdk.sdk import WeatherSDK
 
 sdk = WeatherSDK(api_key="YOUR_API_KEY_HERE")
 
 * Get Weather by City Name
 You can retrieve weather data for a city by its name:
 
 data = sdk.get_weather_by_city_name("London")
@@ -37,22 +37,11 @@
 
 * Get Weather by Coordinates
 You can retrieve weather data for a location using its latitude and longitude coordinates:
 
 data = sdk.get_weather_by_coordinates(lat=51.51, lon=-0.13)
 print(data)
 
-* Get Weather Timestamp
-You can retrieve weather data timestamp for a location using its latitude and longitude coordinates and time:
-
-data = sdk.get_weather_by_coordinates(lat=51.51, lon=-0.13, dt=1643803200 )
-print(data)
-
-
-* Get daily Aggregation
-You can retrieve daily aggregation for a location using its latitude and longitude coordinates, date and timezone:
-
-data = sdk.get_weather_by_coordinates(lat=51.51, lon=-0.13,&date=2020-03-04)
-print(data)
+* Replace "YOUR_API_KEY_HERE" with your actual OpenWeatherMap API key.
 
 
 * Make sure to replace `"YOUR_API_KEY_HERE"` with your actual OpenWeatherMap API key in the usage examples.
```

### Comparing `openweatherapi_sdk-0.2/README.md` & `openweatherapi_sdk-0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 A simple SDK for interacting with the OpenWeatherMap API.
 
 ## Installation
 
 You can install the package using pip:
 
-pip install openweatherapi_sdk
+pip install weather_sdk
 
 
 # Usage
 * First, initialize the SDK with your OpenWeatherMap API key:
-from openweatherapi_sdk.sdk import WeatherSDK
+from weather_sdk.sdk import WeatherSDK
 
 sdk = WeatherSDK(api_key="YOUR_API_KEY_HERE")
 
 * Get Weather by City Name
 You can retrieve weather data for a city by its name:
 
 data = sdk.get_weather_by_city_name("London")
@@ -24,22 +24,11 @@
 
 * Get Weather by Coordinates
 You can retrieve weather data for a location using its latitude and longitude coordinates:
 
 data = sdk.get_weather_by_coordinates(lat=51.51, lon=-0.13)
 print(data)
 
-* Get Weather Timestamp
-You can retrieve weather data timestamp for a location using its latitude and longitude coordinates and time:
-
-data = sdk.get_weather_by_coordinates(lat=51.51, lon=-0.13, dt=1643803200 )
-print(data)
-
-
-* Get daily Aggregation
-You can retrieve daily aggregation for a location using its latitude and longitude coordinates, date and timezone:
-
-data = sdk.get_weather_by_coordinates(lat=51.51, lon=-0.13,&date=2020-03-04)
-print(data)
+* Replace "YOUR_API_KEY_HERE" with your actual OpenWeatherMap API key.
 
 
-* Make sure to replace `"YOUR_API_KEY_HERE"` with your actual OpenWeatherMap API key in the usage examples.
+* Make sure to replace `"YOUR_API_KEY_HERE"` with your actual OpenWeatherMap API key in the usage examples.
```

### Comparing `openweatherapi_sdk-0.2/setup.py` & `openweatherapi_sdk-0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r") as fh:
     long_description = fh.read()
 
 setup(
     name="openweatherapi-sdk",
-    version="0.2",
+    version="0.3",
     packages=find_packages(),
-    package_data={'': ['sdk/*.py']},  
+    package_data={'': ['src/*.py']},  
     install_requires=["requests"],
     author="Snehal Palve",
     description="A simple SDK for interacting with the OpenWeatherMap API",
     long_description=long_description,
     long_description_content_type= "text/markdown",
     classifiers =[
     "Programming Language :: Python :: 3",
```

### Comparing `openweatherapi_sdk-0.2/src/openweatherapi_sdk.egg-info/PKG-INFO` & `openweatherapi_sdk-0.3/src/openweatherapi_sdk.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openweatherapi-sdk
-Version: 0.2
+Version: 0.3
 Summary: A simple SDK for interacting with the OpenWeatherMap API
 Author: Snehal Palve
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -15,20 +15,20 @@
 
 A simple SDK for interacting with the OpenWeatherMap API.
 
 ## Installation
 
 You can install the package using pip:
 
-pip install openweatherapi_sdk
+pip install weather_sdk
 
 
 # Usage
 * First, initialize the SDK with your OpenWeatherMap API key:
-from openweatherapi_sdk.sdk import WeatherSDK
+from weather_sdk.sdk import WeatherSDK
 
 sdk = WeatherSDK(api_key="YOUR_API_KEY_HERE")
 
 * Get Weather by City Name
 You can retrieve weather data for a city by its name:
 
 data = sdk.get_weather_by_city_name("London")
@@ -37,22 +37,11 @@
 
 * Get Weather by Coordinates
 You can retrieve weather data for a location using its latitude and longitude coordinates:
 
 data = sdk.get_weather_by_coordinates(lat=51.51, lon=-0.13)
 print(data)
 
-* Get Weather Timestamp
-You can retrieve weather data timestamp for a location using its latitude and longitude coordinates and time:
-
-data = sdk.get_weather_by_coordinates(lat=51.51, lon=-0.13, dt=1643803200 )
-print(data)
-
-
-* Get daily Aggregation
-You can retrieve daily aggregation for a location using its latitude and longitude coordinates, date and timezone:
-
-data = sdk.get_weather_by_coordinates(lat=51.51, lon=-0.13,&date=2020-03-04)
-print(data)
+* Replace "YOUR_API_KEY_HERE" with your actual OpenWeatherMap API key.
 
 
 * Make sure to replace `"YOUR_API_KEY_HERE"` with your actual OpenWeatherMap API key in the usage examples.
```

