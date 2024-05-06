# Comparing `tmp/verify4py-test1-1.0.1.tar.gz` & `tmp/verify4py-test1-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verify4py-test1-1.0.1.tar", last modified: Tue Jul 25 02:44:43 2023, max compression
+gzip compressed data, was "verify4py-test1-1.0.2.tar", last modified: Mon May  6 07:36:22 2024, max compression
```

## Comparing `verify4py-test1-1.0.1.tar` & `verify4py-test1-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 ulzisuren  (1000) ulzisuren  (1000)        0 2023-07-25 02:44:43.871928 verify4py-test1-1.0.1/
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)     1065 2023-07-20 08:00:54.000000 verify4py-test1-1.0.1/LICENSE
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)     9388 2023-07-25 02:44:43.871928 verify4py-test1-1.0.1/PKG-INFO
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)     8817 2023-07-21 04:13:37.000000 verify4py-test1-1.0.1/README.md
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)       84 2023-07-20 08:00:54.000000 verify4py-test1-1.0.1/pyproject.toml
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)       38 2023-07-25 02:44:43.871928 verify4py-test1-1.0.1/setup.cfg
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)      885 2023-07-25 02:43:26.000000 verify4py-test1-1.0.1/setup.py
-drwxr-xr-x   0 ulzisuren  (1000) ulzisuren  (1000)        0 2023-07-25 02:44:43.868594 verify4py-test1-1.0.1/src/
-drwxr-xr-x   0 ulzisuren  (1000) ulzisuren  (1000)        0 2023-07-25 02:44:43.871928 verify4py-test1-1.0.1/src/verify4py/
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)    10560 2023-07-25 02:40:01.000000 verify4py-test1-1.0.1/src/verify4py/Issuer.py
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)     3549 2023-07-25 02:38:29.000000 verify4py-test1-1.0.1/src/verify4py/JsonIssuer.py
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)     2909 2023-07-20 08:00:54.000000 verify4py-test1-1.0.1/src/verify4py/PdfIssuer.py
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)     3662 2023-07-20 08:00:54.000000 verify4py-test1-1.0.1/src/verify4py/UniversityDiplomaIssuer.py
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)        0 2023-07-20 08:00:54.000000 verify4py-test1-1.0.1/src/verify4py/__init__.py
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)    27300 2023-07-25 02:35:26.000000 verify4py-test1-1.0.1/src/verify4py/certify_sc_utils.py
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)     1067 2023-07-20 08:00:54.000000 verify4py-test1-1.0.1/src/verify4py/json_utils.py
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)      689 2023-07-20 08:00:54.000000 verify4py-test1-1.0.1/src/verify4py/pdf.py
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)    19898 2023-07-20 08:00:54.000000 verify4py-test1-1.0.1/src/verify4py/university_abi.py
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)     1526 2023-07-21 03:30:45.000000 verify4py-test1-1.0.1/src/verify4py/utils.py
-drwxr-xr-x   0 ulzisuren  (1000) ulzisuren  (1000)        0 2023-07-25 02:44:43.871928 verify4py-test1-1.0.1/src/verify4py_test1.egg-info/
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)     9388 2023-07-25 02:44:43.000000 verify4py-test1-1.0.1/src/verify4py_test1.egg-info/PKG-INFO
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)      539 2023-07-25 02:44:43.000000 verify4py-test1-1.0.1/src/verify4py_test1.egg-info/SOURCES.txt
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)        1 2023-07-25 02:44:43.000000 verify4py-test1-1.0.1/src/verify4py_test1.egg-info/dependency_links.txt
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)       23 2023-07-25 02:44:43.000000 verify4py-test1-1.0.1/src/verify4py_test1.egg-info/requires.txt
--rw-r--r--   0 ulzisuren  (1000) ulzisuren  (1000)       10 2023-07-25 02:44:43.000000 verify4py-test1-1.0.1/src/verify4py_test1.egg-info/top_level.txt
+drwxrwxr-x   0 ulzisuren  (1000) ulzisuren  (1000)        0 2024-05-06 07:36:22.407030 verify4py-test1-1.0.2/
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     1065 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/LICENSE
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     9388 2024-05-06 07:36:22.407030 verify4py-test1-1.0.2/PKG-INFO
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     8817 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/README.md
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)       84 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/pyproject.toml
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)       38 2024-05-06 07:36:22.407030 verify4py-test1-1.0.2/setup.cfg
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)      885 2024-05-06 07:31:29.000000 verify4py-test1-1.0.2/setup.py
+drwxrwxr-x   0 ulzisuren  (1000) ulzisuren  (1000)        0 2024-05-06 07:36:22.407030 verify4py-test1-1.0.2/src/
+drwxrwxr-x   0 ulzisuren  (1000) ulzisuren  (1000)        0 2024-05-06 07:36:22.407030 verify4py-test1-1.0.2/src/verify4py/
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)    11193 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/Issuer.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     3509 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/JsonIssuer.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     2909 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/PdfIssuer.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     5441 2024-05-06 07:25:40.000000 verify4py-test1-1.0.2/src/verify4py/UniversityDiplomaIssuer.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)        0 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/__init__.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)    27300 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/certify_sc_utils.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     1067 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/json_utils.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)      689 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/pdf.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     2018 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/test_UniversityDiplomaIssuer.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)    29369 2024-05-06 07:04:21.000000 verify4py-test1-1.0.2/src/verify4py/university_abi.py
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     1526 2024-05-06 06:56:26.000000 verify4py-test1-1.0.2/src/verify4py/utils.py
+drwxrwxr-x   0 ulzisuren  (1000) ulzisuren  (1000)        0 2024-05-06 07:36:22.407030 verify4py-test1-1.0.2/src/verify4py_test1.egg-info/
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)     9388 2024-05-06 07:36:22.000000 verify4py-test1-1.0.2/src/verify4py_test1.egg-info/PKG-INFO
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)      585 2024-05-06 07:36:22.000000 verify4py-test1-1.0.2/src/verify4py_test1.egg-info/SOURCES.txt
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)        1 2024-05-06 07:36:22.000000 verify4py-test1-1.0.2/src/verify4py_test1.egg-info/dependency_links.txt
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)       23 2024-05-06 07:36:22.000000 verify4py-test1-1.0.2/src/verify4py_test1.egg-info/requires.txt
+-rw-rw-r--   0 ulzisuren  (1000) ulzisuren  (1000)       10 2024-05-06 07:36:22.000000 verify4py-test1-1.0.2/src/verify4py_test1.egg-info/top_level.txt
```

### Comparing `verify4py-test1-1.0.1/LICENSE` & `verify4py-test1-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.1/PKG-INFO` & `verify4py-test1-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verify4py-test1
-Version: 1.0.1
+Version: 1.0.2
 Summary: Issue certificates using blockchain and smart contract
 Home-page: https://github.com/teo-mn/verify4py
 Author: Surenbayar Doloonjin
 Author-email: surenbayar@corex.mn
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/teo-mn/verify4py/issues
 Platform: UNKNOWN
