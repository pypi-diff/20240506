# Comparing `tmp/extradecorators-0.3.tar.gz` & `tmp/extradecorators-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extradecorators-0.3.tar", last modified: Mon May  6 16:25:45 2024, max compression
+gzip compressed data, was "extradecorators-0.4.tar", last modified: Mon May  6 16:35:49 2024, max compression
```

## Comparing `extradecorators-0.3.tar` & `extradecorators-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 16:25:45.163503 extradecorators-0.3/
-drwxrwxrwx   0        0        0        0 2024-05-06 16:25:45.152126 extradecorators-0.3/ExtraDecorators/
--rw-rw-rw-   0        0        0      180 2024-05-06 16:25:36.000000 extradecorators-0.3/ExtraDecorators/__init__.py
--rw-rw-rw-   0        0        0     1007 2024-05-05 17:43:23.000000 extradecorators-0.3/ExtraDecorators/private.py
--rw-rw-rw-   0        0        0      860 2024-05-05 19:17:46.000000 extradecorators-0.3/ExtraDecorators/read_only.py
--rw-rw-rw-   0        0        0     1588 2024-05-06 16:23:19.000000 extradecorators-0.3/ExtraDecorators/restoreAttributeTypeIntegrity.py
--rw-rw-rw-   0        0        0      596 2024-05-06 15:59:27.000000 extradecorators-0.3/ExtraDecorators/validatetyping.py
--rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 extradecorators-0.3/LICENCE
--rw-rw-rw-   0        0        0     3504 2024-05-06 16:25:45.162995 extradecorators-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2829 2024-05-06 16:24:18.000000 extradecorators-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 16:25:45.161990 extradecorators-0.3/extradecorators.egg-info/
--rw-rw-rw-   0        0        0     3504 2024-05-06 16:25:45.000000 extradecorators-0.3/extradecorators.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2024-05-06 16:25:45.000000 extradecorators-0.3/extradecorators.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 16:25:45.000000 extradecorators-0.3/extradecorators.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-06 16:25:45.000000 extradecorators-0.3/extradecorators.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 16:25:45.164003 extradecorators-0.3/setup.cfg
--rw-rw-rw-   0        0        0      836 2024-05-06 16:25:42.000000 extradecorators-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:35:49.675809 extradecorators-0.4/
+drwxrwxrwx   0        0        0        0 2024-05-06 16:35:49.661683 extradecorators-0.4/ExtraDecorators/
+-rw-rw-rw-   0        0        0      180 2024-05-06 16:25:36.000000 extradecorators-0.4/ExtraDecorators/__init__.py
+-rw-rw-rw-   0        0        0     1007 2024-05-05 17:43:23.000000 extradecorators-0.4/ExtraDecorators/private.py
+-rw-rw-rw-   0        0        0      860 2024-05-05 19:17:46.000000 extradecorators-0.4/ExtraDecorators/read_only.py
+-rw-rw-rw-   0        0        0     1588 2024-05-06 16:23:19.000000 extradecorators-0.4/ExtraDecorators/restoreAttributeTypeIntegrity.py
+-rw-rw-rw-   0        0        0      595 2024-05-06 16:35:30.000000 extradecorators-0.4/ExtraDecorators/validatetyping.py
+-rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 extradecorators-0.4/LICENCE
+-rw-rw-rw-   0        0        0     3504 2024-05-06 16:35:49.675302 extradecorators-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2829 2024-05-06 16:24:18.000000 extradecorators-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 16:35:49.674297 extradecorators-0.4/extradecorators.egg-info/
+-rw-rw-rw-   0        0        0     3504 2024-05-06 16:35:49.000000 extradecorators-0.4/extradecorators.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2024-05-06 16:35:49.000000 extradecorators-0.4/extradecorators.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 16:35:49.000000 extradecorators-0.4/extradecorators.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-06 16:35:49.000000 extradecorators-0.4/extradecorators.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 16:35:49.675809 extradecorators-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      836 2024-05-06 16:35:46.000000 extradecorators-0.4/setup.py
```

### Comparing `extradecorators-0.3/ExtraDecorators/private.py` & `extradecorators-0.4/ExtraDecorators/private.py`

 * *Files identical despite different names*

### Comparing `extradecorators-0.3/ExtraDecorators/read_only.py` & `extradecorators-0.4/ExtraDecorators/read_only.py`

 * *Files identical despite different names*

### Comparing `extradecorators-0.3/ExtraDecorators/restoreAttributeTypeIntegrity.py` & `extradecorators-0.4/ExtraDecorators/restoreAttributeTypeIntegrity.py`

 * *Files identical despite different names*

### Comparing `extradecorators-0.3/ExtraDecorators/validatetyping.py` & `extradecorators-0.4/ExtraDecorators/validatetyping.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,11 +8,11 @@
         sig = inspect.signature(func)
         params = sig.parameters
         bound_values = sig.bind(*args, **kwargs).arguments
 
         for name, value in bound_values.items():
             expected_type = params[name].annotation
             if expected_type is not inspect._empty and not isinstance(value, expected_type):
-                raise ValueError(f"Value {value} is not of {expected_type}")
+                raise TypeError(f"Value {value} is not of {expected_type}")
 
         return func(*args, **kwargs)
     return wrapper
```

### Comparing `extradecorators-0.3/LICENCE` & `extradecorators-0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `extradecorators-0.3/PKG-INFO` & `extradecorators-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extradecorators
-Version: 0.3
+Version: 0.4
 Summary: A package that contains some useful decorators for any case.
 Home-page: UNKNOWN
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: Decorators
 Platform: UNKNOWN
```

### Comparing `extradecorators-0.3/README.md` & `extradecorators-0.4/README.md`

 * *Files identical despite different names*

### Comparing `extradecorators-0.3/extradecorators.egg-info/PKG-INFO` & `extradecorators-0.4/extradecorators.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extradecorators
-Version: 0.3
+Version: 0.4
 Summary: A package that contains some useful decorators for any case.
 Home-page: UNKNOWN
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: Decorators
 Platform: UNKNOWN
```

### Comparing `extradecorators-0.3/setup.py` & `extradecorators-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='extradecorators',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     description='A package that contains some useful decorators for any case.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='MIT with required credit to the author.',
```

