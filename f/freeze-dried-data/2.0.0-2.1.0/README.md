# Comparing `tmp/freeze_dried_data-2.0.0.tar.gz` & `tmp/freeze_dried_data-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeze_dried_data-2.0.0.tar", last modified: Mon Apr 22 17:01:34 2024, max compression
+gzip compressed data, was "freeze_dried_data-2.1.0.tar", last modified: Sun May  5 08:24:48 2024, max compression
```

## Comparing `freeze_dried_data-2.0.0.tar` & `freeze_dried_data-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 17:01:34.360234 freeze_dried_data-2.0.0/
--rw-r--r--   0 root         (0) root         (0)     1072 2024-04-22 17:00:59.000000 freeze_dried_data-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9078 2024-04-22 17:01:34.360234 freeze_dried_data-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8212 2024-04-22 17:00:59.000000 freeze_dried_data-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 17:01:34.356234 freeze_dried_data-2.0.0/freeze_dried_data/
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-22 17:00:59.000000 freeze_dried_data-2.0.0/freeze_dried_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23900 2024-04-22 17:00:59.000000 freeze_dried_data-2.0.0/freeze_dried_data/freeze_dried_data.py
--rw-r--r--   0 root         (0) root         (0)    11613 2024-04-22 17:00:59.000000 freeze_dried_data-2.0.0/freeze_dried_data/freeze_dried_data_old.py
--rw-r--r--   0 root         (0) root         (0)    31972 2024-04-22 17:00:59.000000 freeze_dried_data-2.0.0/freeze_dried_data/test_freeze_dried_data.py
--rw-r--r--   0 root         (0) root         (0)     7982 2024-04-22 17:00:59.000000 freeze_dried_data-2.0.0/freeze_dried_data/test_freeze_dried_data_old.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 17:01:34.356234 freeze_dried_data-2.0.0/freeze_dried_data.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9078 2024-04-22 17:01:34.000000 freeze_dried_data-2.0.0/freeze_dried_data.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      394 2024-04-22 17:01:34.000000 freeze_dried_data-2.0.0/freeze_dried_data.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 17:01:34.000000 freeze_dried_data-2.0.0/freeze_dried_data.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-22 17:01:34.000000 freeze_dried_data-2.0.0/freeze_dried_data.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 17:01:34.360234 freeze_dried_data-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-22 17:00:59.000000 freeze_dried_data-2.0.0/setup.py
+drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-05-05 08:24:48.741749 freeze_dried_data-2.1.0/
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)     1072 2024-04-20 05:46:27.000000 freeze_dried_data-2.1.0/LICENSE
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)    11553 2024-05-05 08:24:48.741749 freeze_dried_data-2.1.0/PKG-INFO
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)    10686 2024-05-05 08:14:55.000000 freeze_dried_data-2.1.0/README.md
+drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-05-05 08:24:48.741749 freeze_dried_data-2.1.0/freeze_dried_data/
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)       33 2024-04-22 05:32:31.000000 freeze_dried_data-2.1.0/freeze_dried_data/__init__.py
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)    28265 2024-05-05 06:11:45.000000 freeze_dried_data-2.1.0/freeze_dried_data/freeze_dried_data.py
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)    11613 2024-04-20 05:48:25.000000 freeze_dried_data-2.1.0/freeze_dried_data/freeze_dried_data_old.py
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)    38572 2024-05-05 07:52:42.000000 freeze_dried_data-2.1.0/freeze_dried_data/test_freeze_dried_data.py
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)     7982 2024-04-22 05:32:19.000000 freeze_dried_data-2.1.0/freeze_dried_data/test_freeze_dried_data_old.py
+drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-05-05 08:24:48.741749 freeze_dried_data-2.1.0/freeze_dried_data.egg-info/
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)    11553 2024-05-05 08:24:48.000000 freeze_dried_data-2.1.0/freeze_dried_data.egg-info/PKG-INFO
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)      394 2024-05-05 08:24:48.000000 freeze_dried_data-2.1.0/freeze_dried_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)        1 2024-05-05 08:24:48.000000 freeze_dried_data-2.1.0/freeze_dried_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)       18 2024-05-05 08:24:48.000000 freeze_dried_data-2.1.0/freeze_dried_data.egg-info/top_level.txt
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)       38 2024-05-05 08:24:48.741749 freeze_dried_data-2.1.0/setup.cfg
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)     1125 2024-05-05 08:14:55.000000 freeze_dried_data-2.1.0/setup.py
```

### Comparing `freeze_dried_data-2.0.0/LICENSE` & `freeze_dried_data-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.0.0/PKG-INFO` & `freeze_dried_data-2.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeze_dried_data
-Version: 2.0.0
+Version: 2.1.0
 Summary: A simple format for machine learning datasets
 Home-page: https://github.com/tstandley/freeze_dried_data
 Author: Trevor Standley
 Author-email: trevor.standley@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -17,19 +17,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Freeze Dried Data
-A robust format for machine learning datasets.
+A format for machine learning datasets.
 
-FDD allows your entire dataset to be a single file. Instances are only loaded from disk when needed and can be loaded in random order.
+FDD allows your entire dataset to be a single file while supporting fast random access to records on disk.
 
-Work with FDDs like you would python dictionaries. Keys map to objects. For extra organization and speed, columns can be defined where every row has a value for each column. 
+Work with FDDs like you would python dictionaries. Keys map to objects. For extra organization and speed, columns can be defined such that every row has a value for each column. 
 
 FDD files can operate in either read mode or write mode. Once a file is finalized, it cannot be modified without being re-written (i.e., it is "freeze-dried"). This allows for increased simplicity and speed compared to databases that allow modification.
 
 Values are written to disk immediately upon insertion, while keys are written as part of the index when the FDD file is closed.
 
 ## Installation
 ```bash
@@ -52,25 +52,28 @@
 If you key by hash, storing your train, val, and test sets in the same file can reduce the chance of having train/test or train/val overlap.
 
 Custom Splits also maintain order. This makes it easy to compare a ciriculum with random training for example.
 
 Splits also take the place of sharding in many cases. With one split per shard, only the index for the selected split is stored in memory. Everything else can remain on disk. And everything can still remain in a single file.
 
 ### Custom Serialization and Deserialization
-FDD allows custom functions for serializing and deserializing data. This flexibility is especially useful when dealing with complex data types or when performance optimizations are necessary. It also allows on-the-fly compression where the compression algorithm can be chosen on a per-column basis.
+FDD allows custom functions for serializing and deserializing data. This flexibility is especially useful when dealing with complex data types or when performance optimizations are necessary. It also allows on-the-fly compression where the compression algorithm can be chosen on a per-column basis. Finally, custom serialization can be much more efficient when storing tensors (numpy, pytorch, etc.)
 
 ### Custom Properties
 Custom properties are a great place to store dataset metadata such as dataset cards or the code/parameters used to generate the data. In read mode, properties are loaded from disk only when accessed, so this need not incur a runtime cost.
 
 ### Seamless Integration
-FDD is designed to work with data loaders in machine learning frameworks like PyTorch. Unlike other solutions, RFDD objects detect when they've been forked to a new process and re-open their files. 
+FDD is designed to work with data loaders in machine learning frameworks like PyTorch. Unlike other solutions, RFDD objects detect when they've been forked to a new process and re-open their file handles. 
 
 ### Context Management
 FDD supports Python’s context management (using `with` statements), which ensures that files are properly closed after operations are completed, preventing data corruption and resource leaks.
 
+### Easy Appending to Existing Files
+FDD supportes reopening existing files for writing. Reopened files retain all rows, custom properties, and splits already added to the file, while allowing new rows, properties, or splits to be written. Splits can also be modified.
+
 ## Examples
 
 ### Example 1: Creating an FDD File
 ```python
 from freeze_dried_data import WFDD
 
 # Create the file "new dataset.fdd"
