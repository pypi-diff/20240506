# Comparing `tmp/mkdocs_spellcheck-1.0.3.tar.gz` & `tmp/mkdocs_spellcheck-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_spellcheck-1.0.3.tar", last modified: Sat Mar 23 20:31:35 2024, max compression
+gzip compressed data, was "mkdocs_spellcheck-1.1.0.tar", last modified: Mon May  6 13:17:37 2024, max compression
```

## Comparing `mkdocs_spellcheck-1.0.3.tar` & `mkdocs_spellcheck-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      754 2024-03-23 20:07:34.247626 mkdocs_spellcheck-1.0.3/LICENSE
--rw-r--r--   0        0        0     2473 2024-03-23 20:07:36.794268 mkdocs_spellcheck-1.0.3/README.md
--rw-r--r--   0        0        0     1950 2024-03-23 20:31:35.848661 mkdocs_spellcheck-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      131 2024-03-23 20:07:34.330959 mkdocs_spellcheck-1.0.3/src/mkdocs_spellcheck/__init__.py
--rw-r--r--   0        0        0      908 2023-09-05 08:57:16.110986 mkdocs_spellcheck-1.0.3/src/mkdocs_spellcheck/backends/__init__.py
--rw-r--r--   0        0        0     1851 2023-09-05 08:57:16.110986 mkdocs_spellcheck-1.0.3/src/mkdocs_spellcheck/backends/codespell.py
--rw-r--r--   0        0        0     1780 2024-03-23 20:30:45.212569 mkdocs_spellcheck-1.0.3/src/mkdocs_spellcheck/backends/symspellpy.py
--rw-r--r--   0        0        0     2852 2024-03-23 20:30:45.212569 mkdocs_spellcheck-1.0.3/src/mkdocs_spellcheck/debug.py
--rw-r--r--   0        0        0      726 2023-09-05 08:57:16.110986 mkdocs_spellcheck-1.0.3/src/mkdocs_spellcheck/loggers.py
--rw-r--r--   0        0        0     4657 2023-09-05 08:59:03.126121 mkdocs_spellcheck-1.0.3/src/mkdocs_spellcheck/plugin.py
--rw-r--r--   0        0        0        0 2024-03-23 20:07:34.334292 mkdocs_spellcheck-1.0.3/src/mkdocs_spellcheck/py.typed
--rw-r--r--   0        0        0     2975 2023-09-05 08:57:16.110986 mkdocs_spellcheck-1.0.3/src/mkdocs_spellcheck/words.py
--rw-r--r--   0        0        0       37 2022-04-11 16:43:15.473251 mkdocs_spellcheck-1.0.3/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      194 2022-04-11 16:43:15.473251 mkdocs_spellcheck-1.0.3/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      295 2022-04-11 16:43:15.473251 mkdocs_spellcheck-1.0.3/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0       27 2022-04-11 16:51:35.689872 mkdocs_spellcheck-1.0.3/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2022-04-11 16:51:38.279841 mkdocs_spellcheck-1.0.3/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-04-11 16:51:38.279841 mkdocs_spellcheck-1.0.3/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       10 2022-04-11 16:51:40.213151 mkdocs_spellcheck-1.0.3/tests/.pytest_cache/v/randomly_seed
--rw-r--r--   0        0        0      170 2024-03-23 20:07:34.344292 mkdocs_spellcheck-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0       47 2024-03-23 20:07:34.344292 mkdocs_spellcheck-1.0.3/tests/conftest.py
--rw-r--r--   0        0        0     3704 2023-09-05 08:57:16.110986 mkdocs_spellcheck-1.0.3/tests/test_words.py
--rw-r--r--   0        0        0     4303 1970-01-01 00:00:00.000000 mkdocs_spellcheck-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      754 2024-03-23 20:07:34.247626 mkdocs_spellcheck-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2530 2024-05-05 17:28:24.797063 mkdocs_spellcheck-1.1.0/README.md
+-rw-r--r--   0        0        0     1950 2024-05-06 13:17:37.232141 mkdocs_spellcheck-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-03-23 20:07:34.330959 mkdocs_spellcheck-1.1.0/src/mkdocs_spellcheck/__init__.py
+-rw-r--r--   0        0        0      908 2023-09-05 08:57:16.110986 mkdocs_spellcheck-1.1.0/src/mkdocs_spellcheck/backends/__init__.py
+-rw-r--r--   0        0        0     1851 2023-09-05 08:57:16.110986 mkdocs_spellcheck-1.1.0/src/mkdocs_spellcheck/backends/codespell.py
+-rw-r--r--   0        0        0     1780 2024-03-23 20:30:45.212569 mkdocs_spellcheck-1.1.0/src/mkdocs_spellcheck/backends/symspellpy.py
+-rw-r--r--   0        0        0     2852 2024-03-23 20:30:45.212569 mkdocs_spellcheck-1.1.0/src/mkdocs_spellcheck/debug.py
+-rw-r--r--   0        0        0      726 2023-09-05 08:57:16.110986 mkdocs_spellcheck-1.1.0/src/mkdocs_spellcheck/loggers.py
+-rw-r--r--   0        0        0     4720 2024-05-05 17:29:18.947786 mkdocs_spellcheck-1.1.0/src/mkdocs_spellcheck/plugin.py
+-rw-r--r--   0        0        0        0 2024-03-23 20:07:34.334292 mkdocs_spellcheck-1.1.0/src/mkdocs_spellcheck/py.typed
+-rw-r--r--   0        0        0     2975 2023-09-05 08:57:16.110986 mkdocs_spellcheck-1.1.0/src/mkdocs_spellcheck/words.py
+-rw-r--r--   0        0        0       37 2022-04-11 16:43:15.473251 mkdocs_spellcheck-1.1.0/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      194 2022-04-11 16:43:15.473251 mkdocs_spellcheck-1.1.0/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      295 2022-04-11 16:43:15.473251 mkdocs_spellcheck-1.1.0/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0       27 2022-04-11 16:51:35.689872 mkdocs_spellcheck-1.1.0/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2022-04-11 16:51:38.279841 mkdocs_spellcheck-1.1.0/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-04-11 16:51:38.279841 mkdocs_spellcheck-1.1.0/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       10 2022-04-11 16:51:40.213151 mkdocs_spellcheck-1.1.0/tests/.pytest_cache/v/randomly_seed
+-rw-r--r--   0        0        0      170 2024-03-23 20:07:34.344292 mkdocs_spellcheck-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0       47 2024-03-23 20:07:34.344292 mkdocs_spellcheck-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     3704 2023-09-05 08:57:16.110986 mkdocs_spellcheck-1.1.0/tests/test_words.py
+-rw-r--r--   0        0        0     4376 1970-01-01 00:00:00.000000 mkdocs_spellcheck-1.1.0/PKG-INFO
```

### Comparing `mkdocs_spellcheck-1.0.3/LICENSE` & `mkdocs_spellcheck-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_spellcheck-1.0.3/README.md` & `mkdocs_spellcheck-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -50,18 +50,19 @@
 
     # maximum number of capital letters in a word
     max_capital: 1
 
     # keep unicode characters
     allow_unicode: no
 
