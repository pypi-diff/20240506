# Comparing `tmp/qase_python_commons-3.0.0.tar.gz` & `tmp/qase_python_commons-3.0.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase_python_commons-3.0.0.tar", last modified: Tue Apr 23 20:00:34 2024, max compression
+gzip compressed data, was "qase_python_commons-3.0.2b1.tar", last modified: Mon May  6 08:33:04 2024, max compression
```

## Comparing `qase_python_commons-3.0.0.tar` & `qase_python_commons-3.0.2b1.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.408674 qase_python_commons-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-23 20:00:34.408674 qase_python_commons-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:00:34.408674 qase_python_commons-3.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.400674 qase_python_commons-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.400674 qase_python_commons-3.0.0/src/qase/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.400674 qase_python_commons-3.0.0/src/qase/commons/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.400674 qase_python_commons-3.0.0/src/qase/commons/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/exceptions/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.404674 qase_python_commons-3.0.0/src/qase/commons/models/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/models/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/models/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/models/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/models/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/models/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/models/suite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.404674 qase_python_commons-3.0.0/src/qase/commons/profilers/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/profilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/profilers/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/profilers/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/profilers/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.404674 qase_python_commons-3.0.0/src/qase/commons/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7253 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/reporters/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/reporters/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    15002 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/reporters/testops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.404674 qase_python_commons-3.0.0/src/qase/commons/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 20:00:25.000000 qase_python_commons-3.0.0/src/qase/commons/validators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:34.404674 qase_python_commons-3.0.0/src/qase_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-23 20:00:34.000000 qase_python_commons-3.0.0/src/qase_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-23 20:00:34.000000 qase_python_commons-3.0.0/src/qase_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:00:34.000000 qase_python_commons-3.0.0/src/qase_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 20:00:34.000000 qase_python_commons-3.0.0/src/qase_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 20:00:34.000000 qase_python_commons-3.0.0/src/qase_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.394394 qase_python_commons-3.0.2b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-06 08:33:04.394394 qase_python_commons-3.0.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:33:04.394394 qase_python_commons-3.0.2b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.386394 qase_python_commons-3.0.2b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.386394 qase_python_commons-3.0.2b1/src/qase/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.390395 qase_python_commons-3.0.2b1/src/qase/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.390395 qase_python_commons-3.0.2b1/src/qase/commons/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/client/api_v1_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/client/base_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.390395 qase_python_commons-3.0.2b1/src/qase/commons/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/exceptions/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.390395 qase_python_commons-3.0.2b1/src/qase/commons/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/models/suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.390395 qase_python_commons-3.0.2b1/src/qase/commons/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/profilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/profilers/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/profilers/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/profilers/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.394394 qase_python_commons-3.0.2b1/src/qase/commons/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/reporters/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/reporters/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/reporters/testops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.394394 qase_python_commons-3.0.2b1/src/qase/commons/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-06 08:32:56.000000 qase_python_commons-3.0.2b1/src/qase/commons/validators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:33:04.394394 qase_python_commons-3.0.2b1/src/qase_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-06 08:33:04.000000 qase_python_commons-3.0.2b1/src/qase_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-06 08:33:04.000000 qase_python_commons-3.0.2b1/src/qase_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:33:04.000000 qase_python_commons-3.0.2b1/src/qase_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-06 08:33:04.000000 qase_python_commons-3.0.2b1/src/qase_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 08:33:04.000000 qase_python_commons-3.0.2b1/src/qase_python_commons.egg-info/top_level.txt
```

### Comparing `qase_python_commons-3.0.0/PKG-INFO` & `qase_python_commons-3.0.2b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 3.0.0
+Version: 3.0.2b1
 Summary: A library for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: certifi>=2024.2.2
 Requires-Dist: attrs>=23.2.0
-Requires-Dist: qaseio
+Requires-Dist: qaseio==4.0.2
 Requires-Dist: more_itertools
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: mock; extra == "testing"
 Requires-Dist: more_itertools; extra == "testing"
 Requires-Dist: requests; extra == "testing"
