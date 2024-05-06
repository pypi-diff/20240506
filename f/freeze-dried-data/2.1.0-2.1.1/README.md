# Comparing `tmp/freeze_dried_data-2.1.0.tar.gz` & `tmp/freeze_dried_data-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeze_dried_data-2.1.0.tar", last modified: Sun May  5 08:24:48 2024, max compression
+gzip compressed data, was "freeze_dried_data-2.1.1.tar", last modified: Mon May  6 05:58:18 2024, max compression
```

## Comparing `freeze_dried_data-2.1.0.tar` & `freeze_dried_data-2.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-05-05 08:24:48.741749 freeze_dried_data-2.1.0/
--rw-rw-r--   0 tstand    (1000) tstand    (1000)     1072 2024-04-20 05:46:27.000000 freeze_dried_data-2.1.0/LICENSE
--rw-rw-r--   0 tstand    (1000) tstand    (1000)    11553 2024-05-05 08:24:48.741749 freeze_dried_data-2.1.0/PKG-INFO
--rw-rw-r--   0 tstand    (1000) tstand    (1000)    10686 2024-05-05 08:14:55.000000 freeze_dried_data-2.1.0/README.md
-drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-05-05 08:24:48.741749 freeze_dried_data-2.1.0/freeze_dried_data/
--rw-rw-r--   0 tstand    (1000) tstand    (1000)       33 2024-04-22 05:32:31.000000 freeze_dried_data-2.1.0/freeze_dried_data/__init__.py
--rw-rw-r--   0 tstand    (1000) tstand    (1000)    28265 2024-05-05 06:11:45.000000 freeze_dried_data-2.1.0/freeze_dried_data/freeze_dried_data.py
--rw-rw-r--   0 tstand    (1000) tstand    (1000)    11613 2024-04-20 05:48:25.000000 freeze_dried_data-2.1.0/freeze_dried_data/freeze_dried_data_old.py
--rw-rw-r--   0 tstand    (1000) tstand    (1000)    38572 2024-05-05 07:52:42.000000 freeze_dried_data-2.1.0/freeze_dried_data/test_freeze_dried_data.py
--rw-rw-r--   0 tstand    (1000) tstand    (1000)     7982 2024-04-22 05:32:19.000000 freeze_dried_data-2.1.0/freeze_dried_data/test_freeze_dried_data_old.py
-drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-05-05 08:24:48.741749 freeze_dried_data-2.1.0/freeze_dried_data.egg-info/
--rw-rw-r--   0 tstand    (1000) tstand    (1000)    11553 2024-05-05 08:24:48.000000 freeze_dried_data-2.1.0/freeze_dried_data.egg-info/PKG-INFO
--rw-rw-r--   0 tstand    (1000) tstand    (1000)      394 2024-05-05 08:24:48.000000 freeze_dried_data-2.1.0/freeze_dried_data.egg-info/SOURCES.txt
--rw-rw-r--   0 tstand    (1000) tstand    (1000)        1 2024-05-05 08:24:48.000000 freeze_dried_data-2.1.0/freeze_dried_data.egg-info/dependency_links.txt
--rw-rw-r--   0 tstand    (1000) tstand    (1000)       18 2024-05-05 08:24:48.000000 freeze_dried_data-2.1.0/freeze_dried_data.egg-info/top_level.txt
--rw-rw-r--   0 tstand    (1000) tstand    (1000)       38 2024-05-05 08:24:48.741749 freeze_dried_data-2.1.0/setup.cfg
--rw-rw-r--   0 tstand    (1000) tstand    (1000)     1125 2024-05-05 08:14:55.000000 freeze_dried_data-2.1.0/setup.py
+drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-05-06 05:58:18.243287 freeze_dried_data-2.1.1/
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)     1072 2024-04-20 05:46:27.000000 freeze_dried_data-2.1.1/LICENSE
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)    11553 2024-05-06 05:58:18.243287 freeze_dried_data-2.1.1/PKG-INFO
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)    10686 2024-05-05 08:14:55.000000 freeze_dried_data-2.1.1/README.md
+drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-05-06 05:58:18.243287 freeze_dried_data-2.1.1/freeze_dried_data/
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)       33 2024-04-22 05:32:31.000000 freeze_dried_data-2.1.1/freeze_dried_data/__init__.py
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)    30126 2024-05-06 05:44:32.000000 freeze_dried_data-2.1.1/freeze_dried_data/freeze_dried_data.py
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)    11613 2024-04-20 05:48:25.000000 freeze_dried_data-2.1.1/freeze_dried_data/freeze_dried_data_old.py
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)    40064 2024-05-06 05:50:10.000000 freeze_dried_data-2.1.1/freeze_dried_data/test_freeze_dried_data.py
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)     7982 2024-04-22 05:32:19.000000 freeze_dried_data-2.1.1/freeze_dried_data/test_freeze_dried_data_old.py
+drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-05-06 05:58:18.243287 freeze_dried_data-2.1.1/freeze_dried_data.egg-info/
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)    11553 2024-05-06 05:58:18.000000 freeze_dried_data-2.1.1/freeze_dried_data.egg-info/PKG-INFO
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)      394 2024-05-06 05:58:18.000000 freeze_dried_data-2.1.1/freeze_dried_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)        1 2024-05-06 05:58:18.000000 freeze_dried_data-2.1.1/freeze_dried_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)       18 2024-05-06 05:58:18.000000 freeze_dried_data-2.1.1/freeze_dried_data.egg-info/top_level.txt
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)       38 2024-05-06 05:58:18.243287 freeze_dried_data-2.1.1/setup.cfg
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)     1125 2024-05-06 05:56:21.000000 freeze_dried_data-2.1.1/setup.py
```

### Comparing `freeze_dried_data-2.1.0/LICENSE` & `freeze_dried_data-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.1.0/PKG-INFO` & `freeze_dried_data-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeze_dried_data
-Version: 2.1.0
+Version: 2.1.1
 Summary: A simple format for machine learning datasets
 Home-page: https://github.com/tstandley/freeze_dried_data
 Author: Trevor Standley
 Author-email: trevor.standley@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `freeze_dried_data-2.1.0/README.md` & `freeze_dried_data-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.1.0/freeze_dried_data/freeze_dried_data.py` & `freeze_dried_data-2.1.1/freeze_dried_data/freeze_dried_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -622,18 +622,14 @@
         self.custom_properties = new_custom_properties
         
 
         self.unfinished_setters = {}
 
         self.file.seek(earliest)
 
-
-        
-
-
     def close(self) -> None:
         """
         Close the WFDD and write data to disk.
         """
         # write out all unfinished setters
         cpy = list(self.unfinished_setters.keys())
         if len(cpy) > 1000:
@@ -733,7 +729,61 @@
         """
         Sets the value of the column with the specified name.
 
         :param key: The name of the column.
         :param value: The value to set.
         """
         self.__setattr__(key, value)
+
+
+def add_column(input_path, output_path, column_name, column_data, overwrite=False, column_serialize=pkl.dumps):
+    """
+    Add a column to a freeze-dried data file.
+
+    :param input_path: The path to the input freeze-dried data file.
+    :param output_path: The path to the output freeze-dried data file.
+    :param column_name: The name of the column to add.
+    :param column_data: The data for the column.
+    """
+    
+    # if it has an items() funciton, call it
+    if hasattr(column_data, 'items'):
+        column_data = column_data.items()
+
+    with RFDD(input_path) as rfdd:
+        if column_name in rfdd.columns:
+            raise ValueError("Column already exists.", column_name)
+
+        new_columns = list(rfdd.columns) + [column_name]
+        with WFDD(output_path, columns=new_columns, overwrite=overwrite) as wfdd:
+            
+            for key, value in column_data:
+                row_index = rfdd.index[key]
+                start, end = row_index[0], row_index[-1]
+
+                row_data = rfdd.read_chunk(start, end)
+
+                new_data_for_row = column_serialize(value)
+                current_index = list(row_index)
+                current_index.append(end+len(row_data))
+
+                start = wfdd.file.tell()
+
+                current_index = [i-current_index[0]+start for i in current_index]
+
+                wfdd.index[key] = tuple(current_index)
+
+                row_data+=new_data_for_row
+                wfdd.file.write(row_data)
+
+            # copy the splits
+            rfdd.get_available_splits()
+            for split in rfdd.get_available_splits():
+                rfdd.load_new_split(split)
+                rows = list(rfdd.index.keys())
+                wfdd.make_split(split, rows)
+
+            for k in rfdd.custom_properties.keys():
+                v = rfdd.__getattr__(k)
+                wfdd.__setattr__(k, v)
+
+
```

