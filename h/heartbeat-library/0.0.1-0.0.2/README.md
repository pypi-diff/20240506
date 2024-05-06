# Comparing `tmp/heartbeat_library-0.0.1.tar.gz` & `tmp/heartbeat_library-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heartbeat_library-0.0.1.tar", last modified: Mon May  6 13:39:15 2024, max compression
+gzip compressed data, was "heartbeat_library-0.0.2.tar", last modified: Mon May  6 13:42:45 2024, max compression
```

## Comparing `heartbeat_library-0.0.1.tar` & `heartbeat_library-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 13:39:15.379364 heartbeat_library-0.0.1/
--rw-rw-rw-   0        0        0     1104 2024-05-03 19:24:03.000000 heartbeat_library-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2083 2024-05-06 13:39:15.376368 heartbeat_library-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1245 2024-05-06 12:39:40.000000 heartbeat_library-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 13:39:15.364393 heartbeat_library-0.0.1/heartbeat-library/
--rw-rw-rw-   0        0        0       61 2024-05-06 11:51:28.000000 heartbeat_library-0.0.1/heartbeat-library/__init__.py
--rw-rw-rw-   0        0        0     3352 2024-05-06 12:00:43.000000 heartbeat_library-0.0.1/heartbeat-library/heartbeat.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:39:15.374365 heartbeat_library-0.0.1/heartbeat_library.egg-info/
--rw-rw-rw-   0        0        0     2083 2024-05-06 13:39:15.000000 heartbeat_library-0.0.1/heartbeat_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-05-06 13:39:15.000000 heartbeat_library-0.0.1/heartbeat_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 13:39:15.000000 heartbeat_library-0.0.1/heartbeat_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-06 13:39:15.000000 heartbeat_library-0.0.1/heartbeat_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-06 13:39:15.000000 heartbeat_library-0.0.1/heartbeat_library.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 13:39:15.379364 heartbeat_library-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1040 2024-05-06 13:36:18.000000 heartbeat_library-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:42:45.286186 heartbeat_library-0.0.2/
+-rw-rw-rw-   0        0        0     1104 2024-05-03 19:24:03.000000 heartbeat_library-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2108 2024-05-06 13:42:45.282801 heartbeat_library-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1270 2024-05-06 13:42:31.000000 heartbeat_library-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 13:42:45.261546 heartbeat_library-0.0.2/heartbeat-library/
+-rw-rw-rw-   0        0        0       61 2024-05-06 11:51:28.000000 heartbeat_library-0.0.2/heartbeat-library/__init__.py
+-rw-rw-rw-   0        0        0     3352 2024-05-06 12:00:43.000000 heartbeat_library-0.0.2/heartbeat-library/heartbeat.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:42:45.273373 heartbeat_library-0.0.2/heartbeat_library.egg-info/
+-rw-rw-rw-   0        0        0     2108 2024-05-06 13:42:45.000000 heartbeat_library-0.0.2/heartbeat_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2024-05-06 13:42:45.000000 heartbeat_library-0.0.2/heartbeat_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 13:42:45.000000 heartbeat_library-0.0.2/heartbeat_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-06 13:42:45.000000 heartbeat_library-0.0.2/heartbeat_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-06 13:42:45.000000 heartbeat_library-0.0.2/heartbeat_library.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 13:42:45.286186 heartbeat_library-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2024-05-06 13:42:41.000000 heartbeat_library-0.0.2/setup.py
```

### Comparing `heartbeat_library-0.0.1/LICENSE` & `heartbeat_library-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heartbeat_library-0.0.1/PKG-INFO` & `heartbeat_library-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heartbeat-library
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library for sending pulses to a process monitoring server
 Author: Pedro Ferreira Braz
 Author-email: pbraz.pedrof@gmail.com
 License: MIT License
 Keywords: heartbeat,heartbeat-library,heartbeat-api,heartbeat-wrapper,heartbeat-python,heartbeat-python-wrapper,heartbeat-python-api,heartbeat-python-wrapper-api,heartbeat-python-api-wrapper,multithreading,threading,requests,python-requests,python-threading,python-multithreading,python-heartbeat,python-heartbeat-api,python-heartbeat-wrapper,python-heartbeat-python,python-heartbeat-python-wrapper,python-heartbeat-python-api,python-heartbeat-python-wrapper-api,python-heartbeat-python-api-wrapper
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,24 +15,24 @@
 
 The Python Heartbeat Library is a simple utility that allows you to send regular "pulses" to a specific endpoint. These pulses serve as confirmation that your main script is functioning correctly. If the main script stops for any reason, the heartbeat will also cease, indicating that something went wrong.
 
 # Installation
 
 You can install the Python Heartbeat Library using pip:
 
