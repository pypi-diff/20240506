# Comparing `tmp/sag-py-cache-decorator-0.1.1.tar.gz` & `tmp/sag_py_cache_decorator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-cache-decorator-0.1.1.tar", last modified: Thu Feb 15 09:37:47 2024, max compression
+gzip compressed data, was "sag_py_cache_decorator-0.1.2.tar", last modified: Mon May  6 10:40:38 2024, max compression
```

## Comparing `sag-py-cache-decorator-0.1.1.tar` & `sag_py_cache_decorator-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:37:47.888873 sag-py-cache-decorator-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-15 09:37:39.000000 sag-py-cache-decorator-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-02-15 09:37:47.888873 sag-py-cache-decorator-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-02-15 09:37:39.000000 sag-py-cache-decorator-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-15 09:37:39.000000 sag-py-cache-decorator-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:37:47.884873 sag-py-cache-decorator-0.1.1/sag_py_cache_decorator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 09:37:39.000000 sag-py-cache-decorator-0.1.1/sag_py_cache_decorator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:37:47.888873 sag-py-cache-decorator-0.1.1/sag_py_cache_decorator/cache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 09:37:39.000000 sag-py-cache-decorator-0.1.1/sag_py_cache_decorator/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-02-15 09:37:39.000000 sag-py-cache-decorator-0.1.1/sag_py_cache_decorator/cache/key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-15 09:37:39.000000 sag-py-cache-decorator-0.1.1/sag_py_cache_decorator/cache/lru.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-02-15 09:37:39.000000 sag-py-cache-decorator-0.1.1/sag_py_cache_decorator/lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 09:37:39.000000 sag-py-cache-decorator-0.1.1/sag_py_cache_decorator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:37:47.888873 sag-py-cache-decorator-0.1.1/sag_py_cache_decorator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-02-15 09:37:47.000000 sag-py-cache-decorator-0.1.1/sag_py_cache_decorator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-02-15 09:37:47.000000 sag-py-cache-decorator-0.1.1/sag_py_cache_decorator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 09:37:47.000000 sag-py-cache-decorator-0.1.1/sag_py_cache_decorator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-15 09:37:47.000000 sag-py-cache-decorator-0.1.1/sag_py_cache_decorator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-15 09:37:47.000000 sag-py-cache-decorator-0.1.1/sag_py_cache_decorator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-15 09:37:47.888873 sag-py-cache-decorator-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-02-15 09:37:39.000000 sag-py-cache-decorator-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:37:47.888873 sag-py-cache-decorator-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-02-15 09:37:39.000000 sag-py-cache-decorator-0.1.1/tests/test_lru_cache_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-02-15 09:37:39.000000 sag-py-cache-decorator-0.1.1/tests/test_lru_cache_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:40:38.544207 sag_py_cache_decorator-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-06 10:40:34.000000 sag_py_cache_decorator-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-05-06 10:40:38.544207 sag_py_cache_decorator-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-06 10:40:34.000000 sag_py_cache_decorator-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-06 10:40:34.000000 sag_py_cache_decorator-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:40:38.540207 sag_py_cache_decorator-0.1.2/sag_py_cache_decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:40:34.000000 sag_py_cache_decorator-0.1.2/sag_py_cache_decorator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:40:38.544207 sag_py_cache_decorator-0.1.2/sag_py_cache_decorator/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:40:34.000000 sag_py_cache_decorator-0.1.2/sag_py_cache_decorator/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-06 10:40:34.000000 sag_py_cache_decorator-0.1.2/sag_py_cache_decorator/cache/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-06 10:40:34.000000 sag_py_cache_decorator-0.1.2/sag_py_cache_decorator/cache/lru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-06 10:40:34.000000 sag_py_cache_decorator-0.1.2/sag_py_cache_decorator/lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:40:34.000000 sag_py_cache_decorator-0.1.2/sag_py_cache_decorator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:40:38.544207 sag_py_cache_decorator-0.1.2/sag_py_cache_decorator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-05-06 10:40:38.000000 sag_py_cache_decorator-0.1.2/sag_py_cache_decorator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-06 10:40:38.000000 sag_py_cache_decorator-0.1.2/sag_py_cache_decorator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:40:38.000000 sag_py_cache_decorator-0.1.2/sag_py_cache_decorator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-06 10:40:38.000000 sag_py_cache_decorator-0.1.2/sag_py_cache_decorator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 10:40:38.000000 sag_py_cache_decorator-0.1.2/sag_py_cache_decorator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 10:40:38.544207 sag_py_cache_decorator-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-06 10:40:34.000000 sag_py_cache_decorator-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:40:38.544207 sag_py_cache_decorator-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-05-06 10:40:34.000000 sag_py_cache_decorator-0.1.2/tests/test_lru_cache_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-06 10:40:34.000000 sag_py_cache_decorator-0.1.2/tests/test_lru_cache_sync.py
```

### Comparing `sag-py-cache-decorator-0.1.1/LICENSE.txt` & `sag_py_cache_decorator-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-cache-decorator-0.1.1/PKG-INFO` & `sag_py_cache_decorator-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-cache-decorator
-Version: 0.1.1
+Version: 0.1.2
 Summary: A decorator to cache method call results with similar parameters
 Home-page: https://github.com/SamhammerAG/sag_py_cache_decorator
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_cache_decorator
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_cache_decorator/issues
@@ -23,14 +23,16 @@
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage-lcov; extra == "dev"
+Requires-Dist: toml; extra == "dev"
+Requires-Dist: coverage==6.5.0; extra == "dev"
 Requires-Dist: mock; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
 
 # sag_py_cache_decorator
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
 [![Known Vulnerabilities][snyk-image]][snyk-url]
