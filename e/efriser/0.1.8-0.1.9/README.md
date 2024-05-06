# Comparing `tmp/efriser-0.1.8.tar.gz` & `tmp/efriser-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efriser-0.1.8.tar", last modified: Tue Apr 16 09:13:40 2024, max compression
+gzip compressed data, was "efriser-0.1.9.tar", last modified: Wed Apr 17 11:40:28 2024, max compression
```

## Comparing `efriser-0.1.8.tar` & `efriser-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-16 09:13:40.977408 efriser-0.1.8/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)    17784 2024-04-16 09:13:40.977408 efriser-0.1.8/PKG-INFO
--rw-rw-r--   0 douglas   (1000) douglas   (1000)    17298 2024-04-16 09:07:55.000000 efriser-0.1.8/README.md
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-16 09:13:40.977408 efriser-0.1.8/efris/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      113 2024-04-15 11:34:23.000000 efriser-0.1.8/efris/__init__.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)    11840 2024-04-16 08:33:38.000000 efriser-0.1.8/efris/invoicing.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)    12249 2024-04-15 10:01:21.000000 efriser-0.1.8/efris/output_cleaner.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        0 2024-04-13 12:16:02.000000 efriser-0.1.8/efris/payload.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     1354 2024-04-13 12:28:02.000000 efriser-0.1.8/efris/services.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      874 2024-04-16 07:59:39.000000 efriser-0.1.8/efris/test_invoicing.py
--rw-rw-r--   0 douglas   (1000) douglas   (1000)     7159 2024-04-16 09:09:50.000000 efriser-0.1.8/efris/utils.py
-drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-16 09:13:40.977408 efriser-0.1.8/efriser.egg-info/
--rw-rw-r--   0 douglas   (1000) douglas   (1000)    17784 2024-04-16 09:13:40.000000 efriser-0.1.8/efriser.egg-info/PKG-INFO
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      307 2024-04-16 09:13:40.000000 efriser-0.1.8/efriser.egg-info/SOURCES.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        1 2024-04-16 09:13:40.000000 efriser-0.1.8/efriser.egg-info/dependency_links.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)       17 2024-04-16 09:13:40.000000 efriser-0.1.8/efriser.egg-info/requires.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)        6 2024-04-16 09:13:40.000000 efriser-0.1.8/efriser.egg-info/top_level.txt
--rw-rw-r--   0 douglas   (1000) douglas   (1000)       38 2024-04-16 09:13:40.977408 efriser-0.1.8/setup.cfg
--rw-rw-r--   0 douglas   (1000) douglas   (1000)      721 2024-04-16 09:12:51.000000 efriser-0.1.8/setup.py
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-17 11:40:28.043610 efriser-0.1.9/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)    20400 2024-04-17 11:40:28.043610 efriser-0.1.9/PKG-INFO
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)    19914 2024-04-17 11:39:20.000000 efriser-0.1.9/README.md
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-17 11:40:28.039610 efriser-0.1.9/efris/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      113 2024-04-15 11:34:23.000000 efriser-0.1.9/efris/__init__.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)    14803 2024-04-17 11:34:41.000000 efriser-0.1.9/efris/invoicing.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)    12249 2024-04-15 10:01:21.000000 efriser-0.1.9/efris/output_cleaner.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        0 2024-04-13 12:16:02.000000 efriser-0.1.9/efris/payload.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     1318 2024-04-17 10:55:48.000000 efriser-0.1.9/efris/services.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      874 2024-04-16 07:59:39.000000 efriser-0.1.9/efris/test_invoicing.py
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)     7159 2024-04-16 09:09:50.000000 efriser-0.1.9/efris/utils.py
+drwxrwxr-x   0 douglas   (1000) douglas   (1000)        0 2024-04-17 11:40:28.043610 efriser-0.1.9/efriser.egg-info/
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)    20400 2024-04-17 11:40:27.000000 efriser-0.1.9/efriser.egg-info/PKG-INFO
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      307 2024-04-17 11:40:27.000000 efriser-0.1.9/efriser.egg-info/SOURCES.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        1 2024-04-17 11:40:27.000000 efriser-0.1.9/efriser.egg-info/dependency_links.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)       17 2024-04-17 11:40:27.000000 efriser-0.1.9/efriser.egg-info/requires.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)        6 2024-04-17 11:40:27.000000 efriser-0.1.9/efriser.egg-info/top_level.txt
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)       38 2024-04-17 11:40:28.043610 efriser-0.1.9/setup.cfg
+-rw-rw-r--   0 douglas   (1000) douglas   (1000)      721 2024-04-17 11:40:05.000000 efriser-0.1.9/setup.py
```

### Comparing `efriser-0.1.8/PKG-INFO` & `efriser-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: efriser
-Version: 0.1.8
+Version: 0.1.9
 Summary: This is a python package to aid in fiscalisation of invoices with the Uganda Revenue Authority (URA) using the EFRIS API.
 Home-page: UNKNOWN
 Author: Douglas Ssekuwanda
 Author-email: cytixdoug@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-# EFRIS Package
