# Comparing `tmp/mediaserver-api-client-4.3.tar.gz` & `tmp/mediaserver_api_client-4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediaserver-api-client-4.3.tar", last modified: Fri Feb  2 08:11:02 2024, max compression
+gzip compressed data, was "mediaserver_api_client-4.4.tar", last modified: Mon May  6 07:21:35 2024, max compression
```

## Comparing `mediaserver-api-client-4.3.tar` & `mediaserver_api_client-4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0     1000     1000        0 2024-02-02 08:11:02.281174 mediaserver-api-client-4.3/
--rw-rw-r--   0     1000     1000     7651 2018-01-16 07:32:19.000000 mediaserver-api-client-4.3/LICENSE
--rw-r--r--   0     1000     1000     7940 2024-02-02 08:11:02.281174 mediaserver-api-client-4.3/PKG-INFO
--rw-r--r--   0     1000     1000     6853 2023-03-08 14:36:31.000000 mediaserver-api-client-4.3/README.md
-drwxr-xr-x   0     1000     1000        0 2024-02-02 08:11:02.281174 mediaserver-api-client-4.3/mediaserver_api_client.egg-info/
--rw-r--r--   0     1000     1000     7940 2024-02-02 08:11:02.000000 mediaserver-api-client-4.3/mediaserver_api_client.egg-info/PKG-INFO
--rw-r--r--   0     1000     1000      479 2024-02-02 08:11:02.000000 mediaserver-api-client-4.3/mediaserver_api_client.egg-info/SOURCES.txt
--rw-r--r--   0     1000     1000        1 2024-02-02 08:11:02.000000 mediaserver-api-client-4.3/mediaserver_api_client.egg-info/dependency_links.txt
--rw-r--r--   0     1000     1000       55 2024-02-02 08:11:02.000000 mediaserver-api-client-4.3/mediaserver_api_client.egg-info/requires.txt
--rw-r--r--   0     1000     1000       10 2024-02-02 08:11:02.000000 mediaserver-api-client-4.3/mediaserver_api_client.egg-info/top_level.txt
-drwxr-xr-x   0     1000     1000        0 2024-02-02 08:11:02.277174 mediaserver-api-client-4.3/ms_client/
--rw-r--r--   0     1000     1000       20 2024-02-02 08:04:09.000000 mediaserver-api-client-4.3/ms_client/__init__.py
--rw-r--r--   0     1000     1000    12057 2023-05-09 09:19:38.000000 mediaserver-api-client-4.3/ms_client/client.py
--rw-r--r--   0     1000     1000     1411 2023-04-26 14:30:33.000000 mediaserver-api-client-4.3/ms_client/conf.py
-drwxr-xr-x   0     1000     1000        0 2024-02-02 08:11:02.277174 mediaserver-api-client-4.3/ms_client/lib/
--rw-r--r--   0     1000     1000        0 2019-05-24 10:00:59.000000 mediaserver-api-client-4.3/ms_client/lib/__init__.py
--rw-r--r--   0     1000     1000     4651 2023-03-08 09:51:11.000000 mediaserver-api-client-4.3/ms_client/lib/configuration.py
--rw-r--r--   0     1000     1000     3778 2023-05-09 09:28:06.000000 mediaserver-api-client-4.3/ms_client/lib/content.py
--rw-r--r--   0     1000     1000     9584 2023-07-18 09:12:31.000000 mediaserver-api-client-4.3/ms_client/lib/upload.py
--rw-r--r--   0     1000     1000     2036 2023-05-09 09:20:25.000000 mediaserver-api-client-4.3/ms_client/lib/users_csv.py
--rw-r--r--   0     1000     1000     1174 2024-02-02 08:11:02.281174 mediaserver-api-client-4.3/setup.cfg
--rwxr-xr-x   0     1000     1000       63 2019-05-23 14:56:48.000000 mediaserver-api-client-4.3/setup.py
-drwxr-xr-x   0     1000     1000        0 2024-02-02 08:11:02.281174 mediaserver-api-client-4.3/tests/
--rw-r--r--   0     1000     1000      943 2023-05-09 09:12:28.000000 mediaserver-api-client-4.3/tests/test_client.py
+drwxr-xr-x   0     1000     1000        0 2024-05-06 07:21:35.683555 mediaserver_api_client-4.4/
+-rw-rw-r--   0     1000     1000     7651 2018-01-16 07:32:19.000000 mediaserver_api_client-4.4/LICENSE
+-rw-r--r--   0     1000     1000     7940 2024-05-06 07:21:35.683555 mediaserver_api_client-4.4/PKG-INFO
+-rw-r--r--   0     1000     1000     6853 2023-03-08 14:36:31.000000 mediaserver_api_client-4.4/README.md
+drwxr-xr-x   0     1000     1000        0 2024-05-06 07:21:35.683555 mediaserver_api_client-4.4/mediaserver_api_client.egg-info/
+-rw-r--r--   0     1000     1000     7940 2024-05-06 07:21:35.000000 mediaserver_api_client-4.4/mediaserver_api_client.egg-info/PKG-INFO
+-rw-r--r--   0     1000     1000      479 2024-05-06 07:21:35.000000 mediaserver_api_client-4.4/mediaserver_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0     1000     1000        1 2024-05-06 07:21:35.000000 mediaserver_api_client-4.4/mediaserver_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0     1000     1000       55 2024-05-06 07:21:35.000000 mediaserver_api_client-4.4/mediaserver_api_client.egg-info/requires.txt
+-rw-r--r--   0     1000     1000       10 2024-05-06 07:21:35.000000 mediaserver_api_client-4.4/mediaserver_api_client.egg-info/top_level.txt
+drwxr-xr-x   0     1000     1000        0 2024-05-06 07:21:35.683555 mediaserver_api_client-4.4/ms_client/
+-rw-r--r--   0     1000     1000       20 2024-05-06 07:17:41.000000 mediaserver_api_client-4.4/ms_client/__init__.py
+-rw-r--r--   0     1000     1000    12204 2024-04-29 08:10:39.000000 mediaserver_api_client-4.4/ms_client/client.py
+-rw-r--r--   0     1000     1000     1553 2024-02-06 08:39:30.000000 mediaserver_api_client-4.4/ms_client/conf.py
+drwxr-xr-x   0     1000     1000        0 2024-05-06 07:21:35.683555 mediaserver_api_client-4.4/ms_client/lib/
+-rw-r--r--   0     1000     1000        0 2019-05-24 10:00:59.000000 mediaserver_api_client-4.4/ms_client/lib/__init__.py
+-rw-r--r--   0     1000     1000     4651 2023-03-08 09:51:11.000000 mediaserver_api_client-4.4/ms_client/lib/configuration.py
+-rw-r--r--   0     1000     1000     4984 2024-04-29 08:10:39.000000 mediaserver_api_client-4.4/ms_client/lib/content.py
+-rw-r--r--   0     1000     1000     9584 2023-07-18 09:12:31.000000 mediaserver_api_client-4.4/ms_client/lib/upload.py
+-rw-r--r--   0     1000     1000     2036 2023-05-09 09:20:25.000000 mediaserver_api_client-4.4/ms_client/lib/users_csv.py
+-rw-r--r--   0     1000     1000     1174 2024-05-06 07:21:35.683555 mediaserver_api_client-4.4/setup.cfg
+-rwxr-xr-x   0     1000     1000       63 2019-05-23 14:56:48.000000 mediaserver_api_client-4.4/setup.py
+drwxr-xr-x   0     1000     1000        0 2024-05-06 07:21:35.683555 mediaserver_api_client-4.4/tests/
+-rw-r--r--   0     1000     1000    12570 2024-04-29 08:10:39.000000 mediaserver_api_client-4.4/tests/test_client.py
```

### Comparing `mediaserver-api-client-4.3/LICENSE` & `mediaserver_api_client-4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mediaserver-api-client-4.3/PKG-INFO` & `mediaserver_api_client-4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediaserver-api-client
-Version: 4.3
+Version: 4.4
 Summary: A python3 reference implementation of an UbiCast MediaServer API client
 Home-page: https://www.ubicast.eu/en/solutions/delivery/
 Download-URL: https://github.com/UbiCastTeam/mediaserver-client
 Author: UbiCast
 Author-email: dev@ubicast.eu
 License: LGPLv3
 Keywords: api,client,mediaserver,nudgis,ubicast