-pip install heartbeat
+pip install heartbeat-library
 
 # Example
 
 ```python
 ===============================================================================================================================
-from heartbeat import defineUrl, heartbeat
+from heartbeat-library import setUrl, heartbeat, killHeartbeat
 
 # Set the URL for sending pulses
-defineUrl("https://")
+setUrl("https://")
 
 # Start the heartbeat with a pulse every 10 seconds
 heartbeat(interval = 600, name = 'process name', description = 'process description', additional_info = '', show_response = True)
 
 # Your main script logic goes here...
 
 # When your script ends or encounters an error, stop the heartbeat
```

### Comparing `heartbeat_library-0.0.1/README.md` & `heartbeat_library-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 The Python Heartbeat Library is a simple utility that allows you to send regular "pulses" to a specific endpoint. These pulses serve as confirmation that your main script is functioning correctly. If the main script stops for any reason, the heartbeat will also cease, indicating that something went wrong.
 
 # Installation
 
 You can install the Python Heartbeat Library using pip:
 
-pip install heartbeat
+pip install heartbeat-library
 
 # Example
 
 ```python
 ===============================================================================================================================
-from heartbeat import defineUrl, heartbeat
+from heartbeat-library import setUrl, heartbeat, killHeartbeat
 
 # Set the URL for sending pulses
-defineUrl("https://")
+setUrl("https://")
 
 # Start the heartbeat with a pulse every 10 seconds
 heartbeat(interval = 600, name = 'process name', description = 'process description', additional_info = '', show_response = True)
 
 # Your main script logic goes here...
 
 # When your script ends or encounters an error, stop the heartbeat
```

### Comparing `heartbeat_library-0.0.1/heartbeat-library/heartbeat.py` & `heartbeat_library-0.0.2/heartbeat-library/heartbeat.py`

 * *Files identical despite different names*

### Comparing `heartbeat_library-0.0.1/heartbeat_library.egg-info/PKG-INFO` & `heartbeat_library-0.0.2/heartbeat_library.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heartbeat-library
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library for sending pulses to a process monitoring server
 Author: Pedro Ferreira Braz
 Author-email: pbraz.pedrof@gmail.com
 License: MIT License
 Keywords: heartbeat,heartbeat-library,heartbeat-api,heartbeat-wrapper,heartbeat-python,heartbeat-python-wrapper,heartbeat-python-api,heartbeat-python-wrapper-api,heartbeat-python-api-wrapper,multithreading,threading,requests,python-requests,python-threading,python-multithreading,python-heartbeat,python-heartbeat-api,python-heartbeat-wrapper,python-heartbeat-python,python-heartbeat-python-wrapper,python-heartbeat-python-api,python-heartbeat-python-wrapper-api,python-heartbeat-python-api-wrapper
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,24 +15,24 @@
 
 The Python Heartbeat Library is a simple utility that allows you to send regular "pulses" to a specific endpoint. These pulses serve as confirmation that your main script is functioning correctly. If the main script stops for any reason, the heartbeat will also cease, indicating that something went wrong.
 
 # Installation
 
 You can install the Python Heartbeat Library using pip:
 
-pip install heartbeat
+pip install heartbeat-library
 
 # Example
 
 ```python
 ===============================================================================================================================
-from heartbeat import defineUrl, heartbeat
+from heartbeat-library import setUrl, heartbeat, killHeartbeat
 
 # Set the URL for sending pulses
-defineUrl("https://")
+setUrl("https://")
 
 # Start the heartbeat with a pulse every 10 seconds
 heartbeat(interval = 600, name = 'process name', description = 'process description', additional_info = '', show_response = True)
 
 # Your main script logic goes here...
 
 # When your script ends or encounters an error, stop the heartbeat
```

### Comparing `heartbeat_library-0.0.1/setup.py` & `heartbeat_library-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='heartbeat-library',
-    version='0.0.1',
+    version='0.0.2',
     license='MIT License',
     author='Pedro Ferreira Braz',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='pbraz.pedrof@gmail.com',
     keywords='heartbeat, heartbeat-library, heartbeat-api, heartbeat-wrapper, heartbeat-python, heartbeat-python-wrapper, heartbeat-python-api, heartbeat-python-wrapper-api, heartbeat-python-api-wrapper, multithreading, threading, requests, python-requests, python-threading, python-multithreading, python-heartbeat, python-heartbeat-api, python-heartbeat-wrapper, python-heartbeat-python, python-heartbeat-python-wrapper, python-heartbeat-python-api, python-heartbeat-python-wrapper-api, python-heartbeat-python-api-wrapper',
     description=u'Library for sending pulses to a process monitoring server',
     packages=['heartbeat-library'],
     install_requires=['requests', 'threading'],)
 
 
 
+
+
```

