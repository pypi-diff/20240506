# Comparing `tmp/sag-py-logging-0.3.3.tar.gz` & `tmp/sag_py_logging-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-logging-0.3.3.tar", last modified: Fri May 12 12:00:09 2023, max compression
+gzip compressed data, was "sag_py_logging-0.3.4.tar", last modified: Mon May  6 10:25:16 2024, max compression
```

## Comparing `sag-py-logging-0.3.3.tar` & `sag_py_logging-0.3.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:00:09.022979 sag-py-logging-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-12 12:00:09.022979 sag-py-logging-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:00:09.022979 sag-py-logging-0.3.3/sag_py_logging/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/sag_py_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/sag_py_logging/console_extra_field_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/sag_py_logging/log_config_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/sag_py_logging/log_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/sag_py_logging/log_config_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/sag_py_logging/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/sag_py_logging/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:00:09.022979 sag-py-logging-0.3.3/sag_py_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-12 12:00:09.000000 sag-py-logging-0.3.3/sag_py_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-12 12:00:09.000000 sag-py-logging-0.3.3/sag_py_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 12:00:09.000000 sag-py-logging-0.3.3/sag_py_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 12:00:09.000000 sag-py-logging-0.3.3/sag_py_logging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-12 12:00:09.000000 sag-py-logging-0.3.3/sag_py_logging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-12 12:00:09.022979 sag-py-logging-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:00:09.022979 sag-py-logging-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/tests/test_console_extra_field_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/tests/test_log_config_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/tests/test_log_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/tests/test_log_config_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:25:16.678125 sag_py_logging-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-06 10:25:13.000000 sag_py_logging-0.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-06 10:25:16.678125 sag_py_logging-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-06 10:25:13.000000 sag_py_logging-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-06 10:25:13.000000 sag_py_logging-0.3.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:25:16.674125 sag_py_logging-0.3.4/sag_py_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-06 10:25:13.000000 sag_py_logging-0.3.4/sag_py_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-06 10:25:13.000000 sag_py_logging-0.3.4/sag_py_logging/console_extra_field_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-06 10:25:13.000000 sag_py_logging-0.3.4/sag_py_logging/log_config_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-06 10:25:13.000000 sag_py_logging-0.3.4/sag_py_logging/log_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-06 10:25:13.000000 sag_py_logging-0.3.4/sag_py_logging/log_config_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-06 10:25:13.000000 sag_py_logging-0.3.4/sag_py_logging/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:25:13.000000 sag_py_logging-0.3.4/sag_py_logging/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:25:16.674125 sag_py_logging-0.3.4/sag_py_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-06 10:25:16.000000 sag_py_logging-0.3.4/sag_py_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-06 10:25:16.000000 sag_py_logging-0.3.4/sag_py_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:25:16.000000 sag_py_logging-0.3.4/sag_py_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-06 10:25:16.000000 sag_py_logging-0.3.4/sag_py_logging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-06 10:25:16.000000 sag_py_logging-0.3.4/sag_py_logging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 10:25:16.678125 sag_py_logging-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-06 10:25:13.000000 sag_py_logging-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:25:16.674125 sag_py_logging-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-06 10:25:13.000000 sag_py_logging-0.3.4/tests/test_console_extra_field_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-06 10:25:13.000000 sag_py_logging-0.3.4/tests/test_log_config_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-06 10:25:13.000000 sag_py_logging-0.3.4/tests/test_log_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-06 10:25:13.000000 sag_py_logging-0.3.4/tests/test_log_config_processors.py
```

### Comparing `sag-py-logging-0.3.3/LICENSE.txt` & `sag_py_logging-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.3/PKG-INFO` & `sag_py_logging-0.3.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-logging
-Version: 0.3.3
+Version: 0.3.4
 Summary: Initialize logging from a configuration json
 Home-page: https://github.com/SamhammerAG/sag_py_logging
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_logging
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_logging/issues
@@ -14,18 +14,34 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 Provides-Extra: dev
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
+Requires-Dist: attrs; extra == "dev"
+Requires-Dist: Jinja2>=3.1.2; extra == "dev"
+Requires-Dist: tomli>=2.0.1; extra == "dev"
 Provides-Extra: jinja
+Requires-Dist: Jinja2>=3.1.2; extra == "jinja"
 Provides-Extra: toml
