# Comparing `tmp/cicc_excel-0.4.0.tar.gz` & `tmp/cicc_excel-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cicc_excel-0.4.0.tar", last modified: Mon Jun  5 07:34:41 2023, max compression
+gzip compressed data, was "cicc_excel-0.4.1.tar", last modified: Mon May  6 11:09:02 2024, max compression
```

## Comparing `cicc_excel-0.4.0.tar` & `cicc_excel-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 07:34:41.412030 cicc_excel-0.4.0/
--rw-rw-rw-   0        0        0     1093 2023-06-05 07:08:14.000000 cicc_excel-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     1876 2023-06-05 07:34:41.412030 cicc_excel-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1274 2023-06-05 07:08:14.000000 cicc_excel-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 07:34:41.402358 cicc_excel-0.4.0/cicc_excel/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:08:14.000000 cicc_excel-0.4.0/cicc_excel/__init__.py
--rw-rw-rw-   0        0        0    14325 2023-06-05 07:26:41.000000 cicc_excel-0.4.0/cicc_excel/excelwriter.py
-drwxrwxrwx   0        0        0        0 2023-06-05 07:34:41.412030 cicc_excel-0.4.0/cicc_excel.egg-info/
--rw-rw-rw-   0        0        0     1876 2023-06-05 07:34:40.000000 cicc_excel-0.4.0/cicc_excel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-06-05 07:34:41.000000 cicc_excel-0.4.0/cicc_excel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 07:34:40.000000 cicc_excel-0.4.0/cicc_excel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-05 07:34:41.000000 cicc_excel-0.4.0/cicc_excel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-05 07:34:41.000000 cicc_excel-0.4.0/cicc_excel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 07:34:41.412030 cicc_excel-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      867 2023-06-05 07:27:18.000000 cicc_excel-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:09:02.661906 cicc_excel-0.4.1/
+-rw-rw-rw-   0        0        0     1093 2024-05-06 11:03:47.000000 cicc_excel-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     1887 2024-05-06 11:09:02.661906 cicc_excel-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1274 2024-05-06 11:03:47.000000 cicc_excel-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 11:09:02.646283 cicc_excel-0.4.1/cicc_excel/
+-rw-rw-rw-   0        0        0        0 2024-05-06 11:03:47.000000 cicc_excel-0.4.1/cicc_excel/__init__.py
+-rw-rw-rw-   0        0        0    14641 2024-05-06 11:03:47.000000 cicc_excel-0.4.1/cicc_excel/excelwriter.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:09:02.661906 cicc_excel-0.4.1/cicc_excel.egg-info/
+-rw-rw-rw-   0        0        0     1887 2024-05-06 11:09:02.000000 cicc_excel-0.4.1/cicc_excel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2024-05-06 11:09:02.000000 cicc_excel-0.4.1/cicc_excel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 11:09:02.000000 cicc_excel-0.4.1/cicc_excel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-06 11:09:02.000000 cicc_excel-0.4.1/cicc_excel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-06 11:09:02.000000 cicc_excel-0.4.1/cicc_excel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 11:09:02.661906 cicc_excel-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      867 2024-05-06 11:03:47.000000 cicc_excel-0.4.1/setup.py
```

### Comparing `cicc_excel-0.4.0/LICENSE` & `cicc_excel-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cicc_excel-0.4.0/PKG-INFO` & `cicc_excel-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cicc_excel
-Version: 0.4.0
+Version: 0.4.1
 Summary: Library of export pandas into excel for CICCers
 Home-page: https://github.com/nyuspc/cicc_excel
 Author: Pengcheng Song
 Author-email: smth_spc@hotmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: xlsxwriter
 
 ## Install
 
 `pip install cicc_excel`
 
 ## How to Use
 
@@ -58,8 +58,7 @@
 #another sheet
 wb.load_data(df3)
 wb.write_data('last_sheet_name')
 
 #save file
 wb.save()
 ```
-
```

### Comparing `cicc_excel-0.4.0/README.md` & `cicc_excel-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cicc_excel-0.4.0/cicc_excel/excelwriter.py` & `cicc_excel-0.4.1/cicc_excel/excelwriter.py`

 * *Files 4% similar despite different names*

```diff
@@ -253,28 +253,34 @@
 
     def hide_col(self, start_col=0, end_col=0, sheet_name='Sheet1'):
         """
         Hide columns.
         """
         ws = self.workbook.get_worksheet_by_name(sheet_name)
         if ws is not None:
-            for col in range(start_col, end_col):
-                ws.set_column(col-1, col, None, None, {'hidden': True})
+            if start_col == end_col:
+                ws.set_column(start_col-1, start_col-1, None, None, {'hidden': True})
+            else:
+                for col in range(start_col, end_col):
+                    ws.set_column(col-1, col, None, None, {'hidden': True})
         else:
             print("Error: worksheets", sheet_name, "not found")
     
     def collapse_col(self, start_col=0, end_col=0, sheet_name='Sheet1'):
         """
         collapse columns.
         """
         ws = self.workbook.get_worksheet_by_name(sheet_name)
         if ws is not None:
         #collapsed note does not work, use hidden + level instead.
-            for col in range(start_col, end_col):
-                ws.set_column(col-1, col, None, None, {'hidden': True, 'level': 1})
+            if start_col == end_col:
+                ws.set_column(start_col-1, start_col-1, None, None, {'hidden': True, 'level': 1})
+            else:
+                for col in range(start_col, end_col):
+                    ws.set_column(col-1, col, None, None, {'hidden': True, 'level': 1})
         else:
             print("Error: worksheets", sheet_name, "not found")
     
     def set_hl_col_by_names(self, col_name, sheet_name, hl_bg_color='#EEECE1', hl_color='#000000'):
         """
         Set col by col name
         """
```

### Comparing `cicc_excel-0.4.0/cicc_excel.egg-info/PKG-INFO` & `cicc_excel-0.4.1/cicc_excel.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
-Name: cicc-excel
-Version: 0.4.0
+Name: cicc_excel
+Version: 0.4.1
 Summary: Library of export pandas into excel for CICCers
 Home-page: https://github.com/nyuspc/cicc_excel
 Author: Pengcheng Song
 Author-email: smth_spc@hotmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: xlsxwriter
 
 ## Install
 
 `pip install cicc_excel`
 
 ## How to Use
 
@@ -58,8 +58,7 @@
 #another sheet
 wb.load_data(df3)
 wb.write_data('last_sheet_name')
 
 #save file
 wb.save()
 ```
-
```

### Comparing `cicc_excel-0.4.0/setup.py` & `cicc_excel-0.4.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cicc_excel",
-    version="0.4.0",
+    version="0.4.1",
     author="Pengcheng Song",
     author_email="smth_spc@hotmail.com",
     description="Library of export pandas into excel for CICCers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nyuspc/cicc_excel",
     install_requires=[
```