```

### Comparing `verify4py-test1-1.0.1/README.md` & `verify4py-test1-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.1/setup.py` & `verify4py-test1-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="verify4py-test1",
-    version="1.0.1",
+    version="1.0.2",
     author="Surenbayar Doloonjin",
     author_email="surenbayar@corex.mn",
     description="Issue certificates using blockchain and smart contract",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/teo-mn/verify4py",
     project_urls={
```

### Comparing `verify4py-test1-1.0.1/src/verify4py/Issuer.py` & `verify4py-test1-1.0.2/src/verify4py/Issuer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import os
 import time
 
 from web3 import Web3
 from web3.auto import w3
 import verify4py.utils as Utils
 from verify4py.certify_sc_utils import abi as abi_cert
@@ -31,14 +30,20 @@
 
         if contract_type == 'university':
             abi = abi_univ
         else:
             abi = abi_cert
         self.__contract_instance = self.__client.eth.contract(address=self.smart_contract_address, abi=abi)
 
+    def get_client(self):
+        return self.__client
+
+    def get_contract_instance(self):
+        return self.__contract_instance
+
     def get_pk(self,
                private_key: str = "",
                key_store="",
                passphrase: str = ""):
         pk = private_key
         if private_key == "":
             if os.path.isdir(key_store):
@@ -56,53 +61,59 @@
               expire_date: int,
               desc: str,
               private_key: str = "",
               key_store="",
               passphrase: str = "",
               do_hash=False,
               hash_image: str = "",
-              hash_json: str = ""
+              hash_json: str = "",
+              signature: str = ""
               ):
         pk = self.get_pk(private_key, key_store, passphrase)
 
         # check credit
         if self.get_credit(self.issuer_address) == 0:
             raise ValueError("Not enough credit")
 
         cert = self.get_certificate(hash_value)
 
-        if cert.isRevoked:  # isRevoked flag
-            raise ValueError("Certificate revoked")
+        # if cert.isRevoked:  # isRevoked flag
+        #     raise ValueError("Certificate revoked")
 
-        if cert.id > 0:  # id
+        if cert.id > 0 and not cert.isRevoked:  # id
             raise ValueError("Certificate already registered")
 
         if self.is_duplicated_cert_num(cert_num=id):
             raise ValueError("Certificate number already registered")
 
         tx, error = self.__issue_util(hash_value, self.issuer_address, id, expire_date, VERSION, desc, pk,
-                                      hash_image, hash_json)
+                                      hash_image, hash_json, signature)
         if error is not None:
             print(error)
             raise RuntimeError(error)
             # insert proof
 
-
         return (tx, None), None
 
     def __issue_util(self, hash_value, issuer_address, cert_num, expire_date, version, desc, pk,
-                     hash_image="", hash_json=""):
+                     hash_image="", hash_json="", signature=""):
         nonce = self.__client.eth.get_transaction_count(self.__client.to_checksum_address(issuer_address))
         try:
             if self.contract_type == "":
                 func = self.__contract_instance.functions.addCertification(hash_value, cert_num, expire_date, version,
                                                                            desc)
             else:
-                func = self.__contract_instance.functions.addCertification(hash_value, hash_image, hash_json,
-                                                                           cert_num, expire_date, desc)
+                if signature == '':
+                    func = self.__contract_instance.functions.addCertification(hash_value, hash_image, hash_json,
+                                                                               cert_num, expire_date, desc)
+                else:
+                    func = self.__contract_instance.functions.addApprovedCertification(hash_value, hash_image,
+                                                                                       hash_json,
+                                                                                       cert_num, expire_date, desc,
+                                                                                       signature)
             tx = func.build_transaction(
                 {'from': issuer_address, 'gasPrice': self.__client.to_wei('1000', 'gwei'),
                  'nonce': nonce, 'gas': DEFAULT_GAS_LIMIT})
             signed = self.__client.eth.account.sign_transaction(tx, pk)
             tx_hash = self.__client.eth.send_raw_transaction(signed.rawTransaction)
             tx_res = self.__client.eth.wait_for_transaction_receipt(tx_hash)
             if tx_res.status == 1:
@@ -165,15 +176,14 @@
             if tx_res.status == 1:
                 return self.__client.to_hex(tx_hash), None
             return '', 'Failed on blockchain'
         except Exception as e:
             print(e)
             return '', e
 
-    # def verify_hash(self, hash_value, chainpoint_proof: str):
     def verify_hash(self, hash_value):
         self.verify_root(hash_value)
 
     def verify_root(self, hash):
         cert = self.get_certificate(hash)
         issuer = self.get_issuer(cert.issuer)
         state = 'ISSUED'
```

### Comparing `verify4py-test1-1.0.1/src/verify4py/JsonIssuer.py` & `verify4py-test1-1.0.2/src/verify4py/JsonIssuer.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,16 +52,15 @@
             }
         }
         f = open(source_file_path)
         json_data = json.load(f)
         json_data['verifymn'] = verifymn
         wrapped_json_str = json_wrap(json_data)
         hash_val = Utils.calc_hash_str(wrapped_json_str)
-        (tx, proof), error = self.issue(id, hash_val,
-                                        expire_date, desc, private_key, key_store, passphrase)
+        (tx, proof), error = self.issue(id, hash_val, expire_date, desc, private_key, key_store, passphrase)
         if error is None:
             verifymn['chainpointProof'] = proof
             json_data['verifymn'] = verifymn
             with open(destination_file_path, 'w') as f:
                 json.dump(json_data, f, indent=4)
         return tx, error
```

### Comparing `verify4py-test1-1.0.1/src/verify4py/PdfIssuer.py` & `verify4py-test1-1.0.2/src/verify4py/PdfIssuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.1/src/verify4py/UniversityDiplomaIssuer.py` & `verify4py-test1-1.0.2/src/verify4py/UniversityDiplomaIssuer.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 
 from pdfrw import PdfReader
 
 import verify4py.pdf as pdf_utils
 import verify4py.utils as Utils
 from verify4py.Issuer import Issuer
