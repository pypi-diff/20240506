# Comparing `tmp/kv_azure_blob-0.1.0.tar.gz` & `tmp/kv_azure_blob-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_azure_blob-0.1.0.tar", last modified: Mon May  6 16:52:44 2024, max compression
+gzip compressed data, was "kv_azure_blob-0.1.1.tar", last modified: Mon May  6 16:53:41 2024, max compression
```

## Comparing `kv_azure_blob-0.1.0.tar` & `kv_azure_blob-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:52:44.213237 kv_azure_blob-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1056 2024-05-06 16:52:44.213237 kv_azure_blob-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      675 2024-05-06 16:51:57.000000 kv_azure_blob-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      593 2024-05-06 16:44:07.000000 kv_azure_blob-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-06 16:52:44.213237 kv_azure_blob-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:52:44.213237 kv_azure_blob-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:52:44.213237 kv_azure_blob-0.1.0/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:52:44.213237 kv_azure_blob-0.1.0/src/kv/azure/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:52:44.213237 kv_azure_blob-0.1.0/src/kv/azure/blob/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-06 16:43:59.000000 kv_azure_blob-0.1.0/src/kv/azure/blob/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2591 2024-05-06 16:48:46.000000 kv_azure_blob-0.1.0/src/kv/azure/blob/api.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:52:44.213237 kv_azure_blob-0.1.0/src/kv_azure_blob.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1056 2024-05-06 16:52:44.000000 kv_azure_blob-0.1.0/src/kv_azure_blob.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      283 2024-05-06 16:52:44.000000 kv_azure_blob-0.1.0/src/kv_azure_blob.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-06 16:52:44.000000 kv_azure_blob-0.1.0/src/kv_azure_blob.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-06 16:52:44.000000 kv_azure_blob-0.1.0/src/kv_azure_blob.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-06 16:52:44.000000 kv_azure_blob-0.1.0/src/kv_azure_blob.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:53:41.836157 kv_azure_blob-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1070 2024-05-06 16:53:41.836157 kv_azure_blob-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      689 2024-05-06 16:53:34.000000 kv_azure_blob-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      593 2024-05-06 16:53:39.000000 kv_azure_blob-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-06 16:53:41.836157 kv_azure_blob-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:53:41.826157 kv_azure_blob-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:53:41.826157 kv_azure_blob-0.1.1/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:53:41.826157 kv_azure_blob-0.1.1/src/kv/azure/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:53:41.826157 kv_azure_blob-0.1.1/src/kv/azure/blob/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-06 16:43:59.000000 kv_azure_blob-0.1.1/src/kv/azure/blob/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2591 2024-05-06 16:48:46.000000 kv_azure_blob-0.1.1/src/kv/azure/blob/api.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-06 16:53:41.836157 kv_azure_blob-0.1.1/src/kv_azure_blob.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1070 2024-05-06 16:53:41.000000 kv_azure_blob-0.1.1/src/kv_azure_blob.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      283 2024-05-06 16:53:41.000000 kv_azure_blob-0.1.1/src/kv_azure_blob.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-06 16:53:41.000000 kv_azure_blob-0.1.1/src/kv_azure_blob.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-06 16:53:41.000000 kv_azure_blob-0.1.1/src/kv_azure_blob.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-06 16:53:41.000000 kv_azure_blob-0.1.1/src/kv_azure_blob.egg-info/top_level.txt
```

### Comparing `kv_azure_blob-0.1.0/PKG-INFO` & `kv_azure_blob-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: kv-azure-blob
-Version: 0.1.0
+Version: 0.1.1
 Summary: KV API implementation on Azure Blob Storage
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: azure-storage-blob
 Requires-Dist: aiohttp
 Requires-Dist: haskellian
 
 # Key-Value: Azure Blob
 
-> Implementation of the `KV[T]` async Key-Value ABC, over HTTP
+> Implementation of the `KV[T]` async Key-Value ABC, over Azure Blob Storage
 
 ([`kv-api`]((https://pypi.org/project/kv-api/)))
 
 ```bash
 pip install kv-azure-blob
 ```
```

### Comparing `kv_azure_blob-0.1.0/pyproject.toml` & `kv_azure_blob-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-azure-blob"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "KV API implementation on Azure Blob Storage"
 dependencies = [
   "azure-storage-blob", "aiohttp", "haskellian"
 ]
```

### Comparing `kv_azure_blob-0.1.0/src/kv/azure/blob/api.py` & `kv_azure_blob-0.1.1/src/kv/azure/blob/api.py`

 * *Files identical despite different names*

### Comparing `kv_azure_blob-0.1.0/src/kv_azure_blob.egg-info/PKG-INFO` & `kv_azure_blob-0.1.1/src/kv_azure_blob.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: kv-azure-blob
-Version: 0.1.0
+Version: 0.1.1
 Summary: KV API implementation on Azure Blob Storage
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: azure-storage-blob
 Requires-Dist: aiohttp
 Requires-Dist: haskellian
 
 # Key-Value: Azure Blob
 
-> Implementation of the `KV[T]` async Key-Value ABC, over HTTP
+> Implementation of the `KV[T]` async Key-Value ABC, over Azure Blob Storage
 
 ([`kv-api`]((https://pypi.org/project/kv-api/)))
 
 ```bash
 pip install kv-azure-blob
 ```
```

