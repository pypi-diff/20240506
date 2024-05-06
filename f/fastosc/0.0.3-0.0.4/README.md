# Comparing `tmp/fastosc-0.0.3.tar.gz` & `tmp/fastosc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sahlen/repositories/oslo1989/fastosc/dist/.tmp-3wowlisi/fastosc-0.0.3.tar", last modified: Sun May  5 19:25:48 2024, max compression
+gzip compressed data, was "/Users/sahlen/repositories/oslo1989/fastosc/dist/.tmp-0y7tkrbr/fastosc-0.0.4.tar", last modified: Sun May  5 19:33:44 2024, max compression
```

## Comparing `fastosc-0.0.3.tar` & `fastosc-0.0.4.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/
--rw-r--r--   0 sahlen     (501) staff       (20)      611 2024-05-05 19:25:48.000000 fastosc-0.0.3/PKG-INFO
--rw-r--r--   0 sahlen     (501) staff       (20)      280 2024-05-05 12:26:24.000000 fastosc-0.0.3/README.md
--rw-r--r--   0 sahlen     (501) staff       (20)      978 2024-05-05 19:25:25.000000 fastosc-0.0.3/pyproject.toml
--rw-r--r--   0 sahlen     (501) staff       (20)       38 2024-05-05 19:25:48.000000 fastosc-0.0.3/setup.cfg
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc/
--rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-13 16:36:43.000000 fastosc-0.0.3/src/fastosc/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc/dispatcher/
--rw-r--r--   0 sahlen     (501) staff       (20)     5984 2024-05-05 18:52:23.000000 fastosc-0.0.3/src/fastosc/dispatcher/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      250 2024-01-20 18:33:22.000000 fastosc-0.0.3/src/fastosc/dispatcher/handler.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc/docs/
--rw-r--r--   0 sahlen     (501) staff       (20)      313 2024-01-20 18:35:02.000000 fastosc-0.0.3/src/fastosc/docs/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc/message/
--rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-13 21:23:05.000000 fastosc-0.0.3/src/fastosc/message/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9145 2024-01-20 16:18:06.000000 fastosc-0.0.3/src/fastosc/message/arg_value.py
--rw-r--r--   0 sahlen     (501) staff       (20)      457 2024-01-20 16:19:12.000000 fastosc-0.0.3/src/fastosc/message/convert.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3789 2024-05-05 18:52:23.000000 fastosc-0.0.3/src/fastosc/message/osc_bundle.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1979 2024-05-05 18:51:01.000000 fastosc-0.0.3/src/fastosc/message/osc_bundle_builder.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4812 2024-05-05 18:54:34.000000 fastosc-0.0.3/src/fastosc/message/osc_message.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7201 2024-05-05 18:52:23.000000 fastosc-0.0.3/src/fastosc/message/osc_message_builder.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc/message/parsing/
--rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-08 21:16:09.000000 fastosc-0.0.3/src/fastosc/message/parsing/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1871 2024-05-05 18:49:06.000000 fastosc-0.0.3/src/fastosc/message/parsing/ntp.py
--rw-r--r--   0 sahlen     (501) staff       (20)    15417 2024-05-05 18:52:23.000000 fastosc-0.0.3/src/fastosc/message/parsing/osc_types.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc/router/
--rw-r--r--   0 sahlen     (501) staff       (20)    11251 2024-05-05 18:52:23.000000 fastosc-0.0.3/src/fastosc/router/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc/server/
--rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-19 10:51:55.000000 fastosc-0.0.3/src/fastosc/server/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      450 2024-05-05 18:27:52.000000 fastosc-0.0.3/src/fastosc/server/dispatcher_server.py
--rw-r--r--   0 sahlen     (501) staff       (20)      964 2024-05-05 18:27:52.000000 fastosc-0.0.3/src/fastosc/server/server_base.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc/server/udp/
--rw-r--r--   0 sahlen     (501) staff       (20)     2657 2024-05-05 18:55:35.000000 fastosc-0.0.3/src/fastosc/server/udp/udp_pull_server.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1447 2024-01-19 14:04:48.000000 fastosc-0.0.3/src/fastosc/server/udp/udp_server_base.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc.egg-info/
--rw-r--r--   0 sahlen     (501) staff       (20)      611 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc.egg-info/PKG-INFO
--rw-r--r--   0 sahlen     (501) staff       (20)      872 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc.egg-info/SOURCES.txt
--rw-r--r--   0 sahlen     (501) staff       (20)        1 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc.egg-info/dependency_links.txt
--rw-r--r--   0 sahlen     (501) staff       (20)        8 2024-05-05 19:25:48.000000 fastosc-0.0.3/src/fastosc.egg-info/top_level.txt
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:33:44.000000 fastosc-0.0.4/
+-rw-r--r--   0 sahlen     (501) staff       (20)       23 2024-05-05 19:32:49.000000 fastosc-0.0.4/MANIFEST.in
+-rw-r--r--   0 sahlen     (501) staff       (20)      611 2024-05-05 19:33:44.000000 fastosc-0.0.4/PKG-INFO
+-rw-r--r--   0 sahlen     (501) staff       (20)      280 2024-05-05 12:26:24.000000 fastosc-0.0.4/README.md
+-rw-r--r--   0 sahlen     (501) staff       (20)      978 2024-05-05 19:33:34.000000 fastosc-0.0.4/pyproject.toml
+-rw-r--r--   0 sahlen     (501) staff       (20)       38 2024-05-05 19:33:44.000000 fastosc-0.0.4/setup.cfg
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:33:44.000000 fastosc-0.0.4/src/
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:33:44.000000 fastosc-0.0.4/src/fastosc/
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-13 16:36:43.000000 fastosc-0.0.4/src/fastosc/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:33:44.000000 fastosc-0.0.4/src/fastosc/dispatcher/
+-rw-r--r--   0 sahlen     (501) staff       (20)     5984 2024-05-05 18:52:23.000000 fastosc-0.0.4/src/fastosc/dispatcher/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      250 2024-01-20 18:33:22.000000 fastosc-0.0.4/src/fastosc/dispatcher/handler.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:33:44.000000 fastosc-0.0.4/src/fastosc/docs/
+-rw-r--r--   0 sahlen     (501) staff       (20)      313 2024-01-20 18:35:02.000000 fastosc-0.0.4/src/fastosc/docs/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:33:44.000000 fastosc-0.0.4/src/fastosc/message/
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-13 21:23:05.000000 fastosc-0.0.4/src/fastosc/message/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9145 2024-01-20 16:18:06.000000 fastosc-0.0.4/src/fastosc/message/arg_value.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      457 2024-01-20 16:19:12.000000 fastosc-0.0.4/src/fastosc/message/convert.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3789 2024-05-05 18:52:23.000000 fastosc-0.0.4/src/fastosc/message/osc_bundle.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1979 2024-05-05 18:51:01.000000 fastosc-0.0.4/src/fastosc/message/osc_bundle_builder.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4812 2024-05-05 18:54:34.000000 fastosc-0.0.4/src/fastosc/message/osc_message.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7201 2024-05-05 18:52:23.000000 fastosc-0.0.4/src/fastosc/message/osc_message_builder.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:33:44.000000 fastosc-0.0.4/src/fastosc/message/parsing/
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-08 21:16:09.000000 fastosc-0.0.4/src/fastosc/message/parsing/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1871 2024-05-05 18:49:06.000000 fastosc-0.0.4/src/fastosc/message/parsing/ntp.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    15417 2024-05-05 18:52:23.000000 fastosc-0.0.4/src/fastosc/message/parsing/osc_types.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:32:58.000000 fastosc-0.0.4/src/fastosc/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:33:44.000000 fastosc-0.0.4/src/fastosc/router/
+-rw-r--r--   0 sahlen     (501) staff       (20)    11251 2024-05-05 18:52:23.000000 fastosc-0.0.4/src/fastosc/router/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:33:44.000000 fastosc-0.0.4/src/fastosc/server/
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-19 10:51:55.000000 fastosc-0.0.4/src/fastosc/server/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      450 2024-05-05 18:27:52.000000 fastosc-0.0.4/src/fastosc/server/dispatcher_server.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      964 2024-05-05 18:27:52.000000 fastosc-0.0.4/src/fastosc/server/server_base.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:33:44.000000 fastosc-0.0.4/src/fastosc/server/udp/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2657 2024-05-05 18:55:35.000000 fastosc-0.0.4/src/fastosc/server/udp/udp_pull_server.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1447 2024-01-19 14:04:48.000000 fastosc-0.0.4/src/fastosc/server/udp/udp_server_base.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:33:44.000000 fastosc-0.0.4/src/fastosc.egg-info/
+-rw-r--r--   0 sahlen     (501) staff       (20)      611 2024-05-05 19:33:44.000000 fastosc-0.0.4/src/fastosc.egg-info/PKG-INFO
+-rw-r--r--   0 sahlen     (501) staff       (20)      905 2024-05-05 19:33:44.000000 fastosc-0.0.4/src/fastosc.egg-info/SOURCES.txt
+-rw-r--r--   0 sahlen     (501) staff       (20)        1 2024-05-05 19:33:44.000000 fastosc-0.0.4/src/fastosc.egg-info/dependency_links.txt
+-rw-r--r--   0 sahlen     (501) staff       (20)        8 2024-05-05 19:33:44.000000 fastosc-0.0.4/src/fastosc.egg-info/top_level.txt
```

### Comparing `fastosc-0.0.3/PKG-INFO` & `fastosc-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastosc
-Version: 0.0.3
+Version: 0.0.4
 Summary: Modern Python Library for OSC, using best practices such as typing, linting/formatting - inspired by FastAPI
 Author-email: Martin Sahlen <martin8900@gmail.com>
 Project-URL: Homepage, https://github.com/oslo1989/fastosc
 Project-URL: Issues, https://github.com/oslo1989/fastosc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fastosc-0.0.3/pyproject.toml` & `fastosc-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools ~=68.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastosc"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     {name = "Martin Sahlen", email = "martin8900@gmail.com"}
 ]
 description = "Modern Python Library for OSC, using best practices such as typing, linting/formatting - inspired by FastAPI"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `fastosc-0.0.3/src/fastosc/dispatcher/__init__.py` & `fastosc-0.0.4/src/fastosc/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.3/src/fastosc/message/arg_value.py` & `fastosc-0.0.4/src/fastosc/message/arg_value.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.3/src/fastosc/message/osc_bundle.py` & `fastosc-0.0.4/src/fastosc/message/osc_bundle.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.3/src/fastosc/message/osc_bundle_builder.py` & `fastosc-0.0.4/src/fastosc/message/osc_bundle_builder.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.3/src/fastosc/message/osc_message.py` & `fastosc-0.0.4/src/fastosc/message/osc_message.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.3/src/fastosc/message/osc_message_builder.py` & `fastosc-0.0.4/src/fastosc/message/osc_message_builder.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.3/src/fastosc/message/parsing/ntp.py` & `fastosc-0.0.4/src/fastosc/message/parsing/ntp.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.3/src/fastosc/message/parsing/osc_types.py` & `fastosc-0.0.4/src/fastosc/message/parsing/osc_types.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.3/src/fastosc/router/__init__.py` & `fastosc-0.0.4/src/fastosc/router/__init__.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.3/src/fastosc/server/server_base.py` & `fastosc-0.0.4/src/fastosc/server/server_base.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.3/src/fastosc/server/udp/udp_pull_server.py` & `fastosc-0.0.4/src/fastosc/server/udp/udp_pull_server.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.3/src/fastosc/server/udp/udp_server_base.py` & `fastosc-0.0.4/src/fastosc/server/udp/udp_server_base.py`

 * *Files identical despite different names*

### Comparing `fastosc-0.0.3/src/fastosc.egg-info/PKG-INFO` & `fastosc-0.0.4/src/fastosc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastosc
-Version: 0.0.3
+Version: 0.0.4
 Summary: Modern Python Library for OSC, using best practices such as typing, linting/formatting - inspired by FastAPI
 Author-email: Martin Sahlen <martin8900@gmail.com>
 Project-URL: Homepage, https://github.com/oslo1989/fastosc
 Project-URL: Issues, https://github.com/oslo1989/fastosc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fastosc-0.0.3/src/fastosc.egg-info/SOURCES.txt` & `fastosc-0.0.4/src/fastosc.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+MANIFEST.in
 README.md
 pyproject.toml
 src/fastosc/__init__.py
+src/fastosc/py.typed
 src/fastosc.egg-info/PKG-INFO
 src/fastosc.egg-info/SOURCES.txt
 src/fastosc.egg-info/dependency_links.txt
 src/fastosc.egg-info/top_level.txt
 src/fastosc/dispatcher/__init__.py
 src/fastosc/dispatcher/handler.py
 src/fastosc/docs/__init__.py
```

