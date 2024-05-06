# Comparing `tmp/ropt_dakota-0.2.0.tar.gz` & `tmp/ropt_dakota-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ropt_dakota-0.2.0.tar", last modified: Mon Apr 29 12:21:27 2024, max compression
+gzip compressed data, was "ropt_dakota-0.3.0.tar", last modified: Mon May  6 15:28:18 2024, max compression
```

## Comparing `ropt_dakota-0.2.0.tar` & `ropt_dakota-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:27.119937 ropt_dakota-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:27.115937 ropt_dakota-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:27.119937 ropt_dakota-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/.github/workflows/static-checks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-29 12:21:27.119937 ropt_dakota-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:21:27.119937 ropt_dakota-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:27.115937 ropt_dakota-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:27.119937 ropt_dakota-0.2.0/src/ropt_dakota/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/src/ropt_dakota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18513 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/src/ropt_dakota/dakota.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/src/ropt_dakota/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 12:21:27.000000 ropt_dakota-0.2.0/src/ropt_dakota/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:27.119937 ropt_dakota-0.2.0/src/ropt_dakota.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-29 12:21:27.000000 ropt_dakota-0.2.0/src/ropt_dakota.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-29 12:21:27.000000 ropt_dakota-0.2.0/src/ropt_dakota.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:21:27.000000 ropt_dakota-0.2.0/src/ropt_dakota.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 12:21:27.000000 ropt_dakota-0.2.0/src/ropt_dakota.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-29 12:21:27.000000 ropt_dakota-0.2.0/src/ropt_dakota.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 12:21:27.000000 ropt_dakota-0.2.0/src/ropt_dakota.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:27.119937 ropt_dakota-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    12950 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/tests/test_dakota_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:18.484045 ropt_dakota-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:18.476045 ropt_dakota-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:18.480045 ropt_dakota-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-06 15:28:14.000000 ropt_dakota-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-06 15:28:14.000000 ropt_dakota-0.3.0/.github/workflows/static-checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-06 15:28:14.000000 ropt_dakota-0.3.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-06 15:28:14.000000 ropt_dakota-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 15:28:14.000000 ropt_dakota-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-06 15:28:18.484045 ropt_dakota-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-06 15:28:14.000000 ropt_dakota-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-06 15:28:14.000000 ropt_dakota-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:28:18.484045 ropt_dakota-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:18.476045 ropt_dakota-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:18.480045 ropt_dakota-0.3.0/src/ropt_dakota/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-06 15:28:14.000000 ropt_dakota-0.3.0/src/ropt_dakota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19482 2024-05-06 15:28:14.000000 ropt_dakota-0.3.0/src/ropt_dakota/dakota.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:14.000000 ropt_dakota-0.3.0/src/ropt_dakota/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 15:28:18.000000 ropt_dakota-0.3.0/src/ropt_dakota/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:18.484045 ropt_dakota-0.3.0/src/ropt_dakota.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-06 15:28:18.000000 ropt_dakota-0.3.0/src/ropt_dakota.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-06 15:28:18.000000 ropt_dakota-0.3.0/src/ropt_dakota.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:28:18.000000 ropt_dakota-0.3.0/src/ropt_dakota.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 15:28:18.000000 ropt_dakota-0.3.0/src/ropt_dakota.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 15:28:18.000000 ropt_dakota-0.3.0/src/ropt_dakota.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 15:28:18.000000 ropt_dakota-0.3.0/src/ropt_dakota.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:18.480045 ropt_dakota-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:28:14.000000 ropt_dakota-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-06 15:28:14.000000 ropt_dakota-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12937 2024-05-06 15:28:14.000000 ropt_dakota-0.3.0/tests/test_dakota_backend.py
```

### Comparing `ropt_dakota-0.2.0/.github/workflows/release.yml` & `ropt_dakota-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ropt_dakota-0.2.0/.github/workflows/static-checks.yml` & `ropt_dakota-0.3.0/.github/workflows/static-checks.yml`

 * *Files identical despite different names*

### Comparing `ropt_dakota-0.2.0/.github/workflows/tests.yml` & `ropt_dakota-0.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ropt_dakota-0.2.0/LICENSE` & `ropt_dakota-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ropt_dakota-0.2.0/PKG-INFO` & `ropt_dakota-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt-dakota
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Dakota optimizer plugin for ropt
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: carolina
-Requires-Dist: ropt>=0.2.1
+Requires-Dist: ropt>=0.3.0
 Provides-Extra: test
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 
 # A Dakota optimizer plugin for `ropt`
 This package installs a plugin for the `ropt` robust optimization package,
```

### Comparing `ropt_dakota-0.2.0/README.md` & `ropt_dakota-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ropt_dakota-0.2.0/pyproject.toml` & `ropt_dakota-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,21 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
 ]
 requires-python = ">=3.8"
 dynamic = ["version"]
-dependencies = ["numpy", "carolina", "ropt>=0.2.1"]
+dependencies = ["numpy", "carolina", "ropt>=0.3.0"]
 
 [project.optional-dependencies]
 test = ["ruff", "mypy", "pytest"]
 
 [project.entry-points."ropt.plugins.optimizer"]
