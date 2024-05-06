# Comparing `tmp/onekit-1.1.0.tar.gz` & `tmp/onekit-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onekit-1.1.0.tar", max compression
+gzip compressed data, was "onekit-1.1.1.tar", max compression
```

## Comparing `onekit-1.1.0.tar` & `onekit-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1514 2024-04-26 19:17:18.569475 onekit-1.1.0/LICENSE
--rw-r--r--   0        0        0     1569 2024-04-26 19:17:18.569475 onekit-1.1.0/README.md
--rw-r--r--   0        0        0     2204 2024-04-26 19:18:12.657121 onekit-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       88 2024-04-26 19:17:18.609475 onekit-1.1.0/src/onekit/__init__.py
--rw-r--r--   0        0        0     3965 2024-04-26 19:17:18.613475 onekit-1.1.0/src/onekit/mathkit.py
--rw-r--r--   0        0        0     1643 2024-04-26 19:17:18.613475 onekit-1.1.0/src/onekit/numpykit.py
--rw-r--r--   0        0        0    14598 2024-04-26 19:17:18.613475 onekit-1.1.0/src/onekit/optfunckit.py
--rw-r--r--   0        0        0     6799 2024-04-26 19:17:18.613475 onekit-1.1.0/src/onekit/pandaskit.py
--rw-r--r--   0        0        0    37190 2024-04-26 19:17:18.613475 onekit-1.1.0/src/onekit/pythonkit.py
--rw-r--r--   0        0        0    37388 2024-04-26 19:17:18.613475 onekit-1.1.0/src/onekit/sparkkit.py
--rw-r--r--   0        0        0    19542 2024-04-26 19:17:18.613475 onekit-1.1.0/src/onekit/vizkit.py
--rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 onekit-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1514 2024-05-06 21:25:32.769600 onekit-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1569 2024-05-06 21:25:32.769600 onekit-1.1.1/README.md
+-rw-r--r--   0        0        0     2217 2024-05-06 21:26:27.089794 onekit-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       88 2024-05-06 21:25:32.809601 onekit-1.1.1/src/onekit/__init__.py
+-rw-r--r--   0        0        0     3965 2024-05-06 21:25:32.809601 onekit-1.1.1/src/onekit/mathkit.py
+-rw-r--r--   0        0        0     1643 2024-05-06 21:25:32.809601 onekit-1.1.1/src/onekit/numpykit.py
+-rw-r--r--   0        0        0    14598 2024-05-06 21:25:32.809601 onekit-1.1.1/src/onekit/optfunckit.py
+-rw-r--r--   0        0        0     6799 2024-05-06 21:25:32.809601 onekit-1.1.1/src/onekit/pandaskit.py
+-rw-r--r--   0        0        0    37190 2024-05-06 21:25:32.809601 onekit-1.1.1/src/onekit/pythonkit.py
+-rw-r--r--   0        0        0    38022 2024-05-06 21:25:32.809601 onekit-1.1.1/src/onekit/sparkkit.py
+-rw-r--r--   0        0        0    19542 2024-05-06 21:25:32.809601 onekit-1.1.1/src/onekit/vizkit.py
+-rw-r--r--   0        0        0     2483 1970-01-01 00:00:00.000000 onekit-1.1.1/PKG-INFO
```

### Comparing `onekit-1.1.0/LICENSE` & `onekit-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `onekit-1.1.0/README.md` & `onekit-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `onekit-1.1.0/pyproject.toml` & `onekit-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onekit"
-version = "1.1.0"
+version = "1.1.1"
 description = "All-in-One Python Kit."
 authors = ["Eugen Stripling <estripling042@gmail.com>"]
 license = "BSD 3-Clause"
 readme = "README.md"
 repository = "https://github.com/estripling/onekit"
 documentation = "https://onekit.readthedocs.io/en/stable/"
 keywords = ["onekit"]
@@ -14,22 +14,23 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4.0"
+python = ">=3.8.1"
 toolz = "^0.12.0"
+pytz = "^2024.1"
 
 [tool.poetry.group.precommit.dependencies]
 autoflake = "^2.2.1"
 black = {extras = ["jupyter"], version = "^23.11.0"}
 isort = "^5.12.0"
-flake8 = "^6.1.0"
+flake8 = ">=5.0.4"
 pre-commit = "^3.5.0"
 pre-commit-hooks = "^4.5.0"
 
 [tool.poetry.group.testing.dependencies]
 pytest = "^7.4.3"
 pytest-cov = "^4.1.0"
 pytest-skip-slow = "^0.0.5"
```

### Comparing `onekit-1.1.0/src/onekit/mathkit.py` & `onekit-1.1.1/src/onekit/mathkit.py`

 * *Files identical despite different names*

### Comparing `onekit-1.1.0/src/onekit/numpykit.py` & `onekit-1.1.1/src/onekit/numpykit.py`

 * *Files identical despite different names*

### Comparing `onekit-1.1.0/src/onekit/optfunckit.py` & `onekit-1.1.1/src/onekit/optfunckit.py`

 * *Files identical despite different names*

### Comparing `onekit-1.1.0/src/onekit/pandaskit.py` & `onekit-1.1.1/src/onekit/pandaskit.py`

 * *Files identical despite different names*

### Comparing `onekit-1.1.0/src/onekit/pythonkit.py` & `onekit-1.1.1/src/onekit/pythonkit.py`

 * *Files identical despite different names*

### Comparing `onekit-1.1.0/src/onekit/sparkkit.py` & `onekit-1.1.1/src/onekit/sparkkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime as dt
 import functools
