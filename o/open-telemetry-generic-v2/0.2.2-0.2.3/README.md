# Comparing `tmp/open_telemetry_generic_v2-0.2.2.tar.gz` & `tmp/open_telemetry_generic_v2-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_telemetry_generic_v2-0.2.2.tar", last modified: Mon May  6 07:07:10 2024, max compression
+gzip compressed data, was "open_telemetry_generic_v2-0.2.3.tar", last modified: Mon May  6 07:40:18 2024, max compression
```

## Comparing `open_telemetry_generic_v2-0.2.2.tar` & `open_telemetry_generic_v2-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:07:10.759099 open_telemetry_generic_v2-0.2.2/
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      746 2024-05-06 07:07:10.758981 open_telemetry_generic_v2-0.2.2/PKG-INFO
--rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 06:00:44.000000 open_telemetry_generic_v2-0.2.2/README.md
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      746 2024-05-06 06:42:11.000000 open_telemetry_generic_v2-0.2.2/app.py
-drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:07:10.758664 open_telemetry_generic_v2-0.2.2/open_telemetry_generic_v2.egg-info/
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      746 2024-05-06 07:07:10.000000 open_telemetry_generic_v2-0.2.2/open_telemetry_generic_v2.egg-info/PKG-INFO
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      297 2024-05-06 07:07:10.000000 open_telemetry_generic_v2-0.2.2/open_telemetry_generic_v2.egg-info/SOURCES.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)        1 2024-05-06 07:07:10.000000 open_telemetry_generic_v2-0.2.2/open_telemetry_generic_v2.egg-info/dependency_links.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)       67 2024-05-06 07:07:10.000000 open_telemetry_generic_v2-0.2.2/open_telemetry_generic_v2.egg-info/requires.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 07:07:10.000000 open_telemetry_generic_v2-0.2.2/open_telemetry_generic_v2.egg-info/top_level.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)       90 2024-05-06 05:54:43.000000 open_telemetry_generic_v2-0.2.2/pyproject.toml
--rw-r--r--   0 atifagboatwala   (501) staff       (20)       38 2024-05-06 07:07:10.759151 open_telemetry_generic_v2-0.2.2/setup.cfg
--rw-r--r--   0 atifagboatwala   (501) staff       (20)     1250 2024-05-06 07:07:07.000000 open_telemetry_generic_v2-0.2.2/setup.py
-drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:07:10.758784 open_telemetry_generic_v2-0.2.2/test/
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      321 2024-05-06 06:42:18.000000 open_telemetry_generic_v2-0.2.2/test/test.py
+drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:40:18.803160 open_telemetry_generic_v2-0.2.3/
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      746 2024-05-06 07:40:18.803045 open_telemetry_generic_v2-0.2.3/PKG-INFO
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 06:00:44.000000 open_telemetry_generic_v2-0.2.3/README.md
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      754 2024-05-06 07:40:07.000000 open_telemetry_generic_v2-0.2.3/app.py
+drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:40:18.802726 open_telemetry_generic_v2-0.2.3/open_telemetry_generic_v2.egg-info/
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      746 2024-05-06 07:40:18.000000 open_telemetry_generic_v2-0.2.3/open_telemetry_generic_v2.egg-info/PKG-INFO
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      297 2024-05-06 07:40:18.000000 open_telemetry_generic_v2-0.2.3/open_telemetry_generic_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)        1 2024-05-06 07:40:18.000000 open_telemetry_generic_v2-0.2.3/open_telemetry_generic_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)       67 2024-05-06 07:40:18.000000 open_telemetry_generic_v2-0.2.3/open_telemetry_generic_v2.egg-info/requires.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 07:40:18.000000 open_telemetry_generic_v2-0.2.3/open_telemetry_generic_v2.egg-info/top_level.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)       90 2024-05-06 05:54:43.000000 open_telemetry_generic_v2-0.2.3/pyproject.toml
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)       38 2024-05-06 07:40:18.803210 open_telemetry_generic_v2-0.2.3/setup.cfg
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)     1250 2024-05-06 07:40:13.000000 open_telemetry_generic_v2-0.2.3/setup.py
+drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:40:18.802846 open_telemetry_generic_v2-0.2.3/test/
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      321 2024-05-06 06:42:18.000000 open_telemetry_generic_v2-0.2.3/test/test.py
```

### Comparing `open_telemetry_generic_v2-0.2.2/PKG-INFO` & `open_telemetry_generic_v2-0.2.3/open_telemetry_generic_v2.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: open_telemetry_generic_v2
-Version: 0.2.2
+Name: open-telemetry-generic-v2
+Version: 0.2.3
 Summary: A generic function to be able to use for open telemtry cases
 Home-page: https://github.com/yourusername/my_package
 Author: Atif Agboatwala
 Author-email: atif.agboat@hotmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `open_telemetry_generic_v2-0.2.2/app.py` & `open_telemetry_generic_v2-0.2.3/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     description="The number of times function has been called",
     )
     @wraps(func)
     def inner_function():
         with tracer.start_as_current_span("generic") as generic:
             result = func()
             generic.set_attribute("generic.value", result)
-            counter.add(1, {"generic.value": result})
+            generic_counter.add(1, {"generic.value": result})
             return result
         
     return inner_function
 
 def hello():
     print("hello")
```

### Comparing `open_telemetry_generic_v2-0.2.2/open_telemetry_generic_v2.egg-info/PKG-INFO` & `open_telemetry_generic_v2-0.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: open-telemetry-generic-v2
-Version: 0.2.2
+Name: open_telemetry_generic_v2
+Version: 0.2.3
 Summary: A generic function to be able to use for open telemtry cases
 Home-page: https://github.com/yourusername/my_package
 Author: Atif Agboatwala
 Author-email: atif.agboat@hotmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `open_telemetry_generic_v2-0.2.2/setup.py` & `open_telemetry_generic_v2-0.2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='open_telemetry_generic_v2',
-    version='0.2.2',
+    version='0.2.3',
     description='A generic function to be able to use for open telemtry cases',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Atif Agboatwala',
     author_email='atif.agboat@hotmail.com',
     url='https://github.com/yourusername/my_package',
     # package_dir={'': 'otel-getting-started'},
```

