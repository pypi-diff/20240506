# Comparing `tmp/verify4py-test1-1.0.2.tar.gz` & `tmp/verify4py-test1-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verify4py-test1-1.0.2.tar", last modified: Mon May  6 07:36:22 2024, max compression
+gzip compressed data, was "verify4py-test1-1.0.3.tar", last modified: Mon May  6 07:59:42 2024, max compression
```

## Comparing `verify4py-test1-1.0.2.tar` & `verify4py-test1-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 ulzisuren  (1000) ulzisuren  (1000)        0 2024-05-06 07:36:22.407030 verify4py-test1-1.0.2/
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     1065 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/LICENSE
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     9388 2024-05-06 07:36:22.407030 verify4py-test1-1.0.2/PKG-INFO
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     8817 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/README.md
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)       84 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/pyproject.toml
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)       38 2024-05-06 07:36:22.407030 verify4py-test1-1.0.2/setup.cfg
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)      885 2024-05-06 07:31:29.000000 verify4py-test1-1.0.2/setup.py
-drwxrwxr-x   0 ulzisuren  (1000) ulzisuren  (1000)        0 2024-05-06 07:36:22.407030 verify4py-test1-1.0.2/src/
-drwxrwxr-x   0 ulzisuren  (1000) ulzisuren  (1000)        0 2024-05-06 07:36:22.407030 verify4py-test1-1.0.2/src/verify4py/
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)    11193 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/Issuer.py
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     3509 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/JsonIssuer.py
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     2909 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/PdfIssuer.py
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     5441 2024-05-06 07:25:40.000000 verify4py-test1-1.0.2/src/verify4py/UniversityDiplomaIssuer.py
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)        0 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/__init__.py
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)    27300 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/certify_sc_utils.py
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     1067 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/json_utils.py
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)      689 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/pdf.py
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     2018 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/test_UniversityDiplomaIssuer.py
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)    29369 2024-05-06 07:04:21.000000 verify4py-test1-1.0.2/src/verify4py/university_abi.py
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     1526 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/utils.py
-drwxrwxr-x   0 ulzisuren  (1000) ulzisuren  (1000)        0 2024-05-06 07:36:22.407030 verify4py-test1-1.0.2/src/verify4py_test1.egg-info/
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     9388 2024-05-06 07:36:22.000000 verify4py-test1-1.0.2/src/verify4py_test1.egg-info/PKG-INFO
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)      585 2024-05-06 07:36:22.000000 verify4py-test1-1.0.2/src/verify4py_test1.egg-info/SOURCES.txt
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)        1 2024-05-06 07:36:22.000000 verify4py-test1-1.0.2/src/verify4py_test1.egg-info/dependency_links.txt
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)       23 2024-05-06 07:36:22.000000 verify4py-test1-1.0.2/src/verify4py_test1.egg-info/requires.txt
--rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)       10 2024-05-06 07:36:22.000000 verify4py-test1-1.0.2/src/verify4py_test1.egg-info/top_level.txt
+drwxrwxr-x   0 ulzisuren  (1000) ulzisuren  (1000)        0 2024-05-06 07:59:42.701578 verify4py-test1-1.0.3/
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     1065 2024-05-06 06:56:26.000000 verify4py-test1-1.0.3/LICENSE
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     9388 2024-05-06 07:59:42.701578 verify4py-test1-1.0.3/PKG-INFO
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     8817 2024-05-06 06:56:26.000000 verify4py-test1-1.0.3/README.md
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)       84 2024-05-06 06:56:26.000000 verify4py-test1-1.0.3/pyproject.toml
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)       38 2024-05-06 07:59:42.701578 verify4py-test1-1.0.3/setup.cfg
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)      885 2024-05-06 07:59:34.000000 verify4py-test1-1.0.3/setup.py
+drwxrwxr-x   0 ulzisuren  (1000) ulzisuren  (1000)        0 2024-05-06 07:59:42.701578 verify4py-test1-1.0.3/src/
+drwxrwxr-x   0 ulzisuren  (1000) ulzisuren  (1000)        0 2024-05-06 07:59:42.701578 verify4py-test1-1.0.3/src/verify4py/
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)    11193 2024-05-06 06:56:26.000000 verify4py-test1-1.0.3/src/verify4py/Issuer.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     3509 2024-05-06 06:56:26.000000 verify4py-test1-1.0.3/src/verify4py/JsonIssuer.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     2909 2024-05-06 06:56:26.000000 verify4py-test1-1.0.3/src/verify4py/PdfIssuer.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     6227 2024-05-06 07:54:38.000000 verify4py-test1-1.0.3/src/verify4py/UniversityDiplomaIssuer.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)        0 2024-05-06 06:56:26.000000 verify4py-test1-1.0.3/src/verify4py/__init__.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)    27300 2024-05-06 06:56:26.000000 verify4py-test1-1.0.3/src/verify4py/certify_sc_utils.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     1067 2024-05-06 06:56:26.000000 verify4py-test1-1.0.3/src/verify4py/json_utils.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)      689 2024-05-06 06:56:26.000000 verify4py-test1-1.0.3/src/verify4py/pdf.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     2018 2024-05-06 06:56:26.000000 verify4py-test1-1.0.3/src/verify4py/test_UniversityDiplomaIssuer.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)    29369 2024-05-06 07:04:21.000000 verify4py-test1-1.0.3/src/verify4py/university_abi.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     1526 2024-05-06 06:56:26.000000 verify4py-test1-1.0.3/src/verify4py/utils.py
+drwxrwxr-x   0 ulzisuren  (1000) ulzisuren  (1000)        0 2024-05-06 07:59:42.701578 verify4py-test1-1.0.3/src/verify4py_test1.egg-info/
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     9388 2024-05-06 07:59:42.000000 verify4py-test1-1.0.3/src/verify4py_test1.egg-info/PKG-INFO
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)      585 2024-05-06 07:59:42.000000 verify4py-test1-1.0.3/src/verify4py_test1.egg-info/SOURCES.txt
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)        1 2024-05-06 07:59:42.000000 verify4py-test1-1.0.3/src/verify4py_test1.egg-info/dependency_links.txt
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)       23 2024-05-06 07:59:42.000000 verify4py-test1-1.0.3/src/verify4py_test1.egg-info/requires.txt
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)       10 2024-05-06 07:59:42.000000 verify4py-test1-1.0.3/src/verify4py_test1.egg-info/top_level.txt
```

### Comparing `verify4py-test1-1.0.2/LICENSE` & `verify4py-test1-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.2/PKG-INFO` & `verify4py-test1-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verify4py-test1
-Version: 1.0.2
+Version: 1.0.3
 Summary: Issue certificates using blockchain and smart contract
 Home-page: https://github.com/teo-mn/verify4py
 Author: Surenbayar Doloonjin
 Author-email: surenbayar@corex.mn
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/teo-mn/verify4py/issues
 Platform: UNKNOWN