### Comparing `freeze_dried_data-2.1.0/freeze_dried_data/freeze_dried_data_old.py` & `freeze_dried_data-2.1.1/freeze_dried_data/freeze_dried_data_old.py`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.1.0/freeze_dried_data/test_freeze_dried_data.py` & `freeze_dried_data-2.1.1/freeze_dried_data/test_freeze_dried_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 import os
 import unittest
 import random
-from freeze_dried_data import RFDD, WFDD
+from freeze_dried_data import RFDD, WFDD, add_column
 
 class TestFDD(unittest.TestCase):
     test_file = '/tmp/test_fdd.fdd'
     test_file2 = '/tmp/test_fdd2.fdd'
-    compression_type = 'none'  # Can be updated for each test subclass
+    test_file3 = '/tmp/test_fdd3.fdd'
+    test_file4 = '/tmp/test_fdd4.fdd'
 
     def setUp(self):
         if os.path.exists(self.test_file):
             os.remove(self.test_file)
         if os.path.exists(self.test_file2):
             os.remove(self.test_file2)
+        # if os.path.exists(self.test_file3):
+        #     os.remove(self.test_file3)
+        # if os.path.exists(self.test_file4):
+        #     os.remove(self.test_file4)
 
     def tearDown(self):
         if os.path.exists(self.test_file):
             os.remove(self.test_file)
         if os.path.exists(self.test_file2):
             os.remove(self.test_file2)
