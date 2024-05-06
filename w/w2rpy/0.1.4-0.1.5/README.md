# Comparing `tmp/w2rpy-0.1.4.tar.gz` & `tmp/w2rpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w2rpy-0.1.4.tar", last modified: Thu May  2 16:08:37 2024, max compression
+gzip compressed data, was "w2rpy-0.1.5.tar", last modified: Mon May  6 19:34:25 2024, max compression
```

## Comparing `w2rpy-0.1.4.tar` & `w2rpy-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 16:08:37.224017 w2rpy-0.1.4/
--rw-rw-rw-   0        0        0     1062 2024-05-01 20:18:19.000000 w2rpy-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      416 2024-05-02 16:08:37.224017 w2rpy-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0        7 2024-05-01 21:03:28.000000 w2rpy-0.1.4/README.md
--rw-rw-rw-   0        0        0       86 2024-05-02 16:08:37.225019 w2rpy-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      702 2024-05-02 16:08:13.000000 w2rpy-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 16:08:37.214014 w2rpy-0.1.4/w2rpy/
--rw-rw-rw-   0        0        0      114 2024-05-01 21:04:56.000000 w2rpy-0.1.4/w2rpy/__init__.py
--rw-rw-rw-   0        0        0    26172 2024-05-02 16:04:08.000000 w2rpy-0.1.4/w2rpy/w2rpy.py
-drwxrwxrwx   0        0        0        0 2024-05-02 16:08:37.223024 w2rpy-0.1.4/w2rpy.egg-info/
--rw-rw-rw-   0        0        0      416 2024-05-02 16:08:37.000000 w2rpy-0.1.4/w2rpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-05-02 16:08:37.000000 w2rpy-0.1.4/w2rpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 16:08:37.000000 w2rpy-0.1.4/w2rpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-02 16:08:37.000000 w2rpy-0.1.4/w2rpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-02 16:08:37.000000 w2rpy-0.1.4/w2rpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 19:34:25.874753 w2rpy-0.1.5/
+-rw-rw-rw-   0        0        0     1062 2024-05-01 20:18:19.000000 w2rpy-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      416 2024-05-06 19:34:25.874753 w2rpy-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2024-05-01 21:03:28.000000 w2rpy-0.1.5/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-06 19:34:25.875753 w2rpy-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      699 2024-05-06 19:34:12.000000 w2rpy-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 19:34:25.873754 w2rpy-0.1.5/w2rpy.egg-info/
+-rw-rw-rw-   0        0        0      416 2024-05-06 19:34:25.000000 w2rpy-0.1.5/w2rpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2024-05-06 19:34:25.000000 w2rpy-0.1.5/w2rpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 19:34:25.000000 w2rpy-0.1.5/w2rpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-06 19:34:25.000000 w2rpy-0.1.5/w2rpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-06 19:34:25.000000 w2rpy-0.1.5/w2rpy.egg-info/top_level.txt
```

### Comparing `w2rpy-0.1.4/LICENSE` & `w2rpy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `w2rpy-0.1.4/setup.py` & `w2rpy-0.1.5/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 @author: lrussell
 """
 
 from distutils.core import setup
 
 setup(
   name = 'w2rpy',         
-  packages = ['w2rpy'],   
-  version = '0.1.4',     
+  py_modules=['w2rpy'],
+  version = '0.1.5',     
   license='MIT',        
   description = 'Water Resource Functions For Fluvial Systems',   
   author = 'Luke Russell',                   
   author_email = 'lrussell@wolfwaterresources.com',      
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   
   install_requires=['pandas',
                     'numpy',
```

