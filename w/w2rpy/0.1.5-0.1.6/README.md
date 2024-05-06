# Comparing `tmp/w2rpy-0.1.5.tar.gz` & `tmp/w2rpy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w2rpy-0.1.5.tar", last modified: Mon May  6 19:34:25 2024, max compression
+gzip compressed data, was "w2rpy-0.1.6.tar", last modified: Mon May  6 19:37:18 2024, max compression
```

## Comparing `w2rpy-0.1.5.tar` & `w2rpy-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 19:34:25.874753 w2rpy-0.1.5/
--rw-rw-rw-   0        0        0     1062 2024-05-01 20:18:19.000000 w2rpy-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      416 2024-05-06 19:34:25.874753 w2rpy-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0        7 2024-05-01 21:03:28.000000 w2rpy-0.1.5/README.md
--rw-rw-rw-   0        0        0       86 2024-05-06 19:34:25.875753 w2rpy-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      699 2024-05-06 19:34:12.000000 w2rpy-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 19:34:25.873754 w2rpy-0.1.5/w2rpy.egg-info/
--rw-rw-rw-   0        0        0      416 2024-05-06 19:34:25.000000 w2rpy-0.1.5/w2rpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2024-05-06 19:34:25.000000 w2rpy-0.1.5/w2rpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 19:34:25.000000 w2rpy-0.1.5/w2rpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-06 19:34:25.000000 w2rpy-0.1.5/w2rpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-06 19:34:25.000000 w2rpy-0.1.5/w2rpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 19:37:18.800166 w2rpy-0.1.6/
+-rw-rw-rw-   0        0        0     1062 2024-05-01 20:18:19.000000 w2rpy-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      416 2024-05-06 19:37:18.800166 w2rpy-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2024-05-01 21:03:28.000000 w2rpy-0.1.6/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-06 19:37:18.801175 w2rpy-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      722 2024-05-06 19:36:37.000000 w2rpy-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 19:37:18.789167 w2rpy-0.1.6/w2rpy/
+-rw-rw-rw-   0        0        0      114 2024-05-01 21:04:56.000000 w2rpy-0.1.6/w2rpy/__init__.py
+-rw-rw-rw-   0        0        0    28193 2024-05-06 19:30:27.000000 w2rpy-0.1.6/w2rpy/w2rpy.py
+drwxrwxrwx   0        0        0        0 2024-05-06 19:37:18.799171 w2rpy-0.1.6/w2rpy.egg-info/
+-rw-rw-rw-   0        0        0      416 2024-05-06 19:37:18.000000 w2rpy-0.1.6/w2rpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-05-06 19:37:18.000000 w2rpy-0.1.6/w2rpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 19:37:18.000000 w2rpy-0.1.6/w2rpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-06 19:37:18.000000 w2rpy-0.1.6/w2rpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-06 19:37:18.000000 w2rpy-0.1.6/w2rpy.egg-info/top_level.txt
```

### Comparing `w2rpy-0.1.5/LICENSE` & `w2rpy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `w2rpy-0.1.5/setup.py` & `w2rpy-0.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 
 @author: lrussell
 """
 
 from distutils.core import setup
 
 setup(
-  name = 'w2rpy',         
+  name = 'w2rpy',    
+  packages=['w2rpy'],     
   py_modules=['w2rpy'],
-  version = '0.1.5',     
+  version = '0.1.6',     
   license='MIT',        
   description = 'Water Resource Functions For Fluvial Systems',   
   author = 'Luke Russell',                   
   author_email = 'lrussell@wolfwaterresources.com',      
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   
   install_requires=['pandas',
                     'numpy',
```

