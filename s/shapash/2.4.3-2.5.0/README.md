# Comparing `tmp/shapash-2.4.3.tar.gz` & `tmp/shapash-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapash-2.4.3.tar", last modified: Tue Mar 12 11:08:10 2024, max compression
+gzip compressed data, was "shapash-2.5.0.tar", last modified: Mon May  6 15:33:06 2024, max compression
```

## Comparing `shapash-2.4.3.tar` & `shapash-2.5.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:08:10.453071 shapash-2.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-03-12 11:05:08.000000 shapash-2.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-12 11:05:08.000000 shapash-2.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    24177 2024-03-12 11:08:10.453071 shapash-2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22090 2024-03-12 11:05:08.000000 shapash-2.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-12 11:08:10.453071 shapash-2.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-03-12 11:05:08.000000 shapash-2.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:08:10.437071 shapash-2.4.3/shapash/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:08:10.441071 shapash-2.4.3/shapash/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/backend/base_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/backend/lime_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/backend/shap_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:08:10.441071 shapash-2.4.3/shapash/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/data/data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:08:10.441071 shapash-2.4.3/shapash/decomposition/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/decomposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/decomposition/contributions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:08:10.441071 shapash-2.4.3/shapash/explainer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/explainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28418 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/explainer/consistency.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/explainer/multi_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    57813 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/explainer/smart_explainer.py
--rw-r--r--   0 runner    (1001) docker     (127)   143801 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/explainer/smart_plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    30494 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/explainer/smart_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/explainer/smart_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:08:10.441071 shapash-2.4.3/shapash/manipulation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/manipulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/manipulation/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/manipulation/mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/manipulation/select_lines.py
--rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/manipulation/summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:08:10.445071 shapash-2.4.3/shapash/report/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/report/base_report.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/report/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/report/data_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/report/generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:08:10.445071 shapash-2.4.3/shapash/report/html/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/report/html/double_table.html
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/report/html/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/report/html/explainability.html
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/report/html/table_two_columns.html
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/report/html/univariate.html
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/report/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    22166 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/report/project_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:08:10.437071 shapash-2.4.3/shapash/report/template/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:08:10.445071 shapash-2.4.3/shapash/report/template/custom/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/report/template/custom/conf.json
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/report/template/custom/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/report/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:08:10.445071 shapash-2.4.3/shapash/style/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/style/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/style/colors.json
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/style/style_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:08:10.449071 shapash-2.4.3/shapash/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/utils/category_encoder_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    19136 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (127)    17684 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/utils/columntransformer_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    12709 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/utils/explanation_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/utils/load_smartpredictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/utils/model_synoptic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/utils/threading.py
--rw-r--r--   0 runner    (1001) docker     (127)    14080 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/utils/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/utils/translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:08:10.449071 shapash-2.4.3/shapash/webapp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/webapp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:08:10.449071 shapash-2.4.3/shapash/webapp/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   215609 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/webapp/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    88145 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/webapp/assets/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/webapp/assets/main.js
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/webapp/assets/material-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    18907 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/webapp/assets/reload.png
--rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/webapp/assets/settings.png
--rw-r--r--   0 runner    (1001) docker     (127)   215609 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/webapp/assets/shapash-fond-fonce.png
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/webapp/assets/style.css
--rw-r--r--   0 runner    (1001) docker     (127)   116915 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/webapp/smart_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:08:10.453071 shapash-2.4.3/shapash/webapp/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/webapp/utils/MyGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)    21533 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/webapp/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/webapp/utils/explanations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/webapp/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/webapp/webapp_launch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-12 11:05:08.000000 shapash-2.4.3/shapash/webapp/webapp_launch_DVF.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 11:08:10.453071 shapash-2.4.3/shapash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24177 2024-03-12 11:08:10.000000 shapash-2.4.3/shapash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-12 11:08:10.000000 shapash-2.4.3/shapash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 11:08:10.000000 shapash-2.4.3/shapash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 11:08:10.000000 shapash-2.4.3/shapash.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-12 11:08:10.000000 shapash-2.4.3/shapash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-12 11:08:10.000000 shapash-2.4.3/shapash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:06.977487 shapash-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-06 15:29:52.000000 shapash-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-06 15:29:52.000000 shapash-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    24166 2024-05-06 15:33:06.977487 shapash-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22090 2024-05-06 15:29:52.000000 shapash-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-06 15:33:06.977487 shapash-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-06 15:29:52.000000 shapash-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:06.961487 shapash-2.5.0/shapash/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:06.961487 shapash-2.5.0/shapash/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/backend/base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/backend/lime_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/backend/shap_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:06.961487 shapash-2.5.0/shapash/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/data/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:06.965487 shapash-2.5.0/shapash/decomposition/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/decomposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/decomposition/contributions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:06.965487 shapash-2.5.0/shapash/explainer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/explainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28418 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/explainer/consistency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/explainer/multi_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58754 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/explainer/smart_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)   143095 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/explainer/smart_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30494 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/explainer/smart_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/explainer/smart_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:06.965487 shapash-2.5.0/shapash/manipulation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/manipulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/manipulation/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/manipulation/mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/manipulation/select_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9321 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/manipulation/summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:06.965487 shapash-2.5.0/shapash/report/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/report/base_report.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/report/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/report/data_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/report/generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:06.969487 shapash-2.5.0/shapash/report/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/report/html/double_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/report/html/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/report/html/explainability.html
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/report/html/table_two_columns.html
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/report/html/univariate.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/report/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22166 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/report/project_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:06.957487 shapash-2.5.0/shapash/report/template/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:06.969487 shapash-2.5.0/shapash/report/template/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/report/template/custom/conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/report/template/custom/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/report/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:06.969487 shapash-2.5.0/shapash/style/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/style/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/style/colors.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/style/style_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:06.969487 shapash-2.5.0/shapash/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/utils/category_encoder_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19136 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17717 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/utils/columntransformer_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12709 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/utils/explanation_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/utils/load_smartpredictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/utils/model_synoptic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/utils/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14179 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/utils/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/utils/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:06.973487 shapash-2.5.0/shapash/webapp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/webapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:06.973487 shapash-2.5.0/shapash/webapp/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   215609 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/webapp/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    88145 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/webapp/assets/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/webapp/assets/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/webapp/assets/material-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18907 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/webapp/assets/reload.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/webapp/assets/settings.png
+-rw-r--r--   0 runner    (1001) docker     (127)   215609 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/webapp/assets/shapash-fond-fonce.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/webapp/assets/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)   116905 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/webapp/smart_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:06.973487 shapash-2.5.0/shapash/webapp/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/webapp/utils/MyGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21533 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/webapp/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/webapp/utils/explanations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/webapp/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/webapp/webapp_launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-06 15:29:52.000000 shapash-2.5.0/shapash/webapp/webapp_launch_DVF.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:33:06.973487 shapash-2.5.0/shapash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24166 2024-05-06 15:33:06.000000 shapash-2.5.0/shapash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-06 15:33:06.000000 shapash-2.5.0/shapash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:33:06.000000 shapash-2.5.0/shapash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:33:06.000000 shapash-2.5.0/shapash.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-06 15:33:06.000000 shapash-2.5.0/shapash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 15:33:06.000000 shapash-2.5.0/shapash.egg-info/top_level.txt
```

### Comparing `shapash-2.4.3/LICENSE` & `shapash-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/PKG-INFO` & `shapash-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: shapash
-Version: 2.4.3
+Version: 2.5.0
 Summary: Shapash is a Python library which aims to make machine learning interpretable and understandable by everyone.
 Home-page: https://github.com/MAIF/shapash
 Author: Yann Golhen, Sebastien Bidault, Yann Lagre, Maxime Gendre
 Author-email: yann.golhen@maif.fr
 License: Apache Software License 2.0
 Keywords: shapash
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >3.7, <3.12
+Requires-Python: >3.8, <3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plotly>=5.0.0
 Requires-Dist: matplotlib>=3.2.0
 Requires-Dist: numpy>1.18.0