```

### Comparing `mediaserver-api-client-4.3/README.md` & `mediaserver_api_client-4.4/README.md`

 * *Files identical despite different names*

### Comparing `mediaserver-api-client-4.3/mediaserver_api_client.egg-info/PKG-INFO` & `mediaserver_api_client-4.4/mediaserver_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediaserver-api-client
-Version: 4.3
+Version: 4.4
 Summary: A python3 reference implementation of an UbiCast MediaServer API client
 Home-page: https://www.ubicast.eu/en/solutions/delivery/
 Download-URL: https://github.com/UbiCastTeam/mediaserver-client
 Author: UbiCast
 Author-email: dev@ubicast.eu
 License: LGPLv3
 Keywords: api,client,mediaserver,nudgis,ubicast
```

### Comparing `mediaserver-api-client-4.3/ms_client/client.py` & `mediaserver_api_client-4.4/ms_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
 MediaServer client class
 
 Copyright 2019, Florent Thiery, Stéphane Diemer
 """
 from json import JSONDecodeError
 import logging
-import requests
 import time
+from typing import Literal
+
+import requests
+
 from .lib import configuration as configuration_lib
 from .lib import content as content_lib
 from .lib import upload as upload_lib
 from .lib import users_csv as users_csv_lib
 
 logger = logging.getLogger(__name__)
 
@@ -295,7 +298,10 @@
         return content_lib.download_metadata_zip(self, *args, **kwargs)
 
     def remove_all_content(self, *args, **kwargs):
         return content_lib.remove_all_content(self, *args, **kwargs)
 
     def import_users_csv(self, *args, **kwargs):
         return users_csv_lib.import_users_csv(self, *args, **kwargs)
+
+    def get_catalog(self, fmt=Literal['flat', 'tree', 'csv']):
+        return content_lib.get_catalog(self, fmt=fmt)
```

### Comparing `mediaserver-api-client-4.3/ms_client/conf.py` & `mediaserver_api_client-4.4/ms_client/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,8 +42,14 @@
     'PROXIES': None,
 
     # Chunk size for uploads (in bytes)
     'UPLOAD_CHUNK_SIZE': 26214400,
 
     # Maximum number of files per request
     'UPLOAD_MAX_FILES': 100,
+
+    # External SMTP server config
+    'SMTP_SERVER': None,
+    'SMTP_LOGIN': None,
+    'SMTP_PASSWORD': None,
+    'SMTP_SENDER_EMAIL': None,
 }
```

### Comparing `mediaserver-api-client-4.3/ms_client/lib/configuration.py` & `mediaserver_api_client-4.4/ms_client/lib/configuration.py`

 * *Files identical despite different names*

### Comparing `mediaserver-api-client-4.3/ms_client/lib/upload.py` & `mediaserver_api_client-4.4/ms_client/lib/upload.py`

 * *Files identical despite different names*

### Comparing `mediaserver-api-client-4.3/ms_client/lib/users_csv.py` & `mediaserver_api_client-4.4/ms_client/lib/users_csv.py`

 * *Files identical despite different names*

### Comparing `mediaserver-api-client-4.3/setup.cfg` & `mediaserver_api_client-4.4/setup.cfg`

 * *Files identical despite different names*