```

### Comparing `qase_python_commons-3.0.0/pyproject.toml` & `qase_python_commons-3.0.2b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-python-commons"
-version = "3.0.0"
+version = "3.0.2b1"
 description = "A library for Qase TestOps and Qase Report"
 readme = "README.md"
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
@@ -26,15 +26,15 @@
     'Programming Language :: Python :: 3.12',
 ]
 urls = {"Homepage" = "https://github.com/qase-tms/qase-python/tree/master/qase-python-commons"}
 requires-python = ">=3.7"
 dependencies = [
     "certifi>=2024.2.2",
     "attrs>=23.2.0",
-    "qaseio",
+    "qaseio==4.0.2",
     "more_itertools"
 ]
 
 [project.optional-dependencies]
 testing = [
     "pytest",
     "pytest-cov",
@@ -95,8 +95,8 @@
     "if 0:",
     "if __name__ == .__main__.:",
 
     # Don't complain about abstract methods, they aren't run:
     "@(abc\\.)?abstractmethod",
     ]
 
-ignore_errors = false
+ignore_errors = false
```

### Comparing `qase_python_commons-3.0.0/src/qase/commons/config.py` & `qase_python_commons-3.0.2b1/src/qase/commons/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         except Exception as e:
             self.logger.log("Failed to load config from env vars {e}", "error")
 
     def get(self, key, default=None, value_type=None):
         # Use _get_config method to get the value. If None, return default.
         value = self._get_config(key)
         if value_type and value_type == bool:
-            return self.parseBool(value or default)
+            return self.parseBool(value)
         return value or default
 
     def validate_config(self):
         if self.validator:
             self.validator.validate(self.config)
 
     def set(self, key, value):
@@ -55,7 +55,10 @@
 
     def _get_config(self, key):
         keys = key.split(".")
         config = self.config
         for key in keys[:-1]:
             config = config.get(key, {})
         return config.get(keys[-1], None)
+
+    def __str__(self):
+        return json.dumps(self.config, indent=4, sort_keys=True)
```

### Comparing `qase_python_commons-3.0.0/src/qase/commons/loader.py` & `qase_python_commons-3.0.2b1/src/qase/commons/loader.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.0/src/qase/commons/logger.py` & `qase_python_commons-3.0.2b1/src/qase/commons/logger.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,11 +18,15 @@
         time_str = self._get_timestamp("%H:%M:%S")
         log = f"[Qase][{time_str}][{level}] {message}\n"
         print(log)
         if self.debug:
             with open(self.log_file, 'a') as f:
                 f.write(log)
 
+    def log_debug(self, message: str):
+        if self.debug:
+            self.log(message, 'debug')
+
     @staticmethod
     def _get_timestamp(format: str = "%Y%m%d_%H:%M:%S"):
         now = datetime.datetime.now()
         return now.strftime(format)
```

### Comparing `qase_python_commons-3.0.0/src/qase/commons/models/attachment.py` & `qase_python_commons-3.0.2b1/src/qase/commons/models/attachment.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 import uuid
-from typing import Optional, Union
-from io import BytesIO, StringIO
 import json
 import pathlib
 
+from typing import Optional, Union
+from io import BytesIO, StringIO
+from .basemodel import BaseModel
+
 
-class Attachment:
+class Attachment(BaseModel):
     def __init__(self,
                  file_name: str,
                  mime_type: str,
                  content: Optional[str] = None,
                  file_path: Optional[str] = None,
                  temporary: bool = False):
         self.file_name = file_name
@@ -36,16 +38,17 @@
             return 0
 
     def get_id(self) -> str:
         return self.id
 
     def get_for_upload(self) -> BytesIO:
         if self.file_path:
-            return pathlib.Path(os.path.abspath(self.file_path))
+            with open(self.file_path, "rb") as fc:
+                content = BytesIO(fc.read())
         else:
             if isinstance(self.content, str):
-                content = BytesIO(self.content.encode('utf-8'))
+                content = BytesIO(bytes(self.content, 'utf-8'))
             elif isinstance(self.content, bytes):
                 content = BytesIO(self.content)
         content.name = self.file_name
         content.mime = self.mime_type
         return content
```

### Comparing `qase_python_commons-3.0.0/src/qase/commons/models/result.py` & `qase_python_commons-3.0.2b1/src/qase/commons/models/result.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-from typing import Type, Optional, Union, Dict, List
-from pathlib import PosixPath
 import time
 import uuid
 import json
+
+from typing import Type, Optional, Union, Dict, List
+from pathlib import PosixPath
+from .basemodel import BaseModel
 from .step import Step
 from .suite import Suite
 from .attachment import Attachment
 from .relation import Relation
 from .. import QaseUtils
 
 
