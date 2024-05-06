# Comparing `tmp/inquirer3-0.4.0.tar.gz` & `tmp/inquirer3-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inquirer3-0.4.0.tar", max compression
+gzip compressed data, was "inquirer3-0.5.0.tar", max compression
```

## Comparing `inquirer3-0.4.0.tar` & `inquirer3-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1090 2023-09-17 12:08:25.903193 inquirer3-0.4.0/LICENSE
--rw-r--r--   0        0        0     5331 2023-09-17 12:08:25.903193 inquirer3-0.4.0/README.md
--rw-r--r--   0        0        0     1853 2023-09-17 12:08:43.888644 inquirer3-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      974 2023-09-17 12:08:25.907193 inquirer3-0.4.0/src/inquirer3/__init__.py
--rw-r--r--   0        0        0      412 2023-09-17 12:08:25.907193 inquirer3-0.4.0/src/inquirer3/errors.py
--rw-r--r--   0        0        0      351 2023-09-17 12:08:25.907193 inquirer3-0.4.0/src/inquirer3/events.py
--rw-r--r--   0        0        0      439 2023-09-17 12:08:25.907193 inquirer3-0.4.0/src/inquirer3/prompt.py
--rw-r--r--   0        0        0    12339 2023-09-17 12:08:25.907193 inquirer3-0.4.0/src/inquirer3/questions.py
--rw-r--r--   0        0        0      315 2023-09-17 12:08:25.907193 inquirer3-0.4.0/src/inquirer3/render/__init__.py
--rw-r--r--   0        0        0     6733 2023-09-17 12:08:25.911193 inquirer3-0.4.0/src/inquirer3/render/console/__init__.py
--rw-r--r--   0        0        0     5368 2023-09-17 12:08:25.911193 inquirer3-0.4.0/src/inquirer3/render/console/_checkbox.py
--rw-r--r--   0        0        0      726 2023-09-17 12:08:25.911193 inquirer3-0.4.0/src/inquirer3/render/console/_confirm.py
--rw-r--r--   0        0        0     1091 2023-09-17 12:08:25.911193 inquirer3-0.4.0/src/inquirer3/render/console/_editor.py
--rw-r--r--   0        0        0     3550 2023-09-17 12:08:25.911193 inquirer3-0.4.0/src/inquirer3/render/console/_list.py
--rw-r--r--   0        0        0      103 2023-09-17 12:08:25.911193 inquirer3-0.4.0/src/inquirer3/render/console/_other.py
--rw-r--r--   0        0        0      382 2023-09-17 12:08:25.911193 inquirer3-0.4.0/src/inquirer3/render/console/_password.py
--rw-r--r--   0        0        0       77 2023-09-17 12:08:25.911193 inquirer3-0.4.0/src/inquirer3/render/console/_path.py
--rw-r--r--   0        0        0     2483 2023-09-17 12:08:25.911193 inquirer3-0.4.0/src/inquirer3/render/console/_text.py
--rw-r--r--   0        0        0     1314 2023-09-17 12:08:25.911193 inquirer3-0.4.0/src/inquirer3/render/console/base.py
--rw-r--r--   0        0        0     6034 2023-09-17 12:08:25.911193 inquirer3-0.4.0/src/inquirer3/shortcuts.py
--rw-r--r--   0        0        0     4484 2023-09-17 12:08:25.911193 inquirer3-0.4.0/src/inquirer3/themes.py
--rw-r--r--   0        0        0     6615 1970-01-01 00:00:00.000000 inquirer3-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-05-06 01:47:49.046846 inquirer3-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5331 2024-05-06 01:47:49.046846 inquirer3-0.5.0/README.md
+-rw-r--r--   0        0        0     1829 2024-05-06 01:47:58.098863 inquirer3-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      974 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/__init__.py
+-rw-r--r--   0        0        0      412 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/errors.py
+-rw-r--r--   0        0        0      351 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/events.py
+-rw-r--r--   0        0        0      439 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/prompt.py
+-rw-r--r--   0        0        0    12339 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/questions.py
+-rw-r--r--   0        0        0      315 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/render/__init__.py
+-rw-r--r--   0        0        0     6678 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/render/console/__init__.py
+-rw-r--r--   0        0        0     5368 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/render/console/_checkbox.py
+-rw-r--r--   0        0        0      726 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/render/console/_confirm.py
+-rw-r--r--   0        0        0     1091 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/render/console/_editor.py
+-rw-r--r--   0        0        0     3550 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/render/console/_list.py
+-rw-r--r--   0        0        0      103 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/render/console/_other.py
+-rw-r--r--   0        0        0      382 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/render/console/_password.py
+-rw-r--r--   0        0        0       77 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/render/console/_path.py
+-rw-r--r--   0        0        0     2483 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/render/console/_text.py
+-rw-r--r--   0        0        0     1314 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/render/console/base.py
+-rw-r--r--   0        0        0     6034 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/shortcuts.py
+-rw-r--r--   0        0        0     4484 2024-05-06 01:47:49.050846 inquirer3-0.5.0/src/inquirer3/themes.py
+-rw-r--r--   0        0        0     6620 1970-01-01 00:00:00.000000 inquirer3-0.5.0/PKG-INFO
```

### Comparing `inquirer3-0.4.0/LICENSE` & `inquirer3-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inquirer3-0.4.0/README.md` & `inquirer3-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `inquirer3-0.4.0/pyproject.toml` & `inquirer3-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inquirer3"
-version = "0.4.0"
+version = "0.5.0"
 description = "Collection of common interactive command line user interfaces, based on Inquirer.js"
 authors = ["Guy Salton <guy123121@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/guysalt/python-inquirer3"
 repository = "https://github.com/guysalt/python-inquirer3"
 documentation = "https://python-inquirer3.readthedocs.io/en/latest/"
@@ -21,32 +21,31 @@
     "Topic :: Software Development :: User Interfaces",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 blessed = "^1.20.0"
-readchar = "^4.0.5"
+readchar = "^4.0.6"
 python-editor = "^1.0.4"
-coloredlogs = "^15.0.1"
 
 [tool.poetry.group.dev.dependencies]
-bandit = "^1.7.5"
+bandit = "^1.7.8"
 flake8 = "^5.0.0"
 flake8-docstrings = "^1.7.0"
-furo = "^2023.5.20"
-isort = "^5.12.0"
-pexpect = "^4.8.0"
+furo = "^2024.4.27"
+isort = "^5.13.2"
+pexpect = "^4.9.0"
 pre-commit = "^3.3.3"
-pre-commit-hooks = "^4.4.0"
+pre-commit-hooks = "^4.6.0"
 pyupgrade = "^3.8.0"
-safety = "^2.3.5"
+safety = "^3.2.0"
 sphinx = "^7.0.1"
 sphinx-autobuild = "^2021.3.14"
-nox = "^2023.4.22"
+nox = "^2024.4.15"
 nox-poetry = "^1.0.3"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
```

