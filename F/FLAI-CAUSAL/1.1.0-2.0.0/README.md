# Comparing `tmp/FLAI_CAUSAL-1.1.0.tar.gz` & `tmp/flai_causal-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLAI_CAUSAL-1.1.0.tar", last modified: Sun Jun  4 10:48:11 2023, max compression
+gzip compressed data, was "flai_causal-2.0.0.tar", last modified: Mon May  6 01:32:14 2024, max compression
```

## Comparing `FLAI_CAUSAL-1.1.0.tar` & `flai_causal-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:48:11.913789 FLAI_CAUSAL-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:48:11.913789 FLAI_CAUSAL-1.1.0/FLAI/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 10:47:59.000000 FLAI_CAUSAL-1.1.0/FLAI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-06-04 10:47:59.000000 FLAI_CAUSAL-1.1.0/FLAI/causal_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-06-04 10:47:59.000000 FLAI_CAUSAL-1.1.0/FLAI/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:48:11.913789 FLAI_CAUSAL-1.1.0/FLAI_CAUSAL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-06-04 10:48:11.000000 FLAI_CAUSAL-1.1.0/FLAI_CAUSAL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-04 10:48:11.000000 FLAI_CAUSAL-1.1.0/FLAI_CAUSAL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 10:48:11.000000 FLAI_CAUSAL-1.1.0/FLAI_CAUSAL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-04 10:48:11.000000 FLAI_CAUSAL-1.1.0/FLAI_CAUSAL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 10:48:11.000000 FLAI_CAUSAL-1.1.0/FLAI_CAUSAL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 10:47:59.000000 FLAI_CAUSAL-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-06-04 10:48:11.913789 FLAI_CAUSAL-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-04 10:47:59.000000 FLAI_CAUSAL-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 10:48:11.913789 FLAI_CAUSAL-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-04 10:47:59.000000 FLAI_CAUSAL-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:32:14.092013 flai_causal-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:32:14.092013 flai_causal-2.0.0/FLAI/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 01:32:09.000000 flai_causal-2.0.0/FLAI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-05-06 01:32:09.000000 flai_causal-2.0.0/FLAI/causal_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-05-06 01:32:09.000000 flai_causal-2.0.0/FLAI/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 01:32:14.092013 flai_causal-2.0.0/FLAI_CAUSAL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-05-06 01:32:14.000000 flai_causal-2.0.0/FLAI_CAUSAL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-06 01:32:14.000000 flai_causal-2.0.0/FLAI_CAUSAL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 01:32:14.000000 flai_causal-2.0.0/FLAI_CAUSAL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-06 01:32:14.000000 flai_causal-2.0.0/FLAI_CAUSAL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 01:32:14.000000 flai_causal-2.0.0/FLAI_CAUSAL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 01:32:09.000000 flai_causal-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-05-06 01:32:14.092013 flai_causal-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-05-06 01:32:09.000000 flai_causal-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 01:32:14.092013 flai_causal-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-06 01:32:09.000000 flai_causal-2.0.0/setup.py
```

### Comparing `FLAI_CAUSAL-1.1.0/FLAI/causal_graph.py` & `flai_causal-2.0.0/FLAI/causal_graph.py`

 * *Files identical despite different names*

### Comparing `FLAI_CAUSAL-1.1.0/FLAI_CAUSAL.egg-info/PKG-INFO` & `flai_causal-2.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: FLAI-CAUSAL
-Version: 1.1.0
-Summary: Library to creat causal model and mitigate the bias.
-Home-page: https://github.com/rugonzs/FLAI
-Author: Rubén González Sendino
-Author-email: rubo.g@icloud.com
-License: Apache-2.0 license
-Project-URL: Documentation, https://rugonzs.github.io/FLAI/
-Project-URL: Source Code, https://github.com/rugonzs/FLAI
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 
 # FLAI : Fairness Learning in Artificial Intelligence
 
 [![Upload Python Package](https://github.com/rugonzs/FLAI/actions/workflows/python-publish.yml/badge.svg)](https://github.com/rugonzs/FLAI/actions/workflows/python-publish.yml)
 
 [![Upload Docs](https://github.com/rugonzs/FLAI/actions/workflows/docs.yml/badge.svg)](https://github.com/rugonzs/FLAI/actions/workflows/docs.yml)
@@ -58,16 +45,35 @@
 ## Installation
 
 **FLAI** can be easily installed using pip, Python's package installer. Open your terminal or command prompt and type the following command:
 
 ```bash
 pip install flai-causal
 ```
+## Features Fairnes Metric
+Measure equality and equity.
+
+```python
+from FLAI import data
+from FLAI import causal_graph
+import pandas as pd
 
-## Features
+df = pd.read_parquet('../Data/case_1.parquet')
+flai_dataset = data.Data(df, transform=False)
+
+df_f,datos_f = flai_dataset.fairness_eqa_eqi(features = ['education'], 
+                              target_column = 'proba', 
+                              column_filter = ['sensible'],
+                              plot = True)
+```
+![Original Graph](https://github.com/rugonzs/FLAI/blob/main/Documents/fairness_metric.svg)
+
+
+
+## Features Mitigation
 
 ### Causal Creation
 
 ```python
 from FLAI import data
 from FLAI import causal_graph
 import pandas as pd
@@ -190,20 +196,43 @@
 ##### Shap Results
 ```python
 import shap
 
 explainer_original = shap.Explainer(model_original)
 explainer_mitigated = shap.Explainer(model_mitigated)
 shap_values_orignal = explainer_original(original_dataset.data[
-                                               ['sex', 'race','age','education']])
+['age', 'sex', 'credit_history','savings','employment']])
 shap_values_mitigated = explainer_mitigated(original_dataset.data[
-                                               ['sex', 'race', 'age','education']])
+ ['age', 'sex', 'credit_history','savings','employment']])
 shap.plots.beeswarm(shap_values_orignal)
 shap.plots.bar(shap_values_orignal)    
 
 shap.plots.beeswarm(shap_values_mitigated)
 shap.plots.bar(shap_values_mitigated)
 
 ```
-![shap values.](https://github.com/rugonzs/FLAI/blob/main/Documents/shap.svg)
+![shap values.](https://github.com/rugonzs/FLAI/blob/main/Documents/shap_o.svg)
+
+![shap values.](https://github.com/rugonzs/FLAI/blob/main/Documents/shap_m.svg)
 
+
+### References
+* https://erdogant.github.io/bnlearn/
+* http://pgmpy.org
 ## Citation
+
+Mitigation Paper
+```
+@article{GONZALEZSENDINO2024384,
+title = {Mitigating bias in artificial intelligence: Fair data generation via causal models for transparent and explainable decision-making},
+journal = {Future Generation Computer Systems},
+volume = {155},
+pages = {384-401},
+year = {2024},
+issn = {0167-739X},
+doi = {https://doi.org/10.1016/j.future.2024.02.023},
+url = {https://www.sciencedirect.com/science/article/pii/S0167739X24000694},
+author = {Rubén González-Sendino and Emilio Serrano and Javier Bajo},
+keywords = {Causal model, Bias mitigation, Fairness, Responsible artificial intelligence, Bayes},
+abstract = {In the evolving field of Artificial Intelligence, concerns have arisen about the opacity of certain models and their potential biases. This study aims to improve fairness and explainability in AI decision making. Existing bias mitigation strategies are classified as pre-training, training, and post-training approaches. This paper proposes a novel technique to create a mitigated bias dataset. This is achieved using a mitigated causal model that adjusts cause-and-effect relationships and probabilities within a Bayesian network. Contributions of this work include (1) the introduction of a novel mitigation training algorithm for causal model; (2) a pioneering pretraining methodology for producing a fair dataset for Artificial Intelligence model training; (3) the diligent maintenance of sensitive features in the dataset, ensuring that these vital attributes are not overlooked during analysis and model training; (4) the enhancement of explainability and transparency around biases; and finally (5) the development of an interactive demonstration that vividly displays experimental results and provides the code for facilitating replication of the work.}
+}
+```
```

### Comparing `FLAI_CAUSAL-1.1.0/LICENSE` & `flai_causal-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FLAI_CAUSAL-1.1.0/setup.py` & `flai_causal-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.1.0' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '2.0.0' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'FLAI_CAUSAL' #Debe coincidir con el nombre de la carpeta 
 AUTHOR = 'Rubén González Sendino' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'rubo.g@icloud.com' #Modificar con vuestros datos
 URL = 'https://github.com/rugonzs/FLAI' #Modificar con vuestros datos
 
 LICENSE = 'Apache-2.0 license' #Tipo de licencia
 DESCRIPTION = 'Library to creat causal model and mitigate the bias.' #Descripción corta
```

