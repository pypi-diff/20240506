# Comparing `tmp/dataanalysistoolkit-1.1.1.tar.gz` & `tmp/dataanalysistoolkit-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataanalysistoolkit-1.1.1.tar", last modified: Sun Jan  7 05:07:39 2024, max compression
+gzip compressed data, was "dataanalysistoolkit-1.2.0.tar", last modified: Mon May  6 16:52:10 2024, max compression
```

## Comparing `dataanalysistoolkit-1.1.1.tar` & `dataanalysistoolkit-1.2.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:39.526431 dataanalysistoolkit-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-01-07 05:07:39.526431 dataanalysistoolkit-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-07 05:07:39.526431 dataanalysistoolkit-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:39.522431 dataanalysistoolkit-1.1.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/data_analysis_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:39.522431 dataanalysistoolkit-1.1.1/src/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/data_sources/api_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/data_sources/excel_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/data_sources/sql_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:39.526431 dataanalysistoolkit-1.1.1/src/dataanalysistoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-01-07 05:07:39.000000 dataanalysistoolkit-1.1.1/src/dataanalysistoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-01-07 05:07:39.000000 dataanalysistoolkit-1.1.1/src/dataanalysistoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-07 05:07:39.000000 dataanalysistoolkit-1.1.1/src/dataanalysistoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-07 05:07:39.000000 dataanalysistoolkit-1.1.1/src/dataanalysistoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:39.526431 dataanalysistoolkit-1.1.1/src/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/formatters/data_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:39.526431 dataanalysistoolkit-1.1.1/src/generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/generators/csv_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/generators/generate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/generators/report_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:39.526431 dataanalysistoolkit-1.1.1/src/integrators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/integrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/integrators/data_integrator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:39.526431 dataanalysistoolkit-1.1.1/src/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/model/feature_engineer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/model/model_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:39.526431 dataanalysistoolkit-1.1.1/src/preprocessor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/preprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/preprocessor/data_prep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:39.526431 dataanalysistoolkit-1.1.1/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/utils/data_imputer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:39.526431 dataanalysistoolkit-1.1.1/src/visualizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/visualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/src/visualizer/data_visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 05:07:39.526431 dataanalysistoolkit-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-01-07 05:07:27.000000 dataanalysistoolkit-1.1.1/tests/test_data_analysis_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:52:10.039099 dataanalysistoolkit-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-05-06 16:52:10.039099 dataanalysistoolkit-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:52:10.039099 dataanalysistoolkit-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:52:10.035099 dataanalysistoolkit-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:52:10.039099 dataanalysistoolkit-1.2.0/src/DataAnalysisToolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-05-06 16:52:10.000000 dataanalysistoolkit-1.2.0/src/DataAnalysisToolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-06 16:52:10.000000 dataanalysistoolkit-1.2.0/src/DataAnalysisToolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:52:10.000000 dataanalysistoolkit-1.2.0/src/DataAnalysisToolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-06 16:52:10.000000 dataanalysistoolkit-1.2.0/src/DataAnalysisToolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-06 16:52:10.000000 dataanalysistoolkit-1.2.0/src/DataAnalysisToolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:52:10.035099 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/data_analysis_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:52:10.035099 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/data_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/data_sources/api_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/data_sources/excel_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/data_sources/sql_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:52:10.035099 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/formatters/data_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:52:10.039099 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/generators/csv_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/generators/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/generators/report_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:52:10.039099 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/integrators/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/integrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/integrators/data_integrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:52:10.039099 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/model/feature_engineer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/model/model_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:52:10.039099 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/preprocessor/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/preprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/preprocessor/data_prep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:52:10.039099 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/utils/data_imputer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:52:10.039099 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/visualizer/data_visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:52:10.039099 dataanalysistoolkit-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-06 16:52:01.000000 dataanalysistoolkit-1.2.0/tests/test_data_analysis_toolkit.py
```

### Comparing `dataanalysistoolkit-1.1.1/PKG-INFO` & `dataanalysistoolkit-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,10 @@
-Metadata-Version: 2.1
-Name: dataanalysistoolkit
-Version: 1.1.1
-Summary: The `DataAnalysisToolkit` project is a Python-based data analysis tool designed to streamline various data analysis tasks. It allows users to load data from CSV files and perform operations such as statistical calculations, outlier detection, data cleaning, and visualization.
-Author-email: Thaddeus Thomas <thaddeus.r.thomas@gmail.com>
-Project-URL: Homepage, https://github.com/thomasthaddeus/dataanalysistoolkit
-Project-URL: Issues, https://github.com/thomasthaddeus/dataanalysistoolkit/issues
-Project-URL: Documentation, https://dataanalysistoolkit.readthedocs.io/en/latest/
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Education
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 # Data Analysis Toolkit
 
