# Comparing `tmp/pytest-exit-code-0.1.0.tar.gz` & `tmp/pytest_exit_code-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-exit-code-0.1.0.tar", last modified: Fri Feb 23 09:19:08 2024, max compression
+gzip compressed data, was "pytest_exit_code-0.2.0.tar", last modified: Mon May  6 08:31:56 2024, max compression
```

## Comparing `pytest-exit-code-0.1.0.tar` & `pytest_exit_code-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:19:08.795181 pytest-exit-code-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-23 09:19:00.000000 pytest-exit-code-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15930 2024-02-23 09:19:08.795181 pytest-exit-code-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-02-23 09:19:00.000000 pytest-exit-code-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-02-23 09:19:00.000000 pytest-exit-code-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 09:19:08.795181 pytest-exit-code-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:19:08.791181 pytest-exit-code-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:19:08.791181 pytest-exit-code-0.1.0/src/pytest_exit_code/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-23 09:19:00.000000 pytest-exit-code-0.1.0/src/pytest_exit_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-02-23 09:19:00.000000 pytest-exit-code-0.1.0/src/pytest_exit_code/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:19:08.795181 pytest-exit-code-0.1.0/src/pytest_exit_code.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15930 2024-02-23 09:19:08.000000 pytest-exit-code-0.1.0/src/pytest_exit_code.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-02-23 09:19:08.000000 pytest-exit-code-0.1.0/src/pytest_exit_code.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 09:19:08.000000 pytest-exit-code-0.1.0/src/pytest_exit_code.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-23 09:19:08.000000 pytest-exit-code-0.1.0/src/pytest_exit_code.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-23 09:19:08.000000 pytest-exit-code-0.1.0/src/pytest_exit_code.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-23 09:19:08.000000 pytest-exit-code-0.1.0/src/pytest_exit_code.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:19:08.795181 pytest-exit-code-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-02-23 09:19:00.000000 pytest-exit-code-0.1.0/tests/test_exit_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:31:56.990366 pytest_exit_code-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-06 08:31:52.000000 pytest_exit_code-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16016 2024-05-06 08:31:56.990366 pytest_exit_code-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-06 08:31:52.000000 pytest_exit_code-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-06 08:31:52.000000 pytest_exit_code-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:31:56.990366 pytest_exit_code-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:31:56.986366 pytest_exit_code-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:31:56.986366 pytest_exit_code-0.2.0/src/pytest_exit_code/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-06 08:31:52.000000 pytest_exit_code-0.2.0/src/pytest_exit_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-06 08:31:52.000000 pytest_exit_code-0.2.0/src/pytest_exit_code/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:31:56.986366 pytest_exit_code-0.2.0/src/pytest_exit_code.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16016 2024-05-06 08:31:56.000000 pytest_exit_code-0.2.0/src/pytest_exit_code.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-06 08:31:56.000000 pytest_exit_code-0.2.0/src/pytest_exit_code.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:31:56.000000 pytest_exit_code-0.2.0/src/pytest_exit_code.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 08:31:56.000000 pytest_exit_code-0.2.0/src/pytest_exit_code.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-06 08:31:56.000000 pytest_exit_code-0.2.0/src/pytest_exit_code.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 08:31:56.000000 pytest_exit_code-0.2.0/src/pytest_exit_code.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:31:56.986366 pytest_exit_code-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-06 08:31:52.000000 pytest_exit_code-0.2.0/tests/test_exit_code.py
```

### Comparing `pytest-exit-code-0.1.0/LICENSE` & `pytest_exit_code-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-exit-code-0.1.0/PKG-INFO` & `pytest_exit_code-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-exit-code
-Version: 0.1.0
+Version: 0.2.0
 Summary: A pytest plugin that overrides the built-in exit codes to retain more information about the test results.
 Author-email: Sander Ploegsma <sanderploegsma@gmail.com>
 Maintainer-email: Sander Ploegsma <sanderploegsma@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -231,23 +231,25 @@
 # pytest-exit-code [![PyPi version][pypi-version-badge]][pypi-project] [![Python versions][pypi-pyversions-badge]][pypi-project]
 
 A [pytest] plugin that overrides the built-in exit codes to retain more information about the test results.
 
 ## Features
 
 This plugin changes the exit code returned by running `pytest`.