-License-File: LICENSE.txt
+Requires-Dist: tomli>=2.0.1; extra == "toml"
 
 # sag_py_logging
 
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
 [![Known Vulnerabilities](https://snyk.io/test/github/SamhammerAG/sag_py_logging/badge.svg)](https://snyk.io/test/github/SamhammerAG/sag_py_logging)
 
@@ -193,7 +209,15 @@
 * Ctl+Alt+S => Click Tools => Actions on save => Reformat code
 * Restart pycharm
 
 ## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
+
+## How to test
+
+To avoid publishing to pypi unnecessarily you can do as follows
+
+* Tag your branch however you like
+* Use the chosen tag in the requirements.txt-file of the project you want to test this library in, eg. `sag_py_logging==<your tag>`
+* Rebuild/redeploy your project
```

### Comparing `sag-py-logging-0.3.3/README.md` & `sag_py_logging-0.3.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -168,7 +168,15 @@
 * Ctl+Alt+S => Click Tools => Actions on save => Reformat code
 * Restart pycharm
 
 ## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
+
+## How to test
+
+To avoid publishing to pypi unnecessarily you can do as follows
+
+* Tag your branch however you like
+* Use the chosen tag in the requirements.txt-file of the project you want to test this library in, eg. `sag_py_logging==<your tag>`
+* Rebuild/redeploy your project
```

### Comparing `sag-py-logging-0.3.3/sag_py_logging/console_extra_field_filter.py` & `sag_py_logging-0.3.4/sag_py_logging/console_extra_field_filter.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.3/sag_py_logging/log_config_initializer.py` & `sag_py_logging-0.3.4/sag_py_logging/log_config_initializer.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.3/sag_py_logging/log_config_loader.py` & `sag_py_logging-0.3.4/sag_py_logging/log_config_loader.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.3/sag_py_logging/log_config_processors.py` & `sag_py_logging-0.3.4/sag_py_logging/log_config_processors.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.3/sag_py_logging.egg-info/PKG-INFO` & `sag_py_logging-0.3.4/sag_py_logging.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-logging
-Version: 0.3.3
+Version: 0.3.4
 Summary: Initialize logging from a configuration json
 Home-page: https://github.com/SamhammerAG/sag_py_logging
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_logging
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_logging/issues
@@ -14,18 +14,34 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 Provides-Extra: dev
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
+Requires-Dist: attrs; extra == "dev"
+Requires-Dist: Jinja2>=3.1.2; extra == "dev"
+Requires-Dist: tomli>=2.0.1; extra == "dev"
 Provides-Extra: jinja
+Requires-Dist: Jinja2>=3.1.2; extra == "jinja"
 Provides-Extra: toml
-License-File: LICENSE.txt
+Requires-Dist: tomli>=2.0.1; extra == "toml"
 
 # sag_py_logging
 
 [![Maintainability][codeclimate-image]][codeclimate-url]
 [![Coverage Status][coveralls-image]][coveralls-url]
 [![Known Vulnerabilities](https://snyk.io/test/github/SamhammerAG/sag_py_logging/badge.svg)](https://snyk.io/test/github/SamhammerAG/sag_py_logging)
 
@@ -193,7 +209,15 @@
 * Ctl+Alt+S => Click Tools => Actions on save => Reformat code
 * Restart pycharm
 
 ## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
+
+## How to test
+
+To avoid publishing to pypi unnecessarily you can do as follows
+
+* Tag your branch however you like
+* Use the chosen tag in the requirements.txt-file of the project you want to test this library in, eg. `sag_py_logging==<your tag>`
+* Rebuild/redeploy your project
```

### Comparing `sag-py-logging-0.3.3/sag_py_logging.egg-info/SOURCES.txt` & `sag_py_logging-0.3.4/sag_py_logging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.3/setup.py` & `sag_py_logging-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
 
 JINJA_EXTRA = [item.split(" #", 1)[0] for item in REQS_DEV if "# extras_require jinia" in item]
 TOMLI_EXTRA = [item.split(" #", 1)[0] for item in REQS_DEV if "# extras_require tomli" in item]
 
 setuptools.setup(
     name="sag-py-logging",
-    version="0.3.3",
+    version="0.3.4",
     description="Initialize logging from a configuration json",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_logging",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
```

### Comparing `sag-py-logging-0.3.3/tests/test_console_extra_field_filter.py` & `sag_py_logging-0.3.4/tests/test_console_extra_field_filter.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.3/tests/test_log_config_initializer.py` & `sag_py_logging-0.3.4/tests/test_log_config_initializer.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.3/tests/test_log_config_loader.py` & `sag_py_logging-0.3.4/tests/test_log_config_loader.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.3/tests/test_log_config_processors.py` & `sag_py_logging-0.3.4/tests/test_log_config_processors.py`

 * *Files identical despite different names*