-[![Upload Python Package](https://github.com/thomasthaddeus/DataAnalysisToolkit/actions/workflows/python-publish.yml/badge.svg)](https://github.com/thomasthaddeus/DataAnalysisToolkit/actions/workflows/python-publish.yml) [![PyPI](https://img.shields.io/pypi/v/DataAnalysisToolkit.svg)](https://pypi.org/project/DataAnalysisToolkit/) ![License](https://img.shields.io/github/license/thomasthaddeus/DataAnalysisToolkit.svg) ![Python Version](https://img.shields.io/pypi/pyversions/DataAnalysisToolkit.svg) ![Code Size](https://img.shields.io/github/languages/code-size/thomasthaddeus/DataAnalysisToolkit.svg) ![Last Commit](https://img.shields.io/github/last-commit/thomasthaddeus/DataAnalysisToolkit.svg) ![Issues](https://img.shields.io/github/issues-raw/thomasthaddeus/DataAnalysisToolkit.svg) ![Pull Requests](https://img.shields.io/github/issues-pr/thomasthaddeus/DataAnalysisToolkit.svg)
+[![Upload Python Package](https://github.com/thomasthaddeus/DataAnalysisToolkit/actions/workflows/python-publish.yml/badge.svg)](https://github.com/thomasthaddeus/DataAnalysisToolkit/actions/workflows/python-publish.yml) [![PyPI](https://img.shields.io/pypi/v/DataAnalysisToolkit.svg)](https://pypi.org/project/DataAnalysisToolkit/) ![License](https://img.shields.io/github/license/thomasthaddeus/DataAnalysisToolkit.svg) ![Python Version](https://img.shields.io/pypi/pyversions/DataAnalysisToolkit.svg) ![Code Size](https://img.shields.io/github/languages/code-size/thomasthaddeus/DataAnalysisToolkit.svg) ![Last Commit](https://img.shields.io/github/last-commit/thomasthaddeus/DataAnalysisToolkit.svg) ![Issues](https://img.shields.io/github/issues-raw/thomasthaddeus/DataAnalysisToolkit.svg) ![Pull Requests](https://img.shields.io/github/issues-pr/thomasthaddeus/DataAnalysisToolkit.svg) [![Documentation Status](https://readthedocs.org/projects/dataanalysistoolkit/badge/?version=latest)](https://dataanalysistoolkit.readthedocs.io/en/latest/?badge=latest)
 
 DataAnalysisToolkit is a comprehensive Python package offering a suite of tools designed for efficient data analysis. This toolkit simplifies tasks such as loading CSV data, performing statistical analysis, cleaning data, and visualizing results. It's an ideal tool for data analysts, scientists, and anyone looking to dive into data exploration and machine learning.
 
 ## Features
 
 - **Data Loading**: Load data directly from CSV files into a Python environment.
 - **Statistical Analysis**: Perform calculations like mean, median, mode, and trimmed mean.
@@ -47,14 +24,16 @@
 
 This toolkit is an asset for conducting preliminary data analysis, and it seamlessly integrates into larger data processing workflows.
 
 ## Getting Started
 
 Here's how you can get started with DataAnalysisToolkit:
 
+<!-- TODO: This coding example needs updated to the most recent release of the package. -->
+
 ```python
 from data_analysis_toolkit import DataAnalysisToolkit
 
 # Initialize the analyzer with the path to a CSV file
 analyzer = DataAnalysisToolkit('../data/test.csv')
 
 
@@ -91,15 +70,15 @@
 
 ```bash
 pip install dataanalysistoolkit
 ```
 
 ## Documentation
 
-For detailed documentation, examples, and usage guides, please visit [DataAnalysisToolkit Documentation](https://github.com/thomasthaddeus/DataAnalysisToolkit/wiki).
+For detailed documentation, examples, and usage guides, please visit [DataAnalysisToolkit Documentation](https://dataanalysistoolkit.readthedocs.io/en/latest/).
 
 ## Contributing
 
 Contributions are welcome! For guidelines on how to contribute, please refer to our [Contribution Guide](https://github.com/thomasthaddeus/DataAnalysisToolkit/CONTRIBUTING.md).
 
 ## License
```

### Comparing `dataanalysistoolkit-1.1.1/src/data_analysis_toolkit.py` & `dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/data_analysis_toolkit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,17 @@
-# MIT License
-#
-# Copyright (c) 2023 Thaddeus Thomas
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
 """data_analysis_toolkit.py
 
 This module contains a class, DataAnalysisToolkit, for performing various data
 analysis tasks on a CSV file. The class is able to load data, calculate various
 statistics, detect outliers, handle missing values, drop duplicates, encode
 categorical features, split data into training and testing sets, visualize data,
 generate reports, preprocess data, and impute missing values.
 
+TODO: Update the example and usage of this program.
+
 Example usage:
 
     from data_analysis_toolkit import DataAnalysisToolkit
 
     # Initialize the analyzer with the path to a CSV file.
     analyzer = DataAnalysisToolkit('path_to_your_file.csv')
 
@@ -74,35 +55,44 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 from scipy.stats import trim_mean, zscore
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import LabelEncoder
 
 # Importing modules from the project's subdirectories
-from generators.report_generator import ReportGenerator
-from model.feature_engineer import FeatureEngineer
-from model.model_evaluator import ModelEvaluator
-from preprocessor.data_prep import DataPreprocessor
-from utils.data_imputer import DataImputer
-from visualizer.data_visualizer import DataVisualizer
+from .generators import ReportGenerator
+from .model import FeatureEngineer, ModelEvaluator
+from .preprocessor import DataPreprocessor
+from .utils import DataImputer
+from .visualizer import DataVisualizer
 
 
 class DataAnalysisToolkit:
     """
     A class to perform various data analysis tasks including loading data,
     calculating statistics, detecting outliers, visualizing data, cleaning data,
     engineering features, splitting data, and exporting data.
     """
 
     def __init__(self, filename):
+        """
+        __init__ _summary_
+
+        _extended_summary_
+
+        Args:
+            filename (_type_): _description_
+        """
         self.data = self.load_data(filename)
-        self.visualizer = DataVisualizer(self.data)
+        self.visualizer = DataVisualizer(self.data, config_path='.conf/plot_config.json')
         self.imputer = DataImputer(self.data)
         self.preprocessor = DataPreprocessor(self.data)
         self.feature_engineer = FeatureEngineer(self.data)
+        # No value for argument 'X_test' in constructor callPylintE1120:no-value-for-parameter
+        # No value for argument 'y_test' in constructor callPylintE1120:no-value-for-parameter
         self.evaluator = ModelEvaluator(self.data)
         self.report_generator = ReportGenerator(self.data)
 
     @property
     def data(self):
         return self._data
 
@@ -280,18 +270,18 @@
     def split_data(self, target_column, test_size=0.2, random_state=None):
         """
         Split the data into training and testing sets.
 
         Args:
             target_column (str): The name of the target (dependent) column.
             test_size (float, optional): The proportion of the dataset to
-            include in the test split. Default is 0.2.
+              include in the test split. Default is 0.2.
             random_state (int, optional): Controls the shuffling applied to the
-            data before applying the split. Pass an int for reproducible output
-            across multiple function calls.
+              data before applying the split. Pass an int for reproducible
+              output across multiple function calls.
 
         Returns:
             tuple: A tuple containing the training and testing data (X_train,
             X_test, y_train, y_test).
         """
         X = self._data.drop(target_column, axis=1)
         y = self._data[target_column]
```

### Comparing `dataanalysistoolkit-1.1.1/src/data_sources/api_connector.py` & `dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/data_sources/api_connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,88 +1,98 @@
-"""api_connector.py
+"""data_sources/api_connector.py
 _summary_
 
 _extended_summary_
 
 Returns:
     _type_: _description_
 
 # Example usage
 connector = APIConnector('https://api.example.com', auth=('username', 'password'))
 response = connector.get('endpoint', params={'key': 'value'})
 update_response = connector.put('endpoint', json={'key': 'updated_value'})
 delete_response = connector.delete('endpoint', params={'key': 'value'})
 patch_response = connector.patch('endpoint', json={'key': 'new_value'})
 print(response.json())
+
+response.raise_for_status()  # Will raise an HTTPError if the HTTP request
+                               returned an unsuccessful status code
 """
 
 import requests
 
+
 class APIConnector:
     """
      _summary_
 
     _extended_summary_
     """
+
     def __init__(self, base_url, auth=None):
         """
         Initialize the APIConnector with the base URL and optional authentication.
 
         Args:
             base_url (str): The base URL for the API.
-            auth (tuple, optional): A tuple for authentication, typically (username, password) or an API token.
+            auth (tuple, optional): A tuple for authentication, typically
+              (username, password) or an API token.
         """
         self.base_url = base_url
         self.auth = auth
         self.session = requests.Session()
         if auth:
             self.session.auth = auth
 
     def get(self, endpoint, params=None):
         """
         Send a GET request to the API.
 
         Args:
             endpoint (str): The API endpoint to send the request to.
-            params (dict, optional): A dictionary of parameters to send with the request.
+            params (dict, optional): A dictionary of parameters to send with
+              the request.
 
         Returns:
             Response: The response from the API.
         """
         url = f"{self.base_url}/{endpoint}"
         response = self.session.get(url, params=params)
-        response.raise_for_status()  # Will raise an HTTPError if the HTTP request returned an unsuccessful status code
+        response.raise_for_status()
         return response
 
     def post(self, endpoint, data=None, json=None):
         """
         Send a POST request to the API.
 
         Args:
             endpoint (str): The API endpoint to send the request to.
-            data (dict, optional): A dictionary of data to send in the body of the request.
-            json (dict, optional): A JSON serializable object to send in the body of the request.
+            data (dict, optional): A dictionary of data to send in the body of
+              the request.
+            json (dict, optional): A JSON serializable object to send in the
+              body of the request.
 
         Returns:
             Response: The response from the API.
         """
         url = f"{self.base_url}/{endpoint}"
         response = self.session.post(url, data=data, json=json)
         response.raise_for_status()
         return response
 
-
     def put(self, endpoint, data=None, json=None):
         """
         Send a PUT request to the API.
 
         Args:
             endpoint (str): The API endpoint to send the request to.
-            data (dict, optional): A dictionary of data to send in the body of the request.
-            json (dict, optional): A JSON serializable object to send in the body of the request.
+            data (dict, optional): A dictionary of data to send in the body of
+              the request.
+            json (dict, optional): A JSON serializable object to send in the
+              body of the request.
 
         Returns:
             Response: The response from the API.
         """
         url = f"{self.base_url}/{endpoint}"
         response = self.session.put(url, data=data, json=json)
         response.raise_for_status()
@@ -90,15 +100,16 @@
 
     def delete(self, endpoint, params=None):
         """
         Send a DELETE request to the API.
 
         Args:
             endpoint (str): The API endpoint to send the request to.
-            params (dict, optional): A dictionary of parameters to send with the request.
+            params (dict, optional): A dictionary of parameters to send with
+              the request.
 
         Returns:
             Response: The response from the API.
         """
         url = f"{self.base_url}/{endpoint}"
         response = self.session.delete(url, params=params)
         response.raise_for_status()
@@ -106,16 +117,18 @@
 
     def patch(self, endpoint, data=None, json=None):
         """
         Send a PATCH request to the API.
 
         Args:
             endpoint (str): The API endpoint to send the request to.
-            data (dict, optional): A dictionary of data to send in the body of the request.
-            json (dict, optional): A JSON serializable object to send in the body of the request.
+            data (dict, optional): A dictionary of data to send in the body of
+              the request.
+            json (dict, optional): A JSON serializable object to send in the
+              body of the request.
 
         Returns:
             Response: The response from the API.
         """
         url = f"{self.base_url}/{endpoint}"
         response = self.session.patch(url, data=data, json=json)
         response.raise_for_status()
```

### Comparing `dataanalysistoolkit-1.1.1/src/formatters/data_formatter.py` & `dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/formatters/data_formatter.py`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.1.1/src/generators/csv_data_generator.py` & `dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/generators/csv_data_generator.py`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.1.1/src/generators/generate_data.py` & `dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/generators/generate_data.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,33 +11,39 @@
 Random choice of 'x', 'y', 'z' in column 'H'
 Some missing values have been introduced in columns 'C' and 'G'.
 """
 
 import numpy as np
 import pandas as pd
 
-# Number of data points
-n = 100
+def gen_data(n=100):
+    """
+    gen_data _summary_
+
+    _extended_summary_
+
+    Args:
+        n (int, optional): Number of data points to be created. Defaults to 100.
+    """
+    # Generating random data
+    data = {
+        "A": np.random.randint(1, 100, n),  # Random integers between 1 and 100
+        "B": np.random.choice(list("abcdefghij"), n),  # Random choice of letters
+        "C": np.random.normal(0, 1, n),  # Random floats from a normal distribution
+        "D": np.random.choice([1, 2, 3], n),  # Random choice of 1, 2, 3
+        "E": np.random.randint(1, 100, n),  # Random integers between 1 and 100
+        "F": np.random.choice(
+            ["apple", "banana", "cherry", "date", "elderberry", "fig"], n
+        ),  # Random choice of fruits
+        "G": np.random.uniform(1, 5, n),  # Random floats from a uniform distribution
+        "H": np.random.choice(["x", "y", "z"], n),  # Random choice of 'x', 'y', 'z'
+    }
+
+    # Converting to a DataFrame
+    df = pd.DataFrame(data)
+
+    # Introducing some missing values in columns 'C' and 'G'
+    df.loc[np.random.choice(df.index, size=int(0.1 * n)), "C"] = np.nan
+    df.loc[np.random.choice(df.index, size=int(0.1 * n)), "G"] = np.nan
 
-# Generating random data
-data = {
-    "A": np.random.randint(1, 100, n),  # Random integers between 1 and 100
-    "B": np.random.choice(list("abcdefghij"), n),  # Random choice of letters
-    "C": np.random.normal(0, 1, n),  # Random floats from a normal distribution
-    "D": np.random.choice([1, 2, 3], n),  # Random choice of 1, 2, 3
-    "E": np.random.randint(1, 100, n),  # Random integers between 1 and 100
-    "F": np.random.choice(
-        ["apple", "banana", "cherry", "date", "elderberry", "fig"], n
-    ),  # Random choice of fruits
-    "G": np.random.uniform(1, 5, n),  # Random floats from a uniform distribution
-    "H": np.random.choice(["x", "y", "z"], n),  # Random choice of 'x', 'y', 'z'
-}
-
-# Converting to a DataFrame
-df = pd.DataFrame(data)
-
-# Introducing some missing values in columns 'C' and 'G'
-df.loc[np.random.choice(df.index, size=int(0.1 * n)), "C"] = np.nan
-df.loc[np.random.choice(df.index, size=int(0.1 * n)), "G"] = np.nan
-
-# Saving the DataFrame to a CSV file
-df.to_csv("./data/test_random.csv", index=False)
+    # Saving the DataFrame to a CSV file
+    df.to_csv("data/test_random.csv", index=False)
```

### Comparing `dataanalysistoolkit-1.1.1/src/generators/report_generator.py` & `dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/generators/report_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,29 +21,33 @@
 from io import BytesIO
 import pandas as pd
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 
 class ReportGenerator:
+    """
+     _summary_
+
+    _extended_summary_
+    """
     def __init__(self, data, columns=None):
         """
         Initializes the ReportGenerator with the dataset and optional specific
         columns.
 
         Args:
             data (DataFrame): The pandas DataFrame from which the report will
             be generated.
             columns (list, optional): Specific columns to be included in the
             report. If None, all columns are used.
         """
         self.data = data
         self.columns = columns if columns else data.columns
 
-
     def _generate_base64_image(self, plot_func):
         """
         Helper method to generate a base64 encoded string of a matplotlib plot.
 
         Args:
             plot_func (function): A function to generate a matplotlib plot.
 
@@ -93,21 +97,25 @@
                 lambda: sns.histplot(self.data[column].dropna())
             )
             report_sections.append(
                 f'<img src="data:image/png;base64,{image}" alt="Histogram of {column}"><br>'
             )
 
         # Add scatter plots for pairwise relationships
-        report_sections.append('<h2>Scatter Plots</h2>')
-        numeric_columns = self.data[self.columns].select_dtypes(include=['float64', 'int64']).columns
+        report_sections.append("<h2>Scatter Plots</h2>")
+        numeric_columns = (
+            self.data[self.columns].select_dtypes(include=["float64", "int64"]).columns
+        )
         if len(numeric_columns) > 1:
             for i, col1 in enumerate(numeric_columns[:-1]):
-                for col2 in numeric_columns[i + 1:]:
+                for col2 in numeric_columns[i + 1 :]:
                     image = self._generate_base64_image(
-                        lambda col1=col1, col2=col2: sns.scatterplot(x=col1, y=col2, data=self.data)
+                        lambda col1=col1, col2=col2: sns.scatterplot(
+                            x=col1, y=col2, data=self.data
+                        )
                     )
                     report_sections.append(
                         f'<img src="data:image/png;base64,{image}" alt="Scatter plot of {col1} vs {col2}"><br>'
                     )
 
         # Add box plots for distributions
         report_sections.append("<h2>Box Plots</h2>")
```

### Comparing `dataanalysistoolkit-1.1.1/src/integrators/data_integrator.py` & `dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/integrators/data_integrator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,129 +1,139 @@
-"""data_integrator.py
-_summary_
-
-_extended_summary_
-
-Returns:
-    _type_: _description_
+"""
+data_integrator.py
 
-# Example usage
-integrator = DataIntegrator()
-integrator.add_data(df1)
-integrator.add_data(df2)
-combined_data = integrator.join_on_multiple_columns(['column1', 'column2'])
-# or
-time_series_data = integrator.integrate_time_series('date', method='nearest')
-# or
-source_data = {'sql': sql_df, 'excel': excel_df, 'api': api_df}
-integrated_data = integrator.integrate_from_different_sources(source_data, 'concat')
+A module for integrating multiple data sources using pandas DataFrames.
+This module provides a class, DataIntegrator, which allows users to
+combine, merge, and join data from various sources such as SQL, Excel,
+and APIs. It also supports time series integration and concatenation
+methods.
+
+The module can be used to handle complex data integration needs in data
+science and analytics projects, enabling seamless combination of data
+from different formats and sources.
+
+Example usage:
+
+    integrator = DataIntegrator()
+    integrator.add_data(df1)
+    integrator.add_data(df2)
+    combined_data = integrator.join_on_multiple_columns(['column1', 'column2'])
+    # or
+    time_series_data = integrator.integrate_time_series('date', method='nearest')
+    # or
+    source_data = {'sql': sql_df, 'excel': excel_df, 'api': api_df}
+    integrated_data = integrator.integrate_from_different_sources(
+        source_data, 'concat'
+    )
 """
 
 import pandas as pd
 
 
 class DataIntegrator:
     """
-     _summary_
+    A class for integrating multiple pandas DataFrames.
+
+    The DataIntegrator class provides methods to add DataFrames and
+    perform various integration operations such as concatenation, merge,
+    join on multiple columns, and time series integration.
 
-    _extended_summary_
+    Attributes:
+        data_frames (list): A list to store the added DataFrames.
     """
 
     def __init__(self):
         """
-        Initialize the DataIntegrator.
+        Initialize the DataIntegrator with an empty list of DataFrames.
         """
         self.data_frames = []
 
     def add_data(self, data_frame):
         """
-        Add a DataFrame to the list of data to be integrated.
+        Add a pandas DataFrame to the list of data to be integrated.
 
         Args:
-            data_frame (DataFrame): A pandas DataFrame to be added.
+            data_frame (pd.DataFrame): A pandas DataFrame to be added.
         """
         self.data_frames.append(data_frame)
 
     def concatenate_data(self):
         """
         Concatenate all added DataFrames into a single DataFrame.
 
         Returns:
-            DataFrame: The concatenated DataFrame.
+            pd.DataFrame: The concatenated DataFrame.
         """
         return pd.concat(self.data_frames, ignore_index=True)
 
     def merge_data(self, on, how="inner"):
         """
-        Merge all added DataFrames into a single DataFrame based on a key
-        column.
+        Merge all added DataFrames into a single DataFrame based on a key column.
 
         Args:
             on (str): Column name to merge on.
-            how (str, optional): Type of merge to be performed. Defaults to
-            'inner'.
+            how (str, optional): Type of merge to be performed.
+              Defaults to 'inner'.
 
         Returns:
-            DataFrame: The merged DataFrame.
+            pd.DataFrame: The merged DataFrame.
         """
         merged_df = self.data_frames[0]
         for df in self.data_frames[1:]:
             merged_df = pd.merge(merged_df, df, on=on, how=how)
         return merged_df
 
     def join_on_multiple_columns(self, columns, how="inner"):
         """
         Join all added DataFrames on multiple columns.
 
         Args:
             columns (list of str): List of column names to join on.
-            how (str, optional): Type of join to be performed. Defaults to
-            'inner'.
+            how (str, optional): Type of join to be performed.
+              Defaults to 'inner'.
 
         Returns:
-            DataFrame: The joined DataFrame.
+            pd.DataFrame: The joined DataFrame.
         """
         joined_df = self.data_frames[0]
         for df in self.data_frames[1:]:
             joined_df = pd.merge(joined_df, df, on=columns, how=how)
         return joined_df
 
     def integrate_time_series(self, time_column, method="nearest"):
         """
         Integrate time series data from added DataFrames based on a time column.
 
         Args:
             time_column (str): The name of the time column for integration.
-            method (str, optional): Method of time series integration (e.g.,
-            'nearest', 'pad'). Defaults to 'nearest'.
+            method (str, optional): Method of time series integration
+              (e.g., 'nearest', 'pad'). Defaults to 'nearest'.
 
         Returns:
-            DataFrame: The integrated DataFrame with time series data.
+            pd.DataFrame: The integrated DataFrame with time series data.
         """
         integrated_df = self.data_frames[0]
         for df in self.data_frames[1:]:
             integrated_df = pd.merge_asof(
-                integrated_df, df, on=time_column, method=method
+                integrated_df, df, on=time_column, direction=method
             )
         return integrated_df
 
-    def integrate_from_different_sources(
-        self, source_data, integration_method="concat"
-    ):
+    def integrate_from_different_sources(self, source_data, integration_method="concat"):
         """
         Integrate data from different sources (like SQL, Excel, APIs).
 
         Args:
             source_data (dict): A dictionary where keys are source names and
-            values are DataFrames.
+              values are DataFrames.
             integration_method (str, optional): The method of integration
-            ('concat', 'merge'). Defaults to 'concat'.
+              ('concat', 'merge'). Defaults to 'concat'.
 
         Returns:
-            DataFrame: The integrated DataFrame from different sources.
+            pd.DataFrame: The integrated DataFrame from different sources.
         """
         self.data_frames = list(source_data.values())
         if integration_method == "concat":
             return self.concatenate_data()
         if integration_method == "merge":
             # Assuming all data frames have a common column for merging
             common_column = source_data.get("common_column")
```

### Comparing `dataanalysistoolkit-1.1.1/src/model/feature_engineer.py` & `dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/model/feature_engineer.py`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.1.1/src/model/model_evaluator.py` & `dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/model/model_evaluator.py`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.1.1/src/preprocessor/data_prep.py` & `dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/preprocessor/data_prep.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 """data_prep.py
 
-This module provides a class, DataPreprocessor, for preprocessing data. It includes functionalities to standardize or
-normalize data, which is an essential step in many data analysis and machine learning workflows.
-
-Extended Summary:
-The DataPreprocessor class is designed to preprocess datasets, particularly useful in preparing data for machine learning models.
-Currently, it supports data standardization, a process of scaling data such that it has a mean of 0 and a standard deviation of 1.
-This is often required to ensure that all features contribute equally to the result and to improve the convergence of algorithms.
+This module provides a class, DataPreprocessor, for preprocessing data. It
+includes functionalities to standardize or normalize data, which is an
+essential step in many data analysis and machine learning workflows.
+
+The DataPreprocessor class is designed to preprocess datasets, particularly
+useful in preparing data for machine learning models. Currently, it supports
+data standardization, a process of scaling data such that it has a mean of 0
+and a standard deviation of 1. This is often required to ensure that all
+features contribute equally to the result and to improve the convergence of
+algorithms.
 """
 
 from sklearn.preprocessing import StandardScaler
 
 class DataPreprocessor:
     """
     A class for preprocessing data for machine learning and data analysis.
 
     This class provides methods to perform various data preprocessing steps.
-    Its primary functionality as of now is to standardize data features, which is crucial in many machine learning algorithms.
+    Its primary functionality as of now is to standardize data features, which
+    is crucial in many machine learning algorithms.
 
     Attributes:
         data (DataFrame): The dataset to be preprocessed.
     """
 
     def __init__(self, data):
         """
         Initializes the DataPreprocessor object with the dataset.
 
         Args:
-            data (DataFrame): The dataset to be preprocessed. It should be a Pandas DataFrame.
+            data (DataFrame): The dataset to be preprocessed. It should be a
+              Pandas DataFrame.
         """
         self.data = data
 
     def standardize(self, columns):
         """
         Standardizes the specified columns in the dataset.
 
-        This method applies standardization to transform the specified columns in the dataset to have a mean of 0 and
-        a standard deviation of 1. It uses sklearn's StandardScaler for this purpose.
+        This method applies standardization to transform the specified columns
+        in the dataset to have a mean of 0 and a standard deviation of 1. It
+        uses sklearn's StandardScaler for this purpose.
 
         Args:
-            columns (list of str): The column names in the dataset that need to be standardized.
+            columns (list of str): The column names in the dataset that need to
+              be standardized.
 
         Returns:
-            None: The method modifies the dataset in place and does not return anything.
+            None: The method modifies the dataset in place and does not return
+              anything.
         """
         scaler = StandardScaler()
         self.data[columns] = scaler.fit_transform(self.data[columns])
```

### Comparing `dataanalysistoolkit-1.1.1/src/utils/data_imputer.py` & `dataanalysistoolkit-1.2.0/src/dataanalysistoolkit/utils/data_imputer.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 imputer.load_imputer_model('imputer.pkl')
 """
 
 import pickle
 from sklearn.impute import SimpleImputer
 import pandas as pd
 
+
 class DataImputer:
     """
     A class for handling missing values in datasets.
 
     This class provides methods to impute missing data using various strategies
     and custom functions. It also offers functionalities to save and load
     imputation models, along with generating imputation reports.
```

### Comparing `dataanalysistoolkit-1.1.1/tests/test_data_analysis_toolkit.py` & `dataanalysistoolkit-1.2.0/tests/test_data_analysis_toolkit.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 Raises:
     AssertionError: If a test fails, an AssertionError is raised with a message
     indicating which test failed and why.
 """
 
 import pytest
 import pandas as pd
-from src.data_analysis_toolkit import DataAnalysisToolkit
+from dataanalysistoolkit.data_analysis_toolkit import DataAnalysisToolkit
 
 
 @pytest.fixture
 def analyzer():
-    return DataAnalysisToolkit("../data/test.csv")
+    return DataAnalysisToolkit("./data/test_random.csv")
 
 
 def test_calculate_budget_statistics(analyzer):
     """
     Test that calculate_budget_statistics returns a dictionary containing mean,
     median, mode, and trimmed mean.
     """
```

