# Comparing `tmp/heartbeat_library-0.0.4.tar.gz` & `tmp/heartbeat_library-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heartbeat_library-0.0.4.tar", last modified: Mon May  6 14:16:04 2024, max compression
+gzip compressed data, was "heartbeat_library-0.0.5.tar", last modified: Mon May  6 14:33:33 2024, max compression
```

## Comparing `heartbeat_library-0.0.4.tar` & `heartbeat_library-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 14:16:04.252015 heartbeat_library-0.0.4/
--rw-rw-rw-   0        0        0     1104 2024-05-03 19:24:03.000000 heartbeat_library-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2057 2024-05-06 14:16:04.251012 heartbeat_library-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1270 2024-05-06 13:42:31.000000 heartbeat_library-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 14:16:04.242687 heartbeat_library-0.0.4/heartbeat-library/
--rw-rw-rw-   0        0        0       61 2024-05-06 11:51:28.000000 heartbeat_library-0.0.4/heartbeat-library/__init__.py
--rw-rw-rw-   0        0        0     3352 2024-05-06 12:00:43.000000 heartbeat_library-0.0.4/heartbeat-library/heartbeat-library.py
-drwxrwxrwx   0        0        0        0 2024-05-06 14:16:04.250020 heartbeat_library-0.0.4/heartbeat_library.egg-info/
--rw-rw-rw-   0        0        0     2057 2024-05-06 14:16:04.000000 heartbeat_library-0.0.4/heartbeat_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-05-06 14:16:04.000000 heartbeat_library-0.0.4/heartbeat_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 14:16:04.000000 heartbeat_library-0.0.4/heartbeat_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-06 14:16:04.000000 heartbeat_library-0.0.4/heartbeat_library.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 14:16:04.252015 heartbeat_library-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1020 2024-05-06 14:14:33.000000 heartbeat_library-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:33:33.383080 heartbeat_library-0.0.5/
+-rw-rw-rw-   0        0        0     1104 2024-05-03 19:24:03.000000 heartbeat_library-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2057 2024-05-06 14:33:33.381930 heartbeat_library-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1270 2024-05-06 13:42:31.000000 heartbeat_library-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 14:33:33.372931 heartbeat_library-0.0.5/heartbeat-library/
+-rw-rw-rw-   0        0        0       69 2024-05-06 14:32:36.000000 heartbeat_library-0.0.5/heartbeat-library/__init__.py
+-rw-rw-rw-   0        0        0     3352 2024-05-06 12:00:43.000000 heartbeat_library-0.0.5/heartbeat-library/heartbeat_library.py
+drwxrwxrwx   0        0        0        0 2024-05-06 14:33:33.379942 heartbeat_library-0.0.5/heartbeat_library.egg-info/
+-rw-rw-rw-   0        0        0     2057 2024-05-06 14:33:33.000000 heartbeat_library-0.0.5/heartbeat_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-05-06 14:33:33.000000 heartbeat_library-0.0.5/heartbeat_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 14:33:33.000000 heartbeat_library-0.0.5/heartbeat_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-06 14:33:33.000000 heartbeat_library-0.0.5/heartbeat_library.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 14:33:33.383080 heartbeat_library-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2024-05-06 14:32:54.000000 heartbeat_library-0.0.5/setup.py
```

### Comparing `heartbeat_library-0.0.4/LICENSE` & `heartbeat_library-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `heartbeat_library-0.0.4/PKG-INFO` & `heartbeat_library-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heartbeat-library
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library for sending pulses to a process monitoring server
 Author: Pedro Ferreira Braz
 Author-email: pbraz.pedrof@gmail.com
 License: MIT License
 Keywords: heartbeat,heartbeat-library,heartbeat-api,heartbeat-wrapper,heartbeat-python,heartbeat-python-wrapper,heartbeat-python-api,heartbeat-python-wrapper-api,heartbeat-python-api-wrapper,multithreading,threading,requests,python-requests,python-threading,python-multithreading,python-heartbeat,python-heartbeat-api,python-heartbeat-wrapper,python-heartbeat-python,python-heartbeat-python-wrapper,python-heartbeat-python-api,python-heartbeat-python-wrapper-api,python-heartbeat-python-api-wrapper
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `heartbeat_library-0.0.4/README.md` & `heartbeat_library-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `heartbeat_library-0.0.4/heartbeat-library/heartbeat-library.py` & `heartbeat_library-0.0.5/heartbeat-library/heartbeat_library.py`

 * *Files identical despite different names*

### Comparing `heartbeat_library-0.0.4/heartbeat_library.egg-info/PKG-INFO` & `heartbeat_library-0.0.5/heartbeat_library.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heartbeat-library
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library for sending pulses to a process monitoring server
 Author: Pedro Ferreira Braz
 Author-email: pbraz.pedrof@gmail.com
 License: MIT License
 Keywords: heartbeat,heartbeat-library,heartbeat-api,heartbeat-wrapper,heartbeat-python,heartbeat-python-wrapper,heartbeat-python-api,heartbeat-python-wrapper-api,heartbeat-python-api-wrapper,multithreading,threading,requests,python-requests,python-threading,python-multithreading,python-heartbeat,python-heartbeat-api,python-heartbeat-wrapper,python-heartbeat-python,python-heartbeat-python-wrapper,python-heartbeat-python-api,python-heartbeat-python-wrapper-api,python-heartbeat-python-api-wrapper
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `heartbeat_library-0.0.4/setup.py` & `heartbeat_library-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='heartbeat-library',
-    version='0.0.4',
+    version='0.0.5',
     license='MIT License',
     author='Pedro Ferreira Braz',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='pbraz.pedrof@gmail.com',
     keywords='heartbeat, heartbeat-library, heartbeat-api, heartbeat-wrapper, heartbeat-python, heartbeat-python-wrapper, heartbeat-python-api, heartbeat-python-wrapper-api, heartbeat-python-api-wrapper, multithreading, threading, requests, python-requests, python-threading, python-multithreading, python-heartbeat, python-heartbeat-api, python-heartbeat-wrapper, python-heartbeat-python, python-heartbeat-python-wrapper, python-heartbeat-python-api, python-heartbeat-python-wrapper-api, python-heartbeat-python-api-wrapper',
     description=u'Library for sending pulses to a process monitoring server',
```