+import math
 import os
 from typing import (
     Callable,
     List,
     Sequence,
     Union,
 )
@@ -663,22 +664,27 @@
             id_col,
             F.expr("sequence(min_date, max_date, interval 1 day)").alias(new_col),
         )
         .withColumn(new_col, F.explode(new_col))
     )
 
 
-def filter_date(date_col: str, d0: Union[str, dt.date], n: int) -> SparkDFTransformFunc:
+def filter_date(
+    date_col: str,
+    d0: Union[str, dt.date],
+    n: Union[int, float],
+) -> SparkDFTransformFunc:
     """Returns dataframe with rows such that date is in :math:`(d_{-n}, d_{0}]`.
 
     Notes
     -----
     - :math:`d_{0}`: reference date (inclusive)
     - :math:`d_{-n} < d_{0}`: relative date (exclusive)
     - :math:`n > 0`: number of dates from :math:`d_{-n}` to :math:`d_{0}`
+    - If `n=float("inf")`, returned dates are in :math:`(d_{-\\infty}, d_{0}]`
 
     Examples
     --------
     >>> from pyspark.sql import SparkSession
     >>> import onekit.sparkkit as sk
     >>> spark = SparkSession.builder.getOrCreate()
     >>> df = spark.createDataFrame(
@@ -698,18 +704,38 @@
     |         d|
     +----------+
     |2024-01-05|
     |2024-01-06|
     |2024-01-07|
     +----------+
     <BLANKLINE>
+
+    >>> df.transform(sk.filter_date("d", d0="2024-01-07", n=float("inf"))).show()
+    +----------+
+    |         d|
+    +----------+
+    |2024-01-01|
+    |2024-01-02|
+    |2024-01-03|
+    |2024-01-04|
+    |2024-01-05|
+    |2024-01-06|
+    |2024-01-07|
+    +----------+
+    <BLANKLINE>
     """
-    if not isinstance(n, int) or n < 1:
+    if not isinstance(n, (int, float)):
+        raise TypeError(f"{type(n)=} - must be an int or float")
+
+    if isinstance(n, int) and n < 1:
         raise ValueError(f"{n=} - must be a positive integer")
 
+    if isinstance(n, float) and not math.isinf(n):
+        raise ValueError(f'{n=} - only valid float value: float("inf")')
+
     def inner(df: SparkDF, /) -> SparkDF:
         date_diff_ago = "_date_diff_ago_"
         return (
             df.transform(with_date_diff_ago(date_col, d0, new_col=date_diff_ago))
             .where((F.col(date_diff_ago) >= 0) & (F.col(date_diff_ago) < n))
             .drop(date_diff_ago)
         )
```

### Comparing `onekit-1.1.0/src/onekit/vizkit.py` & `onekit-1.1.1/src/onekit/vizkit.py`

 * *Files identical despite different names*

### Comparing `onekit-1.1.0/PKG-INFO` & `onekit-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: onekit
-Version: 1.1.0
+Version: 1.1.1
 Summary: All-in-One Python Kit.
 Home-page: https://github.com/estripling/onekit
 License: BSD 3-Clause
 Keywords: onekit
 Author: Eugen Stripling
 Author-email: estripling042@gmail.com
-Requires-Python: >=3.8.1,<4.0
+Requires-Python: >=3.8.1
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
+Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: toolz (>=0.12.0,<0.13.0)
 Project-URL: Documentation, https://onekit.readthedocs.io/en/stable/
 Project-URL: Repository, https://github.com/estripling/onekit
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/estripling/onekit/main/docs/source/_static/onekitlogo.png" width="180" alt="onekit logo.">
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: onekit Version: 1.1.0 Summary: All-in-One Python
+Metadata-Version: 2.1 Name: onekit Version: 1.1.1 Summary: All-in-One Python
 Kit. Home-page: https://github.com/estripling/onekit License: BSD 3-Clause
 Keywords: onekit Author: Eugen Stripling Author-email: estripling042@gmail.com
-Requires-Python: >=3.8.1,<4.0 Classifier: License :: Other/Proprietary License
+Requires-Python: >=3.8.1 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
-Only Classifier: Programming Language :: Python :: 3.8 Requires-Dist: toolz
-(>=0.12.0,<0.13.0) Project-URL: Documentation, https://onekit.readthedocs.io/
-en/stable/ Project-URL: Repository, https://github.com/estripling/onekit
-Description-Content-Type: text/markdown
+Only Classifier: Programming Language :: Python :: 3.8 Requires-Dist: pytz
+(>=2024.1,<2025.0) Requires-Dist: toolz (>=0.12.0,<0.13.0) Project-URL:
+Documentation, https://onekit.readthedocs.io/en/stable/ Project-URL:
+Repository, https://github.com/estripling/onekit Description-Content-Type:
+text/markdown
                                 [onekit logo.]
                   _[_p_y_p_i_]_[_p_y_p_i_]_[_d_o_c_s_]_[_t_e_s_t_]_[_c_o_v_e_r_a_g_e_]_[_l_i_c_e_n_s_e_]
 ## About All-in-One Python Kit: - [Examples](https://onekit.readthedocs.io/en/
 stable/examples.html) - [Documentation](https://onekit.readthedocs.io/en/
 stable/index.html) - [Developer Guide](https://onekit.readthedocs.io/en/stable/
 developers.html) - [API Reference](https://onekit.readthedocs.io/en/stable/
 autoapi/index.html) ## Installation `onekit` is available on [PyPI](https://
```

