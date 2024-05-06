# Comparing `tmp/pih-doc-0.13.tar.gz` & `tmp/pih-doc-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-doc-0.13.tar", last modified: Wed Apr 10 01:38:39 2024, max compression
+gzip compressed data, was "pih-doc-0.14.tar", last modified: Mon May  6 00:47:47 2024, max compression
```

## Comparing `pih-doc-0.13.tar` & `pih-doc-0.14.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 01:38:40.027397 pih-doc-0.13/
-drwxrwxrwx   0        0        0        0 2024-04-10 01:38:39.640781 pih-doc-0.13/DocsService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-doc-0.13/DocsService/__init__.py
--rw-rw-rw-   0        0        0      146 2024-02-13 08:06:49.000000 pih-doc-0.13/DocsService/__main__.py
--rw-rw-rw-   0        0        0    41330 2024-02-09 18:14:29.000000 pih-doc-0.13/DocsService/api.py
--rw-rw-rw-   0        0        0      536 2024-01-15 10:05:42.000000 pih-doc-0.13/DocsService/api_test.py
--rw-rw-rw-   0        0        0     1634 2024-04-10 00:00:05.000000 pih-doc-0.13/DocsService/const.py
--rw-rw-rw-   0        0        0     5275 2024-03-11 13:46:49.000000 pih-doc-0.13/DocsService/service.py
--rw-rw-rw-   0        0        0      729 2024-02-17 13:43:10.000000 pih-doc-0.13/DocsService/tools.py
--rw-rw-rw-   0        0        0      595 2024-04-10 01:38:40.007807 pih-doc-0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 01:38:39.976558 pih-doc-0.13/pih_doc.egg-info/
--rw-rw-rw-   0        0        0      595 2024-04-10 01:38:38.000000 pih-doc-0.13/pih_doc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-04-10 01:38:39.000000 pih-doc-0.13/pih_doc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 01:38:39.000000 pih-doc-0.13/pih_doc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-10 01:38:39.000000 pih-doc-0.13/pih_doc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      123 2024-04-10 01:38:39.000000 pih-doc-0.13/pih_doc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-10 01:38:39.000000 pih-doc-0.13/pih_doc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 01:38:40.043037 pih-doc-0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 00:47:47.935872 pih-doc-0.14/
+drwxrwxrwx   0        0        0        0 2024-05-06 00:47:47.540748 pih-doc-0.14/DocsService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-doc-0.14/DocsService/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-02-13 08:06:49.000000 pih-doc-0.14/DocsService/__main__.py
+-rw-rw-rw-   0        0        0    41563 2024-05-06 00:47:28.000000 pih-doc-0.14/DocsService/api.py
+-rw-rw-rw-   0        0        0     1634 2024-05-06 00:45:54.000000 pih-doc-0.14/DocsService/const.py
+-rw-rw-rw-   0        0        0     5242 2024-04-10 12:59:25.000000 pih-doc-0.14/DocsService/service.py
+-rw-rw-rw-   0        0        0      729 2024-02-17 13:43:10.000000 pih-doc-0.14/DocsService/tools.py
+-rw-rw-rw-   0        0        0      595 2024-05-06 00:47:47.904767 pih-doc-0.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 00:47:47.873311 pih-doc-0.14/pih_doc.egg-info/
+-rw-rw-rw-   0        0        0      595 2024-05-06 00:47:47.000000 pih-doc-0.14/pih_doc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2024-05-06 00:47:47.000000 pih-doc-0.14/pih_doc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 00:47:47.000000 pih-doc-0.14/pih_doc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-06 00:47:47.000000 pih-doc-0.14/pih_doc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      123 2024-05-06 00:47:47.000000 pih-doc-0.14/pih_doc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-06 00:47:47.000000 pih-doc-0.14/pih_doc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 00:47:47.935872 pih-doc-0.14/setup.cfg
```

### Comparing `pih-doc-0.13/DocsService/api.py` & `pih-doc-0.14/DocsService/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,44 @@
+from barcode.writer import ImageWriter
+from PIL import ImageDraw, ImageFont
+from qrcode import QRCode, constants
+from collections import defaultdict
 from dataclasses import dataclass
-import io
-from os import path
-from typing import Any
+from gkeepapi import Keep, _node
 from mailmerge import MailMerge
-from PIL import ImageDraw, ImageFont
-import PIL.Image as mImage
+import plotly.graph_objs as go
+from xlutils.copy import copy
+from datetime import datetime
 from PIL.Image import Image