-The exit codes can range from `0` to `15` and are a combination of the following bitwise flags:
+The exit codes can range from `0` to `63` and are a combination of the following bitwise flags:
 
 | Flag | Description                     |
 | ---- | ------------------------------- |
 | `0`  | All tests passed.               |
 | `1`  | One or more tests passed.       |
 | `2`  | One or more tests failed.       |
 | `4`  | One or more tests errored.      |
 | `8`  | One or more tests were skipped. |
+| `16` | One or more tests xfailed.      |
+| `32` | One or more tests xpassed.      |
 
 So:
 
 - An exit code of `2` means that all tests failed.
 - An exit code of `6` means that all tests either failed or errored.
 - An exit code of `7` indicates that the result contains a mix of passed, failed and errored tests.
```

### Comparing `pytest-exit-code-0.1.0/README.md` & `pytest_exit_code-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # pytest-exit-code [![PyPi version][pypi-version-badge]][pypi-project] [![Python versions][pypi-pyversions-badge]][pypi-project]
 
 A [pytest] plugin that overrides the built-in exit codes to retain more information about the test results.
 
 ## Features
 
 This plugin changes the exit code returned by running `pytest`.
-The exit codes can range from `0` to `15` and are a combination of the following bitwise flags:
+The exit codes can range from `0` to `63` and are a combination of the following bitwise flags:
 
 | Flag | Description                     |
 | ---- | ------------------------------- |
 | `0`  | All tests passed.               |
 | `1`  | One or more tests passed.       |
 | `2`  | One or more tests failed.       |
 | `4`  | One or more tests errored.      |
 | `8`  | One or more tests were skipped. |
+| `16` | One or more tests xfailed.      |
+| `32` | One or more tests xpassed.      |
 
 So:
 
 - An exit code of `2` means that all tests failed.
 - An exit code of `6` means that all tests either failed or errored.
 - An exit code of `7` indicates that the result contains a mix of passed, failed and errored tests.
```

### Comparing `pytest-exit-code-0.1.0/pyproject.toml` & `pytest_exit_code-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytest-exit-code"
 description = "A pytest plugin that overrides the built-in exit codes to retain more information about the test results."
