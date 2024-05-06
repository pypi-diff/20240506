# Comparing `tmp/xl2roefact-0.7rc1.tar.gz` & `tmp/xl2roefact-0.7rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xl2roefact-0.7rc1.tar", last modified: Wed May  1 17:06:29 2024, max compression
+gzip compressed data, was "xl2roefact-0.7rc2.tar", last modified: Mon May  6 03:29:53 2024, max compression
```

## Comparing `xl2roefact-0.7rc1.tar` & `xl2roefact-0.7rc2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    35149 2024-05-01 17:06:04.373227 xl2roefact-0.7rc1/LICENSE
--rw-r--r--   0        0        0    18839 2024-05-01 17:06:04.373227 xl2roefact-0.7rc1/README.md
--rw-r--r--   0        0        0     3336 2024-05-01 17:06:29.456978 xl2roefact-0.7rc1/pyproject.toml
--rw-r--r--   0        0        0     1808 2024-05-01 17:06:04.829223 xl2roefact-0.7rc1/src/data/README_app_config_rules.md
--rw-r--r--   0        0        0        1 2024-05-01 17:06:04.829223 xl2roefact-0.7rc1/src/data/__init__.py
--rw-r--r--   0        0        0     7134 2024-05-01 17:06:04.829223 xl2roefact-0.7rc1/src/data/app_settings.yml
--rw-r--r--   0        0        0        1 2024-05-01 17:06:04.829223 xl2roefact-0.7rc1/tests/.gitkeep
--rw-r--r--   0        0        0    21711 2024-05-01 17:06:04.829223 xl2roefact-0.7rc1/tests/Fact_Petrom_11017969.json
--rw-r--r--   0        0        0   268862 2024-05-01 17:06:04.829223 xl2roefact-0.7rc1/tests/Fact_Petrom_11017969.xlsx
--rw-r--r--   0        0        0    15740 2024-05-01 17:06:04.829223 xl2roefact-0.7rc1/tests/Fact_Petrom_11017969.xml
--rw-r--r--   0        0        0      986 2024-05-01 17:06:04.829223 xl2roefact-0.7rc1/tests/_test_results.txt
--rw-r--r--   0        0        0    24173 2024-05-01 17:06:04.829223 xl2roefact-0.7rc1/tests/fact_RENF1004.json
--rw-r--r--   0        0        0    16332 2024-05-01 17:06:04.829223 xl2roefact-0.7rc1/tests/fact_RENF1004.xlsx
--rw-r--r--   0        0        0    61437 1970-01-01 00:00:00.000000 xl2roefact-0.7rc1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-06 03:29:27.462748 xl2roefact-0.7rc2/LICENSE
+-rw-r--r--   0        0        0    18839 2024-05-06 03:29:27.462748 xl2roefact-0.7rc2/README.md
+-rw-r--r--   0        0        0     3336 2024-05-06 03:29:53.094666 xl2roefact-0.7rc2/pyproject.toml
+-rw-r--r--   0        0        0      176 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/src/commands/__init__.py
+-rw-r--r--   0        0        0     1808 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/src/data/README_app_config_rules.md
+-rw-r--r--   0        0        0      174 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/src/data/__init__.py
+-rw-r--r--   0        0        0     7134 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/src/data/app_settings.yml
+-rw-r--r--   0        0        0        1 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/tests/.gitkeep
+-rw-r--r--   0        0        0    21711 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/tests/Fact_Petrom_11017969.json
+-rw-r--r--   0        0        0   268862 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/tests/Fact_Petrom_11017969.xlsx
+-rw-r--r--   0        0        0    15740 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/tests/Fact_Petrom_11017969.xml
+-rw-r--r--   0        0        0      986 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/tests/_test_results.txt
+-rw-r--r--   0        0        0    24173 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/tests/fact_RENF1004.json
+-rw-r--r--   0        0        0    16332 2024-05-06 03:29:27.978747 xl2roefact-0.7rc2/tests/fact_RENF1004.xlsx
+-rw-r--r--   0        0        0    61437 1970-01-01 00:00:00.000000 xl2roefact-0.7rc2/PKG-INFO
```

### Comparing `xl2roefact-0.7rc1/LICENSE` & `xl2roefact-0.7rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.7rc1/README.md` & `xl2roefact-0.7rc2/README.md`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.7rc1/pyproject.toml` & `xl2roefact-0.7rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     "Programming Language :: Python :: 3.11",
     "Development Status :: 4 - Beta",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Operating System :: OS Independent",
     "Topic :: Office/Business :: Financial",
 ]
-version = "0.7rc1"
+version = "0.7rc2"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://invoicetoroefact.renware.eu"
 PDF-Documentation = "https://invoicetoroefact.renware.eu/pdfs/print_page.html/print_page.pdf"
```

