# Comparing `tmp/pdftext-0.3.5.tar.gz` & `tmp/pdftext-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdftext-0.3.5.tar", max compression
+gzip compressed data, was "pdftext-0.3.6.tar", max compression
```

## Comparing `pdftext-0.3.5.tar` & `pdftext-0.3.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11269 2024-05-02 23:57:18.410537 pdftext-0.3.5/LICENSE
--rw-r--r--   0        0        0     7170 2024-05-02 23:57:18.410537 pdftext-0.3.5/README.md
--rw-r--r--   0        0        0     1726 2024-05-02 23:57:18.410537 pdftext-0.3.5/extract_text.py
--rw-r--r--   0        0        0    14097 2024-05-02 23:57:18.410537 pdftext-0.3.5/models/dt.joblib
--rw-r--r--   0        0        0     2426 2024-05-02 23:57:18.410537 pdftext-0.3.5/pdftext/extraction.py
--rw-r--r--   0        0        0     7212 2024-05-02 23:57:18.410537 pdftext-0.3.5/pdftext/inference.py
--rw-r--r--   0        0        0      153 2024-05-02 23:57:18.410537 pdftext-0.3.5/pdftext/model.py
--rw-r--r--   0        0        0     3817 2024-05-02 23:57:18.410537 pdftext-0.3.5/pdftext/pdf/chars.py
--rw-r--r--   0        0        0     4613 2024-05-02 23:57:18.410537 pdftext-0.3.5/pdftext/pdf/utils.py
--rw-r--r--   0        0        0     3222 2024-05-02 23:57:18.410537 pdftext-0.3.5/pdftext/postprocessing.py
--rw-r--r--   0        0        0      488 2024-05-02 23:57:18.410537 pdftext-0.3.5/pdftext/settings.py
--rw-r--r--   0        0        0      856 2024-05-02 23:57:18.414537 pdftext-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     8146 1970-01-01 00:00:00.000000 pdftext-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11269 2024-05-06 17:27:02.808858 pdftext-0.3.6/LICENSE
+-rw-r--r--   0        0        0     7170 2024-05-06 17:27:02.808858 pdftext-0.3.6/README.md
+-rw-r--r--   0        0        0     1726 2024-05-06 17:27:02.808858 pdftext-0.3.6/extract_text.py
+-rw-r--r--   0        0        0    14097 2024-05-06 17:27:02.808858 pdftext-0.3.6/models/dt.joblib
+-rw-r--r--   0        0        0     2426 2024-05-06 17:27:02.808858 pdftext-0.3.6/pdftext/extraction.py
+-rw-r--r--   0        0        0     7212 2024-05-06 17:27:02.812858 pdftext-0.3.6/pdftext/inference.py
+-rw-r--r--   0        0        0      153 2024-05-06 17:27:02.812858 pdftext-0.3.6/pdftext/model.py
+-rw-r--r--   0        0        0     3877 2024-05-06 17:27:02.812858 pdftext-0.3.6/pdftext/pdf/chars.py
+-rw-r--r--   0        0        0     4613 2024-05-06 17:27:02.812858 pdftext-0.3.6/pdftext/pdf/utils.py
+-rw-r--r--   0        0        0     3222 2024-05-06 17:27:02.812858 pdftext-0.3.6/pdftext/postprocessing.py
+-rw-r--r--   0        0        0      488 2024-05-06 17:27:02.812858 pdftext-0.3.6/pdftext/settings.py
+-rw-r--r--   0        0        0      856 2024-05-06 17:27:02.812858 pdftext-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     8146 1970-01-01 00:00:00.000000 pdftext-0.3.6/PKG-INFO
```

### Comparing `pdftext-0.3.5/LICENSE` & `pdftext-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.5/README.md` & `pdftext-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.5/extract_text.py` & `pdftext-0.3.6/extract_text.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.5/models/dt.joblib` & `pdftext-0.3.6/models/dt.joblib`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.5/pdftext/extraction.py` & `pdftext-0.3.6/pdftext/extraction.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.5/pdftext/inference.py` & `pdftext-0.3.6/pdftext/inference.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.5/pdftext/pdf/chars.py` & `pdftext-0.3.6/pdftext/pdf/chars.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                 prev_fontflags = fontflags
                 fontname, fontflags = get_fontname(text_page, i)
                 if (fontname != prev_fontname or fontflags != prev_fontflags) and i > 0:
                     update_previous_fonts(text_chars, i, prev_fontname, prev_fontflags, text_page, fontname_sample_freq)
 
             rotation = pdfium_c.FPDFText_GetCharAngle(text_page, i)
             rotation = rotation * 180 / math.pi # convert from radians to degrees
-            coords = text_page.get_charbox(i, loose=True)
+            coords = text_page.get_charbox(i, loose=rotation == 0) # Loose doesn't work properly when page is rotated
             device_coords = page_bbox_to_device_bbox(page, coords, page_width, page_height, bl_origin, page_rotation, normalize=True)
 
             char_info = {
                 "font": {
                     "size": fontsize,
                     "weight": fontweight,
                     "name": fontname,
```

### Comparing `pdftext-0.3.5/pdftext/pdf/utils.py` & `pdftext-0.3.6/pdftext/pdf/utils.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.5/pdftext/postprocessing.py` & `pdftext-0.3.6/pdftext/postprocessing.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.5/pyproject.toml` & `pdftext-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdftext"
-version = "0.3.5"
+version = "0.3.6"
 description = "Extract structured text from pdfs quickly"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/VikParuchuri/pdftext"
 keywords = ["pdf", "text", "extraction"]
 packages = [
```

### Comparing `pdftext-0.3.5/PKG-INFO` & `pdftext-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdftext
-Version: 0.3.5
+Version: 0.3.6
 Summary: Extract structured text from pdfs quickly
 Home-page: https://github.com/VikParuchuri/pdftext
 License: Apache-2.0
 Keywords: pdf,text,extraction
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
```

