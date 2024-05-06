# Comparing `tmp/qase-robotframework-2.0.1.tar.gz` & `tmp/qase_robotframework-3.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase-robotframework-2.0.1.tar", last modified: Wed Mar 13 08:51:00 2024, max compression
+gzip compressed data, was "qase_robotframework-3.0.0b1.tar", last modified: Mon May  6 09:41:56 2024, max compression
```

## Comparing `qase-robotframework-2.0.1.tar` & `qase_robotframework-3.0.0b1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 08:51:00.810555 qase-robotframework-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-13 08:50:51.000000 qase-robotframework-2.0.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-03-13 08:50:51.000000 qase-robotframework-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16907 2024-03-13 08:51:00.810555 qase-robotframework-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-03-13 08:50:51.000000 qase-robotframework-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-13 08:50:51.000000 qase-robotframework-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 08:51:00.810555 qase-robotframework-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 08:51:00.810555 qase-robotframework-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 08:51:00.810555 qase-robotframework-2.0.1/src/qase_robotframework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16907 2024-03-13 08:51:00.000000 qase-robotframework-2.0.1/src/qase_robotframework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-13 08:51:00.000000 qase-robotframework-2.0.1/src/qase_robotframework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 08:51:00.000000 qase-robotframework-2.0.1/src/qase_robotframework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-13 08:51:00.000000 qase-robotframework-2.0.1/src/qase_robotframework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-13 08:51:00.000000 qase-robotframework-2.0.1/src/qase_robotframework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 08:51:00.810555 qase-robotframework-2.0.1/src/qaseio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 08:51:00.810555 qase-robotframework-2.0.1/src/qaseio/robotframework/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-13 08:50:51.000000 qase-robotframework-2.0.1/src/qaseio/robotframework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-03-13 08:50:51.000000 qase-robotframework-2.0.1/src/qaseio/robotframework/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-03-13 08:50:51.000000 qase-robotframework-2.0.1/src/qaseio/robotframework/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-13 08:50:51.000000 qase-robotframework-2.0.1/src/qaseio/robotframework/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:41:56.231186 qase_robotframework-3.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-06 09:41:48.000000 qase_robotframework-3.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16305 2024-05-06 09:41:56.231186 qase_robotframework-3.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-06 09:41:48.000000 qase_robotframework-3.0.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-06 09:41:48.000000 qase_robotframework-3.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 09:41:56.231186 qase_robotframework-3.0.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:41:56.227186 qase_robotframework-3.0.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:41:56.231186 qase_robotframework-3.0.0b1/src/qase_robotframework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16305 2024-05-06 09:41:56.000000 qase_robotframework-3.0.0b1/src/qase_robotframework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-06 09:41:56.000000 qase_robotframework-3.0.0b1/src/qase_robotframework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 09:41:56.000000 qase_robotframework-3.0.0b1/src/qase_robotframework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-06 09:41:56.000000 qase_robotframework-3.0.0b1/src/qase_robotframework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 09:41:56.000000 qase_robotframework-3.0.0b1/src/qase_robotframework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:41:56.227186 qase_robotframework-3.0.0b1/src/qaseio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 09:41:56.231186 qase_robotframework-3.0.0b1/src/qaseio/robotframework/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-06 09:41:48.000000 qase_robotframework-3.0.0b1/src/qaseio/robotframework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-06 09:41:48.000000 qase_robotframework-3.0.0b1/src/qaseio/robotframework/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-06 09:41:48.000000 qase_robotframework-3.0.0b1/src/qaseio/robotframework/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-06 09:41:48.000000 qase_robotframework-3.0.0b1/src/qaseio/robotframework/types.py
```

### Comparing `qase-robotframework-2.0.1/LICENSE` & `qase_robotframework-3.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `qase-robotframework-2.0.1/PKG-INFO` & `qase_robotframework-3.0.0b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-robotframework
-Version: 2.0.1
+Version: 3.0.0b1
 Summary: Qase Robot Framework Plugin
 Author-email: Qase Team <support@qase.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -205,37 +205,89 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-robotframework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Robot Framework
 Classifier: Programming Language :: Python
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS.rst
-Requires-Dist: qase-python-commons<2.0.0,>=1.0.4
+Requires-Dist: qase-python-commons~=3.0.2b1
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
-> # Qase Robot Framework Listener
->
-> Publish results simple and easy.
+# [Qase TestOps](https://qase.io) Robot Framework Reporter
 
-## How to integrate
+[![License](https://lxgaming.github.io/badges/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
+## Installation
+
+```sh
+pip install qase-robotframework==3.0.0b1
 ```
-pip install qase-robotframework
+
+## Upgrade from 2.x to 3.x
+
+The new version 3.x of the Robot Framework reporter has breaking changes.
+To migrate from versions 2.x, follow the [upgrade guide](docs/UPGRADE.md).
+
+## Configuration
+
+Qase Robot Framework Reporter is configured in multiple ways:
+
+- using a config file `qase.config.json`
+- using environment variables
+
+Environment variables override the values given in the config file.
+
+Configuration options are described in the
+[configuration reference](docs/CONFIGURATION.md).
+
+### Example: qase.config.json
+
+```json
+{
+  "mode": "testops", 
+  "fallback": "report",
+  "debug": true,
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
+  "environment": "local"
+}
 ```
 
+
 ## Usage
 
-If you want to create a persistent link to Test Cases in Qase, you should add Qase test case IDs to robot framework tests.
-They should be added as a tags in form like `Q-<case id without project code>`. You can use upper and lower case to indicate the test case IDs. Example:
+### Link tests with test cases in Qase TestOps
+
+To link the automated tests with the test cases in Qase TestOps, use the tags in form like `Q-<case id without project code>`.
+Example:
 
 ```robotframework
 *** Test Cases ***
 Push button
     [Tags]  q-2
     Push button    1
     Result should be    1
