# Comparing `tmp/verify4py-2.0.0.tar.gz` & `tmp/verify4py-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verify4py-2.0.0.tar", last modified: Mon Mar  4 09:23:48 2024, max compression
+gzip compressed data, was "verify4py-2.0.1.tar", last modified: Mon May  6 13:18:30 2024, max compression
```

## Comparing `verify4py-2.0.0.tar` & `verify4py-2.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2024-03-04 09:23:48.864350 verify4py-2.0.0/
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1065 2024-02-23 08:57:08.000000 verify4py-2.0.0/LICENSE
--rw-r--r--   0 surenbayar  (1000) surenbayar  (1000)     9398 2024-03-04 09:23:48.864350 verify4py-2.0.0/PKG-INFO
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     8817 2024-02-23 08:57:08.000000 verify4py-2.0.0/README.md
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       84 2024-02-23 08:57:08.000000 verify4py-2.0.0/pyproject.toml
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       38 2024-03-04 09:23:48.864350 verify4py-2.0.0/setup.cfg
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      879 2024-03-04 09:23:32.000000 verify4py-2.0.0/setup.py
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2024-03-04 09:23:48.860350 verify4py-2.0.0/src/
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2024-03-04 09:23:48.864350 verify4py-2.0.0/src/verify4py/
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    11193 2024-03-04 08:46:35.000000 verify4py-2.0.0/src/verify4py/Issuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     3509 2024-02-23 08:57:08.000000 verify4py-2.0.0/src/verify4py/JsonIssuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     2909 2024-02-23 08:57:08.000000 verify4py-2.0.0/src/verify4py/PdfIssuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     5302 2024-03-04 08:45:08.000000 verify4py-2.0.0/src/verify4py/UniversityDiplomaIssuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        0 2024-02-23 08:57:08.000000 verify4py-2.0.0/src/verify4py/__init__.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    27300 2024-02-23 08:57:08.000000 verify4py-2.0.0/src/verify4py/certify_sc_utils.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1067 2024-02-23 08:57:08.000000 verify4py-2.0.0/src/verify4py/json_utils.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      689 2024-02-23 08:57:08.000000 verify4py-2.0.0/src/verify4py/pdf.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     2018 2024-03-04 08:49:05.000000 verify4py-2.0.0/src/verify4py/test_UniversityDiplomaIssuer.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    21276 2024-02-23 09:00:59.000000 verify4py-2.0.0/src/verify4py/university_abi.py
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1526 2024-02-23 08:57:08.000000 verify4py-2.0.0/src/verify4py/utils.py
-drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2024-03-04 09:23:48.864350 verify4py-2.0.0/src/verify4py.egg-info/
--rw-r--r--   0 surenbayar  (1000) surenbayar  (1000)     9398 2024-03-04 09:23:48.000000 verify4py-2.0.0/src/verify4py.egg-info/PKG-INFO
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      555 2024-03-04 09:23:48.000000 verify4py-2.0.0/src/verify4py.egg-info/SOURCES.txt
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        1 2024-03-04 09:23:48.000000 verify4py-2.0.0/src/verify4py.egg-info/dependency_links.txt
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       23 2024-03-04 09:23:48.000000 verify4py-2.0.0/src/verify4py.egg-info/requires.txt
--rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       10 2024-03-04 09:23:48.000000 verify4py-2.0.0/src/verify4py.egg-info/top_level.txt
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2024-05-06 13:18:30.761310 verify4py-2.0.1/
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1065 2024-02-23 08:57:08.000000 verify4py-2.0.1/LICENSE
+-rw-r--r--   0 surenbayar  (1000) surenbayar  (1000)     9398 2024-05-06 13:18:30.761310 verify4py-2.0.1/PKG-INFO
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     8817 2024-02-23 08:57:08.000000 verify4py-2.0.1/README.md
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       84 2024-02-23 08:57:08.000000 verify4py-2.0.1/pyproject.toml
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       38 2024-05-06 13:18:30.761310 verify4py-2.0.1/setup.cfg
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      879 2024-05-06 13:18:25.000000 verify4py-2.0.1/setup.py
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2024-05-06 13:18:30.757310 verify4py-2.0.1/src/
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2024-05-06 13:18:30.761310 verify4py-2.0.1/src/verify4py/
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    12118 2024-05-06 13:17:03.000000 verify4py-2.0.1/src/verify4py/Issuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     3509 2024-02-23 08:57:08.000000 verify4py-2.0.1/src/verify4py/JsonIssuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     2909 2024-02-23 08:57:08.000000 verify4py-2.0.1/src/verify4py/PdfIssuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     5302 2024-05-06 13:15:22.000000 verify4py-2.0.1/src/verify4py/UniversityDiplomaIssuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        0 2024-02-23 08:57:08.000000 verify4py-2.0.1/src/verify4py/__init__.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    27300 2024-02-23 08:57:08.000000 verify4py-2.0.1/src/verify4py/certify_sc_utils.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1067 2024-02-23 08:57:08.000000 verify4py-2.0.1/src/verify4py/json_utils.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      689 2024-02-23 08:57:08.000000 verify4py-2.0.1/src/verify4py/pdf.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     2018 2024-05-06 13:15:22.000000 verify4py-2.0.1/src/verify4py/test_UniversityDiplomaIssuer.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)    29369 2024-05-06 13:17:03.000000 verify4py-2.0.1/src/verify4py/university_abi.py
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)     1526 2024-02-23 08:57:08.000000 verify4py-2.0.1/src/verify4py/utils.py
+drwxrwxr-x   0 surenbayar  (1000) surenbayar  (1000)        0 2024-05-06 13:18:30.761310 verify4py-2.0.1/src/verify4py.egg-info/
+-rw-r--r--   0 surenbayar  (1000) surenbayar  (1000)     9398 2024-05-06 13:18:30.000000 verify4py-2.0.1/src/verify4py.egg-info/PKG-INFO
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)      555 2024-05-06 13:18:30.000000 verify4py-2.0.1/src/verify4py.egg-info/SOURCES.txt
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)        1 2024-05-06 13:18:30.000000 verify4py-2.0.1/src/verify4py.egg-info/dependency_links.txt
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       23 2024-05-06 13:18:30.000000 verify4py-2.0.1/src/verify4py.egg-info/requires.txt
+-rw-rw-r--   0 surenbayar  (1000) surenbayar  (1000)       10 2024-05-06 13:18:30.000000 verify4py-2.0.1/src/verify4py.egg-info/top_level.txt
```

### Comparing `verify4py-2.0.0/LICENSE` & `verify4py-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `verify4py-2.0.0/PKG-INFO` & `verify4py-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verify4py
-Version: 2.0.0
+Version: 2.0.1
 Summary: Issue certificates using blockchain and smart contract
 Home-page: https://github.com/teo-mn/verify4py
 Author: Surenbayar Doloonjin
 Author-email: surenbayar@corex.mn
 Project-URL: Bug Tracker, https://github.com/teo-mn/verify4py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `verify4py-2.0.0/README.md` & `verify4py-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `verify4py-2.0.0/setup.py` & `verify4py-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="verify4py",
-    version="2.0.0",
+    version="2.0.1",
     author="Surenbayar Doloonjin",
     author_email="surenbayar@corex.mn",
     description="Issue certificates using blockchain and smart contract",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/teo-mn/verify4py",
     project_urls={
```

