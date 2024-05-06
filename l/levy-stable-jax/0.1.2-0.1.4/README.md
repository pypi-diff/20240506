# Comparing `tmp/levy_stable_jax-0.1.2.tar.gz` & `tmp/levy_stable_jax-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "levy_stable_jax-0.1.2.tar", max compression
+gzip compressed data, was "levy_stable_jax-0.1.4.tar", max compression
```

## Comparing `levy_stable_jax-0.1.2.tar` & `levy_stable_jax-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-10-22 07:47:03.747679 levy_stable_jax-0.1.2/LICENSE
--rw-r--r--   0        0        0     1259 2024-05-03 14:16:08.822396 levy_stable_jax-0.1.2/README.md
--rw-r--r--   0        0        0     2608 2024-05-03 14:18:49.454450 levy_stable_jax-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      336 2024-05-03 13:29:34.962247 levy_stable_jax-0.1.2/src/levy_stable_jax/__init__.py
--rw-r--r--   0        0        0      708 2024-04-24 12:12:58.006634 levy_stable_jax-0.1.2/src/levy_stable_jax/_cache.py
--rw-r--r--   0        0        0     4270 2024-05-03 11:58:27.607858 levy_stable_jax-0.1.2/src/levy_stable_jax/_generate_data.py
--rw-r--r--   0        0        0      975 2024-05-03 13:51:24.346392 levy_stable_jax-0.1.2/src/levy_stable_jax/_interp.py
--rw-r--r--   0        0        0      559 2024-05-03 13:29:34.962247 levy_stable_jax-0.1.2/src/levy_stable_jax/_typing.py
--rw-r--r--   0        0        0     7742 2024-05-03 13:50:38.658201 levy_stable_jax-0.1.2/src/levy_stable_jax/_utils.py
--rw-r--r--   0        0        0    12470 2024-05-03 13:43:26.840236 levy_stable_jax-0.1.2/src/levy_stable_jax/distribution.py
--rw-r--r--   0        0        0     4556 2024-05-03 13:29:34.966248 levy_stable_jax-0.1.2/src/levy_stable_jax/estimation.py
--rw-r--r--   0        0        0  6464128 2024-05-03 13:29:34.994248 levy_stable_jax-0.1.2/src/levy_stable_jax/logpdf.npy
--rw-r--r--   0        0        0     6069 2024-05-03 13:31:25.623373 levy_stable_jax-0.1.2/src/levy_stable_jax/pymc.py
--rw-r--r--   0        0        0     2137 1970-01-01 00:00:00.000000 levy_stable_jax-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-06 07:08:26.556737 levy_stable_jax-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1259 2024-05-06 07:08:26.556737 levy_stable_jax-0.1.4/README.md
+-rw-r--r--   0        0        0     2994 2024-05-06 19:04:42.206410 levy_stable_jax-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      336 2024-05-06 07:08:26.576737 levy_stable_jax-0.1.4/src/levy_stable_jax/__init__.py
+-rw-r--r--   0        0        0      708 2024-05-06 07:08:26.576737 levy_stable_jax-0.1.4/src/levy_stable_jax/_cache.py
+-rw-r--r--   0        0        0     4270 2024-05-06 07:08:26.576737 levy_stable_jax-0.1.4/src/levy_stable_jax/_generate_data.py
+-rw-r--r--   0        0        0      975 2024-05-06 07:08:26.576737 levy_stable_jax-0.1.4/src/levy_stable_jax/_interp.py
+-rw-r--r--   0        0        0      559 2024-05-06 07:08:26.576737 levy_stable_jax-0.1.4/src/levy_stable_jax/_typing.py
+-rw-r--r--   0        0        0     7742 2024-05-06 07:08:26.576737 levy_stable_jax-0.1.4/src/levy_stable_jax/_utils.py
+-rw-r--r--   0        0        0    12470 2024-05-06 07:08:26.576737 levy_stable_jax-0.1.4/src/levy_stable_jax/distribution.py
+-rw-r--r--   0        0        0     4556 2024-05-06 07:08:26.580737 levy_stable_jax-0.1.4/src/levy_stable_jax/estimation.py
+-rw-r--r--   0        0        0  6464128 2024-05-06 07:08:26.628737 levy_stable_jax-0.1.4/src/levy_stable_jax/logpdf.npy
+-rw-r--r--   0        0        0     6194 2024-05-06 19:03:37.395619 levy_stable_jax-0.1.4/src/levy_stable_jax/pymc.py
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 levy_stable_jax-0.1.4/PKG-INFO
```

### Comparing `levy_stable_jax-0.1.2/LICENSE` & `levy_stable_jax-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1.2/README.md` & `levy_stable_jax-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1.2/pyproject.toml` & `levy_stable_jax-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [project]
 name = "levy-stable-jax"
