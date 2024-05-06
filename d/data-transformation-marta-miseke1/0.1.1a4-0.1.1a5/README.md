# Comparing `tmp/data_transformation_marta_miseke1-0.1.1a4.tar.gz` & `tmp/data_transformation_marta_miseke1-0.1.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_transformation_marta_miseke1-0.1.1a4.tar", max compression
+gzip compressed data, was "data_transformation_marta_miseke1-0.1.1a5.tar", max compression
```

## Comparing `data_transformation_marta_miseke1-0.1.1a4.tar` & `data_transformation_marta_miseke1-0.1.1a5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-05 14:08:47.019323 data_transformation_marta_miseke1-0.1.1a4/data_transformation_marta_miseke1/__init__.py
--rw-r--r--   0        0        0     6640 2024-05-06 10:02:07.918178 data_transformation_marta_miseke1-0.1.1a4/data_transformation_marta_miseke1/transformation.py
--rw-r--r--   0        0        0      530 2024-05-06 12:15:28.618061 data_transformation_marta_miseke1-0.1.1a4/pyproject.toml
--rw-r--r--   0        0        0     3887 2024-05-06 12:15:18.964332 data_transformation_marta_miseke1-0.1.1a4/README.md
--rw-r--r--   0        0        0     4219 1970-01-01 00:00:00.000000 data_transformation_marta_miseke1-0.1.1a4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-05 14:08:47.019323 data_transformation_marta_miseke1-0.1.1a5/data_transformation_marta_miseke1/__init__.py
+-rw-r--r--   0        0        0     6640 2024-05-06 10:02:07.918178 data_transformation_marta_miseke1-0.1.1a5/data_transformation_marta_miseke1/transformation.py
+-rw-r--r--   0        0        0      530 2024-05-06 12:21:23.195932 data_transformation_marta_miseke1-0.1.1a5/pyproject.toml
+-rw-r--r--   0        0        0     4216 2024-05-06 12:21:00.255983 data_transformation_marta_miseke1-0.1.1a5/README.md
+-rw-r--r--   0        0        0     4540 1970-01-01 00:00:00.000000 data_transformation_marta_miseke1-0.1.1a5/PKG-INFO
```

### Comparing `data_transformation_marta_miseke1-0.1.1a4/data_transformation_marta_miseke1/transformation.py` & `data_transformation_marta_miseke1-0.1.1a5/data_transformation_marta_miseke1/transformation.py`

 * *Files identical despite different names*

### Comparing `data_transformation_marta_miseke1-0.1.1a4/pyproject.toml` & `data_transformation_marta_miseke1-0.1.1a5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-transformation-marta-miseke1"
-version = "0.1.1a4"
+version = "0.1.1a5"
 description = ""
 authors = ["Marta <marta.miseke@seb.se>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.11"
 numpy = "~1.26.4"
```

### Comparing `data_transformation_marta_miseke1-0.1.1a4/README.md` & `data_transformation_marta_miseke1-0.1.1a5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,14 @@
      [4.0, 5.5, 6.4]])
      
 After applying "transpose2d" result matrix would look like:
     [[1.0, 4.0, 1.0, 4.0], 
      [2.0, 5.5, 2.0, 5.5], 
      [3.8, 6.4, 3.8, 6.4]]  
 ```
-
 * **Sliding Window**: "window1d" function creates a sliding window over a sequence of data (NumPy array).
 Given a window size, shift and stride, it iterates through the data, providing overlapping subsets. 
 For example:
 ```
 You have an array: np.array([1, 2, 3, 4, 5, 6, 7, 8, 9]
 
 And you would like to get sliding windows of 4 elements each, containing every second element from the sequence
@@ -51,14 +50,23 @@
 And you decide that stride will be 2.
 
 After applying "convolution2d" function, received convolutional matrix (sum of kernel multiplied by parts of the
 input matrix) would look like:
     [[ 550.  790.]
      [1510. 1750.]]
 ```
+Project package is publised here: https://pypi.org/project/data-transformation-marta-miseke1/
+Package is written using python 3.11 and it uses these packages with particular versions (allowing posibility 
+to upgrade to next minor version):
+```
+python = "~3.11"
+numpy = "~1.26.4"
+logging = "~0.4.9.6"
+pytest = "~8.2.0"
+```
 
 # How to Install and Run the Project
 Installation instruction assumes that package user is using Windows OS and poetry, since it is a prerequisite in the
 project we currently work.
 * **Install Poetry**: Open PowerShell and execute the following command:
 ```
 curl -sSL https://install.python-poetry.org | python3 -
```

### Comparing `data_transformation_marta_miseke1-0.1.1a4/PKG-INFO` & `data_transformation_marta_miseke1-0.1.1a5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-transformation-marta-miseke1
-Version: 0.1.1a4
+Version: 0.1.1a5
 Summary: 
 Author: Marta
 Author-email: marta.miseke@seb.se
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: logging (>=0.4.9.6,<0.5.0.0)
@@ -32,15 +32,14 @@
      [4.0, 5.5, 6.4]])
      
 After applying "transpose2d" result matrix would look like:
     [[1.0, 4.0, 1.0, 4.0], 
      [2.0, 5.5, 2.0, 5.5], 
      [3.8, 6.4, 3.8, 6.4]]  
 ```
-
 * **Sliding Window**: "window1d" function creates a sliding window over a sequence of data (NumPy array).
 Given a window size, shift and stride, it iterates through the data, providing overlapping subsets. 
 For example:
 ```
 You have an array: np.array([1, 2, 3, 4, 5, 6, 7, 8, 9]
 
 And you would like to get sliding windows of 4 elements each, containing every second element from the sequence
@@ -65,14 +64,23 @@
 And you decide that stride will be 2.
 
 After applying "convolution2d" function, received convolutional matrix (sum of kernel multiplied by parts of the
 input matrix) would look like:
     [[ 550.  790.]
      [1510. 1750.]]
 ```
+Project package is publised here: https://pypi.org/project/data-transformation-marta-miseke1/
+Package is written using python 3.11 and it uses these packages with particular versions (allowing posibility 
+to upgrade to next minor version):
+```
+python = "~3.11"
+numpy = "~1.26.4"
+logging = "~0.4.9.6"
+pytest = "~8.2.0"
+```
 
 # How to Install and Run the Project
 Installation instruction assumes that package user is using Windows OS and poetry, since it is a prerequisite in the
 project we currently work.
 * **Install Poetry**: Open PowerShell and execute the following command:
 ```
 curl -sSL https://install.python-poetry.org | python3 -
```