```

### Comparing `verify4py-test1-1.0.2/README.md` & `verify4py-test1-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.2/setup.py` & `verify4py-test1-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="verify4py-test1",
-    version="1.0.2",
+    version="1.0.3",
     author="Surenbayar Doloonjin",
     author_email="surenbayar@corex.mn",
     description="Issue certificates using blockchain and smart contract",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/teo-mn/verify4py",
     project_urls={
```

### Comparing `verify4py-test1-1.0.2/src/verify4py/Issuer.py` & `verify4py-test1-1.0.3/src/verify4py/Issuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.2/src/verify4py/JsonIssuer.py` & `verify4py-test1-1.0.3/src/verify4py/JsonIssuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.2/src/verify4py/PdfIssuer.py` & `verify4py-test1-1.0.3/src/verify4py/PdfIssuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.2/src/verify4py/UniversityDiplomaIssuer.py` & `verify4py-test1-1.0.3/src/verify4py/UniversityDiplomaIssuer.py`

 * *Files 13% similar despite different names*

```diff
@@ -120,9 +120,24 @@
         hash_val = Utils.calc_hash(file_path)
         pdf = PdfReader(file_path)
         metadata = pdf.Info.get('/verifymn')
         result = self.verify_root(hash_val.lower())
         result['metadata'] = metadata
         return result
 
-    def set_qr_code_data(self, cert_num: str, hash: str):
-        return self.__contract_instance.functions.setQrCodeData(cert_num, hash)
+    def set_qr_code_data(self, cert_num: str, hash: str, pk: str):
+        nonce = self.__client.eth.get_transaction_count(self.__client.to_checksum_address(self.issuer_address))
+        try:
+            func = self.__contract_instance.functions.setQrCodeData(cert_num, hash)
+
+            tx = func.build_transaction(
+                {'from': self.issuer_address, 'gasPrice': self.__client.to_wei('1000', 'gwei'),
+                 'nonce': nonce, 'gas': DEFAULT_GAS_LIMIT})
+            signed = self.__client.eth.account.sign_transaction(tx, pk)
+            tx_hash = self.__client.eth.send_raw_transaction(signed.rawTransaction)
+            tx_res = self.__client.eth.wait_for_transaction_receipt(tx_hash)
+            if tx_res.status == 1:
+                return self.__client.to_hex(tx_hash), None
+            return '', 'Failed on blockchain'
+        except Exception as e:
+            print(e)
+            return '', e
```

### Comparing `verify4py-test1-1.0.2/src/verify4py/certify_sc_utils.py` & `verify4py-test1-1.0.3/src/verify4py/certify_sc_utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.2/src/verify4py/json_utils.py` & `verify4py-test1-1.0.3/src/verify4py/json_utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.2/src/verify4py/pdf.py` & `verify4py-test1-1.0.3/src/verify4py/pdf.py`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.2/src/verify4py/test_UniversityDiplomaIssuer.py` & `verify4py-test1-1.0.3/src/verify4py/test_UniversityDiplomaIssuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.2/src/verify4py/university_abi.py` & `verify4py-test1-1.0.3/src/verify4py/university_abi.py`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.2/src/verify4py/utils.py` & `verify4py-test1-1.0.3/src/verify4py/utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.2/src/verify4py_test1.egg-info/PKG-INFO` & `verify4py-test1-1.0.3/src/verify4py_test1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verify4py-test1
-Version: 1.0.2
+Version: 1.0.3
 Summary: Issue certificates using blockchain and smart contract
 Home-page: https://github.com/teo-mn/verify4py
 Author: Surenbayar Doloonjin
 Author-email: surenbayar@corex.mn
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/teo-mn/verify4py/issues
 Platform: UNKNOWN
```

### Comparing `verify4py-test1-1.0.2/src/verify4py_test1.egg-info/SOURCES.txt` & `verify4py-test1-1.0.3/src/verify4py_test1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

