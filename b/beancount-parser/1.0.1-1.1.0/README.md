# Comparing `tmp/beancount_parser-1.0.1.tar.gz` & `tmp/beancount_parser-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount_parser-1.0.1.tar", max compression
+gzip compressed data, was "beancount_parser-1.1.0.tar", max compression
```

## Comparing `beancount_parser-1.0.1.tar` & `beancount_parser-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1076 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/LICENSE
--rw-r--r--   0        0        0     2434 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/__init__.py
--rw-r--r--   0        0        0      335 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/account.lark
--rw-r--r--   0        0        0     3467 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/beancount.lark
--rw-r--r--   0        0        0       26 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/boolean.lark
--rw-r--r--   0        0        0       22 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/comment.lark
--rw-r--r--   0        0        0      162 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/currency.lark
--rw-r--r--   0        0        0      404 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/date.lark
--rw-r--r--   0        0        0      397 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/escaped_string.lark
--rw-r--r--   0        0        0      208 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/flag.lark
--rw-r--r--   0        0        0      223 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/link.lark
--rw-r--r--   0        0        0      162 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/numbers.lark
--rw-r--r--   0        0        0       29 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/section_header.lark
--rw-r--r--   0        0        0      289 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/tag.lark
--rw-r--r--   0        0        0      403 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/parser.py
--rw-r--r--   0        0        0      529 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3168 1970-01-01 00:00:00.000000 beancount_parser-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-05 21:43:27.542408 beancount_parser-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2434 2024-05-05 21:43:27.542408 beancount_parser-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 21:43:27.542408 beancount_parser-1.1.0/beancount_parser/__init__.py
+-rw-r--r--   0        0        0      335 2024-05-05 21:43:27.542408 beancount_parser-1.1.0/beancount_parser/grammar/account.lark
+-rw-r--r--   0        0        0     3467 2024-05-05 21:43:27.542408 beancount_parser-1.1.0/beancount_parser/grammar/beancount.lark
+-rw-r--r--   0        0        0       26 2024-05-05 21:43:27.542408 beancount_parser-1.1.0/beancount_parser/grammar/boolean.lark
+-rw-r--r--   0        0        0       22 2024-05-05 21:43:27.542408 beancount_parser-1.1.0/beancount_parser/grammar/comment.lark
+-rw-r--r--   0        0        0      162 2024-05-05 21:43:27.542408 beancount_parser-1.1.0/beancount_parser/grammar/currency.lark
+-rw-r--r--   0        0        0      404 2024-05-05 21:43:27.542408 beancount_parser-1.1.0/beancount_parser/grammar/date.lark
+-rw-r--r--   0        0        0      397 2024-05-05 21:43:27.542408 beancount_parser-1.1.0/beancount_parser/grammar/escaped_string.lark
+-rw-r--r--   0        0        0      208 2024-05-05 21:43:27.546408 beancount_parser-1.1.0/beancount_parser/grammar/flag.lark
+-rw-r--r--   0        0        0      223 2024-05-05 21:43:27.546408 beancount_parser-1.1.0/beancount_parser/grammar/link.lark
+-rw-r--r--   0        0        0      162 2024-05-05 21:43:27.546408 beancount_parser-1.1.0/beancount_parser/grammar/numbers.lark
+-rw-r--r--   0        0        0       29 2024-05-05 21:43:27.546408 beancount_parser-1.1.0/beancount_parser/grammar/section_header.lark
+-rw-r--r--   0        0        0      289 2024-05-05 21:43:27.546408 beancount_parser-1.1.0/beancount_parser/grammar/tag.lark
+-rw-r--r--   0        0        0     2337 2024-05-05 21:43:27.546408 beancount_parser-1.1.0/beancount_parser/parser.py
+-rw-r--r--   0        0        0      529 2024-05-05 21:43:27.546408 beancount_parser-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3168 1970-01-01 00:00:00.000000 beancount_parser-1.1.0/PKG-INFO
```

### Comparing `beancount_parser-1.0.1/LICENSE` & `beancount_parser-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beancount_parser-1.0.1/README.md` & `beancount_parser-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `beancount_parser-1.0.1/beancount_parser/grammar/beancount.lark` & `beancount_parser-1.1.0/beancount_parser/grammar/beancount.lark`

 * *Files identical despite different names*

### Comparing `beancount_parser-1.0.1/pyproject.toml` & `beancount_parser-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beancount-parser"
-version = "1.0.1"
+version = "1.1.0"
 description = "Standalone Lark based Beancount syntax parser (not relying on Beancount library), MIT license"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 repository = "https://github.com/LaunchPlatform/beancount-parser"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `beancount_parser-1.0.1/PKG-INFO` & `beancount_parser-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beancount-parser
-Version: 1.0.1
+Version: 1.1.0
 Summary: Standalone Lark based Beancount syntax parser (not relying on Beancount library), MIT license
 Home-page: https://github.com/LaunchPlatform/beancount-parser
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: beancount-parser Version: 1.0.1 Summary: Standalone
+Metadata-Version: 2.1 Name: beancount-parser Version: 1.1.0 Summary: Standalone
 Lark based Beancount syntax parser (not relying on Beancount library), MIT
 license Home-page: https://github.com/LaunchPlatform/beancount-parser License:
 MIT Author: Fang-Pen Lin Author-email: fangpen@launchplatform.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: lark
```

