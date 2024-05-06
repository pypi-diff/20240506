# Comparing `tmp/torchcvnn-0.4.0.tar.gz` & `tmp/torchcvnn-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchcvnn-0.4.0.tar", last modified: Wed Mar 27 12:27:04 2024, max compression
+gzip compressed data, was "torchcvnn-0.5.0.tar", last modified: Mon May  6 19:12:53 2024, max compression
```

## Comparing `torchcvnn-0.4.0.tar` & `torchcvnn-0.5.0.tar`

### file list

```diff
@@ -1,53 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:27:04.970281 torchcvnn-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-27 12:27:04.970281 torchcvnn-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 12:27:04.970281 torchcvnn-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:27:04.962281 torchcvnn-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:27:04.966281 torchcvnn-0.4.0/src/torchcvnn/
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:27:04.966281 torchcvnn-0.4.0/src/torchcvnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:27:04.966281 torchcvnn-0.4.0/src/torchcvnn/datasets/alos2/
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/datasets/alos2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/datasets/alos2/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/datasets/alos2/leader_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/datasets/alos2/parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/datasets/alos2/sar_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/datasets/alos2/trailer_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/datasets/alos2/vol_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:27:04.966281 torchcvnn-0.4.0/src/torchcvnn/datasets/bretigny/
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/datasets/bretigny/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/datasets/bretigny/dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4895 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/datasets/polsf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:27:04.970281 torchcvnn-0.4.0/src/torchcvnn/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:27:04.970281 torchcvnn-0.4.0/src/torchcvnn/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/nn/modules/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14118 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/nn/modules/batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/nn/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/nn/modules/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/nn/modules/initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/nn/modules/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/nn/modules/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/nn/modules/pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/src/torchcvnn/nn/modules/upsampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:27:04.970281 torchcvnn-0.4.0/src/torchcvnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-27 12:27:04.000000 torchcvnn-0.4.0/src/torchcvnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-27 12:27:04.000000 torchcvnn-0.4.0/src/torchcvnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 12:27:04.000000 torchcvnn-0.4.0/src/torchcvnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-27 12:27:04.000000 torchcvnn-0.4.0/src/torchcvnn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-27 12:27:04.000000 torchcvnn-0.4.0/src/torchcvnn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 12:27:04.970281 torchcvnn-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/tests/test_nn_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/tests/test_nn_batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/tests/test_nn_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/tests/test_nn_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/tests/test_nn_initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/tests/test_nn_layernorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/tests/test_nn_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/tests/test_nn_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-03-27 12:26:51.000000 torchcvnn-0.4.0/tests/test_nn_upsample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:12:53.931590 torchcvnn-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-06 19:12:53.931590 torchcvnn-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:12:53.931590 torchcvnn-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:12:53.923590 torchcvnn-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:12:53.923590 torchcvnn-0.5.0/src/torchcvnn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:12:53.923590 torchcvnn-0.5.0/src/torchcvnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:12:53.923590 torchcvnn-0.5.0/src/torchcvnn/datasets/alos2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/datasets/alos2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/datasets/alos2/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/datasets/alos2/leader_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/datasets/alos2/parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/datasets/alos2/sar_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/datasets/alos2/trailer_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/datasets/alos2/vol_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:12:53.927590 torchcvnn-0.5.0/src/torchcvnn/datasets/bretigny/
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/datasets/bretigny/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/datasets/bretigny/dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4895 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/datasets/polsf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:12:53.927590 torchcvnn-0.5.0/src/torchcvnn/datasets/slc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/datasets/slc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/datasets/slc/ann_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/datasets/slc/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/datasets/slc/slc_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:12:53.927590 torchcvnn-0.5.0/src/torchcvnn/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:12:53.927590 torchcvnn-0.5.0/src/torchcvnn/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/nn/modules/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14118 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/nn/modules/batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/nn/modules/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/nn/modules/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/nn/modules/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/nn/modules/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/nn/modules/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/src/torchcvnn/nn/modules/upsampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:12:53.927590 torchcvnn-0.5.0/src/torchcvnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-06 19:12:53.000000 torchcvnn-0.5.0/src/torchcvnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-06 19:12:53.000000 torchcvnn-0.5.0/src/torchcvnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:12:53.000000 torchcvnn-0.5.0/src/torchcvnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 19:12:53.000000 torchcvnn-0.5.0/src/torchcvnn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 19:12:53.000000 torchcvnn-0.5.0/src/torchcvnn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:12:53.927590 torchcvnn-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/tests/test_nn_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/tests/test_nn_batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/tests/test_nn_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/tests/test_nn_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/tests/test_nn_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/tests/test_nn_layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/tests/test_nn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/tests/test_nn_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-06 19:12:47.000000 torchcvnn-0.5.0/tests/test_nn_upsample.py
```

### Comparing `torchcvnn-0.4.0/LICENSE` & `torchcvnn-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/PKG-INFO` & `torchcvnn-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchcvnn
-Version: 0.4.0
+Version: 0.5.0
 Summary: torchcvnn provides complex valued layers to be used with pytorch
 Author-email: Jeremy Fix <jeremy.fix@centralesupelec.fr>
 Maintainer-email: Jeremy Fix <jeremy.fix@centralesupelec.fr>
 Keywords: deep learning,pytorch,complex valued neural networks
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
```

### Comparing `torchcvnn-0.4.0/README.md` & `torchcvnn-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/pyproject.toml` & `torchcvnn-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/__init__.py` & `torchcvnn-0.5.0/src/torchcvnn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 """
 # Torchcvnn
 
 This provides several modules (layers, activation functions) suitable for
 optimizing complex valued neural networks with the pytorch framework.
 """
