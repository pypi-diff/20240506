# Comparing `tmp/aissemble_foundation_pdp_client_python-1.7.0.dev1714770285.tar.gz` & `tmp/aissemble_foundation_pdp_client_python-1.7.0.dev1714997815.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_foundation_pdp_client_python-1.7.0.dev1714770285.tar", max compression
+gzip compressed data, was "aissemble_foundation_pdp_client_python-1.7.0.dev1714997815.tar", max compression
```

## Comparing `aissemble_foundation_pdp_client_python-1.7.0.dev1714770285.tar` & `aissemble_foundation_pdp_client_python-1.7.0.dev1714997815.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     9580 2024-05-03 21:04:35.069823 aissemble_foundation_pdp_client_python-1.7.0.dev1714770285/LICENSE
--rw-r--r--   0        0        0      680 2024-05-03 20:59:00.678689 aissemble_foundation_pdp_client_python-1.7.0.dev1714770285/README.md
--rw-r--r--   0        0        0      628 2024-05-03 21:04:46.009534 aissemble_foundation_pdp_client_python-1.7.0.dev1714770285/pyproject.toml
--rw-r--r--   0        0        0      228 2024-05-03 20:59:00.678689 aissemble_foundation_pdp_client_python-1.7.0.dev1714770285/src/aiops_security/__init__.py
--rw-r--r--   0        0        0      951 2024-05-03 20:59:00.678689 aissemble_foundation_pdp_client_python-1.7.0.dev1714770285/src/aiops_security/pdp_client.py
--rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 aissemble_foundation_pdp_client_python-1.7.0.dev1714770285/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-06 12:16:45.683193 aissemble_foundation_pdp_client_python-1.7.0.dev1714997815/LICENSE
+-rw-r--r--   0        0        0      680 2024-05-06 12:10:56.992644 aissemble_foundation_pdp_client_python-1.7.0.dev1714997815/README.md
+-rw-r--r--   0        0        0      628 2024-05-06 12:16:56.262906 aissemble_foundation_pdp_client_python-1.7.0.dev1714997815/pyproject.toml
+-rw-r--r--   0        0        0      228 2024-05-06 12:10:56.992644 aissemble_foundation_pdp_client_python-1.7.0.dev1714997815/src/aiops_security/__init__.py
+-rw-r--r--   0        0        0      951 2024-05-06 12:10:56.992644 aissemble_foundation_pdp_client_python-1.7.0.dev1714997815/src/aiops_security/pdp_client.py
+-rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 aissemble_foundation_pdp_client_python-1.7.0.dev1714997815/PKG-INFO
```

### Comparing `aissemble_foundation_pdp_client_python-1.7.0.dev1714770285/LICENSE` & `aissemble_foundation_pdp_client_python-1.7.0.dev1714997815/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_pdp_client_python-1.7.0.dev1714770285/README.md` & `aissemble_foundation_pdp_client_python-1.7.0.dev1714997815/README.md`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_pdp_client_python-1.7.0.dev1714770285/pyproject.toml` & `aissemble_foundation_pdp_client_python-1.7.0.dev1714997815/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aissemble-foundation-pdp-client-python"
-version = "1.7.0.dev1714770285"
+version = "1.7.0.dev1714997815"
 description = "REST Policy Decision Point (PDP) client for Python-based components"
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 readme = "README.md"
 packages = [
     {include = "aiops_security", from = "src"}
 ]
```

### Comparing `aissemble_foundation_pdp_client_python-1.7.0.dev1714770285/src/aiops_security/pdp_client.py` & `aissemble_foundation_pdp_client_python-1.7.0.dev1714997815/src/aiops_security/pdp_client.py`

 * *Files identical despite different names*

### Comparing `aissemble_foundation_pdp_client_python-1.7.0.dev1714770285/PKG-INFO` & `aissemble_foundation_pdp_client_python-1.7.0.dev1714997815/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-foundation-pdp-client-python
-Version: 1.7.0.dev1714770285
+Version: 1.7.0.dev1714997815
 Summary: REST Policy Decision Point (PDP) client for Python-based components
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.26.0)
```

