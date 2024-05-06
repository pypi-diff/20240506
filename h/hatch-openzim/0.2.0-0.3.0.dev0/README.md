# Comparing `tmp/hatch_openzim-0.2.0.tar.gz` & `tmp/hatch_openzim-0.3.0.dev0.tar.gz`

## Comparing `hatch_openzim-0.2.0.tar` & `hatch_openzim-0.3.0.dev0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tasks.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/src/hatch_openzim/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/src/hatch_openzim/__init__.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/src/hatch_openzim/build_hook.py
--rw-r--r--   0        0        0     8885 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/src/hatch_openzim/files_install.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/src/hatch_openzim/hooks.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/src/hatch_openzim/metadata.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/src/hatch_openzim/metadata_hook.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/src/hatch_openzim/shared.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/src/hatch_openzim/utils.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/test_basic.py
--rw-r--r--   0        0        0     7970 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/test_files_install.py
--rw-r--r--   0        0        0     7039 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/test_metadata.py
--rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/configs/empty.toml
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/configs/execute_after_failure.toml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/configs/extract_all_missing_target_dir.toml
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/configs/extract_items_length_not_matching.toml
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/configs/extract_items_missing_target_paths.toml
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/configs/extract_items_missing_zip_paths.toml
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/configs/full.toml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/configs/get_file_missing_target_file.toml
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/configs/gitconfig
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/configs/missing_action.toml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/configs/missing_config.toml
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/configs/missing_source.toml
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/configs/missing_target_dir.toml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/configs/other_stuff.toml
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/configs/unsupported_action.toml
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/configs/unsupported_protocol_dl.toml
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/tests/configs/unsupported_protocol_zip.toml
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/LICENSE
--rw-r--r--   0        0        0    11902 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/README.md
--rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    13582 2020-02-02 00:00:00.000000 hatch_openzim-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/CHANGELOG.md
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tasks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/src/hatch_openzim/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/src/hatch_openzim/__init__.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/src/hatch_openzim/build_hook.py
+-rw-r--r--   0        0        0     9044 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/src/hatch_openzim/files_install.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/src/hatch_openzim/hooks.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/src/hatch_openzim/metadata.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/src/hatch_openzim/metadata_hook.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/src/hatch_openzim/shared.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/src/hatch_openzim/utils.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/test_basic.py
+-rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/test_files_install.py
+-rw-r--r--   0        0        0     7039 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/test_metadata.py
+-rw-r--r--   0        0        0     4134 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/configs/empty.toml
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/configs/execute_after_failure.toml
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/configs/extract_all_missing_target_dir.toml
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/configs/extract_items_length_not_matching.toml
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/configs/extract_items_missing_target_paths.toml
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/configs/extract_items_missing_zip_paths.toml
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/configs/full.toml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/configs/get_file_missing_target_file.toml
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/configs/gitconfig
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/configs/missing_action.toml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/configs/missing_config.toml
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/configs/missing_source.toml
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/configs/missing_target_dir.toml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/configs/other_stuff.toml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/configs/unsupported_action.toml
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/configs/unsupported_protocol_dl.toml
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/tests/configs/unsupported_protocol_zip.toml
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/LICENSE
+-rw-r--r--   0        0        0    11912 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/README.md
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0    13597 2020-02-02 00:00:00.000000 hatch_openzim-0.3.0.dev0/PKG-INFO
```

### Comparing `hatch_openzim-0.2.0/.pre-commit-config.yaml` & `hatch_openzim-0.3.0.dev0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
   hooks:
   -   id: trailing-whitespace
   -   id: end-of-file-fixer
 - repo: https://github.com/psf/black
-  rev: "24.2.0"
+  rev: "24.4.2"
   hooks:
   -   id: black
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.2.1
+  rev: v0.4.3
   hooks:
   - id: ruff
 - repo: https://github.com/RobertCraigie/pyright-python