@@ -270,63 +322,11 @@
     Should Be Equal As Strings    1  ${response.json()}[id]                 ## 2-nd step - "Should Be Equal As Strings"
 
 Initializing the test case                                                  ## Test case: "Initializing the test case"
     [Tags]  q-4
     Set To Dictionary    ${info}   field1=A sample string                   ## 1-st step - "Set To Dictionary"
 ```
 
-## Configuration
-
-Listener supports loading configuration both from environment variables and from `tox.ini` file.
-
-ENV variables:
-- `QASE_MODE` - Define mode: `testops` to enable report
-- `QASE_ENVIRONMENT` - Environment ID for the run
-- `QASE_DEBUG` - If passed something - will enable debug logging for listener. Default: `False`
-- `QASE_TESTOPS_MODE` - You can switch between `sync` and `async` modes. Default is `async`
-- `QASE_TESTOPS_API_TOKEN` - API token to access Qase TestOps
-- `QASE_TESTOPS_PROJECT` - Project code from Qase TestOps
-- `QASE_TESTOPS_PLAN_ID` - Plan ID if you want to add results to existing run from Test Plan
-- `QASE_TESTOPS_RUN_ID` - Run ID if you want to add results to existing run
-- `QASE_TESTOPS_RUN_TITLE` - Set custom run name when no run ID is provided
-- `QASE_TESTOPS_COMPLETE_RUN` - Will complete run after all tests are finished. Default: `False`
-- `QASE_TESTOPS_HOST` - Define a host for Qase TestOps. Default: `qase.io`
-### Usage:
-```
-QASE_API_TOKEN=<API TOKEN> QASE_PROJECT=PRJCODE robot --listener qaseio.robotframework.Listener keyword_driven.robot data_driven.robot
-```
-Moving variables to `tox.ini`, example configuration:
-```ini
-[qase]
-qase_testops_api_token=api_key
-qase_testops_project=project_code
-qase_testops_run_id=run_id
-qase_testops_run_title=New Robot Framework Run
-qase_debug=True
-qase_testops_complete_run=True
-```
-Execution:
+### Execution:
 ```
-robot --listener qaseio.robotframework.Listener someTest.robot
-```
-## Contribution
-
-Install project locally:
-
-```bash
-python3 -m venv .venv
-source .venv/bin/activate
-pip install -e .[testing]
-```
-
-Install dev requirements:
-
-```bash
-pip install pre-commit
-pre-commit install
-```
-
-Test project:
-
-```bash
-tox
+robot --listener qase.robotframework.Listener someTest.robot
 ```
```

### Comparing `qase-robotframework-2.0.1/pyproject.toml` & `qase_robotframework-3.0.0b1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 [build-system]
-requires = ["setuptools>=69", "wheel"]
+requires = ["setuptools>=68", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-robotframework"
-version = "2.0.1"
+version = "3.0.0b1"
 description = "Qase Robot Framework Plugin"
 readme = "README.md"
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Robot Framework",
     "Programming Language :: Python",
 ]
 urls = {"Homepage" = "https://github.com/qase-tms/qase-python/tree/master/qase-robotframework"}
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 dependencies = [
-    "qase-python-commons>=1.0.4,<2.0.0",
+    "qase-python-commons~=3.0.2b1",
 ]
 
 [project.optional-dependencies]
 testing = [
     "pytest",
     "pytest-cov",
 ]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-minversion = 3.8
-envlist = py{38,39,310,311}
+minversion = 3.7
+envlist = py{37,38,39,310,311}
 
 [testenv]
 deps =
     pytest
     pytest-cov
 passenv =
     HOME
@@ -57,15 +57,15 @@
 [tool.flake8]
 exclude = [".tox", "build", "dist", ".eggs"]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.paths]
-source = ["src/qaseio/robotframework"]
+source = ["src/qase/robotframework"]
 
 [tool.coverage.report]
 # Regexes for lines to exclude from consideration
 exclude_also = [
     # Don't complain about missing debug-only code:
     "def __repr__",
     "if self\\.debug",
@@ -78,8 +78,8 @@
     "if 0:",
     "if __name__ == .__main__.:",
 
     # Don't complain about abstract methods, they aren't run:
     "@(abc\\.)?abstractmethod",
     ]
 
