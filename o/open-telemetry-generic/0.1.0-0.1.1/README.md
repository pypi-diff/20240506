# Comparing `tmp/open_telemetry_generic-0.1.0.tar.gz` & `tmp/open_telemetry_generic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_telemetry_generic-0.1.0.tar", last modified: Mon May  6 06:22:19 2024, max compression
+gzip compressed data, was "open_telemetry_generic-0.1.1.tar", last modified: Mon May  6 06:42:42 2024, max compression
```

## Comparing `open_telemetry_generic-0.1.0.tar` & `open_telemetry_generic-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 06:22:19.402660 open_telemetry_generic-0.1.0/
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      692 2024-05-06 06:22:19.402426 open_telemetry_generic-0.1.0/PKG-INFO
--rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 06:00:44.000000 open_telemetry_generic-0.1.0/README.md
-drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 06:22:19.401232 open_telemetry_generic-0.1.0/otel-getting-started/
-drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 06:22:19.402210 open_telemetry_generic-0.1.0/otel-getting-started/open_telemetry_generic.egg-info/
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      692 2024-05-06 06:22:19.000000 open_telemetry_generic-0.1.0/otel-getting-started/open_telemetry_generic.egg-info/PKG-INFO
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      352 2024-05-06 06:22:19.000000 open_telemetry_generic-0.1.0/otel-getting-started/open_telemetry_generic.egg-info/SOURCES.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)        1 2024-05-06 06:22:19.000000 open_telemetry_generic-0.1.0/otel-getting-started/open_telemetry_generic.egg-info/dependency_links.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)       24 2024-05-06 06:22:19.000000 open_telemetry_generic-0.1.0/otel-getting-started/open_telemetry_generic.egg-info/requires.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)        1 2024-05-06 06:22:19.000000 open_telemetry_generic-0.1.0/otel-getting-started/open_telemetry_generic.egg-info/top_level.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)       38 2024-05-06 06:22:19.402714 open_telemetry_generic-0.1.0/setup.cfg
--rw-r--r--   0 atifagboatwala   (501) staff       (20)     1128 2024-05-06 05:59:25.000000 open_telemetry_generic-0.1.0/setup.py
+drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 06:42:42.942345 open_telemetry_generic-0.1.1/
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      692 2024-05-06 06:42:42.942202 open_telemetry_generic-0.1.1/PKG-INFO
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 06:00:44.000000 open_telemetry_generic-0.1.1/README.md
+drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 06:42:42.940636 open_telemetry_generic-0.1.1/otel-getting-started/
+drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 06:42:42.941848 open_telemetry_generic-0.1.1/otel-getting-started/open_telemetry_generic.egg-info/
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      692 2024-05-06 06:42:42.000000 open_telemetry_generic-0.1.1/otel-getting-started/open_telemetry_generic.egg-info/PKG-INFO
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      365 2024-05-06 06:42:42.000000 open_telemetry_generic-0.1.1/otel-getting-started/open_telemetry_generic.egg-info/SOURCES.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)        1 2024-05-06 06:42:42.000000 open_telemetry_generic-0.1.1/otel-getting-started/open_telemetry_generic.egg-info/dependency_links.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)       24 2024-05-06 06:42:42.000000 open_telemetry_generic-0.1.1/otel-getting-started/open_telemetry_generic.egg-info/requires.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)        1 2024-05-06 06:42:42.000000 open_telemetry_generic-0.1.1/otel-getting-started/open_telemetry_generic.egg-info/top_level.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)       38 2024-05-06 06:42:42.942402 open_telemetry_generic-0.1.1/setup.cfg
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)     1128 2024-05-06 06:42:15.000000 open_telemetry_generic-0.1.1/setup.py
+drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 06:42:42.941985 open_telemetry_generic-0.1.1/test/
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      321 2024-05-06 06:42:18.000000 open_telemetry_generic-0.1.1/test/test.py
```

### Comparing `open_telemetry_generic-0.1.0/PKG-INFO` & `open_telemetry_generic-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_telemetry_generic
-Version: 0.1.0
+Version: 0.1.1
 Summary: A generic function to be able to use for open telemtry cases
 Home-page: https://github.com/yourusername/my_package
 Author: Atif Agboatwala
 Author-email: atif.agboat@hotmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `open_telemetry_generic-0.1.0/otel-getting-started/open_telemetry_generic.egg-info/PKG-INFO` & `open_telemetry_generic-0.1.1/otel-getting-started/open_telemetry_generic.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-telemetry-generic
-Version: 0.1.0
+Version: 0.1.1
 Summary: A generic function to be able to use for open telemtry cases
 Home-page: https://github.com/yourusername/my_package
 Author: Atif Agboatwala
 Author-email: atif.agboat@hotmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `open_telemetry_generic-0.1.0/setup.py` & `open_telemetry_generic-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='open_telemetry_generic',
-    version='0.1.0',
+    version='0.1.1',
     description='A generic function to be able to use for open telemtry cases',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Atif Agboatwala',
     author_email='atif.agboat@hotmail.com',
     url='https://github.com/yourusername/my_package',
     package_dir={'': 'otel-getting-started'},
```

