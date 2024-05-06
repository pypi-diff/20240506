# Comparing `tmp/data_transformation_marta_miseke1-0.1.1a0.tar.gz` & `tmp/data_transformation_marta_miseke1-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_transformation_marta_miseke1-0.1.1a0.tar", max compression
+gzip compressed data, was "data_transformation_marta_miseke1-0.1.1a2.tar", max compression
```

## Comparing `data_transformation_marta_miseke1-0.1.1a0.tar` & `data_transformation_marta_miseke1-0.1.1a2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-05 14:08:47.019323 data_transformation_marta_miseke1-0.1.1a0/data_transformation_marta_miseke1/__init__.py
--rw-r--r--   0        0        0     6667 2024-05-05 14:09:27.191760 data_transformation_marta_miseke1-0.1.1a0/data_transformation_marta_miseke1/transformation.py
--rw-r--r--   0        0        0      530 2024-05-05 14:16:41.426461 data_transformation_marta_miseke1-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-05 14:08:47.019323 data_transformation_marta_miseke1-0.1.1a0/README.md
--rw-r--r--   0        0        0      431 1970-01-01 00:00:00.000000 data_transformation_marta_miseke1-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-05 14:08:47.019323 data_transformation_marta_miseke1-0.1.1a2/data_transformation_marta_miseke1/__init__.py
+-rw-r--r--   0        0        0     6640 2024-05-06 10:02:07.918178 data_transformation_marta_miseke1-0.1.1a2/data_transformation_marta_miseke1/transformation.py
+-rw-r--r--   0        0        0      530 2024-05-06 11:46:15.098533 data_transformation_marta_miseke1-0.1.1a2/pyproject.toml
+-rw-r--r--   0        0        0     5016 2024-05-06 11:42:40.867965 data_transformation_marta_miseke1-0.1.1a2/README.md
+-rw-r--r--   0        0        0     5348 1970-01-01 00:00:00.000000 data_transformation_marta_miseke1-0.1.1a2/PKG-INFO
```

### Comparing `data_transformation_marta_miseke1-0.1.1a0/data_transformation_marta_miseke1/transformation.py` & `data_transformation_marta_miseke1-0.1.1a2/data_transformation_marta_miseke1/transformation.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,24 +34,23 @@
             list: The transposed matrix.
         """
         # Validate input_matrix
         for row in input_matrix:
             for element in row:
                 if not isinstance(element, float):
                     raise ValueError('Input matrix should contain only floats.')
-        if (min(len(item) for item in input_matrix) !=
-                max(len(item) for item in input_matrix)):
+        if (min(len(row) for row in input_matrix) !=
+                max(len(row) for row in input_matrix)):
             raise ValueError('Input matrix is not 2D matrix, rows has different'
                              ' number of elements')
         my_logger = DataTransformation.setup_logging()
         my_logger.info(f'Provided input matrix:{input_matrix}')
-        # Transpose input_matrix
         try:
             transposed_matrix = []
-            a = min(len(item) for item in input_matrix)
+            a = min(len(row) for row in input_matrix)
             b = len(input_matrix)
             i = 0
             while i != a:
                 j = 0
                 tranposed_line = []
                 while j != b:
                     tranposed_line.append(input_matrix[j][i])
@@ -81,25 +80,25 @@
         """
         # Validate input_array
         if not isinstance(input_array, np.ndarray):
             raise ValueError('Input must be a NumPy array')
         try:
             window_matrix = []
             a = len(input_array)
-            j = 0
             if size > a or stride > a or shift > a:
-                raise ValueError('Defined size or stride is larger than the '
-                                 'provided input array')
+                raise ValueError('Defined size or stride or shift is larger than'
+                                 ' the provided input array')
             else:
+                j = 0
                 while j <= size:
                     shifted = input_array[j:]
                     if len(shifted) >= size:
                         strided = shifted[stride-1::stride]
                         sized = strided[:size]
-                        if len(sized) >= size:
+                        if len(sized) == size:
                             window_matrix.append(sized)
                         j += shift
             my_logger = DataTransformation.setup_logging()
             my_logger.info(f'Sliding window: {window_matrix}')
             return np.array(window_matrix)
         except Exception as e:
             my_logger.error(f'Error during creation of sliding window: {e}')
```

### Comparing `data_transformation_marta_miseke1-0.1.1a0/pyproject.toml` & `data_transformation_marta_miseke1-0.1.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-transformation-marta-miseke1"
-version = "0.1.1a0"
+version = "0.1.1a2"
 description = ""
 authors = ["Marta <marta.miseke@seb.se>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.11"
 numpy = "~1.26.4"
```