-version = "0.1.2"
+version = "0.1.4"
 authors = [
     {name = "Tim Hunter", email = "tjhunter@cs.stanford.edu"},
 ]
 license = { text = "Apache 2 License" }
 description = "Implementation of the Lévy stable distributions for Jax."
 readme = "README.md"
 requires-python = ">=3.9"
@@ -20,71 +20,89 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "jax>=0.3",
-    "jaxopt>=0.8",
     "numpy>=1.19",
     "scipy>=1.5",    
 ]
 
+
+[project.optional-dependencies]
+pymc = [
+    "pymc>=5.13",
+    "numpyro>=0.14"
+]
+inference = [
+    "jaxopt>=0.8"
+]
+
 [project.urls]
 Homepage = "https://github.com/tjhunter/levy-stable-jax"
 Documentation = "https://github.com/tjhunter/levy-stable-jax"
 Repository = "https://github.com/tjhunter/levy-stable-jax"
 
 [tool.poetry]
 packages = [{include = "levy_stable_jax", from="src"}]
 name = "levy-stable-jax"
-version = "0.1.2"
+version = "0.1.4"
 authors = ["Tim Hunter <tjhunter@cs.stanford.edu>"]
 description = "Implementation of the Lévy alpha-stable distributions for Jax."
 readme = "README.md"
 license = "Apache 2.0"
 homepage = "https://github.com/tjhunter/levy-stable-jax"
-documentation = "https://github.com/tjhunter/levy-stable-jax"
+documentation = "https://levy-stable-jax.readthedocs.io/en/latest/"
 repository = "https://github.com/tjhunter/levy-stable-jax"
 keywords = ["levy", "stable", "jax", "probability", "statistics"]
 
+# The core dependencies
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 jax = "^0.4"
+jaxlib = "^0.4.26"
 numpy = "^1.19" 
 scipy = "^1.5"
+pymc = {version="^5.13.1", optional=true}
+numpyro = {version="^0.14.0", optional=true}
+jaxopt = {version="^0.8", optional=true}
+
+[tool.poetry.extras]
+pymc = ["pymc", "numpyro"]
+inference = ["jaxopt"]
 
-# For inference
-# jaxopt = "^0.8"
-
-# For MCMC
+[tool.poetry.group.docs]
+optional = true
 
+[tool.poetry.group.docs.dependencies]
+mkdocs = "^1.6.0"
+sphinx = "^7.3.7"
+sphinx-rtd-theme = "^2.0.0"
+mkdocs-material = "^9.5.19"
+mkdocstrings = {extras = ["python"], version = "^0.24.3"}
+pytkdocs = {version = "^0.16.1", extras = ["numpy-style"]}
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.4.0"
 mypy = "^1.9.0"
 ruff = "^0.4.1"
-mkdocs = "^1.6.0"
 hypothesis = "^6.100.1"
-jaxopt = "^0.8.3"
 pytest = "^8.1.1"
 absl-py = "^2.1.0"
 scikit-learn = "^1.4.2"
 # Interactive sessions
 jupyter = "^1.0.0"
 seaborn = "^0.13.2"
