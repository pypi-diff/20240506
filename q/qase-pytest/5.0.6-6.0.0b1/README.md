# Comparing `tmp/qase-pytest-5.0.6.tar.gz` & `tmp/qase_pytest-6.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase-pytest-5.0.6.tar", last modified: Wed Apr 10 14:45:12 2024, max compression
+gzip compressed data, was "qase_pytest-6.0.0b1.tar", last modified: Mon May  6 08:53:15 2024, max compression
```

## Comparing `qase-pytest-5.0.6.tar` & `qase_pytest-6.0.0b1.tar`

### file list

```diff
@@ -1,39 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:12.861262 qase-pytest-5.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/CONFIGURATION.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-10 14:45:12.861262 qase-pytest-5.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/UPGRADE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:12.861262 qase-pytest-5.0.6/example/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/example/test_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-10 14:45:12.861262 qase-pytest-5.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:12.857262 qase-pytest-5.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:12.861262 qase-pytest-5.0.6/src/qase_pytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-10 14:45:12.000000 qase-pytest-5.0.6/src/qase_pytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-10 14:45:12.000000 qase-pytest-5.0.6/src/qase_pytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:45:12.000000 qase-pytest-5.0.6/src/qase_pytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 14:45:12.000000 qase-pytest-5.0.6/src/qase_pytest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 14:45:12.000000 qase-pytest-5.0.6/src/qase_pytest.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:45:12.000000 qase-pytest-5.0.6/src/qase_pytest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-10 14:45:12.000000 qase-pytest-5.0.6/src/qase_pytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 14:45:12.000000 qase-pytest-5.0.6/src/qase_pytest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:12.857262 qase-pytest-5.0.6/src/qaseio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:12.861262 qase-pytest-5.0.6/src/qaseio/pytest/
--rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/src/qaseio/pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/src/qaseio/pytest/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/src/qaseio/pytest/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9873 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/src/qaseio/pytest/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:12.861262 qase-pytest-5.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-10 14:45:09.000000 qase-pytest-5.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:53:15.688541 qase_pytest-6.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-05-06 08:53:15.688541 qase_pytest-6.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:53:15.688541 qase_pytest-6.0.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:53:15.684541 qase_pytest-6.0.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:53:15.684541 qase_pytest-6.0.0b1/src/qase/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:53:15.684541 qase_pytest-6.0.0b1/src/qase/pytest/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/src/qase/pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/src/qase/pytest/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/src/qase/pytest/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/src/qase/pytest/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/src/qase/pytest/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-05-06 08:53:09.000000 qase_pytest-6.0.0b1/src/qase/pytest/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:53:15.688541 qase_pytest-6.0.0b1/src/qase_pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7486 2024-05-06 08:53:15.000000 qase_pytest-6.0.0b1/src/qase_pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-06 08:53:15.000000 qase_pytest-6.0.0b1/src/qase_pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:53:15.000000 qase_pytest-6.0.0b1/src/qase_pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-06 08:53:15.000000 qase_pytest-6.0.0b1/src/qase_pytest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 08:53:15.000000 qase_pytest-6.0.0b1/src/qase_pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 08:53:15.000000 qase_pytest-6.0.0b1/src/qase_pytest.egg-info/top_level.txt
```

### Comparing `qase-pytest-5.0.6/LICENSE.txt` & `qase_pytest-6.0.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qase-pytest-5.0.6/PKG-INFO` & `qase_pytest-6.0.0b1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,252 +1,232 @@
-Metadata-Version: 2.1
-Name: qase-pytest
-Version: 5.0.6
-Summary: Qase Pytest Plugin for Qase TestOps and Qase Report
-Home-page: https://github.com/qase-tms/qase-python/tree/master/qase-pytest
-Author: Qase Team
-Author-email: support@qase.io
-License: apache
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Pytest
-Classifier: Programming Language :: Python
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Provides-Extra: testing
-License-File: LICENSE.txt
-License-File: AUTHORS.rst
-
-# [Qase](https://qase.io) Pytest Plugin
+# [Qase TestOps](https://qase.io) Pytest Reporter
 
 [![License](https://lxgaming.github.io/badges/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
 ## Installation
 
-```
+```sh
 pip install qase-pytest
 ```
 
-## Upgrade from 4.x to 5.x
-A new version of qase-pytest reporter has breaking changes. Follow these [guide](UPGRADE.md) that will help you to migrate to a new version.
+## Upgrade from 4.x to 5.x and to 6.x
+
+The new version 6.x of the Pytest reporter has breaking changes.
+To migrate from versions 4.x or 5.x, follow the [upgrade guide](UPGRADE.md).
 
 ## Configuration
 
-Qase Pytest Plugin can be configured in multiple ways:
- - using a config file `qase.config.json`
- - using environment variables
- - using CLI options
+Qase Pytest Reporter is configured in multiple ways:
 
-All configuration options are listed in the following doc: [Configuration](../README.md#configuration).
+- using a config file `qase.config.json`
+- using environment variables
+- using command line options
+
+Environment variables override the values given in the config file, 
+and command line options override both other values.
+
+Configuration options are described in the
+[configuration reference](docs/CONFIGURATION.md).
 
 
 ### Example: qase.config.json
 
-```
+```json
 {
-	"mode": "testops", 
-	"fallback": "report",
-	"report": {
-		"driver": "local",
-		"connection": {
-			"local": {
-				"path": "./build/qase-report",
-				"format": "json" 
-			}
-		}
-	},
-	"testops": {
-		"bulk": true,
-		"api": {
-			"token": "YOUR_API_TOKEN",
-			"host": "qase.io"
-		},
-		"run": {
-            "id": 1,
-			"title": "Test run title",
-			"complete": true
-		},
-        "plan": {
-            "id": 1
-        },
-		"defect": true,
-		"project": "YOUR_PROJECT_CODE",
-		"chunk": 200
-	},
-	"framework": {
-		"pytest": {
-			"capture": {
-				"logs": true,
-				"http": true
-			}
-		}
-	},
-	"environment": "local"
+  "mode": "testops", 
+  "fallback": "report",
+  "testops": {
+    "project": "YOUR_PROJECT_CODE",
+    "api": {
+      "token": "YOUR_API_TOKEN",
+      "host": "qase.io"
+    },
+    "run": {
+      "title": "Test run title"
+    },
+    "batch": {
+      "size": 100
+    }
+  },
+    "report": {
+    "driver": "local",
+    "connection": {
+      "local": {
+        "path": "./build/qase-report",
+        "format": "json" 
+      }
+    }
+  },
+  "framework": {
+    "pytest": {
+      "capture": {
+        "logs": true,
+        "http": true
+      }
+    }
+  },
+  "environment": "local"
 }
 ```
 
 ## Usage
 
 ### Link tests with test cases in Qase TestOps
 
-To link tests in code with tests in Qase TestOps you can use predefined decorators:
+To link the automated tests with the test cases in Qase TestOps, use the `@qase.id()` decorator.
+Other test data, such as case title, system and custom fields,
+can be added with `@qase.title()` and `@qase.fields()`:
 
 ```python
-from qaseio.pytest import qase
+from qase.pytest import qase
 
 @qase.id(13)
 @qase.title("My first test")
 @qase.fields(
     ("severity", "critical"),
-    ("priority", "hight"),
+    ("priority", "high"),
     ("layer", "unit"),
-    ("description", "Try to login in Qase TestOps using login and password"),
-    ("description", "*Precondition 1*. Markdown is supported."),
+    ("description", "Try to login to Qase TestOps using login and password"),
+    ("preconditions", "*Precondition 1*. Markdown is supported."),
 )
 def test_example_1():
     pass
 ```
 
 Each unique number can only be assigned once to the class or function being used.
 
 ### Ignore a particular test
-If you want to exclude a particular test from the report, you can use the `@qase.ignore` decorator:
+
+To exclude a particular test from the report, use the `@qase.ignore` decorator:
 
 ```python
-from qaseio.pytest import qase
+from qase.pytest import qase
 
 @qase.ignore
 def test_example_1():
     pass
 ```
 
 ### Possible test result statuses
 
 - PASSED - when test passed
-- FAILED - when test failed with AssertionError
+- FAILED - when test failed with `AssertionError`
 - BLOCKED - when test failed with any other exception
 - SKIPPED - when test has been skipped
 
 ### Capture network logs
-In order to capture network logs, you need to enable the `http` option in the `capture` section of the `framework` section in the config file.
 
-Qase Pytest reporter will capture all requests and responses and save as a test step automatically.
+To capture the network logs, enable the `http` option in the `framework.capture` section
+of the configuration file.
+
+The Qase Pytest reporter will capture all HTTP requests and responses
+and save them as a test steps automatically.
 
 ### Add attachments to test results
 
-When you need to push some additional information to server you could use
-attachments:
+To upload screenshots, logs, and other information to Qase.io,
+use `qase.attach()`.
+It works both with files in the filesystem and with data available in the code.
+There is no limit on the amount of attachments from a single test.
 
 ```python
 import pytest
-from qaseio.pytest import qase
-
-@pytest.fixture(scope="session")
-def driver():
-    driver = webdriver.Chrome()
-    yield driver
-    logs = "\n".join(str(row) for row in driver.get_log('browser')).encode('utf-8')
-    qase.attach((logs, "text/plain", "browser.log"))
-    driver.quit()
+from qase.pytest import qase
 
-@qase.title("My first test")
+@qase.title("File attachments")
 def test_example_1():
+    # attach files from the filesystem:
     qase.attach("/path/to/file", "/path/to/file/2")
+    # to add multiple attachments, pass them in tuples:
     qase.attach(
         ("/path/to/file/1", "application/json"),
         ("/path/to/file/3", "application/xml"),
     )
 
-@qase.id(12)
-def test_example_2(driver):
-    qase.attach((driver.get_screenshot_as_png(), "image/png", "result.png"))
-```
-
-You could pass as much files as you need.
-
-Also you should know, that if no case id is associated with current test in
-pytest - attachment would not be uploaded:
-
-```python
-import pytest
-from qaseio.pytest import qase
-
 @pytest.fixture(scope="session")
 def driver():
     driver = webdriver.Chrome()
     yield driver
     logs = "\n".join(str(row) for row in driver.get_log('browser')).encode('utf-8')
-    # This would do nothing, because last test does not have case id link
+    # attach logs from a code variable as a text file:
     qase.attach((logs, "text/plain", "browser.log"))
     driver.quit()
 
+@qase.id(12)
 def test_example_2(driver):
-    # This would do nothing
+    # attach the output of driver.get_screenshot_as_png() as a png image
     qase.attach((driver.get_screenshot_as_png(), "image/png", "result.png"))
 ```
 
 ### Linking code with steps
 
-It is possible to link test step with function, or using context.
+To mark a test step, either annotate a function with `@qase.step()`,
+or use the `with qase.step()` context:
 
 ```python
-from qaseio.pytest import qase
+from qase.pytest import qase
 
 @qase.step("First step") # test step name
 def some_step():
     sleep(5)
 
 @qase.step("Second step")  # test step name
 def another_step():
     sleep(3)
 
-...
+# ...
 
 def test_example():
     some_step()
     another_step()
     # test step hash
     with qase.step("Third step"):
         sleep(1)
 ```
 
-### Sending tests to existing testrun
+### Creating new testrun according to current pytest run
 
-Testrun in TestOps will contain only those test results, which are presented in testrun,
-but every test would be executed.
+By default, qase-pytest will create a new test run in Qase TestOps
+and report results to this test run.
+To provide a custom name for this run, add
+the option `--qase-testops-run-title`.
 
 ```bash
 pytest \
     --qase-mode=testops \
     --qase-testops-api-token=<your api token here> \
-    --qase-testops-project=PRJCODE \ # project, where your testrun exists in
-    --qase-testops-run-id=3 # testrun id
+    --qase-testops-project=PRJCODE \ # project, where your testrun would be created
+    --qase-testops-run-title=My\ First\ Automated\ Run
 ```
 
-### Creating test run base on test plan (selective launch)
+### Sending tests to existing testrun
+
+Test results can be reported to an existing test run in Qase using its ID.
+This is useful when a test run combines tests from multiple sources:
 
-Create new testrun base on testplan. Testrun in Qase TestOps will contain only those
-test results. `qase-pytest` supports selective execution
+* manual and automated
+* autotests from different frameworks
+* tests running in multiple shards on different machines
+
+For example, if the test run has ID=3, the following command will
+run tests and report results to this test run:
 
 ```bash
 pytest \
     --qase-mode=testops \
     --qase-testops-api-token=<your api token here> \
-    --qase-testops-project=PRJCODE \ # project, where your testrun exists in
-    --qase-testops-plan-id=3 # testplan id
+    --qase-testops-project=PRJCODE \ # project, where the test run is created
+    --qase-testops-run-id=3 # testrun id
 ```
 
-### Creating new testrun according to current pytest run
+### Creating test run based on test plan (selective launch)
 
-If you want to create a new test run in Qase TestOps for each execution, you can simply 
-skip `--qase-testops-run` option. If you want to provide a custom name for this run, you can add an
-option `--qase-testops-run-title` 
+Create a new testrun base on a testplan. Testrun in Qase TestOps will contain only those
+test results. `qase-pytest` supports selective execution.
 
 ```bash
 pytest \
     --qase-mode=testops \
     --qase-testops-api-token=<your api token here> \
-    --qase-testops-project=PRJCODE \ # project, where your testrun would be created
-    --qase-testops-run-title=My\ First\ Automated\ Run
-```
-
-
+    --qase-testops-project=PRJCODE \ # project, where your testrun exists in
+    --qase-testops-plan-id=3 # testplan id
+```
```

### Comparing `qase-pytest-5.0.6/pyproject.toml` & `qase_pytest-6.0.0b1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,52 @@
 [build-system]
 requires = ["setuptools>=68", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-pytest"
-version = "5.0.6"
+version = "6.0.0b1"
 description = "Qase Pytest Plugin for Qase TestOps and Qase Report"
 readme = "README.md"
+keywords = ["qase", "pytest", "plugin", "testops", "report", "qase reporting", "test observability"]
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
-    "Framework :: Pytest",
     "Programming Language :: Python",
+    "Framework :: Pytest",
+    'Intended Audience :: Developers',
+    'License :: OSI Approved :: Apache Software License',
+    'Topic :: Software Development :: Quality Assurance',
+    'Topic :: Software Development :: Testing',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3 :: Only',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
 ]
-urls = {"Homepage" = "https://github.com/qase-tms/qase-python/tree/master/qase-pytest"}
 requires-python = ">=3.7"
 dependencies = [
-    "qase-python-commons>=2.0.11,<2.1.0",
+    "qase-python-commons~=3.0.2b1",
     "pytest>=7.4.4",
     "filelock~=3.12.2",
     "more_itertools",
 ]
 
+[project.urls]
+Homepage = "https://qase.io"
+Repository = "https://github.com/qase-tms/qase-python/tree/master/qase-pytest"
+Documentation = "https://developers.qase.io"
+
+[project.entry-points.pytest11]
+qase_pytest = "qase.pytest.conftest"
+
 [project.optional-dependencies]
 testing = [
     "pytest",
     "pytest-cov",
 ]
 
 [tool.tox]
@@ -41,17 +61,18 @@
     pytest-cov
 passenv =
     HOME
 commands =
     pytest --cov-config=pyproject.toml {posargs}
 extras =
     all
-    testing
+    testing 
 """
 
+
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.pytest.ini_options]
 addopts = "--cov-report=term-missing --verbose"
 norecursedirs = ["dist", "build", ".tox"]
 testpaths = ["tests"]
@@ -59,15 +80,15 @@
 [tool.flake8]
 exclude = [".tox", "build", "dist", ".eggs"]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.paths]
-source = ["src/qaseio/pytest"]
+source = ["src/qase/pytest"]
 
 [tool.coverage.report]
 # Regexes for lines to exclude from consideration
 exclude_also = [
     # Don't complain about missing debug-only code:
     "def __repr__",
     "if self\\.debug",
@@ -80,8 +101,8 @@
     "if 0:",
     "if __name__ == .__main__.:",
 
     # Don't complain about abstract methods, they aren't run:
     "@(abc\\.)?abstractmethod",
     ]
 
-ignore_errors = false
+ignore_errors = false
```

### Comparing `qase-pytest-5.0.6/src/qase_pytest.egg-info/PKG-INFO` & `qase_pytest-6.0.0b1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,252 +1,267 @@
 Metadata-Version: 2.1
 Name: qase-pytest
-Version: 5.0.6
+Version: 6.0.0b1
 Summary: Qase Pytest Plugin for Qase TestOps and Qase Report
-Home-page: https://github.com/qase-tms/qase-python/tree/master/qase-pytest
-Author: Qase Team
-Author-email: support@qase.io
-License: apache
-Platform: any
+Author-email: Qase Team <support@qase.io>
+Project-URL: Homepage, https://qase.io
+Project-URL: Repository, https://github.com/qase-tms/qase-python/tree/master/qase-pytest
+Project-URL: Documentation, https://developers.qase.io
+Keywords: qase,pytest,plugin,testops,report,qase reporting,test observability
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Provides-Extra: testing
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-License-File: AUTHORS.rst
+Requires-Dist: qase-python-commons~=3.0.2b1
+Requires-Dist: pytest>=7.4.4
+Requires-Dist: filelock~=3.12.2
+Requires-Dist: more_itertools
+Provides-Extra: testing
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
 
-# [Qase](https://qase.io) Pytest Plugin
+# [Qase TestOps](https://qase.io) Pytest Reporter
 
 [![License](https://lxgaming.github.io/badges/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
 ## Installation
 
-```
+```sh
 pip install qase-pytest
 ```
 
-## Upgrade from 4.x to 5.x
-A new version of qase-pytest reporter has breaking changes. Follow these [guide](UPGRADE.md) that will help you to migrate to a new version.
+## Upgrade from 4.x to 5.x and to 6.x
+
+The new version 6.x of the Pytest reporter has breaking changes.
+To migrate from versions 4.x or 5.x, follow the [upgrade guide](UPGRADE.md).
 
 ## Configuration
 
-Qase Pytest Plugin can be configured in multiple ways:
- - using a config file `qase.config.json`
- - using environment variables
- - using CLI options
+Qase Pytest Reporter is configured in multiple ways:
+
+- using a config file `qase.config.json`
+- using environment variables
+- using command line options
 
-All configuration options are listed in the following doc: [Configuration](../README.md#configuration).
+Environment variables override the values given in the config file, 
+and command line options override both other values.
+
+Configuration options are described in the
+[configuration reference](docs/CONFIGURATION.md).
 
 
 ### Example: qase.config.json
 
-```
+```json
 {
-	"mode": "testops", 
-	"fallback": "report",
-	"report": {
-		"driver": "local",
-		"connection": {
-			"local": {
-				"path": "./build/qase-report",
-				"format": "json" 
-			}
-		}
-	},
-	"testops": {
-		"bulk": true,
-		"api": {
-			"token": "YOUR_API_TOKEN",
-			"host": "qase.io"
-		},
-		"run": {
-            "id": 1,
-			"title": "Test run title",
-			"complete": true
-		},
-        "plan": {
-            "id": 1
-        },
-		"defect": true,
-		"project": "YOUR_PROJECT_CODE",
-		"chunk": 200
-	},
-	"framework": {
-		"pytest": {
-			"capture": {
-				"logs": true,
-				"http": true
-			}
-		}
-	},
-	"environment": "local"
+  "mode": "testops", 
+  "fallback": "report",
+  "testops": {
+    "project": "YOUR_PROJECT_CODE",
+    "api": {
+      "token": "YOUR_API_TOKEN",
+      "host": "qase.io"
+    },
+    "run": {
+      "title": "Test run title"
+    },
+    "batch": {
+      "size": 100
+    }
+  },
+    "report": {
+    "driver": "local",
+    "connection": {
+      "local": {
+        "path": "./build/qase-report",
+        "format": "json" 
+      }
+    }
+  },
+  "framework": {
+    "pytest": {
+      "capture": {
+        "logs": true,
+        "http": true
+      }
+    }
+  },
+  "environment": "local"
 }
 ```
 
 ## Usage
 
 ### Link tests with test cases in Qase TestOps
 
-To link tests in code with tests in Qase TestOps you can use predefined decorators:
+To link the automated tests with the test cases in Qase TestOps, use the `@qase.id()` decorator.
+Other test data, such as case title, system and custom fields,
+can be added with `@qase.title()` and `@qase.fields()`:
 
 ```python
-from qaseio.pytest import qase
+from qase.pytest import qase
 
 @qase.id(13)
 @qase.title("My first test")
 @qase.fields(
     ("severity", "critical"),
-    ("priority", "hight"),
+    ("priority", "high"),
     ("layer", "unit"),
-    ("description", "Try to login in Qase TestOps using login and password"),
-    ("description", "*Precondition 1*. Markdown is supported."),
+    ("description", "Try to login to Qase TestOps using login and password"),
+    ("preconditions", "*Precondition 1*. Markdown is supported."),
 )
 def test_example_1():
     pass
 ```
 
 Each unique number can only be assigned once to the class or function being used.
 
 ### Ignore a particular test
-If you want to exclude a particular test from the report, you can use the `@qase.ignore` decorator:
+
+To exclude a particular test from the report, use the `@qase.ignore` decorator:
 
 ```python
-from qaseio.pytest import qase
+from qase.pytest import qase
 
 @qase.ignore
 def test_example_1():
     pass
 ```
 
 ### Possible test result statuses
 
 - PASSED - when test passed
-- FAILED - when test failed with AssertionError
+- FAILED - when test failed with `AssertionError`
 - BLOCKED - when test failed with any other exception
 - SKIPPED - when test has been skipped
 
 ### Capture network logs
-In order to capture network logs, you need to enable the `http` option in the `capture` section of the `framework` section in the config file.
 
-Qase Pytest reporter will capture all requests and responses and save as a test step automatically.
+To capture the network logs, enable the `http` option in the `framework.capture` section
+of the configuration file.
+
+The Qase Pytest reporter will capture all HTTP requests and responses
+and save them as a test steps automatically.
 
 ### Add attachments to test results
 
-When you need to push some additional information to server you could use
-attachments:
+To upload screenshots, logs, and other information to Qase.io,
+use `qase.attach()`.
+It works both with files in the filesystem and with data available in the code.
+There is no limit on the amount of attachments from a single test.
 
 ```python
 import pytest
-from qaseio.pytest import qase
+from qase.pytest import qase
 
-@pytest.fixture(scope="session")
-def driver():
-    driver = webdriver.Chrome()
-    yield driver
-    logs = "\n".join(str(row) for row in driver.get_log('browser')).encode('utf-8')
-    qase.attach((logs, "text/plain", "browser.log"))
-    driver.quit()
-
-@qase.title("My first test")
+@qase.title("File attachments")
 def test_example_1():
+    # attach files from the filesystem:
     qase.attach("/path/to/file", "/path/to/file/2")
+    # to add multiple attachments, pass them in tuples:
     qase.attach(
         ("/path/to/file/1", "application/json"),
         ("/path/to/file/3", "application/xml"),
     )
 
-@qase.id(12)
-def test_example_2(driver):
-    qase.attach((driver.get_screenshot_as_png(), "image/png", "result.png"))
-```
-
-You could pass as much files as you need.
-
-Also you should know, that if no case id is associated with current test in
-pytest - attachment would not be uploaded:
-
-```python
-import pytest
-from qaseio.pytest import qase
-
 @pytest.fixture(scope="session")
 def driver():
     driver = webdriver.Chrome()
     yield driver
     logs = "\n".join(str(row) for row in driver.get_log('browser')).encode('utf-8')
-    # This would do nothing, because last test does not have case id link
+    # attach logs from a code variable as a text file:
     qase.attach((logs, "text/plain", "browser.log"))
     driver.quit()
 
+@qase.id(12)
 def test_example_2(driver):
-    # This would do nothing
+    # attach the output of driver.get_screenshot_as_png() as a png image
     qase.attach((driver.get_screenshot_as_png(), "image/png", "result.png"))
 ```
 
 ### Linking code with steps
 
-It is possible to link test step with function, or using context.
+To mark a test step, either annotate a function with `@qase.step()`,
+or use the `with qase.step()` context:
 
 ```python
-from qaseio.pytest import qase
+from qase.pytest import qase
 
 @qase.step("First step") # test step name
 def some_step():
     sleep(5)
 
 @qase.step("Second step")  # test step name
 def another_step():
     sleep(3)
 
-...
+# ...
 
 def test_example():
     some_step()
     another_step()
     # test step hash
     with qase.step("Third step"):
         sleep(1)
 ```
 
-### Sending tests to existing testrun
+### Creating new testrun according to current pytest run
 
-Testrun in TestOps will contain only those test results, which are presented in testrun,
-but every test would be executed.
+By default, qase-pytest will create a new test run in Qase TestOps
+and report results to this test run.
+To provide a custom name for this run, add
+the option `--qase-testops-run-title`.
 
 ```bash
 pytest \
     --qase-mode=testops \
     --qase-testops-api-token=<your api token here> \
-    --qase-testops-project=PRJCODE \ # project, where your testrun exists in
-    --qase-testops-run-id=3 # testrun id
+    --qase-testops-project=PRJCODE \ # project, where your testrun would be created
+    --qase-testops-run-title=My\ First\ Automated\ Run
 ```
 
-### Creating test run base on test plan (selective launch)
+### Sending tests to existing testrun
 
-Create new testrun base on testplan. Testrun in Qase TestOps will contain only those
-test results. `qase-pytest` supports selective execution
+Test results can be reported to an existing test run in Qase using its ID.
+This is useful when a test run combines tests from multiple sources:
+
+* manual and automated
+* autotests from different frameworks
+* tests running in multiple shards on different machines
+
+For example, if the test run has ID=3, the following command will
+run tests and report results to this test run:
 
 ```bash
 pytest \
     --qase-mode=testops \
     --qase-testops-api-token=<your api token here> \
-    --qase-testops-project=PRJCODE \ # project, where your testrun exists in
-    --qase-testops-plan-id=3 # testplan id
+    --qase-testops-project=PRJCODE \ # project, where the test run is created
+    --qase-testops-run-id=3 # testrun id
 ```
 
-### Creating new testrun according to current pytest run
+### Creating test run based on test plan (selective launch)
 
-If you want to create a new test run in Qase TestOps for each execution, you can simply 
-skip `--qase-testops-run` option. If you want to provide a custom name for this run, you can add an
-option `--qase-testops-run-title` 
+Create a new testrun base on a testplan. Testrun in Qase TestOps will contain only those
+test results. `qase-pytest` supports selective execution.
 
 ```bash
 pytest \
     --qase-mode=testops \
     --qase-testops-api-token=<your api token here> \
-    --qase-testops-project=PRJCODE \ # project, where your testrun would be created
-    --qase-testops-run-title=My\ First\ Automated\ Run
+    --qase-testops-project=PRJCODE \ # project, where your testrun exists in
+    --qase-testops-plan-id=3 # testplan id
 ```
-
-
```

### Comparing `qase-pytest-5.0.6/src/qaseio/pytest/plugin.py` & `qase_pytest-6.0.0b1/src/qase/pytest/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,60 @@
 import pathlib
 from typing import Tuple, Union
-import pytest
 import mimetypes
 import re
 
-from qaseio.commons.models.result import Result, Field
-from qaseio.commons.models.attachment import Attachment
-from qaseio.commons.utils import QaseUtils
-from qaseio.commons.models.runtime import Runtime
+from qase.commons.models.result import Result, Field
+from qase.commons.models.attachment import Attachment
+from qase.commons.models.suite import Suite
+from qase.commons.models.runtime import Runtime
+
+from qase.commons import QaseUtils
 
 from filelock import FileLock
+from itertools import chain, islice
 
 PYTEST_TO_QASE_STATUS = {
     "PASSED": 'passed',
     "FAILED": 'failed',
     "SKIPPED": 'skipped',
     "BLOCKED": 'blocked',
     "BROKEN": 'invalid'
 }
 
 try:
     from xdist import is_xdist_controller
 except ImportError:
     def is_xdist_controller(*args, **kwargs):
         return True
-    
+
 try:
     import pytest
 except ImportError:
     raise ImportError("pytest is not installed")
 
+
 class PluginNotInitializedException(Exception):
     pass
 
+
 class QasePytestPlugin:
     run = None
     meta_run_file = pathlib.Path("src.run")
 
     def __init__(
             self,
-            reporter,
-            fallback,
-            xdist_enabled = False,
-            capture_logs = False,
-            execution_plan = None,
-            intercept_requests = False,
+            reporter
     ):
         self.runtime = Runtime()
         self.reporter = reporter
         self.run_id = None
-        self.xdist_enabled = xdist_enabled
-        self.fallback = fallback
-        self.capture_logs = capture_logs
-        self.debug = True
-        self.execution_plan = execution_plan
-        self.intercept_requests = intercept_requests
-        self.interceptor = None
-        if self.intercept_requests:
-            # Lazy import
-            from qaseio.commons.interceptor import InterceptorSingleton
-            InterceptorSingleton.init(runtime=self.runtime)
-            self.interceptor = InterceptorSingleton.get_instance()
+        self.execution_plan = None
+
+        self.reporter.setup_profilers(runtime=self.runtime)
 
     def start_step(self, step):
         self.runtime.add_step(step)
 
     def finish_step(self, id, exception=None):
         status = PYTEST_TO_QASE_STATUS['PASSED']
         if exception:
@@ -75,99 +65,106 @@
     @staticmethod
     def drop_run_id():
         if QasePytestPlugin.meta_run_file.exists():
             QasePytestPlugin.meta_run_file.unlink()
 
     def pytest_collection_modifyitems(self, session, config, items):
         # Filter test cases based on ids
-        if (self.execution_plan):
-            items[:] = [item for item in items if item.get_closest_marker('qase_id') and item.get_closest_marker('qase_id').kwargs.get("id") in self.execution_plan]
+        if self.execution_plan:
+            items[:] = [item for item in items if
+                        item.get_closest_marker('qase_id') and item.get_closest_marker('qase_id').kwargs.get(
+                            "id") in self.execution_plan]
 
     def pytest_sessionstart(self, session):
-        if (not self.xdist_enabled) or (self.xdist_enabled and is_xdist_controller(session)):
+        if is_xdist_controller(session):
             self.run_id = self.reporter.start_run()
-            with FileLock("qaseio.lock"):
+            with FileLock("qase.lock"):
                 if self.run_id:
                     with open(self.meta_run_file, "w") as lock_file:
                         lock_file.write(str(self.run_id))
         else:
             self.load_run_from_lock()
-        self.has_started = True
 
     def pytest_sessionfinish(self, session, exitstatus):
-        main = False
-        if (not self.xdist_enabled) or (self.xdist_enabled and is_xdist_controller(session)):
-            main = True
+        if is_xdist_controller(session):
             QasePytestPlugin.drop_run_id()
-        self.reporter.complete_run(main)
-        self.has_started = False
+        else:
+            self.reporter.complete_worker()
+
+        self.reporter.complete_run()
 
     @pytest.hookimpl(hookwrapper=True)
     def pytest_runtest_protocol(self, item):
         self.ignore = True if item.get_closest_marker("qase_ignore") else False
 
         if not self.ignore:
-            # Capture HTTP requests inside test
-            if self.interceptor:
-                self.interceptor.enable()
+            self.reporter.enable_profilers()
             self.start_pytest_item(item)
             yield
-            if self.interceptor:
-                self.interceptor.disable()
+            self.reporter.disable_profilers()
             self.finish_pytest_item(item)
         else:
             yield
 
     @pytest.hookimpl(hookwrapper=True)
     def pytest_runtest_makereport(self, item, call):
         if not self.ignore:
             report = (yield).get_result()
+
             def set_result(res):
                 self.runtime.result.execution.status = res
 
+            def _attach_logs():
+                # TODO: can be attached twice
+                if report.caplog:
+                    self.add_attachments((report.caplog, "text/plain", "log.txt"))
+                if report.capstdout:
+                    self.add_attachments((report.capstdout, "text/plain", "stdout.txt"))
+                if report.capstderr:
+                    self.add_attachments((report.capstderr, "text/plain", "stderr.txt"))
+
             if report.longrepr:
                 self.runtime.result.execution.stacktrace = report.longreprtext
 
             if report.failed:
                 if call.excinfo.typename != "AssertionError":
                     set_result(PYTEST_TO_QASE_STATUS['BROKEN'])
                 else:
                     set_result(PYTEST_TO_QASE_STATUS['FAILED'])
                 self.runtime.result.add_message(call.excinfo.exconly())
+                if self.reporter.config.get("capture.logs", "failed") == "failed" and report.when == "call":
+                    _attach_logs()
             elif report.skipped:
                 if self.runtime.result.execution.status in (
                         None,
                         PYTEST_TO_QASE_STATUS['PASSED'],
                 ):
                     set_result(PYTEST_TO_QASE_STATUS['SKIPPED'])
             else:
                 if self.runtime.result.execution.status is None:
                     set_result(PYTEST_TO_QASE_STATUS['PASSED'])
 
-            if self.capture_logs and report.when == "call":
-                if report.caplog:
-                    self.add_attachments((report.caplog, "text/plain", "log.txt"))
-                if report.capstdout:
-                    self.add_attachments((report.capstdout, "text/plain", "stdout.txt"))
-                if report.capstderr:
-                    self.add_attachments((report.capstderr, "text/plain", "stderr.txt"))
+            if self.reporter.config.get("capture.logs", "failed") == "always" and report.when == "call":
+                _attach_logs()
         else:
             yield
 
     def start_pytest_item(self, item):
         self.runtime.result = Result(
-            title = self._get_title(item), 
-            signature = self._get_signature(item),
-            )
+            title=self._get_title(item),
+            signature=self._get_signature(item),
+        )
         self._set_fields(item)
         self._set_tags(item)
         self._set_author(item)
         self._set_muted(item)
         self._set_testops_id(item)
         self._set_params(item)
+        self._set_suite(item)
+        self._set_relations(item)
 
     def finish_pytest_item(self, item):
         self.runtime.result.execution.complete()
         self.runtime.result.add_steps([step for key, step in self.runtime.steps.items()])
         self.reporter.add_result(self.runtime.result)
 
         self.runtime = Runtime()
@@ -198,34 +195,36 @@
         if QasePytestPlugin.meta_run_file.exists():
             with open(QasePytestPlugin.meta_run_file, "r") as lock_file:
                 try:
                     self.run_id = str(lock_file.read())
                     self.reporter.set_run_id(self.run_id)
                 except ValueError:
                     pass
-    
+        else:
+            self.run_id = self.reporter.start_run()
+
     def _get_title(self, item):
         title = None
         try:
             title = item.get_closest_marker("qase_title").kwargs.get("title")
         except:
             pass
 
         if not title:
             title = item.originalname
 
         return str(title)
-    
+
     def _get_signature(self, item) -> str:
         return re.sub(r'\[.*?\]', '', item.nodeid)
-    
+
     def _set_relations(self, item) -> None:
         # TODO: Add support for relations
         pass
-    
+
     def _set_fields(self, item) -> None:
         # Legacy fields support
         for name in ["description", "preconditions", "postconditions", "layer", "severity", "priority"]:
             try:
                 self.runtime.result.add_field(Field(name, item.get_closest_marker("qase_" + name).kwargs.get(name)))
             except:
                 pass
@@ -264,14 +263,36 @@
             pass
 
     def _set_params(self, item) -> None:
         if hasattr(item, 'callspec'):
             for key, val in item.callspec.params.items():
                 self.runtime.result.add_param(key, str(val))
 
+    def _set_suite(self, item) -> None:
+        marker = item.get_closest_marker("qase_suite")
+        if marker:
+            self.runtime.result.suite = Suite(marker.kwargs.get("title"), marker.kwargs.get("description"))
+        self._get_suite(item)
+
+    def _get_suite(self, item):
+        path, class_name, tail = islice(chain(item.nodeid.split('::'), [None], [None]), 3)
+
+        class_name = class_name if tail else None
+        file_name, file_path = islice(chain(reversed(path.rsplit('/', 1)), [None]), 2)
+
+        module = file_name.split('.')[0]
+        package = path.replace('/', '.') if path else None
+
+        title = file_path + '.' + module
+        if class_name:
+            title += '.' + class_name
+
+        self.runtime.result.suite = Suite(title, package)
+
+
 class QasePytestPluginSingleton:
     _instance = None
 
     @staticmethod
     def init(**kwargs):
         if QasePytestPluginSingleton._instance is None:
             QasePytestPluginSingleton._instance = QasePytestPlugin(**kwargs)
```