@@ -110,14 +112,21 @@
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
+* Use the chosen tag in the requirements.txt-file of the project you want to test this library in, eg. `sag_py_cache_decorator==<your tag>`
+* Rebuild/redeploy your project
 
 [codeclimate-image]:https://api.codeclimate.com/v1/badges/e29dcd8f76877962c93b/maintainability
 [codeclimate-url]:https://codeclimate.com/github/SamhammerAG/sag_py_cache_decorator/maintainability
 [coveralls-image]:https://coveralls.io/repos/github/SamhammerAG/sag_py_cache_decorator/badge.svg?branch=master
 [coveralls-url]:https://coveralls.io/github/SamhammerAG/sag_py_cache_decorator?branch=master
 [snyk-image]:https://snyk.io/test/github/SamhammerAG/sag_py_cache_decorator/badge.svg
 [snyk-url]:https://snyk.io/test/github/SamhammerAG/sag_py_cache_decorator
```

### Comparing `sag-py-cache-decorator-0.1.1/README.md` & `sag_py_cache_decorator-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -78,14 +78,21 @@
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
+* Use the chosen tag in the requirements.txt-file of the project you want to test this library in, eg. `sag_py_cache_decorator==<your tag>`
+* Rebuild/redeploy your project
 
 [codeclimate-image]:https://api.codeclimate.com/v1/badges/e29dcd8f76877962c93b/maintainability
 [codeclimate-url]:https://codeclimate.com/github/SamhammerAG/sag_py_cache_decorator/maintainability
 [coveralls-image]:https://coveralls.io/repos/github/SamhammerAG/sag_py_cache_decorator/badge.svg?branch=master
 [coveralls-url]:https://coveralls.io/github/SamhammerAG/sag_py_cache_decorator?branch=master
 [snyk-image]:https://snyk.io/test/github/SamhammerAG/sag_py_cache_decorator/badge.svg
 [snyk-url]:https://snyk.io/test/github/SamhammerAG/sag_py_cache_decorator
```

### Comparing `sag-py-cache-decorator-0.1.1/sag_py_cache_decorator/cache/key.py` & `sag_py_cache_decorator-0.1.2/sag_py_cache_decorator/cache/key.py`

 * *Files identical despite different names*

### Comparing `sag-py-cache-decorator-0.1.1/sag_py_cache_decorator/cache/lru.py` & `sag_py_cache_decorator-0.1.2/sag_py_cache_decorator/cache/lru.py`

 * *Files identical despite different names*

### Comparing `sag-py-cache-decorator-0.1.1/sag_py_cache_decorator/lru_cache.py` & `sag_py_cache_decorator-0.1.2/sag_py_cache_decorator/lru_cache.py`

 * *Files identical despite different names*

### Comparing `sag-py-cache-decorator-0.1.1/sag_py_cache_decorator.egg-info/PKG-INFO` & `sag_py_cache_decorator-0.1.2/sag_py_cache_decorator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-cache-decorator
-Version: 0.1.1
+Version: 0.1.2
 Summary: A decorator to cache method call results with similar parameters
 Home-page: https://github.com/SamhammerAG/sag_py_cache_decorator
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_cache_decorator
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_cache_decorator/issues
@@ -23,14 +23,16 @@
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: coverage-lcov; extra == "dev"
+Requires-Dist: toml; extra == "dev"
+Requires-Dist: coverage==6.5.0; extra == "dev"
 Requires-Dist: mock; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
 
 # sag_py_cache_decorator
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
 [![Known Vulnerabilities][snyk-image]][snyk-url]
@@ -110,14 +112,21 @@
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
+* Use the chosen tag in the requirements.txt-file of the project you want to test this library in, eg. `sag_py_cache_decorator==<your tag>`
+* Rebuild/redeploy your project
 
 [codeclimate-image]:https://api.codeclimate.com/v1/badges/e29dcd8f76877962c93b/maintainability
 [codeclimate-url]:https://codeclimate.com/github/SamhammerAG/sag_py_cache_decorator/maintainability
 [coveralls-image]:https://coveralls.io/repos/github/SamhammerAG/sag_py_cache_decorator/badge.svg?branch=master
 [coveralls-url]:https://coveralls.io/github/SamhammerAG/sag_py_cache_decorator?branch=master
 [snyk-image]:https://snyk.io/test/github/SamhammerAG/sag_py_cache_decorator/badge.svg
 [snyk-url]:https://snyk.io/test/github/SamhammerAG/sag_py_cache_decorator
```

### Comparing `sag-py-cache-decorator-0.1.1/sag_py_cache_decorator.egg-info/SOURCES.txt` & `sag_py_cache_decorator-0.1.2/sag_py_cache_decorator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sag-py-cache-decorator-0.1.1/setup.py` & `sag_py_cache_decorator-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     REQS = fin.read().splitlines()
 
 with open("requirements-dev.txt", "r") as fin:
     REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
 
 setuptools.setup(
     name="sag-py-cache-decorator",
-    version="0.1.1",
+    version="0.1.2",
     description="A decorator to cache method call results with similar parameters",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_cache_decorator",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
```

### Comparing `sag-py-cache-decorator-0.1.1/tests/test_lru_cache_async.py` & `sag_py_cache_decorator-0.1.2/tests/test_lru_cache_async.py`

 * *Files identical despite different names*

### Comparing `sag-py-cache-decorator-0.1.1/tests/test_lru_cache_sync.py` & `sag_py_cache_decorator-0.1.2/tests/test_lru_cache_sync.py`

 * *Files identical despite different names*

