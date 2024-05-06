# Comparing `tmp/poetry_plugin_dotenv-1.0.1.tar.gz` & `tmp/poetry_plugin_dotenv-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_dotenv-1.0.1.tar", max compression
+gzip compressed data, was "poetry_plugin_dotenv-2.0.0.tar", max compression
```

## Comparing `poetry_plugin_dotenv-1.0.1.tar` & `poetry_plugin_dotenv-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1077 2024-04-26 13:46:10.240793 poetry_plugin_dotenv-1.0.1/LICENSE
--rw-r--r--   0        0        0     9687 2024-04-26 13:46:10.240793 poetry_plugin_dotenv-1.0.1/README.md
--rw-r--r--   0        0        0     7134 2024-04-26 13:46:35.701019 poetry_plugin_dotenv-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      778 2024-04-26 13:46:35.701019 poetry_plugin_dotenv-1.0.1/src/poetry_plugin_dotenv/__init__.py
--rw-r--r--   0        0        0     3084 2024-04-26 13:46:10.248793 poetry_plugin_dotenv-1.0.1/src/poetry_plugin_dotenv/config.py
--rw-r--r--   0        0        0      335 2024-04-26 13:46:10.248793 poetry_plugin_dotenv-1.0.1/src/poetry_plugin_dotenv/dotenv/__init__.py
--rw-r--r--   0        0        0     5421 2024-04-26 13:46:10.248793 poetry_plugin_dotenv-1.0.1/src/poetry_plugin_dotenv/dotenv/core.py
--rw-r--r--   0        0        0     6005 2024-04-26 13:46:10.248793 poetry_plugin_dotenv-1.0.1/src/poetry_plugin_dotenv/dotenv/parsers.py
--rw-r--r--   0        0        0     1572 2024-04-26 13:46:10.248793 poetry_plugin_dotenv-1.0.1/src/poetry_plugin_dotenv/dotenv/variables.py
--rw-r--r--   0        0        0     3287 2024-04-26 13:46:10.248793 poetry_plugin_dotenv-1.0.1/src/poetry_plugin_dotenv/plugin.py
--rw-r--r--   0        0        0        0 2024-04-26 13:46:10.248793 poetry_plugin_dotenv-1.0.1/src/poetry_plugin_dotenv/py.typed
--rw-r--r--   0        0        0    11690 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-06 20:55:24.914678 poetry_plugin_dotenv-2.0.0/LICENSE
+-rw-r--r--   0        0        0     9687 2024-05-06 20:55:24.914678 poetry_plugin_dotenv-2.0.0/README.md
+-rw-r--r--   0        0        0     6906 2024-05-06 20:55:45.866966 poetry_plugin_dotenv-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      778 2024-05-06 20:55:45.866966 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/__init__.py
+-rw-r--r--   0        0        0     3051 2024-05-06 20:55:24.926678 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/config.py
+-rw-r--r--   0        0        0      335 2024-05-06 20:55:24.926678 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/dotenv/__init__.py
+-rw-r--r--   0        0        0     5421 2024-05-06 20:55:24.926678 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/dotenv/core.py
+-rw-r--r--   0        0        0     6005 2024-05-06 20:55:24.926678 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/dotenv/parsers.py
+-rw-r--r--   0        0        0     1572 2024-05-06 20:55:24.926678 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/dotenv/variables.py
+-rw-r--r--   0        0        0     1558 2024-05-06 20:55:24.926678 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/logger.py
+-rw-r--r--   0        0        0     1999 2024-05-06 20:55:24.926678 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/plugin.py
+-rw-r--r--   0        0        0        0 2024-05-06 20:55:24.926678 poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/py.typed
+-rw-r--r--   0        0        0    11690 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-2.0.0/PKG-INFO
```

### Comparing `poetry_plugin_dotenv-1.0.1/LICENSE` & `poetry_plugin_dotenv-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-1.0.1/README.md` & `poetry_plugin_dotenv-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-1.0.1/pyproject.toml` & `poetry_plugin_dotenv-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-dotenv"
-version = "1.0.1"
+version = "2.0.0"
 description = "poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 license = "MIT"
 authors = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 maintainers = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 keywords = [
   "python",
   "pypi",
@@ -100,28 +100,18 @@
 [tool.poetry.group.ci.dependencies]
 python-semantic-release = ">=8.7,<10.0"
 
 [tool.poetry.plugins."poetry.application.plugin"]
 poetry-plugin-dotenv = "poetry_plugin_dotenv.plugin:DotenvPlugin"
 
 [tool.semantic_release]
-branch = "main"
 changelog_file = "CHANGELOG.md"
-dist_path = "dist"
-upload_to_repository = true
-upload_to_release = true
-remove_dist = false
 version_toml = ["pyproject.toml:tool.poetry.version"]
 version_variables = ["src/poetry_plugin_dotenv/__init__.py:__version__"]
 commit_author = "github-actions <github-actions@github.com>"
-commit_parser = "angular"
-
-[tool.semantic_release.publish]
-dist_glob_patterns = ["dist/*"]
-upload_to_vcs_release = true
 
 [tool.semantic_release.commit_parser_options]
 major_tags = ["feat"]
 minor_tags = ["fix", "perf", "refactor"]
 patch_tags = ["docs", "style"]
 allowed_tags = [
   "build",
```

### Comparing `poetry_plugin_dotenv-1.0.1/src/poetry_plugin_dotenv/__init__.py` & `poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."""
 
 __title__ = "poetry-plugin-dotenv"
 __summary__ = "poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 __uri__ = "https://github.com/pivoshenko/poetry-plugin-dotenv"
 
-__version__ = "1.0.1"
+__version__ = "2.0.0"
 
 __author__ = "Volodymyr Pivoshenko"
 __email__ = "volodymyr.pivoshenko@gmail.com"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023, Volodymyr Pivoshenko"
```

### Comparing `poetry_plugin_dotenv-1.0.1/src/poetry_plugin_dotenv/config.py` & `poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 import os
 import dataclasses
 
 from pathlib import Path
 
-import tomli
+import tomlkit
 
 
 CONFIG_SOURCES: dict[str, str] = {
     "pyproject.toml": "tool.poetry.plugins.dotenv",
     "os": "POETRY_PLUGIN_DOTENV_",
 }
 
@@ -35,16 +35,15 @@
 class _Config:
     """Defines the data schema and defaults used for plugin configuration."""
 
     ignore: bool = False
     location: str | None = None
 
 
-# TODO(pivoshenko): this configuration loader is a "quick patch" solution.
-# It should be considered to rewrite it
+# TODO(pivoshenko): this configuration loader is a "quick patch" solution
 class Config(_Config):
     """Configuration loader."""
 
     def __init__(self) -> None:
         """Initialize."""
 
         source_config = {}
@@ -83,15 +82,15 @@
 ) -> dict[str, str | bool | None]:
     """Load configuration from the TOML file."""
 
     filepath = Path(filename)
 
     if filepath.exists():
         with filepath.open("rb") as toml_file:
-            toml = tomli.load(toml_file)
+            toml = tomlkit.load(toml_file)
 
         config = toml
         for key in section.split("."):
             config = config.get(key, {})
 
         return config
 
@@ -109,15 +108,15 @@
         if key.startswith(section)
     }
 
 
 def _as_bool(value: str) -> bool:
     """Given a string value that represents True or False, returns the Boolean equivalent.
 
-    Heavily inspired from distutils strtobool.
+    Heavily inspired from ``distutils strtobool``.
     """
 
     try:
         return _STR_BOOLEAN_MAPPING[value.lower()]
 
     except KeyError:
         msg = f"Invalid truth value {value}"
```

### Comparing `poetry_plugin_dotenv-1.0.1/src/poetry_plugin_dotenv/dotenv/core.py` & `poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/dotenv/core.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-1.0.1/src/poetry_plugin_dotenv/dotenv/parsers.py` & `poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/dotenv/parsers.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-1.0.1/src/poetry_plugin_dotenv/dotenv/variables.py` & `poetry_plugin_dotenv-2.0.0/src/poetry_plugin_dotenv/dotenv/variables.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-1.0.1/PKG-INFO` & `poetry_plugin_dotenv-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-dotenv
-Version: 1.0.1
+Version: 2.0.0
 Summary: poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run.
 Home-page: https://github.com/pivoshenko/poetry-plugin-dotenv
 License: MIT
 Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-plugins,env,dotenv,config,configuration,configuration-management,cross-platform,hacktoberfest
 Author: Volodymyr Pivoshenko
 Author-email: volodymyr.pivoshenko@gmail.com
 Maintainer: Volodymyr Pivoshenko
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poetry-plugin-dotenv Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: poetry-plugin-dotenv Version: 2.0.0 Summary:
 poetry-plugin-dotenv - is the plugin that automatically loads environment
 variables from a dotenv file into the environment before poetry commands are
 run. Home-page: https://github.com/pivoshenko/poetry-plugin-dotenv License: MIT
 Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-
 plugins,env,dotenv,config,configuration,configuration-management,cross-
 platform,hacktoberfest Author: Volodymyr Pivoshenko Author-email:
 volodymyr.pivoshenko@gmail.com Maintainer: Volodymyr Pivoshenko Maintainer-
```

