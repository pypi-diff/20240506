# Comparing `tmp/app_server-0.9.8.tar.gz` & `tmp/app_server-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app_server-0.9.8.tar", last modified: Wed Nov 22 10:14:01 2023, max compression
+gzip compressed data, was "app_server-0.9.9.tar", last modified: Thu Jan 18 06:47:01 2024, max compression
```

## Comparing `app_server-0.9.8.tar` & `app_server-0.9.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 10:14:01.846865 app_server-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-22 10:13:54.000000 app_server-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2023-11-22 10:14:01.846865 app_server-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-11-22 10:13:54.000000 app_server-0.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-22 10:13:54.000000 app_server-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-11-22 10:14:01.846865 app_server-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-11-22 10:13:54.000000 app_server-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 10:14:01.838865 app_server-0.9.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 10:14:01.838865 app_server-0.9.8/src/app_server/
--rw-r--r--   0 runner    (1001) docker     (127)    14506 2023-11-22 10:13:54.000000 app_server-0.9.8/src/app_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 10:14:01.842865 app_server-0.9.8/src/app_server/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2023-11-22 10:13:54.000000 app_server-0.9.8/src/app_server/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-22 10:13:54.000000 app_server-0.9.8/src/app_server/storage/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 10:14:01.842865 app_server-0.9.8/src/app_server/storage/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 10:13:54.000000 app_server-0.9.8/src/app_server/storage/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2023-11-22 10:13:54.000000 app_server-0.9.8/src/app_server/storage/handlers/buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2023-11-22 10:13:54.000000 app_server-0.9.8/src/app_server/storage/handlers/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     9836 2023-11-22 10:13:54.000000 app_server-0.9.8/src/app_server/storage/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-11-22 10:13:54.000000 app_server-0.9.8/src/app_server/storage/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11007 2023-11-22 10:13:54.000000 app_server-0.9.8/src/app_server/storage/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 10:14:01.842865 app_server-0.9.8/src/app_server/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2023-11-22 10:13:54.000000 app_server-0.9.8/src/app_server/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 10:14:01.842865 app_server-0.9.8/src/app_server/tasks/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 10:13:54.000000 app_server-0.9.8/src/app_server/tasks/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63475 2023-11-22 10:13:54.000000 app_server-0.9.8/src/app_server/tasks/proto/cloudtasks_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    22213 2023-11-22 10:13:54.000000 app_server-0.9.8/src/app_server/tasks/proto/cloudtasks_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    32068 2023-11-22 10:13:54.000000 app_server-0.9.8/src/app_server/tasks/proto/queue_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    44125 2023-11-22 10:13:54.000000 app_server-0.9.8/src/app_server/tasks/proto/target_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    22177 2023-11-22 10:13:54.000000 app_server-0.9.8/src/app_server/tasks/proto/task_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19357 2023-11-22 10:13:54.000000 app_server-0.9.8/src/app_server/tasks/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 10:14:01.846865 app_server-0.9.8/src/app_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2023-11-22 10:14:01.000000 app_server-0.9.8/src/app_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      930 2023-11-22 10:14:01.000000 app_server-0.9.8/src/app_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-22 10:14:01.000000 app_server-0.9.8/src/app_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-11-22 10:14:01.000000 app_server-0.9.8/src/app_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-22 10:14:01.000000 app_server-0.9.8/src/app_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-22 10:14:01.000000 app_server-0.9.8/src/app_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 06:47:01.862007 app_server-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-18 06:46:54.000000 app_server-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-01-18 06:47:01.862007 app_server-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-01-18 06:46:54.000000 app_server-0.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-18 06:46:54.000000 app_server-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-01-18 06:47:01.862007 app_server-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-18 06:46:54.000000 app_server-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 06:47:01.854007 app_server-0.9.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 06:47:01.858007 app_server-0.9.9/src/app_server/
+-rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-01-18 06:46:54.000000 app_server-0.9.9/src/app_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 06:47:01.858007 app_server-0.9.9/src/app_server/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-01-18 06:46:54.000000 app_server-0.9.9/src/app_server/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-18 06:46:54.000000 app_server-0.9.9/src/app_server/storage/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 06:47:01.858007 app_server-0.9.9/src/app_server/storage/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 06:46:54.000000 app_server-0.9.9/src/app_server/storage/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-01-18 06:46:54.000000 app_server-0.9.9/src/app_server/storage/handlers/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-01-18 06:46:54.000000 app_server-0.9.9/src/app_server/storage/handlers/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-01-18 06:46:54.000000 app_server-0.9.9/src/app_server/storage/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-18 06:46:54.000000 app_server-0.9.9/src/app_server/storage/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-01-18 06:46:54.000000 app_server-0.9.9/src/app_server/storage/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 06:47:01.858007 app_server-0.9.9/src/app_server/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-01-18 06:46:54.000000 app_server-0.9.9/src/app_server/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 06:47:01.862007 app_server-0.9.9/src/app_server/tasks/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 06:46:54.000000 app_server-0.9.9/src/app_server/tasks/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63475 2024-01-18 06:46:54.000000 app_server-0.9.9/src/app_server/tasks/proto/cloudtasks_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22213 2024-01-18 06:46:54.000000 app_server-0.9.9/src/app_server/tasks/proto/cloudtasks_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32068 2024-01-18 06:46:54.000000 app_server-0.9.9/src/app_server/tasks/proto/queue_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44125 2024-01-18 06:46:54.000000 app_server-0.9.9/src/app_server/tasks/proto/target_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22177 2024-01-18 06:46:54.000000 app_server-0.9.9/src/app_server/tasks/proto/task_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19357 2024-01-18 06:46:54.000000 app_server-0.9.9/src/app_server/tasks/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 06:47:01.862007 app_server-0.9.9/src/app_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-01-18 06:47:01.000000 app_server-0.9.9/src/app_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-01-18 06:47:01.000000 app_server-0.9.9/src/app_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 06:47:01.000000 app_server-0.9.9/src/app_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-18 06:47:01.000000 app_server-0.9.9/src/app_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-18 06:47:01.000000 app_server-0.9.9/src/app_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-18 06:47:01.000000 app_server-0.9.9/src/app_server.egg-info/top_level.txt
```

### Comparing `app_server-0.9.8/LICENSE` & `app_server-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `app_server-0.9.8/PKG-INFO` & `app_server-0.9.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: app_server
-Version: 0.9.8
+Version: 0.9.9
 Summary: a lightweight web application launcher for gunicorn and static files.
-Home-page: https://github.com/XeoN-GHMB/app_server
+Home-page: https://github.com/viur-framework/viur-app_server
 Author: Andreas H. Kelch
 Author-email: ak@mausbrand.de
-Project-URL: Bug Tracker, https://github.com/XeoN-GHMB/app_server/issues
+Project-URL: Bug Tracker, https://github.com/viur-framework/viur-app_server/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: werkzeug==2.3.7
-Requires-Dist: pyyaml==6.0
-Requires-Dist: gunicorn==21.2.0
-Requires-Dist: fs==2.4.16
-Requires-Dist: grpcio==1.58.0
+Requires-Dist: werkzeug~=2.3.7
+Requires-Dist: pyyaml~=6.0
+Requires-Dist: gunicorn~=21.2.0
+Requires-Dist: fs~=2.4.16
+Requires-Dist: grpcio>=1.58.0
 
 ## App Server
 The App Server project allows to start a gunicorn server to deliver application logic. Which is wrapped by a [werkzeug](https://werkzeug.palletsprojects.com/) server to deliver staticfiles. 
 Primarily the App Server is used as a lightweight alternative to the [dev_appserver](https://cloud.google.com/appengine/docs/standard/python3/testing-and-deploying-your-app?hl=de#local-dev-server) for the google appengine build with python. 
 But all [gunicorn](https://gunicorn.org/) projects can be started with it. 
 The static paths are stored in an app.yaml as handlers and are therefore compatible to google appengine projects.
```

