# Comparing `tmp/ropt_nomad-0.2.1.tar.gz` & `tmp/ropt_nomad-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ropt_nomad-0.2.1.tar", last modified: Mon Apr 29 12:25:44 2024, max compression
+gzip compressed data, was "ropt_nomad-0.3.0.tar", last modified: Mon May  6 15:27:39 2024, max compression
```

## Comparing `ropt_nomad-0.2.1.tar` & `ropt_nomad-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:44.680877 ropt_nomad-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:44.676877 ropt_nomad-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:44.676877 ropt_nomad-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/.github/workflows/static-checks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-29 12:25:44.680877 ropt_nomad-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:44.676877 ropt_nomad-0.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/examples/discrete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/examples/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:25:44.680877 ropt_nomad-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:44.676877 ropt_nomad-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:44.680877 ropt_nomad-0.2.1/src/ropt_nomad/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/src/ropt_nomad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/src/ropt_nomad/nomad.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/src/ropt_nomad/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 12:25:44.000000 ropt_nomad-0.2.1/src/ropt_nomad/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:44.680877 ropt_nomad-0.2.1/src/ropt_nomad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-29 12:25:44.000000 ropt_nomad-0.2.1/src/ropt_nomad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-29 12:25:44.000000 ropt_nomad-0.2.1/src/ropt_nomad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:25:44.000000 ropt_nomad-0.2.1/src/ropt_nomad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-29 12:25:44.000000 ropt_nomad-0.2.1/src/ropt_nomad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 12:25:44.000000 ropt_nomad-0.2.1/src/ropt_nomad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 12:25:44.000000 ropt_nomad-0.2.1/src/ropt_nomad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:44.680877 ropt_nomad-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/tests/test_nomad_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:27:39.383321 ropt_nomad-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:27:39.375321 ropt_nomad-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:27:39.379321 ropt_nomad-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-06 15:27:35.000000 ropt_nomad-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-06 15:27:35.000000 ropt_nomad-0.3.0/.github/workflows/static-checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-06 15:27:35.000000 ropt_nomad-0.3.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-06 15:27:35.000000 ropt_nomad-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 15:27:35.000000 ropt_nomad-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-06 15:27:39.383321 ropt_nomad-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-06 15:27:35.000000 ropt_nomad-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:27:39.379321 ropt_nomad-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-06 15:27:35.000000 ropt_nomad-0.3.0/examples/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-06 15:27:35.000000 ropt_nomad-0.3.0/examples/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-06 15:27:35.000000 ropt_nomad-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 15:27:39.383321 ropt_nomad-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:27:39.375321 ropt_nomad-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:27:39.379321 ropt_nomad-0.3.0/src/ropt_nomad/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 15:27:35.000000 ropt_nomad-0.3.0/src/ropt_nomad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13788 2024-05-06 15:27:35.000000 ropt_nomad-0.3.0/src/ropt_nomad/nomad.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:27:35.000000 ropt_nomad-0.3.0/src/ropt_nomad/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-06 15:27:39.000000 ropt_nomad-0.3.0/src/ropt_nomad/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:27:39.383321 ropt_nomad-0.3.0/src/ropt_nomad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-06 15:27:39.000000 ropt_nomad-0.3.0/src/ropt_nomad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-06 15:27:39.000000 ropt_nomad-0.3.0/src/ropt_nomad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 15:27:39.000000 ropt_nomad-0.3.0/src/ropt_nomad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-06 15:27:39.000000 ropt_nomad-0.3.0/src/ropt_nomad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-06 15:27:39.000000 ropt_nomad-0.3.0/src/ropt_nomad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 15:27:39.000000 ropt_nomad-0.3.0/src/ropt_nomad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 15:27:39.379321 ropt_nomad-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 15:27:35.000000 ropt_nomad-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-06 15:27:35.000000 ropt_nomad-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-06 15:27:35.000000 ropt_nomad-0.3.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12977 2024-05-06 15:27:35.000000 ropt_nomad-0.3.0/tests/test_nomad_backend.py
```

### Comparing `ropt_nomad-0.2.1/.github/workflows/release.yml` & `ropt_nomad-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.2.1/.github/workflows/static-checks.yml` & `ropt_nomad-0.3.0/.github/workflows/static-checks.yml`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.2.1/.github/workflows/tests.yml` & `ropt_nomad-0.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.2.1/LICENSE` & `ropt_nomad-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.2.1/PKG-INFO` & `ropt_nomad-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: ropt-nomad
-Version: 0.2.1
-Summary: A NOMAD backend for the ropt robust optimization package
+Version: 0.3.0
+Summary: A NOMAD plugin for the ropt robust optimization package
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyNomadBBO
-Requires-Dist: ropt>=0.2.1
+Requires-Dist: ropt>=0.3.0
 Provides-Extra: test
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 
 # A NOMAD optimizer plugin for ropt
 This package installs a plugin for the [ropt](https://github.com/tno-ropt/ropt)
```

