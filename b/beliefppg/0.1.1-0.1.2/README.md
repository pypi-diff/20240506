# Comparing `tmp/beliefppg-0.1.1.tar.gz` & `tmp/beliefppg-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beliefppg-0.1.1.tar", last modified: Mon May  6 17:08:24 2024, max compression
+gzip compressed data, was "beliefppg-0.1.2.tar", last modified: Mon May  6 17:26:49 2024, max compression
```

## Comparing `beliefppg-0.1.1.tar` & `beliefppg-0.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 17:08:24.739470 beliefppg-0.1.1/
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     1097 2023-06-14 15:10:08.000000 beliefppg-0.1.1/LICENSE
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)       22 2024-05-06 16:59:14.000000 beliefppg-0.1.1/MANIFEST.in
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     6557 2024-05-06 17:08:24.739470 beliefppg-0.1.1/PKG-INFO
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     5655 2024-05-06 16:44:29.000000 beliefppg-0.1.1/README.md
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     5655 2024-05-06 16:49:24.000000 beliefppg-0.1.1/README_PyPI.md
-drwxrwxr-x   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 17:08:24.735470 beliefppg-0.1.1/beliefppg/
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)       42 2024-05-06 16:02:39.000000 beliefppg-0.1.1/beliefppg/__init__.py
-drwxrwxr-x   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 17:08:24.735470 beliefppg-0.1.1/beliefppg/datasets/
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 16:02:39.000000 beliefppg-0.1.1/beliefppg/datasets/__init__.py
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     9657 2024-04-30 10:09:32.000000 beliefppg-0.1.1/beliefppg/datasets/file_reader.py
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     8176 2024-05-01 08:34:31.000000 beliefppg-0.1.1/beliefppg/datasets/pipeline_generator.py
-drwxrwxr-x   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 17:08:24.739470 beliefppg-0.1.1/beliefppg/inference/
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 16:02:39.000000 beliefppg-0.1.1/beliefppg/inference/__init__.py
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     5672 2024-05-06 16:36:20.000000 beliefppg-0.1.1/beliefppg/inference/inference.py
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)   853618 2024-05-06 14:12:27.000000 beliefppg-0.1.1/beliefppg/inference/inference_model.keras
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)   495336 2024-05-06 15:10:37.000000 beliefppg-0.1.1/beliefppg/inference/inference_model_notimebackbone.keras
-drwxrwxr-x   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 17:08:24.739470 beliefppg-0.1.1/beliefppg/model/
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 16:02:39.000000 beliefppg-0.1.1/beliefppg/model/__init__.py
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)    10315 2024-05-06 08:39:26.000000 beliefppg-0.1.1/beliefppg/model/belief_ppg.py
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     2611 2024-05-05 21:54:45.000000 beliefppg-0.1.1/beliefppg/model/binned_regression_loss.py
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)      354 2024-04-30 10:05:48.000000 beliefppg-0.1.1/beliefppg/model/config.py
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     1008 2024-05-06 08:50:49.000000 beliefppg-0.1.1/beliefppg/model/load.py
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     2508 2024-05-06 08:38:53.000000 beliefppg-0.1.1/beliefppg/model/positional_encoding.py
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)    11691 2024-05-06 15:36:11.000000 beliefppg-0.1.1/beliefppg/model/prior_layer.py
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     1284 2024-05-03 11:44:45.000000 beliefppg-0.1.1/beliefppg/model/timedomain_backbone.py
-drwxrwxr-x   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 17:08:24.739470 beliefppg-0.1.1/beliefppg/util/
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 16:02:39.000000 beliefppg-0.1.1/beliefppg/util/__init__.py
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     4221 2024-05-04 13:52:31.000000 beliefppg-0.1.1/beliefppg/util/args.py
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     4294 2023-06-14 15:10:08.000000 beliefppg-0.1.1/beliefppg/util/augmentations.py
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)      825 2023-06-14 15:10:08.000000 beliefppg-0.1.1/beliefppg/util/callbacks.py
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     5318 2023-06-14 15:10:08.000000 beliefppg-0.1.1/beliefppg/util/preprocessing.py
-drwxrwxr-x   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 17:08:24.735470 beliefppg-0.1.1/beliefppg.egg-info/
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     6557 2024-05-06 17:08:24.000000 beliefppg-0.1.1/beliefppg.egg-info/PKG-INFO
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)      910 2024-05-06 17:08:24.000000 beliefppg-0.1.1/beliefppg.egg-info/SOURCES.txt
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)        1 2024-05-06 17:08:24.000000 beliefppg-0.1.1/beliefppg.egg-info/dependency_links.txt
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)       82 2024-05-06 17:08:24.000000 beliefppg-0.1.1/beliefppg.egg-info/requires.txt
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)       10 2024-05-06 17:08:24.000000 beliefppg-0.1.1/beliefppg.egg-info/top_level.txt
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)       38 2024-05-06 17:08:24.739470 beliefppg-0.1.1/setup.cfg
--rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     1443 2024-05-06 17:06:49.000000 beliefppg-0.1.1/setup.py
+drwxrwxr-x   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 17:26:49.642684 beliefppg-0.1.2/
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     1097 2023-06-14 15:10:08.000000 beliefppg-0.1.2/LICENSE
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)       22 2024-05-06 16:59:14.000000 beliefppg-0.1.2/MANIFEST.in
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     3962 2024-05-06 17:26:49.642684 beliefppg-0.1.2/PKG-INFO
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     5655 2024-05-06 16:44:29.000000 beliefppg-0.1.2/README.md
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     3060 2024-05-06 17:12:04.000000 beliefppg-0.1.2/README_PyPI.md
+drwxrwxr-x   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 17:26:49.638684 beliefppg-0.1.2/beliefppg/
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)       42 2024-05-06 16:02:39.000000 beliefppg-0.1.2/beliefppg/__init__.py
+drwxrwxr-x   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 17:26:49.638684 beliefppg-0.1.2/beliefppg/datasets/
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 16:02:39.000000 beliefppg-0.1.2/beliefppg/datasets/__init__.py
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     9657 2024-04-30 10:09:32.000000 beliefppg-0.1.2/beliefppg/datasets/file_reader.py
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     8176 2024-05-01 08:34:31.000000 beliefppg-0.1.2/beliefppg/datasets/pipeline_generator.py
+drwxrwxr-x   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 17:26:49.638684 beliefppg-0.1.2/beliefppg/inference/
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 16:02:39.000000 beliefppg-0.1.2/beliefppg/inference/__init__.py
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     5672 2024-05-06 16:36:20.000000 beliefppg-0.1.2/beliefppg/inference/inference.py
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)   853618 2024-05-06 14:12:27.000000 beliefppg-0.1.2/beliefppg/inference/inference_model.keras
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)   495336 2024-05-06 15:10:37.000000 beliefppg-0.1.2/beliefppg/inference/inference_model_notimebackbone.keras
+drwxrwxr-x   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 17:26:49.638684 beliefppg-0.1.2/beliefppg/model/
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 16:02:39.000000 beliefppg-0.1.2/beliefppg/model/__init__.py
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)    10315 2024-05-06 08:39:26.000000 beliefppg-0.1.2/beliefppg/model/belief_ppg.py
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     2611 2024-05-05 21:54:45.000000 beliefppg-0.1.2/beliefppg/model/binned_regression_loss.py
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)      354 2024-04-30 10:05:48.000000 beliefppg-0.1.2/beliefppg/model/config.py
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     1008 2024-05-06 08:50:49.000000 beliefppg-0.1.2/beliefppg/model/load.py
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     2508 2024-05-06 08:38:53.000000 beliefppg-0.1.2/beliefppg/model/positional_encoding.py
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)    11691 2024-05-06 15:36:11.000000 beliefppg-0.1.2/beliefppg/model/prior_layer.py
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     1284 2024-05-03 11:44:45.000000 beliefppg-0.1.2/beliefppg/model/timedomain_backbone.py
+drwxrwxr-x   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 17:26:49.642684 beliefppg-0.1.2/beliefppg/util/
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 16:02:39.000000 beliefppg-0.1.2/beliefppg/util/__init__.py
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     4221 2024-05-04 13:52:31.000000 beliefppg-0.1.2/beliefppg/util/args.py
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     4294 2023-06-14 15:10:08.000000 beliefppg-0.1.2/beliefppg/util/augmentations.py
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)      825 2023-06-14 15:10:08.000000 beliefppg-0.1.2/beliefppg/util/callbacks.py
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     5318 2023-06-14 15:10:08.000000 beliefppg-0.1.2/beliefppg/util/preprocessing.py
+drwxrwxr-x   0 pstreli   (1000) pstreli   (1000)        0 2024-05-06 17:26:49.638684 beliefppg-0.1.2/beliefppg.egg-info/
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     3962 2024-05-06 17:26:49.000000 beliefppg-0.1.2/beliefppg.egg-info/PKG-INFO
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)      910 2024-05-06 17:26:49.000000 beliefppg-0.1.2/beliefppg.egg-info/SOURCES.txt
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)        1 2024-05-06 17:26:49.000000 beliefppg-0.1.2/beliefppg.egg-info/dependency_links.txt
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)       82 2024-05-06 17:26:49.000000 beliefppg-0.1.2/beliefppg.egg-info/requires.txt
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)       10 2024-05-06 17:26:49.000000 beliefppg-0.1.2/beliefppg.egg-info/top_level.txt
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)       38 2024-05-06 17:26:49.642684 beliefppg-0.1.2/setup.cfg
+-rw-rw-r--   0 pstreli   (1000) pstreli   (1000)     1443 2024-05-06 17:26:40.000000 beliefppg-0.1.2/setup.py
```

### Comparing `beliefppg-0.1.1/LICENSE` & `beliefppg-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beliefppg-0.1.1/PKG-INFO` & `beliefppg-0.1.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: beliefppg
-Version: 0.1.1
-Summary: Taking multi-channel PPG and Accelerometer signals as input, BeliefPPG predicts the instantaneous heart rate and provides an uncertainty estimate for the prediction.
-Home-page: https://github.com/eth-siplab/BeliefPPG
-Author: Paul Streli
-Author-email: paul.streli@inf.ethz.ch
-Keywords: PPG,heart rate,signal processing,uncertainty estimation,biomedical signals
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## BeliefPPG: Uncertainty-aware Heart Rate Estimation from PPG signals via Belief Propagation (UAI 2023, Official Code)
 
 Valentin Bieri<sup>*2</sup>, [Paul Streli](https://paulstreli.com/)<sup>*1</sup>, Berken Utku Demirel<sup>1</sup>, [Christian Holz](https://www.christianholz.net/)<sup>1</sup>
 
 <sup>1</sup> [Sensing, Interaction & Perception Lab](https://siplab.org/), Department of Computer Science, ETH Zürich, Switzerland
 <br>
 <sup>2</sup> MSc Student, Department of Computer Science, ETH Zürich, Switzerland
```

### Comparing `beliefppg-0.1.1/beliefppg/datasets/file_reader.py` & `beliefppg-0.1.2/beliefppg/datasets/file_reader.py`

 * *Files identical despite different names*

### Comparing `beliefppg-0.1.1/beliefppg/datasets/pipeline_generator.py` & `beliefppg-0.1.2/beliefppg/datasets/pipeline_generator.py`

 * *Files identical despite different names*

### Comparing `beliefppg-0.1.1/beliefppg/inference/inference.py` & `beliefppg-0.1.2/beliefppg/inference/inference.py`

 * *Files identical despite different names*

### Comparing `beliefppg-0.1.1/beliefppg/inference/inference_model.keras` & `beliefppg-0.1.2/beliefppg/inference/inference_model.keras`

 * *Files identical despite different names*

### Comparing `beliefppg-0.1.1/beliefppg/inference/inference_model_notimebackbone.keras` & `beliefppg-0.1.2/beliefppg/inference/inference_model_notimebackbone.keras`

 * *Files identical despite different names*

### Comparing `beliefppg-0.1.1/beliefppg/model/belief_ppg.py` & `beliefppg-0.1.2/beliefppg/model/belief_ppg.py`

 * *Files identical despite different names*

### Comparing `beliefppg-0.1.1/beliefppg/model/binned_regression_loss.py` & `beliefppg-0.1.2/beliefppg/model/binned_regression_loss.py`

 * *Files identical despite different names*

### Comparing `beliefppg-0.1.1/beliefppg/model/load.py` & `beliefppg-0.1.2/beliefppg/model/load.py`

 * *Files identical despite different names*

### Comparing `beliefppg-0.1.1/beliefppg/model/positional_encoding.py` & `beliefppg-0.1.2/beliefppg/model/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `beliefppg-0.1.1/beliefppg/model/prior_layer.py` & `beliefppg-0.1.2/beliefppg/model/prior_layer.py`

 * *Files identical despite different names*

### Comparing `beliefppg-0.1.1/beliefppg/model/timedomain_backbone.py` & `beliefppg-0.1.2/beliefppg/model/timedomain_backbone.py`

 * *Files identical despite different names*

### Comparing `beliefppg-0.1.1/beliefppg/util/args.py` & `beliefppg-0.1.2/beliefppg/util/args.py`

 * *Files identical despite different names*

### Comparing `beliefppg-0.1.1/beliefppg/util/augmentations.py` & `beliefppg-0.1.2/beliefppg/util/augmentations.py`

 * *Files identical despite different names*

### Comparing `beliefppg-0.1.1/beliefppg/util/callbacks.py` & `beliefppg-0.1.2/beliefppg/util/callbacks.py`

 * *Files identical despite different names*

### Comparing `beliefppg-0.1.1/beliefppg/util/preprocessing.py` & `beliefppg-0.1.2/beliefppg/util/preprocessing.py`

 * *Files identical despite different names*

### Comparing `beliefppg-0.1.1/beliefppg.egg-info/SOURCES.txt` & `beliefppg-0.1.2/beliefppg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `beliefppg-0.1.1/setup.py` & `beliefppg-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README_PyPI.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='beliefppg',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     package_data={'beliefppg': ['inference/inference_model.keras', 'inference/inference_model_notimebackbone.keras']},
     install_requires=[
         'numpy',
         'pandas',
         'scikit-learn',
         'tensorflow~=2.14.0',
```