-    # skip files entirely
+    # skip files entirely (supports Unix shell-style wildcards)
     skip_files:
     - credits.md
     - coverage.md
+    - reference/* 
 
     # whether to only check in strict mode
     strict_only: yes
 ```
 
 By default, the `symspellpy` backend is used.
```

### Comparing `mkdocs_spellcheck-1.0.3/pyproject.toml` & `mkdocs_spellcheck-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Topic :: Documentation",
     "Topic :: Software Development",
     "Topic :: Software Development :: Documentation",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = []
-version = "1.0.3"
+version = "1.1.0"
 
 [project.license]
 text = "ISC"
 
 [project.optional-dependencies]
 all = [
     "mkdocs-spellcheck[codespell,symspellpy]",
```

### Comparing `mkdocs_spellcheck-1.0.3/src/mkdocs_spellcheck/backends/__init__.py` & `mkdocs_spellcheck-1.1.0/src/mkdocs_spellcheck/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs_spellcheck-1.0.3/src/mkdocs_spellcheck/backends/codespell.py` & `mkdocs_spellcheck-1.1.0/src/mkdocs_spellcheck/backends/codespell.py`

 * *Files identical despite different names*

### Comparing `mkdocs_spellcheck-1.0.3/src/mkdocs_spellcheck/backends/symspellpy.py` & `mkdocs_spellcheck-1.1.0/src/mkdocs_spellcheck/backends/symspellpy.py`

 * *Files identical despite different names*

### Comparing `mkdocs_spellcheck-1.0.3/src/mkdocs_spellcheck/debug.py` & `mkdocs_spellcheck-1.1.0/src/mkdocs_spellcheck/debug.py`

 * *Files identical despite different names*

### Comparing `mkdocs_spellcheck-1.0.3/src/mkdocs_spellcheck/loggers.py` & `mkdocs_spellcheck-1.1.0/src/mkdocs_spellcheck/loggers.py`

 * *Files identical despite different names*

### Comparing `mkdocs_spellcheck-1.0.3/src/mkdocs_spellcheck/plugin.py` & `mkdocs_spellcheck-1.1.0/src/mkdocs_spellcheck/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """MkDocs SpellCheck package.
 
 A spell checker plugin for MkDocs.
 """
 
 from __future__ import annotations
 
+from fnmatch import fnmatch
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 from mkdocs.config.config_options import Type as MkType
 from mkdocs.plugins import BasePlugin
 
 from mkdocs_spellcheck.loggers import get_plugin_logger
@@ -125,15 +126,15 @@
         Hook for the [`on_page_content` event](https://www.mkdocs.org/user-guide/plugins/#on_page_content).
 
         Arguments:
             html: The HTML text.
             page: The page instance.
             **kwargs: Additional arguments passed by MkDocs.
         """
-        if self.run and page.file.src_path not in self.skip_files:
+        if self.run and not any(fnmatch(page.file.src_path, pattern) for pattern in self.skip_files):
             words = get_words(
                 html,
                 known_words=self.known_words,
                 min_length=self.min_length,
                 max_capital=self.max_capital,
                 ignore_code=self.ignore_code,
                 allow_unicode=self.allow_unicode,
```

### Comparing `mkdocs_spellcheck-1.0.3/src/mkdocs_spellcheck/words.py` & `mkdocs_spellcheck-1.1.0/src/mkdocs_spellcheck/words.py`

 * *Files identical despite different names*

### Comparing `mkdocs_spellcheck-1.0.3/tests/test_words.py` & `mkdocs_spellcheck-1.1.0/tests/test_words.py`

 * *Files identical despite different names*

### Comparing `mkdocs_spellcheck-1.0.3/PKG-INFO` & `mkdocs_spellcheck-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mkdocs-spellcheck
-Version: 1.0.3
+Version: 1.1.0
 Summary: A spell checker plugin for MkDocs.
-Author-Email: Timothée Mazzucotelli <dev@pawamoy.fr>
+Author-Email: =?utf-8?q?Timoth=C3=A9e_Mazzucotelli?= <dev@pawamoy.fr>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -89,18 +89,19 @@
 
     # maximum number of capital letters in a word
     max_capital: 1
 
     # keep unicode characters
     allow_unicode: no
 
-    # skip files entirely
+    # skip files entirely (supports Unix shell-style wildcards)
     skip_files:
     - credits.md
     - coverage.md
+    - reference/* 
 
     # whether to only check in strict mode
     strict_only: yes
 ```
 
 By default, the `symspellpy` backend is used.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

