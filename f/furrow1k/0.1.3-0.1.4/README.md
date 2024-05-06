# Comparing `tmp/furrow1k-0.1.3.tar.gz` & `tmp/furrow1k-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furrow1k-0.1.3.tar", max compression
+gzip compressed data, was "furrow1k-0.1.4.tar", max compression
```

## Comparing `furrow1k-0.1.3.tar` & `furrow1k-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1068 2024-05-05 22:35:02.889442 furrow1k-0.1.3/LICENSE
--rw-r--r--   0        0        0      657 2024-05-05 22:35:02.901477 furrow1k-0.1.3/README.md
--rw-r--r--   0        0        0      420 2024-05-06 02:06:19.138019 furrow1k-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      110 2024-05-05 22:35:02.934491 furrow1k-0.1.3/src/furrow1k/__init__.py
--rw-r--r--   0        0        0       44 2024-05-05 22:35:03.043021 furrow1k-0.1.3/src/furrow1k/furrow1k.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 furrow1k-0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1068 2024-05-05 22:35:02.889442 furrow1k-0.1.4/LICENSE
+-rw-r--r--   0        0        0      657 2024-05-05 22:35:02.901477 furrow1k-0.1.4/README.md
+-rw-r--r--   0        0        0      415 2024-05-06 02:19:08.549884 furrow1k-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-05-05 22:35:02.934491 furrow1k-0.1.4/src/furrow1k/__init__.py
+-rw-r--r--   0        0        0       89 2024-05-06 02:18:50.508629 furrow1k-0.1.4/src/furrow1k/furrow1k.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 furrow1k-0.1.4/PKG-INFO
```

### Comparing `furrow1k-0.1.3/LICENSE` & `furrow1k-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `furrow1k-0.1.3/README.md` & `furrow1k-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `furrow1k-0.1.3/PKG-INFO` & `furrow1k-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furrow1k
-Version: 0.1.3
+Version: 0.1.4
 Summary: Help calculate percentage of salary to contribute to 401k
 License: MIT
 Author: Frank Cao
 Requires-Python: >=3.12.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

