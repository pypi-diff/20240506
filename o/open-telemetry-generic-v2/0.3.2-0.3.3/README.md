# Comparing `tmp/open_telemetry_generic_v2-0.3.2.tar.gz` & `tmp/open_telemetry_generic_v2-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_telemetry_generic_v2-0.3.2.tar", last modified: Mon May  6 07:57:05 2024, max compression
+gzip compressed data, was "open_telemetry_generic_v2-0.3.3.tar", last modified: Mon May  6 07:58:31 2024, max compression
```

## Comparing `open_telemetry_generic_v2-0.3.2.tar` & `open_telemetry_generic_v2-0.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:57:05.902921 open_telemetry_generic_v2-0.3.2/
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      695 2024-05-06 07:57:05.902794 open_telemetry_generic_v2-0.3.2/PKG-INFO
--rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 06:00:44.000000 open_telemetry_generic_v2-0.3.2/README.md
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      709 2024-05-06 07:44:36.000000 open_telemetry_generic_v2-0.3.2/app.py
-drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:57:05.902464 open_telemetry_generic_v2-0.3.2/open_telemetry_generic_v2.egg-info/
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      695 2024-05-06 07:57:05.000000 open_telemetry_generic_v2-0.3.2/open_telemetry_generic_v2.egg-info/PKG-INFO
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      282 2024-05-06 07:57:05.000000 open_telemetry_generic_v2-0.3.2/open_telemetry_generic_v2.egg-info/SOURCES.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)        1 2024-05-06 07:57:05.000000 open_telemetry_generic_v2-0.3.2/open_telemetry_generic_v2.egg-info/dependency_links.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)       57 2024-05-06 07:57:05.000000 open_telemetry_generic_v2-0.3.2/open_telemetry_generic_v2.egg-info/requires.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 07:57:05.000000 open_telemetry_generic_v2-0.3.2/open_telemetry_generic_v2.egg-info/top_level.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)       38 2024-05-06 07:57:05.902980 open_telemetry_generic_v2-0.3.2/setup.cfg
--rw-r--r--   0 atifagboatwala   (501) staff       (20)     1179 2024-05-06 07:57:00.000000 open_telemetry_generic_v2-0.3.2/setup.py
-drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:57:05.902597 open_telemetry_generic_v2-0.3.2/test/
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      321 2024-05-06 06:42:18.000000 open_telemetry_generic_v2-0.3.2/test/test.py
+drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:58:31.898797 open_telemetry_generic_v2-0.3.3/
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      695 2024-05-06 07:58:31.898682 open_telemetry_generic_v2-0.3.3/PKG-INFO
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 06:00:44.000000 open_telemetry_generic_v2-0.3.3/README.md
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      709 2024-05-06 07:44:36.000000 open_telemetry_generic_v2-0.3.3/app.py
+drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:58:31.898382 open_telemetry_generic_v2-0.3.3/open_telemetry_generic_v2.egg-info/
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      695 2024-05-06 07:58:31.000000 open_telemetry_generic_v2-0.3.3/open_telemetry_generic_v2.egg-info/PKG-INFO
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      282 2024-05-06 07:58:31.000000 open_telemetry_generic_v2-0.3.3/open_telemetry_generic_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)        1 2024-05-06 07:58:31.000000 open_telemetry_generic_v2-0.3.3/open_telemetry_generic_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)       18 2024-05-06 07:58:31.000000 open_telemetry_generic_v2-0.3.3/open_telemetry_generic_v2.egg-info/requires.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 07:58:31.000000 open_telemetry_generic_v2-0.3.3/open_telemetry_generic_v2.egg-info/top_level.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)       38 2024-05-06 07:58:31.898845 open_telemetry_generic_v2-0.3.3/setup.cfg
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)     1118 2024-05-06 07:58:21.000000 open_telemetry_generic_v2-0.3.3/setup.py
+drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:58:31.898500 open_telemetry_generic_v2-0.3.3/test/
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      283 2024-05-06 07:57:23.000000 open_telemetry_generic_v2-0.3.3/test/test.py
```

### Comparing `open_telemetry_generic_v2-0.3.2/PKG-INFO` & `open_telemetry_generic_v2-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_telemetry_generic_v2
-Version: 0.3.2
+Version: 0.3.3
 Summary: A generic function to be able to use for open telemtry cases
 Home-page: https://github.com/yourusername/my_package
 Author: Atif Agboatwala
 Author-email: atif.agboat@hotmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `open_telemetry_generic_v2-0.3.2/app.py` & `open_telemetry_generic_v2-0.3.3/app.py`

 * *Files identical despite different names*

### Comparing `open_telemetry_generic_v2-0.3.2/open_telemetry_generic_v2.egg-info/PKG-INFO` & `open_telemetry_generic_v2-0.3.3/open_telemetry_generic_v2.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-telemetry-generic-v2
-Version: 0.3.2
+Version: 0.3.3
 Summary: A generic function to be able to use for open telemtry cases
 Home-page: https://github.com/yourusername/my_package
 Author: Atif Agboatwala
 Author-email: atif.agboat@hotmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `open_telemetry_generic_v2-0.3.2/setup.py` & `open_telemetry_generic_v2-0.3.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='open_telemetry_generic_v2',
-    version='0.3.2',
+    version='0.3.3',
     description='A generic function to be able to use for open telemtry cases',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Atif Agboatwala',
     author_email='atif.agboat@hotmail.com',
     url='https://github.com/yourusername/my_package',
     # package_dir={'': 'otel-getting-started'},
     # packages=find_packages(where='otel-getting-started'),
     install_requires=[
         # List your project's dependencies here.
         # They will be installed by pip when your project is installed.
         "opentelemetry-api",
-        "opentelemetry-sdk",
-        "opentelemetry-distro",
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

