# Comparing `tmp/amebo-0.3.0.tar.gz` & `tmp/amebo-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amebo-0.3.0.tar", max compression
+gzip compressed data, was "amebo-0.3.1.tar", max compression
```

## Comparing `amebo-0.3.0.tar` & `amebo-0.3.1.tar`

### file list

```diff
@@ -1,4 +1,36 @@
--rw-r--r--   0        0        0     7394 2024-05-05 03:08:04.783226 amebo-0.3.0/README.md
--rw-r--r--   0        0        0     2564 2024-04-23 14:23:49.283283 amebo-0.3.0/amebo.py
--rw-r--r--   0        0        0      522 2024-05-06 10:59:02.487107 amebo-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8142 1970-01-01 00:00:00.000000 amebo-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     7394 2024-05-05 03:08:04.783226 amebo-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:19.995674 amebo-0.3.1/amebo/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:40:37.932901 amebo-0.3.1/amebo/constants/__init__.py
+-rw-r--r--   0        0        0      129 2024-04-23 10:53:18.032385 amebo-0.3.1/amebo/constants/literals.py
+-rw-r--r--   0        0        0     1955 2023-09-06 17:31:38.141358 amebo-0.3.1/amebo/constants/scripts.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:40:46.525615 amebo-0.3.1/amebo/controllers/__init__.py
+-rw-r--r--   0        0        0     2796 2024-05-06 11:48:00.171264 amebo-0.3.1/amebo/controllers/actions.py
+-rw-r--r--   0        0        0      412 2024-04-23 14:07:10.599429 amebo-0.3.1/amebo/controllers/app.py
+-rw-r--r--   0        0        0     3895 2024-05-06 11:48:58.620551 amebo-0.3.1/amebo/controllers/events.py
+-rw-r--r--   0        0        0     4558 2024-05-06 11:48:56.511645 amebo-0.3.1/amebo/controllers/gists.py
+-rw-r--r--   0        0        0     4971 2024-05-06 11:50:14.065121 amebo-0.3.1/amebo/controllers/microservices.py
+-rw-r--r--   0        0        0     2874 2024-05-06 11:50:26.656940 amebo-0.3.1/amebo/controllers/subscribers.py
+-rw-r--r--   0        0        0        0 2024-05-06 11:40:52.710933 amebo-0.3.1/amebo/decorators/__init__.py
+-rw-r--r--   0        0        0     1634 2024-05-06 11:50:33.529261 amebo-0.3.1/amebo/decorators/formatters.py
+-rw-r--r--   0        0        0     1899 2024-05-06 11:49:06.630283 amebo-0.3.1/amebo/decorators/providers.py
+-rw-r--r--   0        0        0      593 2024-04-23 10:39:57.541079 amebo-0.3.1/amebo/decorators/security.py
+-rw-r--r--   0        0        0     4196 2023-09-06 17:31:38.137961 amebo-0.3.1/amebo/dist/amebo-0.1.1-py3-none-any.whl
+-rw-r--r--   0        0        0     4013 2023-09-06 17:31:38.138160 amebo-0.3.1/amebo/dist/amebo-0.1.1.tar.gz
+-rw-r--r--   0        0        0     4258 2023-09-06 17:31:38.138307 amebo-0.3.1/amebo/dist/amebo-0.1.2-py3-none-any.whl
+-rw-r--r--   0        0        0     4068 2023-09-06 17:31:38.138496 amebo-0.3.1/amebo/dist/amebo-0.1.2.tar.gz
+-rw-r--r--   0        0        0     4931 2024-05-06 10:43:40.490726 amebo-0.3.1/amebo/dist/amebo-0.2.0-py3-none-any.whl
+-rw-r--r--   0        0        0     4509 2024-05-06 10:43:40.425293 amebo-0.3.1/amebo/dist/amebo-0.2.0.tar.gz
+-rw-r--r--   0        0        0     4936 2024-05-06 11:26:51.191205 amebo-0.3.1/amebo/dist/amebo-0.3.0-py3-none-any.whl
+-rw-r--r--   0        0        0     4514 2024-05-06 11:26:51.126554 amebo-0.3.1/amebo/dist/amebo-0.3.0.tar.gz
+-rw-r--r--   0        0        0        0 2024-05-06 11:41:02.497626 amebo-0.3.1/amebo/middlewares/__init__.py
+-rw-r--r--   0        0        0     1140 2024-05-06 11:50:53.774142 amebo-0.3.1/amebo/middlewares/database.py
+-rw-r--r--   0        0        0      604 2024-04-23 13:28:24.231735 amebo-0.3.1/amebo/middlewares/security.py
+-rw-r--r--   0        0        0      465 2024-04-23 13:24:59.563293 amebo-0.3.1/amebo/middlewares/setup.py
+-rw-r--r--   0        0        0      704 2024-04-23 10:51:13.107504 amebo-0.3.1/amebo/models/actions.py
+-rw-r--r--   0        0        0      726 2024-05-05 19:28:21.684796 amebo-0.3.1/amebo/models/events.py
+-rw-r--r--   0        0        0      793 2024-05-05 16:53:56.861747 amebo-0.3.1/amebo/models/microservices.py
+-rw-r--r--   0        0        0      553 2024-05-06 11:51:13.036509 amebo-0.3.1/amebo/models/subscribers.py
+-rw-r--r--   0        0        0     1261 2024-05-06 11:52:36.970476 amebo-0.3.1/amebo/utils/helpers.py
+-rw-r--r--   0        0        0     1161 2024-04-23 10:52:26.352293 amebo-0.3.1/amebo/utils/structs.py
+-rw-r--r--   0        0        0      522 2024-05-06 11:57:11.873112 amebo-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8142 1970-01-01 00:00:00.000000 amebo-0.3.1/PKG-INFO
```

### Comparing `amebo-0.3.0/README.md` & `amebo-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `amebo-0.3.0/pyproject.toml` & `amebo-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amebo"
-version = "0.3.0"
+version = "0.3.1"
 description = "HTTP Event Notifications Server - Asynchronous Communication Engine"
 authors = ["Tersoo"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `amebo-0.3.0/PKG-INFO` & `amebo-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amebo
-Version: 0.3.0
+Version: 0.3.1
 Summary: HTTP Event Notifications Server - Asynchronous Communication Engine
 License: MIT
 Author: Tersoo
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amebo Version: 0.3.0 Summary: HTTP Event
+Metadata-Version: 2.1 Name: amebo Version: 0.3.1 Summary: HTTP Event
 Notifications Server - Asynchronous Communication Engine License: MIT Author:
 Tersoo Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
 fastjsonschema (==2.19.1) Requires-Dist: httpx (==0.23.3) Requires-Dist: jinja2
 (==3.1.2) Requires-Dist: orjson (==3.8.9) Requires-Dist: pydantic (==1.10.7)
```

