# Comparing `tmp/heartbeat_library-0.0.2.tar.gz` & `tmp/heartbeat_library-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heartbeat_library-0.0.2.tar", last modified: Mon May  6 13:42:45 2024, max compression
+gzip compressed data, was "heartbeat_library-0.0.3.tar", last modified: Mon May  6 13:51:44 2024, max compression
```

## Comparing `heartbeat_library-0.0.2.tar` & `heartbeat_library-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 13:42:45.286186 heartbeat_library-0.0.2/
--rw-rw-rw-   0        0        0     1104 2024-05-03 19:24:03.000000 heartbeat_library-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2108 2024-05-06 13:42:45.282801 heartbeat_library-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1270 2024-05-06 13:42:31.000000 heartbeat_library-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 13:42:45.261546 heartbeat_library-0.0.2/heartbeat-library/
--rw-rw-rw-   0        0        0       61 2024-05-06 11:51:28.000000 heartbeat_library-0.0.2/heartbeat-library/__init__.py
--rw-rw-rw-   0        0        0     3352 2024-05-06 12:00:43.000000 heartbeat_library-0.0.2/heartbeat-library/heartbeat.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:42:45.273373 heartbeat_library-0.0.2/heartbeat_library.egg-info/
--rw-rw-rw-   0        0        0     2108 2024-05-06 13:42:45.000000 heartbeat_library-0.0.2/heartbeat_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-05-06 13:42:45.000000 heartbeat_library-0.0.2/heartbeat_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 13:42:45.000000 heartbeat_library-0.0.2/heartbeat_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-06 13:42:45.000000 heartbeat_library-0.0.2/heartbeat_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-06 13:42:45.000000 heartbeat_library-0.0.2/heartbeat_library.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 13:42:45.286186 heartbeat_library-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1044 2024-05-06 13:42:41.000000 heartbeat_library-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:51:44.915035 heartbeat_library-0.0.3/
+-rw-rw-rw-   0        0        0     1104 2024-05-03 19:24:03.000000 heartbeat_library-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2057 2024-05-06 13:51:44.913034 heartbeat_library-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1270 2024-05-06 13:42:31.000000 heartbeat_library-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 13:51:44.901634 heartbeat_library-0.0.3/heartbeat-library/
+-rw-rw-rw-   0        0        0       61 2024-05-06 11:51:28.000000 heartbeat_library-0.0.3/heartbeat-library/__init__.py
+-rw-rw-rw-   0        0        0     3352 2024-05-06 12:00:43.000000 heartbeat_library-0.0.3/heartbeat-library/heartbeat.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:51:44.911033 heartbeat_library-0.0.3/heartbeat_library.egg-info/
+-rw-rw-rw-   0        0        0     2057 2024-05-06 13:51:44.000000 heartbeat_library-0.0.3/heartbeat_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-05-06 13:51:44.000000 heartbeat_library-0.0.3/heartbeat_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 13:51:44.000000 heartbeat_library-0.0.3/heartbeat_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-06 13:51:44.000000 heartbeat_library-0.0.3/heartbeat_library.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 13:51:44.915035 heartbeat_library-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2024-05-06 13:51:38.000000 heartbeat_library-0.0.3/setup.py
```

### Comparing `heartbeat_library-0.0.2/LICENSE` & `heartbeat_library-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `heartbeat_library-0.0.2/PKG-INFO` & `heartbeat_library-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: heartbeat-library
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for sending pulses to a process monitoring server
 Author: Pedro Ferreira Braz
 Author-email: pbraz.pedrof@gmail.com
 License: MIT License
 Keywords: heartbeat,heartbeat-library,heartbeat-api,heartbeat-wrapper,heartbeat-python,heartbeat-python-wrapper,heartbeat-python-api,heartbeat-python-wrapper-api,heartbeat-python-api-wrapper,multithreading,threading,requests,python-requests,python-threading,python-multithreading,python-heartbeat,python-heartbeat-api,python-heartbeat-wrapper,python-heartbeat-python,python-heartbeat-python-wrapper,python-heartbeat-python-api,python-heartbeat-python-wrapper-api,python-heartbeat-python-api-wrapper
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: threading
 
 # Python Heartbeat Library
 
 The Python Heartbeat Library is a simple utility that allows you to send regular "pulses" to a specific endpoint. These pulses serve as confirmation that your main script is functioning correctly. If the main script stops for any reason, the heartbeat will also cease, indicating that something went wrong.
 
 # Installation
```

### Comparing `heartbeat_library-0.0.2/README.md` & `heartbeat_library-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `heartbeat_library-0.0.2/heartbeat-library/heartbeat.py` & `heartbeat_library-0.0.3/heartbeat-library/heartbeat.py`

 * *Files identical despite different names*

### Comparing `heartbeat_library-0.0.2/heartbeat_library.egg-info/PKG-INFO` & `heartbeat_library-0.0.3/heartbeat_library.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: heartbeat-library
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for sending pulses to a process monitoring server
 Author: Pedro Ferreira Braz
 Author-email: pbraz.pedrof@gmail.com
 License: MIT License
 Keywords: heartbeat,heartbeat-library,heartbeat-api,heartbeat-wrapper,heartbeat-python,heartbeat-python-wrapper,heartbeat-python-api,heartbeat-python-wrapper-api,heartbeat-python-api-wrapper,multithreading,threading,requests,python-requests,python-threading,python-multithreading,python-heartbeat,python-heartbeat-api,python-heartbeat-wrapper,python-heartbeat-python,python-heartbeat-python-wrapper,python-heartbeat-python-api,python-heartbeat-python-wrapper-api,python-heartbeat-python-api-wrapper
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: threading
 
 # Python Heartbeat Library
 
 The Python Heartbeat Library is a simple utility that allows you to send regular "pulses" to a specific endpoint. These pulses serve as confirmation that your main script is functioning correctly. If the main script stops for any reason, the heartbeat will also cease, indicating that something went wrong.
 
 # Installation
```

### Comparing `heartbeat_library-0.0.2/setup.py` & `heartbeat_library-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='heartbeat-library',
-    version='0.0.2',
+    version='0.0.3',
     license='MIT License',
     author='Pedro Ferreira Braz',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='pbraz.pedrof@gmail.com',
     keywords='heartbeat, heartbeat-library, heartbeat-api, heartbeat-wrapper, heartbeat-python, heartbeat-python-wrapper, heartbeat-python-api, heartbeat-python-wrapper-api, heartbeat-python-api-wrapper, multithreading, threading, requests, python-requests, python-threading, python-multithreading, python-heartbeat, python-heartbeat-api, python-heartbeat-wrapper, python-heartbeat-python, python-heartbeat-python-wrapper, python-heartbeat-python-api, python-heartbeat-python-wrapper-api, python-heartbeat-python-api-wrapper',
     description=u'Library for sending pulses to a process monitoring server',
     packages=['heartbeat-library'],
-    install_requires=['requests', 'threading'],)
+    install_requires=[])
```

