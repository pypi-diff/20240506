# Comparing `tmp/sag-py-execution-time-decorator-1.0.1.tar.gz` & `tmp/sag_py_execution_time_decorator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-execution-time-decorator-1.0.1.tar", last modified: Mon Jul 10 04:42:39 2023, max compression
+gzip compressed data, was "sag_py_execution_time_decorator-1.0.2.tar", last modified: Mon May  6 12:22:01 2024, max compression
```

## Comparing `sag-py-execution-time-decorator-1.0.1.tar` & `sag_py_execution_time_decorator-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:42:39.193239 sag-py-execution-time-decorator-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-07-10 04:42:39.193239 sag-py-execution-time-decorator-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:42:39.193239 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator/execution_time_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:42:39.193239 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-07-10 04:42:39.000000 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-10 04:42:39.000000 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 04:42:39.000000 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-10 04:42:39.000000 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-10 04:42:39.000000 sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-10 04:42:39.197239 sag-py-execution-time-decorator-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:42:39.193239 sag-py-execution-time-decorator-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-10 04:42:29.000000 sag-py-execution-time-decorator-1.0.1/tests/test_execution_time_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:22:01.853528 sag_py_execution_time_decorator-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-06 12:21:55.000000 sag_py_execution_time_decorator-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-06 12:22:01.853528 sag_py_execution_time_decorator-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-06 12:21:55.000000 sag_py_execution_time_decorator-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-06 12:21:55.000000 sag_py_execution_time_decorator-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:22:01.849528 sag_py_execution_time_decorator-1.0.2/sag_py_execution_time_decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-06 12:21:55.000000 sag_py_execution_time_decorator-1.0.2/sag_py_execution_time_decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-06 12:21:55.000000 sag_py_execution_time_decorator-1.0.2/sag_py_execution_time_decorator/execution_time_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:21:55.000000 sag_py_execution_time_decorator-1.0.2/sag_py_execution_time_decorator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:22:01.849528 sag_py_execution_time_decorator-1.0.2/sag_py_execution_time_decorator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-06 12:22:01.000000 sag_py_execution_time_decorator-1.0.2/sag_py_execution_time_decorator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-06 12:22:01.000000 sag_py_execution_time_decorator-1.0.2/sag_py_execution_time_decorator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 12:22:01.000000 sag_py_execution_time_decorator-1.0.2/sag_py_execution_time_decorator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-06 12:22:01.000000 sag_py_execution_time_decorator-1.0.2/sag_py_execution_time_decorator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-06 12:22:01.000000 sag_py_execution_time_decorator-1.0.2/sag_py_execution_time_decorator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 12:22:01.853528 sag_py_execution_time_decorator-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-06 12:21:55.000000 sag_py_execution_time_decorator-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:22:01.849528 sag_py_execution_time_decorator-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-06 12:21:55.000000 sag_py_execution_time_decorator-1.0.2/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-06 12:21:55.000000 sag_py_execution_time_decorator-1.0.2/tests/test_execution_time_decorator.py
```

### Comparing `sag-py-execution-time-decorator-1.0.1/LICENSE.txt` & `sag_py_execution_time_decorator-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-execution-time-decorator-1.0.1/PKG-INFO` & `sag_py_execution_time_decorator-1.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-execution-time-decorator
-Version: 1.0.1
+Version: 1.0.2
 Summary: A decorator for methods to log the execution time (sync and async)
 Home-page: https://github.com/SamhammerAG/sag_py_execution_time_decorator
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_execution_time_decorator
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_execution_time_decorator/issues
@@ -14,16 +14,27 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE.txt
+Provides-Extra: dev
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: coverage-lcov; extra == "dev"
+Requires-Dist: toml; extra == "dev"
+Requires-Dist: coverage==6.5.0; extra == "dev"
+Requires-Dist: mock; extra == "dev"
+Requires-Dist: types-mock; extra == "dev"
 
 # sag_py_execution_time_decorator
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
 [![Known Vulnerabilities][snyk-image]][snyk-url]
 
 A decorator for methods to log the execution time (sync and async)
@@ -88,13 +99,21 @@
 * Restart pycharm
 
 ## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
 
+## How to test
+
+To avoid publishing to pypi unnecessarily you can do as follows
+
+* Tag your branch however you like
+* Use the chosen tag in the requirements.txt-file of the project you want to test this library in, eg. `sag_py_execution_time_decorator==<your tag>`
+* Rebuild/redeploy your project
+
 [codeclimate-image]:https://api.codeclimate.com/v1/badges/fa4312e587c8185db077/maintainability
 [codeclimate-url]:https://codeclimate.com/github/SamhammerAG/sag_py_execution_time_decorator/maintainability
 [coveralls-image]:https://coveralls.io/repos/github/SamhammerAG/sag_py_execution_time_decorator/badge.svg?branch=master
 [coveralls-url]:https://coveralls.io/github/SamhammerAG/sag_py_execution_time_decorator?branch=master
 [snyk-image]:https://snyk.io/test/github/SamhammerAG/sag_py_execution_time_decorator/badge.svg
 [snyk-url]:https://snyk.io/test/github/SamhammerAG/sag_py_execution_time_decorator
