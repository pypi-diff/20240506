# Comparing `tmp/bol_sdk-0.1.0.tar.gz` & `tmp/bol_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bol_sdk-0.1.0.tar", max compression
+gzip compressed data, was "bol_sdk-0.1.1.tar", max compression
```

## Comparing `bol_sdk-0.1.0.tar` & `bol_sdk-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       45 2024-05-03 17:53:19.404594 bol_sdk-0.1.0/bol_SDK/__init__.py
--rw-r--r--   0        0        0      895 2024-05-06 09:27:23.359081 bol_sdk-0.1.0/bol_SDK/__main__.py
--rw-r--r--   0        0        0    15932 2024-05-06 09:27:23.357641 bol_sdk-0.1.0/bol_SDK/bol_SDK.py
--rw-r--r--   0        0        0       43 2024-05-03 17:53:19.405330 bol_sdk-0.1.0/bol_SDK/constants.py
--rw-r--r--   0        0        0      408 2024-05-06 09:23:44.574639 bol_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 bol_sdk-0.1.0/setup.py
--rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 bol_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       45 2024-05-03 17:53:19.404594 bol_sdk-0.1.1/bol_SDK/__init__.py
+-rw-r--r--   0        0        0      895 2024-05-06 09:27:23.359081 bol_sdk-0.1.1/bol_SDK/__main__.py
+-rw-r--r--   0        0        0    15932 2024-05-06 09:27:23.357641 bol_sdk-0.1.1/bol_SDK/bol_SDK.py
+-rw-r--r--   0        0        0       43 2024-05-03 17:53:19.405330 bol_sdk-0.1.1/bol_SDK/constants.py
+-rw-r--r--   0        0        0      407 2024-05-06 15:59:50.100580 bol_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 bol_sdk-0.1.1/setup.py
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 bol_sdk-0.1.1/PKG-INFO
```

### Comparing `bol_sdk-0.1.0/bol_SDK/__main__.py` & `bol_sdk-0.1.1/bol_SDK/__main__.py`

 * *Files identical despite different names*

### Comparing `bol_sdk-0.1.0/bol_SDK/bol_SDK.py` & `bol_sdk-0.1.1/bol_SDK/bol_SDK.py`

 * *Files identical despite different names*

### Comparing `bol_sdk-0.1.0/setup.py` & `bol_sdk-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 ['numpy>=1.23.1,<2.0.0',
  'pandas>=1.4.3,<2.0.0',
  'python-dotenv>=0.20.0,<0.21.0',
  'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'bol-sdk',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': 'None',
     'author': 'AyumiOsawa',
     'author_email': 'a.osawa1002@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

