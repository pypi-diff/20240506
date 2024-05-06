# Comparing `tmp/dualbounds-1.0.0.tar.gz` & `tmp/dualbounds-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dualbounds-1.0.0.tar", last modified: Fri May  3 18:48:55 2024, max compression
+gzip compressed data, was "dualbounds-1.0.1.tar", last modified: Mon May  6 14:31:52 2024, max compression
```

## Comparing `dualbounds-1.0.0.tar` & `dualbounds-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:48:55.466821 dualbounds-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     3327 2024-05-03 18:48:55.466821 dualbounds-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2371 2024-01-11 14:24:27.000000 dualbounds-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:48:55.465821 dualbounds-1.0.0/dualbounds/
--rw-r--r--   0 root         (0) root         (0)      137 2024-04-30 02:35:02.000000 dualbounds-1.0.0/dualbounds/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3995 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     5094 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/delta.py
--rw-r--r--   0 root         (0) root         (0)    24096 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/dist_reg.py
--rw-r--r--   0 root         (0) root         (0)     5951 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/gen_data.py
--rw-r--r--   0 root         (0) root         (0)    34162 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/generic.py
--rw-r--r--   0 root         (0) root         (0)     2631 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/interpolation.py
--rw-r--r--   0 root         (0) root         (0)    23650 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/lee.py
--rw-r--r--   0 root         (0) root         (0)    13631 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/utilities.py
--rw-r--r--   0 root         (0) root         (0)     3585 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/varcate.py
--rw-r--r--   0 root         (0) root         (0)     3249 2024-05-03 18:46:42.000000 dualbounds-1.0.0/dualbounds/varite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:48:55.465821 dualbounds-1.0.0/dualbounds.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3327 2024-05-03 18:48:55.000000 dualbounds-1.0.0/dualbounds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      632 2024-05-03 18:48:55.000000 dualbounds-1.0.0/dualbounds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 18:48:55.000000 dualbounds-1.0.0/dualbounds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-05-03 18:48:55.000000 dualbounds-1.0.0/dualbounds.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-03 18:48:55.000000 dualbounds-1.0.0/dualbounds.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 18:48:55.466821 dualbounds-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1339 2024-04-30 02:35:02.000000 dualbounds-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:48:55.466821 dualbounds-1.0.0/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-21 06:09:47.000000 dualbounds-1.0.0/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-12-22 19:17:19.000000 dualbounds-1.0.0/test/context.py
--rw-r--r--   0 root         (0) root         (0)     2188 2024-05-03 18:46:42.000000 dualbounds-1.0.0/test/test_bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     3046 2024-05-03 18:46:42.000000 dualbounds-1.0.0/test/test_delta.py
--rw-r--r--   0 root         (0) root         (0)     3886 2024-02-26 00:25:26.000000 dualbounds-1.0.0/test/test_dist_reg.py
--rw-r--r--   0 root         (0) root         (0)    10928 2024-05-03 18:46:42.000000 dualbounds-1.0.0/test/test_generic.py
--rw-r--r--   0 root         (0) root         (0)     1092 2024-02-26 00:25:26.000000 dualbounds-1.0.0/test/test_interp.py
--rw-r--r--   0 root         (0) root         (0)    13179 2024-05-03 18:46:42.000000 dualbounds-1.0.0/test/test_lee.py
--rw-r--r--   0 root         (0) root         (0)     3552 2024-02-26 00:25:26.000000 dualbounds-1.0.0/test/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     4188 2024-05-03 18:46:42.000000 dualbounds-1.0.0/test/test_varbounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:31:52.483528 dualbounds-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)     3331 2024-05-06 14:31:52.482527 dualbounds-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2375 2024-05-03 18:50:13.000000 dualbounds-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:31:52.479527 dualbounds-1.0.1/dualbounds/
+-rw-r--r--   0 root         (0) root         (0)      137 2024-05-06 14:28:58.000000 dualbounds-1.0.1/dualbounds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3995 2024-05-03 18:46:42.000000 dualbounds-1.0.1/dualbounds/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     5094 2024-05-03 18:46:42.000000 dualbounds-1.0.1/dualbounds/delta.py
+-rw-r--r--   0 root         (0) root         (0)    24096 2024-05-03 18:46:42.000000 dualbounds-1.0.1/dualbounds/dist_reg.py
+-rw-r--r--   0 root         (0) root         (0)     5951 2024-05-06 14:28:56.000000 dualbounds-1.0.1/dualbounds/gen_data.py
+-rw-r--r--   0 root         (0) root         (0)    34162 2024-05-06 14:28:56.000000 dualbounds-1.0.1/dualbounds/generic.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2024-05-03 18:46:42.000000 dualbounds-1.0.1/dualbounds/interpolation.py
+-rw-r--r--   0 root         (0) root         (0)    23692 2024-05-06 14:28:58.000000 dualbounds-1.0.1/dualbounds/lee.py
+-rw-r--r--   0 root         (0) root         (0)    13631 2024-05-03 18:46:42.000000 dualbounds-1.0.1/dualbounds/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     3585 2024-05-03 18:46:42.000000 dualbounds-1.0.1/dualbounds/varcate.py
+-rw-r--r--   0 root         (0) root         (0)     3249 2024-05-03 18:46:42.000000 dualbounds-1.0.1/dualbounds/varite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:31:52.480527 dualbounds-1.0.1/dualbounds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3331 2024-05-06 14:31:52.000000 dualbounds-1.0.1/dualbounds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      632 2024-05-06 14:31:52.000000 dualbounds-1.0.1/dualbounds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 14:31:52.000000 dualbounds-1.0.1/dualbounds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-06 14:31:52.000000 dualbounds-1.0.1/dualbounds.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-06 14:31:52.000000 dualbounds-1.0.1/dualbounds.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 14:31:52.483528 dualbounds-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1339 2024-04-30 02:35:02.000000 dualbounds-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 14:31:52.482527 dualbounds-1.0.1/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-21 06:09:47.000000 dualbounds-1.0.1/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-12-22 19:17:19.000000 dualbounds-1.0.1/test/context.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2024-05-03 18:46:42.000000 dualbounds-1.0.1/test/test_bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     3046 2024-05-03 18:46:42.000000 dualbounds-1.0.1/test/test_delta.py
+-rw-r--r--   0 root         (0) root         (0)     3886 2024-02-26 00:25:26.000000 dualbounds-1.0.1/test/test_dist_reg.py
+-rw-r--r--   0 root         (0) root         (0)    10928 2024-05-04 18:33:47.000000 dualbounds-1.0.1/test/test_generic.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2024-02-26 00:25:26.000000 dualbounds-1.0.1/test/test_interp.py
+-rw-r--r--   0 root         (0) root         (0)    13179 2024-05-03 18:46:42.000000 dualbounds-1.0.1/test/test_lee.py
+-rw-r--r--   0 root         (0) root         (0)     3552 2024-02-26 00:25:26.000000 dualbounds-1.0.1/test/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2024-05-03 18:46:42.000000 dualbounds-1.0.1/test/test_varbounds.py
```

### Comparing `dualbounds-1.0.0/PKG-INFO` & `dualbounds-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: dualbounds
-Version: 1.0.0
+Version: 1.0.1
 Summary: Dual bounds for model-agnostic inference
 Home-page: https://github.com/amspector100/dualbounds/
 Author: Asher Spector
 Author-email: amspector100@gmail.com
 License: UNKNOWN