```

### Comparing `sag-py-execution-time-decorator-1.0.1/README.md` & `sag_py_execution_time_decorator-1.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -65,13 +65,21 @@
 * Restart pycharm
 
 ## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
 
+## How to test
+
+To avoid publishing to pypi unnecessarily you can do as follows
+
+* Tag your branch however you like
+* Use the chosen tag in the requirements.txt-file of the project you want to test this library in, eg. `sag_py_execution_time_decorator==<your tag>`
+* Rebuild/redeploy your project
+
 [codeclimate-image]:https://api.codeclimate.com/v1/badges/fa4312e587c8185db077/maintainability
 [codeclimate-url]:https://codeclimate.com/github/SamhammerAG/sag_py_execution_time_decorator/maintainability
 [coveralls-image]:https://coveralls.io/repos/github/SamhammerAG/sag_py_execution_time_decorator/badge.svg?branch=master
 [coveralls-url]:https://coveralls.io/github/SamhammerAG/sag_py_execution_time_decorator?branch=master
 [snyk-image]:https://snyk.io/test/github/SamhammerAG/sag_py_execution_time_decorator/badge.svg
 [snyk-url]:https://snyk.io/test/github/SamhammerAG/sag_py_execution_time_decorator
```

### Comparing `sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator/execution_time_decorator.py` & `sag_py_execution_time_decorator-1.0.2/sag_py_execution_time_decorator/execution_time_decorator.py`

 * *Files identical despite different names*

### Comparing `sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator.egg-info/PKG-INFO` & `sag_py_execution_time_decorator-1.0.2/sag_py_execution_time_decorator.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-execution-time-decorator
-Version: 1.0.1
+Version: 1.0.2
 Summary: A decorator for methods to log the execution time (sync and async)
 Home-page: https://github.com/SamhammerAG/sag_py_execution_time_decorator
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_execution_time_decorator
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_execution_time_decorator/issues
@@ -14,16 +14,27 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE.txt
+Provides-Extra: dev
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: coverage-lcov; extra == "dev"
+Requires-Dist: toml; extra == "dev"
+Requires-Dist: coverage==6.5.0; extra == "dev"
+Requires-Dist: mock; extra == "dev"
+Requires-Dist: types-mock; extra == "dev"
 
 # sag_py_execution_time_decorator
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
 [![Known Vulnerabilities][snyk-image]][snyk-url]
 
 A decorator for methods to log the execution time (sync and async)
@@ -88,13 +99,21 @@
 * Restart pycharm
 
 ## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
 
+## How to test
+
+To avoid publishing to pypi unnecessarily you can do as follows
+
+* Tag your branch however you like
+* Use the chosen tag in the requirements.txt-file of the project you want to test this library in, eg. `sag_py_execution_time_decorator==<your tag>`
+* Rebuild/redeploy your project
+
 [codeclimate-image]:https://api.codeclimate.com/v1/badges/fa4312e587c8185db077/maintainability
 [codeclimate-url]:https://codeclimate.com/github/SamhammerAG/sag_py_execution_time_decorator/maintainability
 [coveralls-image]:https://coveralls.io/repos/github/SamhammerAG/sag_py_execution_time_decorator/badge.svg?branch=master
 [coveralls-url]:https://coveralls.io/github/SamhammerAG/sag_py_execution_time_decorator?branch=master
 [snyk-image]:https://snyk.io/test/github/SamhammerAG/sag_py_execution_time_decorator/badge.svg
 [snyk-url]:https://snyk.io/test/github/SamhammerAG/sag_py_execution_time_decorator
```

### Comparing `sag-py-execution-time-decorator-1.0.1/sag_py_execution_time_decorator.egg-info/SOURCES.txt` & `sag_py_execution_time_decorator-1.0.2/sag_py_execution_time_decorator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sag-py-execution-time-decorator-1.0.1/setup.py` & `sag_py_execution_time_decorator-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     REQS = fin.read().splitlines()
 
 with open("requirements-dev.txt", "r") as fin:
     REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
 
 setuptools.setup(
     name="sag-py-execution-time-decorator",
-    version="1.0.1",
+    version="1.0.2",
     description="A decorator for methods to log the execution time (sync and async)",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_execution_time_decorator",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
```

### Comparing `sag-py-execution-time-decorator-1.0.1/tests/test_data.py` & `sag_py_execution_time_decorator-1.0.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `sag-py-execution-time-decorator-1.0.1/tests/test_execution_time_decorator.py` & `sag_py_execution_time_decorator-1.0.2/tests/test_execution_time_decorator.py`

 * *Files identical despite different names*