-  rev: v1.1.350
+  rev: v1.1.361
   hooks:
   - id: pyright
     name: pyright (system)
     description: 'pyright static type checker'
     entry: pyright
     language: system
     'types_or': [python, pyi]
```

### Comparing `hatch_openzim-0.2.0/CHANGELOG.md` & `hatch_openzim-0.3.0.dev0/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [Unreleased]
+
+### Fixed
+
+- Indentation of `execute_after` logs is too deep  #15
+
+### Changed
+
+- `execute_after` does not display detailled logs of stuff run #16
+
 ## [0.2.0] - 2024-02-16
 
 ### Added
 
 - Metadata hook: add suport for additional-classifiers property #10
 
 ### Fixed
 
 - Build hook: fix issue with extract_items when target_path is in a subfolder #11
-- Tests: ensure tests are also ok when ran from a fork or outside any Git structure
+- Tests: ensure tests are also ok when ran from a fork or outside any Git structure #13
 
 ## [0.1.0] - 2024-02-05
 
 ### Added
 
 - Initial release
```

### Comparing `hatch_openzim-0.2.0/tasks.py` & `hatch_openzim-0.3.0.dev0/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     ctx.run(f"black {args}", pty=use_pty)
 
 
 @task(optional=["args"], help={"args": "ruff additional arguments"})
 def fix_ruff(ctx: Context, args: str = "."):
     """fix all ruff rules"""
     args = args or "."  # needed for hatch script
