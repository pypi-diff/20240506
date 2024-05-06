# Comparing `tmp/azure-kusto-data-4.4.0.tar.gz` & `tmp/azure-kusto-data-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/azure-kusto-data-4.4.0.tar", last modified: Tue Apr  9 05:14:46 2024, max compression
+gzip compressed data, was "dist/azure-kusto-data-4.4.1.tar", last modified: Mon May  6 13:23:21 2024, max compression
```

## Comparing `azure-kusto-data-4.4.0.tar` & `azure-kusto-data-4.4.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure/kusto/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure/kusto/data/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/_cloud_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/_string_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    28110 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/_token_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure/kusto/data/aio/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/aio/_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/aio/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/aio/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16494 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/client_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/client_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/client_request_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/data_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/env_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    30943 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/kcsb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/kusto_trusted_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/security.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/azure/kusto/data/wellKnownKustoEndpoints.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure_kusto_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure_kusto_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure_kusto_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure_kusto_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure_kusto_data.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure_kusto_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/azure_kusto_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 05:14:46.000000 azure-kusto-data-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-09 05:14:33.000000 azure-kusto-data-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:23:21.000000 azure-kusto-data-4.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-06 13:23:21.000000 azure-kusto-data-4.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:23:21.000000 azure-kusto-data-4.4.1/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:23:21.000000 azure-kusto-data-4.4.1/azure/kusto/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:23:21.000000 azure-kusto-data-4.4.1/azure/kusto/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/_cloud_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/_string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28116 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/_token_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:23:21.000000 azure-kusto-data-4.4.1/azure/kusto/data/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/aio/_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/aio/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/aio/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16494 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/client_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/client_request_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/env_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30943 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/kcsb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/kusto_trusted_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/azure/kusto/data/wellKnownKustoEndpoints.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:23:21.000000 azure-kusto-data-4.4.1/azure_kusto_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-06 13:23:20.000000 azure-kusto-data-4.4.1/azure_kusto_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-06 13:23:21.000000 azure-kusto-data-4.4.1/azure_kusto_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:23:20.000000 azure-kusto-data-4.4.1/azure_kusto_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 13:23:20.000000 azure-kusto-data-4.4.1/azure_kusto_data.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-06 13:23:20.000000 azure-kusto-data-4.4.1/azure_kusto_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 13:23:20.000000 azure-kusto-data-4.4.1/azure_kusto_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-06 13:23:21.000000 azure-kusto-data-4.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-06 13:23:09.000000 azure-kusto-data-4.4.1/setup.py
```

### Comparing `azure-kusto-data-4.4.0/PKG-INFO` & `azure-kusto-data-4.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kusto-data
-Version: 4.4.0
+Version: 4.4.1
 Summary: Kusto Data Client
 Home-page: https://github.com/Azure/azure-kusto-python
 Author: Microsoft Corporation
 Author-email: kustalk@microsoft.com
 License: MIT
 Description: Microsoft Azure Kusto Library for Python
         ========================================
```

### Comparing `azure-kusto-data-4.4.0/README.rst` & `azure-kusto-data-4.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/_cloud_settings.py` & `azure-kusto-data-4.4.1/azure/kusto/data/_cloud_settings.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/_converters.py` & `azure-kusto-data-4.4.1/azure/kusto/data/_converters.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/_models.py` & `azure-kusto-data-4.4.1/azure/kusto/data/_models.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/_telemetry.py` & `azure-kusto-data-4.4.1/azure/kusto/data/_telemetry.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/_token_providers.py` & `azure-kusto-data-4.4.1/azure/kusto/data/_token_providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,15 @@
 
     def _get_token_from_cache_impl(self) -> Optional[dict]:
         return None
 
     def close(self):
         if self._msi_auth_context is not None:
             self._msi_auth_context.close()
-        if self._msi_auth_context is not None:
+        if self._msi_auth_context_async is not None:
             raise KustoAsyncUsageError("Can't close async token provider with sync close", self.is_async)
 
     async def close_async(self):
         if self._msi_auth_context is not None:
             await sync_to_async(self._msi_auth_context.close())
 
         if self._msi_auth_context_async is not None:
```

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/aio/_models.py` & `azure-kusto-data-4.4.1/azure/kusto/data/aio/_models.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/aio/client.py` & `azure-kusto-data-4.4.1/azure/kusto/data/aio/client.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/aio/response.py` & `azure-kusto-data-4.4.1/azure/kusto/data/aio/response.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/aio/streaming_response.py` & `azure-kusto-data-4.4.1/azure/kusto/data/aio/streaming_response.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/client.py` & `azure-kusto-data-4.4.1/azure/kusto/data/client.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/client_base.py` & `azure-kusto-data-4.4.1/azure/kusto/data/client_base.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/client_details.py` & `azure-kusto-data-4.4.1/azure/kusto/data/client_details.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/client_request_properties.py` & `azure-kusto-data-4.4.1/azure/kusto/data/client_request_properties.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/data_format.py` & `azure-kusto-data-4.4.1/azure/kusto/data/data_format.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/env_utils.py` & `azure-kusto-data-4.4.1/azure/kusto/data/env_utils.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/exceptions.py` & `azure-kusto-data-4.4.1/azure/kusto/data/exceptions.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/helpers.py` & `azure-kusto-data-4.4.1/azure/kusto/data/helpers.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/kcsb.py` & `azure-kusto-data-4.4.1/azure/kusto/data/kcsb.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/kusto_trusted_endpoints.py` & `azure-kusto-data-4.4.1/azure/kusto/data/kusto_trusted_endpoints.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/response.py` & `azure-kusto-data-4.4.1/azure/kusto/data/response.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/security.py` & `azure-kusto-data-4.4.1/azure/kusto/data/security.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/streaming_response.py` & `azure-kusto-data-4.4.1/azure/kusto/data/streaming_response.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure/kusto/data/wellKnownKustoEndpoints.json` & `azure-kusto-data-4.4.1/azure/kusto/data/wellKnownKustoEndpoints.json`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/azure_kusto_data.egg-info/PKG-INFO` & `azure-kusto-data-4.4.1/azure_kusto_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kusto-data
-Version: 4.4.0
+Version: 4.4.1
 Summary: Kusto Data Client
 Home-page: https://github.com/Azure/azure-kusto-python
 Author: Microsoft Corporation
 Author-email: kustalk@microsoft.com
 License: MIT
 Description: Microsoft Azure Kusto Library for Python
         ========================================
```

### Comparing `azure-kusto-data-4.4.0/azure_kusto_data.egg-info/SOURCES.txt` & `azure-kusto-data-4.4.1/azure_kusto_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-kusto-data-4.4.0/setup.py` & `azure-kusto-data-4.4.1/setup.py`

 * *Files identical despite different names*