-Requires-Dist: pandas>1.0.2
-Requires-Dist: shap<0.45.0,>=0.38.1
+Requires-Dist: pandas>=2.1.0
+Requires-Dist: shap>=0.45.0
 Requires-Dist: Flask<2.3.0
 Requires-Dist: dash>=2.3.1
 Requires-Dist: dash-bootstrap-components>=1.1.0
 Requires-Dist: dash-core-components>=2.0.0
 Requires-Dist: dash-daq>=0.5.0
 Requires-Dist: dash-html-components>=2.0.0
 Requires-Dist: dash-renderer==1.8.3
 Requires-Dist: dash-table>=5.0.0
 Requires-Dist: nbformat>4.2.0
 Requires-Dist: numba>=0.53.1
-Requires-Dist: scikit-learn<1.4,>=1.0.1
+Requires-Dist: scikit-learn>=1.4.0
 Requires-Dist: category_encoders>=2.6.0
 Requires-Dist: scipy>=0.19.1
 Provides-Extra: report
 Requires-Dist: nbconvert>=6.0.7; extra == "report"
 Requires-Dist: papermill>=2.0.0; extra == "report"
 Requires-Dist: jupyter-client>=7.4.0; extra == "report"
 Requires-Dist: seaborn==0.12.2; extra == "report"
@@ -193,15 +193,15 @@
 
 Shapash can use category-encoders object, sklearn ColumnTransformer or simply features dictionary. <br />
 - Category_encoder: *OneHotEncoder*, *OrdinalEncoder*, *BaseNEncoder*, *BinaryEncoder*, *TargetEncoder*
 - Sklearn ColumnTransformer: *OneHotEncoder*, *OrdinalEncoder*, *StandardScaler*, *QuantileTransformer*, *PowerTransformer*
 
 ## 🛠 Installation
 
-Shapash is intended to work with Python versions 3.8 to 3.11. Installation can be done with pip:
+Shapash is intended to work with Python versions 3.9 to 3.12. Installation can be done with pip:
 
 ```bash
 pip install shapash
 ```
 
 In order to generate the Shapash Report some extra requirements are needed.
 You can install these using the following command :
```

#### html2text {}

```diff
@@ -1,35 +1,34 @@
-Metadata-Version: 2.1 Name: shapash Version: 2.4.3 Summary: Shapash is a Python
+Metadata-Version: 2.1 Name: shapash Version: 2.5.0 Summary: Shapash is a Python
 library which aims to make machine learning interpretable and understandable by
 everyone. Home-page: https://github.com/MAIF/shapash Author: Yann Golhen,
 Sebastien Bidault, Yann Lagre, Maxime Gendre Author-email: yann.golhen@maif.fr
 License: Apache Software License 2.0 Keywords: shapash Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Operating System :: OS Independent Requires-Python: >3.7, <3.12 Description-
+Operating System :: OS Independent Requires-Python: >3.8, <3.13 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: plotly>=5.0.0
 Requires-Dist: matplotlib>=3.2.0 Requires-Dist: numpy>1.18.0 Requires-Dist:
-pandas>1.0.2 Requires-Dist: shap<0.45.0,>=0.38.1 Requires-Dist: Flask<2.3.0
-Requires-Dist: dash>=2.3.1 Requires-Dist: dash-bootstrap-components>=1.1.0
-Requires-Dist: dash-core-components>=2.0.0 Requires-Dist: dash-daq>=0.5.0
-Requires-Dist: dash-html-components>=2.0.0 Requires-Dist: dash-renderer==1.8.3
-Requires-Dist: dash-table>=5.0.0 Requires-Dist: nbformat>4.2.0 Requires-Dist:
-numba>=0.53.1 Requires-Dist: scikit-learn<1.4,>=1.0.1 Requires-Dist:
-category_encoders>=2.6.0 Requires-Dist: scipy>=0.19.1 Provides-Extra: report
-Requires-Dist: nbconvert>=6.0.7; extra == "report" Requires-Dist:
-papermill>=2.0.0; extra == "report" Requires-Dist: jupyter-client>=7.4.0; extra
-== "report" Requires-Dist: seaborn==0.12.2; extra == "report" Requires-Dist:
-notebook; extra == "report" Requires-Dist: Jinja2>=2.11.0; extra == "report"
-Requires-Dist: phik; extra == "report" Provides-Extra: xgboost Requires-Dist:
-xgboost>=1.0.0; extra == "xgboost" Provides-Extra: lightgbm Requires-Dist:
-lightgbm>=2.3.0; extra == "lightgbm" Provides-Extra: catboost Requires-Dist:
-catboost>=1.0.1; extra == "catboost" Provides-Extra: lime Requires-Dist:
-lime>=0.2.0.0; extra == "lime"
+pandas>=2.1.0 Requires-Dist: shap>=0.45.0 Requires-Dist: Flask<2.3.0 Requires-
+Dist: dash>=2.3.1 Requires-Dist: dash-bootstrap-components>=1.1.0 Requires-
+Dist: dash-core-components>=2.0.0 Requires-Dist: dash-daq>=0.5.0 Requires-Dist:
+dash-html-components>=2.0.0 Requires-Dist: dash-renderer==1.8.3 Requires-Dist:
+dash-table>=5.0.0 Requires-Dist: nbformat>4.2.0 Requires-Dist: numba>=0.53.1
+Requires-Dist: scikit-learn>=1.4.0 Requires-Dist: category_encoders>=2.6.0
+Requires-Dist: scipy>=0.19.1 Provides-Extra: report Requires-Dist:
+nbconvert>=6.0.7; extra == "report" Requires-Dist: papermill>=2.0.0; extra ==
+"report" Requires-Dist: jupyter-client>=7.4.0; extra == "report" Requires-Dist:
+seaborn==0.12.2; extra == "report" Requires-Dist: notebook; extra == "report"
+Requires-Dist: Jinja2>=2.11.0; extra == "report" Requires-Dist: phik; extra ==
+"report" Provides-Extra: xgboost Requires-Dist: xgboost>=1.0.0; extra ==
+"xgboost" Provides-Extra: lightgbm Requires-Dist: lightgbm>=2.3.0; extra ==
+"lightgbm" Provides-Extra: catboost Requires-Dist: catboost>=1.0.1; extra ==
+"catboost" Provides-Extra: lime Requires-Dist: lime>=0.2.0.0; extra == "lime"
  [https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/shapash-
                                   resize.png]
                _[_t_e_s_t_s_]_[_p_y_p_i_]_[_d_o_w_n_l_o_a_d_s_]_[_p_y_v_e_r_s_i_o_n_]_[_l_i_c_e_n_s_e_]_[_d_o_c_]
 ## ð Overview Shapash is a Python library designed to **make machine
 learning interpretable and comprehensible for everyone**. It offers various
 visualizations with clear and explicit labels that are easily understood by
 all. With Shapash, you can generate a **Webapp** that simplifies the
