# Comparing `tmp/pyserrf-0.1.0.tar.gz` & `tmp/pyserrf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyserrf-0.1.0.tar", max compression
+gzip compressed data, was "pyserrf-0.1.1.tar", max compression
```

## Comparing `pyserrf-0.1.0.tar` & `pyserrf-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      603 2024-05-04 16:40:19.958150 pyserrf-0.1.0/README.md
--rw-r--r--   0        0        0      432 2024-04-29 15:18:37.086331 pyserrf-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       26 2024-04-26 15:26:59.997208 pyserrf-0.1.0/pyserrf/__init__.py
--rw-r--r--   0        0        0     4293 2024-04-18 18:16:53.290329 pyserrf-0.1.0/pyserrf/read_data.py
--rwxr-xr-x   0        0        0      359 2024-05-06 09:54:41.577379 pyserrf-0.1.0/pyserrf/run.py
--rw-r--r--   0        0        0    27794 2024-05-06 13:20:54.494887 pyserrf-0.1.0/pyserrf/serrf.py
--rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 pyserrf-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      603 2024-05-04 16:40:19.958150 pyserrf-0.1.1/README.md
+-rw-r--r--   0        0        0      449 2024-05-06 13:59:26.971450 pyserrf-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       26 2024-04-26 15:26:59.997208 pyserrf-0.1.1/pyserrf/__init__.py
+-rw-r--r--   0        0        0     4293 2024-04-18 18:16:53.290329 pyserrf-0.1.1/pyserrf/read_data.py
+-rwxr-xr-x   0        0        0      359 2024-05-06 09:54:41.577379 pyserrf-0.1.1/pyserrf/run.py
+-rw-r--r--   0        0        0    27781 2024-05-06 13:58:04.081344 pyserrf-0.1.1/pyserrf/serrf.py
+-rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 pyserrf-0.1.1/PKG-INFO
```

### Comparing `pyserrf-0.1.0/README.md` & `pyserrf-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyserrf-0.1.0/pyserrf/read_data.py` & `pyserrf-0.1.1/pyserrf/read_data.py`

 * *Files identical despite different names*

### Comparing `pyserrf-0.1.0/pyserrf/serrf.py` & `pyserrf-0.1.1/pyserrf/serrf.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,17 @@
         new column names (MET_1, MET_2, etc.).
     corrs_qc : pandas DataFrame
         DataFrame with the Pearson correlation coefficients between the
         metabolites and the batch information.
     corrs_target : pandas DataFrame
         DataFrame with the Pearson correlation coefficients between the
         metabolites and the samples.
-    normalized_data_ : pandas DataFrame
+    normalized_data : pandas DataFrame
         DataFrame with the normalized data.
-    normalized_dataset_ : pandas DataFrame
+    normalized_dataset : pandas DataFrame
         DataFrame with the normalized data and the sample metadata.
 
     References
     ----------
     .. [1] Fan et al.:
         Systematic Error Removal using Random Forest (SERRF) for Normalizing
         Large-Scale Untargeted Lipidomics Data
@@ -142,17 +142,17 @@
         _sample_metadata : pandas DataFrame containing the sample metadata.
         corrs_qc : pandas DataFrame
             DataFrame with the Pearson correlation coefficients between the
             metabolites and the batch information.
         corrs_target : pandas DataFrame
             DataFrame with the Pearson correlation coefficients between the
             metabolites and the samples.
-        normalized_data_ : pandas DataFrame
+        normalized_data : pandas DataFrame
             DataFrame with the normalized data.
-        normalized_dataset_ : pandas DataFrame
+        normalized_dataset : pandas DataFrame
             DataFrame with the normalized data and the sample metadata.
         """
         # attributes for the preprocessing
         self.sample_metadata_columns = list(sample_metadata_columns)
         self.sample_type_column = sample_type_column
         self.batch_column = batch_column
         # attributes for the analysis
@@ -162,16 +162,16 @@
         # internal class attributes obtained from preprocessing
         self._metabolites = None
         self._dataset = None
         self._metabolite_dict = None
         self._sample_metadata = None
         self._corrs_qc = None
         self._corrs_target = None
-        self.normalized_data_ = None
-        self.normalized_dataset_ = None
+        self.normalized_data = None
+        self.normalized_dataset = None
         self.n_features_ = None
 
     def fit(self, X):
         """
         Fit the transformer on the data X and returns self.
 
         Parameters
@@ -286,25 +286,25 @@
         ) as p:
             normalized_metabolites = list(
                 tqdm(
                     p.imap(self._normalize_metabolite_parallel, self._metabolites),
                     total=len(self._metabolites),
                 )
             )
-        self.normalized_data_ = pd.concat(normalized_metabolites, axis=1)
-        self.normalized_data_.columns = [
-            self._metabolite_dict[i] for i in self.normalized_data_.columns
+        self.normalized_data = pd.concat(normalized_metabolites, axis=1)
+        self.normalized_data.columns = [
+            self._metabolite_dict[i] for i in self.normalized_data.columns
         ]
-        self.normalized_dataset_ = pd.concat(
-            [self._sample_metadata, self.normalized_data_], axis=1
+        self.normalized_dataset = pd.concat(
+            [self._sample_metadata, self.normalized_data], axis=1
         )
         if return_data_only:
-            X = self.normalized_data_
+            X = self.normalized_data
         else:
-            X = self.normalized_dataset_
+            X = self.normalized_dataset
         return X
 
     def _center_data(self, data: np.ndarray) -> np.ndarray:
         mean = np.nanmean(data)
         centered = data - mean
         return centered
```

### Comparing `pyserrf-0.1.0/PKG-INFO` & `pyserrf-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pyserrf
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python implementation of the Systematic Error Removal Using Random Forest algorithm
 Author: matteobolner
 Author-email: matteo.bolner2@unibo.it
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pytest (>=8.2.0,<9.0.0)
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
+Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Description-Content-Type: text/markdown
 
 # pySERRF
 Python implementation of the Systematic Error Removal Using Random Forest (SERRF) algorithm.
 SERRF is a qc-based sample normalization method designed for large-scale untargeted metabolomics data.
 The method was developed by the Fan et al. in 2015 (see https://slfan2013.github.io/SERRF-online/).
 This is simply an attempt to port its functionality from R to python.
```