+# EFRIS Python Package (EFRISER)
 
 This Python package provides a simple interface to interact with the EFRIS (Electronic Fiscal Receipt Information System) API provided by the Uganda Revenue Authority (URA) for invoicing.
 
 ## Features
 
 - Create EFRIS invoices
 - Retrieve the status of credit notes
@@ -101,15 +101,14 @@
 
 The method then sends a POST request to an external server (possibly the EFRIS server) using `self.efris_post(ic, message)`. This method handles the POST request and retrieves the response.
 
 The response from the POST request is then passed to the `format_invoice_query_output` function (not shown in this snippet), which likely processes the response and formats it into a more usable dictionary.
 
 Finally, the formatted output of the invoice query is returned as a dictionary by the `query_document` method.
 
-
 ---
 
 ## Function: query_invoice_details(self, fdn)
 
 This method queries the details of an invoice using its Fiscal Document Number (FDN).
 
 ### Parameters:
@@ -348,15 +347,81 @@
 
 The response from the server is passed to the `format_taxpayer_output` function, which formats and processes the tax payer data received from the server.
 
 Finally, the formatted tax payer output is returned as a dictionary by the `query_tax_payer_by_tin` method.
 
 ---
 
+## Function: upload_products(self, invoice_data)
+
+This method is used to create EFRIS invoices using the provided invoice data.
+
+### Args
+- `invoice_data (list)`: A list of dictionaries representing invoices. Each dictionary should contain the following keys:
+  - `"havePieceUnit"`: Indicator for piece unit availability.
+  - `"goodsName"`: Name of the goods.
+  - `"goodsCode"`: Code assigned to the goods should be unique.
+  - `"measureUnit"`: Measurement unit for the goods as per URA documentation.
+  - `"unitPrice"`: Price per unit of the goods.
+  - `"currency"`: Currency code for the price as per URA.
+  - `"commodityCategoryId"`: Category ID for the goods as per URA goods ID.
+  - `"haveExciseTax"`: Indicator for excise tax availability.
+  - `"description"`: Description of the goods.
+  - `"stockPrewarning"`: Stock prewarning threshold.
+
+
+
+### Returns
+- `list` or `False`: A list of return messages from the EFRIS service if successful, or `False` if any invalid invoices are encountered.
+
+### Code Explanation
+
+The `upload_products` method validates each invoice in the provided `invoice_data` list to ensure all required keys are present. If any invalid invoices are found, they are logged, and the function returns `False`.
+
+The method then makes a POST request to the EFRIS server using the action code `'T130'` (assigned to the variable `ic`) and the `invoice_data` list as the message.
+
+If the response from the server (`return_msg`) is empty (`[]`), the method returns an empty list.
+
+If the response contains data, the `content` is decoded using base64 and parsed as JSON (`decoded_data`). If `decoded_data` is empty, an empty list is returned.
+
+Otherwise, the method extracts the `returnMessage` from each dictionary in `decoded_data` to compile a list of return messages (`return_messages`), which is returned as the final result.
+
+### Example
+```
+[
+    {
+        "havePieceUnit": "102",
+        "goodsName": "Service ABC",
+        "goodsCode": "ABC123",
+        "measureUnit": "115",
+        "unitPrice": "10.00",
+        "currency": "101",
+        "commodityCategoryId": "84111601",
+        "haveExciseTax": "102",
+        "description": "This is Service A",
+        "stockPrewarning": "0"
+    },
+      {
+        "havePieceUnit": "102",
+        "goodsName": "Product",
+        "goodsCode": "ABC123",
+        "measureUnit": "115",
+        "unitPrice": "10.00",
+        "currency": "101",
+        "commodityCategoryId": "84111601",
+        "haveExciseTax": "102",
+        "description": "This is Product A",
+        "stockPrewarning": "50"
+    }
+]
+```
+---
 If you found this package helpful, consider buying me a coffee! 😊
 
 Mobile money number: +256705860416
 
