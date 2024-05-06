# Comparing `tmp/truststore-0.9.0.tar.gz` & `tmp/truststore-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truststore-0.9.0.tar", last modified: Mon Apr 29 17:14:14 2024, max compression
+gzip compressed data, was "truststore-0.9.1.tar", last modified: Mon May  6 17:41:09 2024, max compression
```

## Comparing `truststore-0.9.0.tar` & `truststore-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1086 2024-04-29 17:14:14.000000 truststore-0.9.0/LICENSE
--rw-r--r--   0        0        0     3399 2024-04-29 17:14:14.000000 truststore-0.9.0/README.md
--rw-r--r--   0        0        0      639 2024-04-29 17:14:14.000000 truststore-0.9.0/docs/Makefile
--rw-r--r--   0        0        0      805 2024-04-29 17:14:14.000000 truststore-0.9.0/docs/make.bat
--rw-r--r--   0        0        0       31 2024-04-29 17:14:14.000000 truststore-0.9.0/docs/requirements.txt
--rw-r--r--   0        0        0      620 2024-04-29 17:14:14.000000 truststore-0.9.0/docs/source/conf.py
--rw-r--r--   0        0        0     6386 2024-04-29 17:14:14.000000 truststore-0.9.0/docs/source/index.md
--rw-r--r--   0        0        0     1389 2024-04-29 17:14:14.000000 truststore-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      403 2024-04-29 17:14:14.000000 truststore-0.9.0/src/truststore/__init__.py
--rw-r--r--   0        0        0    10325 2024-04-29 17:14:14.000000 truststore-0.9.0/src/truststore/_api.py
--rw-r--r--   0        0        0    17608 2024-04-29 17:14:14.000000 truststore-0.9.0/src/truststore/_macos.py
--rw-r--r--   0        0        0     2324 2024-04-29 17:14:14.000000 truststore-0.9.0/src/truststore/_openssl.py
--rw-r--r--   0        0        0     1130 2024-04-29 17:14:14.000000 truststore-0.9.0/src/truststore/_ssl_constants.py
--rw-r--r--   0        0        0    17891 2024-04-29 17:14:14.000000 truststore-0.9.0/src/truststore/_windows.py
--rw-r--r--   0        0        0        0 2024-04-29 17:14:14.000000 truststore-0.9.0/src/truststore/py.typed
--rw-r--r--   0        0        0      561 2024-04-29 17:14:14.000000 truststore-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0     5293 2024-04-29 17:14:14.000000 truststore-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0    13592 2024-04-29 17:14:14.000000 truststore-0.9.0/tests/test_api.py
--rw-r--r--   0        0        0     1288 2024-04-29 17:14:14.000000 truststore-0.9.0/tests/test_custom_ca.py
--rw-r--r--   0        0        0     3814 2024-04-29 17:14:14.000000 truststore-0.9.0/tests/test_inject.py
--rw-r--r--   0        0        0     1663 2024-04-29 17:14:14.000000 truststore-0.9.0/tests/test_sslcontext.py
--rw-r--r--   0        0        0     4490 1970-01-01 00:00:00.000000 truststore-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-06 17:41:09.000000 truststore-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3399 2024-05-06 17:41:09.000000 truststore-0.9.1/README.md
+-rw-r--r--   0        0        0      639 2024-05-06 17:41:09.000000 truststore-0.9.1/docs/Makefile
+-rw-r--r--   0        0        0      805 2024-05-06 17:41:09.000000 truststore-0.9.1/docs/make.bat
+-rw-r--r--   0        0        0       31 2024-05-06 17:41:09.000000 truststore-0.9.1/docs/requirements.txt
+-rw-r--r--   0        0        0      620 2024-05-06 17:41:09.000000 truststore-0.9.1/docs/source/conf.py
+-rw-r--r--   0        0        0     6386 2024-05-06 17:41:09.000000 truststore-0.9.1/docs/source/index.md
+-rw-r--r--   0        0        0     1389 2024-05-06 17:41:09.000000 truststore-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      403 2024-05-06 17:41:09.000000 truststore-0.9.1/src/truststore/__init__.py
+-rw-r--r--   0        0        0    10425 2024-05-06 17:41:09.000000 truststore-0.9.1/src/truststore/_api.py
+-rw-r--r--   0        0        0    17608 2024-05-06 17:41:09.000000 truststore-0.9.1/src/truststore/_macos.py
+-rw-r--r--   0        0        0     2324 2024-05-06 17:41:09.000000 truststore-0.9.1/src/truststore/_openssl.py
+-rw-r--r--   0        0        0     1130 2024-05-06 17:41:09.000000 truststore-0.9.1/src/truststore/_ssl_constants.py
+-rw-r--r--   0        0        0    17891 2024-05-06 17:41:09.000000 truststore-0.9.1/src/truststore/_windows.py
+-rw-r--r--   0        0        0        0 2024-05-06 17:41:09.000000 truststore-0.9.1/src/truststore/py.typed
+-rw-r--r--   0        0        0      561 2024-05-06 17:41:09.000000 truststore-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0     5293 2024-05-06 17:41:09.000000 truststore-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0    13592 2024-05-06 17:41:09.000000 truststore-0.9.1/tests/test_api.py
+-rw-r--r--   0        0        0     1288 2024-05-06 17:41:09.000000 truststore-0.9.1/tests/test_custom_ca.py
+-rw-r--r--   0        0        0     3814 2024-05-06 17:41:09.000000 truststore-0.9.1/tests/test_inject.py
+-rw-r--r--   0        0        0     1663 2024-05-06 17:41:09.000000 truststore-0.9.1/tests/test_sslcontext.py
+-rw-r--r--   0        0        0     4490 1970-01-01 00:00:00.000000 truststore-0.9.1/PKG-INFO
```

### Comparing `truststore-0.9.0/LICENSE` & `truststore-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `truststore-0.9.0/README.md` & `truststore-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `truststore-0.9.0/docs/Makefile` & `truststore-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `truststore-0.9.0/docs/make.bat` & `truststore-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `truststore-0.9.0/docs/source/conf.py` & `truststore-0.9.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `truststore-0.9.0/docs/source/index.md` & `truststore-0.9.1/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `truststore-0.9.0/pyproject.toml` & `truststore-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `truststore-0.9.0/src/truststore/_api.py` & `truststore-0.9.1/src/truststore/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import platform
 import socket
 import ssl
 import sys
 import typing
 
+import _ssl  # type: ignore[import-not-found]
+
 from ._ssl_constants import (
     _original_SSLContext,
     _original_super_SSLContext,
     _truststore_SSLContext_dunder_class,
     _truststore_SSLContext_super_class,
 )
 
@@ -275,18 +277,20 @@
 # Python 3.13+ makes get_unverified_chain() a public API that only returns DER
 # encoded certificates. We detect whether we need to call public_bytes() for 3.10->3.12
 # Pre-3.13 returned None instead of an empty list from get_unverified_chain()
 if sys.version_info >= (3, 13):
 
     def _get_unverified_chain_bytes(sslobj: ssl.SSLObject) -> list[bytes]:
         unverified_chain = sslobj.get_unverified_chain() or ()  # type: ignore[attr-defined]
-        return [cert for cert in unverified_chain]
+        return [
+            cert if isinstance(cert, bytes) else cert.public_bytes(_ssl.ENCODING_DER)
+            for cert in unverified_chain
+        ]
 
 else:
-    import _ssl  # type: ignore[import-not-found]
 
     def _get_unverified_chain_bytes(sslobj: ssl.SSLObject) -> list[bytes]:
         unverified_chain = sslobj.get_unverified_chain() or ()  # type: ignore[attr-defined]
         return [cert.public_bytes(_ssl.ENCODING_DER) for cert in unverified_chain]
 
 
 def _verify_peercerts(
```

