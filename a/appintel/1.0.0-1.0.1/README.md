# Comparing `tmp/appintel-1.0.0.tar.gz` & `tmp/appintel-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appintel-1.0.0.tar", max compression
+gzip compressed data, was "appintel-1.0.1.tar", max compression
```

## Comparing `appintel-1.0.0.tar` & `appintel-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35147 2024-05-05 16:55:39.804868 appintel-1.0.0/LICENSE
--rw-r--r--   0        0        0     1558 2024-05-05 16:55:39.805276 appintel-1.0.0/README.md
--rw-r--r--   0        0        0        1 2024-05-05 16:55:39.805480 appintel-1.0.0/appintel/__init__.py
--rw-r--r--   0        0        0       35 2024-05-06 03:37:07.369923 appintel-1.0.0/appintel/__main__.py
--rw-r--r--   0        0        0     6221 2024-05-06 03:47:47.375673 appintel-1.0.0/appintel/appintel.py
--rw-r--r--   0        0        0      689 2024-05-06 03:37:41.056445 appintel-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 appintel-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-05-05 16:55:39.804868 appintel-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1519 2024-05-06 03:54:06.750378 appintel-1.0.1/README.md
+-rw-r--r--   0        0        0        1 2024-05-05 16:55:39.805480 appintel-1.0.1/appintel/__init__.py
+-rw-r--r--   0        0        0       35 2024-05-06 03:37:07.369923 appintel-1.0.1/appintel/__main__.py
+-rw-r--r--   0        0        0     6221 2024-05-06 03:54:19.953210 appintel-1.0.1/appintel/appintel.py
+-rw-r--r--   0        0        0      689 2024-05-06 03:54:38.616332 appintel-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2397 1970-01-01 00:00:00.000000 appintel-1.0.1/PKG-INFO
```

### Comparing `appintel-1.0.0/LICENSE` & `appintel-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `appintel-1.0.0/README.md` & `appintel-1.0.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-# itunizer
-🎵🎵🎵🎵🎵🎵🎵🎵🎵🎵
+# appintel
 
 ## What
 
-Gather market data into a machine readable form from iTunes store data. 
+Gather market data into a machine readable form from iTunes store data.
 
 ## Install
 
-The easiest way is pip: `pip3 install itunizer`. 
+The easiest way is pip: `pip3 install appintel`.
 
 ## Usage
 
-Use the `-h` for options:   
+Use the `-h` for options:
 
-```
+```bash
 $ itunizer -h
-usage: itunizer [-h] [-s SEARCH_TERM] [-c CATEGORY_LOCATION] [-p] [-n] [-t]
+usage: appintel [-h] [-s SEARCH_TERM] [-c CATEGORY_LOCATION] [-p] [-n] [-t]
                 [--country STORE_COUNTRY] [--version]
 
-collects and processes itunes data including ibook, application, and other
+collects and processes app store data including ibook, application, and other
 store items with metadata, example: itunizer -c ibook -s "corn" -t
 
 optional arguments:
   -h, --help            show this help message and exit
   -s SEARCH_TERM, --search SEARCH_TERM
                         search term to search itunes store for (default:
                         nginx)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `appintel-1.0.0/appintel/appintel.py` & `appintel-1.0.1/appintel/appintel.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from pprint import pprint
 from statistics import mean, median
 
 import pandas as pd
 import requests
 
 # globals
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 logo = """
 +-------------------------------------+
 |                         --\         |
 |                        /   -\       |
 |                       /      -\     |
 |                      /         -    |
 |    \                /               |
```

### Comparing `appintel-1.0.0/pyproject.toml` & `appintel-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "appintel"
-version = "1.0.0"
+version = "1.0.1"
 description = "A command line tool to search and compare prices of apps and music on the Apple Store"
 authors = ["James Campbell <james@jamescampbell.us>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 argparse = "^1.4.0"
```

### Comparing `appintel-1.0.0/PKG-INFO` & `appintel-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appintel
-Version: 1.0.0
+Version: 1.0.1
 Summary: A command line tool to search and compare prices of apps and music on the Apple Store
 Author: James Campbell
 Author-email: james@jamescampbell.us
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -17,35 +17,34 @@
 Requires-Dist: python-dateutil (>=2.9.0.post0,<3.0.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Requires-Dist: urllib3 (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
 
-# itunizer
-🎵🎵🎵🎵🎵🎵🎵🎵🎵🎵
+# appintel
 
 ## What
 
-Gather market data into a machine readable form from iTunes store data. 
+Gather market data into a machine readable form from iTunes store data.
 
 ## Install
 
-The easiest way is pip: `pip3 install itunizer`. 
+The easiest way is pip: `pip3 install appintel`.
 
 ## Usage
 
-Use the `-h` for options:   
+Use the `-h` for options:
 
-```
+```bash
 $ itunizer -h
-usage: itunizer [-h] [-s SEARCH_TERM] [-c CATEGORY_LOCATION] [-p] [-n] [-t]
+usage: appintel [-h] [-s SEARCH_TERM] [-c CATEGORY_LOCATION] [-p] [-n] [-t]
                 [--country STORE_COUNTRY] [--version]
 
-collects and processes itunes data including ibook, application, and other
+collects and processes app store data including ibook, application, and other
 store items with metadata, example: itunizer -c ibook -s "corn" -t
 
 optional arguments:
   -h, --help            show this help message and exit
   -s SEARCH_TERM, --search SEARCH_TERM
                         search term to search itunes store for (default:
                         nginx)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

