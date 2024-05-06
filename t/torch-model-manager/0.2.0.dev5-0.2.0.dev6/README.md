# Comparing `tmp/torch_model_manager-0.2.0.dev5.tar.gz` & `tmp/torch_model_manager-0.2.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.2.0.dev5.tar", last modified: Fri May  3 10:03:00 2024, max compression
+gzip compressed data, was "torch_model_manager-0.2.0.dev6.tar", last modified: Mon May  6 08:23:32 2024, max compression
```

## Comparing `torch_model_manager-0.2.0.dev5.tar` & `torch_model_manager-0.2.0.dev6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 10:03:00.270626 torch_model_manager-0.2.0.dev5/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-03 10:03:00.270626 torch_model_manager-0.2.0.dev5/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev5/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-03 10:03:00.274626 torch_model_manager-0.2.0.dev5/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1482 2024-05-03 10:02:57.000000 torch_model_manager-0.2.0.dev5/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 10:03:00.266626 torch_model_manager-0.2.0.dev5/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 10:03:00.266626 torch_model_manager-0.2.0.dev5/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev5/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev5/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 10:03:00.266626 torch_model_manager-0.2.0.dev5/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev5/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev5/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 10:03:00.270626 torch_model_manager-0.2.0.dev5/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev5/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22544 2024-05-03 10:00:24.000000 torch_model_manager-0.2.0.dev5/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.2.0.dev5/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 10:03:00.270626 torch_model_manager-0.2.0.dev5/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-03 10:03:00.000000 torch_model_manager-0.2.0.dev5/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-03 10:03:00.000000 torch_model_manager-0.2.0.dev5/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-03 10:03:00.000000 torch_model_manager-0.2.0.dev5/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-03 10:03:00.000000 torch_model_manager-0.2.0.dev5/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-03 10:03:00.000000 torch_model_manager-0.2.0.dev5/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-03 10:03:00.270626 torch_model_manager-0.2.0.dev5/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev5/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     7112 2024-05-03 09:50:17.000000 torch_model_manager-0.2.0.dev5/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 08:23:32.468479 torch_model_manager-0.2.0.dev6/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-06 08:23:32.468479 torch_model_manager-0.2.0.dev6/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev6/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-06 08:23:32.468479 torch_model_manager-0.2.0.dev6/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1482 2024-05-06 08:23:29.000000 torch_model_manager-0.2.0.dev6/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 08:23:32.460478 torch_model_manager-0.2.0.dev6/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 08:23:32.464478 torch_model_manager-0.2.0.dev6/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev6/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev6/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 08:23:32.464478 torch_model_manager-0.2.0.dev6/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev6/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev6/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 08:23:32.464478 torch_model_manager-0.2.0.dev6/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev6/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22115 2024-05-06 08:17:30.000000 torch_model_manager-0.2.0.dev6/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.2.0.dev6/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 08:23:32.464478 torch_model_manager-0.2.0.dev6/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-06 08:23:32.000000 torch_model_manager-0.2.0.dev6/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-06 08:23:32.000000 torch_model_manager-0.2.0.dev6/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-06 08:23:32.000000 torch_model_manager-0.2.0.dev6/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-06 08:23:32.000000 torch_model_manager-0.2.0.dev6/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-06 08:23:32.000000 torch_model_manager-0.2.0.dev6/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 08:23:32.464478 torch_model_manager-0.2.0.dev6/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev6/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     7112 2024-05-03 09:50:17.000000 torch_model_manager-0.2.0.dev6/utils/helpers.py
```

### Comparing `torch_model_manager-0.2.0.dev5/PKG-INFO` & `torch_model_manager-0.2.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0.dev5
+Version: 0.2.0.dev6
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0.dev5/README.md` & `torch_model_manager-0.2.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev5/setup.py` & `torch_model_manager-0.2.0.dev6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.2.0.dev5',
+    version='0.2.0.dev6',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.2.0.dev5/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.2.0.dev6/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev5/tests/test_utils/test_helpers.py` & `torch_model_manager-0.2.0.dev6/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev5/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.2.0.dev6/torch_model_manager/neptune_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,29 +193,29 @@
                         self.run[namespace].append(File.as_image(to_pil(tensor)), name=name, description=description)
                 else:
                     for name, tensor in zip(names, tensors):
                         self.run[namespace].append(File.as_image(to_pil(tensor)), name=name)            
 
             print(Fore.GREEN+"The tensors are successfully uploaded to Neptune.", Fore.WHITE)
         
-        def log_files(self, data, namespace, from_path=None, extension=None):
+        def log_files(self, data, namespace, from_path=None, extension=None, wait = False):
             """
             Log files to Neptune.
 
             Args:
                 data: The data to log.
                 namespace (str): The namespace to log the data.
                 from_path (str, optional): The path of the file to log. Defaults to None.
                 extension (str, optional): The extension of the file. Defaults to None.
             """
             try:
                 if from_path is not None:
