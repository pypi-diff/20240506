# Comparing `tmp/ema-pytorch-0.4.5.tar.gz` & `tmp/ema_pytorch-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ema-pytorch-0.4.5.tar", last modified: Sat Mar 30 15:34:24 2024, max compression
+gzip compressed data, was "ema_pytorch-0.4.6.tar", last modified: Mon May  6 14:35:42 2024, max compression
```

## Comparing `ema-pytorch-0.4.5.tar` & `ema_pytorch-0.4.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:34:24.711880 ema-pytorch-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-30 15:34:20.000000 ema-pytorch-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-30 15:34:24.711880 ema-pytorch-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-03-30 15:34:20.000000 ema-pytorch-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:34:24.711880 ema-pytorch-0.4.5/ema_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-30 15:34:20.000000 ema-pytorch-0.4.5/ema_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-03-30 15:34:20.000000 ema-pytorch-0.4.5/ema_pytorch/ema_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-03-30 15:34:20.000000 ema-pytorch-0.4.5/ema_pytorch/post_hoc_ema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:34:24.711880 ema-pytorch-0.4.5/ema_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-30 15:34:24.000000 ema-pytorch-0.4.5/ema_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-30 15:34:24.000000 ema-pytorch-0.4.5/ema_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 15:34:24.000000 ema-pytorch-0.4.5/ema_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-30 15:34:24.000000 ema-pytorch-0.4.5/ema_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-30 15:34:24.000000 ema-pytorch-0.4.5/ema_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 15:34:24.711880 ema-pytorch-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-30 15:34:20.000000 ema-pytorch-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:42.609905 ema_pytorch-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-06 14:35:36.000000 ema_pytorch-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-06 14:35:42.609905 ema_pytorch-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-06 14:35:36.000000 ema_pytorch-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:42.609905 ema_pytorch-0.4.6/ema_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-06 14:35:36.000000 ema_pytorch-0.4.6/ema_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-05-06 14:35:36.000000 ema_pytorch-0.4.6/ema_pytorch/ema_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-05-06 14:35:36.000000 ema_pytorch-0.4.6/ema_pytorch/post_hoc_ema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:42.609905 ema_pytorch-0.4.6/ema_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-06 14:35:42.000000 ema_pytorch-0.4.6/ema_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-06 14:35:42.000000 ema_pytorch-0.4.6/ema_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:35:42.000000 ema_pytorch-0.4.6/ema_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-06 14:35:42.000000 ema_pytorch-0.4.6/ema_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 14:35:42.000000 ema_pytorch-0.4.6/ema_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 14:35:42.609905 ema_pytorch-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-06 14:35:36.000000 ema_pytorch-0.4.6/setup.py
```

### Comparing `ema-pytorch-0.4.5/LICENSE` & `ema_pytorch-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ema-pytorch-0.4.5/PKG-INFO` & `ema_pytorch-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ema-pytorch
-Version: 0.4.5
+Version: 0.4.6
 Summary: Easy way to keep track of exponential moving average version of your pytorch module
 Home-page: https://github.com/lucidrains/ema-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,exponential moving average
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ema-pytorch-0.4.5/README.md` & `ema_pytorch-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `ema-pytorch-0.4.5/ema_pytorch/ema_pytorch.py` & `ema_pytorch-0.4.6/ema_pytorch/ema_pytorch.py`

 * *Files identical despite different names*

### Comparing `ema-pytorch-0.4.5/ema_pytorch/post_hoc_ema.py` & `ema_pytorch-0.4.6/ema_pytorch/post_hoc_ema.py`

 * *Files 8% similar despite different names*

```diff
@@ -358,19 +358,19 @@
             timesteps.append(timestep)
 
         step = default(step, max(timesteps))
         assert step <= max(timesteps), f'you can only synthesize for a timestep that is less than the max timestep {max(timesteps)}'
 
         # line up with Algorithm 3
 
-        gamma_i = Tensor(gammas, device = device)
-        t_i = Tensor(timesteps, device = device)
+        gamma_i = torch.tensor(gammas, device = device)
+        t_i = torch.tensor(timesteps, device = device)
 
-        gamma_r = Tensor([gamma], device = device)
-        t_r = Tensor([step], device = device)
+        gamma_r = torch.tensor([gamma], device = device)
+        t_r = torch.tensor([step], device = device)
 
         # solve for weights for combining all checkpoints into synthesized, using least squares as in paper
 
         weights = solve_weights(t_i, gamma_i, t_r, gamma_r)
         weights = weights.squeeze(-1)
 
         # now sum up all the checkpoints using the weights one by one
```

### Comparing `ema-pytorch-0.4.5/ema_pytorch.egg-info/PKG-INFO` & `ema_pytorch-0.4.6/ema_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ema-pytorch
-Version: 0.4.5
+Version: 0.4.6
 Summary: Easy way to keep track of exponential moving average version of your pytorch module
 Home-page: https://github.com/lucidrains/ema-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,exponential moving average
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ema-pytorch-0.4.5/setup.py` & `ema_pytorch-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'ema-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.4.5',
+  version = '0.4.6',
   license='MIT',
   description = 'Easy way to keep track of exponential moving average version of your pytorch module',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/ema-pytorch',
   keywords = [
```

