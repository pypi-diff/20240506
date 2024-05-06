# Comparing `tmp/heartbeat_library-0.0.6.tar.gz` & `tmp/heartbeat_library-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heartbeat_library-0.0.6.tar", last modified: Mon May  6 18:05:06 2024, max compression
+gzip compressed data, was "heartbeat_library-0.0.7.tar", last modified: Mon May  6 18:17:15 2024, max compression
```

## Comparing `heartbeat_library-0.0.6.tar` & `heartbeat_library-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 18:05:06.918808 heartbeat_library-0.0.6/
--rw-rw-rw-   0        0        0     1104 2024-05-03 19:24:03.000000 heartbeat_library-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     2057 2024-05-06 18:05:06.917811 heartbeat_library-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1270 2024-05-06 13:42:31.000000 heartbeat_library-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 18:05:06.907822 heartbeat_library-0.0.6/heartbeat-library/
--rw-rw-rw-   0        0        0       65 2024-05-06 17:58:23.000000 heartbeat_library-0.0.6/heartbeat-library/__init__.py
--rw-rw-rw-   0        0        0     3416 2024-05-06 17:50:42.000000 heartbeat_library-0.0.6/heartbeat-library/heartbeat_library.py
-drwxrwxrwx   0        0        0        0 2024-05-06 18:05:06.916809 heartbeat_library-0.0.6/heartbeat_library.egg-info/
--rw-rw-rw-   0        0        0     2057 2024-05-06 18:05:06.000000 heartbeat_library-0.0.6/heartbeat_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2024-05-06 18:05:06.000000 heartbeat_library-0.0.6/heartbeat_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 18:05:06.000000 heartbeat_library-0.0.6/heartbeat_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-06 18:02:12.000000 heartbeat_library-0.0.6/heartbeat_library.egg-info/requirements.txt
--rw-rw-rw-   0        0        0       18 2024-05-06 18:05:06.000000 heartbeat_library-0.0.6/heartbeat_library.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 18:05:06.918808 heartbeat_library-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1010 2024-05-06 18:05:05.000000 heartbeat_library-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:17:15.523853 heartbeat_library-0.0.7/
+-rw-rw-rw-   0        0        0     1104 2024-05-03 19:24:03.000000 heartbeat_library-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2057 2024-05-06 18:17:15.521843 heartbeat_library-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1270 2024-05-06 13:42:31.000000 heartbeat_library-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 18:17:15.495804 heartbeat_library-0.0.7/heartbeat-library/
+-rw-rw-rw-   0        0        0       65 2024-05-06 17:58:23.000000 heartbeat_library-0.0.7/heartbeat-library/__init__.py
+-rw-rw-rw-   0        0        0     3416 2024-05-06 17:50:42.000000 heartbeat_library-0.0.7/heartbeat-library/heartbeat_library.py
+drwxrwxrwx   0        0        0        0 2024-05-06 18:17:15.511812 heartbeat_library-0.0.7/heartbeat_library.egg-info/
+-rw-rw-rw-   0        0        0     2057 2024-05-06 18:17:15.000000 heartbeat_library-0.0.7/heartbeat_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2024-05-06 18:17:15.000000 heartbeat_library-0.0.7/heartbeat_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 18:17:15.000000 heartbeat_library-0.0.7/heartbeat_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-06 18:02:12.000000 heartbeat_library-0.0.7/heartbeat_library.egg-info/requirements.txt
+-rw-rw-rw-   0        0        0       18 2024-05-06 18:17:15.000000 heartbeat_library-0.0.7/heartbeat_library.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 18:17:15.523853 heartbeat_library-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2024-05-06 18:17:13.000000 heartbeat_library-0.0.7/setup.py
```

### Comparing `heartbeat_library-0.0.6/LICENSE` & `heartbeat_library-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `heartbeat_library-0.0.6/PKG-INFO` & `heartbeat_library-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heartbeat-library
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library for sending pulses to a process monitoring server
 Author: Pedro Ferreira Braz
 Author-email: pbraz.pedrof@gmail.com
 License: MIT License
 Keywords: heartbeat,heartbeat-library,heartbeat-api,heartbeat-wrapper,heartbeat-python,heartbeat-python-wrapper,heartbeat-python-api,heartbeat-python-wrapper-api,heartbeat-python-api-wrapper,multithreading,threading,requests,python-requests,python-threading,python-multithreading,python-heartbeat,python-heartbeat-api,python-heartbeat-wrapper,python-heartbeat-python,python-heartbeat-python-wrapper,python-heartbeat-python-api,python-heartbeat-python-wrapper-api,python-heartbeat-python-api-wrapper
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `heartbeat_library-0.0.6/README.md` & `heartbeat_library-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `heartbeat_library-0.0.6/heartbeat-library/heartbeat_library.py` & `heartbeat_library-0.0.7/heartbeat-library/heartbeat_library.py`

 * *Files identical despite different names*

### Comparing `heartbeat_library-0.0.6/heartbeat_library.egg-info/PKG-INFO` & `heartbeat_library-0.0.7/heartbeat_library.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heartbeat-library
-Version: 0.0.6
+Version: 0.0.7
 Summary: Library for sending pulses to a process monitoring server
 Author: Pedro Ferreira Braz
 Author-email: pbraz.pedrof@gmail.com
 License: MIT License
 Keywords: heartbeat,heartbeat-library,heartbeat-api,heartbeat-wrapper,heartbeat-python,heartbeat-python-wrapper,heartbeat-python-api,heartbeat-python-wrapper-api,heartbeat-python-api-wrapper,multithreading,threading,requests,python-requests,python-threading,python-multithreading,python-heartbeat,python-heartbeat-api,python-heartbeat-wrapper,python-heartbeat-python,python-heartbeat-python-wrapper,python-heartbeat-python-api,python-heartbeat-python-wrapper-api,python-heartbeat-python-api-wrapper
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