-dakota = "ropt_dakota.dakota:DakotaOptimizer"
+dakota = "ropt_dakota.dakota:DakotaOptimizerPlugin"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["ropt_dakota"]
 
 [tool.setuptools.package-data]
 ropt_dakota = ["py.typed"]
```

### Comparing `ropt_dakota-0.2.0/src/ropt_dakota/dakota.py` & `ropt_dakota-0.3.0/src/ropt_dakota/dakota.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,77 @@
 """This module implements the Dakota optimization plugin."""
 
 from math import isfinite
 from os import chdir
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import Any, ClassVar, Dict, List, Optional, Set, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
 import numpy as np
 from dakota import _USER_DATA, DakotaBase, DakotaInput, run_dakota
 from numpy.typing import NDArray
 from ropt.config.enopt import EnOptConfig, OptimizerConfig
 from ropt.enums import ConstraintType
 from ropt.exceptions import ConfigError
-from ropt.plugins.optimizer.protocol import OptimizerCallback
+from ropt.plugins.optimizer.protocol import (
+    OptimizerCallback,
+    OptimizerPluginProtocol,
+    OptimizerProtocol,
+)
 from ropt.plugins.optimizer.utils import create_output_path, filter_linear_constraints
 
 _PRECISION: int = 8
 _LARGE_NUMBER_FOR_INF = 1e30
 
 _ConstraintIndices = Tuple[
     NDArray[np.intc],
     NDArray[np.intc],
     NDArray[np.intc],
 ]
 
+_SUPPORTED_METHODS = {
+    "optpp_q_newton",
+    "conmin_mfd",
+    "conmin_frcg",
+    "mesh_adaptive_search",
+    "coliny_ea",
+    "soga",
+    "moga",
+    "asynch_pattern_search",
+}
 
-class DakotaOptimizer:
-    """Backend class for optimization via Dakota."""
 
-    SUPPORTED_ALGORITHMS: ClassVar[Set[str]] = {
-        "optpp_q_newton",
-        "conmin_mfd",
-        "conmin_frcg",
-        "mesh_adaptive_search",
-        "coliny_ea",
-        "soga",
-        "moga",
-        "asynch_pattern_search",
-    }
+class DakotaOptimizer(OptimizerProtocol):
+    """Plugin class for optimization via Dakota."""
 
     def __init__(
         self, config: EnOptConfig, optimizer_callback: OptimizerCallback
     ) -> None:
         """Initialize the optimizer implemented by the Dakota plugin.
 
-        See the [ropt.plugins.optimizer.protocol.Optimizer][] protocol.
+        See the [ropt.plugins.optimizer.protocol.OptimizerProtocol][] protocol.
 
         # noqa
         """
         self._config = config
         self._optimizer_callback = optimizer_callback
         self._constraint_indices = self._get_constraint_indices()
         self._output_dir: Path
 
+        _, _, self._method = self._config.optimizer.method.lower().rpartition("/")
+        if self._method == "default":
+            self._method = "optpp_q_newton"
+        if self._method not in _SUPPORTED_METHODS:
+            msg = f"Dakota optimizer algorithm {self._method} is not supported"
+            raise NotImplementedError(msg)
+
     def start(self, initial_values: NDArray[np.float64]) -> None:
         """Start the optimization.
 
-        See the [ropt.plugins.optimizer.protocol.Optimizer][] protocol.
+        See the [ropt.plugins.optimizer.protocol.OptimizerProtocol][] protocol.
 
         # noqa
         """
         if self._config.optimizer.output_dir is None:
             with TemporaryDirectory() as output_dir:
                 self._output_dir = Path(output_dir)
                 self._start(initial_values)
@@ -68,15 +79,15 @@
             self._output_dir = self._config.optimizer.output_dir
             self._start(initial_values)
 
     @property
     def allow_nan(self) -> bool:
         """Whether NaN is allowed.
 
-        See the [ropt.plugins.optimizer.protocol.Optimizer][] protocol.
+        See the [ropt.plugins.optimizer.protocol.OptimizerProtocol][] protocol.
 
         # noqa
         """
         return False
 
     def _get_constraint_indices(self) -> Optional[_ConstraintIndices]:
         if self._config.nonlinear_constraints is None:
@@ -115,41 +126,38 @@
                 "no_hessians",
                 *self._get_responses_section(),
             ],
         }
 
     def _get_method_section(self) -> List[str]:
         inputs: List[str] = []
-        algorithm = self._config.optimizer.algorithm
-        if algorithm is None:
-            algorithm = "optpp_q_newton"
-        inputs.append(algorithm)
+        inputs.append(self._method)
         # Scaling is always on
         inputs.append("scaling")
         iterations = self._config.optimizer.max_iterations
