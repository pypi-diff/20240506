# Comparing `tmp/luxos-0.0.5b20.tar.gz` & `tmp/luxos-0.0.6b21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luxos-0.0.5b20.tar", last modified: Sat May  4 07:53:37 2024, max compression
+gzip compressed data, was "luxos-0.0.6b21.tar", last modified: Sun May  5 23:55:31 2024, max compression
```

## Comparing `luxos-0.0.5b20.tar` & `luxos-0.0.6b21.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:53:37.259047 luxos-0.0.5b20/
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-05-04 07:53:37.259047 luxos-0.0.5b20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-04 07:53:08.000000 luxos-0.0.5b20/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-04 07:53:35.000000 luxos-0.0.5b20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 07:53:37.259047 luxos-0.0.5b20/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:53:37.251047 luxos-0.0.5b20/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:53:37.255047 luxos-0.0.5b20/src/luxos/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-04 07:53:35.000000 luxos-0.0.5b20/src/luxos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-04 07:53:08.000000 luxos-0.0.5b20/src/luxos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-04 07:53:08.000000 luxos-0.0.5b20/src/luxos/api.json
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-04 07:53:08.000000 luxos-0.0.5b20/src/luxos/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-04 07:53:08.000000 luxos-0.0.5b20/src/luxos/asyncops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:53:37.255047 luxos-0.0.5b20/src/luxos/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 07:53:08.000000 luxos-0.0.5b20/src/luxos/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-04 07:53:08.000000 luxos-0.0.5b20/src/luxos/cli/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-04 07:53:08.000000 luxos-0.0.5b20/src/luxos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-04 07:53:08.000000 luxos-0.0.5b20/src/luxos/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 07:53:08.000000 luxos-0.0.5b20/src/luxos/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:53:37.255047 luxos-0.0.5b20/src/luxos/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 07:53:08.000000 luxos-0.0.5b20/src/luxos/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-04 07:53:08.000000 luxos-0.0.5b20/src/luxos/scripts/async_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-05-04 07:53:08.000000 luxos-0.0.5b20/src/luxos/scripts/health_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-04 07:53:08.000000 luxos-0.0.5b20/src/luxos/scripts/luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-04 07:53:08.000000 luxos-0.0.5b20/src/luxos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:53:37.259047 luxos-0.0.5b20/src/luxos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-05-04 07:53:37.000000 luxos-0.0.5b20/src/luxos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-04 07:53:37.000000 luxos-0.0.5b20/src/luxos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 07:53:37.000000 luxos-0.0.5b20/src/luxos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-04 07:53:37.000000 luxos-0.0.5b20/src/luxos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-04 07:53:37.000000 luxos-0.0.5b20/src/luxos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 07:53:37.000000 luxos-0.0.5b20/src/luxos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 07:53:37.259047 luxos-0.0.5b20/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-04 07:53:08.000000 luxos-0.0.5b20/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-04 07:53:08.000000 luxos-0.0.5b20/tests/test_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-04 07:53:08.000000 luxos-0.0.5b20/tests/test_luxos_asyncops.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-04 07:53:08.000000 luxos-0.0.5b20/tests/test_luxos_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:55:31.472222 luxos-0.0.6b21/
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-05 23:55:31.472222 luxos-0.0.6b21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-05 23:54:57.000000 luxos-0.0.6b21/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-05 23:55:29.000000 luxos-0.0.6b21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 23:55:31.472222 luxos-0.0.6b21/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:55:31.464223 luxos-0.0.6b21/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:55:31.468222 luxos-0.0.6b21/src/luxos/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-05 23:55:29.000000 luxos-0.0.6b21/src/luxos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-05 23:54:57.000000 luxos-0.0.6b21/src/luxos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-05 23:54:57.000000 luxos-0.0.6b21/src/luxos/api.json
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-05 23:54:57.000000 luxos-0.0.6b21/src/luxos/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-05 23:54:57.000000 luxos-0.0.6b21/src/luxos/asyncops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:55:31.468222 luxos-0.0.6b21/src/luxos/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:54:57.000000 luxos-0.0.6b21/src/luxos/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-05 23:54:57.000000 luxos-0.0.6b21/src/luxos/cli/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-05 23:54:57.000000 luxos-0.0.6b21/src/luxos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-05 23:54:57.000000 luxos-0.0.6b21/src/luxos/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:54:57.000000 luxos-0.0.6b21/src/luxos/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:55:31.468222 luxos-0.0.6b21/src/luxos/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 23:54:57.000000 luxos-0.0.6b21/src/luxos/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-05 23:54:57.000000 luxos-0.0.6b21/src/luxos/scripts/async_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-05-05 23:54:57.000000 luxos-0.0.6b21/src/luxos/scripts/health_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-05 23:54:57.000000 luxos-0.0.6b21/src/luxos/scripts/luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-05 23:54:57.000000 luxos-0.0.6b21/src/luxos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:55:31.472222 luxos-0.0.6b21/src/luxos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-05 23:55:31.000000 luxos-0.0.6b21/src/luxos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-05 23:55:31.000000 luxos-0.0.6b21/src/luxos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 23:55:31.000000 luxos-0.0.6b21/src/luxos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-05 23:55:31.000000 luxos-0.0.6b21/src/luxos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-05 23:55:31.000000 luxos-0.0.6b21/src/luxos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 23:55:31.000000 luxos-0.0.6b21/src/luxos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 23:55:31.472222 luxos-0.0.6b21/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-05 23:54:57.000000 luxos-0.0.6b21/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-05 23:54:57.000000 luxos-0.0.6b21/tests/test_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-05 23:54:57.000000 luxos-0.0.6b21/tests/test_luxos_asyncops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-05 23:54:57.000000 luxos-0.0.6b21/tests/test_luxos_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-05 23:54:57.000000 luxos-0.0.6b21/tests/test_utils.py
```

### Comparing `luxos-0.0.5b20/PKG-INFO` & `luxos-0.0.6b21/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.5b20
+Version: 0.0.6b21
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -29,20 +29,19 @@
 [![Build](https://github.com/LuxorLabs/luxos-tooling/actions/workflows/push-main.yml/badge.svg)](https://github.com/LuxorLabs/luxos/actions/runs/0)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/luxos)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 This repository contains scripts we built to operate and troubleshoot miners running LuxOS.
 
-For an example how to use the luxos line tool 👉 [here](#usage-cli)
+For an example how to use the luxos command line tool 👉 [here](#usage-cli).
 
-For a quick example how to control miners using the luxos api 👉 [here](#usage-api)
+For a quick example how to control miners using the luxos api 👉 [here](#usage-api).
 
-
-For an example how to use the command line tool 👉 [here](docs/CLI.md)
+If you're developing a script, you might want to leverage the luxos cli package 👉 [here](docs/CLI.md).
 
 
 ## Installation
 
 To install the latest and greatest version:
 ```bash
    $> pip install -U luxos
@@ -72,15 +71,15 @@
 
 See files under the docs/folder.
 
 
 ## Examples
 This is a curated list of examples.
 
-### The LuxOS API - luxos
+### The LuxOS package - luxos
 
 This package offers a convenient way to interact with LuxOS through a command-line interface (CLI) or as Python packages for more advanced integrations.
 
 #### Usage (cli)
 
 The luxos wheel package comes with a luxos comand line script:
```

### Comparing `luxos-0.0.5b20/README.md` & `luxos-0.0.6b21/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 [![Build](https://github.com/LuxorLabs/luxos-tooling/actions/workflows/push-main.yml/badge.svg)](https://github.com/LuxorLabs/luxos/actions/runs/0)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/luxos)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 This repository contains scripts we built to operate and troubleshoot miners running LuxOS.
 
-For an example how to use the luxos line tool 👉 [here](#usage-cli)
+For an example how to use the luxos command line tool 👉 [here](#usage-cli).
 
-For a quick example how to control miners using the luxos api 👉 [here](#usage-api)
+For a quick example how to control miners using the luxos api 👉 [here](#usage-api).
 
-
-For an example how to use the command line tool 👉 [here](docs/CLI.md)
+If you're developing a script, you might want to leverage the luxos cli package 👉 [here](docs/CLI.md).
 
 
 ## Installation
 
 To install the latest and greatest version:
 ```bash
    $> pip install -U luxos
@@ -49,15 +48,15 @@
 
 See files under the docs/folder.
 
 
 ## Examples
 This is a curated list of examples.
 
-### The LuxOS API - luxos
+### The LuxOS package - luxos
 
 This package offers a convenient way to interact with LuxOS through a command-line interface (CLI) or as Python packages for more advanced integrations.
 
 #### Usage (cli)
 
 The luxos wheel package comes with a luxos comand line script:
```

### Comparing `luxos-0.0.5b20/pyproject.toml` & `luxos-0.0.6b21/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "luxos"
-version = "0.0.5b20"
+version = "0.0.6b21"
 description = "The all encompassing LuxOS python library."
 readme = "README.md"
 license = { text = "MIT" }  # TODO I don't think this is a MIT??
 requires-python = ">= 3.9"
 
 authors = [
   { name = "Antonio Cavallo", email = "antonio.cavallo@luxor.tech" },
```

### Comparing `luxos-0.0.5b20/src/luxos/api.json` & `luxos-0.0.6b21/src/luxos/api.json`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b20/src/luxos/api.py` & `luxos-0.0.6b21/src/luxos/api.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b20/src/luxos/asyncops.py` & `luxos-0.0.6b21/src/luxos/asyncops.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         return ((host, port), ret) if add_address else ret
     finally:
         if sid:
             await logoff(host, port, sid)
 
 
 def _rexec_paramteres(
-    parameters: str | list[str] | dict[str, Any] | None = None,
+    parameters: str | list[Any] | dict[str, Any] | None = None,
 ) -> list[str]:
     if isinstance(parameters, dict):
         data = []
         for key, value in parameters.items():
             if value is None:
                 value = "null"
             elif value is True:
@@ -248,15 +248,15 @@
     return parameters
 
 
 async def rexec(
     host: str,
     port: int,
     cmd: str,
-    parameters: str | list[str] | dict[str, Any] | None = None,
+    parameters: str | list[Any] | dict[str, Any] | None = None,
     timeout: float | None = None,
     retry: int | None = None,
     retry_delay: float | None = None,
 ) -> dict[str, Any] | None:
     from . import api
 
     parameters = _rexec_paramteres(parameters)
```

### Comparing `luxos-0.0.5b20/src/luxos/cli/v1.py` & `luxos-0.0.6b21/src/luxos/cli/v1.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b20/src/luxos/exceptions.py` & `luxos-0.0.6b21/src/luxos/exceptions.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b20/src/luxos/misc.py` & `luxos-0.0.6b21/src/luxos/misc.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b20/src/luxos/scripts/async_luxos.py` & `luxos-0.0.6b21/src/luxos/scripts/async_luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b20/src/luxos/scripts/health_checker.py` & `luxos-0.0.6b21/src/luxos/scripts/health_checker.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b20/src/luxos/scripts/luxos.py` & `luxos-0.0.6b21/src/luxos/scripts/luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b20/src/luxos.egg-info/PKG-INFO` & `luxos-0.0.6b21/src/luxos.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.5b20
+Version: 0.0.6b21
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -29,20 +29,19 @@
 [![Build](https://github.com/LuxorLabs/luxos-tooling/actions/workflows/push-main.yml/badge.svg)](https://github.com/LuxorLabs/luxos/actions/runs/0)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/luxos)
 [![Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 This repository contains scripts we built to operate and troubleshoot miners running LuxOS.
 
-For an example how to use the luxos line tool 👉 [here](#usage-cli)
+For an example how to use the luxos command line tool 👉 [here](#usage-cli).
 
-For a quick example how to control miners using the luxos api 👉 [here](#usage-api)
+For a quick example how to control miners using the luxos api 👉 [here](#usage-api).
 
-
-For an example how to use the command line tool 👉 [here](docs/CLI.md)
+If you're developing a script, you might want to leverage the luxos cli package 👉 [here](docs/CLI.md).
 
 
 ## Installation
 
 To install the latest and greatest version:
 ```bash
    $> pip install -U luxos
@@ -72,15 +71,15 @@
 
 See files under the docs/folder.
 
 
 ## Examples
 This is a curated list of examples.
 
-### The LuxOS API - luxos
+### The LuxOS package - luxos
 
 This package offers a convenient way to interact with LuxOS through a command-line interface (CLI) or as Python packages for more advanced integrations.
 
 #### Usage (cli)
 
 The luxos wheel package comes with a luxos comand line script:
```

### Comparing `luxos-0.0.5b20/src/luxos.egg-info/SOURCES.txt` & `luxos-0.0.6b21/src/luxos.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 src/luxos/scripts/__init__.py
 src/luxos/scripts/async_luxos.py
 src/luxos/scripts/health_checker.py
 src/luxos/scripts/luxos.py
 tests/test_cli.py
 tests/test_luxos.py
 tests/test_luxos_asyncops.py
-tests/test_luxos_misc.py
+tests/test_luxos_misc.py
+tests/test_utils.py
```

### Comparing `luxos-0.0.5b20/tests/test_cli.py` & `luxos-0.0.6b21/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b20/tests/test_luxos_asyncops.py` & `luxos-0.0.6b21/tests/test_luxos_asyncops.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.5b20/tests/test_luxos_misc.py` & `luxos-0.0.6b21/tests/test_luxos_misc.py`

 * *Files identical despite different names*