### Comparing `app_server-0.9.8/README.md` & `app_server-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `app_server-0.9.8/setup.cfg` & `app_server-0.9.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 name = app_server
 version = attr: app_server.__version__
 author = Andreas H. Kelch
 author_email = ak@mausbrand.de
 description = a lightweight web application launcher for gunicorn and static files.
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/XeoN-GHMB/app_server
+url = https://github.com/viur-framework/viur-app_server
 project_urls = 
-	Bug Tracker = https://github.com/XeoN-GHMB/app_server/issues
+	Bug Tracker = https://github.com/viur-framework/viur-app_server/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	werkzeug==2.3.7
-	pyyaml==6.0
-	gunicorn==21.2.0
-	fs==2.4.16
-	grpcio==1.58.0
+	werkzeug~=2.3.7
+	pyyaml~=6.0
+	gunicorn~=21.2.0
+	fs~=2.4.16
+	grpcio>=1.58.0
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	app_server = app_server:main
```

### Comparing `app_server-0.9.8/src/app_server/__init__.py` & `app_server-0.9.9/src/app_server/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from werkzeug.utils import get_content_type
 from werkzeug.http import http_date, is_resource_modified
 from werkzeug._internal import _logger
 from werkzeug.urls import uri_to_iri, url_unquote
 
 
 
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 subprocesses = []
 
 class myWSGIRequestHandler(WSGIRequestHandler):
     def log_date_time_string(self):
         """Return the current time formatted for logging."""
         now = time.time()
