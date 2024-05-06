# Comparing `tmp/vsvnapplicationmonitoring-0.1.2.tar.gz` & `tmp/vsvnapplicationmonitoring-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsvnapplicationmonitoring-0.1.2.tar", last modified: Fri Apr 26 04:58:02 2024, max compression
+gzip compressed data, was "vsvnapplicationmonitoring-0.1.4.tar", last modified: Mon May  6 03:04:59 2024, max compression
```

## Comparing `vsvnapplicationmonitoring-0.1.2.tar` & `vsvnapplicationmonitoring-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 04:58:02.306088 vsvnapplicationmonitoring-0.1.2/
--rw-rw-rw-   0        0        0    11558 2024-04-26 03:33:01.000000 vsvnapplicationmonitoring-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      833 2024-04-26 04:58:02.305084 vsvnapplicationmonitoring-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      626 2024-04-26 04:56:43.000000 vsvnapplicationmonitoring-0.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-26 04:58:02.287085 vsvnapplicationmonitoring-0.1.2/VSVNApplicationMonitoring/
--rw-rw-rw-   0        0        0        0 2024-04-26 03:33:01.000000 vsvnapplicationmonitoring-0.1.2/VSVNApplicationMonitoring/__init__.py
--rw-rw-rw-   0        0        0      725 2024-04-26 03:42:34.000000 vsvnapplicationmonitoring-0.1.2/VSVNApplicationMonitoring/run.py
-drwxrwxrwx   0        0        0        0 2024-04-26 04:58:02.304083 vsvnapplicationmonitoring-0.1.2/VSVNApplicationMonitoring.egg-info/
--rw-rw-rw-   0        0        0      833 2024-04-26 04:58:02.000000 vsvnapplicationmonitoring-0.1.2/VSVNApplicationMonitoring.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2024-04-26 04:58:02.000000 vsvnapplicationmonitoring-0.1.2/VSVNApplicationMonitoring.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 04:58:02.000000 vsvnapplicationmonitoring-0.1.2/VSVNApplicationMonitoring.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-26 04:58:02.000000 vsvnapplicationmonitoring-0.1.2/VSVNApplicationMonitoring.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 04:58:02.307084 vsvnapplicationmonitoring-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      470 2024-04-26 04:57:48.000000 vsvnapplicationmonitoring-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:04:59.499319 vsvnapplicationmonitoring-0.1.4/
+-rw-rw-rw-   0        0        0    11558 2024-04-26 03:33:01.000000 vsvnapplicationmonitoring-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1338 2024-05-06 03:04:59.497318 vsvnapplicationmonitoring-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1131 2024-05-06 03:02:52.000000 vsvnapplicationmonitoring-0.1.4/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-06 03:04:59.479318 vsvnapplicationmonitoring-0.1.4/VSVNApplicationMonitoring/
+-rw-rw-rw-   0        0        0        0 2024-04-26 03:33:01.000000 vsvnapplicationmonitoring-0.1.4/VSVNApplicationMonitoring/__init__.py
+-rw-rw-rw-   0        0        0     1432 2024-05-06 03:04:01.000000 vsvnapplicationmonitoring-0.1.4/VSVNApplicationMonitoring/run.py
+drwxrwxrwx   0        0        0        0 2024-05-06 03:04:59.497318 vsvnapplicationmonitoring-0.1.4/VSVNApplicationMonitoring.egg-info/
+-rw-rw-rw-   0        0        0     1338 2024-05-06 03:04:59.000000 vsvnapplicationmonitoring-0.1.4/VSVNApplicationMonitoring.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-05-06 03:04:59.000000 vsvnapplicationmonitoring-0.1.4/VSVNApplicationMonitoring.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 03:04:59.000000 vsvnapplicationmonitoring-0.1.4/VSVNApplicationMonitoring.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-06 03:04:59.000000 vsvnapplicationmonitoring-0.1.4/VSVNApplicationMonitoring.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 03:04:59.499319 vsvnapplicationmonitoring-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      470 2024-05-06 03:04:49.000000 vsvnapplicationmonitoring-0.1.4/setup.py
```

### Comparing `vsvnapplicationmonitoring-0.1.2/LICENSE` & `vsvnapplicationmonitoring-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vsvnapplicationmonitoring-0.1.2/VSVNApplicationMonitoring/run.py` & `vsvnapplicationmonitoring-0.1.4/VSVNApplicationMonitoring/run.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,37 @@
 
 import requests
 
 
-def save(data_to_send : any, api_url: any):
+def saveActiveUser(data_user : any, api_url: any):
     try:
         # Send a POST request to the specified URL with the data
-        url = api_url + '/application.service/update-active-user-cost'
-        response = requests.post(url, json=data_to_send)
+        url = api_url + '/applications/create-active-user'
+        response = requests.post(url, json=data_user)
+        
+        # Check if the request was successful
+        response.raise_for_status()
+        
+        # Extract data from the response
+        data = response.json()
+        
+        # Return the data
+        return data
+    except requests.exceptions.RequestException as e:
+        # If an error occurs during the request, catch it here
+        print('Lỗi khi gọi API:', e)
+        
+        # Rethrow the error
+        raise
+    
+def saveRequestCost(data_request : any, api_url: any):
+    try:
+        # Send a POST request to the specified URL with the data
+        url = api_url + '/application.service/create-service-cost'
+        response = requests.post(url, json=data_request)
         
         # Check if the request was successful
         response.raise_for_status()
         
         # Extract data from the response
         data = response.json()
```

