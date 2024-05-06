# Comparing `tmp/markcrowe-0.0.9.tar.gz` & `tmp/markcrowe-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markcrowe-0.0.9.tar", last modified: Sat Jan 29 04:26:00 2022, max compression
+gzip compressed data, was "markcrowe-0.1.0.tar", last modified: Mon May  6 19:13:14 2024, max compression
```

## Comparing `markcrowe-0.0.9.tar` & `markcrowe-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxrwxrwx   0        0        0        0 2022-01-29 04:26:00.085866 markcrowe-0.0.9/
--rw-rw-rw-   0        0        0     2743 2022-01-29 04:26:00.085866 markcrowe-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       86 2021-12-26 14:07:47.000000 markcrowe-0.0.9/license
--rw-rw-rw-   0        0        0      108 2021-12-26 14:07:47.000000 markcrowe-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0      672 2022-01-29 04:26:00.104867 markcrowe-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-01-29 04:25:59.853868 markcrowe-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2022-01-29 04:25:59.902866 markcrowe-0.0.9/src/code_builder/
--rw-rw-rw-   0        0        0        0 2021-12-31 19:30:18.000000 markcrowe-0.0.9/src/code_builder/__init__.py
--rw-rw-rw-   0        0        0      795 2022-01-29 04:23:34.000000 markcrowe-0.0.9/src/code_builder/name_conventions.py
--rw-rw-rw-   0        0        0     1247 2022-01-29 04:23:46.000000 markcrowe-0.0.9/src/code_builder/streamlit_builder.py
-drwxrwxrwx   0        0        0        0 2022-01-29 04:25:59.991870 markcrowe-0.0.9/src/data_analytics/
--rw-rw-rw-   0        0        0        0 2021-12-31 19:30:18.000000 markcrowe-0.0.9/src/data_analytics/__init__.py
--rw-rw-rw-   0        0        0     5254 2022-01-27 02:31:07.000000 markcrowe-0.0.9/src/data_analytics/exploratory_data_analysis.py
--rw-rw-rw-   0        0        0     4455 2022-01-27 04:04:27.000000 markcrowe-0.0.9/src/data_analytics/exploratory_data_analysis_reports.py
--rw-rw-rw-   0        0        0     4716 2022-01-13 05:15:59.000000 markcrowe-0.0.9/src/data_analytics/github.py
--rw-rw-rw-   0        0        0     6481 2021-12-26 14:07:47.000000 markcrowe-0.0.9/src/data_analytics/graphs.py
--rw-rw-rw-   0        0        0      429 2022-01-29 04:25:08.000000 markcrowe-0.0.9/src/data_analytics/machine_learning.py
--rw-rw-rw-   0        0        0     1233 2022-01-26 01:50:33.000000 markcrowe-0.0.9/src/data_analytics/zip_file.py
-drwxrwxrwx   0        0        0        0 2022-01-29 04:26:00.026863 markcrowe-0.0.9/src/markcrowe.egg-info/
--rw-rw-rw-   0        0        0     2743 2022-01-29 04:25:59.000000 markcrowe-0.0.9/src/markcrowe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      670 2022-01-29 04:25:59.000000 markcrowe-0.0.9/src/markcrowe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-29 04:25:59.000000 markcrowe-0.0.9/src/markcrowe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2022-01-29 04:25:59.000000 markcrowe-0.0.9/src/markcrowe.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-01-29 04:26:00.082868 markcrowe-0.0.9/src/population_planning/
--rw-rw-rw-   0        0        0        0 2021-12-31 19:30:18.000000 markcrowe-0.0.9/src/population_planning/__init__.py
--rw-rw-rw-   0        0        0     1766 2021-12-26 14:07:47.000000 markcrowe-0.0.9/src/population_planning/dataframe_labels.py
--rw-rw-rw-   0        0        0     3981 2021-12-31 19:30:18.000000 markcrowe-0.0.9/src/population_planning/project_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-06 19:13:14.253527 markcrowe-0.1.0/
+-rw-rw-rw-   0        0        0     2753 2024-05-06 19:13:14.253527 markcrowe-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2024-05-06 19:08:04.000000 markcrowe-0.1.0/license
+-rw-rw-rw-   0        0        0      108 2021-12-26 14:07:47.000000 markcrowe-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     2240 2024-02-29 10:29:56.000000 markcrowe-0.1.0/readme.md
+-rw-rw-rw-   0        0        0      663 2024-05-06 19:13:14.255938 markcrowe-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 19:13:14.212358 markcrowe-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 19:13:14.218913 markcrowe-0.1.0/src/code_builder/
+-rw-rw-rw-   0        0        0        0 2021-12-31 19:30:18.000000 markcrowe-0.1.0/src/code_builder/__init__.py
+-rw-rw-rw-   0        0        0     2144 2023-01-04 22:54:41.000000 markcrowe-0.1.0/src/code_builder/ml_data_class_builder.py
+-rw-rw-rw-   0        0        0      892 2023-01-04 03:59:04.000000 markcrowe-0.1.0/src/code_builder/name_conventions.py
+-rw-rw-rw-   0        0        0     1453 2023-01-04 04:03:26.000000 markcrowe-0.1.0/src/code_builder/streamlit_builder.py
+drwxrwxrwx   0        0        0        0 2024-05-06 19:13:14.224589 markcrowe-0.1.0/src/data_analytics/
+-rw-rw-rw-   0        0        0        0 2021-12-31 19:30:18.000000 markcrowe-0.1.0/src/data_analytics/__init__.py
+-rw-rw-rw-   0        0        0     5800 2023-01-04 19:41:48.000000 markcrowe-0.1.0/src/data_analytics/exploratory_data_analysis.py
+-rw-rw-rw-   0        0        0     5339 2023-01-04 19:46:16.000000 markcrowe-0.1.0/src/data_analytics/exploratory_data_analysis_reports.py
+-rw-rw-rw-   0        0        0     5930 2024-04-19 00:58:28.000000 markcrowe-0.1.0/src/data_analytics/github.py
+-rw-rw-rw-   0        0        0     6476 2023-01-04 19:09:36.000000 markcrowe-0.1.0/src/data_analytics/graphs.py
+-rw-rw-rw-   0        0        0     1629 2024-05-06 19:05:45.000000 markcrowe-0.1.0/src/data_analytics/machine_learning.py
+-rw-rw-rw-   0        0        0     1345 2023-01-04 03:59:04.000000 markcrowe-0.1.0/src/data_analytics/zip_file.py
+drwxrwxrwx   0        0        0        0 2024-05-06 19:13:14.226589 markcrowe-0.1.0/src/markcrowe/
+-rw-rw-rw-   0        0        0        0 2023-01-04 20:18:54.000000 markcrowe-0.1.0/src/markcrowe/__init__.py
+-rw-rw-rw-   0        0        0     1254 2024-05-06 19:04:37.000000 markcrowe-0.1.0/src/markcrowe/support.py
+drwxrwxrwx   0        0        0        0 2024-05-06 19:13:14.252044 markcrowe-0.1.0/src/markcrowe.egg-info/
+-rw-rw-rw-   0        0        0     2753 2024-05-06 19:13:14.000000 markcrowe-0.1.0/src/markcrowe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      793 2024-05-06 19:13:14.000000 markcrowe-0.1.0/src/markcrowe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 19:13:14.000000 markcrowe-0.1.0/src/markcrowe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-06 19:13:14.000000 markcrowe-0.1.0/src/markcrowe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 19:13:14.250673 markcrowe-0.1.0/src/population_planning/
+-rw-rw-rw-   0        0        0        0 2021-12-31 19:30:18.000000 markcrowe-0.1.0/src/population_planning/__init__.py
+-rw-rw-rw-   0        0        0     2018 2023-01-04 03:59:04.000000 markcrowe-0.1.0/src/population_planning/dataframe_labels.py
+-rw-rw-rw-   0        0        0     3986 2023-01-04 03:59:04.000000 markcrowe-0.1.0/src/population_planning/project_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-06 19:13:14.250673 markcrowe-0.1.0/tests/
+-rw-rw-rw-   0        0        0     2430 2024-02-29 10:24:00.000000 markcrowe-0.1.0/tests/test_basic.py
```

### Comparing `markcrowe-0.0.9/PKG-INFO` & `markcrowe-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 Metadata-Version: 2.1
 Name: markcrowe
