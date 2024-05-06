# Comparing `tmp/deprogressapi-0.4.0.tar.gz` & `tmp/deprogressapi-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deprogressapi-0.4.0.tar", last modified: Wed Mar 20 14:18:16 2024, max compression
+gzip compressed data, was "deprogressapi-0.4.1.tar", last modified: Mon May  6 09:33:30 2024, max compression
```

## Comparing `deprogressapi-0.4.0.tar` & `deprogressapi-0.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:18:16.928589 deprogressapi-0.4.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:18:16.922588 deprogressapi-0.4.0/LICENSES/
--rw-rw-rw-   0 root         (0) root         (0)    10280 2024-03-20 14:15:27.000000 deprogressapi-0.4.0/LICENSES/Apache-2.0.txt
--rw-rw-rw-   0 root         (0) root         (0)    17023 2024-03-20 14:15:27.000000 deprogressapi-0.4.0/LICENSES/CC-BY-4.0.txt
--rw-rw-rw-   0 root         (0) root         (0)     7048 2024-03-20 14:15:27.000000 deprogressapi-0.4.0/LICENSES/CC0-1.0.txt
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-03-20 14:17:48.000000 deprogressapi-0.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8641 2024-03-20 14:18:16.927589 deprogressapi-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6294 2024-03-20 14:17:48.000000 deprogressapi-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:18:16.924588 deprogressapi-0.4.0/deprogressapi/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2024-03-20 14:17:48.000000 deprogressapi-0.4.0/deprogressapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-03-20 14:18:16.928589 deprogressapi-0.4.0/deprogressapi/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     9491 2024-03-20 14:17:48.000000 deprogressapi-0.4.0/deprogressapi/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2487 2024-03-20 14:17:48.000000 deprogressapi-0.4.0/deprogressapi/print.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 14:17:49.000000 deprogressapi-0.4.0/deprogressapi/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     2093 2024-03-20 14:17:48.000000 deprogressapi-0.4.0/deprogressapi/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     2490 2024-03-20 14:17:48.000000 deprogressapi-0.4.0/deprogressapi/tree.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 14:18:16.925588 deprogressapi-0.4.0/deprogressapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8641 2024-03-20 14:18:16.000000 deprogressapi-0.4.0/deprogressapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      501 2024-03-20 14:18:16.000000 deprogressapi-0.4.0/deprogressapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 14:18:16.000000 deprogressapi-0.4.0/deprogressapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 14:18:16.000000 deprogressapi-0.4.0/deprogressapi.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      259 2024-03-20 14:18:16.000000 deprogressapi-0.4.0/deprogressapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-20 14:18:16.000000 deprogressapi-0.4.0/deprogressapi.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     3095 2024-03-20 14:17:48.000000 deprogressapi-0.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-20 14:18:16.928589 deprogressapi-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      331 2024-03-20 14:17:48.000000 deprogressapi-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:33:30.691168 deprogressapi-0.4.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:33:30.687168 deprogressapi-0.4.1/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    10280 2024-05-06 09:33:04.000000 deprogressapi-0.4.1/LICENSES/Apache-2.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)    17023 2024-05-06 09:33:04.000000 deprogressapi-0.4.1/LICENSES/CC-BY-4.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-05-06 09:33:04.000000 deprogressapi-0.4.1/LICENSES/CC0-1.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-05-06 09:33:04.000000 deprogressapi-0.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8898 2024-05-06 09:33:30.691168 deprogressapi-0.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6289 2024-05-06 09:33:04.000000 deprogressapi-0.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:33:30.687168 deprogressapi-0.4.1/deprogressapi/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2024-05-06 09:33:04.000000 deprogressapi-0.4.1/deprogressapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-06 09:33:30.691168 deprogressapi-0.4.1/deprogressapi/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     9491 2024-05-06 09:33:04.000000 deprogressapi-0.4.1/deprogressapi/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2024-05-06 09:33:04.000000 deprogressapi-0.4.1/deprogressapi/print.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-06 09:33:04.000000 deprogressapi-0.4.1/deprogressapi/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2024-05-06 09:33:04.000000 deprogressapi-0.4.1/deprogressapi/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2024-05-06 09:33:04.000000 deprogressapi-0.4.1/deprogressapi/tree.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:33:30.687168 deprogressapi-0.4.1/deprogressapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8898 2024-05-06 09:33:30.000000 deprogressapi-0.4.1/deprogressapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      501 2024-05-06 09:33:30.000000 deprogressapi-0.4.1/deprogressapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 09:33:30.000000 deprogressapi-0.4.1/deprogressapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 09:33:30.000000 deprogressapi-0.4.1/deprogressapi.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      307 2024-05-06 09:33:30.000000 deprogressapi-0.4.1/deprogressapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-06 09:33:30.000000 deprogressapi-0.4.1/deprogressapi.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3330 2024-05-06 09:33:04.000000 deprogressapi-0.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 09:33:30.691168 deprogressapi-0.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      331 2024-05-06 09:33:04.000000 deprogressapi-0.4.1/setup.py
```

### Comparing `deprogressapi-0.4.0/LICENSES/Apache-2.0.txt` & `deprogressapi-0.4.1/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `deprogressapi-0.4.0/LICENSES/CC-BY-4.0.txt` & `deprogressapi-0.4.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `deprogressapi-0.4.0/LICENSES/CC0-1.0.txt` & `deprogressapi-0.4.1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `deprogressapi-0.4.0/PKG-INFO` & `deprogressapi-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deprogressapi
-Version: 0.4.0
+Version: 0.4.1
 Summary: basic back-end progress api for the data analytics software framework dasf
 Author-email: Daniel Eggert <daniel.eggert@gfz-potsdam.de>, Adam Sasin <sasin@hu-potsdam.de>, "Philipp S. Sommer" <philipp.sommer@hereon.de>
 Maintainer-email: "Philipp S. Sommer" <philipp.sommer@hereon.de>
 License: Apache-2.0
 Project-URL: Homepage, https://git.geomar.de/digital-earth/dasf/dasf-progress-api
 Project-URL: Documentation, https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/
 Project-URL: Source, https://git.geomar.de/digital-earth/dasf/dasf-progress-api
@@ -12,24 +12,29 @@
 Keywords: digital-earth,dasf,pulsar,gfz,hzg,hereon,hgf,helmholtz,remote procedure call,rpc,django,python,websocket,progress reporting
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSES/Apache-2.0.txt
 License-File: LICENSES/CC-BY-4.0.txt
 License-File: LICENSES/CC0-1.0.txt
 Requires-Dist: pydantic<3.0,>=2.2
 Requires-Dist: pydantic-settings
+Requires-Dist: windows-curses; platform_system == "Windows"
 Provides-Extra: testsite
 Requires-Dist: tox; extra == "testsite"
 Requires-Dist: isort==5.12.0; extra == "testsite"
 Requires-Dist: black==23.1.0; extra == "testsite"
 Requires-Dist: blackdoc==0.3.8; extra == "testsite"
 Requires-Dist: flake8==6.0.0; extra == "testsite"
 Requires-Dist: pre-commit; extra == "testsite"
@@ -79,15 +84,15 @@
 ## Installation
 
 Install this package in a dedicated python environment via
 
 ```bash
 python -m venv venv
 source venv/bin/activate
