# Comparing `tmp/pytest_kookit-0.0.1.tar.gz` & `tmp/pytest_kookit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_kookit-0.0.1.tar", max compression
+gzip compressed data, was "pytest_kookit-0.0.2.tar", max compression
```

## Comparing `pytest_kookit-0.0.1.tar` & `pytest_kookit-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       54 2024-05-06 14:50:08.683302 pytest_kookit-0.0.1/README.md
--rw-r--r--   0        0        0       75 2023-11-06 13:41:07.948506 pytest_kookit-0.0.1/kookit/__init__.py
--rw-r--r--   0        0        0      214 2023-11-12 18:28:31.769606 pytest_kookit-0.0.1/kookit/http_models/__init__.py
--rw-r--r--   0        0        0      703 2023-11-09 17:45:27.482151 pytest_kookit-0.0.1/kookit/http_models/json_request.py
--rw-r--r--   0        0        0      575 2023-11-05 18:49:47.755140 pytest_kookit-0.0.1/kookit/http_models/json_response.py
--rw-r--r--   0        0        0     1508 2023-11-19 16:30:07.918932 pytest_kookit-0.0.1/kookit/http_models/request.py
--rw-r--r--   0        0        0     2381 2023-11-19 17:12:16.124553 pytest_kookit-0.0.1/kookit/http_models/response.py
--rw-r--r--   0        0        0      688 2023-11-12 18:28:34.204324 pytest_kookit-0.0.1/kookit/http_models/xml_response.py
--rw-r--r--   0        0        0      241 2023-11-19 15:35:09.982479 pytest_kookit-0.0.1/kookit/http_service/__init__.py
--rw-r--r--   0        0        0     1624 2023-11-19 16:34:30.896092 pytest_kookit-0.0.1/kookit/http_service/actions_parser.py
--rw-r--r--   0        0        0     3514 2023-11-19 17:18:34.236485 pytest_kookit-0.0.1/kookit/http_service/http_handler.py
--rw-r--r--   0        0        0     1216 2023-11-19 16:41:07.246600 pytest_kookit-0.0.1/kookit/http_service/interfaces.py
--rw-r--r--   0        0        0     2472 2023-11-19 17:17:29.161759 pytest_kookit-0.0.1/kookit/http_service/request_runner.py
--rw-r--r--   0        0        0     1329 2023-11-19 16:41:01.233034 pytest_kookit-0.0.1/kookit/http_service/requests_diff.py
--rw-r--r--   0        0        0     3244 2023-11-19 16:34:37.564876 pytest_kookit-0.0.1/kookit/http_service/service.py
--rw-r--r--   0        0        0      230 2023-11-06 18:56:26.540666 pytest_kookit-0.0.1/kookit/logging.py
--rw-r--r--   0        0        0       62 2023-11-10 17:05:20.824624 pytest_kookit-0.0.1/kookit/main/__init__.py
--rw-r--r--   0        0        0     1542 2023-11-06 13:18:56.655258 pytest_kookit-0.0.1/kookit/main/client_side.py
--rw-r--r--   0        0        0       68 2023-11-10 16:52:08.681070 pytest_kookit-0.0.1/kookit/main/http_kookit/__init__.py
--rw-r--r--   0        0        0      572 2023-11-10 16:51:08.309827 pytest_kookit-0.0.1/kookit/main/http_kookit/interfaces.py
--rw-r--r--   0        0        0     3416 2023-11-10 17:03:35.550575 pytest_kookit-0.0.1/kookit/main/http_kookit/kookit.py
--rw-r--r--   0        0        0      945 2023-11-10 16:16:39.938982 pytest_kookit-0.0.1/kookit/main/http_kookit/server.py
--rw-r--r--   0        0        0      435 2023-11-10 17:01:20.657362 pytest_kookit-0.0.1/kookit/main/interfaces.py
--rw-r--r--   0        0        0     2146 2023-11-12 19:22:29.082774 pytest_kookit-0.0.1/kookit/main/kookit.py
--rw-r--r--   0        0        0        0 2023-11-04 21:29:12.485907 pytest_kookit-0.0.1/kookit/py.typed
--rw-r--r--   0        0        0     3492 2024-05-06 14:25:54.392002 pytest_kookit-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 pytest_kookit-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/README.md
+-rw-r--r--   0        0        0       75 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_models/__init__.py
+-rw-r--r--   0        0        0      703 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_models/json_request.py
+-rw-r--r--   0        0        0      575 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_models/json_response.py
+-rw-r--r--   0        0        0     1508 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_models/request.py
+-rw-r--r--   0        0        0     2381 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_models/response.py
+-rw-r--r--   0        0        0      688 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_models/xml_response.py
+-rw-r--r--   0        0        0      241 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_service/__init__.py
+-rw-r--r--   0        0        0     1624 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_service/actions_parser.py
+-rw-r--r--   0        0        0     3514 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_service/http_handler.py
+-rw-r--r--   0        0        0     1216 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_service/interfaces.py
+-rw-r--r--   0        0        0     2472 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_service/request_runner.py
+-rw-r--r--   0        0        0     1329 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_service/requests_diff.py
+-rw-r--r--   0        0        0     3244 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/http_service/service.py
+-rw-r--r--   0        0        0      230 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/logging.py
+-rw-r--r--   0        0        0       62 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/main/__init__.py
+-rw-r--r--   0        0        0     1542 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/main/client_side.py
+-rw-r--r--   0        0        0       68 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/main/http_kookit/__init__.py
+-rw-r--r--   0        0        0      572 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/main/http_kookit/interfaces.py
+-rw-r--r--   0        0        0     3416 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/main/http_kookit/kookit.py
+-rw-r--r--   0        0        0      945 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/main/http_kookit/server.py
+-rw-r--r--   0        0        0      435 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/main/interfaces.py
+-rw-r--r--   0        0        0     2146 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/main/kookit.py
+-rw-r--r--   0        0        0        0 2024-05-06 14:56:54.690275 pytest_kookit-0.0.2/kookit/py.typed
+-rw-r--r--   0        0        0     3492 2024-05-06 14:56:54.694275 pytest_kookit-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 pytest_kookit-0.0.2/PKG-INFO
```

### Comparing `pytest_kookit-0.0.1/kookit/http_models/json_request.py` & `pytest_kookit-0.0.2/kookit/http_models/json_request.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.0.1/kookit/http_models/json_response.py` & `pytest_kookit-0.0.2/kookit/http_models/json_response.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.0.1/kookit/http_models/request.py` & `pytest_kookit-0.0.2/kookit/http_models/request.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.0.1/kookit/http_models/response.py` & `pytest_kookit-0.0.2/kookit/http_models/response.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.0.1/kookit/http_models/xml_response.py` & `pytest_kookit-0.0.2/kookit/http_models/xml_response.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.0.1/kookit/http_service/actions_parser.py` & `pytest_kookit-0.0.2/kookit/http_service/actions_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.0.1/kookit/http_service/http_handler.py` & `pytest_kookit-0.0.2/kookit/http_service/http_handler.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.0.1/kookit/http_service/interfaces.py` & `pytest_kookit-0.0.2/kookit/http_service/interfaces.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.0.1/kookit/http_service/request_runner.py` & `pytest_kookit-0.0.2/kookit/http_service/request_runner.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.0.1/kookit/http_service/requests_diff.py` & `pytest_kookit-0.0.2/kookit/http_service/requests_diff.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.0.1/kookit/http_service/service.py` & `pytest_kookit-0.0.2/kookit/http_service/service.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.0.1/kookit/main/client_side.py` & `pytest_kookit-0.0.2/kookit/main/client_side.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.0.1/kookit/main/http_kookit/interfaces.py` & `pytest_kookit-0.0.2/kookit/main/http_kookit/interfaces.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.0.1/kookit/main/http_kookit/kookit.py` & `pytest_kookit-0.0.2/kookit/main/http_kookit/kookit.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.0.1/kookit/main/http_kookit/server.py` & `pytest_kookit-0.0.2/kookit/main/http_kookit/server.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.0.1/kookit/main/kookit.py` & `pytest_kookit-0.0.2/kookit/main/kookit.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.0.1/pyproject.toml` & `pytest_kookit-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 lines_after_imports = 2
 include_trailing_comma = true
 use_parentheses= true
 
 
 [tool.poetry]
 name = "pytest-kookit"
-version = "0.0.1"
+version = "0.0.2"
 description = "Your simple but kooky integration testing with pytest"
 readme = "README.md"
 license = "MIT"
 authors = ["Dmitry Makarov <mit.makaroff@gmail.com>"]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pytest_kookit-0.0.1/PKG-INFO` & `pytest_kookit-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-kookit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Your simple but kooky integration testing with pytest
 License: MIT
 Keywords: Integration Testing,External Services' mocks
 Author: Dmitry Makarov
 Author-email: mit.makaroff@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Intended Audience :: Developers
```