### Comparing `verify4py-2.0.0/src/verify4py/Issuer.py` & `verify4py-2.0.1/src/verify4py/Issuer.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,32 @@
             'addr': arr[5],
             'metaDataUrl': arr[6],
             'isActive': arr[7],
             'createdAt': arr[8],
             'updatedAt': arr[9],
         })
 
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
+
 
 class CertStruct:
     id: int
     certNum: str
     hash: str
     issuer: str
     expireDate: int
```

### Comparing `verify4py-2.0.0/src/verify4py/JsonIssuer.py` & `verify4py-2.0.1/src/verify4py/JsonIssuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-2.0.0/src/verify4py/PdfIssuer.py` & `verify4py-2.0.1/src/verify4py/PdfIssuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-2.0.0/src/verify4py/UniversityDiplomaIssuer.py` & `verify4py-2.0.1/src/verify4py/UniversityDiplomaIssuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-2.0.0/src/verify4py/certify_sc_utils.py` & `verify4py-2.0.1/src/verify4py/certify_sc_utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-2.0.0/src/verify4py/json_utils.py` & `verify4py-2.0.1/src/verify4py/json_utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-2.0.0/src/verify4py/pdf.py` & `verify4py-2.0.1/src/verify4py/pdf.py`

 * *Files identical despite different names*

### Comparing `verify4py-2.0.0/src/verify4py/test_UniversityDiplomaIssuer.py` & `verify4py-2.0.1/src/verify4py/test_UniversityDiplomaIssuer.py`

 * *Files identical despite different names*

### Comparing `verify4py-2.0.0/src/verify4py/university_abi.py` & `verify4py-2.0.1/src/verify4py/university_abi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,1045 +1,1107 @@
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
-        "name": "metaHash",
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
-      },
-      {
-        "internalType": "bytes",
-        "name": "signature",
-        "type": "bytes"
-      }
-    ],
-    "name": "addApprovedCertification",
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
-        "name": "_metaHash",
-        "type": "string"
-      },
-      {
-        "internalType": "string",
-        "name": "_certNum",
-        "type": "string"
-      }
-    ],
-    "name": "getMetaCertNumHash",
-    "outputs": [
-      {
-        "internalType": "bytes32",
-        "name": "",
-        "type": "bytes32"
-      }
-    ],
-    "stateMutability": "pure",
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
-        "name": "_creditAddress",
-        "type": "address"
-      }
-    ],
-    "name": "setCreditAddress",
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
-        "internalType": "bytes",
-        "name": "sig",
-        "type": "bytes"
-      }
-    ],
-    "name": "splitSignature",
-    "outputs": [
-      {
-        "internalType": "bytes32",
-        "name": "r",
-        "type": "bytes32"
-      },
-      {
-        "internalType": "bytes32",
-        "name": "s",
-        "type": "bytes32"
-      },
-      {
-        "internalType": "uint8",
-        "name": "v",
-        "type": "uint8"
-      }
-    ],
-    "stateMutability": "pure",
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

### Comparing `verify4py-2.0.0/src/verify4py/utils.py` & `verify4py-2.0.1/src/verify4py/utils.py`

 * *Files identical despite different names*

### Comparing `verify4py-2.0.0/src/verify4py.egg-info/PKG-INFO` & `verify4py-2.0.1/src/verify4py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verify4py
-Version: 2.0.0
+Version: 2.0.1
 Summary: Issue certificates using blockchain and smart contract
 Home-page: https://github.com/teo-mn/verify4py
 Author: Surenbayar Doloonjin
 Author-email: surenbayar@corex.mn
 Project-URL: Bug Tracker, https://github.com/teo-mn/verify4py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `verify4py-2.0.0/src/verify4py.egg-info/SOURCES.txt` & `verify4py-2.0.1/src/verify4py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

