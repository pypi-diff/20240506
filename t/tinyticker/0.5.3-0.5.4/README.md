# Comparing `tmp/tinyticker-0.5.3.tar.gz` & `tmp/tinyticker-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.5.3.tar", max compression
+gzip compressed data, was "tinyticker-0.5.4.tar", max compression
```

## Comparing `tinyticker-0.5.3.tar` & `tinyticker-0.5.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1068 2024-05-06 18:01:20.863834 tinyticker-0.5.3/LICENSE
--rw-r--r--   0        0        0     3863 2024-05-06 18:01:20.863834 tinyticker-0.5.3/README.md
--rw-r--r--   0        0        0      899 2024-05-06 18:01:20.863834 tinyticker-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      207 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/__init__.py
--rw-r--r--   0        0        0     6196 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/__main__.py
--rw-r--r--   0        0        0     1773 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/config.py
--rw-r--r--   0        0        0     8880 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/display.py
--rw-r--r--   0        0        0      345 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/paths.py
--rw-r--r--   0        0        0    15609 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/ticker.py
--rw-r--r--   0        0        0     2476 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/utils.py
--rw-r--r--   0        0        0      318 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1259 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     8376 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    11895 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14581 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10457 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     5835 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6627 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5690 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0     3148 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/waveshare_lib/epdconfig.py
--rw-r--r--   0        0        0     1283 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2547 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     6610 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/web/app.py
--rw-r--r--   0        0        0     2909 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/web/command.py
--rw-r--r--   0        0        0   274777 2024-05-06 18:01:20.867834 tinyticker-0.5.3/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-06 18:01:20.871834 tinyticker-0.5.3/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-06 18:01:20.871834 tinyticker-0.5.3/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-06 18:01:20.871834 tinyticker-0.5.3/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    15426 2024-05-06 18:01:20.871834 tinyticker-0.5.3/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0      787 2024-05-06 18:01:20.871834 tinyticker-0.5.3/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-06 18:01:20.871834 tinyticker-0.5.3/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-06 18:01:20.871834 tinyticker-0.5.3/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     1369 2024-05-06 18:01:20.871834 tinyticker-0.5.3/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     5111 1970-01-01 00:00:00.000000 tinyticker-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-06 18:05:56.712088 tinyticker-0.5.4/LICENSE
+-rw-r--r--   0        0        0     3863 2024-05-06 18:05:56.712088 tinyticker-0.5.4/README.md
+-rw-r--r--   0        0        0      899 2024-05-06 18:05:56.712088 tinyticker-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-05-06 18:05:56.712088 tinyticker-0.5.4/tinyticker/__init__.py
+-rw-r--r--   0        0        0     6196 2024-05-06 18:05:56.712088 tinyticker-0.5.4/tinyticker/__main__.py
+-rw-r--r--   0        0        0     1773 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/config.py
+-rw-r--r--   0        0        0     8880 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/display.py
+-rw-r--r--   0        0        0      345 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/paths.py
+-rw-r--r--   0        0        0    15609 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/ticker.py
+-rw-r--r--   0        0        0     2476 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/utils.py
+-rw-r--r--   0        0        0      318 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1259 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     8376 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    11895 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14581 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10457 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     5835 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6627 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5690 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0     3148 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/waveshare_lib/epdconfig.py
+-rw-r--r--   0        0        0     1283 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2547 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     6610 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/web/app.py
+-rw-r--r--   0        0        0     2909 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/web/command.py
+-rw-r--r--   0        0        0   274777 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    15426 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0      787 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-06 18:05:56.716088 tinyticker-0.5.4/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-06 18:05:56.720088 tinyticker-0.5.4/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     1369 2024-05-06 18:05:56.720088 tinyticker-0.5.4/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     5111 1970-01-01 00:00:00.000000 tinyticker-0.5.4/PKG-INFO
```

### Comparing `tinyticker-0.5.3/LICENSE` & `tinyticker-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/README.md` & `tinyticker-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/pyproject.toml` & `tinyticker-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.5.3"
+version = "0.5.4"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.5.3/tinyticker/__main__.py` & `tinyticker-0.5.4/tinyticker/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/config.py` & `tinyticker-0.5.4/tinyticker/config.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/display.py` & `tinyticker-0.5.4/tinyticker/display.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/ticker.py` & `tinyticker-0.5.4/tinyticker/ticker.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/utils.py` & `tinyticker-0.5.4/tinyticker/utils.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.5.4/tinyticker/waveshare_lib/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.5.4/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.5.4/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.5.4/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.5.4/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.5.4/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.5.4/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.5.4/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/waveshare_lib/epdconfig.py` & `tinyticker-0.5.4/tinyticker/waveshare_lib/epdconfig.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/waveshare_lib/models.py` & `tinyticker-0.5.4/tinyticker/waveshare_lib/models.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/web/__main__.py` & `tinyticker-0.5.4/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/web/app.py` & `tinyticker-0.5.4/tinyticker/web/app.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/web/command.py` & `tinyticker-0.5.4/tinyticker/web/command.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.5.4/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.5.4/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.5.4/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.5.4/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/web/templates/index.html` & `tinyticker-0.5.4/tinyticker/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/web/templates/js/index.js` & `tinyticker-0.5.4/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.5.4/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.5.4/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/tinyticker/web/templates/logfiles.html` & `tinyticker-0.5.4/tinyticker/web/templates/logfiles.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.3/PKG-INFO` & `tinyticker-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.5.3
+Version: 0.5.4
 Summary: A tiny Raspberry Pi powered ePaper ticker.
 Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT
 Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyticker Version: 0.5.3 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.5.4 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