@@ -80,14 +83,19 @@
 dataset['key1'] = 'value1'
 
 # Add the entry 1234: 5678 to the dataset and write the value to disk
 dataset[1234] = 5678
 
 # Write the index including all keys to disk and close the file
 dataset.close()
+
+# or use a with statement to ensure files are closed when finished
+with WFDD('new dataset.fdd', overwrite=True)
+    dataset['key1'] = 'value1'
+    dataset[1234] = 5678
 ```
 
 ### Example 2: Reading an FDD File
 ```python
 from freeze_dried_data import RFDD
 
 # Open the existing file and unpickle the index including all keys into memory
@@ -96,14 +104,24 @@
 # Print each key-value pair
 for k, v in dataset.items():
   print(k, v)
 
 # Directly access and print specific items
 print(dataset[1234])        # prints "5678"
 print(list(dataset.keys())) # prints "['key1', 1234]"
+
+dataset.close()
+
+# or using a with statement
+with RFDD('new dataset.fdd'):
+    for k, v in dataset.items():
+        print(k,v)
+    print(dataset[1234])
+    print(list(dataset.keys()))
+    
 ```
 
 ### Example 3: Creating a file with columns
 
 ```python
 from freeze_dried_data import WFDD
 
@@ -131,45 +149,74 @@
 ```
 
 ### Example 4: Reading a file with columns
 ```python
 from freeze_dried_data import RFDD
 
 with RFDD('text_dataset.fdd') as dataset:
-    for row in dataset:
-        print(row['text'], row['label']) 
+    print(dataset.columns)
+    for key, row in dataset.items():
+        print(row['text'], row['label'])
+        # or
+        print(row.text, row.label)
+        # or
+        print(row[0], row[1])
 
 # output:
+# ['text', 'label']
+# This is an example document. 1
+# This is an example document. 1
 # This is an example document. 1
 # Another document for classification. 0
+# Another document for classification. 0
+# Another document for classification. 0
+# A third document. 1
 # A third document. 1
+# A third document. 1
+# A fourth document. 0
 # A fourth document. 0
+# A fourth document. 0
+# A fifth document. None
 # A fifth document. None
+# A fifth document. None
+# A sixth document. None
+# A sixth document. None
 # A sixth document. None
 
 ```
 
-### Example 5: Using Custom Properties
+### Example 5: Using Custom Properties and Custom Splits
 ```python
 from freeze_dried_data import WFDD
 
 # Open a new FDD file, adding custom properties to store additional metadata
 with WFDD('dataset_with_properties.fdd') as dataset:
     dataset.creator = 'Data Scientist'
     dataset.creation_date = '2024-04-12'
     dataset.description = 'Sample dataset with custom properties.'
 
     # Add data to the dataset
-    dataset['key1'] = 'value1'
+    dataset['key1'] = 'train_data1'
+    dataset['key2'] = 'train_data2'
+    dataset['key3'] = 'train_data3'
+    dataset['key4'] = 'val_data1'
+    dataset['key5'] = 'val_data2'
+    dataset.make_split('train', ['key1', 'key2', 'key3'])
+    dataset.make_split('val', ['key4', 'key5'])
+
 
 # Verify and print custom properties
-with RFDD('dataset_with_properties.fdd') as loaded_dataset:
+with RFDD('dataset_with_properties.fdd', split='train') as loaded_dataset:
     print('Creator:', loaded_dataset.creator)
     print('Creation Date:', loaded_dataset.creation_date)
     print('Description:', loaded_dataset.description)
+    # train rows loaded into the index
+    dataset.load_new_split('val')
+    # val rows loaded into the index
+
 ```
 
 ### Example 6: Using custom Serialization
 ```python
 import json
 from freeze_dried_data import WFDD
 
@@ -186,45 +233,71 @@
     print(dataset['key1'])
 
 # outputs:
 # {'complex_data': [1, 2, 3]}
 
 ```
 
-### Example 7: Using in a PyTorch DataLoader with Workers
+### Example 7: File Reopening
+```python
+data = {f'key{i}': f'value{i}' for i in range(1000)}
+with WFDD('test_file.fdd', overwrite=True) as wfdd:
+    for k, v in data.items():
+        wfdd[k] = v
+
+    wfdd.custom_attribute1 = 'custom1'
+    wfdd.custom_attribute2 = 'custom2'
+    wfdd.make_split('evens', [f'key{i}' for i in range(0,1000,2)])
+
+data_2 = {f'key{i}': f'value{i}' for i in range(1000,2000)}
+with WFDD('test_file.fdd', reopen=True) as wfdd:
+    for k, v in data_2.items():
+        wfdd[k] = v
+    
+    wfdd.custom_attribute1 = 're-written custom1'
+    wfdd.custom_attribute3 = 'custom3'
+
+    wfdd.add_to_split('evens', [f'key{i}' for i in range(1000,2000,2)])
+    wfdd.make_split('odds', [f'key{i}' for i in range(1,2000,2)])
+
+# test_file.fdd now contains all 2k rows, both full splits, and all three attributes.
+```
+
+### Example 8: Using in a PyTorch DataLoader with Workers
 ```python
 import torch
 from torch.utils.data import Dataset, DataLoader
 from freeze_dried_data import WFDD
 
 with WFDD('new dataset.fdd') as dataset:
-    dataset.train_keys = ['key1', 'key2', 'key3']
-    dataset.val_keys = ['key4', 'key5']
+    
     dataset['key1'] = 'train_data1'
     dataset['key2'] = 'train_data2'
     dataset['key3'] = 'train_data3'
     dataset['key4'] = 'val_data1'
     dataset['key5'] = 'val_data2'
+    dataset.make_split('train', ['key1', 'key2', 'key3'])
+    dataset.make_split('val', ['key4', 'key5'])
 
 class FDDDataset(Dataset):
     def __init__(self, filename, split='train'):
-        self.fdd = RFDD(filename)
-        if split == 'train':
-            self.keys = self.fdd.train_keys
-        else:
-            self.keys = self.fdd.val_keys
+        self.fdd = RFDD(filename,split=split)
+        self.keys = list(self.fdd.keys())
     
     def __len__(self):
         return len(self.keys)
     
     def __getitem__(self, idx):
         key = self.keys[idx]
         return key, self.fdd[key]
 
 dataset = FDDDataset('new dataset.fdd', split='train')