-ignore_errors = false
+ignore_errors = false
```

### Comparing `qase-robotframework-2.0.1/src/qase_robotframework.egg-info/PKG-INFO` & `qase_robotframework-3.0.0b1/src/qase_robotframework.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-robotframework
-Version: 2.0.1
+Version: 3.0.0b1
 Summary: Qase Robot Framework Plugin
 Author-email: Qase Team <support@qase.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -205,37 +205,89 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-robotframework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Robot Framework
 Classifier: Programming Language :: Python
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS.rst
-Requires-Dist: qase-python-commons<2.0.0,>=1.0.4
+Requires-Dist: qase-python-commons~=3.0.2b1
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
-> # Qase Robot Framework Listener
->
-> Publish results simple and easy.
+# [Qase TestOps](https://qase.io) Robot Framework Reporter
 
-## How to integrate
+[![License](https://lxgaming.github.io/badges/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
+## Installation
+
+```sh
+pip install qase-robotframework==3.0.0b1
 ```
-pip install qase-robotframework
+
+## Upgrade from 2.x to 3.x
+
+The new version 3.x of the Robot Framework reporter has breaking changes.
+To migrate from versions 2.x, follow the [upgrade guide](docs/UPGRADE.md).
+
+## Configuration
+
+Qase Robot Framework Reporter is configured in multiple ways:
+
+- using a config file `qase.config.json`
+- using environment variables
+
+Environment variables override the values given in the config file.
+
+Configuration options are described in the
+[configuration reference](docs/CONFIGURATION.md).
+
+### Example: qase.config.json
+
+```json
+{
+  "mode": "testops", 
+  "fallback": "report",
+  "debug": true,
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
+  "environment": "local"
+}
 ```
 
+
 ## Usage
 
-If you want to create a persistent link to Test Cases in Qase, you should add Qase test case IDs to robot framework tests.
-They should be added as a tags in form like `Q-<case id without project code>`. You can use upper and lower case to indicate the test case IDs. Example:
+### Link tests with test cases in Qase TestOps
+
+To link the automated tests with the test cases in Qase TestOps, use the tags in form like `Q-<case id without project code>`.
+Example:
 
 ```robotframework
 *** Test Cases ***
 Push button
     [Tags]  q-2
     Push button    1
     Result should be    1
@@ -270,63 +322,11 @@
     Should Be Equal As Strings    1  ${response.json()}[id]                 ## 2-nd step - "Should Be Equal As Strings"
 
 Initializing the test case                                                  ## Test case: "Initializing the test case"
     [Tags]  q-4
     Set To Dictionary    ${info}   field1=A sample string                   ## 1-st step - "Set To Dictionary"
 ```
 
-## Configuration
-
-Listener supports loading configuration both from environment variables and from `tox.ini` file.
-
-ENV variables:
-- `QASE_MODE` - Define mode: `testops` to enable report
-- `QASE_ENVIRONMENT` - Environment ID for the run
-- `QASE_DEBUG` - If passed something - will enable debug logging for listener. Default: `False`
-- `QASE_TESTOPS_MODE` - You can switch between `sync` and `async` modes. Default is `async`
-- `QASE_TESTOPS_API_TOKEN` - API token to access Qase TestOps
-- `QASE_TESTOPS_PROJECT` - Project code from Qase TestOps
-- `QASE_TESTOPS_PLAN_ID` - Plan ID if you want to add results to existing run from Test Plan
-- `QASE_TESTOPS_RUN_ID` - Run ID if you want to add results to existing run
-- `QASE_TESTOPS_RUN_TITLE` - Set custom run name when no run ID is provided
-- `QASE_TESTOPS_COMPLETE_RUN` - Will complete run after all tests are finished. Default: `False`
-- `QASE_TESTOPS_HOST` - Define a host for Qase TestOps. Default: `qase.io`
-### Usage:
-```
-QASE_API_TOKEN=<API TOKEN> QASE_PROJECT=PRJCODE robot --listener qaseio.robotframework.Listener keyword_driven.robot data_driven.robot
-```
-Moving variables to `tox.ini`, example configuration:
-```ini
-[qase]
-qase_testops_api_token=api_key
-qase_testops_project=project_code
-qase_testops_run_id=run_id
-qase_testops_run_title=New Robot Framework Run
-qase_debug=True
-qase_testops_complete_run=True
-```
-Execution:
+### Execution:
 ```
-robot --listener qaseio.robotframework.Listener someTest.robot
-```
-## Contribution
-
-Install project locally:
-
-```bash
-python3 -m venv .venv
-source .venv/bin/activate
-pip install -e .[testing]
-```
-
-Install dev requirements:
-
-```bash
-pip install pre-commit
-pre-commit install
-```
-
-Test project:
-
-```bash
-tox
+robot --listener qase.robotframework.Listener someTest.robot
 ```
```

### Comparing `qase-robotframework-2.0.1/src/qaseio/robotframework/models.py` & `qase_robotframework-3.0.0b1/src/qaseio/robotframework/models.py`

 * *Files identical despite different names*

