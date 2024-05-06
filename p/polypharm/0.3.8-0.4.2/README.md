# Comparing `tmp/polypharm-0.3.8.tar.gz` & `tmp/polypharm-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polypharm-0.3.8.tar", last modified: Fri Jan 20 13:28:55 2023, max compression
+gzip compressed data, was "polypharm-0.4.2.tar", last modified: Mon May  6 21:24:27 2024, max compression
```

## Comparing `polypharm-0.3.8.tar` & `polypharm-0.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:28:55.766201 polypharm-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-20 13:28:39.000000 polypharm-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-20 13:28:39.000000 polypharm-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-01-20 13:28:55.766201 polypharm-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-01-20 13:28:39.000000 polypharm-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:28:55.762201 polypharm-0.3.8/polypharm/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-01-20 13:28:39.000000 polypharm-0.3.8/polypharm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-01-20 13:28:39.000000 polypharm-0.3.8/polypharm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-01-20 13:28:39.000000 polypharm-0.3.8/polypharm/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-01-20 13:28:39.000000 polypharm-0.3.8/polypharm/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18482 2023-01-20 13:28:39.000000 polypharm-0.3.8/polypharm/polypharm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:28:55.766201 polypharm-0.3.8/polypharm/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-01-20 13:28:39.000000 polypharm-0.3.8/polypharm/scripts/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:28:55.766201 polypharm-0.3.8/polypharm/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-01-20 13:28:39.000000 polypharm-0.3.8/polypharm/templates/ifd.inp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 13:28:55.766201 polypharm-0.3.8/polypharm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-01-20 13:28:55.000000 polypharm-0.3.8/polypharm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-01-20 13:28:55.000000 polypharm-0.3.8/polypharm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 13:28:55.000000 polypharm-0.3.8/polypharm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-20 13:28:55.000000 polypharm-0.3.8/polypharm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-20 13:28:55.000000 polypharm-0.3.8/polypharm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-20 13:28:55.000000 polypharm-0.3.8/polypharm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-01-20 13:28:39.000000 polypharm-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 13:28:55.766201 polypharm-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 13:28:39.000000 polypharm-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:24:27.143323 polypharm-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-06 21:24:22.000000 polypharm-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-06 21:24:22.000000 polypharm-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-06 21:24:27.143323 polypharm-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-06 21:24:22.000000 polypharm-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:24:27.139323 polypharm-0.4.2/polypharm/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-06 21:24:22.000000 polypharm-0.4.2/polypharm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-05-06 21:24:22.000000 polypharm-0.4.2/polypharm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-06 21:24:22.000000 polypharm-0.4.2/polypharm/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-06 21:24:22.000000 polypharm-0.4.2/polypharm/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18482 2024-05-06 21:24:22.000000 polypharm-0.4.2/polypharm/polypharm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:24:27.139323 polypharm-0.4.2/polypharm/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-06 21:24:22.000000 polypharm-0.4.2/polypharm/scripts/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:24:27.139323 polypharm-0.4.2/polypharm/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-06 21:24:22.000000 polypharm-0.4.2/polypharm/templates/ifd.inp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:24:27.139323 polypharm-0.4.2/polypharm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-06 21:24:27.000000 polypharm-0.4.2/polypharm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-06 21:24:27.000000 polypharm-0.4.2/polypharm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:24:27.000000 polypharm-0.4.2/polypharm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 21:24:27.000000 polypharm-0.4.2/polypharm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-06 21:24:27.000000 polypharm-0.4.2/polypharm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 21:24:27.000000 polypharm-0.4.2/polypharm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-06 21:24:22.000000 polypharm-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:24:27.143323 polypharm-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:24:22.000000 polypharm-0.4.2/setup.py
```

### Comparing `polypharm-0.3.8/LICENSE` & `polypharm-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polypharm-0.3.8/PKG-INFO` & `polypharm-0.4.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polypharm
-Version: 0.3.8
+Version: 0.4.2
 Summary: A Python-based library to perform IFD and MMGBSA calculations on different targets using a polypharmacological approach.
 Author-email: Mauricio Bedoya <mbedoya@ucm.cl>, Francisco Adasme <fadasme@ucm.cl>
 License: MIT License
         
         Copyright (c) 2023 Mauricio Bedoya
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,20 +31,26 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: pandas>=1.4.3
+Requires-Dist: jinja2>=3.1.2
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: sphinx-rtd-theme; extra == "dev"
 
 # Polypharm
 
