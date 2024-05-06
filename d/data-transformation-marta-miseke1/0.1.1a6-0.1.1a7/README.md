# Comparing `tmp/data_transformation_marta_miseke1-0.1.1a6.tar.gz` & `tmp/data_transformation_marta_miseke1-0.1.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_transformation_marta_miseke1-0.1.1a6.tar", max compression
+gzip compressed data, was "data_transformation_marta_miseke1-0.1.1a7.tar", max compression
```

## Comparing `data_transformation_marta_miseke1-0.1.1a6.tar` & `data_transformation_marta_miseke1-0.1.1a7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-05 14:08:47.019323 data_transformation_marta_miseke1-0.1.1a6/data_transformation_marta_miseke1/__init__.py
--rw-r--r--   0        0        0     6640 2024-05-06 10:02:07.918178 data_transformation_marta_miseke1-0.1.1a6/data_transformation_marta_miseke1/transformation.py
--rw-r--r--   0        0        0      530 2024-05-06 12:23:33.051115 data_transformation_marta_miseke1-0.1.1a6/pyproject.toml
--rw-r--r--   0        0        0     4222 2024-05-06 12:22:53.361340 data_transformation_marta_miseke1-0.1.1a6/README.md
--rw-r--r--   0        0        0     4545 1970-01-01 00:00:00.000000 data_transformation_marta_miseke1-0.1.1a6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-05 14:08:47.019323 data_transformation_marta_miseke1-0.1.1a7/data_transformation_marta_miseke1/__init__.py
+-rw-r--r--   0        0        0     6640 2024-05-06 10:02:07.918178 data_transformation_marta_miseke1-0.1.1a7/data_transformation_marta_miseke1/transformation.py
+-rw-r--r--   0        0        0      530 2024-05-06 18:05:03.201202 data_transformation_marta_miseke1-0.1.1a7/pyproject.toml
+-rw-r--r--   0        0        0     4422 2024-05-06 12:39:12.157483 data_transformation_marta_miseke1-0.1.1a7/README.md
+-rw-r--r--   0        0        0     4741 1970-01-01 00:00:00.000000 data_transformation_marta_miseke1-0.1.1a7/PKG-INFO
```

### Comparing `data_transformation_marta_miseke1-0.1.1a6/data_transformation_marta_miseke1/transformation.py` & `data_transformation_marta_miseke1-0.1.1a7/data_transformation_marta_miseke1/transformation.py`

 * *Files identical despite different names*

### Comparing `data_transformation_marta_miseke1-0.1.1a6/pyproject.toml` & `data_transformation_marta_miseke1-0.1.1a7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-transformation-marta-miseke1"
-version = "0.1.1a6"
+version = "0.1.1a7"
 description = ""
 authors = ["Marta <marta.miseke@seb.se>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.11"
 numpy = "~1.26.4"
```

### Comparing `data_transformation_marta_miseke1-0.1.1a6/README.md` & `data_transformation_marta_miseke1-0.1.1a7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -102,8 +102,11 @@
     print('transposed matrix', transposed)
     window = data.window1d(np.array([1, 2, 3, 4, 5, 6, 7, 8, 9]), 4, 1, 2)
     print('Sliding windows:',window)
     convolution = data.convolution2d(np.array(
         [[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]]),
         np.array([[10, 20], [40, 50]]), 2)
     print('convolutional matrix:',convolution)
-```
+```
+# What could be improved next:
+* More unit tests could be written, in order to perform better testing and cover more test cases
+* More sophisticated algorithms could be used in package functions
```

### Comparing `data_transformation_marta_miseke1-0.1.1a6/PKG-INFO` & `data_transformation_marta_miseke1-0.1.1a7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-transformation-marta-miseke1
-Version: 0.1.1a6
+Version: 0.1.1a7
 Summary: 
 Author: Marta
 Author-email: marta.miseke@seb.se
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: logging (>=0.4.9.6,<0.5.0.0)
@@ -117,7 +117,11 @@
     window = data.window1d(np.array([1, 2, 3, 4, 5, 6, 7, 8, 9]), 4, 1, 2)
     print('Sliding windows:',window)
     convolution = data.convolution2d(np.array(
         [[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]]),
         np.array([[10, 20], [40, 50]]), 2)
     print('convolutional matrix:',convolution)
 ```
+# What could be improved next:
+* More unit tests could be written, in order to perform better testing and cover more test cases
+* More sophisticated algorithms could be used in package functions
+
```