-Version: 0.0.9
+Version: 0.1.0
 Summary: Data analytic functions for data projects.
-Home-page: https://github.com/markcrowe-com/markcrowe.pypi/
+Home-page: https://github.com/marcocrowe/markcrowe.pypi/
 Author: Mark Crowe
-Author-email: 66536097+markcrowe-com@users.noreply.github.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/markcrowe-com/markcrowe.pypi/issues
-Platform: UNKNOWN
+Author-email: 66536097+marcocrowe@users.noreply.github.com
+Project-URL: Bug Tracker, https://github.com/marcocrowe/markcrowe.pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: license
 
-# [markcrowe.pypi](https://github.com/markcrowe-com/markcrowe.pypi)
+
+# [markcrowe.pypi](https://github.com/marcocrowe/markcrowe.pypi)
 
 This package is published at <https://pypi.org/project/markcrowe/>
 
 ## Requirements
 
-- [Python &GreaterEqual; 3.8.0](https://www.python.org/downloads/)
+- [Python &GreaterEqual; 3.10.0](https://www.python.org/downloads/)
 
 The packages in this archive are:
--  data_analytics
--  population_planning
+
+- data_analytics
+- population_planning
 
 ## Install Python Package Builders
+
 To install/upgrade Python packages to build a Python package run these commands:
 
 ```bash
+pip install -r requirements.txt
+```
+
+```bash
 pip install --upgrade pip
 pip install --upgrade build
 pip install --upgrade twine
 ```
 
 In the event of an error, consider running the following commands:
 
@@ -44,62 +49,69 @@
 
 ## Recommended IDEs
 
 - [VS Code](https://code.visualstudio.com/): [`Python`](https://code.visualstudio.com/docs/languages/python)
 
 ## Build and publish a Python package
 
-*All these commands must be run from the project root:*  
+*All these commands must be run from the project root:*
 
 ### Update the required packages
+
 To build the requirements.txt file run these commands:
+
 ```bash
 pipreqs --force
 ```
 
 ### Build/rebuild the Python package
+
 To build the Python package, run the following command:
+
 ```bash
 python -m build
 ```
 
 ### Publish the Python package
+
 To publish the package to PyPI, run the following command:
+
 ```bash
 python -m twine upload dist/*
 ```
-For username enter `__token__` and then your password.  
+
+For username enter `__token__` and then your password.
 
 The package is then available at [markcrowe](https://pypi.org/project/markcrowe/)
 
 ### Installation of the Python package
 
 #### Remote installation
 
 To install the package from [pypi.org](https://pypi.org), run the following command:
 
 ```bash
 pip install markcrowe
 ```
 
 #### Local installation
+
 To install the package from local sources, run the following command:
 
 ```bash
-pip install .\dist\markcrowe-0.0.9-py3-none-any.whl
+pip install .\dist\markcrowe-0.1.0-py3-none-any.whl
 ```
 
 To force a reinstall of the package from local sources, run the following command:
 
 ```bash
-pip install .\dist\markcrowe-0.0.9-py3-none-any.whl --force-reinstall
+pip install .\dist\markcrowe-0.1.0-py3-none-any.whl --force-reinstall
 ```
 
-Conda:  
+Conda:
+
 ```bash
-conda install .\dist\markcrowe-0.0.9-py3-none-any.whl --channel conda-forge
+conda install .\dist\markcrowe-0.1.0-py3-none-any.whl --channel conda-forge
 ```
 
 ---
-Copyright &copy; 2021 Mark Crowe <https://github.com/markcrowe-com>. All rights reserved.
-
-
+Copyright &copy; 2021 Mark Crowe <https://github.com/marcocrowe>. All rights reserved.
```

### Comparing `markcrowe-0.0.9/src/code_builder/streamlit_builder.py` & `markcrowe-0.1.0/src/code_builder/streamlit_builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,35 @@
+# Copyright (c) 2021 Mark Crowe <https://github.com/markcrowe-com>. All rights reserved.
+
 from code_builder.name_conventions import english_to_snake_case
 from data_analytics.exploratory_data_analysis import is_numeric_data_type_column
 from pandas import DataFrame
 import os
 import math
 
 
 def build_sliders(dataframe: DataFrame) -> str:
     text: str = ""
-    columns = dataframe.columns.tolist()
+    columns: list = dataframe.columns.tolist()
 
-    string_values = ""
+    string_values: str = ""
     for column_name in columns:
         variable_name: str = english_to_snake_case(column_name)
         string_values += f"{variable_name}, "
 
         if (is_numeric_data_type_column(dataframe[column_name])):
             max_value = round(dataframe[column_name].max() * 2)
-            min_value = 0
-            intervals = math.ceil((max_value - min_value) / 20)
+            min_value: int = 0
+            intervals: int = math.ceil((max_value - min_value) / 20)
             text += f"{variable_name} = streamlit.sidebar.slider('{column_name}', {min_value}, {max_value}, {intervals}){os.linesep}"
+            text += f"{variable_name} = {dataframe[column_name].mean()}{os.linesep}"
         else:
-            value_list=""
+            value_list = ""
             unique_values = dataframe[column_name].unique()
             for word in unique_values:
-                value_list+=f'"{word}",'
+                value_list += f'"{word}",'
 
             text += f"{value_list}{os.linesep}"
             text += f"{variable_name} = streamlit.sidebar.selectbox('{column_name}', {value_list}){os.linesep}"
 
-    return text + os.linesep + string_values
+    return f"{text}{os.linesep}{string_values}"
```

### Comparing `markcrowe-0.0.9/src/data_analytics/exploratory_data_analysis.py` & `markcrowe-0.1.0/src/data_analytics/exploratory_data_analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright (c) 2021 Mark Crowe <https://github.com/markcrowe-com>. All rights reserved.
 
 from pandas import DataFrame
 from pandas import Series
 
-Q1 = 0.25
-Q2 = 0.5
-Q3 = 0.75
-TUKEY_IQR_SCALE = 1.5
+Q1: float = 0.25
+Q2: float = 0.5
+Q3: float = 0.75
+TUKEY_IQR_SCALE: float = 1.5
 
 
 def calculate_iqr(q1: float, q3: float) -> float:
     """
     Calculate the interquartile range
     :param q1: first quantile
     :param q3: third quantile
@@ -22,51 +22,55 @@
 def calculate_iqr_of_column(dataframe: DataFrame, column_label: str) -> float:
     """
     Calculate the interquartile range
     :param dataframe: DataFrame
     :param column_label: The Column to use for calculating interquartile range
     :return: interquartile range
     """
+    q1: float
+    q3: float
     q1, q3 = calculate_quantile_bounds(dataframe, column_label)
     return q3 - q1
 
 
 def calculate_missing_value_statistics(dataframe: DataFrame) -> DataFrame:
-    missing_stats_dataframe = DataFrame(
+    missing_stats_dataframe: DataFrame = DataFrame(
         {
             'Missing': dataframe.isnull().sum(),
             '% Missing': dataframe.isnull().sum() / len(dataframe) * 100
         })
     missing_stats_dataframe = missing_stats_dataframe[missing_stats_dataframe['Missing'] > 0]
     return missing_stats_dataframe.sort_values(by='Missing', ascending=False)
 
 
-def calculate_outlier_limits(dataframe: DataFrame, column_label: str) -> tuple:
+def calculate_outlier_limits(dataframe: DataFrame, column_label: str) -> tuple[float, float]:
     """
     Calculate the limits of outliers
     :param dataframe: DataFrame
     :param column_label: The Column to use for removing outliers
     :return: tuple of lower and upper limits
     """
+    q1: float
+    q3: float
     q1, q3 = calculate_quantile_bounds(dataframe, column_label)
-    iqr = calculate_iqr(q1, q3)
-    lower_limit = q1 - TUKEY_IQR_SCALE * iqr
-    upper_limit = q3 + TUKEY_IQR_SCALE * iqr
+    iqr: float = calculate_iqr(q1, q3)
+    lower_limit: float = q1 - TUKEY_IQR_SCALE * iqr
+    upper_limit: float = q3 + TUKEY_IQR_SCALE * iqr
     return lower_limit, upper_limit
 
 
-def calculate_quantile_bounds(dataframe: DataFrame, column_label: str) -> tuple:
+def calculate_quantile_bounds(dataframe: DataFrame, column_label: str) -> tuple[float, float]:
     """
     Calculates the first (q1) and third (q3) quantiles of the column
     :param dataframe: DataFrame
     :param column_label: The Column to use first and third quantiles
     :return: the first (q1) and third (q3) quantiles of the column
     """
-    q1 = dataframe[column_label].quantile(Q1)
-    q3 = dataframe[column_label].quantile(Q3)
+    q1: float = dataframe[column_label].quantile(Q1)
+    q3: float = dataframe[column_label].quantile(Q3)
     return q1, q3
 
 
 def count_outliers(dataframe: DataFrame, column_label: str) -> int:
     """
     Get the count of outliers
     :param dataframe: DataFrame
@@ -79,20 +83,22 @@
 def get_expected_range_dataframe(dataframe: DataFrame, column_label: str) -> DataFrame:
     """
     Get expected range of rows by excluding outliers
     :param dataframe: DataFrame
     :param column_label: The Column to use for removing outliers
     :return: DataFrame of expected range
     """
+    lower_limit: float
+    upper_limit: float
     lower_limit, upper_limit = calculate_outlier_limits(
         dataframe, column_label)
     return dataframe[(dataframe[column_label] >= lower_limit) & (dataframe[column_label] <= upper_limit)]
 
 
-def get_names_of_columns_with_null_values(dataframe: DataFrame) -> list:
+def get_names_of_columns_with_null_values(dataframe: DataFrame) -> list[str]:
     """
     Get the names of columns with null values
     :param dataframe: DataFrame
     :return: names of columns with null values
     """
     return dataframe.columns[dataframe.isna().any()].tolist()
 
@@ -100,14 +106,16 @@
 def get_outliers_dataframe(dataframe: DataFrame, column_label: str) -> DataFrame:
     """
     Get outliers of rows by excluding expected range
     :param dataframe: DataFrame
     :param column_label: The Column to use for removing outliers
     :return: DataFrame of outliers
     """
+    lower_limit: float
+    upper_limit: float
     lower_limit, upper_limit = calculate_outlier_limits(
         dataframe, column_label)
     return dataframe[(dataframe[column_label] < lower_limit) | (dataframe[column_label] > upper_limit)]
 
 
 def has_outliers(dataframe: DataFrame, column_label: str) -> bool:
     """
@@ -115,14 +123,23 @@
     :param dataframe: DataFrame
     :param column_label: The Column to use for checking
     :return: True if the column has outliers
     """
     return count_outliers(dataframe, column_label) > 0
 
 
+def contains_only_integer_values(series: Series) -> bool:
+    """
+    Check if the float column has only integer values
+    :param series: Series the array to use for checking
+    :return: True if the column has only integer values
+    """
+    return all(series % 1 == 0)
+
+
 def is_numeric_data_type_column(series: Series) -> bool:
     """
     Check if the column is a numeric data type
     :param series: Series the array to use for checking
     :return: True if the column is a numeric data type
     """
     NUMERIC_DATA_TYPE_CHARACTER_CODES = 'ifu'  # i	signed integer, u	unsigned integer, f	floating-point
```

### Comparing `markcrowe-0.0.9/src/data_analytics/exploratory_data_analysis_reports.py` & `markcrowe-0.1.0/src/data_analytics/exploratory_data_analysis_reports.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 # Copyright (c) 2021 Mark Crowe <https://github.com/markcrowe-com>. All rights reserved.
 
-from IPython.core.display import display, HTML
+from IPython.display import display, HTML
 from pandas import DataFrame
 import data_analytics.exploratory_data_analysis as eda
 
+class HtmlTags:
+    UL: str = '<ul>'
+    UL_CLOSE: str = '</ul>'
+
 
 def print_dataframe_analysis_report(dataframe: DataFrame, name: str = 'dataframe', sample_size: int = 5) -> None:
     """
-    Print an analysis report of the data frame. 
+    Print an analysis report of the data frame.
     - Show the top five rows of the data frame as a quick sample.
     - Show the data types of each column.
     - Report count of any duplicates.
     - Report count of any missing values.
     - Report any single value columns.
-    :param dataframe: The data frame to be analysed
+    :param dataframe: The data frame to be analyzed
     :param name: The name of the data frame
     """
     display(HTML(f'<h4>{name}</h4>'))
     display(HTML(f'<p>Row, Column Count: {dataframe.shape}</p>'))
     display(HTML('<h5>Sample: Top five rows</h5>'))
     display(dataframe.sample(sample_size))
     display(HTML('<h5>Data Types</h5>'))
     display(dataframe.dtypes)
+    display(HTML('<h5>Object/String columns</h5>'))
+    report_object_value_columns(dataframe)
     display(HTML('<h5>Duplicates</h5>'))
     duplicate_rows_dataframe: DataFrame = dataframe[dataframe.duplicated()]
     display(
         HTML(f'<p>Number of duplicate rows: {duplicate_rows_dataframe.shape[0]}</p>'))
     report_missing_values(dataframe)
     display(HTML('<h5>Single Value Columns</h5>'))
     report_single_value_columns(dataframe)
@@ -36,79 +42,99 @@
 
 
 def report_missing_values(dataframe: DataFrame) -> None:
     """
     Report the number of missing values for each column
     :param dataframe: DataFrame
     """
-    nulls_dataframe = eda.calculate_missing_value_statistics(dataframe)
+    nulls_dataframe: DataFrame = eda.calculate_missing_value_statistics(dataframe)
     if len(nulls_dataframe.index) > 0:
         display(HTML('<h5>Null Values</h5>'))
         display(nulls_dataframe)
     else:
         display(HTML('<h5>No Columns with Null values</h5>'))
 
 
 def report_columns_unique_value_counts(dataframe: DataFrame) -> None:
     """
     Report the unique value counts for each column
     :param dataframe: DataFrame
     """
-    html: str = '<ul>'
+    html: str = HtmlTags.UL
     for column in dataframe.columns:
         html += f'<li>The column "{column}" has {dataframe[column].nunique()} unique values.</li>'
-    html += '</ul>'
+    html += HtmlTags.UL_CLOSE
     display(HTML(html))
 
 
 def report_single_value_columns(dataframe: DataFrame) -> None:
     """
     Report any columns that have only one value
     :param dataframe: DataFrame
     """
-    html: str = '<ul>'
-    has_no_single_value_columns = True
+    html: str = HtmlTags.UL
+    has_no_single_value_columns: bool = True
     for column in dataframe.columns:
         if eda.is_single_value_column(dataframe, column):
             html += f'<li>The column `{column}` has only one value. Recommend removing.</li>'
             has_no_single_value_columns = False
-    html += '</ul>'
+    html += HtmlTags.UL_CLOSE
 
     if(has_no_single_value_columns):
         display(HTML('<p>No single value columns found.</p>'))
     else:
         display(HTML(html))
 
 
 def print_columns_rows_with_missing_values(dataframe: DataFrame, identifying_columns: list) -> None:
     """
     Print the rows with missing values for each column
     :param dataframe: DataFrame
     :param name: Name of the data frame
     """
-    null_columns_list = identifying_columns + \
+    null_columns_list: str = identifying_columns + \
         eda.get_names_of_columns_with_null_values(dataframe)
     display(dataframe[null_columns_list][dataframe.isnull().any(axis=1)])
 
 
+def report_object_value_columns(dataframe: DataFrame) -> None:
+    """
+    Report any columns that have object/string values
+    :param dataframe: DataFrame
+    """
+    html: str = HtmlTags.UL
+    has_no_single_value_columns: bool = True
+    for column in dataframe.columns:
+        if dataframe[column].dtype == 'object':
+            html += f'<li>The column `{column}` has object/string values.</li>'
+            has_no_single_value_columns = False
+
+    html += HtmlTags.UL_CLOSE
+
+    if(has_no_single_value_columns):
+        display(HTML('<p>No object/string value columns found.</p>'))
+    else:
+        display(HTML(html))
+
+
 def report_outliers_columns(dataframe: DataFrame) -> None:
     """
     Report any columns that have outliers
     :param dataframe: DataFrame
     """
-    has_no_outlier_columns = True
-    html: str = '<ul>'
+    has_no_outlier_columns: bool = True
+    html: str = HtmlTags.UL
     for column_label in dataframe.columns:
         if eda.is_numeric_data_type_column(dataframe[column_label]):
             outlier_count = eda.count_outliers(dataframe, column_label)
             if outlier_count > 1:
                 html += f'<li>The column "{column_label}" has {outlier_count} outliers. Recommend removing outliers.</li>'
                 has_no_outlier_columns = False
             elif outlier_count == 1:
                 html += f'<li>The column "{column_label}" has {outlier_count} outlier. Recommend removing outlier.</li>'
                 has_no_outlier_columns = False
-    html += '</ul>'
+    html += HtmlTags.UL_CLOSE
 
     if(has_no_outlier_columns):
         display(HTML('<p>No columns with outliers found.</p>'))
     else:
         display(HTML(html))
```

### Comparing `markcrowe-0.0.9/src/data_analytics/github.py` & `markcrowe-0.1.0/src/data_analytics/github.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,101 +1,161 @@
-# Copyright (c) 2021 Mark Crowe <https://github.com/markcrowe-com>. All rights reserved.
+"""
+Copyright © 2024 Mark Crowe <https://github.com/marcocrowe>. All rights reserved.
+"""
 
-from IPython.core.display import display, HTML
 import os
+from IPython.display import display, HTML
 
-GITHUB_RAW_QUERY_STRING = '?raw=true'
-RELATIVE_PATH = './..'
+GITHUB_RAW_QUERY_STRING: str = "?raw=true"
+RELATIVE_PATH: str = "./.."
 
 
-def create_jupyter_notebook_header(github_username: str, repository: str, notebook_filepath: str, branch: str = 'master', style: str = 'style="margin: auto;"') -> str:
-    """
-    Create an edit online header for Jupyter Notebook.
-    :param github_username: GitHub username
-    :param repository: repository name
-    :param notebook_filepath: notebook filepath
-    :param branch: branch name
-    :return: HTML header
-    """
-
-    html_comment = f'''<!--{os.linesep}import data_analytics.github as github{os.linesep}print(github.create_jupyter_notebook_header("{github_username}", "{repository}", "{notebook_filepath}", "{branch}")){os.linesep}-->{os.linesep}'''
-    binder_url = f'https://mybinder.org/v2/gh/{github_username}/{repository}/{branch}?filepath={notebook_filepath}'
-    colab_url = f'https://colab.research.google.com/github/{github_username}/{repository}/blob/{branch}/{notebook_filepath}'
+def create_jupyter_notebook_header(
+    github_username: str,
+    repository: str,
+    notebook_filepath: str,
+    branch: str = "master",
+    style: str = 'style="margin: auto;"',
+) -> str:
+    """Create an edit online header for Jupyter Notebook.
+
+    Args:
+        github_username (str): The GitHub username
+        repository (str): The repository name
+        notebook_filepath (str): The notebook filepath relative to the repository root
+        branch (str, optional): The branch name. Defaults to 'master'.
+        style (_type_, optional): The style attribute. Defaults to 'style="margin: auto;"'.
+
+    Returns:
+        str: The HTML header
+    """
+
+    html_comment: str = (
+        f"""<!--{os.linesep}import data_analytics.github as github{os.linesep}print(github.create_jupyter_notebook_header("{github_username}", "{repository}", "{notebook_filepath}", "{branch}")){os.linesep}-->{os.linesep}"""
+    )
+    binder_url: str = (
+        f"https://mybinder.org/v2/gh/{github_username}/{repository}/{branch}?filepath={notebook_filepath}"
+    )
+    colab_url: str = (
+        f"https://colab.research.google.com/github/{github_username}/{repository}/blob/{branch}/{notebook_filepath}"
+    )
     return f'{html_comment}<table {style}><tr><td><a href="{binder_url}" target="_parent"><img src="https://mybinder.org/badge_logo.svg" alt="Open In Binder"/></a></td><td>online editors</td><td><a href="{colab_url}" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a></td></tr></table>'
 
 
 def display_jupyter_notebook_data_sources(datasource_filenames: list) -> None:
     """
     Print Data Sources for this notebook.
     :param repository_url: GitHub repository URL
     :param datasource_filenames: list of Data Source filenames
     """
-    display(HTML('<strong>Data Sources</strong>'))
-    display(HTML('<p>Data Sources available at</p>'))
+    display(HTML("<strong>Data Sources</strong>"))
+    display(HTML("<p>Data Sources available at</p>"))
     for datasource_filename in datasource_filenames:
         print(datasource_filename)
 
 
-def display_jupyter_notebook_header(github_username: str, repository: str, notebook_filepath: str, branch: str = 'master') -> None:
-    """
-    Display an edit online header for Jupyter Notebook
-    :param github_username: GitHub username
-    :param repository: repository name
-    :param notebook_filepath: notebook filepath
-    :param branch: branch name
-    """
-    display(HTML(create_jupyter_notebook_header(
-        github_username, repository, notebook_filepath, branch)))
-
+def display_jupyter_notebook_header(
+    github_username: str,
+    repository: str,
+    notebook_filepath: str,
+    branch: str = "master",
+) -> None:
+    """Display an edit online header for Jupyter Notebook.
+
+    Args:
+        github_username (str): The GitHub username
+        repository (str): The repository name
+        notebook_filepath (str): The notebook filepath relative to the repository root
+        branch (str, optional): The branch name. Defaults to 'master'.
+    """
+    display(
+        HTML(
+            create_jupyter_notebook_header(
+                github_username, repository, notebook_filepath, branch
+            )
+        )
+    )
+
+
+def get_filepath(
+    repository_url: str,
+    filename: str,
+    is_remote: bool = True,
+    relative_path: str = RELATIVE_PATH,
+    query_string: str = GITHUB_RAW_QUERY_STRING,
+) -> str:
+    """Get the filepath for a file in the repository.
+
+    Args:
+        repository_url (str): The GitHub repository URL
+        filename (str): The filename
+        is_remote (bool, optional): Is the repository remote. Defaults to True.
+        relative_path (str, optional): The relative path to use to access the files. Defaults to RELATIVE_PATH.
+        query_string (str, optional): The query string. Defaults to GITHUB_RAW_QUERY_STRING.
 
-def get_filepath(repository_url: str, filename: str, is_remote: bool = True, relative_path: str = RELATIVE_PATH, query_string: str = GITHUB_RAW_QUERY_STRING) -> str:
+    Returns:
+        str: The filepath
+    """
     if is_remote:
-        return f'{repository_url}/{filename}{query_string}'
+        return f"{repository_url}/{filename}{query_string}"
     else:
-        return f'{relative_path}/{filename}'
+        return f"{relative_path}/{filename}"
 
 
 def get_github_url(repository_url: str, filename: str) -> str:
     """
     Get GitHub URL
     :param repository_url: GitHub repository URL
     :param filename: filename
     :return: GitHub URL
     """
-    return f'{repository_url}/{filename}'
+    return f"{repository_url}/{filename}"
 
 
 def get_raw_github_url(repository_url: str, filename: str) -> str:
     """
     Get raw GitHub URL
     :param repository_url: GitHub repository URL
     :param filename: filename
     :return: raw GitHub URL
     """
-    return get_github_url(repository_url, filename) + '?raw=true'
+    return f"{get_github_url(repository_url, filename)}?raw=true"
 
 
-def print_jupyter_notebook_header_html(github_username: str, repository: str, notebook_filepath: str, branch: str = 'master') -> None:
+def print_jupyter_notebook_header_html(
+    github_username: str,
+    repository: str,
+    notebook_filepath: str,
+    branch: str = "master",
+) -> None:
     """
     print an edit online header for Jupyter Notebook
     :param github_username: GitHub username
     :param repository: repository name
     :param notebook_filepath: notebook filepath
     :param branch: branch name
     """
-    print(create_jupyter_notebook_header(
-        github_username, repository, notebook_filepath, branch))
+    print(
+        create_jupyter_notebook_header(
+            github_username, repository, notebook_filepath, branch
+        )
+    )
 
 
 class RepositoryFileManager:
     """
     A RepositoryFileManager is a class that manages the filepaths for a GitHub repository.
     """
 
-    def __init__(self, repository_url: str, relative_path: str = RELATIVE_PATH, is_remote: bool = False):
+    def __init__(
+        self,
+        repository_url: str,
+        relative_path: str = RELATIVE_PATH,
+        is_remote: bool = False,
+    ):
         """
         Initialize a RepositoryFileManager
         :param repository_url: GitHub repository URL
         :param relative_path: relative path to use to access the files
         :param is_remote: is the repository remote
         """
         self.is_remote = is_remote
@@ -103,8 +163,14 @@
         self.repository_url = repository_url
         self.query_string = GITHUB_RAW_QUERY_STRING
 
     def get_repository_filepath(self, filename: str) -> str:
         """
         Get the filepath for a file in the repository
         """
-        return get_filepath(self.repository_url, filename, self.is_remote, self.relative_path, self.query_string)
+        return get_filepath(
+            self.repository_url,
+            filename,
+            self.is_remote,
+            self.relative_path,
+            self.query_string,
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `markcrowe-0.0.9/src/data_analytics/graphs.py` & `markcrowe-0.1.0/src/data_analytics/graphs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) 2021 Mark Crowe <https://github.com/markcrowe-com>. All rights reserved.
 
 from altair.vegalite.v4.api import ConcatChart
-from IPython.core.display import display, HTML
+from IPython.display import display, HTML
 from pandas import DataFrame
 import altair
 import matplotlib.pyplot as pyplot
 import numpy as numpy
 import seaborn as seaborn
 
 
@@ -17,15 +17,15 @@
     :return: The Caption html.
     """
     return f'<p class="{css_class}">{title}</p>'
 
 
 def build_interactive_population_pyramid_chart(population_dataframe: DataFrame, age_field: str = "Age", population_field: str = "Population",
                                                sex_field: str = "Sex", time_field: str = "Year",
-                                               male_value: str = "Male", female_value: str = "Female", male_color: str = "darkblue", female_color: str = "darkgreen",
+                                               male_value: str = "Male", female_value: str = "Female", male_color: str = "darkblue", female_color: str = "darkGreen",
                                                year_min: int = 1950, year_max: int = 2021, year_init: int = 2020) -> ConcatChart:
     """
     Build a interactive population pyramid chart.
     :param population_dataframe: The population dataframe to display.
     :param age_field: The age field label.
     :param population_field: The population field label.
     :param sex_field: The sex field label.
```

### Comparing `markcrowe-0.0.9/src/data_analytics/zip_file.py` & `markcrowe-0.1.0/src/data_analytics/zip_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+# Copyright (c) 2021 Mark Crowe <https://github.com/markcrowe-com>. All rights reserved.
+
 from zipfile import ZipFile
 import os
 
 
-def join_split_zip_files(split_zip_files_directory: str, destination_dir: str = './temp/', zip_filename: str = 'temp.zip') -> None:
-    split_zip_files = os.listdir(split_zip_files_directory)
-    zip_filepath = os.path.join(destination_dir, zip_filename)
+def join_split_zip_files(split_zip_files_directory: str, destination_dir: str = './temp/', zip_filename: str = 'temp.zip') -> str:
+    split_zip_files: list[str] = os.listdir(split_zip_files_directory)
+    zip_filepath: str = os.path.join(destination_dir, zip_filename)
     if os.path.isfile(zip_filepath):
         os.remove(zip_filepath)
     for split_zip_file in split_zip_files:
         with open(zip_filepath, "ab") as zip_file:
             with open(os.path.join(split_zip_files_directory, split_zip_file), "rb") as split_zip:
                 zip_file.write(split_zip.read())
     return zip_filepath
@@ -20,10 +22,10 @@
 
 
 def unzip_required_asset(filepath: str, zip_path: str, destination_dir: str) -> None:
     if not os.path.isfile(filepath):
         if os.path.isfile(zip_path):
             unzip_file(zip_path, destination_dir)
         elif os.path.isdir(zip_path):
-            zip_filepath = join_split_zip_files(zip_path, destination_dir)
+            zip_filepath: str = join_split_zip_files(zip_path, destination_dir)
             unzip_file(zip_filepath, destination_dir)
             os.remove(zip_filepath)
```

### Comparing `markcrowe-0.0.9/src/markcrowe.egg-info/PKG-INFO` & `markcrowe-0.1.0/src/markcrowe.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 Metadata-Version: 2.1
 Name: markcrowe
-Version: 0.0.9
+Version: 0.1.0
 Summary: Data analytic functions for data projects.
-Home-page: https://github.com/markcrowe-com/markcrowe.pypi/
+Home-page: https://github.com/marcocrowe/markcrowe.pypi/
 Author: Mark Crowe
-Author-email: 66536097+markcrowe-com@users.noreply.github.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/markcrowe-com/markcrowe.pypi/issues
-Platform: UNKNOWN
+Author-email: 66536097+marcocrowe@users.noreply.github.com
+Project-URL: Bug Tracker, https://github.com/marcocrowe/markcrowe.pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: license
 
-# [markcrowe.pypi](https://github.com/markcrowe-com/markcrowe.pypi)
+
+# [markcrowe.pypi](https://github.com/marcocrowe/markcrowe.pypi)
 
 This package is published at <https://pypi.org/project/markcrowe/>
 
 ## Requirements
 
-- [Python &GreaterEqual; 3.8.0](https://www.python.org/downloads/)
+- [Python &GreaterEqual; 3.10.0](https://www.python.org/downloads/)
 
 The packages in this archive are:
--  data_analytics
--  population_planning
+
+- data_analytics
+- population_planning
 
 ## Install Python Package Builders
+
 To install/upgrade Python packages to build a Python package run these commands:
 
 ```bash
+pip install -r requirements.txt
+```
+
+```bash
 pip install --upgrade pip
 pip install --upgrade build
 pip install --upgrade twine
 ```
 
 In the event of an error, consider running the following commands:
 
@@ -44,62 +49,69 @@
 
 ## Recommended IDEs
 
 - [VS Code](https://code.visualstudio.com/): [`Python`](https://code.visualstudio.com/docs/languages/python)
 
 ## Build and publish a Python package
 
-*All these commands must be run from the project root:*  
+*All these commands must be run from the project root:*
 
 ### Update the required packages
+
 To build the requirements.txt file run these commands:
+
 ```bash
 pipreqs --force
 ```
 
 ### Build/rebuild the Python package
+
 To build the Python package, run the following command:
+
 ```bash
 python -m build
 ```
 
 ### Publish the Python package
+
 To publish the package to PyPI, run the following command:
+
 ```bash
 python -m twine upload dist/*
 ```
-For username enter `__token__` and then your password.  
+
+For username enter `__token__` and then your password.
 
 The package is then available at [markcrowe](https://pypi.org/project/markcrowe/)
 
 ### Installation of the Python package
 
 #### Remote installation
 
 To install the package from [pypi.org](https://pypi.org), run the following command:
 
 ```bash
 pip install markcrowe
 ```
 
 #### Local installation
+
 To install the package from local sources, run the following command:
 
 ```bash
-pip install .\dist\markcrowe-0.0.9-py3-none-any.whl
+pip install .\dist\markcrowe-0.1.0-py3-none-any.whl
 ```
 
 To force a reinstall of the package from local sources, run the following command:
 
 ```bash
-pip install .\dist\markcrowe-0.0.9-py3-none-any.whl --force-reinstall
+pip install .\dist\markcrowe-0.1.0-py3-none-any.whl --force-reinstall
 ```
 
-Conda:  
+Conda:
+
 ```bash
-conda install .\dist\markcrowe-0.0.9-py3-none-any.whl --channel conda-forge
+conda install .\dist\markcrowe-0.1.0-py3-none-any.whl --channel conda-forge
 ```
 
 ---
-Copyright &copy; 2021 Mark Crowe <https://github.com/markcrowe-com>. All rights reserved.
-
-
+Copyright &copy; 2021 Mark Crowe <https://github.com/marcocrowe>. All rights reserved.
```

### Comparing `markcrowe-0.0.9/src/markcrowe.egg-info/SOURCES.txt` & `markcrowe-0.1.0/src/markcrowe.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 license
 pyproject.toml
+readme.md
 setup.cfg
 src/code_builder/__init__.py
+src/code_builder/ml_data_class_builder.py
 src/code_builder/name_conventions.py
 src/code_builder/streamlit_builder.py
 src/data_analytics/__init__.py
 src/data_analytics/exploratory_data_analysis.py
 src/data_analytics/exploratory_data_analysis_reports.py
 src/data_analytics/github.py
 src/data_analytics/graphs.py
 src/data_analytics/machine_learning.py
 src/data_analytics/zip_file.py
+src/markcrowe/__init__.py
+src/markcrowe/support.py
 src/markcrowe.egg-info/PKG-INFO
 src/markcrowe.egg-info/SOURCES.txt
 src/markcrowe.egg-info/dependency_links.txt
 src/markcrowe.egg-info/top_level.txt
 src/population_planning/__init__.py
 src/population_planning/dataframe_labels.py
-src/population_planning/project_manager.py
+src/population_planning/project_manager.py
+tests/test_basic.py
```

### Comparing `markcrowe-0.0.9/src/population_planning/dataframe_labels.py` & `markcrowe-0.1.0/src/population_planning/dataframe_labels.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,56 @@
+# Copyright (c) 2021 Mark Crowe <https://github.com/markcrowe-com>. All rights reserved.
+
 # Names of the Series in the DataFrame for the births, deaths, and marriages data
 
-BIRTHS = 'Births'
-BIRTH_RATE = 'Birth Rate'
-DEATHS = 'Deaths'
-DEATH_RATE = 'Death Rate'
-ESTIMATED_POPULATION = 'Estimated Population'
-ESTIMATED_POPULATION_STD = 'Estimated Population STD'
-INFANT_MORTALITY_RATE = 'Infant Mortality Rate'
-MARRIAGES = 'Marriages'
-MARRIAGE_RATE = 'Marriage Rate'
-QUARTER = 'Quarter'
-QUARTERS = 'Quarters'
-RECORD_COMPLETENESS = 'Record Completeness%'
-STATE = 'State'
-YEAR = 'Year'
+BIRTHS: str = 'Births'
+BIRTH_RATE: str = 'Birth Rate'
+DEATHS: str = 'Deaths'
+DEATH_RATE: str = 'Death Rate'
+ESTIMATED_POPULATION: str = 'Estimated Population'
+ESTIMATED_POPULATION_STD: str = 'Estimated Population STD'
+INFANT_MORTALITY_RATE: str = 'Infant Mortality Rate'
+MARRIAGES: str = 'Marriages'
+MARRIAGE_RATE: str = 'Marriage Rate'
+QUARTER: str = 'Quarter'
+QUARTERS: str = 'Quarters'
+RECORD_COMPLETENESS: str = 'Record Completeness%'
+STATE: str = 'State'
+YEAR: str = 'Year'
 
 # Names of the Series in the DataFrame for the county births data
 
-ALL_BIRTHS = 'All Births'
-AVERAGE_AGE_OF_FIRST_TIME_MOTHER = 'Average Age of First Time Mother'
-AVERAGE_AGE_OF_MOTHER = 'Average Age of Mother'
-BIRTHS_OUTSIDE_MARRIAGE = 'Births outside Marriage'
-BIRTHS_WITHIN_MARRIAGE = 'Births within Marriage'
-COUNTY = 'County'
-FIRST_BIRTHS = 'First Births'
+ALL_BIRTHS: str = 'All Births'
+AVERAGE_AGE_OF_FIRST_TIME_MOTHER: str = 'Average Age of First Time Mother'
+AVERAGE_AGE_OF_MOTHER: str = 'Average Age of Mother'
+BIRTHS_OUTSIDE_MARRIAGE: str = 'Births outside Marriage'
+BIRTHS_WITHIN_MARRIAGE: str = 'Births within Marriage'
+COUNTY: str = 'County'
+FIRST_BIRTHS: str = 'First Births'
 # YEAR # This is the same as the YEAR column in the births data
 
 # Names of the Series in the DataFrame for the deaths region data
 
-AGE_AT_DEATH = 'Age at Death'
-AREA_OF_RESIDENCE = 'Area of Residence'
-SEX = 'Sex'
-STATISTIC = 'Statistic'
-UNIT = 'UNIT'
-VALUE = 'VALUE'
+AGE_AT_DEATH: str = 'Age at Death'
+AREA_OF_RESIDENCE: str = 'Area of Residence'
+SEX: str = 'Sex'
+STATISTIC: str = 'Statistic'
+UNIT: str = 'UNIT'
+VALUE: str = 'VALUE'
 # YEAR # This is the same as the YEAR column in the births data
 
 # Names of the Series in the DataFrame for the county divorces
 
-AGE_RANGE = "Age Range"
-COUNT = 'Count'
-HOUSEHOLD_CHILD_COUNT = 'Household Child Count'
+AGE_RANGE: str = "Age Range"
+COUNT: str = 'Count'
+HOUSEHOLD_CHILD_COUNT: str = 'Household Child Count'
 # SEX # This is the same as the SEX column in the deaths region data
 
 # YEAR # This is the same as the YEAR column in the births data.
 
 # Names of the Series in the DataFrame for the population data
 
-AGE = "Age"
-POPULATION = "Population"
+AGE: str = "Age"
+POPULATION: str = "Population"
 # SEX # This is the same as the SEX column in the deaths region data
 
 # YEAR # This is the same as the YEAR column in the births data.
```

### Comparing `markcrowe-0.0.9/src/population_planning/project_manager.py` & `markcrowe-0.1.0/src/population_planning/project_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) 2021 Mark Crowe <https://github.com/markcrowe-com>. All rights reserved.
 
 from data_analytics.github import RepositoryFileManager, RELATIVE_PATH
 
 
-REPOSITORY_URL = 'https://github.com/markcrowe-com/population-planning-data-analytics/blob/master'
+REPOSITORY_URL: str = 'https://github.com/markcrowe-com/population-planning-data-analytics/blob/master'
 
 
 class ProjectArtifactManager(RepositoryFileManager):
 
     def __init__(self, repository_url: str = REPOSITORY_URL, relative_path: str = RELATIVE_PATH, is_remote: bool = False):
         super().__init__(repository_url, relative_path, is_remote)
```

