# Comparing `tmp/torch_model_manager-0.2.0.dev6.tar.gz` & `tmp/torch_model_manager-0.2.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.2.0.dev6.tar", last modified: Mon May  6 08:23:32 2024, max compression
+gzip compressed data, was "torch_model_manager-0.2.0.dev7.tar", last modified: Mon May  6 14:38:30 2024, max compression
```

## Comparing `torch_model_manager-0.2.0.dev6.tar` & `torch_model_manager-0.2.0.dev7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 08:23:32.468479 torch_model_manager-0.2.0.dev6/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-06 08:23:32.468479 torch_model_manager-0.2.0.dev6/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev6/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-06 08:23:32.468479 torch_model_manager-0.2.0.dev6/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1482 2024-05-06 08:23:29.000000 torch_model_manager-0.2.0.dev6/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 08:23:32.460478 torch_model_manager-0.2.0.dev6/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 08:23:32.464478 torch_model_manager-0.2.0.dev6/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev6/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev6/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 08:23:32.464478 torch_model_manager-0.2.0.dev6/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev6/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev6/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 08:23:32.464478 torch_model_manager-0.2.0.dev6/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev6/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22115 2024-05-06 08:17:30.000000 torch_model_manager-0.2.0.dev6/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.2.0.dev6/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 08:23:32.464478 torch_model_manager-0.2.0.dev6/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-06 08:23:32.000000 torch_model_manager-0.2.0.dev6/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-06 08:23:32.000000 torch_model_manager-0.2.0.dev6/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-06 08:23:32.000000 torch_model_manager-0.2.0.dev6/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-06 08:23:32.000000 torch_model_manager-0.2.0.dev6/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-06 08:23:32.000000 torch_model_manager-0.2.0.dev6/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 08:23:32.464478 torch_model_manager-0.2.0.dev6/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev6/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     7112 2024-05-03 09:50:17.000000 torch_model_manager-0.2.0.dev6/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 14:38:30.770833 torch_model_manager-0.2.0.dev7/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-06 14:38:30.766833 torch_model_manager-0.2.0.dev7/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev7/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-06 14:38:30.770833 torch_model_manager-0.2.0.dev7/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1482 2024-05-06 14:38:28.000000 torch_model_manager-0.2.0.dev7/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 14:38:30.762833 torch_model_manager-0.2.0.dev7/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 14:38:30.762833 torch_model_manager-0.2.0.dev7/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev7/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev7/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 14:38:30.766833 torch_model_manager-0.2.0.dev7/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev7/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev7/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 14:38:30.766833 torch_model_manager-0.2.0.dev7/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev7/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22180 2024-05-06 14:38:02.000000 torch_model_manager-0.2.0.dev7/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.2.0.dev7/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 14:38:30.766833 torch_model_manager-0.2.0.dev7/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-06 14:38:30.000000 torch_model_manager-0.2.0.dev7/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-06 14:38:30.000000 torch_model_manager-0.2.0.dev7/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-06 14:38:30.000000 torch_model_manager-0.2.0.dev7/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-06 14:38:30.000000 torch_model_manager-0.2.0.dev7/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-06 14:38:30.000000 torch_model_manager-0.2.0.dev7/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 14:38:30.766833 torch_model_manager-0.2.0.dev7/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev7/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     7112 2024-05-03 09:50:17.000000 torch_model_manager-0.2.0.dev7/utils/helpers.py
```

### Comparing `torch_model_manager-0.2.0.dev6/PKG-INFO` & `torch_model_manager-0.2.0.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0.dev6
+Version: 0.2.0.dev7
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0.dev6/README.md` & `torch_model_manager-0.2.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev6/setup.py` & `torch_model_manager-0.2.0.dev7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.2.0.dev6',
+    version='0.2.0.dev7',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.2.0.dev6/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.2.0.dev7/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev6/tests/test_utils/test_helpers.py` & `torch_model_manager-0.2.0.dev7/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev6/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.2.0.dev7/torch_model_manager/neptune_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,15 +278,15 @@
                 "model_state_dict": model.state_dict(),
                 "optimizer_state_dict": optimizer.state_dict(),
                 "loss": loss,
                 "epoch": epoch,
                 **kwargs
             }
             
-            tmp_file = tempfile.NamedTemporaryFile(suffix = '.pth', delete=False)
+            tmp_file = tempfile.NamedTemporaryFile(suffix = '.pth', delete=True, delete_on_close=True)
             torch.save(state_dict, tmp_file.name)
                 
                 
             self.log_files(namespace=namespace, data= None, from_path=tmp_file.name, extension='pth', wait=wait)
             
             print(Fore.GREEN+"The checkpoint is successfully logged to Neptune.", Fore.WHITE)
 
@@ -464,28 +464,28 @@
                                 on_series=True)
                     
             print(Fore.GREEN+"The hidden conv2d layer outputs are successfully logged to Neptune.", Fore.WHITE)
             return result, row_index, col_index
         
         def fetch_pkl_data(self, namespace: str):
             
-            tmp_file = tempfile.NamedTemporaryFile(delete=True)
+            tmp_file = tempfile.NamedTemporaryFile(delete=True, delete_on_close=True)
             try :
                 self.run[namespace].download(tmp_file.name)
                 with open(tmp_file.name, 'rb') as f:
                     data = pickle.load(f)
             
                 print(Fore.GREEN+"The data is successfully fetched from Neptune.", Fore.WHITE)
                 return data
                 
             except:
                 print(Fore.RED+"The data is not fetched from Neptune. Please check the namespace."+Fore.WHITE)
 
         def load_model_checkpoint(self, namespace, **kwargs):
-            tmp_file = tempfile.NamedTemporaryFile(delete=True)
+            tmp_file = tempfile.NamedTemporaryFile(delete=True, delete_on_close=True)
             try:
                 self.run[namespace].download(tmp_file.name)
                 state_dict = torch.load(tmp_file.name, **kwargs)
                 
                 return state_dict
             except:
                 print(Fore.RED+"The checkpoint is not fetched from Neptune. Please check the namespace."+Fore.WHITE)
```

### Comparing `torch_model_manager-0.2.0.dev6/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.2.0.dev7/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev6/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.2.0.dev7/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0.dev6
+Version: 0.2.0.dev7
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0.dev6/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.2.0.dev7/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev6/utils/helpers.py` & `torch_model_manager-0.2.0.dev7/utils/helpers.py`

 * *Files identical despite different names*

