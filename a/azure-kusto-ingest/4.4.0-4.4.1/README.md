# Comparing `tmp/azure-kusto-ingest-4.4.0.tar.gz` & `tmp/azure-kusto-ingest-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/azure-kusto-ingest-4.4.0.tar", last modified: Tue Apr  9 05:14:47 2024, max compression
+gzip compressed data, was "dist/azure-kusto-ingest-4.4.1.tar", last modified: Mon May  6 13:23:21 2024, max compression
```

## Comparing `azure-kusto-ingest-4.4.0.tar` & `azure-kusto-ingest-4.4.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure/kusto/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/_ingest_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/_ranked_storage_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/_resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/_status_q.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/_storage_account_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/_stream_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/base_ingest_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/ingest_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/ingestion_blob_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/ingestion_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/managed_streaming_ingest_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/azure/kusto/ingest/streaming_ingest_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 05:14:47.000000 azure-kusto-ingest-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-09 05:14:33.000000 azure-kusto-ingest-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:23:21.000000 azure-kusto-ingest-4.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-06 13:23:21.000000 azure-kusto-ingest-4.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:23:21.000000 azure-kusto-ingest-4.4.1/azure/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:23:21.000000 azure-kusto-ingest-4.4.1/azure/kusto/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:23:21.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/_ingest_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/_ranked_storage_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/_resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/_status_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/_storage_account_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/_stream_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7689 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/base_ingest_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/ingest_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/ingestion_blob_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/ingestion_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/managed_streaming_ingest_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/azure/kusto/ingest/streaming_ingest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:23:21.000000 azure-kusto-ingest-4.4.1/azure_kusto_ingest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-06 13:23:21.000000 azure-kusto-ingest-4.4.1/azure_kusto_ingest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-06 13:23:21.000000 azure-kusto-ingest-4.4.1/azure_kusto_ingest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:23:21.000000 azure-kusto-ingest-4.4.1/azure_kusto_ingest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 13:23:21.000000 azure-kusto-ingest-4.4.1/azure_kusto_ingest.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-06 13:23:21.000000 azure-kusto-ingest-4.4.1/azure_kusto_ingest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 13:23:21.000000 azure-kusto-ingest-4.4.1/azure_kusto_ingest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-06 13:23:21.000000 azure-kusto-ingest-4.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-06 13:23:09.000000 azure-kusto-ingest-4.4.1/setup.py
```

### Comparing `azure-kusto-ingest-4.4.0/PKG-INFO` & `azure-kusto-ingest-4.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kusto-ingest
-Version: 4.4.0
+Version: 4.4.1
 Summary: Kusto Ingest Client
 Home-page: https://github.com/Azure/azure-kusto-python
 Author: Microsoft Corporation
 Author-email: kustalk@microsoft.com
 License: MIT
 Description: Microsoft Azure Kusto Ingest Library for Python
         ===============================================
```

### Comparing `azure-kusto-ingest-4.4.0/README.rst` & `azure-kusto-ingest-4.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.4.0/azure/kusto/ingest/__init__.py` & `azure-kusto-ingest-4.4.1/azure/kusto/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.4.0/azure/kusto/ingest/_ingest_telemetry.py` & `azure-kusto-ingest-4.4.1/azure/kusto/ingest/_ingest_telemetry.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.4.0/azure/kusto/ingest/_ranked_storage_account.py` & `azure-kusto-ingest-4.4.1/azure/kusto/ingest/_ranked_storage_account.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.4.0/azure/kusto/ingest/_resource_manager.py` & `azure-kusto-ingest-4.4.1/azure/kusto/ingest/_resource_manager.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.4.0/azure/kusto/ingest/_status_q.py` & `azure-kusto-ingest-4.4.1/azure/kusto/ingest/_status_q.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.4.0/azure/kusto/ingest/_storage_account_set.py` & `azure-kusto-ingest-4.4.1/azure/kusto/ingest/_storage_account_set.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.4.0/azure/kusto/ingest/_stream_extensions.py` & `azure-kusto-ingest-4.4.1/azure/kusto/ingest/_stream_extensions.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.4.0/azure/kusto/ingest/base_ingest_client.py` & `azure-kusto-ingest-4.4.1/azure/kusto/ingest/base_ingest_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,17 +61,19 @@
         self.database = database
         self.table = table
         self.source_id = source_id
         self.blob_uri = blob_uri
 
     def __repr__(self):
         # Remove query parameters from blob_uri, if exists
+        obfuscated_path = None
         if isinstance(self.blob_uri, str):
             obfuscated_path = self.blob_uri.split("?")[0].split(";")[0]
-        return f"IngestionResult(status={self.status}, database={self.database}, table={self.table}, source_id={self.source_id}, blob_uri={obfuscated_path})"
+        blob_uri = f", obfuscated_blob_uri={obfuscated_path}" if obfuscated_path else ""
+        return f"IngestionResult(status={self.status}, database={self.database}, table={self.table}, source_id={self.source_id}{blob_uri})"
 
 
 class BaseIngestClient(metaclass=ABCMeta):
     def __init__(self):
         self._is_closed: bool = False
 
     def ingest_from_file(self, file_descriptor: Union[FileDescriptor, str], ingestion_properties: IngestionProperties) -> IngestionResult:
```

### Comparing `azure-kusto-ingest-4.4.0/azure/kusto/ingest/descriptors.py` & `azure-kusto-ingest-4.4.1/azure/kusto/ingest/descriptors.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.4.0/azure/kusto/ingest/exceptions.py` & `azure-kusto-ingest-4.4.1/azure/kusto/ingest/exceptions.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.4.0/azure/kusto/ingest/ingest_client.py` & `azure-kusto-ingest-4.4.1/azure/kusto/ingest/ingest_client.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.4.0/azure/kusto/ingest/ingestion_blob_info.py` & `azure-kusto-ingest-4.4.1/azure/kusto/ingest/ingestion_blob_info.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.4.0/azure/kusto/ingest/ingestion_properties.py` & `azure-kusto-ingest-4.4.1/azure/kusto/ingest/ingestion_properties.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.4.0/azure/kusto/ingest/managed_streaming_ingest_client.py` & `azure-kusto-ingest-4.4.1/azure/kusto/ingest/managed_streaming_ingest_client.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.4.0/azure/kusto/ingest/status.py` & `azure-kusto-ingest-4.4.1/azure/kusto/ingest/status.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.4.0/azure/kusto/ingest/streaming_ingest_client.py` & `azure-kusto-ingest-4.4.1/azure/kusto/ingest/streaming_ingest_client.py`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/PKG-INFO` & `azure-kusto-ingest-4.4.1/azure_kusto_ingest.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kusto-ingest
-Version: 4.4.0
+Version: 4.4.1
 Summary: Kusto Ingest Client
 Home-page: https://github.com/Azure/azure-kusto-python
 Author: Microsoft Corporation
 Author-email: kustalk@microsoft.com
 License: MIT
 Description: Microsoft Azure Kusto Ingest Library for Python
         ===============================================
```

### Comparing `azure-kusto-ingest-4.4.0/azure_kusto_ingest.egg-info/SOURCES.txt` & `azure-kusto-ingest-4.4.1/azure_kusto_ingest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-kusto-ingest-4.4.0/setup.py` & `azure-kusto-ingest-4.4.1/setup.py`

 * *Files identical despite different names*

