# Comparing `tmp/espy_pdfier-0.1.tar.gz` & `tmp/espy_pdfier-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espy_pdfier-0.1.tar", last modified: Sun May  5 23:56:27 2024, max compression
+gzip compressed data, was "espy_pdfier-0.3.tar", last modified: Mon May  6 00:08:04 2024, max compression
```

## Comparing `espy_pdfier-0.1.tar` & `espy_pdfier-0.3.tar`

### file list

```diff
@@ -1,11 +1,16 @@
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-05 23:56:27.549752 espy_pdfier-0.1/
--rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-05-05 23:47:48.000000 espy_pdfier-0.1/LICENSE
--rw-r--r--   0 philipadigun   (501) staff       (20)      326 2024-05-05 23:56:27.549380 espy_pdfier-0.1/PKG-INFO
-drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-05 23:56:27.547783 espy_pdfier-0.1/espy_pdfier.egg-info/
--rw-r--r--   0 philipadigun   (501) staff       (20)      326 2024-05-05 23:56:27.000000 espy_pdfier-0.1/espy_pdfier.egg-info/PKG-INFO
--rw-r--r--   0 philipadigun   (501) staff       (20)      190 2024-05-05 23:56:27.000000 espy_pdfier-0.1/espy_pdfier.egg-info/SOURCES.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-05 23:56:27.000000 espy_pdfier-0.1/espy_pdfier.egg-info/dependency_links.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       17 2024-05-05 23:56:27.000000 espy_pdfier-0.1/espy_pdfier.egg-info/requires.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-05 23:56:27.000000 espy_pdfier-0.1/espy_pdfier.egg-info/top_level.txt
--rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-05 23:56:27.549813 espy_pdfier-0.1/setup.cfg
--rw-r--r--   0 philipadigun   (501) staff       (20)      554 2024-05-05 23:55:28.000000 espy_pdfier-0.1/setup.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 00:08:04.394139 espy_pdfier-0.3/
+-rw-r--r--   0 philipadigun   (501) staff       (20)     1072 2024-05-05 23:47:48.000000 espy_pdfier-0.3/LICENSE
+-rw-r--r--   0 philipadigun   (501) staff       (20)      326 2024-05-06 00:08:04.393884 espy_pdfier-0.3/PKG-INFO
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 00:08:04.392272 espy_pdfier-0.3/espy_pdfier/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-06 00:00:35.000000 espy_pdfier-0.3/espy_pdfier/__init__.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 00:08:04.393285 espy_pdfier-0.3/espy_pdfier/service/
+-rw-r--r--   0 philipadigun   (501) staff       (20)        0 2024-05-05 23:40:00.000000 espy_pdfier-0.3/espy_pdfier/service/__init__.py
+-rw-r--r--   0 philipadigun   (501) staff       (20)     2933 2024-05-05 23:40:00.000000 espy_pdfier-0.3/espy_pdfier/service/service.py
+drwxr-xr-x   0 philipadigun   (501) staff       (20)        0 2024-05-06 00:08:04.393618 espy_pdfier-0.3/espy_pdfier.egg-info/
+-rw-r--r--   0 philipadigun   (501) staff       (20)      326 2024-05-06 00:08:04.000000 espy_pdfier-0.3/espy_pdfier.egg-info/PKG-INFO
+-rw-r--r--   0 philipadigun   (501) staff       (20)      277 2024-05-06 00:08:04.000000 espy_pdfier-0.3/espy_pdfier.egg-info/SOURCES.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)        1 2024-05-06 00:08:04.000000 espy_pdfier-0.3/espy_pdfier.egg-info/dependency_links.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       17 2024-05-06 00:08:04.000000 espy_pdfier-0.3/espy_pdfier.egg-info/requires.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       12 2024-05-06 00:08:04.000000 espy_pdfier-0.3/espy_pdfier.egg-info/top_level.txt
+-rw-r--r--   0 philipadigun   (501) staff       (20)       38 2024-05-06 00:08:04.394190 espy_pdfier-0.3/setup.cfg
+-rw-r--r--   0 philipadigun   (501) staff       (20)      554 2024-05-06 00:05:59.000000 espy_pdfier-0.3/setup.py
```

### Comparing `espy_pdfier-0.1/LICENSE` & `espy_pdfier-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `espy_pdfier-0.1/setup.py` & `espy_pdfier-0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'ESSL assets management'
 LONG_DESCRIPTION = 'Internal helper package for ESSL assets management'
 setup(
     name='espy_pdfier',
-    version='0.1',
+    version='0.3',
     packages=find_packages(),
     install_requires=[
         'reportlab==4.2.0',
         ],
     author='Femi Adigun',
     author_email='femi.adigun@myeverlasting.net',
     description=DESCRIPTION,
```