+
+# Each worker gets a separate copy of the dataset object.
+# The file handles will be refreshed automatically.
 dataloader = DataLoader(dataset, batch_size=2, shuffle=True, num_workers=4)
 
 for key, value in dataloader:
     print(f'Batch: {key} - {value}')
 
 # Example output:
 # Batch: ('key3', 'key2') - ('train_data3', 'train_data2')
```

### Comparing `freeze_dried_data-2.0.0/README.md` & `freeze_dried_data-2.1.0/freeze_dried_data.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,35 @@
+Metadata-Version: 2.1
+Name: freeze-dried-data
+Version: 2.1.0
+Summary: A simple format for machine learning datasets
+Home-page: https://github.com/tstandley/freeze_dried_data
+Author: Trevor Standley
+Author-email: trevor.standley@gmail.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Freeze Dried Data
-A robust format for machine learning datasets.
+A format for machine learning datasets.
 
-FDD allows your entire dataset to be a single file. Instances are only loaded from disk when needed and can be loaded in random order.
+FDD allows your entire dataset to be a single file while supporting fast random access to records on disk.
 
-Work with FDDs like you would python dictionaries. Keys map to objects. For extra organization and speed, columns can be defined where every row has a value for each column. 
+Work with FDDs like you would python dictionaries. Keys map to objects. For extra organization and speed, columns can be defined such that every row has a value for each column. 
 
 FDD files can operate in either read mode or write mode. Once a file is finalized, it cannot be modified without being re-written (i.e., it is "freeze-dried"). This allows for increased simplicity and speed compared to databases that allow modification.
 
 Values are written to disk immediately upon insertion, while keys are written as part of the index when the FDD file is closed.
 
 ## Installation
 ```bash
@@ -30,25 +52,28 @@
 If you key by hash, storing your train, val, and test sets in the same file can reduce the chance of having train/test or train/val overlap.
 
 Custom Splits also maintain order. This makes it easy to compare a ciriculum with random training for example.
 
 Splits also take the place of sharding in many cases. With one split per shard, only the index for the selected split is stored in memory. Everything else can remain on disk. And everything can still remain in a single file.
 
 ### Custom Serialization and Deserialization
-FDD allows custom functions for serializing and deserializing data. This flexibility is especially useful when dealing with complex data types or when performance optimizations are necessary. It also allows on-the-fly compression where the compression algorithm can be chosen on a per-column basis.
+FDD allows custom functions for serializing and deserializing data. This flexibility is especially useful when dealing with complex data types or when performance optimizations are necessary. It also allows on-the-fly compression where the compression algorithm can be chosen on a per-column basis. Finally, custom serialization can be much more efficient when storing tensors (numpy, pytorch, etc.)
 
 ### Custom Properties
 Custom properties are a great place to store dataset metadata such as dataset cards or the code/parameters used to generate the data. In read mode, properties are loaded from disk only when accessed, so this need not incur a runtime cost.
 
 ### Seamless Integration
-FDD is designed to work with data loaders in machine learning frameworks like PyTorch. Unlike other solutions, RFDD objects detect when they've been forked to a new process and re-open their files. 
+FDD is designed to work with data loaders in machine learning frameworks like PyTorch. Unlike other solutions, RFDD objects detect when they've been forked to a new process and re-open their file handles. 
 
 ### Context Management
 FDD supports Python’s context management (using `with` statements), which ensures that files are properly closed after operations are completed, preventing data corruption and resource leaks.
 
+### Easy Appending to Existing Files
+FDD supportes reopening existing files for writing. Reopened files retain all rows, custom properties, and splits already added to the file, while allowing new rows, properties, or splits to be written. Splits can also be modified.
+
 ## Examples
 
 ### Example 1: Creating an FDD File
 ```python
 from freeze_dried_data import WFDD
 
 # Create the file "new dataset.fdd"
@@ -58,14 +83,19 @@
 dataset['key1'] = 'value1'
 
 # Add the entry 1234: 5678 to the dataset and write the value to disk
 dataset[1234] = 5678
 
 # Write the index including all keys to disk and close the file
 dataset.close()
+
+# or use a with statement to ensure files are closed when finished
+with WFDD('new dataset.fdd', overwrite=True)
+    dataset['key1'] = 'value1'
+    dataset[1234] = 5678
 ```
 
 ### Example 2: Reading an FDD File
 ```python
 from freeze_dried_data import RFDD
 
 # Open the existing file and unpickle the index including all keys into memory
@@ -74,14 +104,24 @@
 # Print each key-value pair
 for k, v in dataset.items():
   print(k, v)
 
 # Directly access and print specific items
 print(dataset[1234])        # prints "5678"
 print(list(dataset.keys())) # prints "['key1', 1234]"
+
+dataset.close()
+
+# or using a with statement
+with RFDD('new dataset.fdd'):
+    for k, v in dataset.items():
+        print(k,v)
+    print(dataset[1234])
+    print(list(dataset.keys()))
+    
 ```
 
 ### Example 3: Creating a file with columns
 
 ```python
 from freeze_dried_data import WFDD
 
@@ -109,45 +149,74 @@
 ```
 
 ### Example 4: Reading a file with columns
 ```python
 from freeze_dried_data import RFDD
 
 with RFDD('text_dataset.fdd') as dataset:
-    for row in dataset:
-        print(row['text'], row['label']) 
+    print(dataset.columns)
+    for key, row in dataset.items():
+        print(row['text'], row['label'])
+        # or
+        print(row.text, row.label)
+        # or
+        print(row[0], row[1])
 
 # output:
+# ['text', 'label']
+# This is an example document. 1
 # This is an example document. 1
+# This is an example document. 1
+# Another document for classification. 0
+# Another document for classification. 0
 # Another document for classification. 0
 # A third document. 1
+# A third document. 1
+# A third document. 1
 # A fourth document. 0
+# A fourth document. 0
+# A fourth document. 0
+# A fifth document. None
+# A fifth document. None
 # A fifth document. None
 # A sixth document. None
+# A sixth document. None
+# A sixth document. None
 
 ```
 
-### Example 5: Using Custom Properties
+### Example 5: Using Custom Properties and Custom Splits
 ```python
 from freeze_dried_data import WFDD
 
 # Open a new FDD file, adding custom properties to store additional metadata
 with WFDD('dataset_with_properties.fdd') as dataset:
     dataset.creator = 'Data Scientist'
     dataset.creation_date = '2024-04-12'
     dataset.description = 'Sample dataset with custom properties.'
 
     # Add data to the dataset
-    dataset['key1'] = 'value1'
+    dataset['key1'] = 'train_data1'
+    dataset['key2'] = 'train_data2'
+    dataset['key3'] = 'train_data3'
+    dataset['key4'] = 'val_data1'
+    dataset['key5'] = 'val_data2'
+    dataset.make_split('train', ['key1', 'key2', 'key3'])
+    dataset.make_split('val', ['key4', 'key5'])
+
 
 # Verify and print custom properties
-with RFDD('dataset_with_properties.fdd') as loaded_dataset:
+with RFDD('dataset_with_properties.fdd', split='train') as loaded_dataset:
     print('Creator:', loaded_dataset.creator)
     print('Creation Date:', loaded_dataset.creation_date)
     print('Description:', loaded_dataset.description)
