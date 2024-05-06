# Comparing `tmp/autocombobox-1.0.1.tar.gz` & `tmp/autocombobox-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocombobox-1.0.1.tar", last modified: Tue Mar  5 21:34:47 2024, max compression
+gzip compressed data, was "autocombobox-1.0.2.tar", last modified: Mon May  6 15:59:05 2024, max compression
```

## Comparing `autocombobox-1.0.1.tar` & `autocombobox-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-05 21:34:47.411829 autocombobox-1.0.1/
--rw-rw-rw-   0        0        0    35823 2024-03-01 14:21:39.000000 autocombobox-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    42840 2024-03-05 21:34:47.410428 autocombobox-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      935 2024-03-05 21:31:37.000000 autocombobox-1.0.1/README.md
--rw-rw-rw-   0        0        0      812 2024-03-05 21:34:35.000000 autocombobox-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-05 21:34:47.411829 autocombobox-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-05 21:34:47.385147 autocombobox-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-05 21:34:47.391955 autocombobox-1.0.1/src/autocombobox/
--rw-rw-rw-   0        0        0    10138 2024-03-05 21:34:34.000000 autocombobox-1.0.1/src/autocombobox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-05 21:34:47.409428 autocombobox-1.0.1/src/autocombobox.egg-info/
--rw-rw-rw-   0        0        0    42840 2024-03-05 21:34:47.000000 autocombobox-1.0.1/src/autocombobox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-03-05 21:34:47.000000 autocombobox-1.0.1/src/autocombobox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-05 21:34:47.000000 autocombobox-1.0.1/src/autocombobox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-03-05 21:34:47.000000 autocombobox-1.0.1/src/autocombobox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-05 21:34:47.408424 autocombobox-1.0.1/tests/
--rw-rw-rw-   0        0        0     1954 2024-03-05 21:10:25.000000 autocombobox-1.0.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:59:05.589203 autocombobox-1.0.2/
+-rw-rw-rw-   0        0        0    35823 2024-03-01 14:21:39.000000 autocombobox-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    42841 2024-05-06 15:59:05.587198 autocombobox-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      935 2024-03-05 21:31:37.000000 autocombobox-1.0.2/README.md
+-rw-rw-rw-   0        0        0      813 2024-05-06 15:58:33.000000 autocombobox-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 15:59:05.589765 autocombobox-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 15:59:05.552653 autocombobox-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 15:59:05.561454 autocombobox-1.0.2/src/autocombobox/
+-rw-rw-rw-   0        0        0    10138 2024-05-06 15:58:44.000000 autocombobox-1.0.2/src/autocombobox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 15:59:05.584563 autocombobox-1.0.2/src/autocombobox.egg-info/
+-rw-rw-rw-   0        0        0    42841 2024-05-06 15:59:05.000000 autocombobox-1.0.2/src/autocombobox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-05-06 15:59:05.000000 autocombobox-1.0.2/src/autocombobox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 15:59:05.000000 autocombobox-1.0.2/src/autocombobox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-06 15:59:05.000000 autocombobox-1.0.2/src/autocombobox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 15:59:05.582215 autocombobox-1.0.2/tests/
+-rw-rw-rw-   0        0        0     1954 2024-03-05 21:10:25.000000 autocombobox-1.0.2/tests/test.py
```

### Comparing `autocombobox-1.0.1/LICENSE` & `autocombobox-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autocombobox-1.0.1/PKG-INFO` & `autocombobox-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocombobox
-Version: 1.0.1
+Version: 1.0.2
 Summary: Insert a ttk-Combobox into your GUI that allows suggestions based on what the user writes
 Author-email: Matteo Chiesa <matteo.chiesa.mc@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -681,15 +681,15 @@
 Project-URL: Homepage, https://github.com/Church-17/autocombobox
 Keywords: autocombobox,combobox,autocomplete
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.0
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AutoCombobox
 
 AutoCombobox is a ttk widget based on the existing Combobox. It allows the user to write on the Entry field, viewing at the same time the options that the Combobox suggest based on what the user writes.
```

### Comparing `autocombobox-1.0.1/README.md` & `autocombobox-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `autocombobox-1.0.1/pyproject.toml` & `autocombobox-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 [project]
 name = "autocombobox"
 authors = [
     {name = "Matteo Chiesa", email = "matteo.chiesa.mc@gmail.com"}
 ]
 description = "Insert a ttk-Combobox into your GUI that allows suggestions based on what the user writes"
-version = "1.0.1"
+version = "1.0.2"
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["autocombobox", "combobox", "autocomplete"]
-requires-python = ">=3.0"
+requires-python = ">=3.10"
 
 [project.urls]
 Homepage = "https://github.com/Church-17/autocombobox"
```

### Comparing `autocombobox-1.0.1/src/autocombobox/__init__.py` & `autocombobox-1.0.2/src/autocombobox/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections.abc import Callable
 from tkinter import Listbox, Event, Frame
 from tkinter.ttk import Combobox, Scrollbar
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 class AutoCombobox(Combobox):
     """Autocomplete Combobox"""
 
     def __init__(self, *args, **kwargs):
         """Create an Autocomplete ttk Combobox. All the ttk Combobox options are available.
```

### Comparing `autocombobox-1.0.1/src/autocombobox.egg-info/PKG-INFO` & `autocombobox-1.0.2/src/autocombobox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocombobox
-Version: 1.0.1
+Version: 1.0.2
 Summary: Insert a ttk-Combobox into your GUI that allows suggestions based on what the user writes
 Author-email: Matteo Chiesa <matteo.chiesa.mc@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -681,15 +681,15 @@
 Project-URL: Homepage, https://github.com/Church-17/autocombobox
 Keywords: autocombobox,combobox,autocomplete
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.0
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AutoCombobox
 
 AutoCombobox is a ttk widget based on the existing Combobox. It allows the user to write on the Entry field, viewing at the same time the options that the Combobox suggest based on what the user writes.
```

### Comparing `autocombobox-1.0.1/tests/test.py` & `autocombobox-1.0.2/tests/test.py`

 * *Files identical despite different names*

