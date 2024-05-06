# Comparing `tmp/CustomtkinterCodeViewer-0.0.2.tar.gz` & `tmp/CustomtkinterCodeViewer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CustomtkinterCodeViewer-0.0.2.tar", last modified: Sun Nov 19 11:36:52 2023, max compression
+gzip compressed data, was "CustomtkinterCodeViewer-0.0.3.tar", last modified: Mon May  6 12:41:57 2024, max compression
```

## Comparing `CustomtkinterCodeViewer-0.0.2.tar` & `CustomtkinterCodeViewer-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 maheshmaanas   (501) staff       (20)        0 2023-11-19 11:36:52.936951 CustomtkinterCodeViewer-0.0.2/
-drwxr-xr-x   0 maheshmaanas   (501) staff       (20)        0 2023-11-19 11:36:52.936027 CustomtkinterCodeViewer-0.0.2/CustomtkinterCodeViewer/
--rw-r--r--   0 maheshmaanas   (501) staff       (20)     1361 2023-11-17 15:49:04.000000 CustomtkinterCodeViewer-0.0.2/CustomtkinterCodeViewer/CTkCodeViewer.py
--rw-r--r--   0 maheshmaanas   (501) staff       (20)       41 2023-11-17 16:25:20.000000 CustomtkinterCodeViewer-0.0.2/CustomtkinterCodeViewer/__init__.py
-drwxr-xr-x   0 maheshmaanas   (501) staff       (20)        0 2023-11-19 11:36:52.936678 CustomtkinterCodeViewer-0.0.2/CustomtkinterCodeViewer.egg-info/
--rw-r--r--   0 maheshmaanas   (501) staff       (20)     1437 2023-11-19 11:36:52.000000 CustomtkinterCodeViewer-0.0.2/CustomtkinterCodeViewer.egg-info/PKG-INFO
--rw-r--r--   0 maheshmaanas   (501) staff       (20)      329 2023-11-19 11:36:52.000000 CustomtkinterCodeViewer-0.0.2/CustomtkinterCodeViewer.egg-info/SOURCES.txt
--rw-r--r--   0 maheshmaanas   (501) staff       (20)        1 2023-11-19 11:36:52.000000 CustomtkinterCodeViewer-0.0.2/CustomtkinterCodeViewer.egg-info/dependency_links.txt
--rw-r--r--   0 maheshmaanas   (501) staff       (20)       33 2023-11-19 11:36:52.000000 CustomtkinterCodeViewer-0.0.2/CustomtkinterCodeViewer.egg-info/requires.txt
--rw-r--r--   0 maheshmaanas   (501) staff       (20)       24 2023-11-19 11:36:52.000000 CustomtkinterCodeViewer-0.0.2/CustomtkinterCodeViewer.egg-info/top_level.txt
--rw-r--r--   0 maheshmaanas   (501) staff       (20)     1437 2023-11-19 11:36:52.936837 CustomtkinterCodeViewer-0.0.2/PKG-INFO
--rw-r--r--   0 maheshmaanas   (501) staff       (20)      902 2023-11-17 16:36:02.000000 CustomtkinterCodeViewer-0.0.2/README.md
--rw-r--r--   0 maheshmaanas   (501) staff       (20)       38 2023-11-19 11:36:52.936980 CustomtkinterCodeViewer-0.0.2/setup.cfg
--rw-r--r--   0 maheshmaanas   (501) staff       (20)     1170 2023-11-19 11:27:03.000000 CustomtkinterCodeViewer-0.0.2/setup.py
+drwxr-xr-x   0 maheshmaanas   (501) staff       (20)        0 2024-05-06 12:41:57.909144 CustomtkinterCodeViewer-0.0.3/
+drwxr-xr-x   0 maheshmaanas   (501) staff       (20)        0 2024-05-06 12:41:57.908143 CustomtkinterCodeViewer-0.0.3/CustomtkinterCodeViewer/
+-rw-r--r--   0 maheshmaanas   (501) staff       (20)     1361 2023-11-17 15:49:04.000000 CustomtkinterCodeViewer-0.0.3/CustomtkinterCodeViewer/CTkCodeViewer.py
+-rw-r--r--   0 maheshmaanas   (501) staff       (20)       49 2024-05-06 12:36:39.000000 CustomtkinterCodeViewer-0.0.3/CustomtkinterCodeViewer/__init__.py
+drwxr-xr-x   0 maheshmaanas   (501) staff       (20)        0 2024-05-06 12:41:57.908782 CustomtkinterCodeViewer-0.0.3/CustomtkinterCodeViewer.egg-info/
+-rw-r--r--   0 maheshmaanas   (501) staff       (20)     1437 2024-05-06 12:41:57.000000 CustomtkinterCodeViewer-0.0.3/CustomtkinterCodeViewer.egg-info/PKG-INFO
+-rw-r--r--   0 maheshmaanas   (501) staff       (20)      329 2024-05-06 12:41:57.000000 CustomtkinterCodeViewer-0.0.3/CustomtkinterCodeViewer.egg-info/SOURCES.txt
+-rw-r--r--   0 maheshmaanas   (501) staff       (20)        1 2024-05-06 12:41:57.000000 CustomtkinterCodeViewer-0.0.3/CustomtkinterCodeViewer.egg-info/dependency_links.txt
+-rw-r--r--   0 maheshmaanas   (501) staff       (20)       33 2024-05-06 12:41:57.000000 CustomtkinterCodeViewer-0.0.3/CustomtkinterCodeViewer.egg-info/requires.txt
+-rw-r--r--   0 maheshmaanas   (501) staff       (20)       24 2024-05-06 12:41:57.000000 CustomtkinterCodeViewer-0.0.3/CustomtkinterCodeViewer.egg-info/top_level.txt
+-rw-r--r--   0 maheshmaanas   (501) staff       (20)     1437 2024-05-06 12:41:57.908951 CustomtkinterCodeViewer-0.0.3/PKG-INFO
+-rw-r--r--   0 maheshmaanas   (501) staff       (20)      902 2023-11-17 16:36:02.000000 CustomtkinterCodeViewer-0.0.3/README.md
+-rw-r--r--   0 maheshmaanas   (501) staff       (20)       38 2024-05-06 12:41:57.909182 CustomtkinterCodeViewer-0.0.3/setup.cfg
+-rw-r--r--   0 maheshmaanas   (501) staff       (20)     1170 2024-05-06 12:40:19.000000 CustomtkinterCodeViewer-0.0.3/setup.py
```

### Comparing `CustomtkinterCodeViewer-0.0.2/CustomtkinterCodeViewer/CTkCodeViewer.py` & `CustomtkinterCodeViewer-0.0.3/CustomtkinterCodeViewer/CTkCodeViewer.py`

 * *Files identical despite different names*

### Comparing `CustomtkinterCodeViewer-0.0.2/CustomtkinterCodeViewer.egg-info/PKG-INFO` & `CustomtkinterCodeViewer-0.0.3/CustomtkinterCodeViewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CustomtkinterCodeViewer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Display syntax highlighted code in customtkinter
 Author: Rigved Maanas
 Author-email: <rigvedmaanas@gmail.com>
 Keywords: python,customtkinter,code view,code viewer,CTkCodeViewer,tkinter
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `CustomtkinterCodeViewer-0.0.2/PKG-INFO` & `CustomtkinterCodeViewer-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CustomtkinterCodeViewer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Display syntax highlighted code in customtkinter
 Author: Rigved Maanas
 Author-email: <rigvedmaanas@gmail.com>
 Keywords: python,customtkinter,code view,code viewer,CTkCodeViewer,tkinter
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `CustomtkinterCodeViewer-0.0.2/README.md` & `CustomtkinterCodeViewer-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `CustomtkinterCodeViewer-0.0.2/setup.py` & `CustomtkinterCodeViewer-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codecs
 import os
 here = os.path.abspath(os.path.dirname(__file__))
 print(find_packages())
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Display syntax highlighted code in customtkinter'
 LONG_DESCRIPTION = 'This is a package for displaying code with syntax highlighting in a customtkinter application.'
 
 # Setting up
 setup(
     name="CustomtkinterCodeViewer",
     version=VERSION,
```