@@ -177,16 +176,16 @@
 of how to provide contributions to Shapash. An [issue](https://github.com/MAIF/
 shapash/issues/488) has been created to enhance this use case. Shapash can use
 category-encoders object, sklearn ColumnTransformer or simply features
 dictionary.
 - Category_encoder: *OneHotEncoder*, *OrdinalEncoder*, *BaseNEncoder*,
 *BinaryEncoder*, *TargetEncoder* - Sklearn ColumnTransformer: *OneHotEncoder*,
 *OrdinalEncoder*, *StandardScaler*, *QuantileTransformer*, *PowerTransformer*
-## ð  Installation Shapash is intended to work with Python versions 3.8 to
-3.11. Installation can be done with pip: ```bash pip install shapash ``` In
+## ð  Installation Shapash is intended to work with Python versions 3.9 to
+3.12. Installation can be done with pip: ```bash pip install shapash ``` In
 order to generate the Shapash Report some extra requirements are needed. You
 can install these using the following command : ```bash pip install shapash
 [report] ``` If you encounter **compatibility issues** you may check the
 corresponding section in the Shapash documentation [here](https://
 shapash.readthedocs.io/en/latest/installation-instructions/index.html). ## ð
 Quickstart The 4 steps to display results: - Step 1: Declare SmartExplainer
 Object > There 1 mandatory parameter in compile method: Model > You can declare
```

### Comparing `shapash-2.4.3/README.md` & `shapash-2.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
 Shapash can use category-encoders object, sklearn ColumnTransformer or simply features dictionary. <br />
 - Category_encoder: *OneHotEncoder*, *OrdinalEncoder*, *BaseNEncoder*, *BinaryEncoder*, *TargetEncoder*
 - Sklearn ColumnTransformer: *OneHotEncoder*, *OrdinalEncoder*, *StandardScaler*, *QuantileTransformer*, *PowerTransformer*
 
 ## 🛠 Installation
 
-Shapash is intended to work with Python versions 3.8 to 3.11. Installation can be done with pip:
+Shapash is intended to work with Python versions 3.9 to 3.12. Installation can be done with pip:
 
 ```bash
 pip install shapash
 ```
 
 In order to generate the Shapash Report some extra requirements are needed.
 You can install these using the following command :
```

#### html2text {}

```diff
@@ -149,16 +149,16 @@
 of how to provide contributions to Shapash. An [issue](https://github.com/MAIF/
 shapash/issues/488) has been created to enhance this use case. Shapash can use
 category-encoders object, sklearn ColumnTransformer or simply features
 dictionary.
 - Category_encoder: *OneHotEncoder*, *OrdinalEncoder*, *BaseNEncoder*,
 *BinaryEncoder*, *TargetEncoder* - Sklearn ColumnTransformer: *OneHotEncoder*,
 *OrdinalEncoder*, *StandardScaler*, *QuantileTransformer*, *PowerTransformer*
-## ð  Installation Shapash is intended to work with Python versions 3.8 to
-3.11. Installation can be done with pip: ```bash pip install shapash ``` In
+## ð  Installation Shapash is intended to work with Python versions 3.9 to
+3.12. Installation can be done with pip: ```bash pip install shapash ``` In
 order to generate the Shapash Report some extra requirements are needed. You
 can install these using the following command : ```bash pip install shapash
 [report] ``` If you encounter **compatibility issues** you may check the
 corresponding section in the Shapash documentation [here](https://
 shapash.readthedocs.io/en/latest/installation-instructions/index.html). ## ð
 Quickstart The 4 steps to display results: - Step 1: Declare SmartExplainer
 Object > There 1 mandatory parameter in compile method: Model > You can declare
```

### Comparing `shapash-2.4.3/setup.py` & `shapash-2.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,27 +16,27 @@
     exec(f.read(), version_d)
 
 
 requirements = [
     "plotly>=5.0.0",
     "matplotlib>=3.2.0",
     "numpy>1.18.0",
-    "pandas>1.0.2",
-    "shap>=0.38.1,<0.45.0",
+    "pandas>=2.1.0",
+    "shap>=0.45.0",
     "Flask<2.3.0",
     "dash>=2.3.1",
     "dash-bootstrap-components>=1.1.0",
     "dash-core-components>=2.0.0",
     "dash-daq>=0.5.0",
     "dash-html-components>=2.0.0",
     "dash-renderer==1.8.3",
     "dash-table>=5.0.0",
     "nbformat>4.2.0",
     "numba>=0.53.1",
-    "scikit-learn>=1.0.1,<1.4",
+    "scikit-learn>=1.4.0",
     "category_encoders>=2.6.0",
     "scipy>=0.19.1",
 ]
 
 extras = dict()
 
 # This list should be identical to the list in shapash/report/__init__.py
