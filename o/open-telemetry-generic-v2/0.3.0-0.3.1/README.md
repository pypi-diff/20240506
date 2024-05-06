# Comparing `tmp/open_telemetry_generic_v2-0.3.0.tar.gz` & `tmp/open_telemetry_generic_v2-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_telemetry_generic_v2-0.3.0.tar", last modified: Mon May  6 07:51:45 2024, max compression
+gzip compressed data, was "open_telemetry_generic_v2-0.3.1.tar", last modified: Mon May  6 07:54:19 2024, max compression
```

## Comparing `open_telemetry_generic_v2-0.3.0.tar` & `open_telemetry_generic_v2-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:51:45.221521 open_telemetry_generic_v2-0.3.0/
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      746 2024-05-06 07:51:45.221400 open_telemetry_generic_v2-0.3.0/PKG-INFO
--rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 06:00:44.000000 open_telemetry_generic_v2-0.3.0/README.md
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      709 2024-05-06 07:44:36.000000 open_telemetry_generic_v2-0.3.0/app.py
-drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:51:45.221081 open_telemetry_generic_v2-0.3.0/open_telemetry_generic_v2.egg-info/
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      746 2024-05-06 07:51:45.000000 open_telemetry_generic_v2-0.3.0/open_telemetry_generic_v2.egg-info/PKG-INFO
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      282 2024-05-06 07:51:45.000000 open_telemetry_generic_v2-0.3.0/open_telemetry_generic_v2.egg-info/SOURCES.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)        1 2024-05-06 07:51:45.000000 open_telemetry_generic_v2-0.3.0/open_telemetry_generic_v2.egg-info/dependency_links.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)       67 2024-05-06 07:51:45.000000 open_telemetry_generic_v2-0.3.0/open_telemetry_generic_v2.egg-info/requires.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 07:51:45.000000 open_telemetry_generic_v2-0.3.0/open_telemetry_generic_v2.egg-info/top_level.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)       38 2024-05-06 07:51:45.221575 open_telemetry_generic_v2-0.3.0/setup.cfg
--rw-r--r--   0 atifagboatwala   (501) staff       (20)     1250 2024-05-06 07:47:21.000000 open_telemetry_generic_v2-0.3.0/setup.py
-drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:51:45.221209 open_telemetry_generic_v2-0.3.0/test/
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      321 2024-05-06 06:42:18.000000 open_telemetry_generic_v2-0.3.0/test/test.py
+drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:54:19.086677 open_telemetry_generic_v2-0.3.1/
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      695 2024-05-06 07:54:19.086560 open_telemetry_generic_v2-0.3.1/PKG-INFO
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 06:00:44.000000 open_telemetry_generic_v2-0.3.1/README.md
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      709 2024-05-06 07:44:36.000000 open_telemetry_generic_v2-0.3.1/app.py
+drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:54:19.086248 open_telemetry_generic_v2-0.3.1/open_telemetry_generic_v2.egg-info/
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      695 2024-05-06 07:54:19.000000 open_telemetry_generic_v2-0.3.1/open_telemetry_generic_v2.egg-info/PKG-INFO
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      282 2024-05-06 07:54:19.000000 open_telemetry_generic_v2-0.3.1/open_telemetry_generic_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)        1 2024-05-06 07:54:19.000000 open_telemetry_generic_v2-0.3.1/open_telemetry_generic_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)       67 2024-05-06 07:54:19.000000 open_telemetry_generic_v2-0.3.1/open_telemetry_generic_v2.egg-info/requires.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 07:54:19.000000 open_telemetry_generic_v2-0.3.1/open_telemetry_generic_v2.egg-info/top_level.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)       38 2024-05-06 07:54:19.086730 open_telemetry_generic_v2-0.3.1/setup.cfg
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)     1200 2024-05-06 07:54:13.000000 open_telemetry_generic_v2-0.3.1/setup.py
+drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:54:19.086368 open_telemetry_generic_v2-0.3.1/test/
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      321 2024-05-06 06:42:18.000000 open_telemetry_generic_v2-0.3.1/test/test.py
```

### Comparing `open_telemetry_generic_v2-0.3.0/PKG-INFO` & `open_telemetry_generic_v2-0.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: open_telemetry_generic_v2
-Version: 0.3.0
+Version: 0.3.1
 Summary: A generic function to be able to use for open telemtry cases
 Home-page: https://github.com/yourusername/my_package
 Author: Atif Agboatwala
 Author-email: atif.agboat@hotmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 test
```

### Comparing `open_telemetry_generic_v2-0.3.0/app.py` & `open_telemetry_generic_v2-0.3.1/app.py`

 * *Files identical despite different names*

### Comparing `open_telemetry_generic_v2-0.3.0/open_telemetry_generic_v2.egg-info/PKG-INFO` & `open_telemetry_generic_v2-0.3.1/open_telemetry_generic_v2.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: open-telemetry-generic-v2
-Version: 0.3.0
+Version: 0.3.1
 Summary: A generic function to be able to use for open telemtry cases
 Home-page: https://github.com/yourusername/my_package
 Author: Atif Agboatwala
 Author-email: atif.agboat@hotmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 test
```

### Comparing `open_telemetry_generic_v2-0.3.0/setup.py` & `open_telemetry_generic_v2-0.3.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='open_telemetry_generic_v2',
-    version='0.3.0',
+    version='0.3.1',
     description='A generic function to be able to use for open telemtry cases',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Atif Agboatwala',
     author_email='atif.agboat@hotmail.com',
     url='https://github.com/yourusername/my_package',
     # package_dir={'': 'otel-getting-started'},
@@ -24,10 +24,9 @@
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.11',
     ],
 )
```