-pip install dasf-progress-api
+pip install deprogessapi
 ```
 
 To use this in a development setup, clone the [source code][source code] from
 gitlab, start the development server and make your changes::
 
 ```bash
 git clone https://git.geomar.de/digital-earth/dasf/dasf-progress-api
```

### Comparing `deprogressapi-0.4.0/README.md` & `deprogressapi-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ## Installation
 
 Install this package in a dedicated python environment via
 
 ```bash
 python -m venv venv
 source venv/bin/activate
-pip install dasf-progress-api
+pip install deprogessapi
 ```
 
 To use this in a development setup, clone the [source code][source code] from
 gitlab, start the development server and make your changes::
 
 ```bash
 git clone https://git.geomar.de/digital-earth/dasf/dasf-progress-api
```

### Comparing `deprogressapi-0.4.0/deprogressapi/__init__.py` & `deprogressapi-0.4.1/deprogressapi/__init__.py`

 * *Files identical despite different names*

### Comparing `deprogressapi-0.4.0/deprogressapi/base.py` & `deprogressapi-0.4.1/deprogressapi/base.py`

 * *Files identical despite different names*

### Comparing `deprogressapi-0.4.0/deprogressapi/print.py` & `deprogressapi-0.4.1/deprogressapi/print.py`

 * *Files identical despite different names*