-Description: A python implementation of the dual bounds framework for inference on partially identified estimands (and the solutions to optimization problems more generally). See https://amspector100.github.io/dualbounds/ for detailed documentation and tutorials.
+Description: A python implementation of the dual bounds framework for inference on partially identified estimands (and the solutions to optimization problems more generally). See https://dualbounds.readthedocs.io/en/latest/ for detailed documentation and tutorials.
         
         ## Installation
         
         To install ``dualbounds``, just use pip:
         
         ``pip install dualbounds``
         
         ## Documentation
         
-        Documentation and tutorials are available at https://amspector100.github.io/dualbounds/.
+        Documentation and tutorials are available at https://dualbounds.readthedocs.io/en/latest/.
         
         ## Quickstart
         
         Given a response vector ``y``, binary treatment vector ``W``, covariate matrix ``X``, and an (optional) propensity score vector ``pis``, dualbounds allows analysts to perform inference on partially identified estimands of the form E[f(Y(0), Y(1), X)], for any choice of f. For example, the code below shows how to perform inference in P(Y(0) < Y(1)), the proportion of individuals who benefit from the treatment. Dual bounds can wrap on top of *any* machine learning model to provide provably valid confidence intervals in randomized experiments.
         
         ```
         	import dualbounds as db
```

### Comparing `dualbounds-1.0.0/README.md` & `dualbounds-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-A python implementation of the dual bounds framework for inference on partially identified estimands (and the solutions to optimization problems more generally). See https://amspector100.github.io/dualbounds/ for detailed documentation and tutorials.
+A python implementation of the dual bounds framework for inference on partially identified estimands (and the solutions to optimization problems more generally). See https://dualbounds.readthedocs.io/en/latest/ for detailed documentation and tutorials.
 
 ## Installation
 
 To install ``dualbounds``, just use pip:
 
 ``pip install dualbounds``
 
 ## Documentation
 