### Comparing `inquirer3-0.4.0/src/inquirer3/__init__.py` & `inquirer3-0.5.0/src/inquirer3/__init__.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.4.0/src/inquirer3/questions.py` & `inquirer3-0.5.0/src/inquirer3/questions.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.4.0/src/inquirer3/render/console/__init__.py` & `inquirer3-0.5.0/src/inquirer3/render/console/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-import logging
 import math
 import sys
 
-import coloredlogs
 from blessed import Terminal
 
 from inquirer3 import errors
 from inquirer3 import events
 from inquirer3 import themes
 from inquirer3.render.console._checkbox import Checkbox
 from inquirer3.render.console._confirm import Confirm
 from inquirer3.render.console._editor import Editor
 from inquirer3.render.console._list import List
 from inquirer3.render.console._password import Password
 from inquirer3.render.console._path import Path
 from inquirer3.render.console._text import Text
 
-coloredlogs.install()
-logger = logging.getLogger(__name__)
-
 
 class ConsoleRender:
     def __init__(self, event_generator=None, theme=None, raise_keyboard_interrupt: bool = False, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._event_gen = event_generator or events.KeyEventGenerator()
         self.terminal = Terminal()
         self._previous_error = None
@@ -55,16 +50,16 @@
 
                 self._process_input(render)
 
         except KeyboardInterrupt:
             if self._raise_keyboard_interrupt:
                 raise
             self.clear_bottombar()
-            print()
-            logger.info("Cancelled by user")
+            print("\n", end="\n" if render.title_inline else "")
+            print("Cancelled by user")
 
         except errors.EndOfInput as e:
             self._go_to_end(render)
             return e.selection
 
     def _print_status_bar(self):
         if self._previous_error is None:
```

### Comparing `inquirer3-0.4.0/src/inquirer3/render/console/_checkbox.py` & `inquirer3-0.5.0/src/inquirer3/render/console/_checkbox.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.4.0/src/inquirer3/render/console/_confirm.py` & `inquirer3-0.5.0/src/inquirer3/render/console/_confirm.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.4.0/src/inquirer3/render/console/_editor.py` & `inquirer3-0.5.0/src/inquirer3/render/console/_editor.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.4.0/src/inquirer3/render/console/_list.py` & `inquirer3-0.5.0/src/inquirer3/render/console/_list.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.4.0/src/inquirer3/render/console/_text.py` & `inquirer3-0.5.0/src/inquirer3/render/console/_text.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.4.0/src/inquirer3/render/console/base.py` & `inquirer3-0.5.0/src/inquirer3/render/console/base.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.4.0/src/inquirer3/shortcuts.py` & `inquirer3-0.5.0/src/inquirer3/shortcuts.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.4.0/src/inquirer3/themes.py` & `inquirer3-0.5.0/src/inquirer3/themes.py`

 * *Files identical despite different names*

### Comparing `inquirer3-0.4.0/PKG-INFO` & `inquirer3-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inquirer3
-Version: 0.4.0
+Version: 0.5.0
 Summary: Collection of common interactive command line user interfaces, based on Inquirer.js
 Home-page: https://github.com/guysalt/python-inquirer3
 License: MIT
 Author: Guy Salton
 Author-email: guy123121@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,20 +13,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Dist: blessed (>=1.20.0,<2.0.0)
-Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: python-editor (>=1.0.4,<2.0.0)
-Requires-Dist: readchar (>=4.0.5,<5.0.0)
+Requires-Dist: readchar (>=4.0.6,<5.0.0)
 Project-URL: Documentation, https://python-inquirer3.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/guysalt/python-inquirer3
 Description-Content-Type: text/markdown
 
 [![PyPI](https://img.shields.io/pypi/v/inquirer3.svg)][pypi status]
 [![Status](https://img.shields.io/pypi/status/inquirer3.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/inquirer3.svg)][pypi status]
```

