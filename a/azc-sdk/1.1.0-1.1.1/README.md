# Comparing `tmp/azc-sdk-1.1.0.tar.gz` & `tmp/azc-sdk-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\azc-sdk-1.1.0.tar", last modified: Mon May  6 06:31:39 2024, max compression
+gzip compressed data, was "dist\azc-sdk-1.1.1.tar", last modified: Mon May  6 11:13:57 2024, max compression
```

## Comparing `azc-sdk-1.1.0.tar` & `azc-sdk-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 06:31:39.144807 azc-sdk-1.1.0/
--rw-rw-rw-   0        0        0      441 2024-05-06 06:31:39.144807 azc-sdk-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 06:31:39.130762 azc-sdk-1.1.0/azc/
--rw-rw-rw-   0        0        0        0 2024-05-06 04:42:29.000000 azc-sdk-1.1.0/azc/__init__.py
--rw-rw-rw-   0        0        0      120 2024-05-06 05:02:58.000000 azc-sdk-1.1.0/azc/azc_demo.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:31:39.143273 azc-sdk-1.1.0/azc_sdk.egg-info/
--rw-rw-rw-   0        0        0      441 2024-05-06 06:31:39.000000 azc-sdk-1.1.0/azc_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2024-05-06 06:31:39.000000 azc-sdk-1.1.0/azc_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 06:31:39.000000 azc-sdk-1.1.0/azc_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-06 06:31:39.000000 azc-sdk-1.1.0/azc_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-06 06:31:39.000000 azc-sdk-1.1.0/azc_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 06:31:39.145822 azc-sdk-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      709 2024-05-06 06:30:37.000000 azc-sdk-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:13:57.210776 azc-sdk-1.1.1/
+-rw-rw-rw-   0        0        0      441 2024-05-06 11:13:57.209777 azc-sdk-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 11:13:57.196776 azc-sdk-1.1.1/azc/
+-rw-rw-rw-   0        0        0       24 2024-05-06 11:08:30.000000 azc-sdk-1.1.1/azc/__init__.py
+-rw-rw-rw-   0        0        0      120 2024-05-06 05:02:58.000000 azc-sdk-1.1.1/azc/azc_demo.py
+drwxrwxrwx   0        0        0        0 2024-05-06 11:13:57.207777 azc-sdk-1.1.1/azc_sdk.egg-info/
+-rw-rw-rw-   0        0        0      441 2024-05-06 11:13:57.000000 azc-sdk-1.1.1/azc_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2024-05-06 11:13:57.000000 azc-sdk-1.1.1/azc_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 11:13:57.000000 azc-sdk-1.1.1/azc_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-06 11:13:57.000000 azc-sdk-1.1.1/azc_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-06 11:13:57.000000 azc-sdk-1.1.1/azc_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 11:13:57.210776 azc-sdk-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      709 2024-05-06 11:13:19.000000 azc-sdk-1.1.1/setup.py
```

### Comparing `azc-sdk-1.1.0/setup.py` & `azc-sdk-1.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", mode="r", encoding="utf-8") as f:
     readme = f.read()
 
-VERSION = "1.1.0"
+VERSION = "1.1.1"
 
 setup(
     name="azc-sdk",
     version=VERSION[:],
     description="AZC SDK for Python",
     long_description=readme,
     long_description_content_type="text/markdown",
```

