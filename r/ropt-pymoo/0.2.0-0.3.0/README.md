# Comparing `tmp/ropt_pymoo-0.2.0.tar.gz` & `tmp/ropt_pymoo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ropt_pymoo-0.2.0.tar", last modified: Mon Apr 29 12:25:57 2024, max compression
+gzip compressed data, was "ropt_pymoo-0.3.0.tar", last modified: Mon May  6 15:28:40 2024, max compression
```

## Comparing `ropt_pymoo-0.2.0.tar` & `ropt_pymoo-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:57.961099 ropt_pymoo-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:57.957099 ropt_pymoo-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:57.957099 ropt_pymoo-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/.github/workflows/static-checks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-29 12:25:57.961099 ropt_pymoo-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:57.957099 ropt_pymoo-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/examples/discrete_ga.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/examples/discrete_ga.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/examples/rosenbrock_cmaes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:25:57.961099 ropt_pymoo-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:57.957099 ropt_pymoo-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:57.961099 ropt_pymoo-0.2.0/src/ropt_pymoo/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/src/ropt_pymoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8641 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/src/ropt_pymoo/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/src/ropt_pymoo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/src/ropt_pymoo/pymoo.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 12:25:57.000000 ropt_pymoo-0.2.0/src/ropt_pymoo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:57.961099 ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-29 12:25:57.000000 ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-29 12:25:57.000000 ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:25:57.000000 ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-29 12:25:57.000000 ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 12:25:57.000000 ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 12:25:57.000000 ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:57.961099 ropt_pymoo-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/tests/test_pymoo_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:40.171637 ropt_pymoo-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:40.163637 ropt_pymoo-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:40.163637 ropt_pymoo-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/.github/workflows/static-checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-06 15:28:40.167637 ropt_pymoo-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:40.163637 ropt_pymoo-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/examples/discrete_ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/examples/discrete_ga.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/examples/rosenbrock_nm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:28:40.171637 ropt_pymoo-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:40.163637 ropt_pymoo-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:40.167637 ropt_pymoo-0.3.0/src/ropt_pymoo/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/src/ropt_pymoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/src/ropt_pymoo/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/src/ropt_pymoo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/src/ropt_pymoo/pymoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 15:28:40.000000 ropt_pymoo-0.3.0/src/ropt_pymoo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:40.167637 ropt_pymoo-0.3.0/src/ropt_pymoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-06 15:28:40.000000 ropt_pymoo-0.3.0/src/ropt_pymoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-06 15:28:40.000000 ropt_pymoo-0.3.0/src/ropt_pymoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:28:40.000000 ropt_pymoo-0.3.0/src/ropt_pymoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-06 15:28:40.000000 ropt_pymoo-0.3.0/src/ropt_pymoo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-06 15:28:40.000000 ropt_pymoo-0.3.0/src/ropt_pymoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 15:28:40.000000 ropt_pymoo-0.3.0/src/ropt_pymoo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:40.167637 ropt_pymoo-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13506 2024-05-06 15:28:33.000000 ropt_pymoo-0.3.0/tests/test_pymoo_backend.py
```

### Comparing `ropt_pymoo-0.2.0/.github/workflows/release.yml` & `ropt_pymoo-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ropt_pymoo-0.2.0/.github/workflows/static-checks.yml` & `ropt_pymoo-0.3.0/.github/workflows/static-checks.yml`

 * *Files identical despite different names*

### Comparing `ropt_pymoo-0.2.0/.github/workflows/tests.yml` & `ropt_pymoo-0.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ropt_pymoo-0.2.0/LICENSE` & `ropt_pymoo-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ropt_pymoo-0.2.0/PKG-INFO` & `ropt_pymoo-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ropt-pymoo
-Version: 0.2.0
-Summary: A pymoo backend for the ropt robust optimization library
+Version: 0.3.0
+Summary: A pymoo plugin for the ropt robust optimization library
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,15 +14,15 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pymoo
 Requires-Dist: pydantic
-Requires-Dist: ropt>=0.2.1
+Requires-Dist: ropt>=0.3.0
 Provides-Extra: test
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: ruamel.yaml; extra == "test"
 
 # A pymoo optimizer plugin for ropt