### Comparing `xl2roefact-0.7rc1/src/data/README_app_config_rules.md` & `xl2roefact-0.7rc2/src/data/README_app_config_rules.md`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.7rc1/src/data/app_settings.yml` & `xl2roefact-0.7rc2/src/data/app_settings.yml`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.7rc1/tests/Fact_Petrom_11017969.json` & `xl2roefact-0.7rc2/tests/Fact_Petrom_11017969.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9857142857142858%*

 * *Differences: {"'Invoice'": "{'cbc_Note': 'generated @2024-05-06T03:19:09.003169+00:00 with xl2roefact by "*

 * *              "RENware Software Systems'}",*

 * * "'meta_info'": "{'last_processing_time': '2024-05-06T03:19:09.002798+00:00'}"}*

```diff
@@ -171,15 +171,15 @@
             "cbc_TaxAmount": 8123.66
         },
         "cbc_DocumentCurrencyCode": "RON",
         "cbc_DueDate": "2023-11-16",
         "cbc_ID": "11017969",
         "cbc_InvoiceTypeCode": "380",
         "cbc_IssueDate": "2023-10-17",
-        "cbc_Note": "generated @2024-05-01T02:36:47.338315+00:00 with xl2roefact by RENware Software Systems",
+        "cbc_Note": "generated @2024-05-06T03:19:09.003169+00:00 with xl2roefact by RENware Software Systems",
         "cbc_TaxPointDate": "2023-11-25"
     },
     "excel_original_data": {
         "invoice_footer_area": {
             "end_cell": [
                 49,
                 8
@@ -485,15 +485,15 @@
         "invoice_max_rows": 49,
         "invoice_worksheet": "Factura(Invoice)",
         "items_table_start_cell": [
             29,
             1
         ],
         "items_table_start_marker": "No. crt.",
-        "last_processing_time": "2024-05-01T02:36:47.337934+00:00",
+        "last_processing_time": "2024-05-06T03:19:09.002798+00:00",
         "map_JSONkeys_XMLtags": [
             [
                 "cac_InvoiceLine",
                 "cac:InvoiceLine"
             ],
             [
                 "cac_Item",
```

### Comparing `xl2roefact-0.7rc1/tests/Fact_Petrom_11017969.xlsx` & `xl2roefact-0.7rc2/tests/Fact_Petrom_11017969.xlsx`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.7rc1/tests/Fact_Petrom_11017969.xml` & `xl2roefact-0.7rc2/tests/Fact_Petrom_11017969.xml`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.7rc1/tests/_test_results.txt` & `xl2roefact-0.7rc2/tests/_test_results.txt`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.7rc1/tests/fact_RENF1004.json` & `xl2roefact-0.7rc2/tests/fact_RENF1004.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9857142857142858%*

 * *Differences: {"'Invoice'": "{'cbc_Note': 'generated @2024-05-06T03:19:09.081098+00:00 with xl2roefact by "*

 * *              "RENware Software Systems'}",*

 * * "'meta_info'": "{'last_processing_time': '2024-05-06T03:19:09.080691+00:00'}"}*

```diff
@@ -198,15 +198,15 @@
             "cbc_TaxAmount": 7389.15
         },
         "cbc_DocumentCurrencyCode": "RON",
         "cbc_DueDate": "2023-09-27",
         "cbc_ID": "RENF-1004",
         "cbc_InvoiceTypeCode": "380",
         "cbc_IssueDate": "2023-08-28",
-        "cbc_Note": "generated @2024-05-01T02:36:47.415605+00:00 with xl2roefact by RENware Software Systems",
+        "cbc_Note": "generated @2024-05-06T03:19:09.081098+00:00 with xl2roefact by RENware Software Systems",
         "cbc_TaxPointDate": "2023-09-25"
     },
     "excel_original_data": {
         "invoice_footer_area": {
             "end_cell": [
                 31,
                 9
@@ -560,15 +560,15 @@
         "invoice_max_rows": 31,
         "invoice_worksheet": "FACTURA FINALA",
         "items_table_start_cell": [
             20,
             1
         ],
         "items_table_start_marker": "#",
-        "last_processing_time": "2024-05-01T02:36:47.415171+00:00",
+        "last_processing_time": "2024-05-06T03:19:09.080691+00:00",
         "map_JSONkeys_XMLtags": [
             [
                 "cac_InvoiceLine",
                 "cac:InvoiceLine"
             ],
             [
                 "cac_Item",
```

### Comparing `xl2roefact-0.7rc1/tests/fact_RENF1004.xlsx` & `xl2roefact-0.7rc2/tests/fact_RENF1004.xlsx`

 * *Files identical despite different names*

### Comparing `xl2roefact-0.7rc1/PKG-INFO` & `xl2roefact-0.7rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xl2roefact
-Version: 0.7rc1
+Version: 0.7rc2
 Summary: Excel invoices data retrieve, export & upload to RO E-Fact system
 Author-Email: Petre Iordanescu <petre.iordanescu@gmail.com>, RENware Software Systems <renware.systems@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