```

### Comparing `torchcvnn-0.4.0/src/torchcvnn/datasets/__init__.py` & `torchcvnn-0.5.0/src/torchcvnn/datasets/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from .polsf import PolSFDataset
 from .alos2 import ALOSDataset
 from .bretigny import Bretigny
+from .slc import SLCDataset
```

### Comparing `torchcvnn-0.4.0/src/torchcvnn/datasets/alos2/__init__.py` & `torchcvnn-0.5.0/src/torchcvnn/datasets/alos2/__init__.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/datasets/alos2/dataset.py` & `torchcvnn-0.5.0/src/torchcvnn/datasets/alos2/dataset.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/datasets/alos2/leader_file.py` & `torchcvnn-0.5.0/src/torchcvnn/datasets/alos2/leader_file.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/datasets/alos2/parse_utils.py` & `torchcvnn-0.5.0/src/torchcvnn/datasets/alos2/parse_utils.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/datasets/alos2/sar_image.py` & `torchcvnn-0.5.0/src/torchcvnn/datasets/alos2/sar_image.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/datasets/alos2/trailer_file.py` & `torchcvnn-0.5.0/src/torchcvnn/datasets/alos2/trailer_file.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/datasets/alos2/vol_file.py` & `torchcvnn-0.5.0/src/torchcvnn/datasets/alos2/vol_file.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/datasets/bretigny/__init__.py` & `torchcvnn-0.5.0/src/torchcvnn/datasets/bretigny/__init__.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/datasets/bretigny/dataset.py` & `torchcvnn-0.5.0/src/torchcvnn/datasets/bretigny/dataset.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/datasets/polsf.py` & `torchcvnn-0.5.0/src/torchcvnn/datasets/polsf.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/nn/__init__.py` & `torchcvnn-0.5.0/src/torchcvnn/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/nn/modules/__init__.py` & `torchcvnn-0.5.0/src/torchcvnn/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/nn/modules/activation.py` & `torchcvnn-0.5.0/src/torchcvnn/nn/modules/activation.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/nn/modules/batchnorm.py` & `torchcvnn-0.5.0/src/torchcvnn/nn/modules/batchnorm.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/nn/modules/conv.py` & `torchcvnn-0.5.0/src/torchcvnn/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/nn/modules/dropout.py` & `torchcvnn-0.5.0/src/torchcvnn/nn/modules/dropout.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/nn/modules/initialization.py` & `torchcvnn-0.5.0/src/torchcvnn/nn/modules/initialization.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/nn/modules/loss.py` & `torchcvnn-0.5.0/src/torchcvnn/nn/modules/loss.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/nn/modules/normalization.py` & `torchcvnn-0.5.0/src/torchcvnn/nn/modules/normalization.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/nn/modules/pooling.py` & `torchcvnn-0.5.0/src/torchcvnn/nn/modules/pooling.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn/nn/modules/upsampling.py` & `torchcvnn-0.5.0/src/torchcvnn/nn/modules/upsampling.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/src/torchcvnn.egg-info/PKG-INFO` & `torchcvnn-0.5.0/src/torchcvnn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchcvnn
-Version: 0.4.0
+Version: 0.5.0
 Summary: torchcvnn provides complex valued layers to be used with pytorch
 Author-email: Jeremy Fix <jeremy.fix@centralesupelec.fr>
 Maintainer-email: Jeremy Fix <jeremy.fix@centralesupelec.fr>
 Keywords: deep learning,pytorch,complex valued neural networks
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
```

### Comparing `torchcvnn-0.4.0/src/torchcvnn.egg-info/SOURCES.txt` & `torchcvnn-0.5.0/src/torchcvnn.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 src/torchcvnn/datasets/alos2/leader_file.py
 src/torchcvnn/datasets/alos2/parse_utils.py
 src/torchcvnn/datasets/alos2/sar_image.py
 src/torchcvnn/datasets/alos2/trailer_file.py
 src/torchcvnn/datasets/alos2/vol_file.py
 src/torchcvnn/datasets/bretigny/__init__.py
 src/torchcvnn/datasets/bretigny/dataset.py
+src/torchcvnn/datasets/slc/__init__.py
+src/torchcvnn/datasets/slc/ann_file.py
+src/torchcvnn/datasets/slc/dataset.py
+src/torchcvnn/datasets/slc/slc_file.py
 src/torchcvnn/nn/__init__.py
 src/torchcvnn/nn/modules/__init__.py
 src/torchcvnn/nn/modules/activation.py
 src/torchcvnn/nn/modules/batchnorm.py
 src/torchcvnn/nn/modules/conv.py
 src/torchcvnn/nn/modules/dropout.py
 src/torchcvnn/nn/modules/initialization.py
```

### Comparing `torchcvnn-0.4.0/tests/test_nn_activation.py` & `torchcvnn-0.5.0/tests/test_nn_activation.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/tests/test_nn_batchnorm.py` & `torchcvnn-0.5.0/tests/test_nn_batchnorm.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/tests/test_nn_conv.py` & `torchcvnn-0.5.0/tests/test_nn_conv.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/tests/test_nn_dropout.py` & `torchcvnn-0.5.0/tests/test_nn_dropout.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/tests/test_nn_initialization.py` & `torchcvnn-0.5.0/tests/test_nn_initialization.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/tests/test_nn_layernorm.py` & `torchcvnn-0.5.0/tests/test_nn_layernorm.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/tests/test_nn_loss.py` & `torchcvnn-0.5.0/tests/test_nn_loss.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/tests/test_nn_pooling.py` & `torchcvnn-0.5.0/tests/test_nn_pooling.py`

 * *Files identical despite different names*

### Comparing `torchcvnn-0.4.0/tests/test_nn_upsample.py` & `torchcvnn-0.5.0/tests/test_nn_upsample.py`

 * *Files identical despite different names*

