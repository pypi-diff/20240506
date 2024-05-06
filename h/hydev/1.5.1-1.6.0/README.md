# Comparing `tmp/hydev-1.5.1.tar.gz` & `tmp/hydev-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydev-1.5.1.tar", max compression
+gzip compressed data, was "hydev-1.6.0.tar", max compression
```

## Comparing `hydev-1.5.1.tar` & `hydev-1.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      252 2024-05-01 07:45:10.622666 hydev-1.5.1/LICENSE
--rw-r--r--   0        0        0     2525 2024-05-01 08:00:52.847272 hydev-1.5.1/pyproject.toml
--rw-r--r--   0        0        0       35 2024-05-01 07:45:10.622666 hydev-1.5.1/src/hydev/__init__.py
--rw-r--r--   0        0        0     2021 2024-05-01 08:00:11.955072 hydev-1.5.1/src/hydev/common_pyproject.toml
--rw-r--r--   0        0        0     7828 2024-05-01 07:45:10.622666 hydev-1.5.1/src/hydev/main.py
--rw-r--r--   0        0        0     2888 2024-05-01 08:00:36.151190 hydev-1.5.1/src/hydev/utils.py
--rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 hydev-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0      252 2024-05-01 07:45:10.622666 hydev-1.6.0/LICENSE
+-rw-r--r--   0        0        0     2525 2024-05-06 08:57:44.114690 hydev-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-05-01 07:45:10.622666 hydev-1.6.0/src/hydev/__init__.py
+-rw-r--r--   0        0        0     2021 2024-05-01 08:00:11.955072 hydev-1.6.0/src/hydev/common_pyproject.toml
+-rw-r--r--   0        0        0     7919 2024-05-06 08:56:45.854405 hydev-1.6.0/src/hydev/main.py
+-rw-r--r--   0        0        0     2888 2024-05-01 08:00:36.151190 hydev-1.6.0/src/hydev/utils.py
+-rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 hydev-1.6.0/PKG-INFO
```

### Comparing `hydev-1.5.1/pyproject.toml` & `hydev-1.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hydev"
-version = "1.5.1"
+version = "1.6.0"
 description = "Common tooling and configuration for pythonic development"
 authors = ["hoverhell <hoverhell@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.scripts]
 hydautoflake = "hydev.main:Autoflake.run_cli"
 hydblack = "hydev.main:Black.run_cli"
```

### Comparing `hydev-1.5.1/src/hydev/common_pyproject.toml` & `hydev-1.6.0/src/hydev/common_pyproject.toml`

 * *Files identical despite different names*

### Comparing `hydev-1.5.1/src/hydev/main.py` & `hydev-1.6.0/src/hydev/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 from .utils import TCfg, deep_merge, dumps_configparser, getitem_path, pair_window
 
 HERE = Path(__file__).parent
 MAIN_CONFIG = toml.loads((HERE / "common_pyproject.toml").read_text())
 
 
 def read_local_config(local_path: str | Path = "pyproject.toml") -> TCfg:
-    return toml.loads(Path(local_path).read_text())
+    try:
+        config_text = Path(local_path).read_text()
+    except FileNotFoundError:
+        return {}
+    return toml.loads(config_text)
 
 
 class CLIToolBase:
     def run(self) -> None:
         raise NotImplementedError
 
     @classmethod
```

### Comparing `hydev-1.5.1/src/hydev/utils.py` & `hydev-1.6.0/src/hydev/utils.py`

 * *Files identical despite different names*

### Comparing `hydev-1.5.1/PKG-INFO` & `hydev-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydev
-Version: 1.5.1
+Version: 1.6.0
 Summary: Common tooling and configuration for pythonic development
 License: MIT
 Author: hoverhell
 Author-email: hoverhell@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