-class Field:
+class Field(BaseModel):
     def __init__(self,
                  name: str,
                  value: Union[str, list]):
         self.name = name
         self.value = value
 
 
-class Execution(object):
+class Execution(BaseModel):
     def __init__(self,
                  status: Optional[str] = None,
                  end_time: int = 0,
                  duration: int = 0,
                  stacktrace: Optional[str] = None,
                  thread: Optional[str] = QaseUtils.get_thread_name()
                  ):
@@ -43,15 +45,15 @@
         return self.status
 
     def complete(self):
         self.end_time = time.time()
         self.duration = (int)((self.end_time - self.start_time) * 1000)
 
 
-class Request(object):
+class Request(BaseModel):
     def __init__(self,
                  method: str,
                  url: str,
                  status: int,
                  request_headers: Dict[str, str],
                  request_body: str,
                  response_headers: Dict[str, str],
@@ -61,15 +63,15 @@
         self.status = status
         self.request_headers = request_headers
         self.request_body = request_body
         self.response_headers = response_headers
         self.response_body = response_body
 
 
-class Result(object):
+class Result(BaseModel):
     def __init__(self, title: str, signature: str) -> None:
         self.id: str = str(uuid.uuid4())
         self.title: str = title
         self.signature: str = signature
         self.run_id: Optional[str] = None
         self.testops_id: Optional[int] = None
         self.execution: Type[Execution] = Execution()
@@ -133,11 +135,7 @@
 
     def get_suite_title(self) -> Optional[str]:
         if self.suite:
             return self.suite.title
 
     def set_run_id(self, run_id: str) -> None:
         self.run_id = run_id
-
-    def to_json(self) -> str:
-        return json.dumps(self, default=lambda o: o.__str__() if isinstance(o, PosixPath) else o.__dict__,
-                          sort_keys=False, indent=4)
```

### Comparing `qase_python_commons-3.0.0/src/qase/commons/models/run.py` & `qase_python_commons-3.0.2b1/src/qase/commons/models/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import json
+
 from typing import Optional, List
 
+from .basemodel import BaseModel
+
 
-class RunExecution(object):
+class RunExecution(BaseModel):
     def __init__(self,
                  start_time: float,
                  end_time: float,
                  cumulative_duration: int = 0,
                  ) -> None:
         self.start_time = start_time
         self.end_time = end_time
         self.duration = int((end_time - start_time) * 1000)
         self.cumulative_duration = cumulative_duration
 
     def track(self, result: dict):
         self.cumulative_duration += result["execution"]["duration"]
 
 
-class RunStats(object):
+class RunStats(BaseModel):
     def __init__(self) -> None:
         self.passed = 0
         self.failed = 0
         self.skipped = 0
         self.broken = 0
         self.muted = 0
         self.total = 0
@@ -37,15 +40,15 @@
         elif status == "broken":
             self.broken += 1
         self.total += 1
         if result.get('muted', False):
             self.muted += 1
 
 
-class Run(object):
+class Run(BaseModel):
     def __init__(self,
                  title: str,
                  start_time: float,
                  end_time: float,
                  results: List[str] = [],
                  threads: List[str] = [],
                  suites: List[str] = [],
@@ -56,17 +59,14 @@
         self.execution = RunExecution(start_time=start_time, end_time=end_time)
         self.stats = RunStats()
         self.results = results
         self.threads = threads
         self.suites = suites
         self.environment = environment
 
-    def to_json(self) -> str:
-        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=False, indent=4)
-
     def add_result(self, result: dict):
         compact_result = {
             "id": result["id"],
             "title": result["title"],
             "status": result["execution"]["status"],
             "duration": result["execution"]["duration"],
             "thread": result["execution"]["thread"]
```

### Comparing `qase_python_commons-3.0.0/src/qase/commons/models/runtime.py` & `qase_python_commons-3.0.2b1/src/qase/commons/models/runtime.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.0/src/qase/commons/models/step.py` & `qase_python_commons-3.0.2b1/src/qase/commons/models/step.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,46 @@
-from enum import Enum
-from typing import Optional, Union, Dict, List, Type
 import time
 import uuid
+
+from enum import Enum
+from typing import Optional, Union, Dict, List, Type
 from .attachment import Attachment
+from .basemodel import BaseModel
 
 
 class StepType(Enum):
     TEXT = 'text'
     ASSERT = 'assert'
     GHERKIN = 'gherkin'
     REQUEST = 'request'
     DB_QUERY = 'db_query'
     SLEEP = 'sleep'
 
 
-class StepTextData(object):
+class StepTextData(BaseModel):
     def __init__(self, action: str, expected_result: Optional[str] = None):
         self.action = action
         self.expected_result = expected_result
 
 
-class StepAssertData(object):
+class StepAssertData(BaseModel):
     def __init__(self, expected: str, actual: str, message: str):
         self.expected = expected
         self.actual = actual
         self.message = message
 
 
-class StepGherkinData(object):
+class StepGherkinData(BaseModel):
     def __init__(self, keyword: str, name: str, line: int):
         self.keyword = keyword
         self.name = name
         self.line = line
 
 
-class StepRequestData(object):
+class StepRequestData(BaseModel):
     def __init__(self, request_body: str, request_headers: Dict[str, str], request_method: str, request_url: str):
         self.response_headers = None
         self.response_body = None
         self.status_code = None
         if isinstance(request_body, bytes):
             request_body = request_body.decode('utf-8')
         self.request_body = request_body
@@ -56,25 +58,25 @@
             response_body = response_body.decode('utf-8')
         self.response_body = response_body
         if isinstance(response_headers, bytes):
             response_headers = response_headers.decode('utf-8')
         self.response_headers = response_headers
 
 
-class StepDbQueryData(object):
+class StepDbQueryData(BaseModel):
     def __init__(self, query: str, expected_result: str):
         self.query = query
 
 
-class StepSleepData(object):
+class StepSleepData(BaseModel):
     def __init__(self, duration: int):
         self.duration = duration
 
 
-class StepExecution(object):
+class StepExecution(BaseModel):
     def __init__(self, status: Optional[str] = 'untested', end_time: int = 0, duration: int = 0):
         self.start_time = time.time()
         self.status = status
         self.end_time = end_time
         self.duration = duration
 
     def set_status(self, status: Optional[str]):
@@ -84,15 +86,15 @@
             raise ValueError('Step status must be one of: passed, failed, skipped, untested')
 
     def complete(self):
         self.end_time = time.time()
         self.duration = int((self.end_time - self.start_time) * 1000)
 
 
-class Step(object):
+class Step(BaseModel):
     def __init__(self,
                  step_type: StepType,
                  id: Optional[str],
                  data: Optional[
                      Union[StepTextData, StepAssertData, StepGherkinData, StepRequestData, StepSleepData]] = None,
                  parent_id: Optional[str] = None
                  ):
```

### Comparing `qase_python_commons-3.0.0/src/qase/commons/profilers/network.py` & `qase_python_commons-3.0.2b1/src/qase/commons/profilers/network.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.0/src/qase/commons/profilers/sleep.py` & `qase_python_commons-3.0.2b1/src/qase/commons/profilers/sleep.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.0/src/qase/commons/reporters/core.py` & `qase_python_commons-3.0.2b1/src/qase/commons/reporters/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+import os
+import json
+import time
+
 from ..config import ConfigManager as Config
 from ..logger import Logger
 
 from .report import QaseReport
 from .testops import QaseTestOps
 
 from ..models import Result, Attachment, Runtime
 from typing import Union
 
-import os
-import json
-import time
-
 """
     CoreReporter is a facade for all reporters and it is used to initialize and manage them.
     It is also used to pass configuration and logger to reporters, handle fallback logic and error handling.
 """
 
 
 class QaseCoreReporter:
@@ -24,14 +24,16 @@
         self.execution_plan = None
         self.profilers = []
         self.overhead = 0
 
         self._selective_execution_setup()
         self.fallback = self._fallback_setup()
 
+        self.logger.log_debug(f"Config: {self.config}")
+
         # Reading reporter mode from config file
         mode = config.get("mode", "off")
 
         if mode == 'testops':
             try:
                 self._load_testops_plan()
                 self.reporter = QaseTestOps(config=config, logger=self.logger)
@@ -44,51 +46,59 @@
         else:
             self.reporter = None
 
     def start_run(self) -> Union[str, None]:
         if self.reporter:
             try:
                 ts = time.time()
+                self.logger.log_debug("Starting run")
                 run_id = self.reporter.start_run()
+                self.logger.log_debug(f"Run ID: {run_id}")
                 self.overhead += time.time() - ts
                 return run_id
             except Exception as e:
                 self.logger.log('Failed to start run, disabling reporting', 'info')
                 self.logger.log(e, 'error')
                 self.reporter = None
 
-    def complete_run(self, exit_code=None) -> None:
+    def complete_run(self) -> None:
         if self.reporter:
             try:
                 ts = time.time()
-                self.reporter.complete_run(exit_code)
+                self.logger.log_debug("Completing run")
+                self.reporter.complete_run()
+                self.logger.log_debug("Run completed")
                 self.overhead += time.time() - ts
                 self.logger.log(f"Overhead for Qase Report: {round(self.overhead * 1000)}ms", 'info')
             except Exception as e:
                 # We don't want to disable reporting here
                 self.logger.log('Failed to complete run', 'info')
                 self.logger.log(e, 'error')
 
     def add_result(self, result: Result) -> None:
         if self.reporter:
             try:
                 ts = time.time()
+                self.logger.log_debug(f"Adding result {result}")
                 self.reporter.add_result(result)
+                self.logger.log_debug(f"Result {result.get_title()} added")
                 self.overhead += time.time() - ts
             except Exception as e:
                 # Log error, disable reporting and continue
                 self.logger.log(f'Failed to add result {result.get_title()}', 'info')
                 self.logger.log(e, 'error')
                 self._run_fallback()
 
     def add_attachment(self, attachment: Attachment) -> None:
         if self.reporter:
             try:
                 ts = time.time()
+                self.logger.log_debug(f"Adding attachment {attachment}")
                 self.reporter.add_attachment(attachment)
+                self.logger.log_debug(f"Attachment {attachment.id} added")
                 self.overhead += time.time() - ts
             except Exception as e:
                 # Log error and run fallback
                 self.logger.log('Failed to add attachment', 'info')
                 self.logger.log(e, 'error')
                 self._run_fallback()
```

### Comparing `qase_python_commons-3.0.0/src/qase/commons/reporters/report.py` & `qase_python_commons-3.0.2b1/src/qase/commons/reporters/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.run_id = None
         self.environment = self.config.get("environment", None)
 
     def start_run(self):
         self._check_report_path()
         self.start_time = str(time.time())
 
-    def complete_run(self, exit_code=None):
+    def complete_run(self):
         self.end_time = str(time.time())
         self._compile_report()
 
     def complete_worker(self):
         pass
 
     def add_result(self, result: Result):
```

### Comparing `qase_python_commons-3.0.0/src/qase/commons/utils.py` & `qase_python_commons-3.0.2b1/src/qase/commons/utils.py`

 * *Files identical despite different names*

### Comparing `qase_python_commons-3.0.0/src/qase_python_commons.egg-info/PKG-INFO` & `qase_python_commons-3.0.2b1/src/qase_python_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 3.0.0
+Version: 3.0.2b1
 Summary: A library for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: certifi>=2024.2.2
 Requires-Dist: attrs>=23.2.0
-Requires-Dist: qaseio
+Requires-Dist: qaseio==4.0.2
 Requires-Dist: more_itertools
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: mock; extra == "testing"
 Requires-Dist: more_itertools; extra == "testing"
 Requires-Dist: requests; extra == "testing"
```

### Comparing `qase_python_commons-3.0.0/src/qase_python_commons.egg-info/SOURCES.txt` & `qase_python_commons-3.0.2b1/src/qase_python_commons.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 README.md
 pyproject.toml
 src/qase/commons/__init__.py
 src/qase/commons/config.py
 src/qase/commons/loader.py
 src/qase/commons/logger.py
 src/qase/commons/utils.py
+src/qase/commons/client/api_v1_client.py
+src/qase/commons/client/base_api_client.py
 src/qase/commons/exceptions/reporter.py
 src/qase/commons/models/__init__.py
 src/qase/commons/models/attachment.py
+src/qase/commons/models/basemodel.py
 src/qase/commons/models/relation.py
 src/qase/commons/models/result.py
 src/qase/commons/models/run.py
 src/qase/commons/models/runtime.py
 src/qase/commons/models/step.py
 src/qase/commons/models/suite.py
 src/qase/commons/profilers/__init__.py
```

