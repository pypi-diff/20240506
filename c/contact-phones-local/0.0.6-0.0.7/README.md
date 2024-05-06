# Comparing `tmp/contact-phones-local-0.0.6.tar.gz` & `tmp/contact_phones_local-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact-phones-local-0.0.6.tar", last modified: Wed Feb 28 18:01:28 2024, max compression
+gzip compressed data, was "contact_phones_local-0.0.7.tar", last modified: Mon May  6 18:19:50 2024, max compression
```

## Comparing `contact-phones-local-0.0.6.tar` & `contact_phones_local-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 18:01:28.063847 contact-phones-local-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-28 18:01:28.063847 contact-phones-local-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-28 18:00:45.000000 contact-phones-local-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 18:01:28.059847 contact-phones-local-0.0.6/contact_phones_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 18:01:28.063847 contact-phones-local-0.0.6/contact_phones_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 18:00:45.000000 contact-phones-local-0.0.6/contact_phones_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-02-28 18:00:45.000000 contact-phones-local-0.0.6/contact_phones_local/src/contact_phones_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-02-28 18:00:45.000000 contact-phones-local-0.0.6/contact_phones_local/src/contact_phones_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 18:01:28.063847 contact-phones-local-0.0.6/contact_phones_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-28 18:01:28.000000 contact-phones-local-0.0.6/contact_phones_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-28 18:01:28.000000 contact-phones-local-0.0.6/contact_phones_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 18:01:28.000000 contact-phones-local-0.0.6/contact_phones_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-28 18:01:28.000000 contact-phones-local-0.0.6/contact_phones_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-28 18:01:28.000000 contact-phones-local-0.0.6/contact_phones_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-28 18:00:45.000000 contact-phones-local-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 18:01:28.063847 contact-phones-local-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-02-28 18:00:45.000000 contact-phones-local-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:19:50.244682 contact_phones_local-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-06 18:19:50.244682 contact_phones_local-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 18:19:23.000000 contact_phones_local-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:19:50.240682 contact_phones_local-0.0.7/contact_phones_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:19:50.244682 contact_phones_local-0.0.7/contact_phones_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 18:19:23.000000 contact_phones_local-0.0.7/contact_phones_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-05-06 18:19:23.000000 contact_phones_local-0.0.7/contact_phones_local/src/contact_phones_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-06 18:19:23.000000 contact_phones_local-0.0.7/contact_phones_local/src/contact_phones_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:19:50.244682 contact_phones_local-0.0.7/contact_phones_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-06 18:19:50.000000 contact_phones_local-0.0.7/contact_phones_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-06 18:19:50.000000 contact_phones_local-0.0.7/contact_phones_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:19:50.000000 contact_phones_local-0.0.7/contact_phones_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-06 18:19:50.000000 contact_phones_local-0.0.7/contact_phones_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 18:19:50.000000 contact_phones_local-0.0.7/contact_phones_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-06 18:19:23.000000 contact_phones_local-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 18:19:50.244682 contact_phones_local-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-06 18:19:23.000000 contact_phones_local-0.0.7/setup.py
```

### Comparing `contact-phones-local-0.0.6/PKG-INFO` & `contact_phones_local-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-phones-local
-Version: 0.0.6
+Version: 0.0.7
 Summary: PyPI Package for Circles contact-phones-local Python
 Home-page: https://github.com/circles-zone/contact-phone-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact-phones-local-0.0.6/contact_phones_local/src/contact_phones_local.py` & `contact_phones_local-0.0.7/contact_phones_local/src/contact_phones_local.py`

 * *Files identical despite different names*

### Comparing `contact-phones-local-0.0.6/contact_phones_local/src/contact_phones_local_constants.py` & `contact_phones_local-0.0.7/contact_phones_local/src/contact_phones_local_constants.py`

 * *Files identical despite different names*

### Comparing `contact-phones-local-0.0.6/contact_phones_local.egg-info/PKG-INFO` & `contact_phones_local-0.0.7/contact_phones_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-phones-local
-Version: 0.0.6
+Version: 0.0.7
 Summary: PyPI Package for Circles contact-phones-local Python
 Home-page: https://github.com/circles-zone/contact-phone-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact-phones-local-0.0.6/setup.py` & `contact_phones_local-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "contact-phones-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.6',  # update only the minor version each time # https://pypi.org/project/contact-phones-local/
+    version='0.0.7',  # update only the minor version each time # https://pypi.org/project/contact-phones-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles contact-phones-local Python",
     long_description="PyPI Package for Circles contact-phones-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/contact-phone-local-python-package",  # https://pypi.org/project/contact-phones-local/
     packages=[package_dir],
```

