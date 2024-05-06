# Comparing `tmp/weightfactors-0.0.2.tar.gz` & `tmp/weightfactors-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weightfactors-0.0.2.tar", max compression
+gzip compressed data, was "weightfactors-0.0.3.tar", max compression
```

## Comparing `weightfactors-0.0.2.tar` & `weightfactors-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2024-02-14 09:09:55.954071 weightfactors-0.0.2/LICENSE
--rw-r--r--   0        0        0      606 2024-03-21 09:12:44.254832 weightfactors-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1968 2024-02-14 11:18:20.224047 weightfactors-0.0.2/README.md
--rw-r--r--   0        0        0       92 2024-02-14 09:05:58.768979 weightfactors-0.0.2/weightfactors/__init__.py
--rw-r--r--   0        0        0        0 2024-02-14 09:05:58.769061 weightfactors-0.0.2/weightfactors/raking/__init__.py
--rw-r--r--   0        0        0    12297 2024-02-14 11:36:58.602509 weightfactors-0.0.2/weightfactors/raking/generalized_raker.py
--rw-r--r--   0        0        0        0 2024-02-14 09:38:04.963250 weightfactors-0.0.2/weightfactors/utils/__init__.py
--rw-r--r--   0        0        0      275 2024-02-14 09:05:58.774255 weightfactors-0.0.2/weightfactors/utils/exceptions.py
--rw-r--r--   0        0        0     2501 1970-01-01 00:00:00.000000 weightfactors-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-02-14 09:09:55.954071 weightfactors-0.0.3/LICENSE
+-rw-r--r--   0        0        0      606 2024-05-06 07:47:28.888804 weightfactors-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1958 2024-05-06 07:47:28.886680 weightfactors-0.0.3/README.md
+-rw-r--r--   0        0        0       92 2024-02-14 09:05:58.768979 weightfactors-0.0.3/weightfactors/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:05:58.769061 weightfactors-0.0.3/weightfactors/raking/__init__.py
+-rw-r--r--   0        0        0    12804 2024-05-06 07:47:28.893080 weightfactors-0.0.3/weightfactors/raking/generalized_raker.py
+-rw-r--r--   0        0        0        0 2024-02-14 09:38:04.963250 weightfactors-0.0.3/weightfactors/utils/__init__.py
+-rw-r--r--   0        0        0      275 2024-02-14 09:05:58.774255 weightfactors-0.0.3/weightfactors/utils/exceptions.py
+-rw-r--r--   0        0        0     2491 1970-01-01 00:00:00.000000 weightfactors-0.0.3/PKG-INFO
```

### Comparing `weightfactors-0.0.2/LICENSE` & `weightfactors-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `weightfactors-0.0.2/pyproject.toml` & `weightfactors-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weightfactors"
-version = "0.0.2"
+version = "0.0.3"
 description = "Calculate weight factors for survey data to approximate a representative sample"
 authors = ["DemianvG <d.vangils@markteffect.nl>"]
 readme = "README.md"
 packages = [{include = "weightfactors"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `weightfactors-0.0.2/README.md` & `weightfactors-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ![Continuous Integration](https://github.com/markteffect/weightfactors/actions/workflows/ci.yml/badge.svg)
-![Python](https://img.shields.io/badge/Python-3.9%20|%203.10-blue)
+![Python](https://img.shields.io/badge/Python-3.9+-blue)
 # **Weight Factors**
 Calculate weight factors for survey data to approximate a representative sample
 
 
 ### **Installation**
 ```python
 pip install weightfactors
```

### Comparing `weightfactors-0.0.2/weightfactors/raking/generalized_raker.py` & `weightfactors-0.0.3/weightfactors/raking/generalized_raker.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             A dictionary mapping column names to a dictionary containing each
                 category and its corresponding population targets
                     Example: {"Gender": {"Male": 0.5, "Female": 0.5}}
         raise_on_extreme: bool, optional
             Whether to raise an error when the weight factors are extreme
                 according to `cutoffs`, else we raise a warning. Default is False.
         cutoffs: Dict[str, float], optional
-            What we consider extreme weight factors. 'lo' is the lower bound (defaults to 0.25)
+            When weights are considered to be extreme. 'lo' is the lower bound (defaults to 0.25)
                 and 'hi' is the upper bound (defaults to 4). If `raise_on_extreme` we raise an
                     error if any weight exceeds the cutoffs, otherwise we clip the extremes to the cutoffs
         exclusion_column: str, optional
             a column of 0's and 1's in the input data that denotes which rows should get a weight factor (1)
                 and which rows should not (0). Rows that should not get weighted get a weight factor of exactly 1.
 
     Example:
@@ -114,18 +114,25 @@
             if not np.isclose(sum([v for _, v in value.items()]), 1.0, atol=1e-4):
                 raise ValueError(
                     f"The sum of the population distribution for '{key}' is not 1"
                 )
             # Make sure all keys are present in the dataset
             if key not in data.columns:
                 raise KeyError(f"There is no column {key} in the provided dataset")
-            # Make sure there are no missing values in the questions used for calculating weights
+            # Make sure there are no missing values in the columns used for calculating weights
             if data[key].isna().any(axis=None):
                 raise ValueError(f"Column {key} contains missing values")
+            # Make sure all unique values in the target columns have been mapped
+            # It is impossible to set values with observations to a weight of 0
+            if len(data[key].unique()) != len(value):
+                raise KeyError(
+                    f"There are observations for a value in '{key}' that has not been mapped to a population target"
+                )
             # Make sure we have at least 1 observation for each category
+            # It is impossible to set values without observations to a weight larger than 1
             for k, _ in value.items():
                 if k not in data[key].unique():
                     raise KeyError(f"There are no observations for {k} in column {key}")
             # Make sure the inclusion column is valid
             if self.exclusion_column:
                 if self.exclusion_column not in data.columns:
                     raise KeyError(f"There is no column {key} in the provided dataset")
@@ -189,19 +196,19 @@
     ) -> np.ndarray[np.float64, Any]:
         """Run the generalized raking algorithm
 
         Args:
             data: pd.DataFrame
                 The survey dataset
             max_steps: int
-                Maximum number of iterations
+                The maximum number of iterations to try and reach convergence
             tolerance: float
-                Maximum tolerance for loss, we claim success if the loss is lower than this
+                Maximum tolerance for loss, convergence is reached if the loss is smaller than this value
             early_stopping: int
-                Maximum number of iterations without improvement in loss before we call quits
+                Maximum number of iterations without improvement in loss
 
         Raises:
             WeightsConvergenceError if the algorithm did not converge before `max_steps`
                 was reached or if `early_stopping` has been triggered
 
         Returns:
             Weight factors as a 1d NumPy array of floats
```

### Comparing `weightfactors-0.0.2/PKG-INFO` & `weightfactors-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: weightfactors
-Version: 0.0.2
+Version: 0.0.3
 Summary: Calculate weight factors for survey data to approximate a representative sample
 Author: DemianvG
 Author-email: d.vangils@markteffect.nl
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 ![Continuous Integration](https://github.com/markteffect/weightfactors/actions/workflows/ci.yml/badge.svg)
-![Python](https://img.shields.io/badge/Python-3.9%20|%203.10-blue)
+![Python](https://img.shields.io/badge/Python-3.9+-blue)
 # **Weight Factors**
 Calculate weight factors for survey data to approximate a representative sample
 
 
 ### **Installation**
 ```python
 pip install weightfactors
```