-version = "0.1.0"
+version = "0.2.0"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{ name = "Sander Ploegsma", email = "sanderploegsma@gmail.com" }]
 maintainers = [{ name = "Sander Ploegsma", email = "sanderploegsma@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Framework :: Pytest",
```

### Comparing `pytest-exit-code-0.1.0/src/pytest_exit_code/plugin.py` & `pytest_exit_code-0.2.0/src/pytest_exit_code/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,30 @@
 class ExitCodePlugin:
     def __init__(self) -> None:
         self.exit_code = ExitCode.ALL_PASSED
 
     @pytest.hookimpl
     def pytest_runtest_logreport(self, report: pytest.TestReport) -> None:
         if report.passed and report.when in ["call"]:
-            self.exit_code |= ExitCode.TESTS_PASSED
+            if hasattr(report, "wasxfail"):
+                self.exit_code |= ExitCode.TESTS_XPASSED
+            else:
+                self.exit_code |= ExitCode.TESTS_PASSED
 
         if report.failed:
             if report.when in ["setup", "teardown"]:
                 self.exit_code |= ExitCode.TESTS_ERRORED
             else:
                 self.exit_code |= ExitCode.TESTS_FAILED
 
         if report.skipped:
-            self.exit_code |= ExitCode.TESTS_SKIPPED
+            if hasattr(report, "wasxfail"):
+                self.exit_code |= ExitCode.TESTS_XFAILED
+            else:
+                self.exit_code |= ExitCode.TESTS_SKIPPED
 
     @pytest.hookimpl
     def pytest_sessionfinish(self, session: pytest.Session):
         if self.exit_code > ExitCode.TESTS_PASSED:
             session.exitstatus = self.exit_code
         else:
             session.exitstatus = ExitCode.ALL_PASSED
```

### Comparing `pytest-exit-code-0.1.0/src/pytest_exit_code.egg-info/PKG-INFO` & `pytest_exit_code-0.2.0/src/pytest_exit_code.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-exit-code
-Version: 0.1.0
+Version: 0.2.0
 Summary: A pytest plugin that overrides the built-in exit codes to retain more information about the test results.
 Author-email: Sander Ploegsma <sanderploegsma@gmail.com>
 Maintainer-email: Sander Ploegsma <sanderploegsma@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -231,23 +231,25 @@
 # pytest-exit-code [![PyPi version][pypi-version-badge]][pypi-project] [![Python versions][pypi-pyversions-badge]][pypi-project]
 
 A [pytest] plugin that overrides the built-in exit codes to retain more information about the test results.
 
 ## Features
 
 This plugin changes the exit code returned by running `pytest`.
-The exit codes can range from `0` to `15` and are a combination of the following bitwise flags:
+The exit codes can range from `0` to `63` and are a combination of the following bitwise flags:
 
 | Flag | Description                     |
 | ---- | ------------------------------- |
 | `0`  | All tests passed.               |
 | `1`  | One or more tests passed.       |
 | `2`  | One or more tests failed.       |
 | `4`  | One or more tests errored.      |
 | `8`  | One or more tests were skipped. |
+| `16` | One or more tests xfailed.      |
+| `32` | One or more tests xpassed.      |
 
 So:
 
 - An exit code of `2` means that all tests failed.
 - An exit code of `6` means that all tests either failed or errored.
 - An exit code of `7` indicates that the result contains a mix of passed, failed and errored tests.
```

### Comparing `pytest-exit-code-0.1.0/tests/test_exit_code.py` & `pytest_exit_code-0.2.0/tests/test_exit_code.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import pytest
-
 from pytest_exit_code import ExitCode
 
 
 @pytest.mark.parametrize(
     "keyword,expected",
     [
         ("test_pass", ExitCode.ALL_PASSED),
         ("test_fail", ExitCode.TESTS_FAILED),
         ("test_error", ExitCode.TESTS_ERRORED),
         ("test_skip", ExitCode.TESTS_SKIPPED),
+        ("test_xfail", ExitCode.TESTS_XFAILED),
+        ("test_xpass", ExitCode.TESTS_XPASSED),
+        ("test_strict_xfail", ExitCode.TESTS_FAILED),
         (
             "",
             ExitCode.TESTS_PASSED
             | ExitCode.TESTS_FAILED
             | ExitCode.TESTS_ERRORED
-            | ExitCode.TESTS_SKIPPED,
+            | ExitCode.TESTS_SKIPPED
+            | ExitCode.TESTS_XFAILED
+            | ExitCode.TESTS_XPASSED,
         ),
         ("test_unknown", ExitCode.ALL_PASSED),
     ],
 )
 def test_correct_exit_codes(
     pytester,
     keyword: str,
@@ -41,12 +45,24 @@
 
         def test_error(failing_fixture):
             assert 1 == 1
 
         @pytest.mark.skip
         def test_skip():
             assert 1 == 1
+
+        @pytest.mark.xfail
+        def test_xfail():
+            raise RuntimeError("Failure in test")
+
+        @pytest.mark.xfail
+        def test_xpass():
+            assert 1 == 1
+
+        @pytest.mark.xfail(strict=True)
+        def test_strict_xfail():
+            assert 1 == 1
     """
     )
 
     result = pytester.runpytest("-k", keyword)
     assert result.ret == expected
```