+    # train rows loaded into the index
+    dataset.load_new_split('val')
+    # val rows loaded into the index
+
 ```
 
 ### Example 6: Using custom Serialization
 ```python
 import json
 from freeze_dried_data import WFDD
 
@@ -164,45 +233,71 @@
     print(dataset['key1'])
 
 # outputs:
 # {'complex_data': [1, 2, 3]}
 
 ```
 
-### Example 7: Using in a PyTorch DataLoader with Workers
+### Example 7: File Reopening
+```python
+data = {f'key{i}': f'value{i}' for i in range(1000)}
+with WFDD('test_file.fdd', overwrite=True) as wfdd:
+    for k, v in data.items():
+        wfdd[k] = v
+
+    wfdd.custom_attribute1 = 'custom1'
+    wfdd.custom_attribute2 = 'custom2'
+    wfdd.make_split('evens', [f'key{i}' for i in range(0,1000,2)])
+
+data_2 = {f'key{i}': f'value{i}' for i in range(1000,2000)}
+with WFDD('test_file.fdd', reopen=True) as wfdd:
+    for k, v in data_2.items():
+        wfdd[k] = v
+    
+    wfdd.custom_attribute1 = 're-written custom1'
+    wfdd.custom_attribute3 = 'custom3'
+
+    wfdd.add_to_split('evens', [f'key{i}' for i in range(1000,2000,2)])
+    wfdd.make_split('odds', [f'key{i}' for i in range(1,2000,2)])
+
+# test_file.fdd now contains all 2k rows, both full splits, and all three attributes.
+```
+
+### Example 8: Using in a PyTorch DataLoader with Workers
 ```python
 import torch
 from torch.utils.data import Dataset, DataLoader
 from freeze_dried_data import WFDD
 
 with WFDD('new dataset.fdd') as dataset:
-    dataset.train_keys = ['key1', 'key2', 'key3']
-    dataset.val_keys = ['key4', 'key5']
+    
     dataset['key1'] = 'train_data1'
     dataset['key2'] = 'train_data2'
     dataset['key3'] = 'train_data3'
     dataset['key4'] = 'val_data1'
     dataset['key5'] = 'val_data2'
+    dataset.make_split('train', ['key1', 'key2', 'key3'])
+    dataset.make_split('val', ['key4', 'key5'])
 
 class FDDDataset(Dataset):
     def __init__(self, filename, split='train'):
-        self.fdd = RFDD(filename)
-        if split == 'train':
-            self.keys = self.fdd.train_keys
-        else:
-            self.keys = self.fdd.val_keys
+        self.fdd = RFDD(filename,split=split)
+        self.keys = list(self.fdd.keys())
     
     def __len__(self):
         return len(self.keys)
     
     def __getitem__(self, idx):
         key = self.keys[idx]
         return key, self.fdd[key]
 
 dataset = FDDDataset('new dataset.fdd', split='train')
+
+# Each worker gets a separate copy of the dataset object.
+# The file handles will be refreshed automatically.
 dataloader = DataLoader(dataset, batch_size=2, shuffle=True, num_workers=4)
 
 for key, value in dataloader:
     print(f'Batch: {key} - {value}')
 
 # Example output:
 # Batch: ('key3', 'key2') - ('train_data3', 'train_data2')
```

### Comparing `freeze_dried_data-2.0.0/freeze_dried_data/freeze_dried_data.py` & `freeze_dried_data-2.1.0/freeze_dried_data/freeze_dried_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,14 +185,20 @@
         :param split: The name of the split to load.
         """
         if split not in self.split_to_index:
             raise KeyError("Split not found.", split)
         
         start, end = self.split_to_index[split]
         self.index = self.system_deserialize(self.read_chunk(start, end))
+
+    def get_available_splits(self) -> List[str]:
+        """
+        :return: A list of available splits.
+        """
+        return list(self.split_to_index.keys())
         
 
     def load_indices(self, split: str = 'all_rows') -> None:
         """
         Reads from the end of the file loading custom properties, columns, and the split index.
 
         :param split: The split to load, defaults to 
@@ -258,14 +264,20 @@
     """
 
     def __init__(self, index: Tuple[Any], parent, ) -> None:
         self._fdd_row_index = index
         self._fdd_row_parent = parent
         self._fdd_row_cache = [None for _ in range(len(self._fdd_row_index) - 1)]
 
+    def get_dict(self):
+        """
+        :return: A dictionary representation of the row.
+        """
+        return {k: self[i] for i, k in enumerate(self._fdd_row_parent.columns)}
+    
     def __getitem__(self, key: int | str) -> Any:
         """
         Gets the value of the column at the specified index or with the specified name.
 
         :param key: The index of the column, or the name of the column.
         :return: The value of the column.
         """
@@ -321,20 +333,21 @@
         :param name: The name of the column.
         :param value: The value to set.
         :raises AttributeError: If the column is not found.
         """
         if name.startswith('_fdd_row_'):
             super().__setattr__(name, value)
             return
-        
+        if isinstance(self._fdd_row_parent, WFDD):
+            raise AttributeError("Row has already been finalized.")
         columns = self._fdd_row_parent.columns
         if name not in columns:
             raise AttributeError(f"Column not found: {name}")
         
-        index = columns[name]
+        index = columns[name] if isinstance(columns, dict) else columns.index(name)
         self._fdd_row_cache[index] = value
     
     def __repr__(self) -> str:
         """
         :return: A human readable string representation of the row. One line per column.
         """
         rep = ""
@@ -359,47 +372,58 @@
         when reading back data that was written with a custom serializer.
 
     """
     def __init__(self,
                  filename: str,
                  columns: Tuple[str] = None,
                  overwrite: bool = False,
+                 reopen: bool = False,
                  system_serialize: callable = pkl.dumps,
+                 system_deserialize: callable = pkl.loads,
                  no_columns_serialize: callable = pkl.dumps,
                  column_to_serialize: tuple[callable] = None,
                  no_columns_deserialize: callable = pkl.loads,
                  column_to_deserialize: tuple[callable] = None) -> None:
         self.__dict__['_initializing'] = True # Use self.__dict__ to bypass __setattr__
         super().__init__(filename)
-        if not overwrite and os.path.exists(filename):
+        
+        if not overwrite and not reopen and os.path.exists(filename):
             raise FileExistsError("File already exists.", filename)
         
+        if reopen and not os.path.exists(filename):
+            raise FileNotFoundError("File not found.", filename)
+        
+
+        
 
         if columns is not None:
             if column_to_deserialize is None:
                 self.column_to_deserialize = tuple(pkl.loads for i in range(len(columns)))
             else:
                 self.column_to_deserialize = column_to_deserialize
             if column_to_serialize is None:
                 self.column_to_serialize = tuple(system_serialize for i in range(len(columns)))
             else:
                 self.column_to_serialize = column_to_serialize
         
         
         self.system_serialize = system_serialize
+        self.system_deserialize = system_deserialize
         self.no_columns_serialize = no_columns_serialize
         self.no_columns_deserialize = no_columns_deserialize
 
-        
-        self.file = open(filename, 'wb+')
-        self.unfinished_setters = {}
-        self.index = {}
-        self.columns = columns
-        self.custom_properties = {}
-        self.split_to_index = {}
+        if reopen:
+            self.reopen()
+        else:
+            self.file = open(filename, 'wb+')
+            self.unfinished_setters = {}
+            self.index = {}
+            self.columns = columns
+            self.custom_properties = {}
+            self.split_to_index = {}
         
         self._initializing = False
 
     def __setattr__(self, name: str, value: Any) -> None:
         """
         Set an attribute value.
 