+        # if os.path.exists(self.test_file3):
+        #     os.remove(self.test_file3)
+        # if os.path.exists(self.test_file4):
+        #     os.remove(self.test_file4)
 
     def test_basic_operations_no_columns(self):
         # Write operations
         with WFDD(self.test_file, overwrite=True) as wfdd:
             wfdd['hello'] = 'world'
             wfdd['number'] = 123
             
@@ -787,14 +796,48 @@
             wfdd['house3'] = ('house3', 300, 300000)
 
         with RFDD(self.test_file) as rfdd:
             self.assertEqual(rfdd['house1'].get_dict(), {'name': 'house1', 'area': 100, 'price': 100000})
             self.assertEqual(rfdd['house2'].get_dict(), {'name': 'house2', 'area': 200, 'price': 200000})
             self.assertEqual(rfdd['house3'].get_dict(), {'name': 'house3', 'area': 300, 'price': 300000})
 
+    def test_add_column(self):
+        
+        with WFDD(self.test_file, columns=('name','area'), overwrite=True) as wfdd:
+            for i in range(100):
+                wfdd[f'house_{i}'] = {'name': f'house_{i}', 'area': 100+10*i}
+
+            wfdd.custom_attribute1 = 'custom1'
+
+            wfdd.make_split('evens', [f'house_{i}' for i in range(0,100,2)])
+
+        new_col = {}
+        for i in range(100):
+            new_col[f'house_{i}'] = 1000+100*i
+        
+        
+        if os.path.exists(self.test_file3):
+            os.remove(self.test_file3)
+
+        add_column(self.test_file, self.test_file3, 'price', new_col)
+
+        with RFDD(self.test_file3) as rfdd:
+            for i in range(100):
+                self.assertEqual(rfdd[f'house_{i}'].price, 1000+100*i)
+
+            rfdd.load_new_split('evens')
+            for i in range(50):
+                self.assertEqual(rfdd[f'house_{2*i}'].price, 1000+200*i)
+
+            self.assertEqual(rfdd.custom_attribute1, 'custom1')
+
+        with self.assertRaises(ValueError):
+            add_column(self.test_file3, self.test_file4, 'price', new_col)
+
+            
 
     def test_dataloader_integration(self):
         from torch.utils.data import DataLoader, Dataset
 
         num_records = 100000
         data = {f'key{i}': (f'value{random.random()}', random.random()) for i in range(num_records)}
         with WFDD(self.test_file, overwrite=True) as wfdd:
@@ -852,14 +895,15 @@
             self.assertIsInstance(data[0], torch.Tensor)
             self.assertIsInstance(data[1], torch.Tensor)
             #assert that the tensors have the correct shape
             self.assertEqual(data[0].shape, (10,))
             self.assertEqual(data[1].shape, (10,))
 
         dataset.rfdd.close()
+
             
         
  
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `freeze_dried_data-2.1.0/freeze_dried_data/test_freeze_dried_data_old.py` & `freeze_dried_data-2.1.1/freeze_dried_data/test_freeze_dried_data_old.py`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.1.0/freeze_dried_data.egg-info/PKG-INFO` & `freeze_dried_data-2.1.1/freeze_dried_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeze-dried-data
-Version: 2.1.0
+Version: 2.1.1
 Summary: A simple format for machine learning datasets
 Home-page: https://github.com/tstandley/freeze_dried_data
 Author: Trevor Standley
 Author-email: trevor.standley@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `freeze_dried_data-2.1.0/setup.py` & `freeze_dried_data-2.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='freeze_dried_data',
-    version='2.1.0',
+    version='2.1.1',
     description='A simple format for machine learning datasets',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/tstandley/freeze_dried_data',
     author='Trevor Standley',
     author_email='trevor.standley@gmail.com',
     license='MIT',
```

