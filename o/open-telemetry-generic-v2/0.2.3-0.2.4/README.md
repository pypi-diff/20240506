# Comparing `tmp/open_telemetry_generic_v2-0.2.3.tar.gz` & `tmp/open_telemetry_generic_v2-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_telemetry_generic_v2-0.2.3.tar", last modified: Mon May  6 07:40:18 2024, max compression
+gzip compressed data, was "open_telemetry_generic_v2-0.2.4.tar", last modified: Mon May  6 07:44:43 2024, max compression
```

## Comparing `open_telemetry_generic_v2-0.2.3.tar` & `open_telemetry_generic_v2-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:40:18.803160 open_telemetry_generic_v2-0.2.3/
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      746 2024-05-06 07:40:18.803045 open_telemetry_generic_v2-0.2.3/PKG-INFO
--rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 06:00:44.000000 open_telemetry_generic_v2-0.2.3/README.md
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      754 2024-05-06 07:40:07.000000 open_telemetry_generic_v2-0.2.3/app.py
-drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:40:18.802726 open_telemetry_generic_v2-0.2.3/open_telemetry_generic_v2.egg-info/
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      746 2024-05-06 07:40:18.000000 open_telemetry_generic_v2-0.2.3/open_telemetry_generic_v2.egg-info/PKG-INFO
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      297 2024-05-06 07:40:18.000000 open_telemetry_generic_v2-0.2.3/open_telemetry_generic_v2.egg-info/SOURCES.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)        1 2024-05-06 07:40:18.000000 open_telemetry_generic_v2-0.2.3/open_telemetry_generic_v2.egg-info/dependency_links.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)       67 2024-05-06 07:40:18.000000 open_telemetry_generic_v2-0.2.3/open_telemetry_generic_v2.egg-info/requires.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 07:40:18.000000 open_telemetry_generic_v2-0.2.3/open_telemetry_generic_v2.egg-info/top_level.txt
--rw-r--r--   0 atifagboatwala   (501) staff       (20)       90 2024-05-06 05:54:43.000000 open_telemetry_generic_v2-0.2.3/pyproject.toml
--rw-r--r--   0 atifagboatwala   (501) staff       (20)       38 2024-05-06 07:40:18.803210 open_telemetry_generic_v2-0.2.3/setup.cfg
--rw-r--r--   0 atifagboatwala   (501) staff       (20)     1250 2024-05-06 07:40:13.000000 open_telemetry_generic_v2-0.2.3/setup.py
-drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:40:18.802846 open_telemetry_generic_v2-0.2.3/test/
--rw-r--r--   0 atifagboatwala   (501) staff       (20)      321 2024-05-06 06:42:18.000000 open_telemetry_generic_v2-0.2.3/test/test.py
+drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:44:43.548341 open_telemetry_generic_v2-0.2.4/
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      746 2024-05-06 07:44:43.548226 open_telemetry_generic_v2-0.2.4/PKG-INFO
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 06:00:44.000000 open_telemetry_generic_v2-0.2.4/README.md
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      709 2024-05-06 07:44:36.000000 open_telemetry_generic_v2-0.2.4/app.py
+drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:44:43.547889 open_telemetry_generic_v2-0.2.4/open_telemetry_generic_v2.egg-info/
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      746 2024-05-06 07:44:43.000000 open_telemetry_generic_v2-0.2.4/open_telemetry_generic_v2.egg-info/PKG-INFO
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      297 2024-05-06 07:44:43.000000 open_telemetry_generic_v2-0.2.4/open_telemetry_generic_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)        1 2024-05-06 07:44:43.000000 open_telemetry_generic_v2-0.2.4/open_telemetry_generic_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)       67 2024-05-06 07:44:43.000000 open_telemetry_generic_v2-0.2.4/open_telemetry_generic_v2.egg-info/requires.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)        4 2024-05-06 07:44:43.000000 open_telemetry_generic_v2-0.2.4/open_telemetry_generic_v2.egg-info/top_level.txt
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)       90 2024-05-06 05:54:43.000000 open_telemetry_generic_v2-0.2.4/pyproject.toml
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)       38 2024-05-06 07:44:43.548398 open_telemetry_generic_v2-0.2.4/setup.cfg
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)     1250 2024-05-06 07:44:40.000000 open_telemetry_generic_v2-0.2.4/setup.py
+drwxr-xr-x   0 atifagboatwala   (501) staff       (20)        0 2024-05-06 07:44:43.548033 open_telemetry_generic_v2-0.2.4/test/
+-rw-r--r--   0 atifagboatwala   (501) staff       (20)      321 2024-05-06 06:42:18.000000 open_telemetry_generic_v2-0.2.4/test/test.py
```

### Comparing `open_telemetry_generic_v2-0.2.3/PKG-INFO` & `open_telemetry_generic_v2-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_telemetry_generic_v2
-Version: 0.2.3
+Version: 0.2.4
 Summary: A generic function to be able to use for open telemtry cases
 Home-page: https://github.com/yourusername/my_package
 Author: Atif Agboatwala
 Author-email: atif.agboat@hotmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `open_telemetry_generic_v2-0.2.3/app.py` & `open_telemetry_generic_v2-0.2.4/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 
 from opentelemetry import trace
 from opentelemetry import metrics
 
-from functools import wraps
     
 def wrapper_function(func):
     tracer_generic = trace.get_tracer("generictracer.tracer")
     meter_generic = metrics.get_meter("genericmeter.meter")
 
     generic_counter = meter_generic.create_counter(
     "generic.calls",
     description="The number of times function has been called",
     )
-    @wraps(func)
     def inner_function():
         with tracer.start_as_current_span("generic") as generic:
             result = func()
             generic.set_attribute("generic.value", result)
             generic_counter.add(1, {"generic.value": result})
             return result
```

### Comparing `open_telemetry_generic_v2-0.2.3/open_telemetry_generic_v2.egg-info/PKG-INFO` & `open_telemetry_generic_v2-0.2.4/open_telemetry_generic_v2.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-telemetry-generic-v2
-Version: 0.2.3
+Version: 0.2.4
 Summary: A generic function to be able to use for open telemtry cases
 Home-page: https://github.com/yourusername/my_package
 Author: Atif Agboatwala
 Author-email: atif.agboat@hotmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `open_telemetry_generic_v2-0.2.3/setup.py` & `open_telemetry_generic_v2-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='open_telemetry_generic_v2',
-    version='0.2.3',
+    version='0.2.4',
     description='A generic function to be able to use for open telemtry cases',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Atif Agboatwala',
     author_email='atif.agboat@hotmail.com',
     url='https://github.com/yourusername/my_package',
     # package_dir={'': 'otel-getting-started'},
```

