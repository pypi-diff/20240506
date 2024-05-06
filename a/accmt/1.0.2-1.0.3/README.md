# Comparing `tmp/accmt-1.0.2.tar.gz` & `tmp/accmt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accmt-1.0.2.tar", last modified: Thu May  2 22:07:14 2024, max compression
+gzip compressed data, was "accmt-1.0.3.tar", last modified: Mon May  6 06:10:40 2024, max compression
```

## Comparing `accmt-1.0.2.tar` & `accmt-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 22:07:14.768036 accmt-1.0.2/
--rw-rw-rw-   0        0        0    11558 2024-03-31 07:36:29.000000 accmt-1.0.2/LICENSE
--rw-rw-rw-   0        0        0    14020 2024-05-02 22:07:14.766034 accmt-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    13283 2024-05-02 22:06:41.000000 accmt-1.0.2/README.md
--rw-rw-rw-   0        0        0      108 2024-03-31 07:58:03.000000 accmt-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      841 2024-05-02 22:07:14.770037 accmt-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-02 22:07:14.683153 accmt-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-02 22:07:14.729784 accmt-1.0.2/src/accmt/
--rw-rw-rw-   0        0        0      552 2024-04-28 20:04:39.000000 accmt-1.0.2/src/accmt/__init__.py
--rw-rw-rw-   0        0        0    26995 2024-05-02 22:06:16.000000 accmt-1.0.2/src/accmt/accmt.py
--rw-rw-rw-   0        0        0     3130 2024-04-09 02:58:42.000000 accmt-1.0.2/src/accmt/collate_fns.py
--rw-rw-rw-   0        0        0      484 2024-04-01 00:09:51.000000 accmt-1.0.2/src/accmt/config.py
--rw-rw-rw-   0        0        0      161 2024-04-28 04:10:32.000000 accmt-1.0.2/src/accmt/events.py
--rw-rw-rw-   0        0        0      345 2024-04-28 20:04:47.000000 accmt-1.0.2/src/accmt/loggers.py
--rw-rw-rw-   0        0        0     4524 2024-04-29 15:38:32.000000 accmt-1.0.2/src/accmt/optimizations.py
-drwxrwxrwx   0        0        0        0 2024-05-02 22:07:14.764014 accmt-1.0.2/src/accmt.egg-info/
--rw-rw-rw-   0        0        0    14020 2024-05-02 22:07:14.000000 accmt-1.0.2/src/accmt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-05-02 22:07:14.000000 accmt-1.0.2/src/accmt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 22:07:14.000000 accmt-1.0.2/src/accmt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-02 22:07:14.000000 accmt-1.0.2/src/accmt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-02 22:07:14.000000 accmt-1.0.2/src/accmt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 06:10:40.163909 accmt-1.0.3/
+-rw-rw-rw-   0        0        0    11558 2024-03-31 07:36:29.000000 accmt-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0    14020 2024-05-06 06:10:40.162902 accmt-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    13283 2024-05-02 22:06:41.000000 accmt-1.0.3/README.md
+-rw-rw-rw-   0        0        0      108 2024-03-31 07:58:03.000000 accmt-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      841 2024-05-06 06:10:40.166902 accmt-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 06:10:40.084369 accmt-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 06:10:40.128901 accmt-1.0.3/src/accmt/
+-rw-rw-rw-   0        0        0      552 2024-04-28 20:04:39.000000 accmt-1.0.3/src/accmt/__init__.py
+-rw-rw-rw-   0        0        0    27404 2024-05-06 06:08:11.000000 accmt-1.0.3/src/accmt/accmt.py
+-rw-rw-rw-   0        0        0     3130 2024-04-09 02:58:42.000000 accmt-1.0.3/src/accmt/collate_fns.py
+-rw-rw-rw-   0        0        0      484 2024-04-01 00:09:51.000000 accmt-1.0.3/src/accmt/config.py
+-rw-rw-rw-   0        0        0      161 2024-04-28 04:10:32.000000 accmt-1.0.3/src/accmt/events.py
+-rw-rw-rw-   0        0        0      345 2024-04-28 20:04:47.000000 accmt-1.0.3/src/accmt/loggers.py
+-rw-rw-rw-   0        0        0     4524 2024-04-29 15:38:32.000000 accmt-1.0.3/src/accmt/optimizations.py
+-rw-rw-rw-   0        0        0      451 2024-05-06 05:59:07.000000 accmt-1.0.3/src/accmt/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:10:40.160903 accmt-1.0.3/src/accmt.egg-info/
+-rw-rw-rw-   0        0        0    14020 2024-05-06 06:10:40.000000 accmt-1.0.3/src/accmt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2024-05-06 06:10:40.000000 accmt-1.0.3/src/accmt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 06:10:40.000000 accmt-1.0.3/src/accmt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-06 06:10:40.000000 accmt-1.0.3/src/accmt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-06 06:10:40.000000 accmt-1.0.3/src/accmt.egg-info/top_level.txt
```

### Comparing `accmt-1.0.2/LICENSE` & `accmt-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `accmt-1.0.2/PKG-INFO` & `accmt-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accmt
-Version: 1.0.2
+Version: 1.0.3
 Summary: Accelerator Module and Trainer based on Accelerate library for simple distributed train processes, inspired by PyTorch Lightning.
 Home-page: https://github.com/ghanvert/AcceleratorModule
 Author: ghanvert
 Author-email: martin.pizarro@cenia.cl
 Project-URL: Bug Tracker, https://github.com/ghanvert/AcceleratorModule/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `accmt-1.0.2/README.md` & `accmt-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `accmt-1.0.2/setup.cfg` & `accmt-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6363 6d74 0d0a 7665 7273 696f   = accmt..versio
-00000020: 6e20 3d20 312e 302e 320d 0a61 7574 686f  n = 1.0.2..autho
+00000020: 6e20 3d20 312e 302e 330d 0a61 7574 686f  n = 1.0.3..autho
 00000030: 7220 3d20 6768 616e 7665 7274 0d0a 6175  r = ghanvert..au
 00000040: 7468 6f72 5f65 6d61 696c 203d 206d 6172  thor_email = mar
 00000050: 7469 6e2e 7069 7a61 7272 6f40 6365 6e69  tin.pizarro@ceni
 00000060: 612e 636c 0d0a 6465 7363 7269 7074 696f  a.cl..descriptio
 00000070: 6e20 3d20 4163 6365 6c65 7261 746f 7220  n = Accelerator 
 00000080: 4d6f 6475 6c65 2061 6e64 2054 7261 696e  Module and Train
 00000090: 6572 2062 6173 6564 206f 6e20 4163 6365  er based on Acce
```

