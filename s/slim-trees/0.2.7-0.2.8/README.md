# Comparing `tmp/slim_trees-0.2.7.tar.gz` & `tmp/slim_trees-0.2.8.tar.gz`

## Comparing `slim_trees-0.2.7.tar` & `slim_trees-0.2.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 slim_trees-0.2.7/slim_trees/__init__.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 slim_trees-0.2.7/slim_trees/compression_utils.py
--rw-r--r--   0        0        0     9792 2020-02-02 00:00:00.000000 slim_trees-0.2.7/slim_trees/lgbm_booster.py
--rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 slim_trees-0.2.7/slim_trees/pickling.py
--rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 slim_trees-0.2.7/slim_trees/sklearn_tree.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 slim_trees-0.2.7/slim_trees/utils.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 slim_trees-0.2.7/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 slim_trees-0.2.7/LICENSE
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 slim_trees-0.2.7/README.md
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 slim_trees-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 slim_trees-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 slim_trees-0.2.8/slim_trees/__init__.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 slim_trees-0.2.8/slim_trees/compression_utils.py
+-rw-r--r--   0        0        0     9792 2020-02-02 00:00:00.000000 slim_trees-0.2.8/slim_trees/lgbm_booster.py
+-rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 slim_trees-0.2.8/slim_trees/pickling.py
+-rw-r--r--   0        0        0     6872 2020-02-02 00:00:00.000000 slim_trees-0.2.8/slim_trees/sklearn_tree.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 slim_trees-0.2.8/slim_trees/utils.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 slim_trees-0.2.8/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 slim_trees-0.2.8/LICENSE
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 slim_trees-0.2.8/README.md
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 slim_trees-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 slim_trees-0.2.8/PKG-INFO
```

### Comparing `slim_trees-0.2.7/slim_trees/__init__.py` & `slim_trees-0.2.8/slim_trees/__init__.py`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.7/slim_trees/compression_utils.py` & `slim_trees-0.2.8/slim_trees/compression_utils.py`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.7/slim_trees/lgbm_booster.py` & `slim_trees-0.2.8/slim_trees/lgbm_booster.py`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.7/slim_trees/pickling.py` & `slim_trees-0.2.8/slim_trees/pickling.py`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.7/slim_trees/sklearn_tree.py` & `slim_trees-0.2.8/slim_trees/sklearn_tree.py`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.7/.gitignore` & `slim_trees-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.7/LICENSE` & `slim_trees-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `slim_trees-0.2.7/README.md` & `slim_trees-0.2.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -114,31 +114,20 @@
 You can install the package in development mode using the new conda package manager [`pixi`](https://github.com/prefix-dev/pixi):
 
 ```bash
 ❯ git clone https://github.com/quantco/slim-trees.git
 ❯ cd slim-trees
 
 ❯ pixi install
-❯ pixi run pre-commit install
-❯ pixi run pip install --no-deps --disable-pip-version-check --no-build-isolation -e .
-❯ pixi run python
->>> import slim_trees
-[...]
+❯ pixi run postinstall
 ❯ pixi run test
 [...]
-```
-
-Alternatively, you can use `micromamba` (or `mamba` or `conda`):
-
-```bash
-❯ micromamba create -f environment.yml
-❯ micromamba activate slim_trees
-
-❯ pre-commit install
-❯ pip install --no-build-isolation -e .
+❯ pixi run py312 python
+>>> import slim_trees
+[...]
 ```
 
 ## Benchmark
 
 As a general overview on what you can expect in terms of savings:
 This is a 1.2G large sklearn `RandomForestRegressor`.
```

### Comparing `slim_trees-0.2.7/pyproject.toml` & `slim_trees-0.2.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "slim-trees"
 description = "A python package for efficient pickling of ML models."
-version = "0.2.7"
+version = "0.2.8"
 readme = "README.md"
-license = "MIT"
+license = {file = "LICENSE"}
 requires-python = ">=3.8"
 authors = [
     { name = "Pavel Zwerschke", email = "pavel.zwerschke@quantco.com" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
@@ -25,29 +25,30 @@
 ]
 
 [project.optional-dependencies]
 lightgbm = [
     "lightgbm >=3.2,<4.4",
 ]
 scikit-learn = [
-    "scikit-learn >=1.1.0,<1.4",
+    "scikit-learn >=1.1.0,<1.5",
 ]
 
 [project.urls]
 Homepage = "https://github.com/quantco/slim-trees"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "/slim_trees",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py38"
 
+[tool.ruff.lint]
 select = [
     # pyflakes
     "F",
     # pycodestyle
     "E", "W",
     # flake8-builtins
     "A",
```

### Comparing `slim_trees-0.2.7/PKG-INFO` & `slim_trees-0.2.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,47 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: slim-trees
-Version: 0.2.7
+Version: 0.2.8
 Summary: A python package for efficient pickling of ML models.
 Project-URL: Homepage, https://github.com/quantco/slim-trees
 Author-email: Pavel Zwerschke <pavel.zwerschke@quantco.com>
-License-Expression: MIT
+License: MIT License
+        
+        Copyright (c) 2023 Pavel Zwerschke, Yasin Tatar and Jonas Haag
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: numpy
 Provides-Extra: lightgbm
 Requires-Dist: lightgbm<4.4,>=3.2; extra == 'lightgbm'
 Provides-Extra: scikit-learn
-Requires-Dist: scikit-learn<1.4,>=1.1.0; extra == 'scikit-learn'
+Requires-Dist: scikit-learn<1.5,>=1.1.0; extra == 'scikit-learn'
 Description-Content-Type: text/markdown
 
 # Slim Trees
 
 [![CI](https://github.com/quantco/slim-trees/actions/workflows/ci.yml/badge.svg)](https://github.com/quantco/slim-trees/actions/workflows/ci.yml)
 [![conda-forge](https://img.shields.io/conda/vn/conda-forge/slim-trees?logoColor=white&logo=conda-forge)](https://anaconda.org/conda-forge/slim-trees)
 [![pypi-version](https://img.shields.io/pypi/v/slim-trees.svg?logo=pypi&logoColor=white)](https://pypi.org/project/slim-trees)
@@ -136,31 +156,20 @@
 You can install the package in development mode using the new conda package manager [`pixi`](https://github.com/prefix-dev/pixi):
 
 ```bash
 ❯ git clone https://github.com/quantco/slim-trees.git
 ❯ cd slim-trees
 
 ❯ pixi install
-❯ pixi run pre-commit install
-❯ pixi run pip install --no-deps --disable-pip-version-check --no-build-isolation -e .
-❯ pixi run python
->>> import slim_trees
-[...]
+❯ pixi run postinstall
 ❯ pixi run test
 [...]
-```
-
-Alternatively, you can use `micromamba` (or `mamba` or `conda`):
-
-```bash
-❯ micromamba create -f environment.yml
-❯ micromamba activate slim_trees
-
-❯ pre-commit install
-❯ pip install --no-build-isolation -e .
+❯ pixi run py312 python
+>>> import slim_trees
+[...]
 ```
 
 ## Benchmark
 
 As a general overview on what you can expect in terms of savings:
 This is a 1.2G large sklearn `RandomForestRegressor`.
```