+Whatsapp: +256705860416
+
 Or get in touch with me on [douglasekuwanda@gmail.com](mailto:douglasekuwanda@gmail.com)
```

### Comparing `efriser-0.1.8/README.md` & `efriser-0.1.9/efriser.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,22 @@
-# EFRIS Package
+Metadata-Version: 2.1
+Name: efriser
+Version: 0.1.9
+Summary: This is a python package to aid in fiscalisation of invoices with the Uganda Revenue Authority (URA) using the EFRIS API.
+Home-page: UNKNOWN
+Author: Douglas Ssekuwanda
+Author-email: cytixdoug@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
+# EFRIS Python Package (EFRISER)
 
 This Python package provides a simple interface to interact with the EFRIS (Electronic Fiscal Receipt Information System) API provided by the Uganda Revenue Authority (URA) for invoicing.
 
 ## Features
 
 - Create EFRIS invoices
 - Retrieve the status of credit notes
@@ -87,15 +101,14 @@
 
 The method then sends a POST request to an external server (possibly the EFRIS server) using `self.efris_post(ic, message)`. This method handles the POST request and retrieves the response.
 
 The response from the POST request is then passed to the `format_invoice_query_output` function (not shown in this snippet), which likely processes the response and formats it into a more usable dictionary.
 
 Finally, the formatted output of the invoice query is returned as a dictionary by the `query_document` method.
 
-
 ---
 
 ## Function: query_invoice_details(self, fdn)
 
 This method queries the details of an invoice using its Fiscal Document Number (FDN).
 
 ### Parameters:
@@ -334,13 +347,81 @@
 
 The response from the server is passed to the `format_taxpayer_output` function, which formats and processes the tax payer data received from the server.
 
 Finally, the formatted tax payer output is returned as a dictionary by the `query_tax_payer_by_tin` method.
 
 ---
 
+## Function: upload_products(self, invoice_data)
+
+This method is used to create EFRIS invoices using the provided invoice data.
+
+### Args
+- `invoice_data (list)`: A list of dictionaries representing invoices. Each dictionary should contain the following keys:
+  - `"havePieceUnit"`: Indicator for piece unit availability.
+  - `"goodsName"`: Name of the goods.
+  - `"goodsCode"`: Code assigned to the goods should be unique.
+  - `"measureUnit"`: Measurement unit for the goods as per URA documentation.
+  - `"unitPrice"`: Price per unit of the goods.
+  - `"currency"`: Currency code for the price as per URA.
+  - `"commodityCategoryId"`: Category ID for the goods as per URA goods ID.
+  - `"haveExciseTax"`: Indicator for excise tax availability.
+  - `"description"`: Description of the goods.
+  - `"stockPrewarning"`: Stock prewarning threshold.
+
+
+
+### Returns
+- `list` or `False`: A list of return messages from the EFRIS service if successful, or `False` if any invalid invoices are encountered.
+
+### Code Explanation
+
+The `upload_products` method validates each invoice in the provided `invoice_data` list to ensure all required keys are present. If any invalid invoices are found, they are logged, and the function returns `False`.
+
+The method then makes a POST request to the EFRIS server using the action code `'T130'` (assigned to the variable `ic`) and the `invoice_data` list as the message.
+
+If the response from the server (`return_msg`) is empty (`[]`), the method returns an empty list.
+
+If the response contains data, the `content` is decoded using base64 and parsed as JSON (`decoded_data`). If `decoded_data` is empty, an empty list is returned.
+
+Otherwise, the method extracts the `returnMessage` from each dictionary in `decoded_data` to compile a list of return messages (`return_messages`), which is returned as the final result.
+
+### Example
+```
+[
+    {
+        "havePieceUnit": "102",
+        "goodsName": "Service ABC",
+        "goodsCode": "ABC123",
+        "measureUnit": "115",
+        "unitPrice": "10.00",
+        "currency": "101",
+        "commodityCategoryId": "84111601",
+        "haveExciseTax": "102",
+        "description": "This is Service A",
+        "stockPrewarning": "0"
+    },
+      {
+        "havePieceUnit": "102",
+        "goodsName": "Product",
+        "goodsCode": "ABC123",
+        "measureUnit": "115",
+        "unitPrice": "10.00",
+        "currency": "101",
+        "commodityCategoryId": "84111601",
+        "haveExciseTax": "102",
+        "description": "This is Product A",
+        "stockPrewarning": "50"
+    }
+]
+```
+---
 If you found this package helpful, consider buying me a coffee! 😊
 
 Mobile money number: +256705860416
 