@@ -453,15 +477,17 @@
         else:
             if self.columns is None:
                 start,end = self.index[key]
                 data = self.read_chunk(start, end)
                 return self.no_columns_deserialize(data)
         
         pos = self.file.tell()
-        row = FDDReadRow(self.index[key], self)
+        #TODO: investigate, I think read-row needs to know where to seek after it does the reading.
+        #the tests do check to make sure this works though.
+        row = FDDReadRow(self.index[key], self) 
         self.file.seek(pos)
         return row
         
     def __setitem__(self, key: Any, item: dict[str, Any] | tuple[Any] | FDDReadRow | Any) -> None:
         """
         Set an item in the WFDD.
 
@@ -484,15 +510,17 @@
                     data = item._fdd_row_parent.read_chunk(item._fdd_row_index[i], item._fdd_row_index[i+1])
                 self.file.write(data)
                 positions.append(self.file.tell())
             self.index[key] = tuple(positions)
             return
         elif isinstance(item, dict):
             if all(col not in item for col in self.columns):
-                raise ValueError("Dict contains no entries for columns.")
+                raise ValueError("Dict contains no entries for columns.", [col for col in self.columns if col not in item])
+            if any(col not in self.columns for col in item):
+                raise ValueError("Dict contains columns not in the column list.", [col for col in item if col not in self.columns])
             item = tuple(item.get(col) for col in self.columns)
         elif isinstance(item, tuple):
             if len(item) != len(self.columns):
                 raise ValueError("Incorrect number of columns.")
             #if it has all attributes in our columns
         elif all(hasattr(item, col) for col in self.columns):
             item = tuple(getattr(item, col) for col in self.columns)
@@ -506,31 +534,106 @@
                     serialize = self.column_to_serialize[i]
                 else:
                     serialize = self.no_columns_serialize
                 data = serialize(v)
                 self.file.write(data)
             positions.append(self.file.tell())
             
-        self.index[key] = tuple(positions)
+        self.index[key] = tuple(positions)    
 
-    def make_split(self, split: str, rows: list) -> None:
+    def make_split(self, split: str, rows: list | tuple | set | frozenset, overwrite=False) -> None:
         """
         Create a split in the WFDD.
 
         :param split: The name of the split.
-        :param rows: The list of keys for the split.
+        :param rows: The iterable of keys for the split.
+        """
+        if split in self.split_to_index and not overwrite:
+            raise ValueError("Split already exists.", split, 'Use overwrite=True to overwrite it.')
+        
+        if isinstance(rows, (list, tuple, set, frozenset)):
+            self.split_to_index[split] = {key: self.index[key] for key in rows}
+        else:
+            raise ValueError("Rows must be an iterable of keys.")
+        
+    def add_to_split(self, split: str, rows: list | tuple | set | frozenset) -> None:
+        """
+        Add rows to a split in the WFDD.
+
+        :param split: The name of the split.
+        :param rows: The iterable of keys for the split.
         """
-        if split in self.split_to_index:
-            raise ValueError("Split already exists.", split)
+        if split not in self.split_to_index:
+            raise ValueError("Split not found.", split)
+        
+        if isinstance(rows, (list, tuple, set, frozenset)):
+            self.split_to_index[split].update({key: self.index[key] for key in rows})
+        else:
+            raise ValueError("Rows must be an iterable of keys.")
+        
+    def reopen(self) -> None:
+        self.file = open(self.filename, 'rb+')
+        self.file.seek(-8, 2)
+        index_index_size = int.from_bytes(self.file.read(8), 'little')
+
+        self.file.seek(-(8 + index_index_size), 2)
+        index_index_data = self.file.read(index_index_size)
+        index_index = self.system_deserialize(index_index_data)
+        
+        self.split_to_index = {k[7:]:v for k,v in index_index.items() if k.startswith('_split_')}
         
-        if isinstance(rows, list):
-            self.split_to_index[split] = {key:self.index[key] for key in rows}
+
+        # remove splits from index_index
+        for k in self.split_to_index:
+            index_index.pop('_split_'+k)
+
+        index_start, index_end = self.split_to_index["all_rows"]
+        
+        self.index = self.system_deserialize(self.read_chunk(index_start, index_end))
+
+        new_split_to_index = {}
+        for k,v in self.split_to_index.items():
+            if k == "all_rows":
+                continue
+            split_start, split_end = v
+            new_split_to_index[k] = self.system_deserialize(self.read_chunk(split_start, split_end))
+
+        self.split_to_index = new_split_to_index
+        
+        if '_columns_' not in index_index:
+            self.columns = None
         else:
-            raise ValueError("Rows must be a list of keys.")
+            columns_start, columns_end = index_index['_columns_']
+            index_index.pop('_columns_')
+
+            self.columns = self.system_deserialize(self.read_chunk(columns_start, columns_end))
+            
+                
+
+        self.custom_properties = {k[6:]:v for k,v in index_index.items() if k.startswith('_prop_')}
         
+        # need to figure out where to seek so that we are at the end of the rows. Everything else shoudl be in ram.
+        earliest = 9e99
+        new_custom_properties = {}
+        for k,v in self.custom_properties.items():
+            prop_start, prop_end = v
+            if prop_start < earliest:
+                earliest = prop_start
+            new_custom_properties[k] = self.system_deserialize(self.read_chunk(prop_start, prop_end))
+        self.custom_properties = new_custom_properties
+        
+
+        self.unfinished_setters = {}
+
+        self.file.seek(earliest)
+
+
+        
+
+
     def close(self) -> None:
         """
         Close the WFDD and write data to disk.
         """
         # write out all unfinished setters
         cpy = list(self.unfinished_setters.keys())
         if len(cpy) > 1000:
@@ -590,33 +693,38 @@
     :param parent: The parent object that holds the data.
     :param key: The key used to identify the data in the parent object.
     """
     def __init__(self, parent: 'WFDD', key: Any) -> None:
         self._fdd_setter_parent = parent
         self._fdd_setter_key = key
         self._fdd_setter_data = {}
+        self._fdd_setter_finalized = False
 
     def finalize(self) -> None:
         """
         Finalizes the data setting process by updating the parent object and removing the setter from the unfinished setters list.
         """
         self._fdd_setter_parent[self._fdd_setter_key] = self._fdd_setter_data
         del self._fdd_setter_parent.unfinished_setters[self._fdd_setter_key]