```

### Comparing `ropt_pymoo-0.2.0/README.md` & `ropt_pymoo-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ropt_pymoo-0.2.0/examples/discrete_ga.py` & `ropt_pymoo-0.3.0/examples/discrete_ga.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,15 @@
     "variables": {
         # Ignored, but needed to establish the number of variables:
         "initial_values": 2 * [0.0],
         "lower_bounds": [0.0, 0.0],
         "upper_bounds": [10.0, 10.0],
     },
     "optimizer": {
-        "backend": "pymoo",
-        "algorithm": "soo.nonconvex.ga.GA",
+        "method": "soo.nonconvex.ga.GA",
         "options": options,
     },
     "nonlinear_constraints": {
         "types": [ConstraintType.LE],
         "rhs_values": [0.0],
     },
 }
```

### Comparing `ropt_pymoo-0.2.0/examples/discrete_ga.yml` & `ropt_pymoo-0.3.0/examples/discrete_ga.yml`

 * *Files identical despite different names*

### Comparing `ropt_pymoo-0.2.0/examples/rosenbrock_cmaes.py` & `ropt_pymoo-0.3.0/examples/rosenbrock_nm.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 CONFIG: Dict[str, Any] = {
     "variables": {
         "initial_values": 2 * [0.0],
         "lower_bounds": [0.0, 0.0],
         "upper_bounds": [2.0, 2.0],
     },
     "optimizer": {
-        "backend": "pymoo",
-        "algorithm": "soo.nonconvex.cmaes.CMAES",
+        "method": "soo.nonconvex.nelder.NelderMead",
         "options": {
             "termination": ("n_iter", 30),
         },
     },
 }
```

### Comparing `ropt_pymoo-0.2.0/pyproject.toml` & `ropt_pymoo-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ropt-pymoo"
-description = "A pymoo backend for the ropt robust optimization library"
+description = "A pymoo plugin for the ropt robust optimization library"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
@@ -16,21 +16,21 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
 ]
 requires-python = ">=3.8"
 dynamic = ["version"]
-dependencies = ["numpy", "pymoo", "pydantic", "ropt>=0.2.1"]
+dependencies = ["numpy", "pymoo", "pydantic", "ropt>=0.3.0"]
 
 [project.optional-dependencies]
 test = ["ruff", "mypy", "pytest", "ruamel.yaml"]
 
 [project.entry-points."ropt.plugins.optimizer"]
-pymoo = "ropt_pymoo.pymoo:PyMooOptimizer"
+pymoo = "ropt_pymoo.pymoo:PyMooOptimizerPlugin"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["ropt_pymoo"]
 
 [tool.setuptools.package-data]
 ropt_pymoo = ["py.typed"]
```

### Comparing `ropt_pymoo-0.2.0/src/ropt_pymoo/_config.py` & `ropt_pymoo-0.3.0/src/ropt_pymoo/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 from pydantic import BaseModel, ConfigDict, Field
 from pymoo.core.algorithm import Algorithm  # noqa: TCH002
 from pymoo.core.operator import Operator  # noqa: TCH002
 from pymoo.core.termination import Termination  # noqa: TCH002
 from pymoo.termination import get_termination
 
-# pylint: disable=no-self-argument,no-self-use
-
 
 class _ParametersBaseModel(BaseModel):
     model_config = ConfigDict(
         arbitrary_types_allowed=True,
         extra="forbid",
         str_min_length=1,
         str_strip_whitespace=True,
```

### Comparing `ropt_pymoo-0.2.0/src/ropt_pymoo/pymoo.py` & `ropt_pymoo-0.3.0/src/ropt_pymoo/pymoo.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """This module implements the pymoo optimization plugin."""
 
 from __future__ import annotations
 
 import copy
+import importlib
+import inspect
 import os
 import sys
 from contextlib import redirect_stdout
 from dataclasses import dataclass, field
 from functools import partial
 from pathlib import Path
 from typing import (
@@ -20,14 +22,19 @@
     Union,
 )
 
 import numpy as np
 from pymoo.core.problem import Problem
 from pymoo.optimize import minimize
 from ropt.enums import ConstraintType
+from ropt.plugins.optimizer.protocol import (
+    OptimizerCallback,
+    OptimizerPluginProtocol,
+    OptimizerProtocol,
+)
 from ropt.plugins.optimizer.utils import create_output_path, filter_linear_constraints
 
 from ._config import ParametersConfig
 
 if TYPE_CHECKING:
     from numpy.typing import NDArray
     from ropt.config.enopt import EnOptConfig
@@ -109,34 +116,35 @@
             lower=copy.deepcopy(self.xl),
             upper=copy.deepcopy(self.xu),
             function=self._function,
             constraints=self._constraints,
         )
 
 