@@ -292,14 +292,16 @@
 
     entrypoint = entrypoint.split()
     if "--reload" not in entrypoint:
         entrypoint.insert(1, "--reload")
     if "--reuse-port" not in entrypoint:
         entrypoint.insert(1, "--reuse-port")
 
+    entrypoint.extend(["--timeout", str(args.timeout)])
+
     os.chdir(appFolder)
     subprocesses.append(subprocess.Popen(entrypoint))
     os.chdir(myFolder)
 
 def main():
     """main entrypoint
```

### Comparing `app_server-0.9.8/src/app_server/storage/__init__.py` & `app_server-0.9.9/src/app_server/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.8/src/app_server/storage/handlers/buckets.py` & `app_server-0.9.9/src/app_server/storage/handlers/buckets.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.8/src/app_server/storage/handlers/objects.py` & `app_server-0.9.9/src/app_server/storage/handlers/objects.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.8/src/app_server/storage/server.py` & `app_server-0.9.9/src/app_server/storage/server.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.8/src/app_server/storage/storage.py` & `app_server-0.9.9/src/app_server/storage/storage.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.8/src/app_server/tasks/__init__.py` & `app_server-0.9.9/src/app_server/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.8/src/app_server/tasks/proto/cloudtasks_pb2.py` & `app_server-0.9.9/src/app_server/tasks/proto/cloudtasks_pb2.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.8/src/app_server/tasks/proto/cloudtasks_pb2_grpc.py` & `app_server-0.9.9/src/app_server/tasks/proto/cloudtasks_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.8/src/app_server/tasks/proto/queue_pb2.py` & `app_server-0.9.9/src/app_server/tasks/proto/queue_pb2.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.8/src/app_server/tasks/proto/target_pb2.py` & `app_server-0.9.9/src/app_server/tasks/proto/target_pb2.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.8/src/app_server/tasks/proto/task_pb2.py` & `app_server-0.9.9/src/app_server/tasks/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.8/src/app_server/tasks/server.py` & `app_server-0.9.9/src/app_server/tasks/server.py`

 * *Files identical despite different names*

### Comparing `app_server-0.9.8/src/app_server.egg-info/PKG-INFO` & `app_server-0.9.9/src/app_server.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
-Name: app-server
-Version: 0.9.8
+Name: app_server
+Version: 0.9.9
 Summary: a lightweight web application launcher for gunicorn and static files.
-Home-page: https://github.com/XeoN-GHMB/app_server
+Home-page: https://github.com/viur-framework/viur-app_server
 Author: Andreas H. Kelch
 Author-email: ak@mausbrand.de
-Project-URL: Bug Tracker, https://github.com/XeoN-GHMB/app_server/issues
+Project-URL: Bug Tracker, https://github.com/viur-framework/viur-app_server/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: werkzeug==2.3.7
-Requires-Dist: pyyaml==6.0
-Requires-Dist: gunicorn==21.2.0
-Requires-Dist: fs==2.4.16
-Requires-Dist: grpcio==1.58.0
+Requires-Dist: werkzeug~=2.3.7
+Requires-Dist: pyyaml~=6.0
+Requires-Dist: gunicorn~=21.2.0
+Requires-Dist: fs~=2.4.16
+Requires-Dist: grpcio>=1.58.0
 
 ## App Server
 The App Server project allows to start a gunicorn server to deliver application logic. Which is wrapped by a [werkzeug](https://werkzeug.palletsprojects.com/) server to deliver staticfiles. 
 Primarily the App Server is used as a lightweight alternative to the [dev_appserver](https://cloud.google.com/appengine/docs/standard/python3/testing-and-deploying-your-app?hl=de#local-dev-server) for the google appengine build with python. 
 But all [gunicorn](https://gunicorn.org/) projects can be started with it. 
 The static paths are stored in an app.yaml as handlers and are therefore compatible to google appengine projects.
```

### Comparing `app_server-0.9.8/src/app_server.egg-info/SOURCES.txt` & `app_server-0.9.9/src/app_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