-A Python-based library to perform induced fit docking (IFD) and MM/GBSA
+[<img align="left" src="./polypharm/assets/polypharm_logo_transparent_001.png" width="250" />](./polypharm/assets/polypharm_logo_transparent_001.png) A Python-based library to perform induced fit docking (IFD) and MM/GBSA
 calculations on different targets using a polypharmacological approach.
 
 Refer to the [official documentation](http://polypharm.rtfd.io/) for
 details about installation, usage, methodology, and developer interface.
 
 ## Installation
```

### Comparing `polypharm-0.3.8/README.md` & `polypharm-0.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Polypharm
 
-A Python-based library to perform induced fit docking (IFD) and MM/GBSA
+[<img align="left" src="./polypharm/assets/polypharm_logo_transparent_001.png" width="250" />](./polypharm/assets/polypharm_logo_transparent_001.png) A Python-based library to perform induced fit docking (IFD) and MM/GBSA
 calculations on different targets using a polypharmacological approach.
 
 Refer to the [official documentation](http://polypharm.rtfd.io/) for
 details about installation, usage, methodology, and developer interface.
 
 ## Installation
```

### Comparing `polypharm-0.3.8/polypharm/__main__.py` & `polypharm-0.4.2/polypharm/__main__.py`

 * *Files identical despite different names*

### Comparing `polypharm-0.3.8/polypharm/concurrency.py` & `polypharm-0.4.2/polypharm/concurrency.py`

 * *Files identical despite different names*

### Comparing `polypharm-0.3.8/polypharm/helpers.py` & `polypharm-0.4.2/polypharm/helpers.py`

 * *Files identical despite different names*

### Comparing `polypharm-0.3.8/polypharm/polypharm.py` & `polypharm-0.4.2/polypharm/polypharm.py`

 * *Files identical despite different names*

### Comparing `polypharm-0.3.8/polypharm/scripts/report.py` & `polypharm-0.4.2/polypharm/scripts/report.py`

 * *Files identical despite different names*

### Comparing `polypharm-0.3.8/polypharm/templates/ifd.inp` & `polypharm-0.4.2/polypharm/templates/ifd.inp`

 * *Files identical despite different names*

### Comparing `polypharm-0.3.8/polypharm.egg-info/PKG-INFO` & `polypharm-0.4.2/polypharm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polypharm
-Version: 0.3.8
+Version: 0.4.2
 Summary: A Python-based library to perform IFD and MMGBSA calculations on different targets using a polypharmacological approach.
 Author-email: Mauricio Bedoya <mbedoya@ucm.cl>, Francisco Adasme <fadasme@ucm.cl>
 License: MIT License
         
         Copyright (c) 2023 Mauricio Bedoya
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,20 +31,26 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: pandas>=1.4.3
+Requires-Dist: jinja2>=3.1.2
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: sphinx-rtd-theme; extra == "dev"
 
 # Polypharm
 
-A Python-based library to perform induced fit docking (IFD) and MM/GBSA
+[<img align="left" src="./polypharm/assets/polypharm_logo_transparent_001.png" width="250" />](./polypharm/assets/polypharm_logo_transparent_001.png) A Python-based library to perform induced fit docking (IFD) and MM/GBSA
 calculations on different targets using a polypharmacological approach.
 
 Refer to the [official documentation](http://polypharm.rtfd.io/) for
 details about installation, usage, methodology, and developer interface.
 
 ## Installation
```

### Comparing `polypharm-0.3.8/pyproject.toml` & `polypharm-0.4.2/pyproject.toml`

 * *Files identical despite different names*