-                    self.run[namespace].upload(File.from_path(from_path, extension=extension))
+                    self.run[namespace].upload(File.from_path(from_path, extension=extension), wait=wait)
                 else:
-                    self.run[namespace].upload(File.as_pickle(data))
+                    self.run[namespace].upload(File.as_pickle(data), wait=wait)
                 print(Fore.GREEN+"The data are successfully loaded to Neptune."+Fore.WHITE)
             except:
                 print(Fore.RED+"The data are not loaded to Neptune. Please check the path or the data format.\
                     This also might due to the existence of the same path in the namespace which risks to be overweighted."+Fore.WHITE)
         
         def log_dataframe(self, 
                           dataframe: pd.DataFrame, 
@@ -269,28 +269,28 @@
             Args:
                 model (nn.Module): The model to track the metric for.
                 metric (Union[float, int]): The metric value.
                 namespace (str): The namespace to log the metric.
             """
             self.run[namespace].append(metric, step=step, timestamp=timestamp, wait=wait)
 
-        def log_checkpoint(self, namespace, model, optimizer, loss, epoch, **kwargs):
+        def log_checkpoint(self, namespace, model, optimizer, loss, epoch, wait=False, **kwargs):
             state_dict = {
                 "model_state_dict": model.state_dict(),
                 "optimizer_state_dict": optimizer.state_dict(),
                 "loss": loss,
                 "epoch": epoch,
                 **kwargs
             }
             
             tmp_file = tempfile.NamedTemporaryFile(suffix = '.pth', delete=False)
             torch.save(state_dict, tmp_file.name)
                 
                 
-            self.log_files(namespace=namespace, data= None, from_path=tmp_file.name, extension='pth')
+            self.log_files(namespace=namespace, data= None, from_path=tmp_file.name, extension='pth', wait=wait)
             
             print(Fore.GREEN+"The checkpoint is successfully logged to Neptune.", Fore.WHITE)
 
         def log_hyperparameters(self, 
                                hyperparams: dict, 
                                namespace: str):  
             """
@@ -503,36 +503,24 @@
             return self.run[namespace].fetch_values()
         
         
 # nm = NeptuneManager(project_name="Billal-MOKHTARI/Image-Clustering-based-on-Dual-Message-Passing",
 #                     api_token="eyJhcGlfYWRkcmVzcyI6Imh0dHBzOi8vYXBwLm5lcHR1bmUuYWkiLCJhcGlfdXJsIjoiaHR0cHM6Ly9hcHAubmVwdHVuZS5haSIsImFwaV9rZXkiOiI0NGRlOTNiZC0zNGZlLTRjNWUtYWEyMC00NzEwOWJkOTRhODgifQ==",
 #                     run_ids_path="run_ids.json")
 
-# from torchvision import models
-# parameters = {
-#     "lr": 1e-2,
-#     "bs": 128,
-#     "input_sz": 32 * 32 * 3,
-#     "n_classes": 10,
-#     "model_filename": "basemodel",
-#     "device": torch.device("cuda" if torch.cuda.is_available() else "cpu"),
-#     "epochs": 2,
-# }
 
 
 # run = nm.Run(name="Image GAT Message Passing")
 # data = run.fetch_pkl_data("embeddings")
 # print(data)
 
-# model = models.resnet18(pretrained=True)
-# optimizer = torch.optim.Adam(model.parameters(), lr=1e-3)
-# loss = "MSE"
-# run.log_checkpoint(namespace="checkpoints", model=model, optimizer=optimizer, loss=loss, epoch=1)
+# from mrg32k3a.mrg32k3a import MRG32k3a
+# from matplotlib import pyplot as plt
+# from torch.nn import init
 
-# chkpt = run.fetch_data("training/checkpoints")
-# print(chkpt)
 
-# data = run.fetch_data("training/losses/MSE")
-# print(data)
-# import time
-# for epoch in range(100):
-#     run.track_metric(epoch, "training/losses/MSE", step=epoch, timestamp=time.time(), wait=True)
+
+# a = init.kaiming_uniform_(torch.empty(10000, 10000), generator=torch.Generator(device="cpu"))
+# print(a.shape)
+# plt.hist2d(a[0], a[1], bins=200)
+# plt.show()
+
```

### Comparing `torch_model_manager-0.2.0.dev5/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.2.0.dev6/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev5/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.2.0.dev6/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0.dev5
+Version: 0.2.0.dev6
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0.dev5/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.2.0.dev6/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev5/utils/helpers.py` & `torch_model_manager-0.2.0.dev6/utils/helpers.py`

 * *Files identical despite different names*