-class PyMooOptimizer:  # pylint: disable=too-many-instance-attributes
-    """Backend class for optimization via pymoo."""
+class PyMooOptimizer(OptimizerProtocol):
+    """Plugin class for optimization via pymoo."""
 
     def __init__(
         self, config: EnOptConfig, optimizer_callback: OptimizerCallback
     ) -> None:
         """Initialize the optimizer implemented by the pymoo plugin.
 
-        See the [ropt.plugins.optimizer.protocol.OptimizerBackend][] protocol.
+        See the [ropt.plugins.optimizer.protocol.OptimizerProtocol][] protocol.
 
         # noqa
         """
         self._config = config
         self._optimizer_callback = optimizer_callback
         options = (
             copy.deepcopy(self._config.optimizer.options)
             if isinstance(self._config.optimizer.options, dict)
             else {}
         )
-        options["algorithm"] = self._config.optimizer.algorithm
+        _, _, method = self._config.optimizer.method.rpartition("/")
+        options["algorithm"] = method
         self._parameters = ParametersConfig.model_validate(options)
         self._bounds = self._get_bounds()
         self._constraints = self._get_constraints()
         self._cached_variables: Optional[NDArray[np.float64]] = None
         self._cached_function: Optional[NDArray[np.float64]] = None
         self._stdout: TextIO
 
@@ -144,15 +152,15 @@
         for algorithm in _NO_FAILURE_HANDLING:
             if algorithm in self._parameters.algorithm:
                 self._allow_nan = False
 
     def start(self, initial_values: NDArray[np.float64]) -> None:
         """Start the optimization.
 
-        See the [ropt.plugins.optimizer.protocol.OptimizerBackend][] protocol.
+        See the [ropt.plugins.optimizer.protocol.Optimizer][] protocol.
 
         # noqa
         """
         self._cached_variables = None
         self._cached_function = None
 
         variable_indices = self._config.variables.indices
@@ -304,7 +312,42 @@
                     return_functions=True,
                     return_gradients=False,
                 )
                 if self._allow_nan:
                     function = np.where(np.isnan(function), np.inf, function)
             self._cached_function = function.copy()
         return self._cached_function
+
+
+class PyMooOptimizerPlugin(OptimizerPluginProtocol):
+    """Default filter transform plugin class."""
+
+    def create(
+        self, config: EnOptConfig, optimizer_callback: OptimizerCallback
+    ) -> PyMooOptimizer:
+        """Initialize the optimizer plugin.
+
+        See the [ropt.plugins.optimizer.protocol.OptimizerPluginProtocol][] protocol.
+
+        # noqa
+        """
+        return PyMooOptimizer(config, optimizer_callback)
+
+    def is_supported(self, method: str) -> bool:
+        """Check if a method is supported.
+
+        See the [ropt.plugins.protocol.PluginProtocol][] protocol.
+
+        # noqa
+        """
+        module_name, _, class_name = method.rpartition(".")
+        if not module_name:
+            return False
+        full_module_name = f"pymoo.algorithms.{module_name}"
+        try:
+            module = importlib.import_module(full_module_name)
+        except ImportError:
+            return False
+        for _, cls in inspect.getmembers(module, inspect.isclass):
+            if cls.__name__ == class_name:
+                return True
+        return False
```

### Comparing `ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/PKG-INFO` & `ropt_pymoo-0.3.0/src/ropt_pymoo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ropt-pymoo
-Version: 0.2.0
-Summary: A pymoo backend for the ropt robust optimization library
+Version: 0.3.0
+Summary: A pymoo plugin for the ropt robust optimization library
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,15 +14,15 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pymoo
 Requires-Dist: pydantic
-Requires-Dist: ropt>=0.2.1
+Requires-Dist: ropt>=0.3.0
 Provides-Extra: test
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: ruamel.yaml; extra == "test"
 
 # A pymoo optimizer plugin for ropt