@@ -62,27 +62,27 @@
 test_requirements = [
     "pytest",
 ]
 
 setup(
     name="shapash",
     version=version_d["__version__"],
-    python_requires=">3.7, <3.12",
+    python_requires=">3.8, <3.13",
     url="https://github.com/MAIF/shapash",
     author="Yann Golhen, Sebastien Bidault, Yann Lagre, Maxime Gendre",
     author_email="yann.golhen@maif.fr",
     description="Shapash is a Python library which aims to make machine learning interpretable and understandable by everyone.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=requirements,
     extras_require=extras,
     license="Apache Software License 2.0",
     keywords="shapash",
```

### Comparing `shapash-2.4.3/shapash/backend/__init__.py` & `shapash-2.5.0/shapash/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/backend/base_backend.py` & `shapash-2.5.0/shapash/backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/backend/lime_backend.py` & `shapash-2.5.0/shapash/backend/lime_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/backend/shap_backend.py` & `shapash-2.5.0/shapash/backend/shap_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/data/data_loader.py` & `shapash-2.5.0/shapash/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/decomposition/contributions.py` & `shapash-2.5.0/shapash/decomposition/contributions.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/explainer/consistency.py` & `shapash-2.5.0/shapash/explainer/consistency.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/explainer/multi_decorator.py` & `shapash-2.5.0/shapash/explainer/multi_decorator.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/explainer/smart_explainer.py` & `shapash-2.5.0/shapash/explainer/smart_explainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,22 @@
         self.features_stability = None
         self.features_compacity = None
         self.contributions = None
         self.explain_data = None
         self.features_imp = None
 
     def compile(
-        self, x, contributions=None, y_pred=None, y_target=None, additional_data=None, additional_features_dict=None
+        self,
+        x,
+        contributions=None,
+        y_pred=None,
+        proba_values=None,
+        y_target=None,
+        additional_data=None,
+        additional_features_dict=None,
     ):
         """
         The compile method is the first step to understand model and
         prediction. It performs the sorting of contributions, the reverse
         preprocessing steps and performs all the calculations necessary for
         a quick display of plots and efficient display of summary of
         explanation. This step can last a few moments with large datasets.
@@ -262,14 +269,19 @@
             generated according to x dataset
         y_pred : pandas.Series or pandas.DataFrame, optional (default: None)
             Prediction values (1 column only).
             The index must be identical to the index of x_init.
             This is an interesting parameter for more explicit outputs.
             Shapash lets users define their own predict,
             as they may wish to set their own threshold (classification)
+        proba_values : pandas.Series or pandas.DataFrame, optional (default: None)
+            Probability values (1 column only).
+            The index must be identical to the index of x_init.
+            This is an interesting parameter for more explicit outputs.
+            Shapash lets users define their own probability values
         y_target : pandas.Series or pandas.DataFrame, optional (default: None)
             Target values (1 column only).
             The index must be identical to the index of x_init.
             This is an interesting parameter for outputs on prediction
         additional_data : pandas.DataFrame, optional (default: None)
             Additional dataset of features outsite the model.
             The index must be identical to the index of x_init.
@@ -287,14 +299,21 @@
             self.backend = backend_cls(
                 model=self.model, preprocessing=self.preprocessing, masker=x, **self.backend_kwargs
             )
         self.x_encoded = handle_categorical_missing(x)
         x_init = inverse_transform(self.x_encoded, self.preprocessing)
         self.x_init = handle_categorical_missing(x_init)
         self.y_pred = check_y(self.x_init, y_pred, y_name="y_pred")
+        if (self.y_pred is None) and (hasattr(self.model, "predict")):
+            self.predict()
+
+        self.proba_values = check_y(self.x_init, proba_values, y_name="proba_values")
+        if (self._case == "classification") and (self.proba_values is None) and (hasattr(self.model, "predict_proba")):
+            self.predict_proba()
+
         self.y_target = check_y(self.x_init, y_target, y_name="y_target")
         self.prediction_error = predict_error(self.y_target, self.y_pred, self._case)
 
         self._get_contributions_from_backend_or_user(x, contributions)
         self.check_contributions()
 
         self.columns_dict = {i: col for i, col in enumerate(self.x_init.columns)}
@@ -401,14 +420,15 @@
             new_colors_dict.update(colors_dict)
         self.colors_dict.update(new_colors_dict)
         self.plot.define_style_attributes(colors_dict=self.colors_dict)
 
     def add(
         self,
         y_pred=None,
+        proba_values=None,
         y_target=None,
         label_dict=None,
         features_dict=None,
         title_story: str = None,
         additional_data=None,
         additional_features_dict=None,
     ):
@@ -419,14 +439,17 @@
         y_pred is needed in the to_pandas method.
         label_dict and features_dict displays allow to display clearer results.
         Parameters
         ----------
         y_pred : pandas.Series, optional (default: None)
             Prediction values (1 column only).
             The index must be identical to the index of x_init.
+        proba_values : pandas.Series, optional (default: None)
+            Probability values (1 column only).
+            The index must be identical to the index of x_init.
         label_dict: dict, optional (default: None)
             Dictionary mapping integer labels to domain names.
         features_dict: dict, optional (default: None)
             Dictionary mapping technical feature names to domain names.
         title_story: str (default: None)
             The default title is empty. You can specify a custom title
             which can be used the webapp, or other methods
@@ -442,14 +465,16 @@
         additional_features_dict : dict
             Dictionary mapping technical feature names to domain names for additional data.
         """
         if y_pred is not None:
             self.y_pred = check_y(self.x_init, y_pred, y_name="y_pred")
             if hasattr(self, "y_target"):
                 self.prediction_error = predict_error(self.y_target, self.y_pred, self._case)
+        if proba_values is not None:
+            self.proba_values = check_y(self.x_init, proba_values, y_name="proba_values")
         if y_target is not None:
             self.y_target = check_y(self.x_init, y_target, y_name="y_target")
             if hasattr(self, "y_pred"):
                 self.prediction_error = predict_error(self.y_target, self.y_pred, self._case)
         if label_dict is not None:
             if isinstance(label_dict, dict) is False:
                 raise ValueError(
@@ -891,15 +916,15 @@
             columns_dict = self.columns_dict
         # Summarize information
         data["summary"] = self.state.summarize(
             data["contrib_sorted"], data["var_dict"], data["x_sorted"], self.mask, columns_dict, self.features_dict
         )
         # Matching with y_pred
         if proba:
-            self.predict_proba() if proba else None
+            self.predict_proba()
             proba_values = self.proba_values
         else:
             proba_values = None
 
         y_pred, summary = keep_right_contributions(
             self.y_pred, data["summary"], self._case, self._classes, self.label_dict, proba_values
         )
@@ -1002,16 +1027,14 @@
         Parameters
         ----------
         settings : dict (default: None)
             A dict describing the default webapp settings values to be used
             Possible settings (dict keys) are 'rows', 'points', 'violin', 'features'
             Values should be positive ints
         """
-        if self.y_pred is None:
-            self.predict()
         self.smartapp = SmartApp(self, settings)
 
     def run_app(
         self, port: int = None, host: str = None, title_story: str = None, settings: dict = None
     ) -> CustomThread:
         """
         run_app method launches the interpretability web app associated with the shapash object.
@@ -1042,16 +1065,14 @@
         --------
         >>> app = xpl.run_app()
         >>> app.kill()
         """
 
         if title_story is not None:
             self.title_story = title_story
-        if self.y_pred is None:
-            self.predict()
         if hasattr(self, "_case"):
             self.smartapp = SmartApp(self, settings)
             if host is None:
                 host = "0.0.0.0"
             if port is None:
                 port = 8050
             host_name = get_host_name()
```

### Comparing `shapash-2.4.3/shapash/explainer/smart_plotter.py` & `shapash-2.5.0/shapash/explainer/smart_plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -945,17 +945,15 @@
             specify the row we want to pred
         label: int (default: None)
         Returns
         -------
         float: Predict or predict_proba value
         """
         if self.explainer._case == "classification":
-            if hasattr(self.explainer.model, "predict_proba"):
-                if not hasattr(self.explainer, "proba_values"):
-                    self.explainer.predict_proba()
+            if self.explainer.proba_values is not None:
                 value = self.explainer.proba_values.iloc[:, [label]].loc[index].values[0]
             else:
                 value = None
         elif self.explainer._case == "regression":
             if self.explainer.y_pred is not None:
                 value = self.explainer.y_pred.loc[index]
             else:
@@ -1233,17 +1231,15 @@
         # Classification Case
         if self.explainer._case == "classification":
             subcontrib = contributions[label_num]
             if self.explainer.y_pred is not None:
                 col_value = self.explainer._classes[label_num]
             subtitle = f"Response: <b>{label_value}</b>"
             # predict proba Color scale
-            if proba and hasattr(self.explainer.model, "predict_proba"):
-                if not hasattr(self.explainer, "proba_values"):
-                    self.explainer.predict_proba()
+            if proba and self.explainer.proba_values is not None:
                 proba_values = self.explainer.proba_values.iloc[:, [label_num]]
                 if not hasattr(self, "pred_colorscale"):
                     self.pred_colorscale = {}
                 if label_num not in self.pred_colorscale:
                     self.pred_colorscale[label_num] = self.tuning_colorscale(proba_values)
                 col_scale = self.pred_colorscale[label_num]
                 # Proba subset:
@@ -1297,21 +1293,21 @@
             metadata = None
         feature_values = feature_values.to_frame()
 
         if self.explainer.y_pred is not None:
             y_pred = self.explainer.y_pred.loc[list_ind]
             # Add labels if exist
             if self.explainer._case == "classification" and self.explainer.label_dict is not None:
-                y_pred = y_pred.applymap(lambda x: self.explainer.label_dict[x])
+                y_pred = y_pred.map(lambda x: self.explainer.label_dict[x])
                 col_value = self.explainer.label_dict[col_value]
             # round predict
             elif self.explainer._case == "regression":
                 if self.round_digit is None:
                     self.tuning_round_digit()
-                y_pred = y_pred.applymap(lambda x: round(x, self.round_digit))
+                y_pred = y_pred.map(lambda x: round(x, self.round_digit))
         else:
             y_pred = None
 
         # selecting the best plot : Scatter, Violin?
         if col_value_count > violin_maxf:
             fig = self.plot_scatter(
                 feature_values,
@@ -3205,20 +3201,15 @@
         list_ind: list
             Contains list of index that we want to plot
         """
         fig = go.Figure()
 
         label_num, _, label_value = self.explainer.check_label_name(label)
         # predict proba Color scale
-        if hasattr(self.explainer.model, "predict_proba"):
-            if not hasattr(self.explainer, "proba_values"):
-                self.explainer.predict_proba()
-            if hasattr(self.explainer.model, "predict"):
-                if not hasattr(self.explainer, "y_pred") or self.explainer.y_pred is None:
-                    self.explainer.predict()
+        if self.explainer.proba_values is not None:
             # Assign proba values of the target
             df_proba_target = self.explainer.proba_values.copy()
             df_proba_target["proba_target"] = df_proba_target.iloc[:, label_num]
             proba_values = df_proba_target[["proba_target"]]
             # Proba subset:
             proba_values = proba_values.loc[list_ind, :]
             target = self.explainer.y_target.loc[list_ind, :]
@@ -3329,17 +3320,14 @@
         ----------
         list_ind: list
             Contains list of index that we want to plot
         """
         fig = go.Figure()
 
         subtitle = None
-        if self.explainer.y_pred is None:
-            if hasattr(self.explainer.model, "predict"):
-                self.explainer.predict()
         prediction_error = self.explainer.prediction_error
         if prediction_error is not None:
             if (self.explainer.y_target == 0).any()[0]:
                 subtitle = "Prediction Error = abs(True Values - Predicted Values)"
             else:
                 subtitle = "Prediction Error = abs(True Values - Predicted Values) / True Values"
             df_equal_bins = prediction_error.describe(percentiles=np.arange(0.1, 1, 0.1).tolist())
@@ -3354,15 +3342,15 @@
 
             y_pred = self.explainer.y_pred.loc[list_ind]
             y_target = self.explainer.y_target.loc[list_ind]
             prediction_error = np.array(prediction_error.loc[list_ind])
             # round predict
             if self.round_digit is None:
                 self.tuning_round_digit()
-            y_pred = y_pred.applymap(lambda x: round(x, self.round_digit))
+            y_pred = y_pred.map(lambda x: round(x, self.round_digit))
 
             hv_text = [
                 f"Id: {x}<br />True Values: {y:,.2f}<br />Predicted Values: {z:,.2f}<br />Prediction Error: {w:,.2f}"
                 for x, y, z, w in zip(
                     y_target.index, y_target.values.flatten(), y_pred.values.flatten(), prediction_error.flatten()
                 )
             ]
```

### Comparing `shapash-2.4.3/shapash/explainer/smart_predictor.py` & `shapash-2.5.0/shapash/explainer/smart_predictor.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/explainer/smart_state.py` & `shapash-2.5.0/shapash/explainer/smart_state.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/manipulation/filters.py` & `shapash-2.5.0/shapash/manipulation/filters.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/manipulation/mask.py` & `shapash-2.5.0/shapash/manipulation/mask.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/manipulation/select_lines.py` & `shapash-2.5.0/shapash/manipulation/select_lines.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         summary = pd.DataFrame(
             [summar[ind] for ind, summar in zip(indexclas, complete_sum)],
             columns=contributions[0].columns,
             index=contributions[0].index,
             dtype=object,
         )
         if label_dict is not None:
-            y_pred = y_pred.applymap(lambda x: label_dict[x])
+            y_pred = y_pred.map(lambda x: label_dict[x])
         if proba_values is not None:
             y_proba = pd.DataFrame(
                 [proba[ind] for ind, proba in zip(indexclas, proba_values.values)],
                 columns=["proba"],
                 index=y_pred.index,
             )
             y_pred = pd.concat([y_pred, y_proba], axis=1)
```

### Comparing `shapash-2.4.3/shapash/manipulation/summarize.py` & `shapash-2.5.0/shapash/manipulation/summarize.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     Returns
     -------
     pd.DataFrame
         Result of the summarize step
     """
     contrib_sum = summarize_el(s_contrib, mask, "contribution_")
-    var_dict_sum = summarize_el(var_dict, mask, "feature_").applymap(
+    var_dict_sum = summarize_el(var_dict, mask, "feature_").map(
         lambda x: features_dict[columns_dict[x]] if not np.isnan(x) else x
     )
     x_sorted_sum = summarize_el(x_sorted, mask, "value_")
 
     # Concatenate pd.DataFrame
     summary = pd.concat([contrib_sum, var_dict_sum, x_sorted_sum], axis=1)
```

### Comparing `shapash-2.4.3/shapash/report/__init__.py` & `shapash-2.5.0/shapash/report/__init__.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/report/base_report.ipynb` & `shapash-2.5.0/shapash/report/base_report.ipynb`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/report/common.py` & `shapash-2.5.0/shapash/report/common.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/report/data_analysis.py` & `shapash-2.5.0/shapash/report/data_analysis.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/report/generation.py` & `shapash-2.5.0/shapash/report/generation.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/report/html/dropdown.html` & `shapash-2.5.0/shapash/report/html/dropdown.html`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/report/html/explainability.html` & `shapash-2.5.0/shapash/report/html/explainability.html`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/report/html/univariate.html` & `shapash-2.5.0/shapash/report/html/univariate.html`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/report/plots.py` & `shapash-2.5.0/shapash/report/plots.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/report/project_report.py` & `shapash-2.5.0/shapash/report/project_report.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/report/template/custom/index.html.j2` & `shapash-2.5.0/shapash/report/template/custom/index.html.j2`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/report/visualisation.py` & `shapash-2.5.0/shapash/report/visualisation.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/style/colors.json` & `shapash-2.5.0/shapash/style/colors.json`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/style/style_utils.py` & `shapash-2.5.0/shapash/style/style_utils.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/utils/category_encoder_backend.py` & `shapash-2.5.0/shapash/utils/category_encoder_backend.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/utils/check.py` & `shapash-2.5.0/shapash/utils/check.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/utils/columntransformer_backend.py` & `shapash-2.5.0/shapash/utils/columntransformer_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 sklearn columntransformer
 """
 
 import numpy as np
 import pandas as pd
+from sklearn.preprocessing import FunctionTransformer
 
 from shapash.utils.category_encoder_backend import (
     category_encoder_binary,
     dummies_category_encoder,
     get_col_mapping_ce,
     inv_transform_ce,
     inv_transform_ordinal,
@@ -87,15 +88,15 @@
 
             # For category encoding we use the mapping
             elif str(type(ct_encoding)) in supported_category_encoder:
                 frame, init = inv_transform_ce_in_ct(x_in, init, name_encoding, col_encoding, ct_encoding)
 
             # columns not encode
             elif name_encoding == "remainder":
-                if ct_encoding == "passthrough":
+                if isinstance(ct_encoding, FunctionTransformer):
                     nb_col = len(col_encoding)
                     frame = x_in.iloc[:, init : init + nb_col]
                 else:
                     frame = pd.DataFrame()
 
             else:
                 raise Exception(f"{ct_encoding} is not supported yet.")
@@ -245,15 +246,15 @@
                     nb_col = len(colname_output)
                     frame = x_contrib.iloc[:, init : init + nb_col]
                     frame.columns = colname_output
                     rst = pd.concat([rst, frame], axis=1)
                     init += nb_col
 
             elif name_encoding == "remainder":
-                if ct_encoding == "passthrough":
+                if isinstance(ct_encoding, FunctionTransformer):
                     nb_col = len(col_encoding)
                     frame = x_contrib.iloc[:, init : init + nb_col]
                     rst = pd.concat([rst, frame], axis=1)
                     init += nb_col
             else:
                 raise Exception(f"{encoding.__class__.__name__} not supported, no inverse done.")
         return rst
@@ -362,15 +363,17 @@
 
     Returns
     -------
     feature_names: list
         List of returned features names when ColumnTransformer is applied.
     """
     feature_names = []
-    l_transformers = list(column_transformer._iter(fitted=True))
+    l_transformers = list(
+        column_transformer._iter(fitted=True, column_as_labels=False, skip_drop=True, skip_empty_columns=True)
+    )
 
     for name, trans, column, _ in l_transformers:
         feature_names.extend(get_names(name, trans, column, column_transformer))
 
     return feature_names
 
 
@@ -459,17 +462,14 @@
                     for _ in dict_mapping_ce[f_name]:
                         dict_col_mapping[name + "_" + f_name].append(x_encoded.columns.to_list()[idx_encoded])
                         idx_encoded += 1
 
             else:
                 raise NotImplementedError(f"Estimator not supported : {estimator}")
 
-        elif estimator == "passthrough":
-            try:
-                features_out = encoder.feature_names_in_[features]
-            except Exception:
-                features_out = encoder._feature_names_in[features]  # for oldest sklearn version
+        elif isinstance(estimator, FunctionTransformer):
+            features_out = encoder.feature_names_in_[features]
             for f_name in features_out:
                 dict_col_mapping[f_name] = [x_encoded.columns.to_list()[idx_encoded]]
                 idx_encoded += 1
 
     return dict_col_mapping
```

### Comparing `shapash-2.4.3/shapash/utils/explanation_metrics.py` & `shapash-2.5.0/shapash/utils/explanation_metrics.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/utils/io.py` & `shapash-2.5.0/shapash/utils/io.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/utils/load_smartpredictor.py` & `shapash-2.5.0/shapash/utils/load_smartpredictor.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/utils/model.py` & `shapash-2.5.0/shapash/utils/model.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/utils/model_synoptic.py` & `shapash-2.5.0/shapash/utils/model_synoptic.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/utils/threading.py` & `shapash-2.5.0/shapash/utils/threading.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/utils/transform.py` & `shapash-2.5.0/shapash/utils/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Transform Module
 """
+
 import re
 
 import numpy as np
 import pandas as pd
+from sklearn.preprocessing import FunctionTransformer
 
 from shapash.utils.category_encoder_backend import (
     get_col_mapping_ce,
     inv_transform_ce,
     supported_category_encoder,
     transform_ce,
 )
@@ -181,15 +183,15 @@
         if str(type(enc)) in columntransformer:
             use_ct = True
             for encoding in enc.transformers_:
                 ct_encoding = encoding[1]
                 if (str(type(ct_encoding)) not in supported_sklearn) and (
                     str(type(ct_encoding)) not in supported_category_encoder
                 ):
-                    if str(type(ct_encoding)) != "<class 'str'>":
+                    if not isinstance(ct_encoding, str) and not isinstance(ct_encoding, FunctionTransformer):
                         raise ValueError("One of the encoders used in ColumnTransformers isn't supported.")
 
         elif str(type(enc)) in supported_category_encoder:
             use_ce = True
 
         # Check we have a list of dict
         elif isinstance(enc, list):
```

### Comparing `shapash-2.4.3/shapash/utils/utils.py` & `shapash-2.5.0/shapash/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/webapp/assets/favicon.ico` & `shapash-2.5.0/shapash/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/webapp/assets/jquery.js` & `shapash-2.5.0/shapash/webapp/assets/jquery.js`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/webapp/assets/material-icons.css` & `shapash-2.5.0/shapash/webapp/assets/material-icons.css`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/webapp/assets/reload.png` & `shapash-2.5.0/shapash/webapp/assets/reload.png`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/webapp/assets/settings.png` & `shapash-2.5.0/shapash/webapp/assets/settings.png`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/webapp/assets/shapash-fond-fonce.png` & `shapash-2.5.0/shapash/webapp/assets/shapash-fond-fonce.png`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/webapp/assets/style.css` & `shapash-2.5.0/shapash/webapp/assets/style.css`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/webapp/smart_app.py` & `shapash-2.5.0/shapash/webapp/smart_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,20 +112,20 @@
             if self.explainer._case == "regression":
                 self.special_cols.append("_error_")
         self.explainer.features_imp = self.explainer.state.compute_features_import(self.explainer.contributions)
         if self.explainer._case == "classification":
             self.label = self.explainer.check_label_name(len(self.explainer._classes) - 1, "num")[1]
             self.selected_feature = self.explainer.features_imp[-1].idxmax()
             self.max_threshold = int(
-                max([x.applymap(lambda x: round_to_k(x, k=1)).max().max() for x in self.explainer.contributions])
+                max([x.map(lambda x: round_to_k(x, k=1)).max().max() for x in self.explainer.contributions])
             )
         else:
             self.label = None
             self.selected_feature = self.explainer.features_imp.idxmax()
-            self.max_threshold = int(self.explainer.contributions.applymap(lambda x: round_to_k(x, k=1)).max().max())
+            self.max_threshold = int(self.explainer.contributions.map(lambda x: round_to_k(x, k=1)).max().max())
         self.list_index = []
         self.subset = None
         self.last_click_data = None
 
         # DATA
         self.explanations = Explanations()  # To get explanations of "?" buttons
         self.dataframe = pd.DataFrame()
```

### Comparing `shapash-2.4.3/shapash/webapp/utils/MyGraph.py` & `shapash-2.5.0/shapash/webapp/utils/MyGraph.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/webapp/utils/callbacks.py` & `shapash-2.5.0/shapash/webapp/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/webapp/utils/explanations.py` & `shapash-2.5.0/shapash/webapp/utils/explanations.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/webapp/utils/utils.py` & `shapash-2.5.0/shapash/webapp/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/webapp/webapp_launch.py` & `shapash-2.5.0/shapash/webapp/webapp_launch.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash/webapp/webapp_launch_DVF.py` & `shapash-2.5.0/shapash/webapp/webapp_launch_DVF.py`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash.egg-info/PKG-INFO` & `shapash-2.5.0/shapash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: shapash
-Version: 2.4.3
+Version: 2.5.0
 Summary: Shapash is a Python library which aims to make machine learning interpretable and understandable by everyone.
 Home-page: https://github.com/MAIF/shapash
 Author: Yann Golhen, Sebastien Bidault, Yann Lagre, Maxime Gendre
 Author-email: yann.golhen@maif.fr
 License: Apache Software License 2.0
 Keywords: shapash
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >3.7, <3.12
+Requires-Python: >3.8, <3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plotly>=5.0.0
 Requires-Dist: matplotlib>=3.2.0
 Requires-Dist: numpy>1.18.0
-Requires-Dist: pandas>1.0.2
-Requires-Dist: shap<0.45.0,>=0.38.1
+Requires-Dist: pandas>=2.1.0
+Requires-Dist: shap>=0.45.0
 Requires-Dist: Flask<2.3.0
 Requires-Dist: dash>=2.3.1
 Requires-Dist: dash-bootstrap-components>=1.1.0
 Requires-Dist: dash-core-components>=2.0.0
 Requires-Dist: dash-daq>=0.5.0
 Requires-Dist: dash-html-components>=2.0.0
 Requires-Dist: dash-renderer==1.8.3
 Requires-Dist: dash-table>=5.0.0
 Requires-Dist: nbformat>4.2.0
 Requires-Dist: numba>=0.53.1
-Requires-Dist: scikit-learn<1.4,>=1.0.1
+Requires-Dist: scikit-learn>=1.4.0
 Requires-Dist: category_encoders>=2.6.0
 Requires-Dist: scipy>=0.19.1
 Provides-Extra: report
 Requires-Dist: nbconvert>=6.0.7; extra == "report"
 Requires-Dist: papermill>=2.0.0; extra == "report"
 Requires-Dist: jupyter-client>=7.4.0; extra == "report"
 Requires-Dist: seaborn==0.12.2; extra == "report"
@@ -193,15 +193,15 @@
 
 Shapash can use category-encoders object, sklearn ColumnTransformer or simply features dictionary. <br />
 - Category_encoder: *OneHotEncoder*, *OrdinalEncoder*, *BaseNEncoder*, *BinaryEncoder*, *TargetEncoder*
 - Sklearn ColumnTransformer: *OneHotEncoder*, *OrdinalEncoder*, *StandardScaler*, *QuantileTransformer*, *PowerTransformer*
 
 ## 🛠 Installation
 
-Shapash is intended to work with Python versions 3.8 to 3.11. Installation can be done with pip:
+Shapash is intended to work with Python versions 3.9 to 3.12. Installation can be done with pip:
 
 ```bash
 pip install shapash
 ```
 
 In order to generate the Shapash Report some extra requirements are needed.
 You can install these using the following command :
```

#### html2text {}

```diff
@@ -1,35 +1,34 @@
-Metadata-Version: 2.1 Name: shapash Version: 2.4.3 Summary: Shapash is a Python
+Metadata-Version: 2.1 Name: shapash Version: 2.5.0 Summary: Shapash is a Python
 library which aims to make machine learning interpretable and understandable by
 everyone. Home-page: https://github.com/MAIF/shapash Author: Yann Golhen,
 Sebastien Bidault, Yann Lagre, Maxime Gendre Author-email: yann.golhen@maif.fr
 License: Apache Software License 2.0 Keywords: shapash Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Operating System :: OS Independent Requires-Python: >3.7, <3.12 Description-
+Operating System :: OS Independent Requires-Python: >3.8, <3.13 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: plotly>=5.0.0
 Requires-Dist: matplotlib>=3.2.0 Requires-Dist: numpy>1.18.0 Requires-Dist:
-pandas>1.0.2 Requires-Dist: shap<0.45.0,>=0.38.1 Requires-Dist: Flask<2.3.0
-Requires-Dist: dash>=2.3.1 Requires-Dist: dash-bootstrap-components>=1.1.0
-Requires-Dist: dash-core-components>=2.0.0 Requires-Dist: dash-daq>=0.5.0
-Requires-Dist: dash-html-components>=2.0.0 Requires-Dist: dash-renderer==1.8.3
-Requires-Dist: dash-table>=5.0.0 Requires-Dist: nbformat>4.2.0 Requires-Dist:
-numba>=0.53.1 Requires-Dist: scikit-learn<1.4,>=1.0.1 Requires-Dist:
-category_encoders>=2.6.0 Requires-Dist: scipy>=0.19.1 Provides-Extra: report
-Requires-Dist: nbconvert>=6.0.7; extra == "report" Requires-Dist:
-papermill>=2.0.0; extra == "report" Requires-Dist: jupyter-client>=7.4.0; extra
-== "report" Requires-Dist: seaborn==0.12.2; extra == "report" Requires-Dist:
-notebook; extra == "report" Requires-Dist: Jinja2>=2.11.0; extra == "report"
-Requires-Dist: phik; extra == "report" Provides-Extra: xgboost Requires-Dist:
-xgboost>=1.0.0; extra == "xgboost" Provides-Extra: lightgbm Requires-Dist:
-lightgbm>=2.3.0; extra == "lightgbm" Provides-Extra: catboost Requires-Dist:
-catboost>=1.0.1; extra == "catboost" Provides-Extra: lime Requires-Dist:
-lime>=0.2.0.0; extra == "lime"
+pandas>=2.1.0 Requires-Dist: shap>=0.45.0 Requires-Dist: Flask<2.3.0 Requires-
+Dist: dash>=2.3.1 Requires-Dist: dash-bootstrap-components>=1.1.0 Requires-
+Dist: dash-core-components>=2.0.0 Requires-Dist: dash-daq>=0.5.0 Requires-Dist:
+dash-html-components>=2.0.0 Requires-Dist: dash-renderer==1.8.3 Requires-Dist:
+dash-table>=5.0.0 Requires-Dist: nbformat>4.2.0 Requires-Dist: numba>=0.53.1
+Requires-Dist: scikit-learn>=1.4.0 Requires-Dist: category_encoders>=2.6.0
+Requires-Dist: scipy>=0.19.1 Provides-Extra: report Requires-Dist:
+nbconvert>=6.0.7; extra == "report" Requires-Dist: papermill>=2.0.0; extra ==
+"report" Requires-Dist: jupyter-client>=7.4.0; extra == "report" Requires-Dist:
+seaborn==0.12.2; extra == "report" Requires-Dist: notebook; extra == "report"
+Requires-Dist: Jinja2>=2.11.0; extra == "report" Requires-Dist: phik; extra ==
+"report" Provides-Extra: xgboost Requires-Dist: xgboost>=1.0.0; extra ==
+"xgboost" Provides-Extra: lightgbm Requires-Dist: lightgbm>=2.3.0; extra ==
+"lightgbm" Provides-Extra: catboost Requires-Dist: catboost>=1.0.1; extra ==
+"catboost" Provides-Extra: lime Requires-Dist: lime>=0.2.0.0; extra == "lime"
  [https://raw.githubusercontent.com/MAIF/shapash/master/docs/_static/shapash-
                                   resize.png]
                _[_t_e_s_t_s_]_[_p_y_p_i_]_[_d_o_w_n_l_o_a_d_s_]_[_p_y_v_e_r_s_i_o_n_]_[_l_i_c_e_n_s_e_]_[_d_o_c_]
 ## ð Overview Shapash is a Python library designed to **make machine
 learning interpretable and comprehensible for everyone**. It offers various
 visualizations with clear and explicit labels that are easily understood by
 all. With Shapash, you can generate a **Webapp** that simplifies the
@@ -177,16 +176,16 @@
 of how to provide contributions to Shapash. An [issue](https://github.com/MAIF/
 shapash/issues/488) has been created to enhance this use case. Shapash can use
 category-encoders object, sklearn ColumnTransformer or simply features
 dictionary.
 - Category_encoder: *OneHotEncoder*, *OrdinalEncoder*, *BaseNEncoder*,
 *BinaryEncoder*, *TargetEncoder* - Sklearn ColumnTransformer: *OneHotEncoder*,
 *OrdinalEncoder*, *StandardScaler*, *QuantileTransformer*, *PowerTransformer*
-## ð  Installation Shapash is intended to work with Python versions 3.8 to
-3.11. Installation can be done with pip: ```bash pip install shapash ``` In
+## ð  Installation Shapash is intended to work with Python versions 3.9 to
+3.12. Installation can be done with pip: ```bash pip install shapash ``` In
 order to generate the Shapash Report some extra requirements are needed. You
 can install these using the following command : ```bash pip install shapash
 [report] ``` If you encounter **compatibility issues** you may check the
 corresponding section in the Shapash documentation [here](https://
 shapash.readthedocs.io/en/latest/installation-instructions/index.html). ## ð
 Quickstart The 4 steps to display results: - Step 1: Declare SmartExplainer
 Object > There 1 mandatory parameter in compile method: Model > You can declare
```

### Comparing `shapash-2.4.3/shapash.egg-info/SOURCES.txt` & `shapash-2.5.0/shapash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shapash-2.4.3/shapash.egg-info/requires.txt` & `shapash-2.5.0/shapash.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 plotly>=5.0.0
 matplotlib>=3.2.0
 numpy>1.18.0
-pandas>1.0.2
-shap<0.45.0,>=0.38.1
+pandas>=2.1.0
+shap>=0.45.0
 Flask<2.3.0
 dash>=2.3.1
 dash-bootstrap-components>=1.1.0
 dash-core-components>=2.0.0
 dash-daq>=0.5.0
 dash-html-components>=2.0.0
 dash-renderer==1.8.3
 dash-table>=5.0.0
 nbformat>4.2.0
 numba>=0.53.1
-scikit-learn<1.4,>=1.0.1
+scikit-learn>=1.4.0
 category_encoders>=2.6.0
 scipy>=0.19.1
 
 [catboost]
 catboost>=1.0.1
 
 [lightgbm]
```

