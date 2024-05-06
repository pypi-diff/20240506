# Comparing `tmp/labhelper-0.0.7.tar.gz` & `tmp/labhelper-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labhelper-0.0.7.tar", last modified: Tue Feb 20 12:25:22 2024, max compression
+gzip compressed data, was "labhelper-0.1.0.tar", last modified: Mon May  6 16:56:30 2024, max compression
```

## Comparing `labhelper-0.0.7.tar` & `labhelper-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 batres    (1000) batres    (1000)        0 2024-02-20 12:25:22.011767 labhelper-0.0.7/
--rw-rw-r--   0 batres    (1000) batres    (1000)      841 2024-02-20 12:25:22.011767 labhelper-0.0.7/PKG-INFO
--rw-rw-r--   0 batres    (1000) batres    (1000)     2342 2023-09-25 14:13:55.000000 labhelper-0.0.7/README.md
-drwxrwxr-x   0 batres    (1000) batres    (1000)        0 2024-02-20 12:25:22.011767 labhelper-0.0.7/labhelper/
--rw-rw-r--   0 batres    (1000) batres    (1000)      379 2024-02-13 10:49:54.000000 labhelper-0.0.7/labhelper/__init__.py
--rw-r--r--   0 batres    (1000) batres    (1000)      225 2024-02-13 10:49:04.000000 labhelper-0.0.7/labhelper/graphing.py
--rw-rw-r--   0 batres    (1000) batres    (1000)     3589 2024-02-06 11:14:57.000000 labhelper-0.0.7/labhelper/pandas_utils.py
--rw-rw-r--   0 batres    (1000) batres    (1000)     1636 2023-10-17 14:06:04.000000 labhelper-0.0.7/labhelper/stats.py
--rw-rw-r--   0 batres    (1000) batres    (1000)    13993 2024-02-05 09:46:05.000000 labhelper-0.0.7/labhelper/symbolic.py
-drwxrwxr-x   0 batres    (1000) batres    (1000)        0 2024-02-20 12:25:22.011767 labhelper-0.0.7/labhelper/unit_systems/
--rw-r--r--   0 batres    (1000) batres    (1000)      751 2024-02-08 11:18:14.000000 labhelper-0.0.7/labhelper/unit_systems/CGS.py
--rw-r--r--   0 batres    (1000) batres    (1000)     1738 2024-02-08 10:57:35.000000 labhelper-0.0.7/labhelper/unit_systems/SI.py
--rw-r--r--   0 batres    (1000) batres    (1000)      111 2024-02-08 10:52:23.000000 labhelper-0.0.7/labhelper/unit_systems/__init__.py
--rw-r--r--   0 batres    (1000) batres    (1000)     2140 2024-02-08 10:52:49.000000 labhelper-0.0.7/labhelper/unit_systems/prefixes.py
--rw-rw-r--   0 batres    (1000) batres    (1000)    11968 2024-02-20 12:15:31.000000 labhelper-0.0.7/labhelper/units.py
-drwxrwxr-x   0 batres    (1000) batres    (1000)        0 2024-02-20 12:25:22.011767 labhelper-0.0.7/labhelper.egg-info/
--rw-rw-r--   0 batres    (1000) batres    (1000)      841 2024-02-20 12:25:21.000000 labhelper-0.0.7/labhelper.egg-info/PKG-INFO
--rw-rw-r--   0 batres    (1000) batres    (1000)      441 2024-02-20 12:25:21.000000 labhelper-0.0.7/labhelper.egg-info/SOURCES.txt
--rw-rw-r--   0 batres    (1000) batres    (1000)        1 2024-02-20 12:25:21.000000 labhelper-0.0.7/labhelper.egg-info/dependency_links.txt
--rw-rw-r--   0 batres    (1000) batres    (1000)       58 2024-02-20 12:25:21.000000 labhelper-0.0.7/labhelper.egg-info/requires.txt
--rw-rw-r--   0 batres    (1000) batres    (1000)       10 2024-02-20 12:25:21.000000 labhelper-0.0.7/labhelper.egg-info/top_level.txt
--rw-rw-r--   0 batres    (1000) batres    (1000)       38 2024-02-20 12:25:22.011767 labhelper-0.0.7/setup.cfg
--rw-rw-r--   0 batres    (1000) batres    (1000)     1182 2024-02-20 12:24:03.000000 labhelper-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:56:30.093887 labhelper-0.1.0/
+-rw-rw-rw-   0        0        0      804 2024-05-06 16:56:30.093887 labhelper-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2382 2023-09-06 19:23:30.000000 labhelper-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 16:56:30.075882 labhelper-0.1.0/labhelper/
+-rw-rw-rw-   0        0        0      335 2024-05-06 16:52:43.000000 labhelper-0.1.0/labhelper/__init__.py
+-rw-rw-rw-   0        0        0      230 2024-03-04 17:11:05.000000 labhelper-0.1.0/labhelper/graphing.py
+-rw-rw-rw-   0        0        0     3673 2024-02-11 21:57:37.000000 labhelper-0.1.0/labhelper/pandas_utils.py
+-rw-rw-rw-   0        0        0     1675 2024-02-02 17:02:37.000000 labhelper-0.1.0/labhelper/stats.py
+-rw-rw-rw-   0        0        0     7478 2024-05-06 16:51:48.000000 labhelper-0.1.0/labhelper/symbolic.py
+-rw-rw-rw-   0        0        0     2087 2024-05-06 16:49:25.000000 labhelper-0.1.0/labhelper/sympy_enclosure.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:56:30.092882 labhelper-0.1.0/labhelper/unit_systems/
+-rw-rw-rw-   0        0        0      773 2024-02-11 21:57:37.000000 labhelper-0.1.0/labhelper/unit_systems/CGS.py
+-rw-rw-rw-   0        0        0     1805 2024-05-06 11:32:38.000000 labhelper-0.1.0/labhelper/unit_systems/SI.py
+-rw-rw-rw-   0        0        0      115 2024-02-11 21:57:37.000000 labhelper-0.1.0/labhelper/unit_systems/__init__.py
+-rw-rw-rw-   0        0        0     1770 2024-04-08 15:16:30.000000 labhelper-0.1.0/labhelper/unit_systems/prefixes.py
+-rw-rw-rw-   0        0        0    12803 2024-05-06 12:07:49.000000 labhelper-0.1.0/labhelper/units.py
+drwxrwxrwx   0        0        0        0 2024-05-06 16:56:30.087884 labhelper-0.1.0/labhelper.egg-info/
+-rw-rw-rw-   0        0        0      804 2024-05-06 16:56:29.000000 labhelper-0.1.0/labhelper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2024-05-06 16:56:29.000000 labhelper-0.1.0/labhelper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 16:56:29.000000 labhelper-0.1.0/labhelper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-06 16:56:29.000000 labhelper-0.1.0/labhelper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-06 16:56:29.000000 labhelper-0.1.0/labhelper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 16:56:30.093887 labhelper-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1213 2024-05-06 16:55:53.000000 labhelper-0.1.0/setup.py
```

### Comparing `labhelper-0.0.7/PKG-INFO` & `labhelper-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-Metadata-Version: 2.1
-Name: labhelper
-Version: 0.0.7
-Summary: A basic package with handy function for lab work, made for Jupyter Notebooks
-Home-page: UNKNOWN
-Author: Batres (Javier Batres)
-Author-email: <javibatresdc@gmail.com>
-License: UNKNOWN
-Keywords: python,data analysis,lab,data,symbolic
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Framework :: Jupyter
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-
-A package with utility functions to make using python in the lab faster, specifically for the Complutense University of Madrid Physics Bachelor.
-
+Metadata-Version: 2.1
+Name: labhelper
+Version: 0.1.0
+Summary: A basic package with handy function for lab work, made for Jupyter Notebooks
+Author: Batres (Javier Batres)
+Author-email: <javibatresdc@gmail.com>
+Keywords: python,data analysis,lab,data,symbolic
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Framework :: Jupyter
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+
+A package with utility functions to make using python in the lab faster, specifically for the Complutense University of Madrid Physics Bachelor.
```

### Comparing `labhelper-0.0.7/README.md` & `labhelper-0.1.0/README.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# Lab-Helper
-
-Basic python library to help with the boring parts of lab work (calculation the error function, making tables, finding the required value of a certain parameter in order to make the error function have a certain value, ...)
-it is currently very much in development, some interesting things have been added, especially in the domain of symbolic computation, but it is quite bare-bones, I hope to add more to it not only this year but even during my Masters and/or PHD.
-
-If anyone wants to contribute it would be very much appreciated, just submit a push request and I'll review and most likely accept it.
-
-## Requirements
-- Python 3.8+ (probably works on earlier versions but I haven't tested nor is there any point in doing so)
-- Jupyter Notebooks (this library is specifically made for use in jupyter, it's not incompatible with regular python scripts, but it also probably won't work very well)
-
-## Installation
-If all you want is the working library you can either install it through `pip` as follows:
-```
-pip install labhelper
-```
-If you want to contribute you should clone the git repository, and install it locally instead of through pip:
-```
-cd C:\Whatever\Directory\You\Want //same as cd [Directory]
-git clone https://github.com/Batres3/Lab-Helper.git
-cd Lab-Helper
-pip install .
-```
-## Contributing
-Simply develop whichever new features you consider useful, the way to do this is to edit the files where you cloned the repository (I use Visual Studio Code), and whenever you want to test a change you have make simply do the following (inside the ./Lab-Helper directory):
-```
-pip uninstall labhelper
-pip install .
-```
-Now when you put `import labhelper as hp` into a new python environment, it will load the changes you have made to it
-
-## Usage
-In order to use this package simply go into a new Jupyter Notebook and, just like any other python package, write `import labhelper as hp` at the very top
-When you want to use a function from the library simply do:
-```
-hp.[name of whatever you want to use]
-```
-You can also do `from labhelper import *` instead of `import labhelper as hp` this will make it so you don't have to add `hp.` in front of every function, although I personally prefer adding it
-## Issues
-You can either post the issues in the `Issues` tab at the top of the github site, or contact me personally.
+# Lab-Helper
+
+Basic python library to help with the boring parts of lab work (calculation the error function, making tables, finding the required value of a certain parameter in order to make the error function have a certain value, ...)
+it is currently very much in development, some interesting things have been added, especially in the domain of symbolic computation, but it is quite bare-bones, I hope to add more to it not only this year but even during my Masters and/or PHD.
+
+If anyone wants to contribute it would be very much appreciated, just submit a push request and I'll review and most likely accept it.
+
+## Requirements
+- Python 3.8+ (probably works on earlier versions but I haven't tested nor is there any point in doing so)
+- Jupyter Notebooks (this library is specifically made for use in jupyter, it's not incompatible with regular python scripts, but it also probably won't work very well)
+
+## Installation
+If all you want is the working library you can either install it through `pip` as follows:
+```
+pip install labhelper
+```
+If you want to contribute you should clone the git repository, and install it locally instead of through pip:
+```
+cd C:\Whatever\Directory\You\Want //same as cd [Directory]
+git clone https://github.com/Batres3/Lab-Helper.git
+cd Lab-Helper
+pip install .
+```
+## Contributing
+Simply develop whichever new features you consider useful, the way to do this is to edit the files where you cloned the repository (I use Visual Studio Code), and whenever you want to test a change you have make simply do the following (inside the ./Lab-Helper directory):
+```
+pip uninstall labhelper
+pip install .
+```
+Now when you put `import labhelper as hp` into a new python environment, it will load the changes you have made to it
+
+## Usage
+In order to use this package simply go into a new Jupyter Notebook and, just like any other python package, write `import labhelper as hp` at the very top
+When you want to use a function from the library simply do:
+```
+hp.[name of whatever you want to use]
+```
+You can also do `from labhelper import *` instead of `import labhelper as hp` this will make it so you don't have to add `hp.` in front of every function, although I personally prefer adding it
+## Issues
+You can either post the issues in the `Issues` tab at the top of the github site, or contact me personally.
```

### Comparing `labhelper-0.0.7/labhelper/pandas_utils.py` & `labhelper-0.1.0/labhelper/pandas_utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-import pandas as pd
-import pyperclip as pc
-from numpy import zeros
-from .units import Quantity
-
-def df_switch_columns(df: pd.DataFrame, column1, column2):
-    """
-    Returns a new DataFrame with the required columns switched (DOES NOT MODIFY ORIGINAL DATAFRAME)
-    """
-    i = list(df.columns)
-    a, b = i.index(column1), i.index(column2)
-    i[b], i[a] = i[a], i[b]
-    df = df[i]
-    return df
-
-def df_switch_rows(df: pd.DataFrame, row1, row2):
-    """
-    Returns a new DataFrame with the required rows switched (DOES NOT MODIFY ORIGINAL DATAFRAME), not efficient for very large DataFrames (>1000 rows)
-    """
-    ids = df.index.tolist()
-    a, b = ids.index(row1), ids.index(row2)
-    ids[a], ids[b] = ids[b], ids[a]
-    df = df.reindex(ids)
-    return df
-
-def df_create(columns, indices) -> pd.DataFrame:
-    """
-    Returns a new DataFrame with the specified columns and indexes, 
-    these can be given as a list of names (columns -> ["Input 1", "Input 2"], rows -> ["Experiment 1", "Experiment 2"])
-    or as a number of columns or indexes.
-    It is valid to supply a list for the columns and a number for the indices, and vice versa.
-    """
-    if type(columns) == int and type(indices) == int:
-        return pd.DataFrame(columns=range(columns), index=range(indices)).fillna(0)
-    elif type(columns) == int and type(indices) == list:
-        return pd.DataFrame(columns=range(columns), index=indices).fillna(0)
-    elif type(columns) == list and type(indices) == int:
-        return pd.DataFrame(columns=columns, index=range(indices)).fillna(0)
-    elif type(columns) == list and type(indices) == list: 
-        return pd.DataFrame(columns=columns, index=indices).fillna(0)
-    else:
-        raise TypeError("Only integers or lists are supported!")
-
-def copy_to_clipboard(var: str):
-    pc.copy(var)
-
-def df_to_latex(df: pd.DataFrame, number_of_decimals: int | None = 2, index: bool = False, copy_to_clipboard: bool = True):
-    """
-    Turns Pandas DataFrame into a LaTeX table, formatted as ||r|...|r|| for the given number of columns in the
-    DataFrame (because I like the way it looks), automatically copies result into clipboard if copy_to_clipboard is not set to False
-    """
-    if number_of_decimals == None:
-        float_format = None
-    else:
-        float_format = "%." + str(number_of_decimals) + "g"
-
-    table_format = r"||"
-    for i in range(len(df.columns)):
-        table_format += r"c|"
-    table_format += "|"
-    new = []
-    for col in df.columns:
-        type = ""
-        if all(isinstance(a, Quantity) for a in df[col]):
-            type = str(df[col][0]).split(" ", 1)[-1]
-            col += f" ({type})"
-        new.append(col)
-    df.columns = new
-    df = df.map(lambda x: float(x) if isinstance(x, Quantity) else x)
-    basic_latex = df.to_latex(index=index, float_format=float_format, column_format=table_format)
-    latex = basic_latex.replace(r"\toprule", r"\hline\hline").replace(r"\midrule", r"\hline\hline").replace(r"\bottomrule", r"\hline")
-    latex = latex.replace(r"\\", r"\\\hline").replace(r"\\\hline", r"\\", 1)
-    latex = latex.replace("e+", r"\cdot10^").replace("e-", r"\cdot10^-")
-    if copy_to_clipboard:
-        pc.copy(latex)
-    return latex
-
-def multiindex_df(superindices: str | list[str], subindices: list[str], num_rows: int = 0) -> pd.DataFrame:
-    if not isinstance(superindices, list):
-        superindices = [superindices]
-    cols = len(subindices) * len(superindices)
-    data = zeros([num_rows, cols])
-    return pd.DataFrame(data=data, columns=pd.MultiIndex.from_product([superindices, subindices]))
-
+import pandas as pd
+import pyperclip as pc
+from numpy import zeros
+from .units import Quantity
+
+def df_switch_columns(df: pd.DataFrame, column1, column2):
+    """
+    Returns a new DataFrame with the required columns switched (DOES NOT MODIFY ORIGINAL DATAFRAME)
+    """
+    i = list(df.columns)
+    a, b = i.index(column1), i.index(column2)
+    i[b], i[a] = i[a], i[b]
+    df = df[i]
+    return df
+
+def df_switch_rows(df: pd.DataFrame, row1, row2):
+    """
+    Returns a new DataFrame with the required rows switched (DOES NOT MODIFY ORIGINAL DATAFRAME), not efficient for very large DataFrames (>1000 rows)
+    """
+    ids = df.index.tolist()
+    a, b = ids.index(row1), ids.index(row2)
+    ids[a], ids[b] = ids[b], ids[a]
+    df = df.reindex(ids)
+    return df
+
+def df_create(columns, indices) -> pd.DataFrame:
+    """
+    Returns a new DataFrame with the specified columns and indexes, 
+    these can be given as a list of names (columns -> ["Input 1", "Input 2"], rows -> ["Experiment 1", "Experiment 2"])
+    or as a number of columns or indexes.
+    It is valid to supply a list for the columns and a number for the indices, and vice versa.
+    """
+    if type(columns) == int and type(indices) == int:
+        return pd.DataFrame(columns=range(columns), index=range(indices)).fillna(0)
+    elif type(columns) == int and type(indices) == list:
+        return pd.DataFrame(columns=range(columns), index=indices).fillna(0)
+    elif type(columns) == list and type(indices) == int:
+        return pd.DataFrame(columns=columns, index=range(indices)).fillna(0)
+    elif type(columns) == list and type(indices) == list: 
+        return pd.DataFrame(columns=columns, index=indices).fillna(0)
+    else:
+        raise TypeError("Only integers or lists are supported!")
+
+def copy_to_clipboard(var: str):
+    pc.copy(var)
+
+def df_to_latex(df: pd.DataFrame, number_of_decimals: int | None = 2, index: bool = False, copy_to_clipboard: bool = True):
+    """
+    Turns Pandas DataFrame into a LaTeX table, formatted as ||r|...|r|| for the given number of columns in the
+    DataFrame (because I like the way it looks), automatically copies result into clipboard if copy_to_clipboard is not set to False
+    """
+    if number_of_decimals == None:
+        float_format = None
+    else:
+        float_format = "%." + str(number_of_decimals) + "g"
+
+    table_format = r"||"
+    for i in range(len(df.columns)):
+        table_format += r"c|"
+    table_format += "|"
+    new = []
+    for col in df.columns:
+        type = ""
+        if all(isinstance(a, Quantity) for a in df[col]):
+            type = str(df[col][0]).split(" ", 1)[-1]
+            col += f" ({type})"
+        new.append(col)
+    df.columns = new
+    df = df.map(lambda x: float(x) if isinstance(x, Quantity) else x)
+    basic_latex = df.to_latex(index=index, float_format=float_format, column_format=table_format)
+    latex = basic_latex.replace(r"\toprule", r"\hline\hline").replace(r"\midrule", r"\hline\hline").replace(r"\bottomrule", r"\hline")
+    latex = latex.replace(r"\\", r"\\\hline").replace(r"\\\hline", r"\\", 1)
+    latex = latex.replace("e+", r"\cdot10^").replace("e-", r"\cdot10^-")
+    if copy_to_clipboard:
+        pc.copy(latex)
+    return latex
+
+def multiindex_df(superindices: str | list[str], subindices: list[str], num_rows: int = 0) -> pd.DataFrame:
+    if not isinstance(superindices, list):
+        superindices = [superindices]
+    cols = len(subindices) * len(superindices)
+    data = zeros([num_rows, cols])
+    return pd.DataFrame(data=data, columns=pd.MultiIndex.from_product([superindices, subindices]))
+
```

### Comparing `labhelper-0.0.7/labhelper/stats.py` & `labhelper-0.1.0/labhelper/stats.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from scipy.stats import t
-from pandas import Series
-import numpy as np
-
-def random_error_of_mean(std, num_samples, confidence):
-    """
-    Calculates the random uncertainty of the mean of a set of samples following the formula:
-
-        t_n-1 * (σ_n-1 / √n)
-    """
-    return std * student_t_n(num_samples - 1, confidence) / np.sqrt(num_samples)
-
-def student_t_n(degrees_of_freedom, confidence):
-    """
-    Returns the t_n,ɑ/2 coefficient for the given degree of freedom and confidence level.
-    Exact same inputs and outputs as the cheat sheet table from year 1
-    """
-    return t.ppf(1 - (1-confidence)*0.5, degrees_of_freedom)
-
-def coefficient_errors(cov):
-    return np.sqrt(np.diag(cov))
-
-def bootstrap_points(x: list[float] | Series, y: list[float] | Series, xerr: list[float], yerr: list[float], num: int, keep_originals: bool = False, full_confidence: bool = False):
-    if len(x) != len(y):
-        raise ValueError("Lengths of x and y do not match!")
-    if len(x) != len(xerr):
-        raise ValueError("Lengths of x and xerr do not match!")
-    if len(y) != len(yerr):
-        raise ValueError("Lengths of y and yerr do not match!")
-
-    xgen, ygen = [list(np.random.normal(xi, xierr * 0.5, num)) for xi, xierr in zip(x, xerr)], [list(np.random.normal(yi, yierr * 0.5, num)) for yi, yierr in zip(y, yerr)]
-    xgen, ygen = sum(xgen, []), sum(ygen, []) # combine lists into one list
-    if keep_originals:
-        if type(x) == Series and type(y) == Series:
-            xgen, ygen = x.to_list() + xgen, y.to_list() + ygen
-        else:
-            xgen, ygen = x.append(xgen), y.append(ygen)
-    return xgen, ygen
-
+from scipy.stats import t
+from pandas import Series
+import numpy as np
+
+def random_error_of_mean(std, num_samples, confidence):
+    """
+    Calculates the random uncertainty of the mean of a set of samples following the formula:
+
+        t_n-1 * (σ_n-1 / √n)
+    """
+    return std * student_t_n(num_samples - 1, confidence) / np.sqrt(num_samples)
+
+def student_t_n(degrees_of_freedom, confidence):
+    """
+    Returns the t_n,ɑ/2 coefficient for the given degree of freedom and confidence level.
+    Exact same inputs and outputs as the cheat sheet table from year 1
+    """
+    return t.ppf(1 - (1-confidence)*0.5, degrees_of_freedom)
+
+def coefficient_errors(cov):
+    return np.sqrt(np.diag(cov))
+
+def bootstrap_points(x: list[float] | Series, y: list[float] | Series, xerr: list[float], yerr: list[float], num: int, keep_originals: bool = False, full_confidence: bool = False):
+    if len(x) != len(y):
+        raise ValueError("Lengths of x and y do not match!")
+    if len(x) != len(xerr):
+        raise ValueError("Lengths of x and xerr do not match!")
+    if len(y) != len(yerr):
+        raise ValueError("Lengths of y and yerr do not match!")
+
+    xgen, ygen = [list(np.random.normal(xi, xierr * 0.5, num)) for xi, xierr in zip(x, xerr)], [list(np.random.normal(yi, yierr * 0.5, num)) for yi, yierr in zip(y, yerr)]
+    xgen, ygen = sum(xgen, []), sum(ygen, []) # combine lists into one list
+    if keep_originals:
+        if type(x) == Series and type(y) == Series:
+            xgen, ygen = x.to_list() + xgen, y.to_list() + ygen
+        else:
+            xgen, ygen = x.append(xgen), y.append(ygen)
+    return xgen, ygen
+
```

### Comparing `labhelper-0.0.7/labhelper/unit_systems/CGS.py` & `labhelper-0.1.0/labhelper/unit_systems/CGS.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from . import __define_unit
-from .prefixes import *
-from ..units import Quantity, DefaultUnits
-
-centimetre = Quantity(1e-2, DefaultUnits.meter, custom_string="cm", expect_self=True)
-gram = Quantity(1e-3, DefaultUnits.kilogram, custom_string="g", expect_self=True)
-second = Quantity(1, DefaultUnits.second, custom_string="s", expect_self=True)
-gal = centimetre/second**2
-__define_unit(gal, "Gal")
-dyne = gram*centimetre/second**2
-__define_unit(dyne, "dyn")
-erg = gram * centimetre**2/second**2
-__define_unit(erg, "erg")
-barye = gram/(centimetre*second**2)
-__define_unit(barye, "Ba")
-poise = gram/(centimetre*second)
-__define_unit(poise, "P")
-stokes = centimetre**2/second
-__define_unit(stokes, "St")
-kayser = centimetre**-1
-__define_unit(kayser, "K")
-
+from . import __define_unit
+from .prefixes import *
+from ..units import Quantity, DefaultUnits
+
+centimetre = Quantity(1e-2, DefaultUnits.meter, custom_string="cm", expect_self=True)
+gram = Quantity(1e-3, DefaultUnits.kilogram, custom_string="g", expect_self=True)
+second = Quantity(1, DefaultUnits.second, custom_string="s", expect_self=True)
+gal = centimetre/second**2
+__define_unit(gal, "Gal")
+dyne = gram*centimetre/second**2
+__define_unit(dyne, "dyn")
+erg = gram * centimetre**2/second**2
+__define_unit(erg, "erg")
+barye = gram/(centimetre*second**2)
+__define_unit(barye, "Ba")
+poise = gram/(centimetre*second)
+__define_unit(poise, "P")
+stokes = centimetre**2/second
+__define_unit(stokes, "St")
+kayser = centimetre**-1
+__define_unit(kayser, "K")
+
```

### Comparing `labhelper-0.0.7/labhelper/unit_systems/SI.py` & `labhelper-0.1.0/labhelper/unit_systems/SI.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,62 @@
-from . import __define_unit
-from .prefixes import *
-from ..units import Quantity, DefaultUnits
-
-meter = Quantity(1, DefaultUnits.meter, custom_string="m", expect_self=True)
-second = Quantity(1, DefaultUnits.second, custom_string="s", expect_self=True)
-kilogram = Quantity(1, DefaultUnits.kilogram, custom_string="kg", expect_self=True)
-gram = Quantity(1e-3, DefaultUnits.kilogram, custom_string="g", expect_self=True)
-kelvin = Quantity(1, DefaultUnits.kelvin, custom_string="K", expect_self=True)
-ampere = Quantity(1, DefaultUnits.ampere, custom_string="A", expect_self=True)
-mol = Quantity(1, DefaultUnits.mol, custom_string="mol", expect_self= True)
-candela = Quantity(1, DefaultUnits.candela,custom_string="cd", expect_self=True)
-
-hertz = second**-1
-__define_unit(hertz, "Hz")
-newton = kilogram*meter*second**-2
-__define_unit(newton, "N")
-pascal = newton/meter**2
-__define_unit(pascal, "Pa")
-joule = newton*meter
-__define_unit(joule, "J")
-watt = joule/second
-__define_unit(watt, "W")
-coulomb = ampere*second
-__define_unit(coulomb, "C")
-volt = joule/coulomb
-__define_unit(volt, "V")
-electronvolt = 1.6e-19*joule
-__define_unit(electronvolt, "eV")
-farad = coulomb/volt
-__define_unit(farad, "F")
-ohm = volt/ampere
-__define_unit(ohm, "Ω")
-siemens = ohm**-1
-__define_unit(siemens, "S")
-weber = volt*second
-__define_unit(weber, "Wb")
-tesla = weber/meter**2
-__define_unit(tesla, "T")
-henry = weber/ampere
-__define_unit(henry, "H")
-# TODO: ºC
-
-lumen = 1*candela
-__define_unit(lumen, "lm")
-lux = lumen/meter**2
-__define_unit(lux, "lx")
-becquerel = second**-1
-__define_unit(becquerel, "Bq")
-gray = joule/kilogram
-__define_unit(gray, "Gy")
-sievert = joule/kilogram
-__define_unit(sievert, "Sv")
-katal = mol*second**-1
-__define_unit(katal, "kat")
+from . import __define_unit
+from .prefixes import *
+from ..units import Quantity
+
+meter = Quantity(1, 2, custom_string="m", expect_self=True)
+second = Quantity(1, 3, custom_string="s", expect_self=True)
+kilogram = Quantity(1, 5, custom_string="kg", expect_self=True)
+gram = Quantity(1e-3, 5, custom_string="g", expect_self=True)
+kelvin = Quantity(1, 7, custom_string="K", expect_self=True)
+ampere = Quantity(1, 11, custom_string="A", expect_self=True)
+mol = Quantity(1, 13, custom_string="mol", expect_self= True)
+candela = Quantity(1, 17,custom_string="cd", expect_self=True)
+
+hertz = second**-1
+__define_unit(hertz, "Hz")
+newton = kilogram*meter*second**-2
+__define_unit(newton, "N")
+pascal = newton/meter**2
+__define_unit(pascal, "Pa")
+atmosphere = 101325 * pascal
+__define_unit(atmosphere, "atm")
+bar = 100000 * pascal
+__define_unit(bar, "bar")
+joule = newton*meter
+__define_unit(joule, "J")
+watt = joule/second
+__define_unit(watt, "W")
+coulomb = ampere*second
+__define_unit(coulomb, "C")
+volt = joule/coulomb
+__define_unit(volt, "V")
+electronvolt = 1.6e-19*joule
+__define_unit(electronvolt, "eV")
+farad = coulomb/volt
+__define_unit(farad, "F")
+ohm = volt/ampere
+__define_unit(ohm, "Ω")
+siemens = ohm**-1
+__define_unit(siemens, "S")
+weber = volt*second
+__define_unit(weber, "Wb")
+tesla = weber/meter**2
+__define_unit(tesla, "T")
+henry = weber/ampere
+__define_unit(henry, "H")
+# TODO: ºC
+
+lumen = 1*candela
+__define_unit(lumen, "lm")
+lux = lumen/meter**2
+__define_unit(lux, "lx")
+becquerel = second**-1
+__define_unit(becquerel, "Bq")
+gray = joule/kilogram
+__define_unit(gray, "Gy")
+sievert = joule/kilogram
+__define_unit(sievert, "Sv")
+katal = mol*second**-1
+__define_unit(katal, "kat")
+
+liter = (deci*meter)**3
+__define_unit(liter, "L")
```

### Comparing `labhelper-0.0.7/labhelper/units.py` & `labhelper-0.1.0/labhelper/units.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,291 +1,283 @@
-from numbers import Number
-from enum import IntEnum
-from typing import Callable
-from fractions import Fraction
-from math import sqrt, prod, ceil, floor, trunc
-
-def prime_factorization_int(n: int) -> list[tuple[int, int]]:
-    if n == 1:
-        return []
-    elif n == 0:
-        return []
-
-    fac = []
-    powers = []
-    count = 0
-    while n % 2 == 0:
-        count += 1
-        n = n // 2
-    fac.append(2) if count > 0 else 0
-    powers.append(count) if count > 0 else 0
-    # n must be odd at this point
-    # so a skip of 2 ( i = i + 2) can be used
-    for i in range(3,int(sqrt(n))+1,2):
-        # while i divides n , add i to the list
-        count = 0
-        while n % i== 0:
-            count += 1
-            n = n // i
-        fac.append(i) if count > 0 else 0
-        powers.append(count) if count > 0 else 0
-    # Condition if n is a prime
-    # number greater than 2
-    if n > 2:
-        fac.append(n)
-        powers.append(1) 
-    return [(factor, power) for factor, power in zip(fac, powers)]
-
-
-def prime_factorization(n: float) -> list[tuple[int, int]]:
-    positive_factors = []
-    negative_factors = []
-
-    top, bottom = Fraction(n).limit_denominator().as_integer_ratio()
-    positive_factors = prime_factorization_int(top)
-    negative_factors = [(factor, -power) for factor, power in prime_factorization_int(bottom)]
-    final = positive_factors + negative_factors
-    final.sort()
-    return final
-
-def custom_factors(n: float, custom_factors: list[float]):
-    num_factors = prime_factorization(n)
-    factors_check = [prime_factorization(custom) for custom in custom_factors]
-    final = []
-    for fac, custom in zip(factors_check, custom_factors):
-        if all(prime_fac[0] in [e[0] for e in num_factors] for prime_fac in fac):
-        #if all(prime_fac[0] == prime_n[0] and abs(prime_fac[1]) <= abs(prime_n[1]) for prime_fac, prime_n in zip(fac, num_factors)):
-            matching = [a for a in num_factors if a[0] in [b[0] for b in fac]]
-            not_matching = [a for a in num_factors if a not in matching]
-            power = min([prime_n[1]//prime_fac[1] for prime_fac, prime_n in zip(fac, matching)], key=abs)
-            num_factors = [(prime_n[0], prime_n[1] - prime_fac[1]*power) for prime_fac, prime_n in zip(fac, matching) if prime_n[1] - prime_fac[1]*power != 0] + not_matching
-            final.append((custom, power))
-    return final + num_factors
-
-class DefaultUnits(IntEnum):
-    none = 1
-    meter = 2
-    second = 3
-    kilogram = 5
-    kelvin = 7
-    ampere = 11
-    mol = 13
-    candela = 17
-
-    def __str__(self):
-        match self:
-            case DefaultUnits.none:
-                return ""
-            case DefaultUnits.meter:
-                return "m"
-            case DefaultUnits.second:
-                return "s"
-            case DefaultUnits.kilogram:
-                return "kg"
-            case DefaultUnits.kelvin:
-                return "K"
-            case DefaultUnits.ampere:
-                return "A"
-            case DefaultUnits.mol:
-                return "mol"
-            case DefaultUnits.candela:
-                return "cd"
-
-class Quantity:
-    _SI_map: dict[int, str] = {2: "m", 3:"s", 5:"kg", 7:"K", 11:"A", 13:"mol", 17:"cd"}
-    def __init__(self, value: Number = 1, units: float = 1, expected_units: list = [], custom_string: str = "", expect_self: bool = False) -> None:
-        self.units = units
-        self.value = value
-        self.expected_units: list[Quantity] = expected_units
-        self.unit_map = Quantity._SI_map
-        self.custom_string: str = custom_string
-        if expect_self:
-            self.expected_units = [self]
-
-    def _units_to_strings(self) -> tuple[Number, str]:
-        units_vals = self.units
-        value = self.value
-        custom_map = self.unit_map | {unit.units:unit.custom_string for unit in self.expected_units}
-        units = []
-        factors = custom_factors(units_vals, [e.units for e in self.expected_units])
-        for unit in self.expected_units:
-            try:
-                power = [e[1] for e in factors if e[0] == unit.units][0]
-            except:
-                continue
-            value /= unit.value**power
-
-        units = [f"{custom_map.get(e[0])}^{e[1]}" if e[1] != 1 else f"{custom_map.get(e[0])}" for e in factors]
-        return value, " * ".join(units)
-
-    def _set_custom_string(self, text: str) -> None:
-        self.custom_string = text
-
-    def _get_expected_units(self, other, division: bool = False) -> list | None:
-        if self.expected_units[0].units == DefaultUnits.none or other.expected_units[0].units == DefaultUnits.none:
-            unit1, unit2 = self.expected_units[0], other.expected_units[0]
-            newUnit = Quantity(value=unit1.value*unit2.value, units=unit1.units*unit2.units)
-            newUnit.custom_string = unit1.custom_string + unit2.custom_string
-            return [newUnit]
-        final_self = [a for a in self.expected_units if a.units not in [e.units for e in other.expected_units]]
-        return final_self + other.expected_units
-    
-    def __str__(self): 
-        val, units = self._units_to_strings() 
-        return f"{val} {units}"
-
-    def __repr__(self):
-        return str(self)
-
-    # Multiplication
-    
-    def __mul__(self, other):
-        if isinstance(other, Number):
-            return Quantity(value=self.value*other, units=self.units, expected_units=self.expected_units, custom_string=self.custom_string)
-        if isinstance(other, Quantity):
-            return Quantity(value=self.value*other.value, units=self.units*other.units, expected_units=self._get_expected_units(other))
-
-    def __rmul__(self, other):
-        if isinstance(other, Number):
-            return Quantity(value=self.value*other, units=self.units, expected_units=self.expected_units, custom_string=self.custom_string)
-
-    def __truediv__(self, other):
-        if isinstance(other, Number):
-            return Quantity(value=self.value/other, units=self.units, custom_string=self.custom_string, expected_units=self.expected_units)
-        if isinstance(other, Quantity):
-            return Quantity(value=self.value/other.value, units=self.units/other.units, expected_units=self._get_expected_units(other))
-
-    def __rtruediv__(self, other):
-        if isinstance(other, Number):
-            return Quantity(value=other/self.value, units=1/self.units, custom_string=self.custom_string, expected_units=self.expected_units)
-
-    def __floordiv__(self, other):
-        if isinstance(other, Number):
-            return Quantity(value=self.value//other, units=self.units, custom_string=self.custom_string, expected_units=self.expected_units)
-        if isinstance(other, Quantity):
-            return Quantity(value=self.value//other.value, units=self.units/other.units, expected_units=self._get_expected_units(other))
-    def __rfloordiv__(self, other):
-        if isinstance(other, Number):
-            return Quantity(value=other//self.value, units=1/self.units, custom_string=self.custom_string, expected_units=self.expected_units)
-    def __mod__(self, other):
-        if isinstance(other, Number):
-            return Quantity(value=self.value%other, units=self.units, custom_string=self.custom_string, expected_units=self.expected_units)
-        if isinstance(other, Quantity):
-            return Quantity(value=self.value%other.value, units=self.units/other.units, expected_units=self._get_expected_units(other))
-    def __rmod__(self, other):
-        if isinstance(other, Number):
-            return Quantity(value=other%self.value, units=1/self.units, custom_string=self.custom_string, expected_units=self.expected_units)
-
-    def __pow__(self, other):
-        if isinstance(other, int):
-            return Quantity(value=self.value**other, units=self.units**other, expected_units=self.expected_units)
-
-    # Comparison
-    def __lt__(self, other):
-        if isinstance(other, Quantity):
-            if other.units == self.units:
-                return self.value < other.value
-            else:
-                raise ValueError("Units do not match!")
-        else:
-            raise ValueError("Comparison is only valid between Quantities")
-    def __gt__(self, other):
-        return not self < other
-    def __eq__(self, other):
-        if isinstance(other, Quantity):
-            if other.units == self.units:
-                return self.value == other.value
-            else:
-                raise ValueError("Units do not match!")
-        else:
-            raise ValueError("Comparison is only valid between Quantities")
-    def __le__(self, other):
-        return self < other or self == other
-    def __ge__(self, other):
-        return self > other or self == other
-    def __ne__(self, other):
-        return not self == other
-
-    
-    # Addition
-    def __neg__(self):
-        return Quantity(value=-self.value, units=self.units, custom_string=self.custom_string, expected_units=self.expected_units)
-    def __add__(self, other):
-        if isinstance(other, Quantity):
-            if self.units != other.units:
-                raise ValueError("Units do not match!")
-            return Quantity(value=self.value+other.value, units=self.units, expected_units=self._get_expected_units(other))
-        else:
-            raise ValueError("Quantities can only be added with other quantities")
-    def __radd__(self, other):
-        if not isinstance(other, Quantity):
-            raise ValueError("Quantities can only be added with other quantities")
-    def __sub__(self, other):
-        return self.__add__(-other)
-
-    def __float__(self):
-        return float(self.value)
-    
-    # Rounding
-
-    def __round_general__(self, method: Callable, decimals: int | None = None):
-        value = self.value
-        value /= prod([e.value for e in self.expected_units])
-        rounded = method(value, decimals) if decimals is not None else method(value)
-        value = rounded * prod([e.value for e in self.expected_units])
-        return Quantity(value=value, units=self.units, custom_string=self.custom_string, expected_units=self.expected_units)
-    def __round__(self, decimals = 0): return self.__round_general__(round, decimals)
-    def __ceil__(self): return self.__round_general__(ceil)
-    def __floor__(self): return self.__round_general__(floor)
-    def __trunc__(self): return self.__round_general__(trunc)
-
-    # For numpy support -> 
-
-    def sqrt(self): return sqrt(self.value)
-    def rint(self): return self.__round__()
-    
-def work_on_units(func):
-    def wrapper(*args, **kwargs):
-        if args:
-            args = list(args)
-            arg = args.pop(0)
-            if isinstance(arg, Quantity):
-                final = func(arg, *args, **kwargs) if args else func(arg, **kwargs)
-            elif isinstance(arg, list):
-                final = []
-                for a in arg:
-                    final.append(wrapper(a, *args, **kwargs) if args else wrapper(a, **kwargs))
-            else:
-                final = arg
-            return final
-        else:
-            arg = kwargs.pop(list(kwargs.keys())[0])
-            if isinstance(arg, Quantity):
-                final = func(arg, **kwargs) if args else func(arg)
-            elif isinstance(arg, list):
-                final = []
-                for a in arg:
-                    final.append(wrapper(a, **kwargs) if args else wrapper(a, **kwargs))
-            else:
-                final = arg
-            return final
-    return wrapper
-@work_on_units
-def remove_units(x: Quantity):
-    val = x.value
-    for unit in x.expected_units:
-        val /= unit.value
-    return val
-
-@work_on_units
-def to_SI(x: Quantity):
-    return Quantity(x.value, x.units, [], custom_string = x.custom_string)
-
-@work_on_units
-def to_units(x, units):
-    if not isinstance(units, list):
-        units = [units]
-    final = []
-    for unit in units:
-        final += unit.expected_units
-    expected_units = final
-    return Quantity(x.value, x.units, expected_units, x.custom_string)
+from numbers import Number
+from enum import IntEnum
+from typing import Callable
+from fractions import Fraction
+from math import sqrt, prod, ceil, floor, trunc, log
+
+def prime_factorization_int(n: int) -> list[tuple[int, int]]:
+    if n == 1:
+        return []
+    elif n == 0:
+        return []
+
+    fac = []
+    powers = []
+    count = 0
+    while n % 2 == 0:
+        count += 1
+        n = n // 2
+    fac.append(2) if count > 0 else 0
+    powers.append(count) if count > 0 else 0
+    # n must be odd at this point
+    # so a skip of 2 ( i = i + 2) can be used
+    for i in range(3,int(sqrt(n))+1,2):
+        # while i divides n , add i to the list
+        count = 0
+        while n % i== 0:
+            count += 1
+            n = n // i
+        fac.append(i) if count > 0 else 0
+        powers.append(count) if count > 0 else 0
+    # Condition if n is a prime
+    # number greater than 2
+    if n > 2:
+        fac.append(n)
+        powers.append(1) 
+    return [(factor, power) for factor, power in zip(fac, powers)]
+
+
+def prime_factorization(n: Fraction) -> list[tuple[int, int]]:
+    positive_factors = []
+    negative_factors = []
+
+    positive_factors = prime_factorization_int(n.numerator)
+    negative_factors = [(factor, -power) for factor, power in prime_factorization_int(n.denominator)]
+    final = positive_factors + negative_factors
+    final.sort()
+    return final
+
+def custom_factors(n: Fraction, custom_factors: list[Fraction]): # TODO: Check this because it's probably wildly unoptimized
+    custom_factors = [e for e in custom_factors if e != 1]
+    num_factors = prime_factorization(n)
+    factors_check = [prime_factorization(custom) for custom in custom_factors]
+    final = []
+    for fac, custom in zip(factors_check, custom_factors):
+        #if all(prime_fac[0] in [e[0] for e in num_factors] for prime_fac in fac):
+        not_matching = [a for a in fac if a[0] not in [b[0] for b in num_factors] ]
+        if not_matching:
+            final.append((custom, 1))
+            common_num = [a for a in num_factors if a[0] in [b[0] for b in fac]]
+            different_num = [a for a in num_factors if a not in common_num]
+            common_fac = [a for a in fac if a[0] in [b[0] for b in num_factors]]
+            different_fac = [a for a in fac if a not in common_fac]
+            common = [(a[0], a[1] - b[1]) for a, b in zip(common_num, common_fac)]
+            num_factors = common + different_num + [(a[0], -a[1]) for a in different_fac]
+            continue
+            
+        matching = [a for a in num_factors if a[0] in [b[0] for b in fac]]
+        not_matching = [a for a in num_factors if a not in matching]
+        power = min([prime_n[1]//prime_fac[1] for prime_fac, prime_n in zip(fac, matching)], key=abs)
+        if power == 0:
+            num_factors = [(prime_n[0], prime_n[1] - prime_fac[1]) for prime_fac, prime_n in zip(fac, matching) if prime_n[1] - prime_fac[1] != 0] + not_matching
+            final.append((custom, 1))
+        else:
+            num_factors = [(prime_n[0], prime_n[1] - prime_fac[1]*power) for prime_fac, prime_n in zip(fac, matching) if prime_n[1] - prime_fac[1]*power != 0] + not_matching
+            final.append((custom, power))
+    return [e for e in final + num_factors if e[1] != 0]
+
+class Quantity:
+    _SI_map: dict[int, str] = {2: "m", 3:"s", 5:"kg", 7:"K", 11:"A", 13:"mol", 17:"cd"}
+    def __init__(self, value: Number = 1, units: Fraction = 1, expected_units: list = [], custom_string: str = "", expect_self: bool = False) -> None:
+        if not isinstance(units, Fraction):
+            units = Fraction(units)
+        self.units: Fraction = units
+        self.value = value
+        self.expected_units: list[Quantity] = expected_units
+        self.custom_string: str = custom_string
+        if expect_self:
+            self.expected_units = [self]
+
+    def _units_to_strings(self) -> tuple[Number, str]:
+        units_vals = self.units
+        value = self.value
+        custom_map = {unit.units: unit.custom_string for unit in self.expected_units} 
+        custom_map |= {key: val for key, val in Quantity._SI_map.items() if key not in custom_map}
+        units = []
+        factors = custom_factors(units_vals, [e.units for e in self.expected_units])
+        for unit in self.expected_units:
+            try:
+                power = [e[1] for e in factors if e[0] == unit.units][0]
+            except:
+                continue
+            value /= unit.value**power
+
+        units = [f"{custom_map.get(e[0])}^{e[1]}" if e[1] != 1 else f"{custom_map.get(e[0])}" for e in factors]
+        return value, " * ".join(units)
+
+    def _set_custom_string(self, text: str) -> None:
+        self.custom_string = text
+
+    def _get_expected_units(self, other, division: bool = False) -> list | None:
+        if not self.expected_units or not other.expected_units:
+            return self.expected_units + other.expected_units
+
+        if self.expected_units[0].units == 1 or other.expected_units[0].units == 1:
+            unit1, unit2 = self.expected_units[0], other.expected_units[0]
+            newUnit = Quantity(value=unit1.value*unit2.value, units=unit1.units*unit2.units)
+            newUnit.custom_string = unit1.custom_string + unit2.custom_string
+            return [newUnit]
+        final_self = [a for a in self.expected_units if a.units not in [e.units for e in other.expected_units]]
+        if division:
+            return final_self
+        return final_self + other.expected_units
+    
+    def __str__(self, significant_digits: int = 3): 
+        val, units = self._units_to_strings() 
+        modifier = "%." + str(significant_digits) + "g"
+        return f"{modifier % val} {units}"
+
+    def __repr__(self):
+        return str(self)
+
+    # Multiplication
+    
+    def __mul__(self, other):
+        if isinstance(other, Number):
+            return Quantity(value=self.value*other, units=self.units, expected_units=self.expected_units, custom_string=self.custom_string)
+        if isinstance(other, Quantity):
+            return Quantity(value=self.value*other.value, units=self.units*other.units, expected_units=self._get_expected_units(other))
+
+    def __rmul__(self, other):
+        if isinstance(other, Number):
+            return Quantity(value=self.value*other, units=self.units, expected_units=self.expected_units, custom_string=self.custom_string)
+
+    def __truediv__(self, other):
+        if isinstance(other, Number):
+            return Quantity(value=self.value/other, units=self.units, custom_string=self.custom_string, expected_units=self.expected_units)
+        if isinstance(other, Quantity):
+            return Quantity(value=self.value/other.value, units=self.units/other.units, expected_units=self._get_expected_units(other, division=True))
+
+    def __rtruediv__(self, other):
+        if isinstance(other, Number):
+            return Quantity(value=other/self.value, units=1/self.units, custom_string=self.custom_string, expected_units=self.expected_units)
+
+    def __floordiv__(self, other):
+        if isinstance(other, Number):
+            return Quantity(value=self.value//other, units=self.units, custom_string=self.custom_string, expected_units=self.expected_units)
+        if isinstance(other, Quantity):
+            return Quantity(value=self.value//other.value, units=self.units/other.units, expected_units=self._get_expected_units(other, division=True))
+    def __rfloordiv__(self, other):
+        if isinstance(other, Number):
+            return Quantity(value=other//self.value, units=1/self.units, custom_string=self.custom_string, expected_units=self.expected_units)
+    def __mod__(self, other):
+        if isinstance(other, Number):
+            return Quantity(value=self.value%other, units=self.units, custom_string=self.custom_string, expected_units=self.expected_units)
+        if isinstance(other, Quantity):
+            return Quantity(value=self.value%other.value, units=self.units/other.units, expected_units=self._get_expected_units(other))
+    def __rmod__(self, other):
+        if isinstance(other, Number):
+            return Quantity(value=other%self.value, units=1/self.units, custom_string=self.custom_string, expected_units=self.expected_units)
+
+    def __pow__(self, other):
+        if isinstance(other, int):
+            return Quantity(value=self.value**other, units=self.units**other, expected_units=self.expected_units)
+
+    # Comparison
+    def __lt__(self, other):
+        if isinstance(other, Quantity):
+            if other.units == self.units:
+                return self.value < other.value
+            else:
+                raise ValueError("Units do not match!")
+        else:
+            raise ValueError("Comparison is only valid between Quantities")
+    def __gt__(self, other):
+        return not self < other
+    def __eq__(self, other):
+        if isinstance(other, Quantity):
+            if other.units == self.units:
+                return self.value == other.value
+            else:
+                raise ValueError("Units do not match!")
+        else:
+            raise ValueError("Comparison is only valid between Quantities")
+    def __le__(self, other):
+        return self < other or self == other
+    def __ge__(self, other):
+        return self > other or self == other
+    def __ne__(self, other):
+        return not self == other
+
+    
+    # Addition
+    def __neg__(self):
+        return Quantity(value=-self.value, units=self.units, custom_string=self.custom_string, expected_units=self.expected_units)
+    def __add__(self, other):
+        if isinstance(other, Quantity):
+            if self.units != other.units:
+                raise ValueError("Units do not match!")
+            return Quantity(value=self.value+other.value, units=self.units, expected_units=self._get_expected_units(other))
+        else:
+            raise ValueError("Quantities can only be added with other quantities")
+    def __radd__(self, other):
+        if not isinstance(other, Quantity):
+            raise ValueError("Quantities can only be added with other quantities")
+    def __sub__(self, other):
+        return self.__add__(-other)
+
+    def __float__(self):
+        return float(self.value)
+    
+    # Rounding
+
+    def __round_general__(self, method: Callable, decimals: int | None = None):
+        value = self.value
+        value /= prod([e.value for e in self.expected_units])
+        rounded = method(value, decimals) if decimals is not None else method(value)
+        value = rounded * prod([e.value for e in self.expected_units])
+        return Quantity(value=value, units=self.units, custom_string=self.custom_string, expected_units=self.expected_units)
+    def __round__(self, decimals = 0): return self.__round_general__(round, decimals)
+    def __ceil__(self): return self.__round_general__(ceil)
+    def __floor__(self): return self.__round_general__(floor)
+    def __trunc__(self): return self.__round_general__(trunc)
+
+    # For numpy support:
+
+    def sqrt(self): return sqrt(self.value)
+    def rint(self): return self.__round__()
+    def log(self): return log(self.value)
+    
+def work_on_units(func):
+    def wrapper(*args, **kwargs):
+        if args:
+            args = list(args)
+            arg = args.pop(0)
+            if isinstance(arg, Quantity):
+                final = func(arg, *args, **kwargs) if args else func(arg, **kwargs)
+            elif isinstance(arg, list):
+                final = []
+                for a in arg:
+                    final.append(wrapper(a, *args, **kwargs) if args else wrapper(a, **kwargs))
+            else:
+                final = arg
+            return final
+        else:
+            arg = kwargs.pop(list(kwargs.keys())[0])
+            if isinstance(arg, Quantity):
+                final = func(arg, **kwargs) if args else func(arg)
+            elif isinstance(arg, list):
+                final = []
+                for a in arg:
+                    final.append(wrapper(a, **kwargs) if args else wrapper(a, **kwargs))
+            else:
+                final = arg
+            return final
+    return wrapper
+@work_on_units
+def remove_units(x: Quantity):
+    val, units = x._units_to_strings()
+    return val
+
+@work_on_units
+def to_SI(x: Quantity):
+    return Quantity(x.value, x.units, [], custom_string = x.custom_string)
+
+@work_on_units
+def to_units(x, units):
+    if not isinstance(units, list):
+        units = [units]
+    final = []
+    for unit in units:
+        final += unit.expected_units
+    expected_units = final
+    return Quantity(x.value, x.units, expected_units, x.custom_string)
```

### Comparing `labhelper-0.0.7/labhelper.egg-info/PKG-INFO` & `labhelper-0.1.0/labhelper.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-Metadata-Version: 2.1
-Name: labhelper
-Version: 0.0.7
-Summary: A basic package with handy function for lab work, made for Jupyter Notebooks
-Home-page: UNKNOWN
-Author: Batres (Javier Batres)
-Author-email: <javibatresdc@gmail.com>
-License: UNKNOWN
-Keywords: python,data analysis,lab,data,symbolic
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Framework :: Jupyter
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-
-A package with utility functions to make using python in the lab faster, specifically for the Complutense University of Madrid Physics Bachelor.
-
+Metadata-Version: 2.1
+Name: labhelper
+Version: 0.1.0
+Summary: A basic package with handy function for lab work, made for Jupyter Notebooks
+Author: Batres (Javier Batres)
+Author-email: <javibatresdc@gmail.com>
+Keywords: python,data analysis,lab,data,symbolic
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Framework :: Jupyter
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+
+A package with utility functions to make using python in the lab faster, specifically for the Complutense University of Madrid Physics Bachelor.
```

### Comparing `labhelper-0.0.7/setup.py` & `labhelper-0.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from setuptools import setup, find_packages
-import codecs
-import os
-
-VERSION = '0.0.7'
-DESCRIPTION = 'A basic package with handy function for lab work, made for Jupyter Notebooks'
-LONG_DESCRIPTION = 'A package with utility functions to make using python in the lab faster, specifically for the Complutense University of Madrid Physics Bachelor.'
-
-# Setting up
-setup(
-    name="labhelper",
-    version=VERSION,
-    author="Batres (Javier Batres)",
-    author_email="<javibatresdc@gmail.com>",
-    description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=LONG_DESCRIPTION,
-    packages=find_packages(),
-    python_requires=">=3.5",
-    install_requires=['scipy', 'pandas', 'numpy', 'sympy', 'IPython', 'pyperclip', 'Jinja2', 'seaborn'],
-    keywords=['python', 'data analysis', 'lab', 'data', 'symbolic'],
-    classifiers=[
-        "Development Status :: 1 - Planning",
-        "Intended Audience :: Science/Research",
-        "Programming Language :: Python :: 3.5",
-        "Framework :: Jupyter",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
-    ]
-)
+from setuptools import setup, find_packages
+import codecs
+import os
+
+VERSION = '0.1.0'
+DESCRIPTION = 'A basic package with handy function for lab work, made for Jupyter Notebooks'
+LONG_DESCRIPTION = 'A package with utility functions to make using python in the lab faster, specifically for the Complutense University of Madrid Physics Bachelor.'
+
+# Setting up
+setup(
+    name="labhelper",
+    version=VERSION,
+    author="Batres (Javier Batres)",
+    author_email="<javibatresdc@gmail.com>",
+    description=DESCRIPTION,
+    long_description_content_type="text/markdown",
+    long_description=LONG_DESCRIPTION,
+    packages=find_packages(),
+    python_requires=">=3.5",
+    install_requires=['scipy', 'pandas', 'numpy', 'sympy', 'IPython', 'pyperclip', 'Jinja2', 'seaborn'],
+    keywords=['python', 'data analysis', 'lab', 'data', 'symbolic'],
+    classifiers=[
+        "Development Status :: 1 - Planning",
+        "Intended Audience :: Science/Research",
+        "Programming Language :: Python :: 3.5",
+        "Framework :: Jupyter",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+    ]
+)
```

