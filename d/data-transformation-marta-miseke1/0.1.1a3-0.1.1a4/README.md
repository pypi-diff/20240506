# Comparing `tmp/data_transformation_marta_miseke1-0.1.1a3.tar.gz` & `tmp/data_transformation_marta_miseke1-0.1.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_transformation_marta_miseke1-0.1.1a3.tar", max compression
+gzip compressed data, was "data_transformation_marta_miseke1-0.1.1a4.tar", max compression
```

## Comparing `data_transformation_marta_miseke1-0.1.1a3.tar` & `data_transformation_marta_miseke1-0.1.1a4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-05 14:08:47.019323 data_transformation_marta_miseke1-0.1.1a3/data_transformation_marta_miseke1/__init__.py
--rw-r--r--   0        0        0     6640 2024-05-06 10:02:07.918178 data_transformation_marta_miseke1-0.1.1a3/data_transformation_marta_miseke1/transformation.py
--rw-r--r--   0        0        0      530 2024-05-06 12:10:00.914863 data_transformation_marta_miseke1-0.1.1a3/pyproject.toml
--rw-r--r--   0        0        0     3838 2024-05-06 12:09:14.545103 data_transformation_marta_miseke1-0.1.1a3/README.md
--rw-r--r--   0        0        0     4180 1970-01-01 00:00:00.000000 data_transformation_marta_miseke1-0.1.1a3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-05 14:08:47.019323 data_transformation_marta_miseke1-0.1.1a4/data_transformation_marta_miseke1/__init__.py
+-rw-r--r--   0        0        0     6640 2024-05-06 10:02:07.918178 data_transformation_marta_miseke1-0.1.1a4/data_transformation_marta_miseke1/transformation.py
+-rw-r--r--   0        0        0      530 2024-05-06 12:15:28.618061 data_transformation_marta_miseke1-0.1.1a4/pyproject.toml
+-rw-r--r--   0        0        0     3887 2024-05-06 12:15:18.964332 data_transformation_marta_miseke1-0.1.1a4/README.md
+-rw-r--r--   0        0        0     4219 1970-01-01 00:00:00.000000 data_transformation_marta_miseke1-0.1.1a4/PKG-INFO
```

### Comparing `data_transformation_marta_miseke1-0.1.1a3/data_transformation_marta_miseke1/transformation.py` & `data_transformation_marta_miseke1-0.1.1a4/data_transformation_marta_miseke1/transformation.py`

 * *Files identical despite different names*

### Comparing `data_transformation_marta_miseke1-0.1.1a3/pyproject.toml` & `data_transformation_marta_miseke1-0.1.1a4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-transformation-marta-miseke1"
-version = "0.1.1a3"
+version = "0.1.1a4"
 description = ""
 authors = ["Marta <marta.miseke@seb.se>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.11"
 numpy = "~1.26.4"
```

### Comparing `data_transformation_marta_miseke1-0.1.1a3/README.md` & `data_transformation_marta_miseke1-0.1.1a4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,85 +1,95 @@
 # Data transformation library
 This project builds python library, containing data transformation functions. 
-Library supposed to be used by data-scientists.
+Library is supposed to be used by data-scientists.
 
 # Project Description
-The Python data transformation package is designed to assist with common data 
+The Python data transformation package is designed to assist with a common data 
 transformation and manipulation tasks. Described data transformation package
 provides three essential functions:
-* **Transpose Data**: "transpose2d" function allows user to swap rows and columns in a matrix
-(list of lists of float values). It’s particularly useful when you need to reorganize data for further
-analysis. For example:
+* **Transpose Data**: "transpose2d" function allows users to swap rows and columns in a matrix
+(list of lists of float values). 
+It’s particularly useful when you need to reorganize data for further analysis. 
+For example:
 ```  
 You have a matrix, which looks like:
     [[1.0, 2.0, 3.8],
      [4.0, 5.5, 6.4],
      [1.0, 2.0, 3.8], 
      [4.0, 5.5, 6.4]])
+     
 After applying "transpose2d" result matrix would look like:
     [[1.0, 4.0, 1.0, 4.0], 
      [2.0, 5.5, 2.0, 5.5], 
      [3.8, 6.4, 3.8, 6.4]]  
 ```
 
 * **Sliding Window**: "window1d" function creates a sliding window over a sequence of data (NumPy array).
 Given a window size, shift and stride, it iterates through the data, providing overlapping subsets. 
 For example:
 ```
 You have an array: np.array([1, 2, 3, 4, 5, 6, 7, 8, 9]
+
 And you would like to get sliding windows of 4 elements each, containing every second element from the sequence
 and shifting by 1 position each time.
+
 After applying "window1d" function, received sliding windows would looke like:
     [[2 4 6 8]
         [3 5 7 9]]
 ```
-* **Convolutional Matrix**: "convolution2d" function performs matrix convolution. Convolution is commonly used
-in image processing, signal analysis, and neural networks. In this package, it will be applied on 2D matrix 
-(NumPy array) with possibility to define stride. Using this function, custom kernels could be applied on data:
+* **Convolutional Matrix**: "convolution2d" function performs matrix convolution. 
+Convolution is commonly used in image processing, signal analysis, and neural networks. In this package, 
+it will be applied on 2D matrix(NumPy array) with possibility to define stride. 
+Using this function, custom kernels could be applied on data. 
+For example:
 ```
 You have a 2D matrix: 
         np.array([[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]])
+        
 You have a kernel matrix:
         np.array([[10, 20], [40, 50]])
+        
 And you decide that stride will be 2.
+
 After applying "convolution2d" function, received convolutional matrix (sum of kernel multiplied by parts of the
 input matrix) would look like:
     [[ 550.  790.]
      [1510. 1750.]]
 ```
 
 # How to Install and Run the Project
 Installation instruction assumes that package user is using Windows OS and poetry, since it is a prerequisite in the
 project we currently work.
-
-    - 1. *Install Poetry*: Open PowerShell and execute the following command:
+* **Install Poetry**: Open PowerShell and execute the following command:
 ```
 curl -sSL https://install.python-poetry.org | python3 -
 ```
-    - 2. *Create a new project using poetry*: In your IDE tool open the terminal and run command to create new project:
+* **Create a new project using poetry**: In your IDE tool open the terminal and run command to create new project:
 ```
 poetry new my_project_name
 ```
-    - 3. *Install data-transformation library*: Using the terminal, enter created project and run this command to install
+* **Install data-transformation library**: Using the terminal, enter created project and run this command to install
 data-transformation package:
 ```
 poetry add data-transformation-marta-miseke1
 ```
-# How to Run Tests
 
+# How to Run Tests
 Project contains 5 unit tests. To make sure that all features work correctly, tests could be run using command:
 ```
 poetry run pytest
 ```
+
 # How to Use the Package
-To your created project, import DataTransformation class. For example:
+To your created project, import DataTransformation class.
+For example:
 ```
 from data_transformation_marta_miseke1 import DataTransformation
 ```
-Examples of usage of library functions:
+**Examples of usage of library functions**:
 ```
     data = DataTransformation()
     transposed = data.transpose2d([[1.0, 2.0, 3.8], [4.0, 5.5, 6.4],
                                    [1.0, 2.0, 3.8], [4.0, 5.5, 6.4]])
     print('transposed matrix', transposed)
     window = data.window1d(np.array([1, 2, 3, 4, 5, 6, 7, 8, 9]), 4, 1, 2)
     print('Sliding windows:',window)
```

### Comparing `data_transformation_marta_miseke1-0.1.1a3/PKG-INFO` & `data_transformation_marta_miseke1-0.1.1a4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,109 @@
 Metadata-Version: 2.1
 Name: data-transformation-marta-miseke1
-Version: 0.1.1a3
+Version: 0.1.1a4
 Summary: 
 Author: Marta
 Author-email: marta.miseke@seb.se
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: logging (>=0.4.9.6,<0.5.0.0)
 Requires-Dist: numpy (>=1.26.4,<1.27.0)
 Requires-Dist: pytest (>=8.2.0,<8.3.0)
 Description-Content-Type: text/markdown
 
 # Data transformation library
 This project builds python library, containing data transformation functions. 
-Library supposed to be used by data-scientists.
+Library is supposed to be used by data-scientists.
 
 # Project Description
-The Python data transformation package is designed to assist with common data 
+The Python data transformation package is designed to assist with a common data 
 transformation and manipulation tasks. Described data transformation package
 provides three essential functions:
-* **Transpose Data**: "transpose2d" function allows user to swap rows and columns in a matrix
-(list of lists of float values). It’s particularly useful when you need to reorganize data for further
-analysis. For example:
+* **Transpose Data**: "transpose2d" function allows users to swap rows and columns in a matrix
+(list of lists of float values). 
+It’s particularly useful when you need to reorganize data for further analysis. 
+For example:
 ```  
 You have a matrix, which looks like:
     [[1.0, 2.0, 3.8],
      [4.0, 5.5, 6.4],
      [1.0, 2.0, 3.8], 
      [4.0, 5.5, 6.4]])
+     
 After applying "transpose2d" result matrix would look like:
     [[1.0, 4.0, 1.0, 4.0], 
      [2.0, 5.5, 2.0, 5.5], 
      [3.8, 6.4, 3.8, 6.4]]  
 ```
 
 * **Sliding Window**: "window1d" function creates a sliding window over a sequence of data (NumPy array).
 Given a window size, shift and stride, it iterates through the data, providing overlapping subsets. 
 For example:
 ```
 You have an array: np.array([1, 2, 3, 4, 5, 6, 7, 8, 9]
+
 And you would like to get sliding windows of 4 elements each, containing every second element from the sequence
 and shifting by 1 position each time.
+
 After applying "window1d" function, received sliding windows would looke like:
     [[2 4 6 8]
         [3 5 7 9]]
 ```
-* **Convolutional Matrix**: "convolution2d" function performs matrix convolution. Convolution is commonly used
-in image processing, signal analysis, and neural networks. In this package, it will be applied on 2D matrix 
-(NumPy array) with possibility to define stride. Using this function, custom kernels could be applied on data:
+* **Convolutional Matrix**: "convolution2d" function performs matrix convolution. 
+Convolution is commonly used in image processing, signal analysis, and neural networks. In this package, 
+it will be applied on 2D matrix(NumPy array) with possibility to define stride. 
+Using this function, custom kernels could be applied on data. 
+For example:
 ```
 You have a 2D matrix: 
         np.array([[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]])
+        
 You have a kernel matrix:
         np.array([[10, 20], [40, 50]])
+        
 And you decide that stride will be 2.
+
 After applying "convolution2d" function, received convolutional matrix (sum of kernel multiplied by parts of the
 input matrix) would look like:
     [[ 550.  790.]
      [1510. 1750.]]
 ```
 
 # How to Install and Run the Project
 Installation instruction assumes that package user is using Windows OS and poetry, since it is a prerequisite in the
 project we currently work.
-
-    - 1. *Install Poetry*: Open PowerShell and execute the following command:
+* **Install Poetry**: Open PowerShell and execute the following command:
 ```
 curl -sSL https://install.python-poetry.org | python3 -
 ```
-    - 2. *Create a new project using poetry*: In your IDE tool open the terminal and run command to create new project:
+* **Create a new project using poetry**: In your IDE tool open the terminal and run command to create new project:
 ```
 poetry new my_project_name
 ```
-    - 3. *Install data-transformation library*: Using the terminal, enter created project and run this command to install
+* **Install data-transformation library**: Using the terminal, enter created project and run this command to install
 data-transformation package:
 ```
 poetry add data-transformation-marta-miseke1
 ```
-# How to Run Tests
 
+# How to Run Tests
 Project contains 5 unit tests. To make sure that all features work correctly, tests could be run using command:
 ```
 poetry run pytest
 ```
+
 # How to Use the Package
-To your created project, import DataTransformation class. For example:
+To your created project, import DataTransformation class.
+For example:
 ```
 from data_transformation_marta_miseke1 import DataTransformation
 ```
-Examples of usage of library functions:
+**Examples of usage of library functions**:
 ```
     data = DataTransformation()
     transposed = data.transpose2d([[1.0, 2.0, 3.8], [4.0, 5.5, 6.4],
                                    [1.0, 2.0, 3.8], [4.0, 5.5, 6.4]])
     print('transposed matrix', transposed)
     window = data.window1d(np.array([1, 2, 3, 4, 5, 6, 7, 8, 9]), 4, 1, 2)
     print('Sliding windows:',window)
```