### Comparing `accmt-1.0.2/src/accmt/__init__.py` & `accmt-1.0.3/src/accmt/__init__.py`

 * *Files identical despite different names*

### Comparing `accmt-1.0.2/src/accmt/accmt.py` & `accmt-1.0.3/src/accmt/accmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import torch
 
 from abc import ABC
 from accelerate import Accelerator
-from accelerate.utils import LoggerType, ProjectConfiguration, tqdm
+from accelerate.utils import ProjectConfiguration, tqdm
 from .loggers import TensorBoard, MLFlow
 from .events import *
 from .config import read, save_status, read_status
 import torch.optim
 import torch.optim.lr_scheduler as lr_scheduler
 from torch.utils.data import Dataset
 from typing import Any
@@ -55,14 +55,15 @@
     "InverseSQRT": get_inverse_sqrt_schedule,
     "LinearWithWarmup": get_linear_schedule_with_warmup,
     "PolynomialDecayWithWarmup": get_polynomial_decay_schedule_with_warmup
 }
 
 accelerator = Accelerator()
 
+
 class AcceleratorModule(ABC):
     """
     Super class to define training and validation logic without the need
     to write a training loop.
 
     The constructor of this class must implement `self.model`, specifying the model
     from `torch.nn.Module`.
@@ -257,16 +258,18 @@
         self.collate_fn = collate_fn
         self.max_shard_size = max_shard_size
         self.safe_serialization = safe_serialization
         self.optimizations = optimizations if optimizations is not None else []
 
         self.accelerator = accelerator
         self.accelerator.project_configuration = ProjectConfiguration(project_dir=".", logging_dir=logging_dir, total_limit=1)
+        
         if not isinstance(log_with, list): log_with = [log_with]
         self.accelerator.log_with = [logger.logger for logger in log_with]
+        self.log_with = self.accelerator.log_with
 
     def fit(self,
             module: AcceleratorModule,
             train_dataset: Dataset,
             val_dataset: Dataset = None
     ):
         """