### Comparing `truststore-0.9.0/src/truststore/_macos.py` & `truststore-0.9.1/src/truststore/_macos.py`

 * *Files identical despite different names*

### Comparing `truststore-0.9.0/src/truststore/_openssl.py` & `truststore-0.9.1/src/truststore/_openssl.py`

 * *Files identical despite different names*

### Comparing `truststore-0.9.0/src/truststore/_ssl_constants.py` & `truststore-0.9.1/src/truststore/_ssl_constants.py`

 * *Files identical despite different names*

### Comparing `truststore-0.9.0/src/truststore/_windows.py` & `truststore-0.9.1/src/truststore/_windows.py`

 * *Files identical despite different names*

### Comparing `truststore-0.9.0/tests/__init__.py` & `truststore-0.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `truststore-0.9.0/tests/conftest.py` & `truststore-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `truststore-0.9.0/tests/test_api.py` & `truststore-0.9.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `truststore-0.9.0/tests/test_custom_ca.py` & `truststore-0.9.1/tests/test_custom_ca.py`

 * *Files identical despite different names*

### Comparing `truststore-0.9.0/tests/test_inject.py` & `truststore-0.9.1/tests/test_inject.py`

 * *Files identical despite different names*

### Comparing `truststore-0.9.0/tests/test_sslcontext.py` & `truststore-0.9.1/tests/test_sslcontext.py`

 * *Files identical despite different names*

### Comparing `truststore-0.9.0/PKG-INFO` & `truststore-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truststore
-Version: 0.9.0
+Version: 0.9.1
 Summary: Verify certificates using native system trust stores
 Author-email: Seth Michael Larson <sethmichaellarson@gmail.com>, David Glick <david@glicksoftware.com>
 Requires-Python: >= 3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