### Comparing `ropt_nomad-0.2.1/README.md` & `ropt_nomad-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.2.1/examples/discrete.py` & `ropt_nomad-0.3.0/examples/discrete.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "variables": {
         "initial_values": 2 * [0.0],
         "lower_bounds": [0.0, 0.0],
         "upper_bounds": [10.0, 10.0],
         "types": VariableType.INTEGER,
     },
     "optimizer": {
-        "backend": "nomad",
+        "method": "nomad/default",
         "options": ["MAX_EVAL 100"],
         "output_dir": ".",
     },
     "nonlinear_constraints": {
         "types": [ConstraintType.LE],
         "rhs_values": [0.0],
     },
```

### Comparing `ropt_nomad-0.2.1/examples/rosenbrock.py` & `ropt_nomad-0.3.0/examples/rosenbrock.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 CONFIG: Dict[str, Any] = {
     "variables": {
         "initial_values": 2 * [0.3],
         "lower_bounds": [0.2, 0.1],
         "upper_bounds": [2.1, 2.2],
     },
     "optimizer": {
-        "backend": "nomad",
+        "method": "nomad/default",
         "max_iterations": 20,
         "output_dir": ".",
     },
 }
 
 
 def rosenbrock(variables: NDArray[np.float64], _: EvaluatorContext) -> EvaluatorResult:
```

### Comparing `ropt_nomad-0.2.1/pyproject.toml` & `ropt_nomad-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ropt-nomad"
-description = "A NOMAD backend for the ropt robust optimization package"
+description = "A NOMAD plugin for the ropt robust optimization package"
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
-dependencies = ["PyNomadBBO", "ropt>=0.2.1"]
+dependencies = ["PyNomadBBO", "ropt>=0.3.0"]
 
 [project.optional-dependencies]
 test = ["ruff", "mypy", "pytest"]
 
 [project.entry-points."ropt.plugins.optimizer"]
-nomad = "ropt_nomad.nomad:NomadOptimizer"
+nomad = "ropt_nomad.nomad:NomadOptimizerPlugin"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["ropt_nomad"]
 
 [tool.setuptools.package-data]
 ropt_nomad = ["py.typed"]
```

### Comparing `ropt_nomad-0.2.1/src/ropt_nomad/nomad.py` & `ropt_nomad-0.3.0/src/ropt_nomad/nomad.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,31 @@
     Union,
 )
 
 import numpy as np
 import PyNomad
 from ropt.enums import ConstraintType, VariableType
 from ropt.exceptions import ConfigError
+from ropt.plugins.optimizer.protocol import (
+    OptimizerCallback,
+    OptimizerPluginProtocol,
+    OptimizerProtocol,
+)
 from ropt.plugins.optimizer.utils import create_output_path, filter_linear_constraints
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from numpy.typing import NDArray
     from ropt.config.enopt import EnOptConfig
-    from ropt.plugins.optimizer.protocol import OptimizerCallback
 
 _OUTPUT_FILE = "optimizer_output"
 
+_SUPPORTED_METHODS = {"mads"}
+
 
 class _Redirector:
     def __init__(self, output_file: Optional[Path]) -> None:
         sys.stdout.flush()
         sys.stderr.flush()
         self._old_stdout = os.dup(1)
         self._old_stderr = os.dup(2)
@@ -67,15 +73,15 @@
         finally:
             sys.stdout.flush()
             sys.stderr.flush()
             os.dup2(self._new_stdout, 1)
             os.dup2(self._new_stdout, 2)
 
 
-class NomadOptimizer:  # pylint: disable=too-many-instance-attributes
+class NomadOptimizer(OptimizerProtocol):
     """Backend class for optimization via nomad."""
 
     def __init__(
         self,
         enopt_config: EnOptConfig,
         optimizer_callback: OptimizerCallback,
     ) -> None:
@@ -90,14 +96,22 @@
         self._bounds = self._get_bounds()
         self._parameters = self._get_parameters()
         self._coefficients: Optional[NDArray[np.float64]] = None
         self._rhs_values: Optional[NDArray[np.float64]] = None
         self._cached_variables: Optional[NDArray[np.float64]] = None
         self._cached_function: Optional[NDArray[np.float64]] = None
         self._redirector: _Redirector