```

### Comparing `ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/SOURCES.txt` & `ropt_pymoo-0.3.0/src/ropt_pymoo.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 README.md
 pyproject.toml
 .github/workflows/release.yml
 .github/workflows/static-checks.yml
 .github/workflows/tests.yml
 examples/discrete_ga.py
 examples/discrete_ga.yml
-examples/rosenbrock_cmaes.py
+examples/rosenbrock_nm.py
 src/ropt_pymoo/__init__.py
 src/ropt_pymoo/_config.py
 src/ropt_pymoo/py.typed
 src/ropt_pymoo/pymoo.py
 src/ropt_pymoo/version.py
 src/ropt_pymoo.egg-info/PKG-INFO
 src/ropt_pymoo.egg-info/SOURCES.txt
```

### Comparing `ropt_pymoo-0.2.0/tests/conftest.py` & `ropt_pymoo-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ropt_pymoo-0.2.0/tests/test_examples.py` & `ropt_pymoo-0.3.0/tests/test_examples.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     assert spec is not None
     module = importlib.util.module_from_spec(spec)
     assert spec.loader is not None
     spec.loader.exec_module(module)
     return module
 
 
-def test_rosenbrock_cmaes(tmp_path: Path) -> None:
+def test_rosenbrock_de(tmp_path: Path) -> None:
     os.chdir(tmp_path)
-    module = _load_from_file("rosenbrock_cmaes")
+    module = _load_from_file("rosenbrock_nm")
     module.main()
 
 
 def test_discrete_ga(tmp_path: Path) -> None:
     shutil.copyfile(
         EXAMPLES_DIR / "discrete_ga.yml",
         tmp_path / "discrete_ga.yml",
```

### Comparing `ropt_pymoo-0.2.0/tests/test_pymoo_backend.py` & `ropt_pymoo-0.3.0/tests/test_pymoo_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable=protected-access
-
 from typing import Any, Dict, cast
 
 import numpy as np
 import pytest
 from numpy.typing import NDArray
 from ropt.enums import ConstraintType, EventType, OptimizerExitCode
 from ropt.events import OptimizationEvent
@@ -13,16 +11,15 @@
 @pytest.fixture(name="enopt_config")
 def enopt_config_fixture() -> Dict[str, Any]:
     return {
         "variables": {
             "initial_values": [0.2, 0.0, 0.1],
         },
         "optimizer": {
-            "backend": "pymoo",
-            "algorithm": "soo.nonconvex.nelder.NelderMead",
+            "method": "soo.nonconvex.nelder.NelderMead",
         },
         "objective_functions": {
             "weights": [0.75, 0.25],
         },
     }
 
 
@@ -311,15 +308,15 @@
 
 
 def test_pymoo_bound_constraints_with_failure(
     enopt_config: Dict[str, Any], evaluator: Any, test_functions: Any
 ) -> None:
     enopt_config["variables"]["lower_bounds"] = [0.15, -1.0, -1.0]
     enopt_config["variables"]["upper_bounds"] = [1.0, 1.0, 0.2]
-    enopt_config["optimizer"]["algorithm"] = "soo.nonconvex.de.DE"
+    enopt_config["optimizer"]["method"] = "soo.nonconvex.de.DE"
     enopt_config["optimizer"]["parallel"] = True
     enopt_config["optimizer"]["max_functions"] = 800
     enopt_config["realizations"] = {"realization_min_success": 0}
     optimizer = EnsembleOptimizer(evaluator())
     result1 = optimizer.start_optimization(
         plan=[
             {"config": enopt_config},
@@ -356,15 +353,15 @@
 
 
 def test_pymoo_bound_constraints_no_failure_handling(
     enopt_config: Dict[str, Any], evaluator: Any, test_functions: Any
 ) -> None:
     enopt_config["variables"]["lower_bounds"] = [0.15, -1.0, -1.0]
     enopt_config["variables"]["upper_bounds"] = [1.0, 1.0, 0.2]
-    enopt_config["optimizer"]["algorithm"] = "soo.nonconvex.nelder.NelderMead"
+    enopt_config["optimizer"]["method"] = "soo.nonconvex.nelder.NelderMead"
     enopt_config["optimizer"]["parallel"] = True
     enopt_config["optimizer"]["max_functions"] = 800
 
     optimizer = EnsembleOptimizer(evaluator())
     result1 = optimizer.start_optimization(
         plan=[
             {"config": enopt_config},
```