+Whatsapp: +256705860416
+
 Or get in touch with me on [douglasekuwanda@gmail.com](mailto:douglasekuwanda@gmail.com)
 
+
+
```

### Comparing `efriser-0.1.8/efris/output_cleaner.py` & `efriser-0.1.9/efris/output_cleaner.py`

 * *Files identical despite different names*

### Comparing `efriser-0.1.8/efris/services.py` & `efriser-0.1.9/efris/services.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,26 +17,26 @@
     decoded_dict = json.loads(decoded_content)
     return decoded_dict
 
 def process_response(ip, data_dump):
     response = requests.post(ip, json=data_dump)
     response.raise_for_status()
     json_data = response.json()
-    print('-------------------------')
     print(json_data)
+    print('-------------------------')
 
     if json_data['returnStateInfo']['returnMessage'] == 'SUCCESS':
         if json_data['data']['dataDescription']['zipCode'] != '1':
             content = json_data['data']['content']
             decoded_data = decode_content(content)
             return decoded_data
         else:
             content = json_data['data']['content']
             gz = base64.b64decode(content)
             decompressed_data = gzip.decompress(gz).decode('utf-8')
             if isinstance(decompressed_data, str):
                 return decompressed_data
             else:
-                return json.loads(decompressed_data)
+                json_data = json.loads(decompressed_data)
+                return json_data
     else:
-        # print(f"Error: {json_data['returnStateInfo']['returnMessage']}")
-        return json_data['returnStateInfo']['returnMessage']
+        return json_data#['returnStateInfo']['returnMessage']
```

### Comparing `efriser-0.1.8/efris/test_invoicing.py` & `efriser-0.1.9/efris/test_invoicing.py`

 * *Files identical despite different names*

### Comparing `efriser-0.1.8/efris/utils.py` & `efriser-0.1.9/efris/utils.py`

 * *Files identical despite different names*

### Comparing `efriser-0.1.8/efriser.egg-info/PKG-INFO` & `efriser-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,8 @@
-Metadata-Version: 2.1
-Name: efriser
-Version: 0.1.8
-Summary: This is a python package to aid in fiscalisation of invoices with the Uganda Revenue Authority (URA) using the EFRIS API.
-Home-page: UNKNOWN
-Author: Douglas Ssekuwanda
-Author-email: cytixdoug@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
-# EFRIS Package
+# EFRIS Python Package (EFRISER)
 
 This Python package provides a simple interface to interact with the EFRIS (Electronic Fiscal Receipt Information System) API provided by the Uganda Revenue Authority (URA) for invoicing.
 
 ## Features
 
 - Create EFRIS invoices
 - Retrieve the status of credit notes
