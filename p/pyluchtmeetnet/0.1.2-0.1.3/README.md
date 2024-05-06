# Comparing `tmp/pyluchtmeetnet-0.1.2.tar.gz` & `tmp/pyluchtmeetnet-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyluchtmeetnet-0.1.2.tar", last modified: Tue Apr 12 14:37:33 2022, max compression
+gzip compressed data, was "pyluchtmeetnet-0.1.3.tar", last modified: Mon May  6 12:24:18 2024, max compression
```

## Comparing `pyluchtmeetnet-0.1.2.tar` & `pyluchtmeetnet-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 14:37:33.905288 pyluchtmeetnet-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-04-12 14:37:26.000000 pyluchtmeetnet-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-04-12 14:37:33.905288 pyluchtmeetnet-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-04-12 14:37:26.000000 pyluchtmeetnet-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 14:37:33.905288 pyluchtmeetnet-0.1.2/pyluchtmeetnet/
--rw-r--r--   0 runner    (1001) docker     (121)    10004 2022-04-12 14:37:26.000000 pyluchtmeetnet-0.1.2/pyluchtmeetnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 14:37:33.905288 pyluchtmeetnet-0.1.2/pyluchtmeetnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-04-12 14:37:33.000000 pyluchtmeetnet-0.1.2/pyluchtmeetnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-04-12 14:37:33.000000 pyluchtmeetnet-0.1.2/pyluchtmeetnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-12 14:37:33.000000 pyluchtmeetnet-0.1.2/pyluchtmeetnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-04-12 14:37:33.000000 pyluchtmeetnet-0.1.2/pyluchtmeetnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-12 14:37:33.000000 pyluchtmeetnet-0.1.2/pyluchtmeetnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-12 14:37:33.905288 pyluchtmeetnet-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-04-12 14:37:26.000000 pyluchtmeetnet-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:18.458310 pyluchtmeetnet-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-06 12:23:58.000000 pyluchtmeetnet-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-06 12:24:18.458310 pyluchtmeetnet-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-06 12:23:58.000000 pyluchtmeetnet-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:18.458310 pyluchtmeetnet-0.1.3/pyluchtmeetnet/
+-rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-05-06 12:23:58.000000 pyluchtmeetnet-0.1.3/pyluchtmeetnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:24:18.458310 pyluchtmeetnet-0.1.3/pyluchtmeetnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-06 12:24:18.000000 pyluchtmeetnet-0.1.3/pyluchtmeetnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-06 12:24:18.000000 pyluchtmeetnet-0.1.3/pyluchtmeetnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 12:24:18.000000 pyluchtmeetnet-0.1.3/pyluchtmeetnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 12:24:18.000000 pyluchtmeetnet-0.1.3/pyluchtmeetnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-06 12:24:18.000000 pyluchtmeetnet-0.1.3/pyluchtmeetnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 12:24:18.458310 pyluchtmeetnet-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-06 12:23:58.000000 pyluchtmeetnet-0.1.3/setup.py
```

### Comparing `pyluchtmeetnet-0.1.2/LICENSE` & `pyluchtmeetnet-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyluchtmeetnet-0.1.2/PKG-INFO` & `pyluchtmeetnet-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: pyluchtmeetnet
-Version: 0.1.2
+Version: 0.1.3
 Summary: A module for getting air quality data from Luchtmeetnet OpenAPI
 Home-page: https://github.com/metbril/pyluchtmeetnet
 Author: Robert van Bregt
 Author-email: robertvanbregt@gmail.com
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/metbril/pyluchtmeetnet/issues
 Project-URL: Funding, https://ko-fi.com/metbril
 Project-URL: Source, https://github.com/metbril/pyluchtmeetnet/
 Keywords: air quality,health,api
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+
+![PyPI - Version](https://img.shields.io/pypi/v/pyluchtmeetnet)
+![PyPI - Status](https://img.shields.io/pypi/status/pyluchtmeetnet)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pyluchtmeetnet)
 
 # pyluchtmeetnet
 
 A python package to use the [Luchtmeetnet 2020 OpenAPI][luchtmeetnet-api].
 
 ## Installation
 
@@ -55,9 +59,7 @@
 
 # Get latest measurements from station
 measurements = lmn.get_latest_station_measurements(station["number"])
 print(measurements)
 ```
 
 [luchtmeetnet-api]: https://api-docs.luchtmeetnet.nl/
-
-
```

### Comparing `pyluchtmeetnet-0.1.2/README.md` & `pyluchtmeetnet-0.1.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+![PyPI - Version](https://img.shields.io/pypi/v/pyluchtmeetnet)
+![PyPI - Status](https://img.shields.io/pypi/status/pyluchtmeetnet)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pyluchtmeetnet)
+
 # pyluchtmeetnet
 
 A python package to use the [Luchtmeetnet 2020 OpenAPI][luchtmeetnet-api].
 
 ## Installation
 
 ```shell
```

### Comparing `pyluchtmeetnet-0.1.2/pyluchtmeetnet/__init__.py` & `pyluchtmeetnet-0.1.3/pyluchtmeetnet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,23 +88,23 @@
                 json_content = json.loads(content)
                 measurements = json_content["data"]
             except json.JSONDecodeError as err:
                 _LOGGER.error("Unable to parse content as json. %s", err)
 
         data = []
         for component in components:
-            json_component = [
-                meas for meas in measurements if meas["formula"] == component
-            ]
-            element = {
-                component: json_component[0]["value"],
-                "timestamp": json_component[0]["timestamp_measured"],
-            }
-            data.append(element)
-
+            for meas in measurements:
+                if meas["formula"] == component:
+                    json_component = [meas]
+                    element = {
+                        component: json_component[0]["value"],
+                        "timestamp": json_component[0]["timestamp_measured"],
+                    }
+                    data.append(element)
+                    
         _LOGGER.debug("Latest measurements:\n%s", data)
         return data
 
     def __get_stations(self):
         _LOGGER.info("Get all stations.")
         stations = []
         result = self.__get_stations_page_json(1)
```

### Comparing `pyluchtmeetnet-0.1.2/pyluchtmeetnet.egg-info/PKG-INFO` & `pyluchtmeetnet-0.1.3/pyluchtmeetnet.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: pyluchtmeetnet
-Version: 0.1.2
+Version: 0.1.3
 Summary: A module for getting air quality data from Luchtmeetnet OpenAPI
 Home-page: https://github.com/metbril/pyluchtmeetnet
 Author: Robert van Bregt
 Author-email: robertvanbregt@gmail.com
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/metbril/pyluchtmeetnet/issues
 Project-URL: Funding, https://ko-fi.com/metbril
 Project-URL: Source, https://github.com/metbril/pyluchtmeetnet/
 Keywords: air quality,health,api
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+
+![PyPI - Version](https://img.shields.io/pypi/v/pyluchtmeetnet)
+![PyPI - Status](https://img.shields.io/pypi/status/pyluchtmeetnet)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/pyluchtmeetnet)
 
 # pyluchtmeetnet
 
 A python package to use the [Luchtmeetnet 2020 OpenAPI][luchtmeetnet-api].
 
 ## Installation
 
@@ -55,9 +59,7 @@
 
 # Get latest measurements from station
 measurements = lmn.get_latest_station_measurements(station["number"])
 print(measurements)
 ```
 
 [luchtmeetnet-api]: https://api-docs.luchtmeetnet.nl/
-
-
```

### Comparing `pyluchtmeetnet-0.1.2/setup.py` & `pyluchtmeetnet-0.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,36 +8,37 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pyluchtmeetnet",
-    version="0.1.2",
+    version="0.1.3",
     description="A module for getting air quality data from Luchtmeetnet OpenAPI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/metbril/pyluchtmeetnet",
     author="Robert van Bregt",
     author_email="robertvanbregt@gmail.com",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords="air quality, health, api",
     packages=find_packages(),
-    python_requires=">=3.7, <4",
+    python_requires=">=3.8, <4",
     install_requires=["requests"],
     project_urls={
         "Bug Reports": "https://github.com/metbril/pyluchtmeetnet/issues",
         "Funding": "https://ko-fi.com/metbril",
         "Source": "https://github.com/metbril/pyluchtmeetnet/",
     },
 )
```

