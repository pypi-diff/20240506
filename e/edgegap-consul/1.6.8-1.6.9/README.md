# Comparing `tmp/edgegap_consul-1.6.8.tar.gz` & `tmp/edgegap_consul-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_consul-1.6.8.tar", max compression
+gzip compressed data, was "edgegap_consul-1.6.9.tar", max compression
```

## Comparing `edgegap_consul-1.6.8.tar` & `edgegap_consul-1.6.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1993 2024-05-04 02:09:59.782354 edgegap_consul-1.6.8/LICENSE
--rw-r--r--   0        0        0     2152 2024-05-04 02:09:59.782354 edgegap_consul-1.6.8/README.md
--rw-r--r--   0        0        0       17 2024-05-04 02:09:59.782354 edgegap_consul-1.6.8/edgegap_consul/BUILD
--rw-r--r--   0        0        0      341 2024-05-04 02:09:59.782354 edgegap_consul-1.6.8/edgegap_consul/__init__.py
--rw-r--r--   0        0        0     2257 2024-05-04 02:09:59.782354 edgegap_consul-1.6.8/edgegap_consul/_client.py
--rw-r--r--   0        0        0      399 2024-05-04 02:09:59.782354 edgegap_consul-1.6.8/edgegap_consul/_configuration.py
--rw-r--r--   0        0        0     1325 2024-05-04 02:09:59.782354 edgegap_consul-1.6.8/edgegap_consul/_factory.py
--rw-r--r--   0        0        0     1623 2024-05-04 02:09:59.782354 edgegap_consul-1.6.8/edgegap_consul/_reader.py
--rw-r--r--   0        0        0      720 2024-05-04 02:11:40.823171 edgegap_consul-1.6.8/pyproject.toml
--rw-r--r--   0        0        0     2778 1970-01-01 00:00:00.000000 edgegap_consul-1.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-06 20:24:27.581272 edgegap_consul-1.6.9/LICENSE
+-rw-r--r--   0        0        0     2152 2024-05-06 20:24:27.581272 edgegap_consul-1.6.9/README.md
+-rw-r--r--   0        0        0       17 2024-05-06 20:24:27.581272 edgegap_consul-1.6.9/edgegap_consul/BUILD
+-rw-r--r--   0        0        0      341 2024-05-06 20:24:27.581272 edgegap_consul-1.6.9/edgegap_consul/__init__.py
+-rw-r--r--   0        0        0     2257 2024-05-06 20:24:27.581272 edgegap_consul-1.6.9/edgegap_consul/_client.py
+-rw-r--r--   0        0        0      399 2024-05-06 20:24:27.581272 edgegap_consul-1.6.9/edgegap_consul/_configuration.py
+-rw-r--r--   0        0        0     1325 2024-05-06 20:24:27.581272 edgegap_consul-1.6.9/edgegap_consul/_factory.py
+-rw-r--r--   0        0        0     1623 2024-05-06 20:24:27.581272 edgegap_consul-1.6.9/edgegap_consul/_reader.py
+-rw-r--r--   0        0        0      720 2024-05-06 20:26:21.033919 edgegap_consul-1.6.9/pyproject.toml
+-rw-r--r--   0        0        0     2778 1970-01-01 00:00:00.000000 edgegap_consul-1.6.9/PKG-INFO
```

### Comparing `edgegap_consul-1.6.8/LICENSE` & `edgegap_consul-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.6.8/README.md` & `edgegap_consul-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.6.8/edgegap_consul/_client.py` & `edgegap_consul-1.6.9/edgegap_consul/_client.py`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.6.8/edgegap_consul/_factory.py` & `edgegap_consul-1.6.9/edgegap_consul/_factory.py`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.6.8/edgegap_consul/_reader.py` & `edgegap_consul-1.6.9/edgegap_consul/_reader.py`

 * *Files identical despite different names*

### Comparing `edgegap_consul-1.6.8/pyproject.toml` & `edgegap_consul-1.6.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-consul"
-version = "1.6.8"
+version = "1.6.9"
 description = "The Edgegap Consul library includes various tools and helpers for interacting with Consul. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = { version = "^3.9.5", extras = ["speedups"] }
```

### Comparing `edgegap_consul-1.6.8/PKG-INFO` & `edgegap_consul-1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-consul
-Version: 1.6.8
+Version: 1.6.9
 Summary: The Edgegap Consul library includes various tools and helpers for interacting with Consul. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