### Comparing `deprogressapi-0.4.0/deprogressapi/settings.py` & `deprogressapi-0.4.1/deprogressapi/settings.py`

 * *Files identical despite different names*

### Comparing `deprogressapi-0.4.0/deprogressapi/tree.py` & `deprogressapi-0.4.1/deprogressapi/tree.py`

 * *Files identical despite different names*

### Comparing `deprogressapi-0.4.0/deprogressapi.egg-info/PKG-INFO` & `deprogressapi-0.4.1/deprogressapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deprogressapi
-Version: 0.4.0
+Version: 0.4.1
 Summary: basic back-end progress api for the data analytics software framework dasf
 Author-email: Daniel Eggert <daniel.eggert@gfz-potsdam.de>, Adam Sasin <sasin@hu-potsdam.de>, "Philipp S. Sommer" <philipp.sommer@hereon.de>
 Maintainer-email: "Philipp S. Sommer" <philipp.sommer@hereon.de>
 License: Apache-2.0
 Project-URL: Homepage, https://git.geomar.de/digital-earth/dasf/dasf-progress-api
 Project-URL: Documentation, https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/
 Project-URL: Source, https://git.geomar.de/digital-earth/dasf/dasf-progress-api
@@ -12,24 +12,29 @@
 Keywords: digital-earth,dasf,pulsar,gfz,hzg,hereon,hgf,helmholtz,remote procedure call,rpc,django,python,websocket,progress reporting
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSES/Apache-2.0.txt
 License-File: LICENSES/CC-BY-4.0.txt
 License-File: LICENSES/CC0-1.0.txt
 Requires-Dist: pydantic<3.0,>=2.2
 Requires-Dist: pydantic-settings
+Requires-Dist: windows-curses; platform_system == "Windows"
 Provides-Extra: testsite
 Requires-Dist: tox; extra == "testsite"
 Requires-Dist: isort==5.12.0; extra == "testsite"
 Requires-Dist: black==23.1.0; extra == "testsite"
 Requires-Dist: blackdoc==0.3.8; extra == "testsite"
 Requires-Dist: flake8==6.0.0; extra == "testsite"
 Requires-Dist: pre-commit; extra == "testsite"
@@ -79,15 +84,15 @@
 ## Installation
 
 Install this package in a dedicated python environment via
 
 ```bash
 python -m venv venv
 source venv/bin/activate
-pip install dasf-progress-api
+pip install deprogessapi
 ```
 
 To use this in a development setup, clone the [source code][source code] from
 gitlab, start the development server and make your changes::
 
 ```bash
 git clone https://git.geomar.de/digital-earth/dasf/dasf-progress-api
```

### Comparing `deprogressapi-0.4.0/pyproject.toml` & `deprogressapi-0.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -42,24 +42,29 @@
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 
-requires-python = '>= 3.9'
+requires-python = '>= 3.7'
 dependencies = [
     # add your dependencies here
     "pydantic>=2.2,<3.0",
     "pydantic-settings",
+    'windows-curses ; platform_system == "Windows"',
 ]
 
 [project.urls]
 Homepage = 'https://git.geomar.de/digital-earth/dasf/dasf-progress-api'
 Documentation = "https://digital-earth.pages.geomar.de/dasf/dasf-messaging-python/"
 Source = "https://git.geomar.de/digital-earth/dasf/dasf-progress-api"
 Tracker = "https://git.geomar.de/digital-earth/dasf/dasf-progress-api/issues/"
```

