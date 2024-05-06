# Comparing `tmp/zyx-0.0.14.tar.gz` & `tmp/zyx-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyx-0.0.14.tar", last modified: Fri May  3 04:07:31 2024, max compression
+gzip compressed data, was "zyx-0.0.15.tar", last modified: Mon May  6 11:07:24 2024, max compression
```

## Comparing `zyx-0.0.14.tar` & `zyx-0.0.15.tar`

### file list

```diff
@@ -1,38 +1,36 @@
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.184996 zyx-0.0.14/
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.179995 zyx-0.0.14/.zyx/
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.179995 zyx-0.0.14/.zyx/src/
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.180995 zyx-0.0.14/.zyx/src/zyx/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      493 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/__cli__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      225 2024-05-01 03:37:03.000000 zyx-0.0.14/.zyx/src/zyx/__init__.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.182995 zyx-0.0.14/.zyx/src/zyx/core/
--rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/core/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      514 2024-05-02 05:26:48.000000 zyx-0.0.14/.zyx/src/zyx/core/chat.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     5030 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/core/input.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2863 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/core/lightning.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2425 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/core/loaders.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1976 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/core/print.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     3506 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/core/validate_path.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1690 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/core/validate_type.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.183996 zyx-0.0.14/.zyx/src/zyx/functions/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      533 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/functions/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     2079 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/functions/create_id.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1020 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/functions/generate_name.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1474 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/functions/get_system_info.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.183996 zyx-0.0.14/.zyx/src/zyx/jupyter/
--rw-r--r--   0 hammad    (1001) hammad    (1001)       30 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/jupyter/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)     4162 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/jupyter/tailwind.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.184996 zyx-0.0.14/.zyx/src/zyx/text/
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1203 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/text/__chunker__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      153 2024-05-01 03:34:56.000000 zyx-0.0.14/.zyx/src/zyx/text/__init__.py
--rw-r--r--   0 hammad    (1001) hammad    (1001)      730 2024-05-02 01:36:57.000000 zyx-0.0.14/.zyx/src/zyx/text/__read_doc__.py
-drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-03 04:07:31.184996 zyx-0.0.14/.zyx/src/zyx.egg-info/
--rw-r--r--   0 hammad    (1001) hammad    (1001)      431 2024-05-03 04:07:31.000000 zyx-0.0.14/.zyx/src/zyx.egg-info/PKG-INFO
--rw-r--r--   0 hammad    (1001) hammad    (1001)      841 2024-05-03 04:07:31.000000 zyx-0.0.14/.zyx/src/zyx.egg-info/SOURCES.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)        1 2024-05-03 04:07:31.000000 zyx-0.0.14/.zyx/src/zyx.egg-info/dependency_links.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)       41 2024-05-03 04:07:31.000000 zyx-0.0.14/.zyx/src/zyx.egg-info/entry_points.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)      104 2024-05-03 04:07:31.000000 zyx-0.0.14/.zyx/src/zyx.egg-info/requires.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)        4 2024-05-03 04:07:31.000000 zyx-0.0.14/.zyx/src/zyx.egg-info/top_level.txt
--rw-r--r--   0 hammad    (1001) hammad    (1001)      431 2024-05-03 04:07:31.184996 zyx-0.0.14/PKG-INFO
--rw-r--r--   0 hammad    (1001) hammad    (1001)      667 2024-05-01 04:05:03.000000 zyx-0.0.14/README.md
--rw-r--r--   0 hammad    (1001) hammad    (1001)       38 2024-05-03 04:07:31.184996 zyx-0.0.14/setup.cfg
--rw-r--r--   0 hammad    (1001) hammad    (1001)     1191 2024-05-03 04:07:20.000000 zyx-0.0.14/setup.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:07:24.209887 zyx-0.0.15/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      431 2024-05-06 11:07:24.209887 zyx-0.0.15/PKG-INFO
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       38 2024-05-06 11:07:24.209887 zyx-0.0.15/setup.cfg
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1122 2024-05-06 11:07:14.000000 zyx-0.0.15/setup.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:07:24.204887 zyx-0.0.15/src/
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:07:24.205886 zyx-0.0.15/src/zyx/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      493 2024-05-05 22:15:21.000000 zyx-0.0.15/src/zyx/__cli__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      225 2024-05-05 22:15:21.000000 zyx-0.0.15/src/zyx/__init__.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:07:24.207887 zyx-0.0.15/src/zyx/core/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        0 2024-05-05 22:15:21.000000 zyx-0.0.15/src/zyx/core/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      873 2024-05-06 10:48:37.000000 zyx-0.0.15/src/zyx/core/chat.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     5030 2024-05-05 22:15:21.000000 zyx-0.0.15/src/zyx/core/input.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2863 2024-05-05 22:15:21.000000 zyx-0.0.15/src/zyx/core/lightning.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2425 2024-05-05 22:15:21.000000 zyx-0.0.15/src/zyx/core/loaders.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1976 2024-05-05 22:15:21.000000 zyx-0.0.15/src/zyx/core/print.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     3506 2024-05-05 22:15:21.000000 zyx-0.0.15/src/zyx/core/validate_path.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1690 2024-05-05 22:15:21.000000 zyx-0.0.15/src/zyx/core/validate_type.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:07:24.207887 zyx-0.0.15/src/zyx/functions/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      533 2024-05-05 22:15:21.000000 zyx-0.0.15/src/zyx/functions/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     2079 2024-05-05 22:15:21.000000 zyx-0.0.15/src/zyx/functions/create_id.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1020 2024-05-05 22:15:21.000000 zyx-0.0.15/src/zyx/functions/generate_name.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1474 2024-05-05 22:15:21.000000 zyx-0.0.15/src/zyx/functions/get_system_info.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:07:24.209887 zyx-0.0.15/src/zyx/jupyter/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       30 2024-05-05 22:15:21.000000 zyx-0.0.15/src/zyx/jupyter/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     4195 2024-05-06 11:06:04.000000 zyx-0.0.15/src/zyx/jupyter/tailwind.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:07:24.209887 zyx-0.0.15/src/zyx/text/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)     1203 2024-05-05 22:15:21.000000 zyx-0.0.15/src/zyx/text/__chunker__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      153 2024-05-05 22:15:21.000000 zyx-0.0.15/src/zyx/text/__init__.py
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      730 2024-05-05 22:15:21.000000 zyx-0.0.15/src/zyx/text/__read_doc__.py
+drwxr-xr-x   0 hammad    (1001) hammad    (1001)        0 2024-05-06 11:07:24.209887 zyx-0.0.15/src/zyx.egg-info/
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      431 2024-05-06 11:07:24.000000 zyx-0.0.15/src/zyx.egg-info/PKG-INFO
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      706 2024-05-06 11:07:24.000000 zyx-0.0.15/src/zyx.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        1 2024-05-06 11:07:24.000000 zyx-0.0.15/src/zyx.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)       41 2024-05-06 11:07:24.000000 zyx-0.0.15/src/zyx.egg-info/entry_points.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)      104 2024-05-06 11:07:24.000000 zyx-0.0.15/src/zyx.egg-info/requires.txt
+-rw-r--r--   0 hammad    (1001) hammad    (1001)        4 2024-05-06 11:07:24.000000 zyx-0.0.15/src/zyx.egg-info/top_level.txt
```

### Comparing `zyx-0.0.14/.zyx/src/zyx/core/input.py` & `zyx-0.0.15/src/zyx/core/input.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.14/.zyx/src/zyx/core/lightning.py` & `zyx-0.0.15/src/zyx/core/lightning.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.14/.zyx/src/zyx/core/loaders.py` & `zyx-0.0.15/src/zyx/core/loaders.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.14/.zyx/src/zyx/core/print.py` & `zyx-0.0.15/src/zyx/core/print.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.14/.zyx/src/zyx/core/validate_path.py` & `zyx-0.0.15/src/zyx/core/validate_path.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.14/.zyx/src/zyx/core/validate_type.py` & `zyx-0.0.15/src/zyx/core/validate_type.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.14/.zyx/src/zyx/functions/__init__.py` & `zyx-0.0.15/src/zyx/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.14/.zyx/src/zyx/functions/create_id.py` & `zyx-0.0.15/src/zyx/functions/create_id.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.14/.zyx/src/zyx/functions/generate_name.py` & `zyx-0.0.15/src/zyx/functions/generate_name.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.14/.zyx/src/zyx/functions/get_system_info.py` & `zyx-0.0.15/src/zyx/functions/get_system_info.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.14/.zyx/src/zyx/jupyter/tailwind.py` & `zyx-0.0.15/src/zyx/jupyter/tailwind.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     """
 
     def __init__(self, className : Optional[str] = None):
         if ModuleNotFoundError:
             print("Please install the 'IPython' package to use this class.")
             print("pip install ipython")
             return
-        self.className = className
+        self.className = className if className is not None else ""
         self.html_template = """
         <!DOCTYPE html>
         <html>
         <head>
             <script src="https://cdn.tailwindcss.com"></script>
             <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;700&family=Lexend:wght@400;500;600;700&family=Lora:wght@400;500;600;700&family=Playfair+Display:wght@400;500;600;700;800;900&family=JetBrains+Mono:wght@400;500;600;700&display=swap" rel="stylesheet">
             <style>
```

### Comparing `zyx-0.0.14/.zyx/src/zyx/text/__chunker__.py` & `zyx-0.0.15/src/zyx/text/__chunker__.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.14/.zyx/src/zyx/text/__read_doc__.py` & `zyx-0.0.15/src/zyx/text/__read_doc__.py`

 * *Files identical despite different names*

### Comparing `zyx-0.0.14/setup.py` & `zyx-0.0.15/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     author = "Hammad Saeed",
     author_email="hammad@supportvectors.com",
 
     name = 'zyx',
-    version = '0.0.14',
-    packages = find_packages(where='.zyx/src'),
-    package_dir = {'': '.zyx/src'},
+    version = '0.0.15',
+    packages = find_packages(where='src'),
+    package_dir = {'': 'src'},
 
     python_requires = '>=3.8',
 
-    package_data={
-        '': ['vendor/*.whl'],  
-    },
-
     install_requires = [
         # Art | ASCII Art
         'art',
 
         # IPython | Interactive Python
         'ipython',
```