-
+        self._fdd_setter_finalized = True
+    
     def __setattr__(self, name: str, value: Any) -> None:
         """
         Sets the appropriate column in the row. Coluns aren't written to disk until the row is finalized.
         Rows are finalized when all columns are set, when finalize() is called, or when the WFDD is closed.
 
 
         """
         if name.startswith('_fdd_setter_'):
             super().__setattr__(name, value)
             return
         
+        if self._fdd_setter_finalized:
+            raise AttributeError("Row has already been finalized.")
+        
         columns = self._fdd_setter_parent.columns
         if name not in columns:
             raise AttributeError(f"Column not found: {name}")
         
         self._fdd_setter_data[name] = value
         if len(self._fdd_setter_data) == len(self._fdd_setter_parent.columns):
             self.finalize()
```

### Comparing `freeze_dried_data-2.0.0/freeze_dried_data/freeze_dried_data_old.py` & `freeze_dried_data-2.1.0/freeze_dried_data/freeze_dried_data_old.py`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.0.0/freeze_dried_data/test_freeze_dried_data.py` & `freeze_dried_data-2.1.0/freeze_dried_data/test_freeze_dried_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -339,14 +339,15 @@
             with self.assertRaises(ValueError):
                 wfdd.make_split('odds', [f'house_{i}' for i in range(1,100,2)])
             with self.assertRaises(ValueError):
                 wfdd.make_split('wrong', 'not_a_list')
 
         with RFDD(self.test_file, split='odds') as rfdd:
             self.assertEqual(len(list(rfdd.keys())), 50)
+            self.assertEqual(rfdd.get_available_splits(), ['odds', 'evens', 'big houses', 'reverse_order', 'all_rows'])
             for i, (k,v) in enumerate(rfdd.items()):
                 self.assertEqual(k, f'house_{2*i+1}')
                 self.assertEqual(v.name, f'house_{2*i+1}')
                 self.assertEqual(v.area, 110+20*i)
                 self.assertEqual(v.price, 1100+200*i)
 
             rfdd.load_new_split('evens')
@@ -636,29 +637,164 @@
             ptr = tensor.data_ptr()
             num_bytes = tensor.nelement() * tensor.element_size()
             buffer = (ctypes.c_char * num_bytes).from_address(ptr)
             return bytes(buffer)
         
         
         def bytes_to_tensor(byte_data, shape=(10,10)):
-            tensor = torch.frombuffer(byte_data, dtype=torch.bfloat16)
+            byte_data = bytearray(byte_data)
+            tensor = torch.frombuffer(byte_data, dtype=torch.bfloat16, )
             return tensor.view(shape)
         
         for custom_serialize, custom_deserialize in zip(custom_serialize_list, custom_deserialize_list):
             with WFDD(self.test_file, overwrite=True, columns=('hash', 'tensor', 'label'),system_serialize=custom_serialize, column_to_serialize=(pkl.dumps,tensor_to_bytes,pkl.dumps)) as wfdd:
                 for k,v in data.items():
                     wfdd[k] = v
 
             with RFDD(self.test_file, system_deserialize=custom_deserialize, column_to_deserialize=(pkl.loads,bytes_to_tensor,pkl.loads)) as rfdd:
                 for k,v in data.items():
                     self.assertEqual(rfdd[k].hash, v['hash'])
                     self.assertTrue(torch.allclose(rfdd[k].tensor, v['tensor']))
                     self.assertEqual(rfdd[k].label, v['label'])
 
-        
+    def test_row_has_already_been_finalized(self):
+        with WFDD(self.test_file,columns=('col1','col2'),overwrite=True) as wfdd:
+            wfdd['key1'].col1 = 1
+            wfdd['key1'].col2 = 2
+            with self.assertRaises(AttributeError):
+                wfdd['key1'].col1 = 3
+
+    def test_reopen_file(self):
+        data = {f'key{i}': f'value{i}' for i in range(1000)}
+        with WFDD(self.test_file, overwrite=True) as wfdd:
+            for k, v in data.items():
+                wfdd[k] = v
+
+            wfdd.custom_attribute1 = 'custom1'
+            wfdd.custom_attribute2 = 'custom2'
+            wfdd.make_split('evens', [f'key{i}' for i in range(0,1000,2)])
+        with RFDD(self.test_file) as rfdd:
+            for k,v in data.items():
+                self.assertEqual(rfdd[k], v)
+            rfdd.load_new_split('evens')
+            self.assertEqual(len(list(rfdd.keys())), 500)
+            for i, (k,v) in enumerate(rfdd.items()):
+                self.assertEqual(k, f'key{2*i}')
+                self.assertEqual(v, f'value{2*i}')
+
+        data_2 = {f'key{i}': f'value{i}' for i in range(1000,2000)}
+        with WFDD(self.test_file, reopen=True) as wfdd:
+
+            for k, v in data_2.items():
+                wfdd[k] = v
+            
+            wfdd.custom_attribute1 = 're-written custom1'
+            wfdd.custom_attribute3 = 'custom3'
+            wfdd.add_to_split('evens', [f'key{i}' for i in range(1000,2000,2)])
+            with self.assertRaises(ValueError):
+                wfdd.add_to_split('fake_split', ['key1'])
+            with self.assertRaises(ValueError):
+                wfdd.add_to_split('evens', 234234)
+            wfdd.make_split('odds', [f'key{i}' for i in range(1,2000,2)])
+
+        with self.assertRaises(FileNotFoundError):
+            WFDD('fake_file_doesnt_exist', reopen=True)
+
+        with RFDD(self.test_file) as rfdd:
+            for k,v in data.items():
+                self.assertEqual(rfdd[k], v)
+            for k,v in data_2.items():
+                self.assertEqual(rfdd[k], v)
+
+            rfdd.load_new_split('evens')
+            self.assertEqual(len(list(rfdd.keys())), 1000)
+            for i, (k,v) in enumerate(rfdd.items()):
+                self.assertEqual(k, f'key{2*i}')
+                self.assertEqual(v, f'value{2*i}')
+
+            rfdd.load_new_split('odds')
+            self.assertEqual(len(list(rfdd.keys())), 1000)
+            for i, (k,v) in enumerate(rfdd.items()):
+                self.assertEqual(k, f'key{2*i+1}')
+                self.assertEqual(v, f'value{2*i+1}')
+
+            self.assertEqual(rfdd.custom_attribute1, 're-written custom1')
+            self.assertEqual(rfdd.custom_attribute2, 'custom2')
+            self.assertEqual(rfdd.custom_attribute3, 'custom3')
+
+
+    def test_reopen_file_with_columns(self):
+        data = {f'key{i}': {'name': f'name{i}', 'area': random.random(), 'price': random.random()} for i in range(1000)}
+        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+            for k, v in data.items():
+                wfdd[k] = v
+
+            wfdd.custom_attribute1 = 'custom1'
+            wfdd.custom_attribute2 = 'custom2'
+            wfdd.make_split('evens', [f'key{i}' for i in range(0,1000,2)])
+        with RFDD(self.test_file) as rfdd:
+            for k,v in data.items():
+                self.assertEqual(rfdd[k].name, v['name'])
+                self.assertEqual(rfdd[k].area, v['area'])
+                self.assertEqual(rfdd[k].price, v['price'])
+            rfdd.load_new_split('evens')
+            self.assertEqual(len(list(rfdd.keys())), 500)
+            for i, (k,v) in enumerate(rfdd.items()):
+                self.assertEqual(k, f'key{2*i}')
+                self.assertEqual(v.name, f'name{2*i}')
+                self.assertEqual(v.area, data[f'key{2*i}']['area'])
+                self.assertEqual(v.price, data[f'key{2*i}']['price'])
+
+        data_2 = {f'key{i}': {'name': f'name{i}', 'area': random.random(), 'price': random.random()} for i in range(1000,2000)}
+        with WFDD(self.test_file, columns=('name','area', 'price'), reopen=True) as wfdd:
+
+            for k, v in data_2.items():
+                wfdd[k] = v
+            
+            wfdd.custom_attribute1 = 're-written custom1'
+            wfdd.custom_attribute3 = 'custom3'
+            wfdd.add_to_split('evens', [f'key{i}' for i in range(1000,2000,2)])
+            with self.assertRaises(ValueError):
+                wfdd.add_to_split('fake_split', ['key1'])
+            with self.assertRaises(ValueError):
+                wfdd.add_to_split('evens', 234234)
+            wfdd.make_split('odds', [f'key{i}' for i in range(1,2000,2)])
+
+
+    def test_columns_with_partial_dicts(self):
+        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+            wfdd['house1'] = {'name': 'house1', 'area': 100}
+            wfdd['house2'] = {'name': 'house2', 'price': 200000}
+
+        with RFDD(self.test_file) as rfdd:
+            self.assertEqual(rfdd['house1'].name, 'house1')
+            self.assertEqual(rfdd['house1'].area, 100)
+            self.assertEqual(rfdd['house1'].price, None)
+            self.assertEqual(rfdd['house2'].name, 'house2')
+            self.assertEqual(rfdd['house2'].area, None)
+            self.assertEqual(rfdd['house2'].price, 200000)
+
+    def test_columns_with_dicts_with_extra_keys(self):
+        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+            with self.assertRaises(ValueError):
+                wfdd['house1'] = {'name': 'house1', 'area': 100, 'extra': 'extra'}
+            with self.assertRaises(ValueError):
+                wfdd['house2'] = {'name': 'house2', 'price': 200000, 'extra': 'extra'}
+
+    def test_get_dict(self):
+        with WFDD(self.test_file, columns=('name','area', 'price'), overwrite=True) as wfdd:
+            wfdd['house1'] = {'name': 'house1', 'area': 100, 'price': 100000}
+            wfdd['house2'] = {'name': 'house2', 'area': 200, 'price': 200000}
+            wfdd['house3'] = ('house3', 300, 300000)
+
+        with RFDD(self.test_file) as rfdd:
+            self.assertEqual(rfdd['house1'].get_dict(), {'name': 'house1', 'area': 100, 'price': 100000})
+            self.assertEqual(rfdd['house2'].get_dict(), {'name': 'house2', 'area': 200, 'price': 200000})
+            self.assertEqual(rfdd['house3'].get_dict(), {'name': 'house3', 'area': 300, 'price': 300000})
+
 
     def test_dataloader_integration(self):
         from torch.utils.data import DataLoader, Dataset
 
         num_records = 100000
         data = {f'key{i}': (f'value{random.random()}', random.random()) for i in range(num_records)}
         with WFDD(self.test_file, overwrite=True) as wfdd:
```