-    ctx.run(f"ruff --fix {args}", pty=use_pty)
+    ctx.run(f"ruff check --fix {args}", pty=use_pty)
 
 
 @task(
     optional=["args"],
     help={
         "args": "linting tools (black, ruff) additional arguments, typically a path",
     },
```

### Comparing `hatch_openzim-0.2.0/src/hatch_openzim/build_hook.py` & `hatch_openzim-0.3.0.dev0/src/hatch_openzim/build_hook.py`

 * *Files identical despite different names*

### Comparing `hatch_openzim-0.2.0/src/hatch_openzim/files_install.py` & `hatch_openzim-0.3.0.dev0/src/hatch_openzim/files_install.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,25 +105,27 @@
     logger.info("    Done")
 
 
 def _process_execute_after(base_target_dir: Path, actions: List[str]):
     """execute actions after file(s) installation"""
 
     for action in actions:
-        logger.info(f"    Executing '{action}'")
-        process = subprocess.run(
+        logger.info(f"  Executing '{action}'")
+        process = subprocess.run(  # noqa: PLW1510
             action,
             shell=True,  # noqa: S602 # nosec: B602
             cwd=base_target_dir,
             text=True,
-            check=True,
-            capture_output=True,
+            stderr=subprocess.STDOUT,
+            stdout=subprocess.PIPE,
         )
         if process.stdout:
-            logger.info(f"      stdout:\n{process.stdout}")
+            logger.info(f"      stdout/stderr:\n{process.stdout}")
+        if process.returncode:
+            raise Exception("execute_after command failed, see logs above for details.")
 
 
 def _process_get_file_action(
     base_target_dir: Path, source: str, action_data: Dict[str, Any]
 ):
     """downloads one file to a given location"""
     target_file = action_data.get("target_file", None)
```

### Comparing `hatch_openzim-0.2.0/src/hatch_openzim/metadata.py` & `hatch_openzim-0.3.0.dev0/src/hatch_openzim/metadata.py`

 * *Files identical despite different names*

### Comparing `hatch_openzim-0.2.0/src/hatch_openzim/metadata_hook.py` & `hatch_openzim-0.3.0.dev0/src/hatch_openzim/metadata_hook.py`

 * *Files identical despite different names*

### Comparing `hatch_openzim-0.2.0/src/hatch_openzim/utils.py` & `hatch_openzim-0.3.0.dev0/src/hatch_openzim/utils.py`

 * *Files identical despite different names*

### Comparing `hatch_openzim-0.2.0/tests/test_files_install.py` & `hatch_openzim-0.3.0.dev0/tests/test_files_install.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import subprocess
 import tempfile
 from pathlib import Path
 from typing import List
 
 import pytest
 
 from hatch_openzim import files_install
@@ -208,15 +207,15 @@
     """Test case where the execute after command is failing"""
 
     # Proceed with installation in a temporary directory
     with tempfile.TemporaryDirectory() as temp_dir:
         os.chdir(temp_dir)
 
         with pytest.raises(
-            subprocess.CalledProcessError,
+            Exception, match="execute_after command failed, see logs above for details."
         ):
             files_install.process(
                 str(
                     (
                         Path(__file__).parent / "configs/execute_after_failure.toml"
                     ).absolute()
                 )
```

### Comparing `hatch_openzim-0.2.0/tests/test_metadata.py` & `hatch_openzim-0.3.0.dev0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `hatch_openzim-0.2.0/tests/test_utils.py` & `hatch_openzim-0.3.0.dev0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hatch_openzim-0.2.0/tests/configs/full.toml` & `hatch_openzim-0.3.0.dev0/tests/configs/full.toml`

 * *Files identical despite different names*

### Comparing `hatch_openzim-0.2.0/.gitignore` & `hatch_openzim-0.3.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_openzim-0.2.0/LICENSE` & `hatch_openzim-0.3.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `hatch_openzim-0.2.0/README.md` & `hatch_openzim-0.3.0.dev0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 - automatically populate common project metadatas
 - install static files (e.g. external JS dependencies) at build time
 
 This plugin intentionally has few dependencies, using the Python standard library whenever possible and hence limiting footprint to a minimum.
 
 hatch-openzim adheres to openZIM's [Contribution Guidelines](https://github.com/openzim/overview/wiki/Contributing).
 
-hatch-openzim has implemented openZIM's [Python bootstrap, conventions and policies](https://github.com/openzim/_python-bootstrap/docs/Policy.md) **v1.0.0**.
+hatch-openzim has implemented openZIM's [Python bootstrap, conventions and policies](https://github.com/openzim/_python-bootstrap/blob/main/docs/Policy.md) **v1.0.1**.
 
 ## Quick start
 
 Assuming you have an openZIM project, you could use such a configuration in your `pyproject.toml`
 
 ```toml
 # Use the hatchling build backend, with the hatch-openzim plugin.
```

### Comparing `hatch_openzim-0.2.0/pyproject.toml` & `hatch_openzim-0.3.0.dev0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,52 +3,44 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "hatch-openzim"
 requires-python = ">=3.8,<3.13"
 description = "openZIM hatch plugin to set metadata automatically and download files at build time"
 readme = "README.md"
-classifiers = [ # needs hatch-openzim 0.2.0 to make it dynamic with additional-classifiers
-    "Framework :: Hatch",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-]
 dependencies = [
   "hatchling==1.21.1",
   "packaging==23.2",
   "toml==0.10.2", # to be removed once only 3.11 and above is supported
 ]
-dynamic = ["authors", "keywords", "license", "version", "urls"]
+dynamic = ["authors", "keywords", "license", "version", "urls", "classifiers"]
 
 [tool.hatch.metadata.hooks.openzim-metadata]
 additional-keywords = ["hatch","plugin","download","file"]
-preserve-classifiers = true # to be removed once 0.2.0 is used
+additional-classifiers = [
+  "Framework :: Hatch",
+]
 
 [project.optional-dependencies]
 scripts = [
   "invoke==2.2.0",
 ]
 lint = [
-  "black==24.2.0",
-  "ruff==0.2.1",
+  "black==24.4.2",
+  "ruff==0.4.3",
 ]
 check = [
-  "pyright==1.1.350",
+  "pyright==1.1.361",
 ]
 test = [
-  "pytest==8.0.0",
-  "coverage==7.4.1",
+  "pytest==8.2.0",
+  "coverage==7.5.1",
 ]
 dev = [
-  "pre-commit==3.6.1",
+  "pre-commit==3.7.0",
   "debugpy==1.8.1",
   "hatch-openzim[scripts]",
   "hatch-openzim[lint]",
   "hatch-openzim[test]",
   "hatch-openzim[check]",
 ]
```

### Comparing `hatch_openzim-0.2.0/PKG-INFO` & `hatch_openzim-0.3.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-openzim
-Version: 0.2.0
+Version: 0.3.0.dev0
 Summary: openZIM hatch plugin to set metadata automatically and download files at build time
 Project-URL: Donate, https://www.kiwix.org/en/support-us/
 Project-URL: Homepage, https://github.com/openzim/hatch-openzim
 Author-email: openZIM <dev@openzim.org>
 License: GPL-3.0-or-later
 License-File: LICENSE
 Keywords: download,file,hatch,openzim,plugin
@@ -17,30 +17,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.8
 Requires-Dist: hatchling==1.21.1
 Requires-Dist: packaging==23.2
 Requires-Dist: toml==0.10.2
 Provides-Extra: check
-Requires-Dist: pyright==1.1.350; extra == 'check'
+Requires-Dist: pyright==1.1.361; extra == 'check'
 Provides-Extra: dev
 Requires-Dist: debugpy==1.8.1; extra == 'dev'
 Requires-Dist: hatch-openzim[check]; extra == 'dev'
 Requires-Dist: hatch-openzim[lint]; extra == 'dev'
 Requires-Dist: hatch-openzim[scripts]; extra == 'dev'
 Requires-Dist: hatch-openzim[test]; extra == 'dev'
-Requires-Dist: pre-commit==3.6.1; extra == 'dev'
+Requires-Dist: pre-commit==3.7.0; extra == 'dev'
 Provides-Extra: lint
-Requires-Dist: black==24.2.0; extra == 'lint'
-Requires-Dist: ruff==0.2.1; extra == 'lint'
+Requires-Dist: black==24.4.2; extra == 'lint'
+Requires-Dist: ruff==0.4.3; extra == 'lint'
 Provides-Extra: scripts
 Requires-Dist: invoke==2.2.0; extra == 'scripts'
 Provides-Extra: test
-Requires-Dist: coverage==7.4.1; extra == 'test'
-Requires-Dist: pytest==8.0.0; extra == 'test'
+Requires-Dist: coverage==7.5.1; extra == 'test'
+Requires-Dist: pytest==8.2.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 hatch-openzim
 =======
 
 [![Code Quality Status](https://github.com/openzim/hatch-openzim/workflows/QA/badge.svg?query=branch%3Amain)](https://github.com/openzim/hatch-openzim/actions/workflows/QA.yml?query=branch%3Amain)
 [![Tests Status](https://github.com/openzim/hatch-openzim/workflows/Tests/badge.svg?query=branch%3Amain)](https://github.com/openzim/hatch-openzim/actions/workflows/Tests.yml?query=branch%3Amain)
@@ -52,15 +52,15 @@
 - automatically populate common project metadatas
 - install static files (e.g. external JS dependencies) at build time
 
 This plugin intentionally has few dependencies, using the Python standard library whenever possible and hence limiting footprint to a minimum.
 
 hatch-openzim adheres to openZIM's [Contribution Guidelines](https://github.com/openzim/overview/wiki/Contributing).
 
-hatch-openzim has implemented openZIM's [Python bootstrap, conventions and policies](https://github.com/openzim/_python-bootstrap/docs/Policy.md) **v1.0.0**.
+hatch-openzim has implemented openZIM's [Python bootstrap, conventions and policies](https://github.com/openzim/_python-bootstrap/blob/main/docs/Policy.md) **v1.0.1**.
 
 ## Quick start
 
 Assuming you have an openZIM project, you could use such a configuration in your `pyproject.toml`
 
 ```toml
 # Use the hatchling build backend, with the hatch-openzim plugin.
```