-        if iterations is not None and algorithm != "asynch_pattern_search":
+        if iterations is not None and self._method != "asynch_pattern_search":
             inputs.append(f"max_iterations = {iterations}")
         convergence_tolerance = self._config.optimizer.tolerance
         if convergence_tolerance is not None:
             tolerance_option = (
                 "variable_tolerance"
-                if algorithm in ["mesh_adaptive_search", "asynch_pattern_search"]
+                if self._method in ["mesh_adaptive_search", "asynch_pattern_search"]
                 else "convergence_tolerance"
             )
             inputs.append(f"{tolerance_option} = {convergence_tolerance}")
         # The Dakota interface seems not be able to deal with with speculative
         # and split_evaluations simultaneously. Do not enable speculative if
         # split_evaluations is defined.
         if (
             self._config.optimizer.speculative
             and not self._config.optimizer.split_evaluations
         ):
             inputs.append("speculative")
         # Options are put in the method section:
-        return inputs + self._get_options(algorithm)
+        return inputs + self._get_options(self._method)
 
     def _get_options(self, algorithm: str) -> List[str]:
         inputs: List[str] = []
         if isinstance(self._config.optimizer.options, list):
             try:
                 for option in self._config.optimizer.options:
                     stripped = option.strip()
@@ -472,7 +480,32 @@
         ge_indices, le_indices, eq_indices = constraint_indices
         indices = np.hstack((0, le_indices + 1, ge_indices + 1, eq_indices + 1))
         if return_functions:
             functions = functions[indices]
         if compute_gradients:
             gradients = gradients[indices, :]
     return functions, gradients
+
+
+class DakotaOptimizerPlugin(OptimizerPluginProtocol):
+    """Plugin class for optimization via Dakota."""
+
+    def create(
+        self, config: EnOptConfig, optimizer_callback: OptimizerCallback
+    ) -> DakotaOptimizer:
+        """Initialize the optimizer plugin.
+
+        See the [ropt.plugins.optimizer.protocol.OptimizerPluginProtocol][] protocol.
+
+        # noqa
+        """
+        return DakotaOptimizer(config, optimizer_callback)
+
+    @classmethod
+    def is_supported(cls, method: str) -> bool:
+        """Check if a method is supported.
+
+        See the [ropt.plugins.protocol.PluginProtocol][] protocol.
+
+        # noqa
+        """
+        return method.lower() in (_SUPPORTED_METHODS | {"default"})
```

### Comparing `ropt_dakota-0.2.0/src/ropt_dakota.egg-info/PKG-INFO` & `ropt_dakota-0.3.0/src/ropt_dakota.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt-dakota
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Dakota optimizer plugin for ropt
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: carolina
-Requires-Dist: ropt>=0.2.1
+Requires-Dist: ropt>=0.3.0
 Provides-Extra: test
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 
 # A Dakota optimizer plugin for `ropt`
 This package installs a plugin for the `ropt` robust optimization package,
```

### Comparing `ropt_dakota-0.2.0/src/ropt_dakota.egg-info/SOURCES.txt` & `ropt_dakota-0.3.0/src/ropt_dakota.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ropt_dakota-0.2.0/tests/conftest.py` & `ropt_dakota-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ropt_dakota-0.2.0/tests/test_dakota_backend.py` & `ropt_dakota-0.3.0/tests/test_dakota_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 import numpy as np
 import pytest
 from numpy.typing import NDArray
 from ropt.enums import ConstraintType, EventType, OptimizerExitCode
 from ropt.events import OptimizationEvent
 from ropt.optimization import EnsembleOptimizer
 from ropt.results import GradientResults
-from ropt_dakota.dakota import DakotaOptimizer
+from ropt_dakota.dakota import _SUPPORTED_METHODS
 
 
 @pytest.fixture(name="enopt_config")
 def enopt_config_fixture() -> Dict[str, Any]:
     return {
         "variables": {
             "initial_values": [0.0, 0.0, 0.1],
         },
         "optimizer": {
-            "backend": "dakota",
+            "method": "dakota/default",
             "tolerance": 1e-6,
         },
         "objective_functions": {
             "weights": [0.75, 0.25],
         },
         "gradient": {
             "perturbation_magnitudes": 0.01,
@@ -63,22 +63,20 @@
 
 
 @pytest.mark.parametrize(
     # The conmin algorithms are not tested, since they produce some output to
     # the terminal that we are not able to suppress. The soga method crashes
     # occasionally.
     "method",
-    sorted(
-        DakotaOptimizer.SUPPORTED_ALGORITHMS - {"conmin_mfd", "conmin_frcg", "soga"}
-    ),
+    sorted(_SUPPORTED_METHODS - {"conmin_mfd", "conmin_frcg", "soga"}),
 )
 def test_dakota_bound_constraint(
     enopt_config: Any, method: str, evaluator: Any
 ) -> None:
-    enopt_config["optimizer"]["algorithm"] = method
+    enopt_config["optimizer"]["method"] = f"dakota/{method}"
     enopt_config["variables"]["lower_bounds"] = -1.0
     enopt_config["variables"]["upper_bounds"] = [1.0, 1.0, 0.2]
 
     optimizer = EnsembleOptimizer(evaluator())
     result = optimizer.start_optimization(
         plan=[
             {"config": enopt_config},
```