@@ -101,15 +87,14 @@
 
 The method then sends a POST request to an external server (possibly the EFRIS server) using `self.efris_post(ic, message)`. This method handles the POST request and retrieves the response.
 
 The response from the POST request is then passed to the `format_invoice_query_output` function (not shown in this snippet), which likely processes the response and formats it into a more usable dictionary.
 
 Finally, the formatted output of the invoice query is returned as a dictionary by the `query_document` method.
 
-
 ---
 
 ## Function: query_invoice_details(self, fdn)
 
 This method queries the details of an invoice using its Fiscal Document Number (FDN).
 
 ### Parameters:
@@ -348,15 +333,79 @@
 
 The response from the server is passed to the `format_taxpayer_output` function, which formats and processes the tax payer data received from the server.
 
 Finally, the formatted tax payer output is returned as a dictionary by the `query_tax_payer_by_tin` method.
 
 ---
 
+## Function: upload_products(self, invoice_data)
+
+This method is used to create EFRIS invoices using the provided invoice data.
+
+### Args
+- `invoice_data (list)`: A list of dictionaries representing invoices. Each dictionary should contain the following keys:
+  - `"havePieceUnit"`: Indicator for piece unit availability.
+  - `"goodsName"`: Name of the goods.
+  - `"goodsCode"`: Code assigned to the goods should be unique.
+  - `"measureUnit"`: Measurement unit for the goods as per URA documentation.
+  - `"unitPrice"`: Price per unit of the goods.
+  - `"currency"`: Currency code for the price as per URA.
+  - `"commodityCategoryId"`: Category ID for the goods as per URA goods ID.
+  - `"haveExciseTax"`: Indicator for excise tax availability.
+  - `"description"`: Description of the goods.
+  - `"stockPrewarning"`: Stock prewarning threshold.
+
+
+
+### Returns
+- `list` or `False`: A list of return messages from the EFRIS service if successful, or `False` if any invalid invoices are encountered.
+
+### Code Explanation
+
+The `upload_products` method validates each invoice in the provided `invoice_data` list to ensure all required keys are present. If any invalid invoices are found, they are logged, and the function returns `False`.
+
+The method then makes a POST request to the EFRIS server using the action code `'T130'` (assigned to the variable `ic`) and the `invoice_data` list as the message.
+
+If the response from the server (`return_msg`) is empty (`[]`), the method returns an empty list.
+
+If the response contains data, the `content` is decoded using base64 and parsed as JSON (`decoded_data`). If `decoded_data` is empty, an empty list is returned.
+
+Otherwise, the method extracts the `returnMessage` from each dictionary in `decoded_data` to compile a list of return messages (`return_messages`), which is returned as the final result.
+
+### Example
+```
+[
+    {
+        "havePieceUnit": "102",
+        "goodsName": "Service ABC",
+        "goodsCode": "ABC123",
+        "measureUnit": "115",
+        "unitPrice": "10.00",
+        "currency": "101",
+        "commodityCategoryId": "84111601",
+        "haveExciseTax": "102",
+        "description": "This is Service A",
+        "stockPrewarning": "0"
+    },
+      {
+        "havePieceUnit": "102",
+        "goodsName": "Product",
+        "goodsCode": "ABC123",
+        "measureUnit": "115",
+        "unitPrice": "10.00",
+        "currency": "101",
+        "commodityCategoryId": "84111601",
+        "haveExciseTax": "102",
+        "description": "This is Product A",
+        "stockPrewarning": "50"
+    }
+]
+```
+---
 If you found this package helpful, consider buying me a coffee! 😊
 
 Mobile money number: +256705860416
 
-Or get in touch with me on [douglasekuwanda@gmail.com](mailto:douglasekuwanda@gmail.com)
-
+Whatsapp: +256705860416
 
+Or get in touch with me on [douglasekuwanda@gmail.com](mailto:douglasekuwanda@gmail.com)
```

### Comparing `efriser-0.1.8/setup.py` & `efriser-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='efriser',
-    version='0.1.8',
+    version='0.1.9',
     author='Douglas Ssekuwanda',
     author_email='cytixdoug@gmail.com',
     description='This is a python package to aid in fiscalisation of invoices with the Uganda Revenue Authority (URA) using the EFRIS API.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