-pymc = "^5.13.1"
-numpyro = "^0.14.0"
-sphinx = "^7.3.7"
-sphinx-rtd-theme = "^2.0.0"
-mkdocs-material = "^9.5.19"
-mkdocstrings = {extras = ["python"], version = "^0.24.3"}
-pytkdocs = {version = "^0.16.1", extras = ["numpy-style"]}
 
 
+
+[tool.poetry.group.pymc.dependencies]
+pytensor = "^2.20.0"
+
 [tool.pytest.ini_options]
 #addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 95"
 minversion = "7.0"
 testpaths = [
     "tests",
 ]
 pythonpath = [
```

### Comparing `levy_stable_jax-0.1.2/src/levy_stable_jax/_cache.py` & `levy_stable_jax-0.1.4/src/levy_stable_jax/_cache.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1.2/src/levy_stable_jax/_generate_data.py` & `levy_stable_jax-0.1.4/src/levy_stable_jax/_generate_data.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1.2/src/levy_stable_jax/_interp.py` & `levy_stable_jax-0.1.4/src/levy_stable_jax/_interp.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1.2/src/levy_stable_jax/_typing.py` & `levy_stable_jax-0.1.4/src/levy_stable_jax/_typing.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1.2/src/levy_stable_jax/_utils.py` & `levy_stable_jax-0.1.4/src/levy_stable_jax/_utils.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1.2/src/levy_stable_jax/distribution.py` & `levy_stable_jax-0.1.4/src/levy_stable_jax/distribution.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1.2/src/levy_stable_jax/estimation.py` & `levy_stable_jax-0.1.4/src/levy_stable_jax/estimation.py`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1.2/src/levy_stable_jax/logpdf.npy` & `levy_stable_jax-0.1.4/src/levy_stable_jax/logpdf.npy`

 * *Files identical despite different names*

### Comparing `levy_stable_jax-0.1.2/src/levy_stable_jax/pymc.py` & `levy_stable_jax-0.1.4/src/levy_stable_jax/pymc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 """
 Monte Carlo sampling of Levy-stable distributions using PyMC.
 
 As far as users are concerned, the only relevant function should be `LevyStableN0`.
+
+A full example notebook is available here:
+https://github.com/tjhunter/levy-stable-jax/blob/main/notebooks/pymc_levy.ipynb
+
 """
 
 # The source of most of this code are the following tutorials:
 # https://www.pymc-labs.com/blog-posts/jax-functions-in-pymc-3-quick-examples/
 # https://www.pymc.io/projects/examples/en/2022.12.0/howto/custom_distribution.html
```

### Comparing `levy_stable_jax-0.1.2/PKG-INFO` & `levy_stable_jax-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: levy-stable-jax
-Version: 0.1.2
+Version: 0.1.4
 Summary: Implementation of the Lévy alpha-stable distributions for Jax.
 Home-page: https://github.com/tjhunter/levy-stable-jax
 License: Apache 2.0
 Keywords: levy,stable,jax,probability,statistics
 Author: Tim Hunter
 Author-email: tjhunter@cs.stanford.edu
 Requires-Python: >=3.10,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: inference
+Provides-Extra: pymc
 Requires-Dist: jax (>=0.4,<0.5)
+Requires-Dist: jaxlib (>=0.4.26,<0.5.0)
+Requires-Dist: jaxopt (>=0.8,<0.9) ; extra == "inference"
 Requires-Dist: numpy (>=1.19,<2.0)
+Requires-Dist: numpyro (>=0.14.0,<0.15.0) ; extra == "pymc"
+Requires-Dist: pymc (>=5.13.1,<6.0.0) ; extra == "pymc"
 Requires-Dist: scipy (>=1.5,<2.0)
-Project-URL: Documentation, https://github.com/tjhunter/levy-stable-jax
+Project-URL: Documentation, https://levy-stable-jax.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/tjhunter/levy-stable-jax
 Description-Content-Type: text/markdown
 
 # Levy-stable-jax
 
 Implementation of the Lévy-stable distributions for the Jax framework.
```