### Comparing `freeze_dried_data-2.0.0/freeze_dried_data/test_freeze_dried_data_old.py` & `freeze_dried_data-2.1.0/freeze_dried_data/test_freeze_dried_data_old.py`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-2.0.0/freeze_dried_data.egg-info/PKG-INFO` & `freeze_dried_data-2.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,13 @@
-Metadata-Version: 2.1
-Name: freeze-dried-data
-Version: 2.0.0
-Summary: A simple format for machine learning datasets
-Home-page: https://github.com/tstandley/freeze_dried_data
-Author: Trevor Standley
-Author-email: trevor.standley@gmail.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Freeze Dried Data
-A robust format for machine learning datasets.
+A format for machine learning datasets.
 
-FDD allows your entire dataset to be a single file. Instances are only loaded from disk when needed and can be loaded in random order.
+FDD allows your entire dataset to be a single file while supporting fast random access to records on disk.
 
-Work with FDDs like you would python dictionaries. Keys map to objects. For extra organization and speed, columns can be defined where every row has a value for each column. 
+Work with FDDs like you would python dictionaries. Keys map to objects. For extra organization and speed, columns can be defined such that every row has a value for each column. 
 
 FDD files can operate in either read mode or write mode. Once a file is finalized, it cannot be modified without being re-written (i.e., it is "freeze-dried"). This allows for increased simplicity and speed compared to databases that allow modification.
 
 Values are written to disk immediately upon insertion, while keys are written as part of the index when the FDD file is closed.
 
 ## Installation
 ```bash
@@ -52,25 +30,28 @@
 If you key by hash, storing your train, val, and test sets in the same file can reduce the chance of having train/test or train/val overlap.
 
 Custom Splits also maintain order. This makes it easy to compare a ciriculum with random training for example.
 
 Splits also take the place of sharding in many cases. With one split per shard, only the index for the selected split is stored in memory. Everything else can remain on disk. And everything can still remain in a single file.
 
 ### Custom Serialization and Deserialization
-FDD allows custom functions for serializing and deserializing data. This flexibility is especially useful when dealing with complex data types or when performance optimizations are necessary. It also allows on-the-fly compression where the compression algorithm can be chosen on a per-column basis.
+FDD allows custom functions for serializing and deserializing data. This flexibility is especially useful when dealing with complex data types or when performance optimizations are necessary. It also allows on-the-fly compression where the compression algorithm can be chosen on a per-column basis. Finally, custom serialization can be much more efficient when storing tensors (numpy, pytorch, etc.)
 
 ### Custom Properties
 Custom properties are a great place to store dataset metadata such as dataset cards or the code/parameters used to generate the data. In read mode, properties are loaded from disk only when accessed, so this need not incur a runtime cost.
 
 ### Seamless Integration
-FDD is designed to work with data loaders in machine learning frameworks like PyTorch. Unlike other solutions, RFDD objects detect when they've been forked to a new process and re-open their files. 
+FDD is designed to work with data loaders in machine learning frameworks like PyTorch. Unlike other solutions, RFDD objects detect when they've been forked to a new process and re-open their file handles. 
 
 ### Context Management
 FDD supports Python’s context management (using `with` statements), which ensures that files are properly closed after operations are completed, preventing data corruption and resource leaks.
 
+### Easy Appending to Existing Files
+FDD supportes reopening existing files for writing. Reopened files retain all rows, custom properties, and splits already added to the file, while allowing new rows, properties, or splits to be written. Splits can also be modified.
+
 ## Examples
 
 ### Example 1: Creating an FDD File
 ```python
 from freeze_dried_data import WFDD
 
 # Create the file "new dataset.fdd"