-from qrcode import QRCode, constants
-import xlrd
+import PIL.Image as mImage
+from typing import Any
+from os import path
 import xlsxwriter
 import openpyxl
 import barcode
-from xlutils.copy import copy
-from barcode.writer import ImageWriter
-from collections import defaultdict
-from datetime import datetime
-from gkeepapi import Keep, _node
+import xlrd
+import io
+
 
 from pih import A
-from pih.consts.errors import IncorrectInputFile
+from DocsService.const import *
 from pih.collections import (
     Note,
     Result,
     FullName,
     FieldItem,
     LoginPasswordPair,
     TimeSeriesStatistics,
     TimeTrackingResultByDate,
     TimeTrackingResultByPerson,
     CTIndicationsValueContainer,
     TimeTrackingResultByDivision,
 )
 from pih.tools import js, j, nn, ne, n, e, nl
-from DocsService.const import *
-import plotly.graph_objs as go
+from pih.consts.errors import IncorrectInputFile
 
 
 @dataclass
 class BarCodeData:
     value: str
     name: str
 
@@ -168,17 +169,17 @@
                         break
                 if type_index != -1:
                     count: int = 24
                     if type_index == 1:
                         count = 7 * 24
                     elif type_index == 2:
                         count = 30 * 24
-                    data: list[
-                        CTIndicationsValueContainer
-                    ] = A.R_IND.last_ct_value_containers(False, count).data
+                    data: list[CTIndicationsValueContainer] = (
+                        A.R_IND.last_ct_value_containers(False, count).data
+                    )
                     figure = go.Figure()
                     x: list[datetime] = A.D.map(lambda item: item.timestamp, data)
                     figure.add_trace(
                         go.Scatter(
                             x=x,
                             mode="lines",
                             y=A.D.map(lambda item: item.temperature, data),
@@ -280,17 +281,17 @@
                 worksheet.set_column("G:G", 15)
                 worksheet.set_column("H:H", 20)
                 person_map: list[TimeTrackingResultByPerson] = []
                 division_person_map: dict[str, str] = defaultdict(list)
                 for division_item in result_data_list:
                     if division_item.name is not None:
                         for person_item in division_item.list:
-                            division_person_map[
-                                person_item.tab_number
-                            ] = division_item.name
+                            division_person_map[person_item.tab_number] = (
+                                division_item.name
+                            )
                             person_map.append(person_item)
                 index: int = 0
                 for item in person_map:
                     for date_item in item.list:
                         date: TimeTrackingResultByDate = date_item
                         worksheet.write_string(
                             index, 0, division_person_map[item.tab_number]
@@ -298,17 +299,19 @@
                         worksheet.write_string(index, 1, item.full_name)
                         worksheet.write_string(index, 2, date.date)
                         worksheet.write_string(index, 3, date.enter_time or "")
                         worksheet.write_string(index, 4, date.exit_time or "")
                         worksheet.write_string(
                             index,
                             5,
-                            ""
-                            if date.duration is None
-                            else self.to_hh_mm(date.duration),
+                            (
+                                ""
+                                if date.duration is None
+                                else self.to_hh_mm(date.duration)
+                            ),
                         )
                         index += 1
             else:
                 title_format = workbook.add_format(
                     {
                         "bold": 1,
                         "border": 1,
@@ -661,19 +664,21 @@
     def is_excel_old(self, file_path: str) -> bool:
         return A.PTH.get_extension(file_path) == A.CT_F_E.EXCEL_OLD
 
     def inventory_report_columns_is_exists(self, report_file_path: str) -> bool:
         old_format: bool = self.is_excel_old(report_file_path)
         return (
             self.get_inventory_report_columns(
-                xlrd.open_workbook(report_file_path).sheet_by_index(0)
-                if old_format
-                else openpyxl.load_workbook(
-                    report_file_path, data_only=True, read_only=True
-                ).active,
+                (
+                    xlrd.open_workbook(report_file_path).sheet_by_index(0)
+                    if old_format
+                    else openpyxl.load_workbook(
+                        report_file_path, data_only=True, read_only=True
+                    ).active
+                ),
                 old_format,
             )
             is not None
         )
 
     def inventory_report(
         self, report_file_path: str, open_for_edit: bool = False
@@ -841,19 +846,19 @@
         polibase = polibase or pc
         email = email or pc
         #
         internal_email = email.login.find(web_site_name) != -1
         if not internal_email:
             email_address = email.login[email.login.find("@") + 1 :]
         #
-        template_path: str | None = None
+        template_file_name: str | None = None
         if polibase.login == pc.login:
-            template_path = "Template1.docx"
+            template_file_name = "Template1.docx"
         else:
-            template_path = "Template2.docx"
+            template_file_name = "Template2.docx"
         #
         pc_password = pc.password
         polibase_password = polibase.password or pc_password
         email_password = email.password or polibase_password
         #
         password_caption_items = [[], [], []]
         password_text_items = ["", "", ""]
@@ -896,32 +901,34 @@
                                     ":",
                                 )
                             )
                         )
                         password_text += password
                         password_text += nl(count=password_caption_item_len)
             if password_caption == "":
-                template_path = "Template0.docx"
+                template_file_name = "Template0.docx"
 
-        full_template_path = A.PTH.get_current_full_path(template_path)
+        template_file_path: str = A.PTH.join(
+            A.PTH.FACADE.SERVICE_FILES(SD.standalone_name), template_file_name
+        )
 
         def fill_template_internal(
-            template_path: str,
+            template_file_path: str,
             name: str,
             tab_number: str,
             email_address: str,
             web_site: str,
             date_now_string: str,
             password_caption: str,
             password_text: str,
             pc: LoginPasswordPair,
             polibase: LoginPasswordPair,
             email: LoginPasswordPair,
         ) -> MailMerge:
-            document = MailMerge(template_path)
+            document = MailMerge(template_file_path)
             document.merge(
                 Name=name,
                 Date=date_now_string,
                 TabNumber=tab_number,
                 Login=pc.login,
                 WebSite=web_site,
                 EMailAddress=email_address,
@@ -929,15 +936,15 @@
                 PolibaseLogin=polibase.login,
                 PasswordCaption=password_caption,
                 PasswordText=password_text,
             )
             return document
 
         return fill_template_internal(
-            full_template_path,
+            template_file_path,
             name,
             tab_number,
             email_address,
             web_site,
             date_now_string,
             password_caption,
             password_text,
```

### Comparing `pih-doc-0.13/DocsService/const.py` & `pih-doc-0.14/DocsService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     QUANTITY_COLUMN_NAME: str = "фактическое наличие"
     NAME_MAX_LENTH: int = 120
     QUANTITY_NOT_SET: str = "-"
 
 
 HOST = Hosts.DC2
 
-VERSION: str = "0.13"
+VERSION: str = "0.14"
 
 PACKAGES: tuple[str, ...] = (
     "xlsxwriter",
     "xlrd",
     "xlutils",
     "openpyxl",
     "python-barcode",
```

### Comparing `pih-doc-0.13/DocsService/service.py` & `pih-doc-0.14/DocsService/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 
 
 def start(as_standalone: bool = False) -> None:
 
     if A.U.for_service(SD, as_standalone=as_standalone):
         from datetime import datetime
         import grpc
-        from pih.collections import FullName, LoginPasswordPair, Result, Note
-        from pih.consts.errors import IncorrectInputFile
-        from pih.rpc import RPC
         from pih.tools import ParameterList
         from DocsService.api import DocumentApi
+        from pih.consts.errors import IncorrectInputFile
+        from pih.collections import FullName, LoginPasswordPair, Result, Note
 
         api: DocumentApi = DocumentApi(ISOLATED)
 
         def service_call_handler(sc: SC, pl: ParameterList, context) -> Any:
             if sc == SC.create_statistics_chart:
                 return api.create_statistics_chart(pl.next())
             if sc == SC.create_user_document:
```

### Comparing `pih-doc-0.13/DocsService/tools.py` & `pih-doc-0.14/DocsService/tools.py`

 * *Files identical despite different names*

### Comparing `pih-doc-0.13/PKG-INFO` & `pih-doc-0.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pih-doc
-Version: 0.13
+Version: 0.14
 Summary: PIH Documents service package
 Home-page: https://pacifichosp.com/
 Author: Nikita Karachentsev
 Author-email: it@pacifichosp.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: ipih
```

### Comparing `pih-doc-0.13/pih_doc.egg-info/PKG-INFO` & `pih-doc-0.14/pih_doc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pih-doc
-Version: 0.13
+Version: 0.14
 Summary: PIH Documents service package
 Home-page: https://pacifichosp.com/
 Author: Nikita Karachentsev
 Author-email: it@pacifichosp.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: ipih
```

