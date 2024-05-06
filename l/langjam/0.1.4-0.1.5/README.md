# Comparing `tmp/langjam-0.1.4.tar.gz` & `tmp/langjam-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langjam-0.1.4.tar", max compression
+gzip compressed data, was "langjam-0.1.5.tar", max compression
```

## Comparing `langjam-0.1.4.tar` & `langjam-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11356 2024-01-21 09:11:55.610347 langjam-0.1.4/LICENSE
--rw-r--r--   0        0        0      208 2024-02-13 03:22:07.507294 langjam-0.1.4/README.md
--rw-r--r--   0        0        0      417 2024-02-15 08:19:25.511868 langjam-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-21 08:21:06.617635 langjam-0.1.4/src/langjam/__init__.py
--rw-r--r--   0        0        0        0 2024-02-12 04:13:22.069279 langjam-0.1.4/src/langjam/openai/__init__.py
--rw-r--r--   0        0        0        0 2024-02-12 06:59:55.786254 langjam-0.1.4/src/langjam/openai/openai_function/__init__.py
--rw-r--r--   0        0        0     4554 2024-02-15 08:05:02.108802 langjam-0.1.4/src/langjam/openai/openai_function/openai_function.py
--rw-r--r--   0        0        0      653 2024-02-14 17:02:38.025634 langjam-0.1.4/src/langjam/openai/openai_function/openai_function_model.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 langjam-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-01-21 09:11:55.610347 langjam-0.1.5/LICENSE
+-rw-r--r--   0        0        0      208 2024-02-13 03:22:07.507294 langjam-0.1.5/README.md
+-rw-r--r--   0        0        0      450 2024-05-06 05:16:46.876359 langjam-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-21 08:21:06.617635 langjam-0.1.5/src/langjam/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-12 04:13:22.069279 langjam-0.1.5/src/langjam/openai/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-12 06:59:55.786254 langjam-0.1.5/src/langjam/openai/openai_function/__init__.py
+-rw-r--r--   0        0        0     4554 2024-02-15 08:05:02.108802 langjam-0.1.5/src/langjam/openai/openai_function/openai_function.py
+-rw-r--r--   0        0        0      653 2024-02-14 17:02:38.025634 langjam-0.1.5/src/langjam/openai/openai_function/openai_function_model.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 langjam-0.1.5/PKG-INFO
```

### Comparing `langjam-0.1.4/LICENSE` & `langjam-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langjam-0.1.4/src/langjam/openai/openai_function/openai_function.py` & `langjam-0.1.5/src/langjam/openai/openai_function/openai_function.py`

 * *Files identical despite different names*

### Comparing `langjam-0.1.4/src/langjam/openai/openai_function/openai_function_model.py` & `langjam-0.1.5/src/langjam/openai/openai_function/openai_function_model.py`

 * *Files identical despite different names*

### Comparing `langjam-0.1.4/PKG-INFO` & `langjam-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langjam
-Version: 0.1.4
+Version: 0.1.5
 Summary: Utils for large language model
 Author: Anurag Jha
 Author-email: toanuragjha@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