-Documentation and tutorials are available at https://amspector100.github.io/dualbounds/.
+Documentation and tutorials are available at https://dualbounds.readthedocs.io/en/latest/.
 
 ## Quickstart
 
 Given a response vector ``y``, binary treatment vector ``W``, covariate matrix ``X``, and an (optional) propensity score vector ``pis``, dualbounds allows analysts to perform inference on partially identified estimands of the form E[f(Y(0), Y(1), X)], for any choice of f. For example, the code below shows how to perform inference in P(Y(0) < Y(1)), the proportion of individuals who benefit from the treatment. Dual bounds can wrap on top of *any* machine learning model to provide provably valid confidence intervals in randomized experiments.
 
 ```
 	import dualbounds as db
```

### Comparing `dualbounds-1.0.0/dualbounds/bootstrap.py` & `dualbounds-1.0.1/dualbounds/bootstrap.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/dualbounds/delta.py` & `dualbounds-1.0.1/dualbounds/delta.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/dualbounds/dist_reg.py` & `dualbounds-1.0.1/dualbounds/dist_reg.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/dualbounds/gen_data.py` & `dualbounds-1.0.1/dualbounds/gen_data.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/dualbounds/generic.py` & `dualbounds-1.0.1/dualbounds/generic.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/dualbounds/interpolation.py` & `dualbounds-1.0.1/dualbounds/interpolation.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/dualbounds/lee.py` & `dualbounds-1.0.1/dualbounds/lee.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,20 +174,20 @@
 
 		- estimates: 2-length array of lower/upper estimates.
 		- ses: 2-length array of lower/upper standard errors.
 		- cis: 2-length array of lower/upper confidence intervals.
 	"""
 	# Rename for simplicity
 	y = outcome
+	n = len(y)
 	W = treatment
 	S = selections
 	pis = propensities
 	if pis is None:
 		pis = np.ones(n) * treatment.mean()
-	n = len(W)
 
 	# compute P(S | W)
 	s0_prob = np.array([np.mean(S[W == 0])])
 	s1_prob = np.array([np.mean(S[W == 1])])
 	s1_prob = np.maximum(s0_prob, s1_prob)
 
 	# compute P(Y(0))
@@ -216,15 +216,19 @@
 	# compute lower, upper bounds
 	ests = compute_analytical_lee_bound(**args)[1][:, 0]
 	if B > 0:
 		bs_ests = np.zeros((B, 2))
 		for b in range(B):
 			inds = np.random.choice(n, n, replace=True)
 			bs_ests[b] = lee_bound_no_covariates(
-				treatment=W[inds], selections=S[inds], outcome=y[inds], B=0
+				treatment=W[inds], 
+				selections=S[inds],
+				outcome=y[inds],
+				propensities=pis[inds],
+				B=0,
 			)['estimates']
 		bias = bs_ests.mean(axis=0) - ests
 		ses = bs_ests.std(axis=0)
 		cis = ests - bias
 		cis[0] -= stats.norm.ppf(1-alpha/2) * ses[0]
 		cis[1] += stats.norm.ppf(1-alpha/2) * ses[1]
 		return dict(
```

### Comparing `dualbounds-1.0.0/dualbounds/utilities.py` & `dualbounds-1.0.1/dualbounds/utilities.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/dualbounds/varcate.py` & `dualbounds-1.0.1/dualbounds/varcate.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/dualbounds/varite.py` & `dualbounds-1.0.1/dualbounds/varite.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/dualbounds.egg-info/PKG-INFO` & `dualbounds-1.0.1/dualbounds.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: dualbounds
-Version: 1.0.0
+Version: 1.0.1
 Summary: Dual bounds for model-agnostic inference
 Home-page: https://github.com/amspector100/dualbounds/
 Author: Asher Spector
 Author-email: amspector100@gmail.com
 License: UNKNOWN
-Description: A python implementation of the dual bounds framework for inference on partially identified estimands (and the solutions to optimization problems more generally). See https://amspector100.github.io/dualbounds/ for detailed documentation and tutorials.
+Description: A python implementation of the dual bounds framework for inference on partially identified estimands (and the solutions to optimization problems more generally). See https://dualbounds.readthedocs.io/en/latest/ for detailed documentation and tutorials.
         
         ## Installation
         
         To install ``dualbounds``, just use pip:
         
         ``pip install dualbounds``
         
         ## Documentation
         
-        Documentation and tutorials are available at https://amspector100.github.io/dualbounds/.
+        Documentation and tutorials are available at https://dualbounds.readthedocs.io/en/latest/.
         
         ## Quickstart
         
         Given a response vector ``y``, binary treatment vector ``W``, covariate matrix ``X``, and an (optional) propensity score vector ``pis``, dualbounds allows analysts to perform inference on partially identified estimands of the form E[f(Y(0), Y(1), X)], for any choice of f. For example, the code below shows how to perform inference in P(Y(0) < Y(1)), the proportion of individuals who benefit from the treatment. Dual bounds can wrap on top of *any* machine learning model to provide provably valid confidence intervals in randomized experiments.
         
         ```
         	import dualbounds as db
```

### Comparing `dualbounds-1.0.0/dualbounds.egg-info/SOURCES.txt` & `dualbounds-1.0.1/dualbounds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/setup.py` & `dualbounds-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/test/context.py` & `dualbounds-1.0.1/test/context.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/test/test_bootstrap.py` & `dualbounds-1.0.1/test/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/test/test_delta.py` & `dualbounds-1.0.1/test/test_delta.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/test/test_dist_reg.py` & `dualbounds-1.0.1/test/test_dist_reg.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/test/test_generic.py` & `dualbounds-1.0.1/test/test_generic.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/test/test_interp.py` & `dualbounds-1.0.1/test/test_interp.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/test/test_lee.py` & `dualbounds-1.0.1/test/test_lee.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/test/test_utils.py` & `dualbounds-1.0.1/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `dualbounds-1.0.0/test/test_varbounds.py` & `dualbounds-1.0.1/test/test_varbounds.py`

 * *Files identical despite different names*

