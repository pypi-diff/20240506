# Comparing `tmp/eapi_sdk-1.0.0.tar.gz` & `tmp/eapi_sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eapi_sdk-1.0.0.tar", last modified: Mon May  6 07:09:48 2024, max compression
+gzip compressed data, was "eapi_sdk-1.0.1.tar", last modified: Mon May  6 07:35:52 2024, max compression
```

## Comparing `eapi_sdk-1.0.0.tar` & `eapi_sdk-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 07:09:48.093708 eapi_sdk-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-05-06 07:09:48.090719 eapi_sdk-1.0.0/EAPI_SDK.egg-info/
--rw-rw-rw-   0        0        0      322 2024-05-06 07:09:47.000000 eapi_sdk-1.0.0/EAPI_SDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-05-06 07:09:47.000000 eapi_sdk-1.0.0/EAPI_SDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 07:09:47.000000 eapi_sdk-1.0.0/EAPI_SDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-06 07:09:47.000000 eapi_sdk-1.0.0/EAPI_SDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-06 07:09:47.000000 eapi_sdk-1.0.0/EAPI_SDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      322 2024-05-06 07:09:48.092712 eapi_sdk-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-22 12:47:14.000000 eapi_sdk-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 07:09:48.089722 eapi_sdk-1.0.0/eapi-sdk/
--rw-rw-rw-   0        0        0      501 2024-04-26 04:15:10.000000 eapi_sdk-1.0.0/eapi-sdk/__init__.py
--rw-rw-rw-   0        0        0     3303 2024-05-06 06:52:14.000000 eapi_sdk-1.0.0/eapi-sdk/client.py
--rw-rw-rw-   0        0        0     1524 2024-04-22 13:32:59.000000 eapi_sdk-1.0.0/eapi-sdk/exceptions.py
--rw-rw-rw-   0        0        0      434 2024-05-06 06:35:41.000000 eapi_sdk-1.0.0/eapi-sdk/main.py
--rw-rw-rw-   0        0        0      974 2024-04-22 13:03:17.000000 eapi_sdk-1.0.0/eapi-sdk/models.py
--rw-rw-rw-   0        0        0     1225 2024-04-22 13:10:59.000000 eapi_sdk-1.0.0/eapi-sdk/utils.py
--rw-rw-rw-   0        0        0     1091 2024-04-27 08:12:45.000000 eapi_sdk-1.0.0/licence.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 07:09:48.093708 eapi_sdk-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      415 2024-05-06 06:55:31.000000 eapi_sdk-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 07:35:52.440951 eapi_sdk-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-05-06 07:35:52.438958 eapi_sdk-1.0.1/EAPI_SDK.egg-info/
+-rw-rw-rw-   0        0        0      322 2024-05-06 07:35:52.000000 eapi_sdk-1.0.1/EAPI_SDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2024-05-06 07:35:52.000000 eapi_sdk-1.0.1/EAPI_SDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 07:35:52.000000 eapi_sdk-1.0.1/EAPI_SDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-06 07:35:52.000000 eapi_sdk-1.0.1/EAPI_SDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-06 07:35:52.000000 eapi_sdk-1.0.1/EAPI_SDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      322 2024-05-06 07:35:52.439955 eapi_sdk-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:47:14.000000 eapi_sdk-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 07:35:52.436964 eapi_sdk-1.0.1/eapisdk/
+-rw-rw-rw-   0        0        0      501 2024-04-26 04:15:10.000000 eapi_sdk-1.0.1/eapisdk/__init__.py
+-rw-rw-rw-   0        0        0     3303 2024-05-06 06:52:14.000000 eapi_sdk-1.0.1/eapisdk/client.py
+-rw-rw-rw-   0        0        0     1524 2024-04-22 13:32:59.000000 eapi_sdk-1.0.1/eapisdk/exceptions.py
+-rw-rw-rw-   0        0        0      434 2024-05-06 06:35:41.000000 eapi_sdk-1.0.1/eapisdk/main.py
+-rw-rw-rw-   0        0        0      974 2024-04-22 13:03:17.000000 eapi_sdk-1.0.1/eapisdk/models.py
+-rw-rw-rw-   0        0        0     1225 2024-04-22 13:10:59.000000 eapi_sdk-1.0.1/eapisdk/utils.py
+-rw-rw-rw-   0        0        0     1091 2024-04-27 08:12:45.000000 eapi_sdk-1.0.1/licence.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 07:35:52.440951 eapi_sdk-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      414 2024-05-06 07:35:48.000000 eapi_sdk-1.0.1/setup.py
```

### Comparing `eapi_sdk-1.0.0/eapi-sdk/client.py` & `eapi_sdk-1.0.1/eapisdk/client.py`

 * *Files identical despite different names*

### Comparing `eapi_sdk-1.0.0/eapi-sdk/exceptions.py` & `eapi_sdk-1.0.1/eapisdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `eapi_sdk-1.0.0/eapi-sdk/models.py` & `eapi_sdk-1.0.1/eapisdk/models.py`

 * *Files identical despite different names*

### Comparing `eapi_sdk-1.0.0/eapi-sdk/utils.py` & `eapi_sdk-1.0.1/eapisdk/utils.py`

 * *Files identical despite different names*

### Comparing `eapi_sdk-1.0.0/licence.txt` & `eapi_sdk-1.0.1/licence.txt`

 * *Files identical despite different names*