@@ -80,14 +61,19 @@
 dataset['key1'] = 'value1'
 
 # Add the entry 1234: 5678 to the dataset and write the value to disk
 dataset[1234] = 5678
 
 # Write the index including all keys to disk and close the file
 dataset.close()
+
+# or use a with statement to ensure files are closed when finished
+with WFDD('new dataset.fdd', overwrite=True)
+    dataset['key1'] = 'value1'
+    dataset[1234] = 5678
 ```
 
 ### Example 2: Reading an FDD File
 ```python
 from freeze_dried_data import RFDD
 
 # Open the existing file and unpickle the index including all keys into memory
@@ -96,14 +82,24 @@
 # Print each key-value pair
 for k, v in dataset.items():
   print(k, v)
 
 # Directly access and print specific items
 print(dataset[1234])        # prints "5678"
 print(list(dataset.keys())) # prints "['key1', 1234]"
+
+dataset.close()
+
+# or using a with statement
+with RFDD('new dataset.fdd'):
+    for k, v in dataset.items():
+        print(k,v)
+    print(dataset[1234])
+    print(list(dataset.keys()))
+    
 ```
 
 ### Example 3: Creating a file with columns
 
 ```python
 from freeze_dried_data import WFDD
 
@@ -131,45 +127,74 @@
 ```
 
 ### Example 4: Reading a file with columns
 ```python
 from freeze_dried_data import RFDD
 
 with RFDD('text_dataset.fdd') as dataset:
-    for row in dataset:
-        print(row['text'], row['label']) 
+    print(dataset.columns)
+    for key, row in dataset.items():
+        print(row['text'], row['label'])
+        # or
+        print(row.text, row.label)
+        # or
+        print(row[0], row[1])
 
 # output:
+# ['text', 'label']
+# This is an example document. 1
+# This is an example document. 1
 # This is an example document. 1
 # Another document for classification. 0
+# Another document for classification. 0
+# Another document for classification. 0
+# A third document. 1
 # A third document. 1
+# A third document. 1
+# A fourth document. 0
 # A fourth document. 0
+# A fourth document. 0
+# A fifth document. None
 # A fifth document. None
+# A fifth document. None
+# A sixth document. None
+# A sixth document. None
 # A sixth document. None
 
 ```
 
-### Example 5: Using Custom Properties
+### Example 5: Using Custom Properties and Custom Splits
 ```python
 from freeze_dried_data import WFDD
 
 # Open a new FDD file, adding custom properties to store additional metadata
 with WFDD('dataset_with_properties.fdd') as dataset:
     dataset.creator = 'Data Scientist'
     dataset.creation_date = '2024-04-12'
     dataset.description = 'Sample dataset with custom properties.'
 
     # Add data to the dataset
-    dataset['key1'] = 'value1'
+    dataset['key1'] = 'train_data1'
+    dataset['key2'] = 'train_data2'
+    dataset['key3'] = 'train_data3'
+    dataset['key4'] = 'val_data1'
+    dataset['key5'] = 'val_data2'
+    dataset.make_split('train', ['key1', 'key2', 'key3'])
+    dataset.make_split('val', ['key4', 'key5'])
+
 
 # Verify and print custom properties
-with RFDD('dataset_with_properties.fdd') as loaded_dataset:
+with RFDD('dataset_with_properties.fdd', split='train') as loaded_dataset:
     print('Creator:', loaded_dataset.creator)
     print('Creation Date:', loaded_dataset.creation_date)
     print('Description:', loaded_dataset.description)
+    # train rows loaded into the index
+    dataset.load_new_split('val')
+    # val rows loaded into the index
+
 ```
 
 ### Example 6: Using custom Serialization
 ```python
 import json
 from freeze_dried_data import WFDD
 
@@ -186,47 +211,73 @@
     print(dataset['key1'])
 
 # outputs:
 # {'complex_data': [1, 2, 3]}
 
 ```
 
-### Example 7: Using in a PyTorch DataLoader with Workers
+### Example 7: File Reopening
+```python
+data = {f'key{i}': f'value{i}' for i in range(1000)}
+with WFDD('test_file.fdd', overwrite=True) as wfdd:
+    for k, v in data.items():
+        wfdd[k] = v
+
+    wfdd.custom_attribute1 = 'custom1'
+    wfdd.custom_attribute2 = 'custom2'
+    wfdd.make_split('evens', [f'key{i}' for i in range(0,1000,2)])
+
+data_2 = {f'key{i}': f'value{i}' for i in range(1000,2000)}
+with WFDD('test_file.fdd', reopen=True) as wfdd:
+    for k, v in data_2.items():
+        wfdd[k] = v
+    
+    wfdd.custom_attribute1 = 're-written custom1'
+    wfdd.custom_attribute3 = 'custom3'
+
+    wfdd.add_to_split('evens', [f'key{i}' for i in range(1000,2000,2)])
+    wfdd.make_split('odds', [f'key{i}' for i in range(1,2000,2)])
+
+# test_file.fdd now contains all 2k rows, both full splits, and all three attributes.
+```
+
+### Example 8: Using in a PyTorch DataLoader with Workers
 ```python
 import torch
 from torch.utils.data import Dataset, DataLoader
 from freeze_dried_data import WFDD
 
 with WFDD('new dataset.fdd') as dataset:
-    dataset.train_keys = ['key1', 'key2', 'key3']
-    dataset.val_keys = ['key4', 'key5']
+    
     dataset['key1'] = 'train_data1'
     dataset['key2'] = 'train_data2'
     dataset['key3'] = 'train_data3'
     dataset['key4'] = 'val_data1'
     dataset['key5'] = 'val_data2'
+    dataset.make_split('train', ['key1', 'key2', 'key3'])
+    dataset.make_split('val', ['key4', 'key5'])
 
 class FDDDataset(Dataset):
     def __init__(self, filename, split='train'):
-        self.fdd = RFDD(filename)
-        if split == 'train':
-            self.keys = self.fdd.train_keys
-        else:
-            self.keys = self.fdd.val_keys
+        self.fdd = RFDD(filename,split=split)
+        self.keys = list(self.fdd.keys())
     
     def __len__(self):
         return len(self.keys)
     
     def __getitem__(self, idx):
         key = self.keys[idx]
         return key, self.fdd[key]
 
 dataset = FDDDataset('new dataset.fdd', split='train')
+
+# Each worker gets a separate copy of the dataset object.
+# The file handles will be refreshed automatically.
 dataloader = DataLoader(dataset, batch_size=2, shuffle=True, num_workers=4)
 
 for key, value in dataloader:
     print(f'Batch: {key} - {value}')
 
 # Example output:
 # Batch: ('key3', 'key2') - ('train_data3', 'train_data2')
 # Batch: ('key1',) - ('train_data1',)
-```
+```
```

### Comparing `freeze_dried_data-2.0.0/setup.py` & `freeze_dried_data-2.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='freeze_dried_data',
-    version='2.0.0',
+    version='2.1.0',
     description='A simple format for machine learning datasets',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/tstandley/freeze_dried_data',
     author='Trevor Standley',
     author_email='trevor.standley@gmail.com',
     license='MIT',
```