@@ -282,14 +285,16 @@
                 dataset is not specified, then the validation logic of `AcceleratorModule`
                 (if specified) will be skipped. If `model_saving` parameter in the constructor is set
                 to `best_valid_loss`, this will be converted to `best_train_loss` in the background.
         """
         import os
         import torch
 
+        self._initialize_loggers()
+
         from torch.utils.data import DataLoader
 
         if self.hps_config is None:
             raise AttributeError("Cannot train without HPS file config.")
 
         model = getattr(module, "model", None)
         if model is None:
@@ -443,15 +448,15 @@
         loss_item = loss.item()
         train_losses.append(loss_item)
         if step % self.log_every == 0 and self.accelerator.is_main_process:
             self.accelerator.log({"train_loss": loss_item}, step=global_step)
         
         self._apply_before_backward_optimizations(self.model.parameters())
         self.accelerator.backward(loss)
-        #self._apply_after_backward_optimizations(self.model.parameters())
+        self._apply_after_backward_optimizations(self.model.parameters())
 
         if (step % self.grad_accumulation_steps == 0) or (step == len(dataloader)):
             optimizer.step()
             if scheduler is not None:
                 scheduler.step()
             optimizer.zero_grad(set_to_none=self.set_to_none)
 
@@ -606,12 +611,21 @@
 
     def _apply_before_backward_optimizations(self, parameters):
         for optimization in self.optimizations:
             type = optimization.__class__.__bases__[0]
             if isinstance(type, BeforeBackward):
                 optimization(parameters)
 
-    def _apply_after_backward_optimizations(self):
+    def _apply_after_backward_optimizations(self, parameters):
         for optimization in self.optimizations:
             type = optimization.__class__.__bases__[0]
             if isinstance(type, AfterBackward):
-                optimization()
+                optimization(parameters)
+
+    def _initialize_loggers(self):
+        from .utils import is_url
+
+        for logger in self.log_with:
+            if isinstance(logger, MLFlow) and is_url(self.logging_dir):
+                import mlflow
+                mlflow.set_tracking_uri(self.logging_dir)
+                break
```

### Comparing `accmt-1.0.2/src/accmt/collate_fns.py` & `accmt-1.0.3/src/accmt/collate_fns.py`

 * *Files identical despite different names*

### Comparing `accmt-1.0.2/src/accmt/optimizations.py` & `accmt-1.0.3/src/accmt/optimizations.py`

 * *Files identical despite different names*

### Comparing `accmt-1.0.2/src/accmt.egg-info/PKG-INFO` & `accmt-1.0.3/src/accmt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accmt
-Version: 1.0.2
+Version: 1.0.3
 Summary: Accelerator Module and Trainer based on Accelerate library for simple distributed train processes, inspired by PyTorch Lightning.
 Home-page: https://github.com/ghanvert/AcceleratorModule
 Author: ghanvert
 Author-email: martin.pizarro@cenia.cl
 Project-URL: Bug Tracker, https://github.com/ghanvert/AcceleratorModule/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