+from verify4py.certify_sc_utils import DEFAULT_GAS_LIMIT
 from verify4py.json_utils import json_wrap
 
 VERSION = 'v1.0-python-university'
 
 
 class UniversityDiplomaIssuer(Issuer):
     def __init__(self, smart_contract_address,
@@ -21,26 +22,21 @@
         super(UniversityDiplomaIssuer, self).__init__(smart_contract_address,
                                                       node_host, issuer_address,
                                                       issuer_name,
                                                       chain_id,
                                                       hash_type,
                                                       contract_type='university')
 
-    def issue_pdf(self,
-                  id: str,
-                  source_file_path: str,
-                  destination_file_path: str,
-                  meta_data: object,
-                  expire_date: int,
-                  desc: str,
-                  additional_info: str,
-                  private_key: str = "",
-                  key_store="",
-                  passphrase: str = ""):
-
+    def prepare_issue(self,
+                      id: str,
+                      source_file_path: str,
+                      destination_file_path: str,
+                      meta_data: object,
+                      desc: str,
+                      additional_info: str):
         verifymn = {
             "issuer": {
                 "name": self.issuer_name,
                 "address": self.issuer_address
             },
             "info": {
                 "name": self.issuer_name,
@@ -65,18 +61,52 @@
         pdf_utils.add_metadata(source_file_path, destination_file_path, verifymn=json.dumps(verifymn))
         hash_image = Utils.calc_hash(destination_file_path)
         verifymn['univ_meta'] = meta_data
         pdf_utils.add_metadata(source_file_path, destination_file_path, verifymn=json.dumps(verifymn))
         hash_val = Utils.calc_hash(destination_file_path)
         meta_str = json_wrap(meta_data)
         hash_meta = Utils.calc_hash_str(meta_str)
+        return hash_val, hash_meta, hash_image
+
+    def issue_pdf(self,
+                  id: str,
+                  source_file_path: str,
+                  destination_file_path: str,
+                  meta_data: object,
+                  expire_date: int,
+                  desc: str,
+                  additional_info: str,
+                  private_key: str = "",
+                  key_store="",
+                  passphrase: str = ""):
+
+        hash_val, hash_meta, hash_image = self.prepare_issue(id, source_file_path, destination_file_path,
+                                                             meta_data, desc, additional_info)
         (tx, proof), error = self.issue(id, hash_val, expire_date, desc, private_key, key_store, passphrase,
                                         hash_image=hash_image, hash_json=hash_meta)
         return tx, error
 
+    def issued_pdf_with_signature(self,
+                                  id: str,
+                                  source_file_path: str,
+                                  destination_file_path: str,
+                                  meta_data: object,
+                                  expire_date: int,
+                                  desc: str,
+                                  additional_info: str,
+                                  signature: str,
+                                  private_key: str = "",
+                                  key_store="",
+                                  passphrase: str = ""):
+        hash_val, hash_meta, hash_image = self.prepare_issue(id, source_file_path, destination_file_path,
+                                                             meta_data, desc, additional_info)
+        (tx, proof), error = self.issue(id, hash_val, expire_date, desc, private_key, key_store, passphrase,
+                                        hash_image=hash_image, hash_json=hash_meta, signature=signature)
+        return tx, error
+
     def revoke_pdf(self,
                    file_path: str,
                    revoker_name: str,
                    private_key: str = "",
                    key_store="",
                    passphrase: str = ""
                    ):
@@ -89,7 +119,10 @@
     def verify_pdf(self, file_path):
         hash_val = Utils.calc_hash(file_path)
         pdf = PdfReader(file_path)
         metadata = pdf.Info.get('/verifymn')
         result = self.verify_root(hash_val.lower())
         result['metadata'] = metadata
         return result
+
+    def set_qr_code_data(self, cert_num: str, hash: str):
+        return self.__contract_instance.functions.setQrCodeData(cert_num, hash)
```

### Comparing `verify4py-test1-1.0.1/src/verify4py/certify_sc_utils.py` & `verify4py-test1-1.0.2/src/verify4py/certify_sc_utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.1/src/verify4py/json_utils.py` & `verify4py-test1-1.0.2/src/verify4py/json_utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.1/src/verify4py/pdf.py` & `verify4py-test1-1.0.2/src/verify4py/pdf.py`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.1/src/verify4py/university_abi.py` & `verify4py-test1-1.0.2/src/verify4py/university_abi.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,973 +1,1107 @@
 abi = [
-  {
-    "anonymous": False,
-    "inputs": [
-      {
-        "indexed": False,
-        "internalType": "address",
+    {
+        "anonymous": False,
+        "inputs": [
+            {
+                "indexed": False,
+                "internalType": "address",
+                "name": "approver",
+                "type": "address"
+            },
+            {
+                "indexed": False,
+                "internalType": "string",
+                "name": "hash",
+                "type": "string"
+            },
+            {
+                "indexed": False,
+                "internalType": "string",
+                "name": "certNum",
+                "type": "string"
+            },
+            {
+                "indexed": False,
+                "internalType": "uint256",
+                "name": "timestamp",
+                "type": "uint256"
+            }
+        ],
+        "name": "Approved",
+        "type": "event"
+    },
+    {
+        "anonymous": False,
+        "inputs": [
+            {
+                "indexed": False,
+                "internalType": "address",
+                "name": "addr",
+                "type": "address"
+            }
+        ],
+        "name": "ApproverAddressAdded",
+        "type": "event"
+    },
+    {
+        "anonymous": False,
+        "inputs": [
+            {
+                "indexed": False,
+                "internalType": "address",
+                "name": "oldAddr",
+                "type": "address"
+            },
+            {
+                "indexed": False,
+                "internalType": "address",
+                "name": "newAddr",
+                "type": "address"
+            },
+            {
+                "indexed": False,
+                "internalType": "uint256",
+                "name": "timestamp",
+                "type": "uint256"
+            }
+        ],
+        "name": "ApproverAddressChanged",
+        "type": "event"
+    },
+    {
+        "anonymous": False,
+        "inputs": [
+            {
+                "indexed": False,
+                "internalType": "address",
+                "name": "addr",
+                "type": "address"
+            }
+        ],
+        "name": "ApproverAddressRemoved",
+        "type": "event"
+    },
+    {
+        "anonymous": False,
+        "inputs": [
+            {
+                "indexed": False,
+                "internalType": "address",
+                "name": "issuer",
+                "type": "address"
+            },
+            {
+                "indexed": False,
+                "internalType": "string",
+                "name": "hash",
+                "type": "string"
+            },
+            {
+                "indexed": False,
+                "internalType": "string",
+                "name": "metaHash",
+                "type": "string"
+            },
+            {
+                "indexed": False,
+                "internalType": "string",
+                "name": "certNum",
+                "type": "string"
+            },
+            {
+                "indexed": False,
+                "internalType": "uint256",
+                "name": "timestamp",
+                "type": "uint256"
+            }
+        ],
+        "name": "Issued",
+        "type": "event"
+    },
+    {
+        "anonymous": False,
+        "inputs": [
+            {
+                "indexed": False,
+                "internalType": "address",
+                "name": "oldAddr",
+                "type": "address"
+            },
+            {
+                "indexed": False,
+                "internalType": "address",
+                "name": "newAddr",
+                "type": "address"
+            },
+            {
+                "indexed": False,
+                "internalType": "uint256",
+                "name": "timestamp",
+                "type": "uint256"
+            }
+        ],
+        "name": "IssuerRegistrationAddressChanged",
+        "type": "event"
+    },
+    {
+        "anonymous": False,
+        "inputs": [
+            {
+                "indexed": True,
+                "internalType": "address",
+                "name": "previousOwner",
+                "type": "address"
+            },
+            {
+                "indexed": True,
+                "internalType": "address",
+                "name": "newOwner",
+                "type": "address"
+            }
+        ],
+        "name": "OwnershipTransferred",
+        "type": "event"
+    },
+    {
+        "anonymous": False,
+        "inputs": [
+            {
+                "indexed": False,
+                "internalType": "address",
+                "name": "revoker",
+                "type": "address"
+            },
+            {
+                "indexed": False,
+                "internalType": "string",
+                "name": "hash",
+                "type": "string"
+            },
+            {
+                "indexed": False,
+                "internalType": "string",
+                "name": "certNum",
+                "type": "string"
+            },
+            {
+                "indexed": False,
+                "internalType": "uint256",
+                "name": "timestamp",
+                "type": "uint256"
+            }
+        ],
+        "name": "Revoked",
+        "type": "event"
+    },
+    {
+        "anonymous": False,
+        "inputs": [
+            {
+                "indexed": False,
+                "internalType": "string",
+                "name": "certNum",
+                "type": "string"
+            },
+            {
+                "indexed": False,
+                "internalType": "string",
+                "name": "qrDataHash",
+                "type": "string"
+            }
+        ],
+        "name": "UpdatedQrCodeData",
+        "type": "event"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "_hash",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "_imageHash",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "_metaHash",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "_certNum",
+                "type": "string"
+            },
+            {
+                "internalType": "uint256",
+                "name": "_expireDate",
+                "type": "uint256"
+            },
+            {
+                "internalType": "string",
+                "name": "_desc",
+                "type": "string"
+            },
+            {
+                "internalType": "bytes",
+                "name": "signature",
+                "type": "bytes"
+            }
+        ],
+        "name": "addApprovedCertification",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "_hash",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "_imageHash",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "_metaHash",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "_certNum",
+                "type": "string"
+            },
+            {
+                "internalType": "uint256",
+                "name": "_expireDate",
+                "type": "uint256"
+            },
+            {
+                "internalType": "string",
+                "name": "_desc",
+                "type": "string"
+            }
+        ],
+        "name": "addCertification",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "_hash",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "_txid",
+                "type": "string"
+            }
+        ],
+        "name": "addTransactionId",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "_hash",
+                "type": "string"
+            }
+        ],
+        "name": "approve",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "",
+                "type": "string"
+            }
+        ],
+        "name": "approveInfos",
+        "outputs": [
+            {
+                "internalType": "string",
+                "name": "hash",
+                "type": "string"
+            },
+            {
+                "internalType": "bool",
+                "name": "isApproved",
+                "type": "bool"
+            },
+            {
+                "internalType": "address",
+                "name": "approverAddress",
+                "type": "address"
+            },
+            {
+                "internalType": "uint256",
+                "name": "approvedAt",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [],
         "name": "approver",
-        "type": "address"
-      },
-      {
-        "indexed": False,
-        "internalType": "string",
-        "name": "hash",
-        "type": "string"
-      },
-      {
-        "indexed": False,
-        "internalType": "string",
-        "name": "certNum",
-        "type": "string"
-      },
-      {
-        "indexed": False,
-        "internalType": "uint256",
-        "name": "timestamp",
-        "type": "uint256"
-      }
-    ],
-    "name": "Approved",
-    "type": "event"
-  },
-  {
-    "anonymous": False,
-    "inputs": [
-      {
-        "indexed": False,
-        "internalType": "address",
-        "name": "oldAddr",
-        "type": "address"
-      },
-      {
-        "indexed": False,
-        "internalType": "address",
-        "name": "newAddr",
-        "type": "address"
-      },
-      {
-        "indexed": False,
-        "internalType": "uint256",
-        "name": "timestamp",
-        "type": "uint256"
-      }
-    ],
-    "name": "ApproverAddressChanged",
-    "type": "event"
-  },
-  {
-    "anonymous": False,
-    "inputs": [
-      {
-        "indexed": False,
-        "internalType": "address",
-        "name": "to",
-        "type": "address"
-      },
-      {
-        "indexed": False,
-        "internalType": "uint256",
-        "name": "value",
-        "type": "uint256"
-      },
-      {
-        "indexed": False,
-        "internalType": "uint256",
-        "name": "timestamp",
-        "type": "uint256"
-      }
-    ],
-    "name": "CreditCharged",
-    "type": "event"
-  },
-  {
-    "anonymous": False,
-    "inputs": [
-      {
-        "indexed": False,
-        "internalType": "address",
-        "name": "issuer",
-        "type": "address"
-      },
-      {
-        "indexed": False,
-        "internalType": "string",
-        "name": "hash",
-        "type": "string"
-      },
-      {
-        "indexed": False,
-        "internalType": "string",
-        "name": "imageHash",
-        "type": "string"
-      },
-      {
-        "indexed": False,
-        "internalType": "string",
-        "name": "certNum",
-        "type": "string"
-      },
-      {
-        "indexed": False,
-        "internalType": "uint256",
-        "name": "timestamp",
-        "type": "uint256"
-      }
-    ],
-    "name": "Issued",
-    "type": "event"
-  },
-  {
-    "anonymous": False,
-    "inputs": [
-      {
-        "indexed": False,
-        "internalType": "address",
-        "name": "oldAddr",
-        "type": "address"
-      },
-      {
-        "indexed": False,
-        "internalType": "address",
-        "name": "newAddr",
-        "type": "address"
-      },
-      {
-        "indexed": False,
-        "internalType": "uint256",
-        "name": "timestamp",
-        "type": "uint256"
-      }
-    ],
-    "name": "IssuerRegistrationAddressChanged",
-    "type": "event"
-  },
-  {
-    "anonymous": False,
-    "inputs": [
-      {
-        "indexed": True,
-        "internalType": "address",
-        "name": "previousOwner",
-        "type": "address"
-      },
-      {
-        "indexed": True,
-        "internalType": "address",
-        "name": "newOwner",
-        "type": "address"
-      }
-    ],
-    "name": "OwnershipTransferred",
-    "type": "event"
-  },
-  {
-    "anonymous": False,
-    "inputs": [
-      {
-        "indexed": False,
-        "internalType": "address",
-        "name": "revoker",
-        "type": "address"
-      },
-      {
-        "indexed": False,
-        "internalType": "string",
-        "name": "hash",
-        "type": "string"
-      },
-      {
-        "indexed": False,
-        "internalType": "string",
-        "name": "certNum",
-        "type": "string"
-      },
-      {
-        "indexed": False,
-        "internalType": "uint256",
-        "name": "timestamp",
-        "type": "uint256"
-      }
-    ],
-    "name": "Revoked",
-    "type": "event"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "string",
-        "name": "_hash",
-        "type": "string"
-      },
-      {
-        "internalType": "string",
-        "name": "_imageHash",
-        "type": "string"
-      },
-      {
-        "internalType": "string",
-        "name": "_metaHash",
-        "type": "string"
-      },
-      {
-        "internalType": "string",
-        "name": "_certNum",
-        "type": "string"
-      },
-      {
-        "internalType": "uint256",
-        "name": "_expireDate",
-        "type": "uint256"
-      },
-      {
-        "internalType": "string",
-        "name": "_desc",
-        "type": "string"
-      }
-    ],
-    "name": "addCertification",
-    "outputs": [
-      {
-        "internalType": "uint256",
-        "name": "",
-        "type": "uint256"
-      }
-    ],
-    "stateMutability": "nonpayable",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "string",
-        "name": "_hash",
-        "type": "string"
-      },
-      {
-        "internalType": "string",
-        "name": "_txid",
-        "type": "string"
-      }
-    ],
-    "name": "addTransactionId",
-    "outputs": [],
-    "stateMutability": "nonpayable",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "string",
-        "name": "_hash",
-        "type": "string"
-      }
-    ],
-    "name": "approve",
-    "outputs": [],
-    "stateMutability": "nonpayable",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "string",
-        "name": "",
-        "type": "string"
-      }
-    ],
-    "name": "approveInfos",
-    "outputs": [
-      {
-        "internalType": "string",
-        "name": "hash",
-        "type": "string"
-      },
-      {
-        "internalType": "bool",
-        "name": "isApproved",
-        "type": "bool"
-      },
-      {
-        "internalType": "address",
-        "name": "approverAddress",
-        "type": "address"
-      },
-      {
-        "internalType": "uint256",
-        "name": "approvedAt",
-        "type": "uint256"
-      }
-    ],
-    "stateMutability": "view",
-    "type": "function"
-  },
-  {
-    "inputs": [],
-    "name": "approver",
-    "outputs": [
-      {
-        "internalType": "address",
-        "name": "",
-        "type": "address"
-      }
-    ],
-    "stateMutability": "view",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "string",
-        "name": "",
-        "type": "string"
-      }
-    ],
-    "name": "certifications",
-    "outputs": [
-      {
-        "internalType": "uint256",
-        "name": "id",
-        "type": "uint256"
-      },
-      {
-        "internalType": "string",
-        "name": "certNum",
-        "type": "string"
-      },
-      {
-        "internalType": "string",
-        "name": "hash",
-        "type": "string"
-      },
-      {
-        "internalType": "string",
-        "name": "imageHash",
-        "type": "string"
-      },
-      {
-        "internalType": "string",
-        "name": "metaHash",
-        "type": "string"
-      },
-      {
-        "internalType": "address",
-        "name": "issuer",
-        "type": "address"
-      },
-      {
-        "internalType": "uint256",
-        "name": "expireDate",
-        "type": "uint256"
-      },
-      {
-        "internalType": "uint256",
-        "name": "createdAt",
-        "type": "uint256"
-      },
-      {
-        "internalType": "string",
-        "name": "description",
-        "type": "string"
-      },
-      {
-        "internalType": "string",
-        "name": "txid",
-        "type": "string"
-      }
-    ],
-    "stateMutability": "view",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "address",
-        "name": "addr",
-        "type": "address"
-      },
-      {
-        "internalType": "uint256",
-        "name": "credit",
-        "type": "uint256"
-      }
-    ],
-    "name": "chargeCredit",
-    "outputs": [],
-    "stateMutability": "payable",
-    "type": "function"
-  },
-  {
-    "inputs": [],
-    "name": "creditAddress",
-    "outputs": [
-      {
-        "internalType": "address",
-        "name": "",
-        "type": "address"
-      }
-    ],
-    "stateMutability": "view",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "address",
-        "name": "",
-        "type": "address"
-      }
-    ],
-    "name": "credits",
-    "outputs": [
-      {
-        "internalType": "uint256",
-        "name": "",
-        "type": "uint256"
-      }
-    ],
-    "stateMutability": "view",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "string",
-        "name": "hash",
-        "type": "string"
-      }
-    ],
-    "name": "getApproveInfo",
-    "outputs": [
-      {
-        "components": [
-          {
-            "internalType": "string",
-            "name": "hash",
-            "type": "string"
-          },
-          {
-            "internalType": "bool",
-            "name": "isApproved",
-            "type": "bool"
-          },
-          {
-            "internalType": "address",
-            "name": "approverAddress",
-            "type": "address"
-          },
-          {
-            "internalType": "uint256",
-            "name": "approvedAt",
-            "type": "uint256"
-          }
-        ],
-        "internalType": "struct UniversityDiploma.ApproveInfo",
-        "name": "",
-        "type": "tuple"
-      }
-    ],
-    "stateMutability": "view",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "string",
-        "name": "hash",
-        "type": "string"
-      }
-    ],
-    "name": "getCertification",
-    "outputs": [
-      {
-        "components": [
-          {
-            "internalType": "uint256",
-            "name": "id",
-            "type": "uint256"
-          },
-          {
-            "internalType": "string",
-            "name": "certNum",
-            "type": "string"
-          },
-          {
-            "internalType": "string",
-            "name": "hash",
-            "type": "string"
-          },
-          {
-            "internalType": "string",
-            "name": "imageHash",
-            "type": "string"
-          },
-          {
-            "internalType": "string",
-            "name": "metaHash",
-            "type": "string"
-          },
-          {
-            "internalType": "address",
-            "name": "issuer",
-            "type": "address"
-          },
-          {
-            "internalType": "uint256",
-            "name": "expireDate",
-            "type": "uint256"
-          },
-          {
-            "internalType": "uint256",
-            "name": "createdAt",
-            "type": "uint256"
-          },
-          {
-            "internalType": "string",
-            "name": "description",
-            "type": "string"
-          },
-          {
-            "internalType": "string",
-            "name": "txid",
-            "type": "string"
-          }
-        ],
-        "internalType": "struct UniversityDiploma.Certification",
-        "name": "",
-        "type": "tuple"
-      }
-    ],
-    "stateMutability": "view",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "string",
-        "name": "certNum",
-        "type": "string"
-      }
-    ],
-    "name": "getCertificationByCertNum",
-    "outputs": [
-      {
-        "components": [
-          {
-            "internalType": "uint256",
-            "name": "id",
-            "type": "uint256"
-          },
-          {
-            "internalType": "string",
-            "name": "certNum",
-            "type": "string"
-          },
-          {
-            "internalType": "string",
-            "name": "hash",
-            "type": "string"
-          },
-          {
-            "internalType": "string",
-            "name": "imageHash",
-            "type": "string"
-          },
-          {
-            "internalType": "string",
-            "name": "metaHash",
-            "type": "string"
-          },
-          {
-            "internalType": "address",
-            "name": "issuer",
-            "type": "address"
-          },
-          {
-            "internalType": "uint256",
-            "name": "expireDate",
-            "type": "uint256"
-          },
-          {
-            "internalType": "uint256",
-            "name": "createdAt",
-            "type": "uint256"
-          },
-          {
-            "internalType": "string",
-            "name": "description",
-            "type": "string"
-          },
-          {
-            "internalType": "string",
-            "name": "txid",
-            "type": "string"
-          }
-        ],
-        "internalType": "struct UniversityDiploma.Certification",
-        "name": "",
-        "type": "tuple"
-      }
-    ],
-    "stateMutability": "view",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "address",
-        "name": "addr",
-        "type": "address"
-      }
-    ],
-    "name": "getCredit",
-    "outputs": [
-      {
-        "internalType": "uint256",
-        "name": "",
-        "type": "uint256"
-      }
-    ],
-    "stateMutability": "view",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "address",
-        "name": "issuer",
-        "type": "address"
-      }
-    ],
-    "name": "getIssuer",
-    "outputs": [
-      {
-        "components": [
-          {
-            "internalType": "uint256",
-            "name": "id",
-            "type": "uint256"
-          },
-          {
-            "internalType": "string",
-            "name": "name",
-            "type": "string"
-          },
-          {
-            "internalType": "string",
-            "name": "regnum",
-            "type": "string"
-          },
-          {
-            "internalType": "string",
-            "name": "description",
-            "type": "string"
-          },
-          {
-            "internalType": "string",
-            "name": "category",
-            "type": "string"
-          },
-          {
-            "internalType": "address",
-            "name": "addr",
-            "type": "address"
-          },
-          {
-            "internalType": "string",
-            "name": "metaDataUrl",
-            "type": "string"
-          },
-          {
-            "internalType": "bool",
-            "name": "isActive",
-            "type": "bool"
-          },
-          {
-            "internalType": "uint256",
-            "name": "createdAt",
-            "type": "uint256"
-          },
-          {
-            "internalType": "uint256",
-            "name": "updatedAt",
-            "type": "uint256"
-          }
-        ],
-        "internalType": "struct SharedStructs.Issuer",
-        "name": "",
-        "type": "tuple"
-      }
-    ],
-    "stateMutability": "view",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "string",
-        "name": "hash",
-        "type": "string"
-      }
-    ],
-    "name": "getRevokeInfo",
-    "outputs": [
-      {
-        "components": [
-          {
-            "internalType": "string",
-            "name": "hash",
-            "type": "string"
-          },
-          {
-            "internalType": "bool",
-            "name": "isRevoked",
-            "type": "bool"
-          },
-          {
-            "internalType": "address",
-            "name": "revokerAddress",
-            "type": "address"
-          },
-          {
-            "internalType": "string",
-            "name": "revokerName",
-            "type": "string"
-          },
-          {
-            "internalType": "string",
-            "name": "description",
-            "type": "string"
-          },
-          {
-            "internalType": "uint256",
-            "name": "revokedAt",
-            "type": "uint256"
-          }
-        ],
-        "internalType": "struct UniversityDiploma.RevokeInfo",
-        "name": "",
-        "type": "tuple"
-      }
-    ],
-    "stateMutability": "view",
-    "type": "function"
-  },
-  {
-    "inputs": [],
-    "name": "id",
-    "outputs": [
-      {
-        "internalType": "uint256",
-        "name": "",
-        "type": "uint256"
-      }
-    ],
-    "stateMutability": "view",
-    "type": "function"
-  },
-  {
-    "inputs": [],
-    "name": "initialize",
-    "outputs": [],
-    "stateMutability": "nonpayable",
-    "type": "function"
-  },
-  {
-    "inputs": [],
-    "name": "issuerRegistrationAddress",
-    "outputs": [
-      {
-        "internalType": "address",
-        "name": "",
-        "type": "address"
-      }
-    ],
-    "stateMutability": "view",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "string",
-        "name": "",
-        "type": "string"
-      }
-    ],
-    "name": "mapByCertNum",
-    "outputs": [
-      {
-        "internalType": "uint256",
+        "outputs": [
+            {
+                "internalType": "address",
+                "name": "",
+                "type": "address"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "",
+                "type": "string"
+            }
+        ],
+        "name": "certifications",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "id",
+                "type": "uint256"
+            },
+            {
+                "internalType": "string",
+                "name": "certNum",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "hash",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "imageHash",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "metaHash",
+                "type": "string"
+            },
+            {
+                "internalType": "address",
+                "name": "issuer",
+                "type": "address"
+            },
+            {
+                "internalType": "uint256",
+                "name": "expireDate",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "createdAt",
+                "type": "uint256"
+            },
+            {
+                "internalType": "string",
+                "name": "description",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "txid",
+                "type": "string"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [],
+        "name": "creditAddress",
+        "outputs": [
+            {
+                "internalType": "address",
+                "name": "",
+                "type": "address"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "address",
+                "name": "",
+                "type": "address"
+            }
+        ],
+        "name": "credits",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "hash",
+                "type": "string"
+            }
+        ],
+        "name": "getApproveInfo",
+        "outputs": [
+            {
+                "components": [
+                    {
+                        "internalType": "string",
+                        "name": "hash",
+                        "type": "string"
+                    },
+                    {
+                        "internalType": "bool",
+                        "name": "isApproved",
+                        "type": "bool"
+                    },
+                    {
+                        "internalType": "address",
+                        "name": "approverAddress",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "approvedAt",
+                        "type": "uint256"
+                    }
+                ],
+                "internalType": "struct UniversityDiploma.ApproveInfo",
+                "name": "",
+                "type": "tuple"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "hash",
+                "type": "string"
+            }
+        ],
+        "name": "getCertification",
+        "outputs": [
+            {
+                "components": [
+                    {
+                        "internalType": "uint256",
+                        "name": "id",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "string",
+                        "name": "certNum",
+                        "type": "string"
+                    },
+                    {
+                        "internalType": "string",
+                        "name": "hash",
+                        "type": "string"
+                    },
+                    {
+                        "internalType": "string",
+                        "name": "imageHash",
+                        "type": "string"
+                    },
+                    {
+                        "internalType": "string",
+                        "name": "metaHash",
+                        "type": "string"
+                    },
+                    {
+                        "internalType": "address",
+                        "name": "issuer",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "expireDate",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "createdAt",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "string",
+                        "name": "description",
+                        "type": "string"
+                    },
+                    {
+                        "internalType": "string",
+                        "name": "txid",
+                        "type": "string"
+                    }
+                ],
+                "internalType": "struct UniversityDiploma.Certification",
+                "name": "",
+                "type": "tuple"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "certNum",
+                "type": "string"
+            }
+        ],
+        "name": "getCertificationByCertNum",
+        "outputs": [
+            {
+                "components": [
+                    {
+                        "internalType": "uint256",
+                        "name": "id",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "string",
+                        "name": "certNum",
+                        "type": "string"
+                    },
+                    {
+                        "internalType": "string",
+                        "name": "hash",
+                        "type": "string"
+                    },
+                    {
+                        "internalType": "string",
+                        "name": "imageHash",
+                        "type": "string"
+                    },
+                    {
+                        "internalType": "string",
+                        "name": "metaHash",
+                        "type": "string"
+                    },
+                    {
+                        "internalType": "address",
+                        "name": "issuer",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "expireDate",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "createdAt",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "string",
+                        "name": "description",
+                        "type": "string"
+                    },
+                    {
+                        "internalType": "string",
+                        "name": "txid",
+                        "type": "string"
+                    }
+                ],
+                "internalType": "struct UniversityDiploma.Certification",
+                "name": "",
+                "type": "tuple"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "address",
+                "name": "addr",
+                "type": "address"
+            }
+        ],
+        "name": "getCredit",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "_metaHash",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "_certNum",
+                "type": "string"
+            }
+        ],
+        "name": "getMetaCertNumHash",
+        "outputs": [
+            {
+                "internalType": "bytes32",
+                "name": "",
+                "type": "bytes32"
+            }
+        ],
+        "stateMutability": "pure",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "_certNum",
+                "type": "string"
+            }
+        ],
+        "name": "getQrCodeData",
+        "outputs": [
+            {
+                "internalType": "string",
+                "name": "",
+                "type": "string"
+            }
+        ],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "hash",
+                "type": "string"
+            }
+        ],
+        "name": "getRevokeInfo",
+        "outputs": [
+            {
+                "components": [
+                    {
+                        "internalType": "string",
+                        "name": "hash",
+                        "type": "string"
+                    },
+                    {
+                        "internalType": "bool",
+                        "name": "isRevoked",
+                        "type": "bool"
+                    },
+                    {
+                        "internalType": "address",
+                        "name": "revokerAddress",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "string",
+                        "name": "revokerName",
+                        "type": "string"
+                    },
+                    {
+                        "internalType": "string",
+                        "name": "description",
+                        "type": "string"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "revokedAt",
+                        "type": "uint256"
+                    }
+                ],
+                "internalType": "struct UniversityDiploma.RevokeInfo",
+                "name": "",
+                "type": "tuple"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [],
         "name": "id",
-        "type": "uint256"
-      },
-      {
-        "internalType": "string",
-        "name": "certNum",
-        "type": "string"
-      },
-      {
-        "internalType": "string",
-        "name": "hash",
-        "type": "string"
-      },
-      {
-        "internalType": "string",
-        "name": "imageHash",
-        "type": "string"
-      },
-      {
-        "internalType": "string",
-        "name": "metaHash",
-        "type": "string"
-      },
-      {
-        "internalType": "address",
-        "name": "issuer",
-        "type": "address"
-      },
-      {
-        "internalType": "uint256",
-        "name": "expireDate",
-        "type": "uint256"
-      },
-      {
-        "internalType": "uint256",
-        "name": "createdAt",
-        "type": "uint256"
-      },
-      {
-        "internalType": "string",
-        "name": "description",
-        "type": "string"
-      },
-      {
-        "internalType": "string",
-        "name": "txid",
-        "type": "string"
-      }
-    ],
-    "stateMutability": "view",
-    "type": "function"
-  },
-  {
-    "inputs": [],
-    "name": "owner",
-    "outputs": [
-      {
-        "internalType": "address",
-        "name": "",
-        "type": "address"
-      }
-    ],
-    "stateMutability": "view",
-    "type": "function"
-  },
-  {
-    "inputs": [],
-    "name": "renounceOwnership",
-    "outputs": [],
-    "stateMutability": "nonpayable",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "string",
-        "name": "hash",
-        "type": "string"
-      },
-      {
-        "internalType": "string",
-        "name": "revokerName",
-        "type": "string"
-      }
-    ],
-    "name": "revoke",
-    "outputs": [],
-    "stateMutability": "nonpayable",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "string",
-        "name": "",
-        "type": "string"
-      }
-    ],
-    "name": "revokeInfos",
-    "outputs": [
-      {
-        "internalType": "string",
-        "name": "hash",
-        "type": "string"
-      },
-      {
-        "internalType": "bool",
-        "name": "isRevoked",
-        "type": "bool"
-      },
-      {
-        "internalType": "address",
-        "name": "revokerAddress",
-        "type": "address"
-      },
-      {
-        "internalType": "string",
-        "name": "revokerName",
-        "type": "string"
-      },
-      {
-        "internalType": "string",
-        "name": "description",
-        "type": "string"
-      },
-      {
-        "internalType": "uint256",
-        "name": "revokedAt",
-        "type": "uint256"
-      }
-    ],
-    "stateMutability": "view",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "address",
-        "name": "_approverAddress",
-        "type": "address"
-      }
-    ],
-    "name": "setApproverAddress",
-    "outputs": [],
-    "stateMutability": "nonpayable",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "address",
-        "name": "_issuerRegistrationAddress",
-        "type": "address"
-      }
-    ],
-    "name": "setIssuerRegistrationAddress",
-    "outputs": [],
-    "stateMutability": "nonpayable",
-    "type": "function"
-  },
-  {
-    "inputs": [
-      {
-        "internalType": "address",
-        "name": "newOwner",
-        "type": "address"
-      }
-    ],
-    "name": "transferOwnership",
-    "outputs": [],
-    "stateMutability": "nonpayable",
-    "type": "function"
-  }
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [],
+        "name": "initialize",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "address",
+                "name": "",
+                "type": "address"
+            }
+        ],
+        "name": "isApprover",
+        "outputs": [
+            {
+                "internalType": "bool",
+                "name": "",
+                "type": "bool"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [],
+        "name": "issuerRegistrationAddress",
+        "outputs": [
+            {
+                "internalType": "address",
+                "name": "",
+                "type": "address"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "",
+                "type": "string"
+            }
+        ],
+        "name": "mapByCertNum",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "id",
+                "type": "uint256"
+            },
+            {
+                "internalType": "string",
+                "name": "certNum",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "hash",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "imageHash",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "metaHash",
+                "type": "string"
+            },
+            {
+                "internalType": "address",
+                "name": "issuer",
+                "type": "address"
+            },
+            {
+                "internalType": "uint256",
+                "name": "expireDate",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "createdAt",
+                "type": "uint256"
+            },
+            {
+                "internalType": "string",
+                "name": "description",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "txid",
+                "type": "string"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [],
+        "name": "owner",
+        "outputs": [
+            {
+                "internalType": "address",
+                "name": "",
+                "type": "address"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "",
+                "type": "string"
+            }
+        ],
+        "name": "qrDataMap",
+        "outputs": [
+            {
+                "internalType": "string",
+                "name": "",
+                "type": "string"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "address",
+                "name": "_addr",
+                "type": "address"
+            }
+        ],
+        "name": "removeApprover",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [],
+        "name": "renounceOwnership",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "hash",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "revokerName",
+                "type": "string"
+            }
+        ],
+        "name": "revoke",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "",
+                "type": "string"
+            }
+        ],
+        "name": "revokeInfos",
+        "outputs": [
+            {
+                "internalType": "string",
+                "name": "hash",
+                "type": "string"
+            },
+            {
+                "internalType": "bool",
+                "name": "isRevoked",
+                "type": "bool"
+            },
+            {
+                "internalType": "address",
+                "name": "revokerAddress",
+                "type": "address"
+            },
+            {
+                "internalType": "string",
+                "name": "revokerName",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "description",
+                "type": "string"
+            },
+            {
+                "internalType": "uint256",
+                "name": "revokedAt",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "address",
+                "name": "_addr",
+                "type": "address"
+            }
+        ],
+        "name": "setApprover",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "address",
+                "name": "_approverAddress",
+                "type": "address"
+            }
+        ],
+        "name": "setApproverAddress",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "address",
+                "name": "_creditAddress",
+                "type": "address"
+            }
+        ],
+        "name": "setCreditAddress",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "string",
+                "name": "_certNum",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "_qrDataHash",
+                "type": "string"
+            }
+        ],
+        "name": "setQrCodeData",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "bytes",
+                "name": "sig",
+                "type": "bytes"
+            }
+        ],
+        "name": "splitSignature",
+        "outputs": [
+            {
+                "internalType": "bytes32",
+                "name": "r",
+                "type": "bytes32"
+            },
+            {
+                "internalType": "bytes32",
+                "name": "s",
+                "type": "bytes32"
+            },
+            {
+                "internalType": "uint8",
+                "name": "v",
+                "type": "uint8"
+            }
+        ],
+        "stateMutability": "pure",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "address",
+                "name": "newOwner",
+                "type": "address"
+            }
+        ],
+        "name": "transferOwnership",
+        "outputs": [],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    }
 ]
```

### Comparing `verify4py-test1-1.0.1/src/verify4py/utils.py` & `verify4py-test1-1.0.2/src/verify4py/utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-test1-1.0.1/src/verify4py_test1.egg-info/PKG-INFO` & `verify4py-test1-1.0.2/src/verify4py_test1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verify4py-test1
-Version: 1.0.1
+Version: 1.0.2
 Summary: Issue certificates using blockchain and smart contract
 Home-page: https://github.com/teo-mn/verify4py
 Author: Surenbayar Doloonjin
 Author-email: surenbayar@corex.mn
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/teo-mn/verify4py/issues
 Platform: UNKNOWN
```

### Comparing `verify4py-test1-1.0.1/src/verify4py_test1.egg-info/SOURCES.txt` & `verify4py-test1-1.0.2/src/verify4py_test1.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/verify4py/JsonIssuer.py
 src/verify4py/PdfIssuer.py
 src/verify4py/UniversityDiplomaIssuer.py
 src/verify4py/__init__.py
 src/verify4py/certify_sc_utils.py
 src/verify4py/json_utils.py
 src/verify4py/pdf.py
+src/verify4py/test_UniversityDiplomaIssuer.py
 src/verify4py/university_abi.py
 src/verify4py/utils.py
 src/verify4py_test1.egg-info/PKG-INFO
 src/verify4py_test1.egg-info/SOURCES.txt
 src/verify4py_test1.egg-info/dependency_links.txt
 src/verify4py_test1.egg-info/requires.txt
 src/verify4py_test1.egg-info/top_level.txt
```