+
+        _, _, self._method = self._config.optimizer.method.lower().rpartition("/")
+        if self._method == "default":
+            self._method = "mads"
+        if self._method not in _SUPPORTED_METHODS:
+            msg = f"NOMAD optimizer algorithm {self._method} is not supported"
+            raise NotImplementedError(msg)
+
         self._get_constraints()
 
     def start(self, initial_values: NDArray[np.float64]) -> None:
         """Start the optimization.
 
         See the [ropt.plugins.optimizer.protocol.OptimizerBackend][] protocol.
 
@@ -113,27 +127,27 @@
         output_dir = self._config.optimizer.output_dir
         output_file: Optional[Path] = None
         if output_dir is not None:
             output_file = create_output_path(_OUTPUT_FILE, output_dir, suffix=".txt")
 
         self._redirector = _Redirector(output_file)
         with self._redirector.start():
-            PyNomad.optimize(  # pylint: disable=c-extension-no-member
+            PyNomad.optimize(
                 self._evaluate,
                 initial_values.tolist(),
                 self._bounds[0],
                 self._bounds[1],
                 self._parameters,
             )
 
     @property
     def allow_nan(self) -> bool:
         """Whether NaN is allowed.
 
-        See the [ropt.plugins.optimizer.protocol.Optimizer][] protocol.
+        See the [ropt.plugins.optimizer.protocol.OptimizerProtocol][] protocol.
 
         # noqa
         """
         return True
 
     def _get_bounds(self) -> Tuple[List[float], List[float]]:
         lower_bounds = self._config.variables.lower_bounds
@@ -334,7 +348,31 @@
                 function, _ = self._optimizer_callback(
                     variables,
                     return_functions=True,
                     return_gradients=False,
                 )
             self._cached_function = function.copy()
         return self._cached_function
+
+
+class NomadOptimizerPlugin(OptimizerPluginProtocol):
+    """Default filter transform plugin class."""
+
+    def create(
+        self, config: EnOptConfig, optimizer_callback: OptimizerCallback
+    ) -> NomadOptimizer:
+        """Initialize the optimizer plugin.
+
+        See the [ropt.plugins.optimizer.protocol.OptimizerPluginProtocol][] protocol.
+
+        # noqa
+        """
+        return NomadOptimizer(config, optimizer_callback)
+
+    def is_supported(self, method: str) -> bool:
+        """Check if a method is supported.
+
+        See the [ropt.plugins.protocol.PluginProtocol][] protocol.
+
+        # noqa
+        """
+        return method.lower() in (_SUPPORTED_METHODS | {"default"})
```

### Comparing `ropt_nomad-0.2.1/src/ropt_nomad.egg-info/PKG-INFO` & `ropt_nomad-0.3.0/src/ropt_nomad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: ropt-nomad
-Version: 0.2.1
-Summary: A NOMAD backend for the ropt robust optimization package
+Version: 0.3.0
+Summary: A NOMAD plugin for the ropt robust optimization package
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyNomadBBO
-Requires-Dist: ropt>=0.2.1
+Requires-Dist: ropt>=0.3.0
 Provides-Extra: test
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 
 # A NOMAD optimizer plugin for ropt
 This package installs a plugin for the [ropt](https://github.com/tno-ropt/ropt)
```

### Comparing `ropt_nomad-0.2.1/src/ropt_nomad.egg-info/SOURCES.txt` & `ropt_nomad-0.3.0/src/ropt_nomad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.2.1/tests/conftest.py` & `ropt_nomad-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.2.1/tests/test_examples.py` & `ropt_nomad-0.3.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.2.1/tests/test_nomad_backend.py` & `ropt_nomad-0.3.0/tests/test_nomad_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pylint: disable=protected-access
-
 from typing import Any, Dict, cast
 
 import numpy as np
 import pytest
 from numpy.typing import NDArray
 from ropt.enums import ConstraintType
 from ropt.exceptions import ConfigError
@@ -13,15 +11,15 @@
 @pytest.fixture(name="enopt_config")
 def enopt_config_fixture() -> Dict[str, Any]:
     return {
         "variables": {
             "initial_values": [0.2, 0.0, 0.1],
         },
         "optimizer": {
-            "backend": "nomad",
+            "method": "nomad/default",
             "max_iterations": 7,
         },
         "objective_functions": {
             "weights": [0.75, 0.25],
         },
     }
```

