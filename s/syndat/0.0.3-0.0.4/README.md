# Comparing `tmp/syndat-0.0.3.tar.gz` & `tmp/syndat-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syndat-0.0.3.tar", last modified: Wed Apr 24 13:58:36 2024, max compression
+gzip compressed data, was "syndat-0.0.4.tar", last modified: Mon May  6 13:41:48 2024, max compression
```

## Comparing `syndat-0.0.3.tar` & `syndat-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:58:36.793765 syndat-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-24 13:58:28.000000 syndat-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-24 13:58:36.793765 syndat-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-24 13:58:28.000000 syndat-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:58:36.793765 syndat-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-24 13:58:34.000000 syndat-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:58:36.793765 syndat-0.0.3/syndat/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 13:58:28.000000 syndat-0.0.3/syndat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 13:58:28.000000 syndat-0.0.3/syndat/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-24 13:58:28.000000 syndat-0.0.3/syndat/quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-24 13:58:28.000000 syndat-0.0.3/syndat/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:58:36.793765 syndat-0.0.3/syndat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-24 13:58:36.000000 syndat-0.0.3/syndat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-24 13:58:36.000000 syndat-0.0.3/syndat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:58:36.000000 syndat-0.0.3/syndat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 13:58:36.000000 syndat-0.0.3/syndat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:58:36.793765 syndat-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-24 13:58:28.000000 syndat-0.0.3/tests/test_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-24 13:58:28.000000 syndat-0.0.3/tests/test_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-24 13:58:28.000000 syndat-0.0.3/tests/test_jsd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:41:48.673997 syndat-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-06 13:41:44.000000 syndat-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-06 13:41:48.673997 syndat-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-06 13:41:44.000000 syndat-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 13:41:48.673997 syndat-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-06 13:41:46.000000 syndat-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:41:48.673997 syndat-0.0.4/syndat/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-06 13:41:44.000000 syndat-0.0.4/syndat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-06 13:41:44.000000 syndat-0.0.4/syndat/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-06 13:41:44.000000 syndat-0.0.4/syndat/quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-06 13:41:44.000000 syndat-0.0.4/syndat/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:41:48.673997 syndat-0.0.4/syndat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-06 13:41:48.000000 syndat-0.0.4/syndat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-06 13:41:48.000000 syndat-0.0.4/syndat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:41:48.000000 syndat-0.0.4/syndat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 13:41:48.000000 syndat-0.0.4/syndat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:41:48.673997 syndat-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-06 13:41:44.000000 syndat-0.0.4/tests/test_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-06 13:41:44.000000 syndat-0.0.4/tests/test_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-06 13:41:44.000000 syndat-0.0.4/tests/test_jsd.py
```

### Comparing `syndat-0.0.3/LICENSE` & `syndat-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `syndat-0.0.3/README.md` & `syndat-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `syndat-0.0.3/setup.py` & `syndat-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 setup(
     name='syndat',
-    version='v0.0.3',
+    version='v0.0.4',
     packages=['syndat'],
     url='https://github.com/SCAI-BIO/syndat',
     license='CC BY-NC-ND 4.0.',
     author='Tim Adams',
     author_email='tim.adams@scai.fraunhofer.de',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
```

### Comparing `syndat-0.0.3/syndat/quality.py` & `syndat-0.0.4/syndat/quality.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,19 @@
     """
     # load datasets & remove id column
     jsd_dict = {}
     for col in real:
         # delete empty cells
         real_wo_missing = real[col].dropna()
         # binning
-        if np.sum(real[col].values) % 1 == 0 and np.sum(synthetic[col].values) % 1 == 0:
+        col_dtype_real = real[col].dtype
+        col_dtype_synthetic = synthetic[col].dtype
+        if col_dtype_real != col_dtype_synthetic:
+            raise TypeError(f'Real data at col {col} is dtype {col_dtype_real} but synthetic is {col_dtype_synthetic}.')
+        if col_dtype_real == "int64" or col_dtype_real == "object":
             # categorical column
             real_binned = np.bincount(real[col])
             virtual_binned = np.bincount(synthetic[col])
         else:
             # get optimal amount of bins
             n_bins = np.histogram_bin_edges(real_wo_missing, bins='auto')
             real_binned = np.bincount(np.digitize(real_wo_missing, n_bins))
```

### Comparing `syndat-0.0.3/syndat/visualization.py` & `syndat-0.0.4/syndat/visualization.py`

 * *Files identical despite different names*

### Comparing `syndat-0.0.3/tests/test_auc.py` & `syndat-0.0.4/tests/test_auc.py`

 * *Files identical despite different names*

### Comparing `syndat-0.0.3/tests/test_correlation.py` & `syndat-0.0.4/tests/test_correlation.py`

 * *Files identical despite different names*

### Comparing `syndat-0.0.3/tests/test_jsd.py` & `syndat-0.0.4/tests/test_jsd.py`

 * *Files identical despite different names*

