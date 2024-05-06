# Comparing `tmp/jaxlie-1.3.4.tar.gz` & `tmp/jaxlie-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxlie-1.3.4.tar", last modified: Mon Dec 11 09:19:33 2023, max compression
+gzip compressed data, was "jaxlie-1.4.0.tar", last modified: Mon May  6 06:03:11 2024, max compression
```

## Comparing `jaxlie-1.3.4.tar` & `jaxlie-1.4.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 09:19:33.934075 jaxlie-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-11 09:19:25.000000 jaxlie-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2023-12-11 09:19:33.934075 jaxlie-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2023-12-11 09:19:25.000000 jaxlie-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 09:19:33.930075 jaxlie-1.3.4/jaxlie/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-11 09:19:25.000000 jaxlie-1.3.4/jaxlie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7878 2023-12-11 09:19:25.000000 jaxlie-1.3.4/jaxlie/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2023-12-11 09:19:25.000000 jaxlie-1.3.4/jaxlie/_se2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2023-12-11 09:19:25.000000 jaxlie-1.3.4/jaxlie/_se3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2023-12-11 09:19:25.000000 jaxlie-1.3.4/jaxlie/_so2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12491 2023-12-11 09:19:25.000000 jaxlie-1.3.4/jaxlie/_so3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 09:19:33.930075 jaxlie-1.3.4/jaxlie/hints/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-12-11 09:19:25.000000 jaxlie-1.3.4/jaxlie/hints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 09:19:33.934075 jaxlie-1.3.4/jaxlie/manifold/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-12-11 09:19:25.000000 jaxlie-1.3.4/jaxlie/manifold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2023-12-11 09:19:25.000000 jaxlie-1.3.4/jaxlie/manifold/_backprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     5802 2023-12-11 09:19:25.000000 jaxlie-1.3.4/jaxlie/manifold/_deltas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2023-12-11 09:19:25.000000 jaxlie-1.3.4/jaxlie/manifold/_tree_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 09:19:25.000000 jaxlie-1.3.4/jaxlie/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 09:19:33.934075 jaxlie-1.3.4/jaxlie/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-12-11 09:19:25.000000 jaxlie-1.3.4/jaxlie/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-12-11 09:19:25.000000 jaxlie-1.3.4/jaxlie/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 09:19:33.934075 jaxlie-1.3.4/jaxlie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2023-12-11 09:19:33.000000 jaxlie-1.3.4/jaxlie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-12-11 09:19:33.000000 jaxlie-1.3.4/jaxlie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 09:19:33.000000 jaxlie-1.3.4/jaxlie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-12-11 09:19:33.000000 jaxlie-1.3.4/jaxlie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-11 09:19:33.000000 jaxlie-1.3.4/jaxlie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 09:19:33.934075 jaxlie-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2023-12-11 09:19:25.000000 jaxlie-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 09:19:33.934075 jaxlie-1.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2023-12-11 09:19:25.000000 jaxlie-1.3.4/tests/test_autodiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2023-12-11 09:19:25.000000 jaxlie-1.3.4/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2023-12-11 09:19:25.000000 jaxlie-1.3.4/tests/test_group_axioms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2023-12-11 09:19:25.000000 jaxlie-1.3.4/tests/test_manifold.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2023-12-11 09:19:25.000000 jaxlie-1.3.4/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-12-11 09:19:25.000000 jaxlie-1.3.4/tests/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:03:11.449120 jaxlie-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-06 06:03:03.000000 jaxlie-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-06 06:03:11.449120 jaxlie-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-06 06:03:03.000000 jaxlie-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:03:11.445120 jaxlie-1.4.0/jaxlie/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-06 06:03:03.000000 jaxlie-1.4.0/jaxlie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-05-06 06:03:03.000000 jaxlie-1.4.0/jaxlie/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-05-06 06:03:03.000000 jaxlie-1.4.0/jaxlie/_se2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-05-06 06:03:03.000000 jaxlie-1.4.0/jaxlie/_se3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-06 06:03:03.000000 jaxlie-1.4.0/jaxlie/_so2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14134 2024-05-06 06:03:03.000000 jaxlie-1.4.0/jaxlie/_so3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:03:11.445120 jaxlie-1.4.0/jaxlie/hints/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-06 06:03:03.000000 jaxlie-1.4.0/jaxlie/hints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:03:11.449120 jaxlie-1.4.0/jaxlie/manifold/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-06 06:03:03.000000 jaxlie-1.4.0/jaxlie/manifold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-06 06:03:03.000000 jaxlie-1.4.0/jaxlie/manifold/_backprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-05-06 06:03:03.000000 jaxlie-1.4.0/jaxlie/manifold/_deltas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-06 06:03:03.000000 jaxlie-1.4.0/jaxlie/manifold/_tree_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 06:03:03.000000 jaxlie-1.4.0/jaxlie/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:03:11.449120 jaxlie-1.4.0/jaxlie/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-06 06:03:03.000000 jaxlie-1.4.0/jaxlie/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-06 06:03:03.000000 jaxlie-1.4.0/jaxlie/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:03:11.449120 jaxlie-1.4.0/jaxlie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-06 06:03:11.000000 jaxlie-1.4.0/jaxlie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-06 06:03:11.000000 jaxlie-1.4.0/jaxlie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 06:03:11.000000 jaxlie-1.4.0/jaxlie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-06 06:03:11.000000 jaxlie-1.4.0/jaxlie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 06:03:11.000000 jaxlie-1.4.0/jaxlie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 06:03:11.449120 jaxlie-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-06 06:03:03.000000 jaxlie-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 06:03:11.449120 jaxlie-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-05-06 06:03:03.000000 jaxlie-1.4.0/tests/test_autodiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-06 06:03:03.000000 jaxlie-1.4.0/tests/test_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-06 06:03:03.000000 jaxlie-1.4.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-06 06:03:03.000000 jaxlie-1.4.0/tests/test_group_axioms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-06 06:03:03.000000 jaxlie-1.4.0/tests/test_manifold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-05-06 06:03:03.000000 jaxlie-1.4.0/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-06 06:03:03.000000 jaxlie-1.4.0/tests/test_serialization.py
```

### Comparing `jaxlie-1.3.4/LICENSE` & `jaxlie-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxlie-1.3.4/PKG-INFO` & `jaxlie-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxlie
-Version: 1.3.4
+Version: 1.4.0
 Summary: Matrix Lie groups in JAX
 Home-page: http://github.com/brentyi/jaxlie
 Author: brentyi
 Author-email: brentyi@berkeley.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jax>=0.3.18
 Requires-Dist: jax_dataclasses>=1.4.4
 Requires-Dist: numpy
+Requires-Dist: typing_extensions>=4.0.0
 Requires-Dist: tyro
 Provides-Extra: testing
 Requires-Dist: mypy; extra == "testing"
 Requires-Dist: jax!=0.3.19; extra == "testing"
 Requires-Dist: flax; extra == "testing"
 Requires-Dist: hypothesis[numpy]; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
@@ -85,14 +86,15 @@
   **`identity()`**, **`from_matrix()`**, and **`as_matrix()`** operations. (see
   [./examples/se3_example.py](./examples/se3_basics.py))
 - Helpers for optimization on manifolds (see
   [./examples/se3_optimization.py](./examples/se3_optimization.py),
   <code>jaxlie.<strong>manifold.\*</strong></code>).
 - Compatibility with standard JAX function transformations. (see
   [./examples/vmap_example.py](./examples/vmap_example.py))
+- Broadcasting for leading axes.
 - (Un)flattening as pytree nodes.
 - Serialization using [flax](https://github.com/google/flax).
 
 We also implement various common utilities for things like uniform random
 sampling (**`sample_uniform()`**) and converting from/to Euler angles (in the
 `SO3` class).
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 2.1 Name: jaxlie Version: 1.3.4 Summary: Matrix Lie groups in
+Metadata-Version: 2.1 Name: jaxlie Version: 1.4.0 Summary: Matrix Lie groups in
 JAX Home-page: http://github.com/brentyi/jaxlie Author: brentyi Author-email:
 brentyi@berkeley.edu License: MIT Classifier: Programming Language :: Python ::
 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: jax>=0.3.18 Requires-Dist:
-jax_dataclasses>=1.4.4 Requires-Dist: numpy Requires-Dist: tyro Provides-Extra:
-testing Requires-Dist: mypy; extra == "testing" Requires-Dist: jax!=0.3.19;
-extra == "testing" Requires-Dist: flax; extra == "testing" Requires-Dist:
-hypothesis[numpy]; extra == "testing" Requires-Dist: pytest; extra == "testing"
-Requires-Dist: pytest-xdist[psutil]; extra == "testing" Requires-Dist: pytest-
-cov; extra == "testing" # jaxlie ![build](https://github.com/brentyi/jaxlie/
-workflows/build/badge.svg) ![mypy](https://github.com/brentyi/jaxlie/workflows/
-mypy/badge.svg?branch=master) ![lint](https://github.com/brentyi/jaxlie/
-workflows/lint/badge.svg) [![codecov](https://codecov.io/gh/brentyi/jaxlie/
-branch/master/graph/badge.svg)](https://codecov.io/gh/brentyi/jaxlie) [!
-[pypi_dowlnoads](https://pepy.tech/badge/jaxlie)](https://pypi.org/project/
-jaxlie) **[ [API reference](https://brentyi.github.io/jaxlie) ]** **[ [PyPI]
-(https://pypi.org/project/jaxlie/) ]** `jaxlie` is a library containing
-implementations of Lie groups commonly used for rigid body transformations,
-targeted at computer vision & robotics applications written in JAX. Heavily
-inspired by the C++ library [Sophus](https://github.com/strasdat/Sophus). We
-implement Lie groups as high-level (data)classes:
+jax_dataclasses>=1.4.4 Requires-Dist: numpy Requires-Dist:
+typing_extensions>=4.0.0 Requires-Dist: tyro Provides-Extra: testing Requires-
+Dist: mypy; extra == "testing" Requires-Dist: jax!=0.3.19; extra == "testing"
+Requires-Dist: flax; extra == "testing" Requires-Dist: hypothesis[numpy]; extra
+== "testing" Requires-Dist: pytest; extra == "testing" Requires-Dist: pytest-
+xdist[psutil]; extra == "testing" Requires-Dist: pytest-cov; extra == "testing"
+# jaxlie ![build](https://github.com/brentyi/jaxlie/workflows/build/badge.svg)
+![mypy](https://github.com/brentyi/jaxlie/workflows/mypy/
+badge.svg?branch=master) ![lint](https://github.com/brentyi/jaxlie/workflows/
+lint/badge.svg) [![codecov](https://codecov.io/gh/brentyi/jaxlie/branch/master/
+graph/badge.svg)](https://codecov.io/gh/brentyi/jaxlie) [![pypi_dowlnoads]
+(https://pepy.tech/badge/jaxlie)](https://pypi.org/project/jaxlie) **[ [API
+reference](https://brentyi.github.io/jaxlie) ]** **[ [PyPI](https://pypi.org/
+project/jaxlie/) ]** `jaxlie` is a library containing implementations of Lie
+groups commonly used for rigid body transformations, targeted at computer
+vision & robotics applications written in JAX. Heavily inspired by the C++
+library [Sophus](https://github.com/strasdat/Sophus). We implement Lie groups
+as high-level (data)classes:
 GGrroouupp      DDeessccrriippttiioonn                    PPaarraammeetteerriizzaattiioonn
 jaxlie.SSOO22 Rotations in 2D.               ((rreeaall,, iimmaaggiinnaarryy)):: unit complex (â
                                           S1)
 jaxlie.SSEE22 Proper rigid transforms in 2D. ((rreeaall,, iimmaaggiinnaarryy,, xx,, yy)):: unit complex
                                           & translation
 jaxlie.SSOO33 Rotations in 3D.               ((qqww,, qqxx,, qqyy,, qqzz)):: wxyz quaternion
                                           (â S3)
@@ -35,26 +36,26 @@
 Where each group supports: - Forward- and reverse-mode AD-friendly **`exp()`**,
 **`log()`**, **`adjoint()`**, **`apply()`**, **`multiply()`**, **`inverse()`**,
 **`identity()`**, **`from_matrix()`**, and **`as_matrix()`** operations. (see
 [./examples/se3_example.py](./examples/se3_basics.py)) - Helpers for
 optimization on manifolds (see [./examples/se3_optimization.py](./examples/
 se3_optimization.py), jaxlie.mmaanniiffoolldd..\\**). - Compatibility with standard JAX
 function transformations. (see [./examples/vmap_example.py](./examples/
-vmap_example.py)) - (Un)flattening as pytree nodes. - Serialization using
-[flax](https://github.com/google/flax). We also implement various common
-utilities for things like uniform random sampling (**`sample_uniform()`**) and
-converting from/to Euler angles (in the `SO3` class). --- ### Install (Python
->=3.7) ```bash # Python 3.6 releases also exist, but are no longer being
-updated. pip install jaxlie ``` --- ### In the wild - [jaxfg](https://
-github.com/brentyi/jaxfg) applies `jaxlie` to nonlinear least squares problems
-with block-sparse structure. (for pose graph optimization, bundle adjustment,
-etc) - [tensorf-jax](https://github.com/brentyi/tensorf-jax) is an unofficial
-implementation of [Tensorial Radiance Fields (Chen et al, ECCV 2022)](https://
-apchenstu.github.io/TensoRF/) using `jaxlie`. ![Render of a lego](https://
-github.com/brentyi/tensorf-jax/raw/main/lego_render.gif) --- ### Misc `jaxlie`
-was originally written for our IROS 2021 paper ([link](https://github.com/
-brentyi/dfgo)). If it's useful for you, you're welcome to cite: ```
-@inproceedings{yi2021iros, author={Brent Yi and Michelle Lee and Alina Kloss
-and Roberto Mart\'in-Mart\'in and Jeannette Bohg}, title = {Differentiable
-Factor Graph Optimization for Learning Smoothers}, year = 2021, BOOKTITLE =
-{2021 IEEE/RSJ International Conference on Intelligent Robots and Systems
-(IROS)} } ```
+vmap_example.py)) - Broadcasting for leading axes. - (Un)flattening as pytree
+nodes. - Serialization using [flax](https://github.com/google/flax). We also
+implement various common utilities for things like uniform random sampling
+(**`sample_uniform()`**) and converting from/to Euler angles (in the `SO3`
+class). --- ### Install (Python >=3.7) ```bash # Python 3.6 releases also
+exist, but are no longer being updated. pip install jaxlie ``` --- ### In the
+wild - [jaxfg](https://github.com/brentyi/jaxfg) applies `jaxlie` to nonlinear
+least squares problems with block-sparse structure. (for pose graph
+optimization, bundle adjustment, etc) - [tensorf-jax](https://github.com/
+brentyi/tensorf-jax) is an unofficial implementation of [Tensorial Radiance
+Fields (Chen et al, ECCV 2022)](https://apchenstu.github.io/TensoRF/) using
+`jaxlie`. ![Render of a lego](https://github.com/brentyi/tensorf-jax/raw/main/
+lego_render.gif) --- ### Misc `jaxlie` was originally written for our IROS 2021
+paper ([link](https://github.com/brentyi/dfgo)). If it's useful for you, you're
+welcome to cite: ``` @inproceedings{yi2021iros, author={Brent Yi and Michelle
+Lee and Alina Kloss and Roberto Mart\'in-Mart\'in and Jeannette Bohg}, title =
+{Differentiable Factor Graph Optimization for Learning Smoothers}, year = 2021,
+BOOKTITLE = {2021 IEEE/RSJ International Conference on Intelligent Robots and
+Systems (IROS)} } ```
```

### Comparing `jaxlie-1.3.4/README.md` & `jaxlie-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
   **`identity()`**, **`from_matrix()`**, and **`as_matrix()`** operations. (see
   [./examples/se3_example.py](./examples/se3_basics.py))
 - Helpers for optimization on manifolds (see
   [./examples/se3_optimization.py](./examples/se3_optimization.py),
   <code>jaxlie.<strong>manifold.\*</strong></code>).
 - Compatibility with standard JAX function transformations. (see
   [./examples/vmap_example.py](./examples/vmap_example.py))
+- Broadcasting for leading axes.
 - (Un)flattening as pytree nodes.
 - Serialization using [flax](https://github.com/google/flax).
 
 We also implement various common utilities for things like uniform random
 sampling (**`sample_uniform()`**) and converting from/to Euler angles (in the
 `SO3` class).
```

#### html2text {}

```diff
@@ -22,26 +22,26 @@
 Where each group supports: - Forward- and reverse-mode AD-friendly **`exp()`**,
 **`log()`**, **`adjoint()`**, **`apply()`**, **`multiply()`**, **`inverse()`**,
 **`identity()`**, **`from_matrix()`**, and **`as_matrix()`** operations. (see
 [./examples/se3_example.py](./examples/se3_basics.py)) - Helpers for
 optimization on manifolds (see [./examples/se3_optimization.py](./examples/
 se3_optimization.py), jaxlie.mmaanniiffoolldd..\\**). - Compatibility with standard JAX
 function transformations. (see [./examples/vmap_example.py](./examples/
-vmap_example.py)) - (Un)flattening as pytree nodes. - Serialization using
-[flax](https://github.com/google/flax). We also implement various common
-utilities for things like uniform random sampling (**`sample_uniform()`**) and
-converting from/to Euler angles (in the `SO3` class). --- ### Install (Python
->=3.7) ```bash # Python 3.6 releases also exist, but are no longer being
-updated. pip install jaxlie ``` --- ### In the wild - [jaxfg](https://
-github.com/brentyi/jaxfg) applies `jaxlie` to nonlinear least squares problems
-with block-sparse structure. (for pose graph optimization, bundle adjustment,
-etc) - [tensorf-jax](https://github.com/brentyi/tensorf-jax) is an unofficial
-implementation of [Tensorial Radiance Fields (Chen et al, ECCV 2022)](https://
-apchenstu.github.io/TensoRF/) using `jaxlie`. ![Render of a lego](https://
-github.com/brentyi/tensorf-jax/raw/main/lego_render.gif) --- ### Misc `jaxlie`
-was originally written for our IROS 2021 paper ([link](https://github.com/
-brentyi/dfgo)). If it's useful for you, you're welcome to cite: ```
-@inproceedings{yi2021iros, author={Brent Yi and Michelle Lee and Alina Kloss
-and Roberto Mart\'in-Mart\'in and Jeannette Bohg}, title = {Differentiable
-Factor Graph Optimization for Learning Smoothers}, year = 2021, BOOKTITLE =
-{2021 IEEE/RSJ International Conference on Intelligent Robots and Systems
-(IROS)} } ```
+vmap_example.py)) - Broadcasting for leading axes. - (Un)flattening as pytree
+nodes. - Serialization using [flax](https://github.com/google/flax). We also
+implement various common utilities for things like uniform random sampling
+(**`sample_uniform()`**) and converting from/to Euler angles (in the `SO3`
+class). --- ### Install (Python >=3.7) ```bash # Python 3.6 releases also
+exist, but are no longer being updated. pip install jaxlie ``` --- ### In the
+wild - [jaxfg](https://github.com/brentyi/jaxfg) applies `jaxlie` to nonlinear
+least squares problems with block-sparse structure. (for pose graph
+optimization, bundle adjustment, etc) - [tensorf-jax](https://github.com/
+brentyi/tensorf-jax) is an unofficial implementation of [Tensorial Radiance
+Fields (Chen et al, ECCV 2022)](https://apchenstu.github.io/TensoRF/) using
+`jaxlie`. ![Render of a lego](https://github.com/brentyi/tensorf-jax/raw/main/
+lego_render.gif) --- ### Misc `jaxlie` was originally written for our IROS 2021
+paper ([link](https://github.com/brentyi/dfgo)). If it's useful for you, you're
+welcome to cite: ``` @inproceedings{yi2021iros, author={Brent Yi and Michelle
+Lee and Alina Kloss and Roberto Mart\'in-Mart\'in and Jeannette Bohg}, title =
+{Differentiable Factor Graph Optimization for Learning Smoothers}, year = 2021,
+BOOKTITLE = {2021 IEEE/RSJ International Conference on Intelligent Robots and
+Systems (IROS)} } ```
```

### Comparing `jaxlie-1.3.4/jaxlie/_base.py` & `jaxlie-1.4.0/jaxlie/_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import abc
-from typing import ClassVar, Generic, Tuple, Type, TypeVar, Union, overload
+from typing import ClassVar, Generic, Tuple, TypeVar, Union, overload
 
 import jax
 import numpy as onp
-from typing_extensions import final, override
+from jax import numpy as jnp
+from typing_extensions import Self, final, override
 
 from . import hints
 
-GroupType = TypeVar("GroupType", bound="MatrixLieGroup")
-SEGroupType = TypeVar("SEGroupType", bound="SEBase")
-
 
 class MatrixLieGroup(abc.ABC):
     """Interface definition for matrix Lie groups."""
 
     # Class properties.
     # > These will be set in `_utils.register_lie_group()`.
 
@@ -40,24 +38,20 @@
     ):
         """Construct a group object from its underlying parameters."""
         raise NotImplementedError()
 
     # Shared implementations.
 
     @overload
-    def __matmul__(self: GroupType, other: GroupType) -> GroupType:
-        ...
+    def __matmul__(self, other: Self) -> Self: ...
 
     @overload
-    def __matmul__(self, other: hints.Array) -> jax.Array:
-        ...
+    def __matmul__(self, other: hints.Array) -> jax.Array: ...
 
-    def __matmul__(
-        self: GroupType, other: Union[GroupType, hints.Array]
-    ) -> Union[GroupType, jax.Array]:
+    def __matmul__(self, other: Union[Self, hints.Array]) -> Union[Self, jax.Array]:
         """Overload for the `@` operator.
 
         Switches between the group action (`.apply()`) and multiplication
         (`.multiply()`) based on the type of `other`.
         """
         if isinstance(other, (onp.ndarray, jax.Array)):
             return self.apply(target=other)
@@ -67,24 +61,27 @@
         else:
             assert False, f"Invalid argument type for `@` operator: {type(other)}"
 
     # Factory.
 
     @classmethod
     @abc.abstractmethod
-    def identity(cls: Type[GroupType]) -> GroupType:
+    def identity(cls, batch_axes: Tuple[int, ...] = ()) -> Self:
         """Returns identity element.
 
+        Args:
+            batch_axes: Any leading batch axes for the output transform.
+
         Returns:
             Identity element.
         """
 
     @classmethod
     @abc.abstractmethod
-    def from_matrix(cls: Type[GroupType], matrix: hints.Array) -> GroupType:
+    def from_matrix(cls, matrix: hints.Array) -> Self:
         """Get group member from matrix representation.
 
         Args:
             matrix: Matrix representaiton.
 
         Returns:
             Group member.
@@ -110,24 +107,24 @@
             target: Point to transform.
 
         Returns:
             Transformed point.
         """
 
     @abc.abstractmethod
-    def multiply(self: GroupType, other: GroupType) -> GroupType:
+    def multiply(self, other: Self) -> Self:
         """Composes this transformation with another.
 
         Returns:
             self @ other
         """
 
     @classmethod
     @abc.abstractmethod
-    def exp(cls: Type[GroupType], tangent: hints.Array) -> GroupType:
+    def exp(cls, tangent: hints.Array) -> Self:
         """Computes `expm(wedge(tangent))`.
 
         Args:
             tangent: Tangent vector to take the exponential of.
 
         Returns:
             Output.
@@ -155,49 +152,50 @@
         across different reference frames.
 
         Returns:
             Output. Shape should be `(tangent_dim, tangent_dim)`.
         """
 
     @abc.abstractmethod
-    def inverse(self: GroupType) -> GroupType:
+    def inverse(self) -> Self:
         """Computes the inverse of our transform.
 
         Returns:
             Output.
         """
 
     @abc.abstractmethod
-    def normalize(self: GroupType) -> GroupType:
+    def normalize(self) -> Self:
         """Normalize/projects values and returns.
 
         Returns:
-            GroupType: Normalized group member.
+            Normalized group member.
         """
 
     @classmethod
     @abc.abstractmethod
-    def sample_uniform(cls: Type[GroupType], key: jax.Array) -> GroupType:
+    def sample_uniform(cls, key: jax.Array, batch_axes: Tuple[int, ...] = ()) -> Self:
         """Draw a uniform sample from the group. Translations (if applicable) are in the
         range [-1, 1].
 
         Args:
             key: PRNG key, as returned by `jax.random.PRNGKey()`.
+            batch_axes: Any leading batch axes for the output transforms. Each
+                sampled transform will be different.
 
         Returns:
             Sampled group member.
         """
 
-    @abc.abstractmethod
+    @final
     def get_batch_axes(self) -> Tuple[int, ...]:
         """Return any leading batch axes in contained parameters. If an array of shape
         `(100, 4)` is placed in the wxyz field of an SO3 object, for example, this will
-        return `(100,)`.
-
-        This should generally be implemented by `jdc.EnforcedAnnotationsMixin`."""
+        return `(100,)`."""
+        return self.parameters().shape[:-1]
 
 
 class SOBase(MatrixLieGroup):
     """Base class for special orthogonal groups."""
 
 
 ContainedSOType = TypeVar("ContainedSOType", bound=SOBase)
@@ -211,34 +209,37 @@
     """
 
     # SE-specific interface.
 
     @classmethod
     @abc.abstractmethod
     def from_rotation_and_translation(
-        cls: Type[SEGroupType],
+        cls,
         rotation: ContainedSOType,
         translation: hints.Array,
-    ) -> SEGroupType:
+    ) -> Self:
         """Construct a rigid transform from a rotation and a translation.
 
         Args:
             rotation: Rotation term.
             translation: translation term.
 
         Returns:
             Constructed transformation.
         """
 
     @final
     @classmethod
-    def from_rotation(cls: Type[SEGroupType], rotation: ContainedSOType) -> SEGroupType:
+    def from_rotation(cls, rotation: ContainedSOType) -> Self:
         return cls.from_rotation_and_translation(
             rotation=rotation,
-            translation=onp.zeros(cls.space_dim, dtype=rotation.parameters().dtype),
+            translation=jnp.zeros(
+                (*rotation.get_batch_axes(), cls.space_dim),
+                dtype=rotation.parameters().dtype,
+            ),
         )
 
     @abc.abstractmethod
     def rotation(self) -> ContainedSOType:
         """Returns a transform's rotation term."""
 
     @abc.abstractmethod
@@ -250,29 +251,29 @@
     @final
     @override
     def apply(self, target: hints.Array) -> jax.Array:
         return self.rotation() @ target + self.translation()  # type: ignore
 
     @final
     @override
-    def multiply(self: SEGroupType, other: SEGroupType) -> SEGroupType:
+    def multiply(self, other: Self) -> Self:
         return type(self).from_rotation_and_translation(
             rotation=self.rotation() @ other.rotation(),
             translation=(self.rotation() @ other.translation()) + self.translation(),
         )
 
     @final
     @override
-    def inverse(self: SEGroupType) -> SEGroupType:
+    def inverse(self) -> Self:
         R_inv = self.rotation().inverse()
         return type(self).from_rotation_and_translation(
             rotation=R_inv,
             translation=-(R_inv @ self.translation()),
         )
 
     @final
     @override
-    def normalize(self: SEGroupType) -> SEGroupType:
+    def normalize(self) -> Self:
         return type(self).from_rotation_and_translation(
             rotation=self.rotation().normalize(),
             translation=self.translation(),
         )
```

### Comparing `jaxlie-1.3.4/jaxlie/_se2.py` & `jaxlie-1.4.0/jaxlie/_se2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-from typing import cast
+from typing import Tuple, cast
 
 import jax
 import jax_dataclasses as jdc
 from jax import numpy as jnp
-from typing_extensions import Annotated, override
+from typing_extensions import override
 
 from . import _base, hints
 from ._so2 import SO2
-from .utils import get_epsilon, register_lie_group
+from .utils import broadcast_leading_axes, get_epsilon, register_lie_group
 
 
 @register_lie_group(
     matrix_dim=3,
     parameters_dim=4,
     tangent_dim=3,
     space_dim=2,
 )
 @jdc.pytree_dataclass
-class SE2(jdc.EnforcedAnnotationsMixin, _base.SEBase[SO2]):
-    """Special Euclidean group for proper rigid transforms in 2D.
+class SE2(_base.SEBase[SO2]):
+    """Special Euclidean group for proper rigid transforms in 2D. Broadcasting
+    rules are the same as for numpy.
 
     Internal parameterization is `(cos, sin, x, y)`. Tangent parameterization is `(vx,
     vy, omega)`.
     """
 
     # SE2-specific.
 
-    unit_complex_xy: Annotated[
-        jax.Array,
-        (..., 4),  # Shape.
-        jnp.floating,  # Data-type.
-    ]
-    """Internal parameters. `(cos, sin, x, y)`."""
+    unit_complex_xy: jax.Array
+    """Internal parameters. `(cos, sin, x, y)`. Shape should be `(*, 3)`."""
 
     @override
     def __repr__(self) -> str:
         unit_complex = jnp.round(self.unit_complex_xy[..., :2], 5)
         xy = jnp.round(self.unit_complex_xy[..., 2:], 5)
         return f"{self.__class__.__name__}(unit_complex={unit_complex}, xy={xy})"
 
@@ -43,93 +40,109 @@
     def from_xy_theta(x: hints.Scalar, y: hints.Scalar, theta: hints.Scalar) -> "SE2":
         """Construct a transformation from standard 2D pose parameters.
 
         Note that this is not the same as integrating over a length-3 twist.
         """
         cos = jnp.cos(theta)
         sin = jnp.sin(theta)
-        return SE2(unit_complex_xy=jnp.array([cos, sin, x, y]))
+        return SE2(unit_complex_xy=jnp.stack([cos, sin, x, y], axis=-1))
 
     # SE-specific.
 
-    @staticmethod
+    @classmethod
     @override
     def from_rotation_and_translation(
+        cls,
         rotation: SO2,
         translation: hints.Array,
     ) -> "SE2":
-        assert translation.shape == (2,)
+        assert translation.shape[-1:] == (2,)
+        rotation, translation = broadcast_leading_axes((rotation, translation))
         return SE2(
-            unit_complex_xy=jnp.concatenate([rotation.unit_complex, translation])
+            unit_complex_xy=jnp.concatenate(
+                [rotation.unit_complex, translation], axis=-1
+            )
         )
 
     @override
     def rotation(self) -> SO2:
         return SO2(unit_complex=self.unit_complex_xy[..., :2])
 
     @override
     def translation(self) -> jax.Array:
         return self.unit_complex_xy[..., 2:]
 
     # Factory.
 
-    @staticmethod
+    @classmethod
     @override
-    def identity() -> "SE2":
-        return SE2(unit_complex_xy=jnp.array([1.0, 0.0, 0.0, 0.0]))
+    def identity(cls, batch_axes: jdc.Static[Tuple[int, ...]] = ()) -> "SE2":
+        return SE2(
+            unit_complex_xy=jnp.broadcast_to(
+                jnp.array([1.0, 0.0, 0.0, 0.0]), (*batch_axes, 4)
+            )
+        )
 
-    @staticmethod
+    @classmethod
     @override
-    def from_matrix(matrix: hints.Array) -> "SE2":
-        assert matrix.shape == (3, 3)
+    def from_matrix(cls, matrix: hints.Array) -> "SE2":
+        assert matrix.shape[-2:] == (3, 3)
         # Currently assumes bottom row is [0, 0, 1].
         return SE2.from_rotation_and_translation(
-            rotation=SO2.from_matrix(matrix[:2, :2]),
-            translation=matrix[:2, 2],
+            rotation=SO2.from_matrix(matrix[..., :2, :2]),
+            translation=matrix[..., :2, 2],
         )
 
     # Accessors.
 
     @override
     def parameters(self) -> jax.Array:
         return self.unit_complex_xy
 
     @override
     def as_matrix(self) -> jax.Array:
-        cos, sin, x, y = self.unit_complex_xy
-        return jnp.array(
+        cos, sin, x, y = jnp.moveaxis(self.unit_complex_xy, -1, 0)
+        out = jnp.stack(
             [
-                [cos, -sin, x],
-                [sin, cos, y],
-                [0.0, 0.0, 1.0],
-            ]
-        )
+                cos,
+                -sin,
+                x,
+                sin,
+                cos,
+                y,
+                jnp.zeros_like(x),
+                jnp.zeros_like(x),
+                jnp.ones_like(x),
+            ],
+            axis=-1,
+        ).reshape((*self.get_batch_axes(), 3, 3))
+        return out
 
     # Operations.
 
-    @staticmethod
+    @classmethod
     @override
-    def exp(tangent: hints.Array) -> "SE2":
+    def exp(cls, tangent: hints.Array) -> "SE2":
         # Reference:
         # > https://github.com/strasdat/Sophus/blob/a0fe89a323e20c42d3cecb590937eb7a06b8343a/sophus/se2.hpp#L558
         # Also see:
         # > http://ethaneade.com/lie.pdf
 
-        assert tangent.shape == (3,)
+        assert tangent.shape[-1:] == (3,)
 
-        theta = tangent[2]
+        theta = tangent[..., 2]
         use_taylor = jnp.abs(theta) < get_epsilon(tangent.dtype)
 
         # Shim to avoid NaNs in jnp.where branches, which cause failures for
         # reverse-mode AD.
         safe_theta = cast(
             jax.Array,
             jnp.where(
                 use_taylor,
-                1.0,  # Any non-zero value should do here.
+                jnp.ones_like(theta),  # Any non-zero value should do here.
                 theta,
             ),
         )
 
         theta_sq = theta**2
         sin_over_theta = cast(
             jax.Array,
@@ -144,79 +157,106 @@
             jnp.where(
                 use_taylor,
                 0.5 * theta - theta * theta_sq / 24.0,
                 (1.0 - jnp.cos(safe_theta)) / safe_theta,
             ),
         )
 
-        V = jnp.array(
+        V = jnp.stack(
             [
-                [sin_over_theta, -one_minus_cos_over_theta],
-                [one_minus_cos_over_theta, sin_over_theta],
-            ]
-        )
+                sin_over_theta,
+                -one_minus_cos_over_theta,
+                one_minus_cos_over_theta,
+                sin_over_theta,
+            ],
+            axis=-1,
+        ).reshape((*tangent.shape[:-1], 2, 2))
         return SE2.from_rotation_and_translation(
             rotation=SO2.from_radians(theta),
-            translation=V @ tangent[:2],
+            translation=jnp.einsum("...ij,...j->...i", V, tangent[..., :2]),
         )
 
     @override
     def log(self) -> jax.Array:
         # Reference:
         # > https://github.com/strasdat/Sophus/blob/a0fe89a323e20c42d3cecb590937eb7a06b8343a/sophus/se2.hpp#L160
         # Also see:
         # > http://ethaneade.com/lie.pdf
 
-        theta = self.rotation().log()[0]
+        theta = self.rotation().log()[..., 0]
 
         cos = jnp.cos(theta)
         cos_minus_one = cos - 1.0
         half_theta = theta / 2.0
         use_taylor = jnp.abs(cos_minus_one) < get_epsilon(theta.dtype)
 
         # Shim to avoid NaNs in jnp.where branches, which cause failures for
         # reverse-mode AD.
         safe_cos_minus_one = jnp.where(
             use_taylor,
-            1.0,  # Any non-zero value should do here.
+            jnp.ones_like(cos_minus_one),  # Any non-zero value should do here.
             cos_minus_one,
         )
 
         half_theta_over_tan_half_theta = jnp.where(
             use_taylor,
             # Taylor approximation.
             1.0 - theta**2 / 12.0,
             # Default.
             -(half_theta * jnp.sin(theta)) / safe_cos_minus_one,
         )
 
-        V_inv = jnp.array(
+        V_inv = jnp.stack(
             [
-                [half_theta_over_tan_half_theta, half_theta],
-                [-half_theta, half_theta_over_tan_half_theta],
-            ]
-        )
+                half_theta_over_tan_half_theta,
+                half_theta,
+                -half_theta,
+                half_theta_over_tan_half_theta,
+            ],
+            axis=-1,
+        ).reshape((*theta.shape, 2, 2))
 
-        tangent = jnp.concatenate([V_inv @ self.translation(), theta[None]])
+        tangent = jnp.concatenate(
+            [
+                jnp.einsum("...ij,...j->...i", V_inv, self.translation()),
+                theta[..., None],
+            ],
+            axis=-1,
+        )
         return tangent
 
     @override
     def adjoint(self: "SE2") -> jax.Array:
-        cos, sin, x, y = self.unit_complex_xy
-        return jnp.array(
+        cos, sin, x, y = jnp.moveaxis(self.unit_complex_xy, -1, 0)
+        return jnp.stack(
             [
-                [cos, -sin, y],
-                [sin, cos, -x],
-                [0.0, 0.0, 1.0],
-            ]
-        )
+                cos,
+                -sin,
+                y,
+                sin,
+                cos,
+                -x,
+                jnp.zeros_like(x),
+                jnp.zeros_like(x),
+                jnp.ones_like(x),
+            ],
+            axis=-1,
+        ).reshape((*self.get_batch_axes(), 3, 3))
 
-    @staticmethod
+    @classmethod
     @override
-    def sample_uniform(key: jax.Array) -> "SE2":
+    def sample_uniform(
+        cls, key: jax.Array, batch_axes: jdc.Static[Tuple[int, ...]] = ()
+    ) -> "SE2":
         key0, key1 = jax.random.split(key)
         return SE2.from_rotation_and_translation(
-            rotation=SO2.sample_uniform(key0),
+            rotation=SO2.sample_uniform(key0, batch_axes=batch_axes),
             translation=jax.random.uniform(
-                key=key1, shape=(2,), minval=-1.0, maxval=1.0
+                key=key1,
+                shape=(
+                    *batch_axes,
+                    2,
+                ),
+                minval=-1.0,
+                maxval=1.0,
             ),
         )
```

### Comparing `jaxlie-1.3.4/jaxlie/_so3.py` & `jaxlie-1.4.0/jaxlie/_so3.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 from __future__ import annotations
 
+from typing import Tuple
+
 import jax
 import jax_dataclasses as jdc
 from jax import numpy as jnp
-from typing_extensions import Annotated, override
+from typing_extensions import override
 
 from . import _base, hints
-from .utils import get_epsilon, register_lie_group
+from .utils import broadcast_leading_axes, get_epsilon, register_lie_group
 
 
 @register_lie_group(
     matrix_dim=3,
     parameters_dim=4,
     tangent_dim=3,
     space_dim=3,
 )
 @jdc.pytree_dataclass
-class SO3(jdc.EnforcedAnnotationsMixin, _base.SOBase):
-    """Special orthogonal group for 3D rotations.
+class SO3(_base.SOBase):
+    """Special orthogonal group for 3D rotations. Broadcasting rules are the same as
+    for numpy.
 
     Internal parameterization is `(qw, qx, qy, qz)`. Tangent parameterization is
     `(omega_x, omega_y, omega_z)`.
     """
 
-    # SO3-specific.
-
-    wxyz: Annotated[
-        jax.Array,
-        (..., 4),  # Shape.
-        jnp.floating,  # Data-type.
-    ]
-    """Internal parameters. `(w, x, y, z)` quaternion."""
+    wxyz: jax.Array
+    """Internal parameters. `(w, x, y, z)` quaternion. Shape should be `(*, 4)`."""
 
     @override
     def __repr__(self) -> str:
         wxyz = jnp.round(self.wxyz, 5)
         return f"{self.__class__.__name__}(wxyz={wxyz})"
 
     @staticmethod
@@ -43,39 +40,42 @@
 
         Args:
             angle: X rotation, in radians.
 
         Returns:
             Output.
         """
-        return SO3.exp(jnp.array([theta, 0.0, 0.0]))
+        zeros = jnp.zeros_like(theta)
+        return SO3.exp(jnp.stack([theta, zeros, zeros], axis=-1))
 
     @staticmethod
     def from_y_radians(theta: hints.Scalar) -> SO3:
         """Generates a y-axis rotation.
 
         Args:
             angle: Y rotation, in radians.
 
         Returns:
             Output.
         """
-        return SO3.exp(jnp.array([0.0, theta, 0.0]))
+        zeros = jnp.zeros_like(theta)
+        return SO3.exp(jnp.stack([zeros, theta, zeros], axis=-1))
 
     @staticmethod
     def from_z_radians(theta: hints.Scalar) -> SO3:
         """Generates a z-axis rotation.
 
         Args:
             angle: Z rotation, in radians.
 
         Returns:
             Output.
         """
-        return SO3.exp(jnp.array([0.0, 0.0, theta]))
+        zeros = jnp.zeros_like(theta)
+        return SO3.exp(jnp.stack([zeros, zeros, theta], axis=-1))
 
     @staticmethod
     def from_rpy_radians(
         roll: hints.Scalar,
         pitch: hints.Scalar,
         yaw: hints.Scalar,
     ) -> SO3:
@@ -100,25 +100,25 @@
     def from_quaternion_xyzw(xyzw: hints.Array) -> SO3:
         """Construct a rotation from an `xyzw` quaternion.
 
         Note that `wxyz` quaternions can be constructed using the default dataclass
         constructor.
 
         Args:
-            xyzw: xyzw quaternion. Shape should be (4,).
+            xyzw: xyzw quaternion. Shape should be (*, 4).
 
         Returns:
             Output.
         """
-        assert xyzw.shape == (4,)
-        return SO3(jnp.roll(xyzw, shift=1))
+        assert xyzw.shape[-1:] == (4,)
+        return SO3(jnp.roll(xyzw, axis=-1, shift=1))
 
     def as_quaternion_xyzw(self) -> jax.Array:
         """Grab parameters as xyzw quaternion."""
-        return jnp.roll(self.wxyz, shift=-1)
+        return jnp.roll(self.wxyz, axis=-1, shift=-1)
 
     def as_rpy_radians(self) -> hints.RollPitchYaw:
         """Computes roll, pitch, and yaw angles. Uses the ZYX mobile robot convention.
 
         Returns:
             Named tuple containing Euler angles in radians.
         """
@@ -131,121 +131,127 @@
     def compute_roll_radians(self) -> jax.Array:
         """Compute roll angle. Uses the ZYX mobile robot convention.
 
         Returns:
             Euler angle in radians.
         """
         # https://en.wikipedia.org/wiki/Conversion_between_quaternions_and_Euler_angles#Quaternion_to_Euler_angles_conversion
-        q0, q1, q2, q3 = self.wxyz
+        q0, q1, q2, q3 = jnp.moveaxis(self.wxyz, -1, 0)
         return jnp.arctan2(2 * (q0 * q1 + q2 * q3), 1 - 2 * (q1**2 + q2**2))
 
     def compute_pitch_radians(self) -> jax.Array:
         """Compute pitch angle. Uses the ZYX mobile robot convention.
 
         Returns:
             Euler angle in radians.
         """
         # https://en.wikipedia.org/wiki/Conversion_between_quaternions_and_Euler_angles#Quaternion_to_Euler_angles_conversion
-        q0, q1, q2, q3 = self.wxyz
+        q0, q1, q2, q3 = jnp.moveaxis(self.wxyz, -1, 0)
         return jnp.arcsin(2 * (q0 * q2 - q3 * q1))
 
     def compute_yaw_radians(self) -> jax.Array:
         """Compute yaw angle. Uses the ZYX mobile robot convention.
 
         Returns:
             Euler angle in radians.
         """
         # https://en.wikipedia.org/wiki/Conversion_between_quaternions_and_Euler_angles#Quaternion_to_Euler_angles_conversion
-        q0, q1, q2, q3 = self.wxyz
+        q0, q1, q2, q3 = jnp.moveaxis(self.wxyz, -1, 0)
         return jnp.arctan2(2 * (q0 * q3 + q1 * q2), 1 - 2 * (q2**2 + q3**2))
 
     # Factory.
 
-    @staticmethod
+    @classmethod
     @override
-    def identity() -> SO3:
-        return SO3(wxyz=jnp.array([1.0, 0.0, 0.0, 0.0]))
+    def identity(cls, batch_axes: jdc.Static[Tuple[int, ...]] = ()) -> SO3:
+        return SO3(
+            wxyz=jnp.broadcast_to(jnp.array([1.0, 0.0, 0.0, 0.0]), (*batch_axes, 4))
+        )
 
-    @staticmethod
+    @classmethod
     @override
-    def from_matrix(matrix: hints.Array) -> SO3:
-        assert matrix.shape == (3, 3)
+    def from_matrix(cls, matrix: hints.Array) -> SO3:
+        assert matrix.shape[-2:] == (3, 3)
 
         # Modified from:
         # > "Converting a Rotation Matrix to a Quaternion" from Mike Day
         # > https://d3cw3dd2w32x2b.cloudfront.net/wp-content/uploads/2015/01/matrix-to-quat.pdf
 
         def case0(m):
-            t = 1 + m[0, 0] - m[1, 1] - m[2, 2]
-            q = jnp.array(
+            t = 1 + m[..., 0, 0] - m[..., 1, 1] - m[..., 2, 2]
+            q = jnp.stack(
                 [
-                    m[2, 1] - m[1, 2],
+                    m[..., 2, 1] - m[..., 1, 2],
                     t,
-                    m[1, 0] + m[0, 1],
-                    m[0, 2] + m[2, 0],
-                ]
+                    m[..., 1, 0] + m[..., 0, 1],
+                    m[..., 0, 2] + m[..., 2, 0],
+                ],
+                axis=-1,
             )
             return t, q
 
         def case1(m):
-            t = 1 - m[0, 0] + m[1, 1] - m[2, 2]
-            q = jnp.array(
+            t = 1 - m[..., 0, 0] + m[..., 1, 1] - m[..., 2, 2]
+            q = jnp.stack(
                 [
-                    m[0, 2] - m[2, 0],
-                    m[1, 0] + m[0, 1],
+                    m[..., 0, 2] - m[..., 2, 0],
+                    m[..., 1, 0] + m[..., 0, 1],
                     t,
-                    m[2, 1] + m[1, 2],
-                ]
+                    m[..., 2, 1] + m[..., 1, 2],
+                ],
+                axis=-1,
             )
             return t, q
 
         def case2(m):
-            t = 1 - m[0, 0] - m[1, 1] + m[2, 2]
-            q = jnp.array(
+            t = 1 - m[..., 0, 0] - m[..., 1, 1] + m[..., 2, 2]
+            q = jnp.stack(
                 [
-                    m[1, 0] - m[0, 1],
-                    m[0, 2] + m[2, 0],
-                    m[2, 1] + m[1, 2],
+                    m[..., 1, 0] - m[..., 0, 1],
+                    m[..., 0, 2] + m[..., 2, 0],
+                    m[..., 2, 1] + m[..., 1, 2],
                     t,
-                ]
+                ],
+                axis=-1,
             )
             return t, q
 
         def case3(m):
-            t = 1 + m[0, 0] + m[1, 1] + m[2, 2]
-            q = jnp.array(
+            t = 1 + m[..., 0, 0] + m[..., 1, 1] + m[..., 2, 2]
+            q = jnp.stack(
                 [
                     t,
-                    m[2, 1] - m[1, 2],
-                    m[0, 2] - m[2, 0],
-                    m[1, 0] - m[0, 1],
-                ]
+                    m[..., 2, 1] - m[..., 1, 2],
+                    m[..., 0, 2] - m[..., 2, 0],
+                    m[..., 1, 0] - m[..., 0, 1],
+                ],
+                axis=-1,
             )
             return t, q
 
         # Compute four cases, then pick the most precise one.
         # Probably worth revisiting this!
         case0_t, case0_q = case0(matrix)
         case1_t, case1_q = case1(matrix)
         case2_t, case2_q = case2(matrix)
         case3_t, case3_q = case3(matrix)
 
-        cond0 = matrix[2, 2] < 0
-        cond1 = matrix[0, 0] > matrix[1, 1]
-        cond2 = matrix[0, 0] < -matrix[1, 1]
+        cond0 = matrix[..., 2, 2] < 0
+        cond1 = matrix[..., 0, 0] > matrix[..., 1, 1]
+        cond2 = matrix[..., 0, 0] < -matrix[..., 1, 1]
 
         t = jnp.where(
             cond0,
             jnp.where(cond1, case0_t, case1_t),
             jnp.where(cond2, case2_t, case3_t),
         )
         q = jnp.where(
-            cond0,
-            jnp.where(cond1, case0_q, case1_q),
-            jnp.where(cond2, case2_q, case3_q),
+            cond0[..., None],
+            jnp.where(cond1[..., None], case0_q, case1_q),
+            jnp.where(cond2[..., None], case2_q, case3_q),
         )
 
         # We can also choose to branch, but this is slower.
         # t, q = jax.lax.cond(
         #     matrix[2, 2] < 0,
         #     true_fun=lambda matrix: jax.lax.cond(
         #         matrix[0, 0] > matrix[1, 1],
@@ -258,78 +264,89 @@
         #         true_fun=case2,
         #         false_fun=case3,
         #         operand=matrix,
         #     ),
         #     operand=matrix,
         # )
 
-        return SO3(wxyz=q * 0.5 / jnp.sqrt(t))
+        return SO3(wxyz=q * 0.5 / jnp.sqrt(t[..., None]))
 
     # Accessors.
 
     @override
     def as_matrix(self) -> jax.Array:
-        norm = self.wxyz @ self.wxyz
-        q = self.wxyz * jnp.sqrt(2.0 / norm)
-        q = jnp.outer(q, q)
-        return jnp.array(
+        norm_sq = jnp.sum(jnp.square(self.wxyz), axis=-1, keepdims=True)
+        q = self.wxyz * jnp.sqrt(2.0 / norm_sq)  # (*, 4)
+        q_outer = jnp.einsum("...i,...j->...ij", q, q)  # (*, 4, 4)
+        return jnp.stack(
             [
-                [1.0 - q[2, 2] - q[3, 3], q[1, 2] - q[3, 0], q[1, 3] + q[2, 0]],
-                [q[1, 2] + q[3, 0], 1.0 - q[1, 1] - q[3, 3], q[2, 3] - q[1, 0]],
-                [q[1, 3] - q[2, 0], q[2, 3] + q[1, 0], 1.0 - q[1, 1] - q[2, 2]],
-            ]
-        )
+                1.0 - q_outer[..., 2, 2] - q_outer[..., 3, 3],
+                q_outer[..., 1, 2] - q_outer[..., 3, 0],
+                q_outer[..., 1, 3] + q_outer[..., 2, 0],
+                q_outer[..., 1, 2] + q_outer[..., 3, 0],
+                1.0 - q_outer[..., 1, 1] - q_outer[..., 3, 3],
+                q_outer[..., 2, 3] - q_outer[..., 1, 0],
+                q_outer[..., 1, 3] - q_outer[..., 2, 0],
+                q_outer[..., 2, 3] + q_outer[..., 1, 0],
+                1.0 - q_outer[..., 1, 1] - q_outer[..., 2, 2],
+            ],
+            axis=-1,
+        ).reshape(*q.shape[:-1], 3, 3)
 
     @override
     def parameters(self) -> jax.Array:
         return self.wxyz
 
     # Operations.
 
     @override
     def apply(self, target: hints.Array) -> jax.Array:
-        assert target.shape == (3,)
+        assert target.shape[-1:] == (3,)
+        self, target = broadcast_leading_axes((self, target))
 
         # Compute using quaternion multiplys.
-        padded_target = jnp.concatenate([jnp.zeros(1), target])
-        return (self @ SO3(wxyz=padded_target) @ self.inverse()).wxyz[1:]
+        padded_target = jnp.concatenate(
+            [jnp.zeros((*self.get_batch_axes(), 1)), target], axis=-1
+        )
+        return (self @ SO3(wxyz=padded_target) @ self.inverse()).wxyz[..., 1:]
 
     @override
     def multiply(self, other: SO3) -> SO3:
-        w0, x0, y0, z0 = self.wxyz
-        w1, x1, y1, z1 = other.wxyz
+        w0, x0, y0, z0 = jnp.moveaxis(self.wxyz, -1, 0)
+        w1, x1, y1, z1 = jnp.moveaxis(other.wxyz, -1, 0)
         return SO3(
-            wxyz=jnp.array(
+            wxyz=jnp.stack(
                 [
                     -x0 * x1 - y0 * y1 - z0 * z1 + w0 * w1,
                     x0 * w1 + y0 * z1 - z0 * y1 + w0 * x1,
                     -x0 * z1 + y0 * w1 + z0 * x1 + w0 * y1,
                     x0 * y1 - y0 * x1 + z0 * w1 + w0 * z1,
-                ]
+                ],
+                axis=-1,
             )
         )
 
-    @staticmethod
+    @classmethod
     @override
-    def exp(tangent: hints.Array) -> SO3:
+    def exp(cls, tangent: hints.Array) -> SO3:
         # Reference:
         # > https://github.com/strasdat/Sophus/blob/a0fe89a323e20c42d3cecb590937eb7a06b8343a/sophus/so3.hpp#L583
 
-        assert tangent.shape == (3,)
+        assert tangent.shape[-1:] == (3,)
 
-        theta_squared = tangent @ tangent
+        theta_squared = jnp.sum(jnp.square(tangent), axis=-1)
         theta_pow_4 = theta_squared * theta_squared
         use_taylor = theta_squared < get_epsilon(tangent.dtype)
 
         # Shim to avoid NaNs in jnp.where branches, which cause failures for
         # reverse-mode AD.
         safe_theta = jnp.sqrt(
             jnp.where(
                 use_taylor,
-                1.0,  # Any constant value should do here.
+                jnp.ones_like(theta_squared),  # Any constant value should do here.
                 theta_squared,
             )
         )
         safe_half_theta = 0.5 * safe_theta
 
         real_factor = jnp.where(
             use_taylor,
@@ -342,27 +359,28 @@
             0.5 - theta_squared / 48.0 + theta_pow_4 / 3840.0,
             jnp.sin(safe_half_theta) / safe_theta,
         )
 
         return SO3(
             wxyz=jnp.concatenate(
                 [
-                    real_factor[None],
-                    imaginary_factor * tangent,
-                ]
+                    real_factor[..., None],
+                    imaginary_factor[..., None] * tangent,
+                ],
+                axis=-1,
             )
         )
 
     @override
     def log(self) -> jax.Array:
         # Reference:
         # > https://github.com/strasdat/Sophus/blob/a0fe89a323e20c42d3cecb590937eb7a06b8343a/sophus/so3.hpp#L247
 
         w = self.wxyz[..., 0]
-        norm_sq = self.wxyz[..., 1:] @ self.wxyz[..., 1:]
+        norm_sq = jnp.sum(jnp.square(self.wxyz[..., 1:]), axis=-1)
         use_taylor = norm_sq < get_epsilon(norm_sq.dtype)
 
         # Shim to avoid NaNs in jnp.where branches, which cause failures for
         # reverse-mode AD.
         norm_safe = jnp.sqrt(
             jnp.where(
                 use_taylor,
@@ -381,46 +399,53 @@
             jnp.where(
                 jnp.abs(w) < get_epsilon(w.dtype),
                 jnp.where(w > 0, 1.0, -1.0) * jnp.pi / norm_safe,
                 2.0 * atan_n_over_w / norm_safe,
             ),
         )
 
-        return atan_factor * self.wxyz[1:]
+        return atan_factor[..., None] * self.wxyz[..., 1:]
 
     @override
     def adjoint(self) -> jax.Array:
         return self.as_matrix()
 
     @override
     def inverse(self) -> SO3:
         # Negate complex terms.
         return SO3(wxyz=self.wxyz * jnp.array([1, -1, -1, -1]))
 
     @override
     def normalize(self) -> SO3:
-        return SO3(wxyz=self.wxyz / jnp.linalg.norm(self.wxyz))
+        return SO3(wxyz=self.wxyz / jnp.linalg.norm(self.wxyz, axis=-1, keepdims=True))
 
-    @staticmethod
+    @classmethod
     @override
-    def sample_uniform(key: jax.Array) -> SO3:
+    def sample_uniform(
+        cls, key: jax.Array, batch_axes: jdc.Static[Tuple[int, ...]] = ()
+    ) -> SO3:
         # Uniformly sample over S^3.
         # > Reference: http://planning.cs.uiuc.edu/node198.html
-        u1, u2, u3 = jax.random.uniform(
-            key=key,
-            shape=(3,),
-            minval=jnp.zeros(3),
-            maxval=jnp.array([1.0, 2.0 * jnp.pi, 2.0 * jnp.pi]),
+        u1, u2, u3 = jnp.moveaxis(
+            jax.random.uniform(
+                key=key,
+                shape=(*batch_axes, 3),
+                minval=jnp.zeros(3),
+                maxval=jnp.array([1.0, 2.0 * jnp.pi, 2.0 * jnp.pi]),
+            ),
+            -1,
+            0,
         )
         a = jnp.sqrt(1.0 - u1)
         b = jnp.sqrt(u1)
 
         return SO3(
-            wxyz=jnp.array(
+            wxyz=jnp.stack(
                 [
                     a * jnp.sin(u2),
                     a * jnp.cos(u2),
                     b * jnp.sin(u3),
                     b * jnp.cos(u3),
-                ]
+                ],
+                axis=-1,
             )
         )
```

### Comparing `jaxlie-1.3.4/jaxlie/hints/__init__.py` & `jaxlie-1.4.0/jaxlie/hints/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, NamedTuple, Union
+from typing import NamedTuple, Union
 
 import jax
 import numpy as onp
 
 # Type aliases for JAX/Numpy arrays; primarily for function inputs.
 
 Array = Union[onp.ndarray, jax.Array]
```

### Comparing `jaxlie-1.3.4/jaxlie/manifold/_backprop.py` & `jaxlie-1.4.0/jaxlie/manifold/_backprop.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,28 +33,26 @@
 def grad(
     fun: Callable[P, Any],
     argnums: int = 0,
     has_aux: bool = False,
     holomorphic: bool = False,
     allow_int: bool = False,
     reduce_axes: Sequence[AxisName] = (),
-) -> Callable[P, _tree_utils.TangentPytree]:
-    ...
+) -> Callable[P, _tree_utils.TangentPytree]: ...
 
 
 @overload
 def grad(
     fun: Callable[P, Any],
     argnums: Sequence[int],
     has_aux: bool = False,
     holomorphic: bool = False,
     allow_int: bool = False,
     reduce_axes: Sequence[AxisName] = (),
-) -> Callable[P, Tuple[_tree_utils.TangentPytree, ...]]:
-    ...
+) -> Callable[P, Tuple[_tree_utils.TangentPytree, ...]]: ...
 
 
 def grad(
     fun: Callable[P, Any],
     argnums: Union[int, Sequence[int]] = 0,
     has_aux: bool = False,
     holomorphic: bool = False,
@@ -68,39 +66,45 @@
         fun=fun,
         argnums=argnums,
         has_aux=has_aux,
         holomorphic=holomorphic,
         allow_int=allow_int,
         reduce_axes=reduce_axes,
     )
-    return lambda *args, **kwargs: compute_value_and_grad(*args, **kwargs)[1]  # type: ignore
+
+    def grad_fun(*args, **kwargs):
+        ret = compute_value_and_grad(*args, **kwargs)
+        if has_aux:
+            return ret[1], ret[0][1]
+        else:
+            return ret[1]
+
+    return grad_fun
 
 
 @overload
 def value_and_grad(
     fun: Callable[P, Any],
     argnums: int = 0,
     has_aux: bool = False,
     holomorphic: bool = False,
     allow_int: bool = False,
     reduce_axes: Sequence[AxisName] = (),
-) -> Callable[P, Tuple[Any, _tree_utils.TangentPytree]]:
-    ...
+) -> Callable[P, Tuple[Any, _tree_utils.TangentPytree]]: ...
 
 
 @overload
 def value_and_grad(
     fun: Callable[P, Any],
     argnums: Sequence[int],
     has_aux: bool = False,
     holomorphic: bool = False,
     allow_int: bool = False,
     reduce_axes: Sequence[AxisName] = (),
-) -> Callable[P, Tuple[Any, Tuple[_tree_utils.TangentPytree, ...]]]:
-    ...
+) -> Callable[P, Tuple[Any, Tuple[_tree_utils.TangentPytree, ...]]]: ...
 
 
 def value_and_grad(
     fun: Callable[P, Any],
     argnums: Union[int, Sequence[int]] = 0,
     has_aux: bool = False,
     holomorphic: bool = False,
@@ -117,18 +121,17 @@
                 **_deltas.rplus(kwargs, tangent_kwargs),
             )
 
         # Put arguments onto tangent space.
         tangent_args = map(zero_tangents, args)
         tangent_kwargs = {k: zero_tangents(v) for k, v in kwargs.items()}
 
-        value, grad = jax.value_and_grad(
+        return jax.value_and_grad(
             fun=tangent_fun,
             argnums=argnums,
             has_aux=has_aux,
             holomorphic=holomorphic,
             allow_int=allow_int,
             reduce_axes=reduce_axes,
         )(*tangent_args, **tangent_kwargs)
-        return value, grad
 
     return wrapped_grad  # type: ignore
```

### Comparing `jaxlie-1.3.4/jaxlie/manifold/_deltas.py` & `jaxlie-1.4.0/jaxlie/manifold/_deltas.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,57 +12,34 @@
 from .._se3 import SE3
 from .._so2 import SO2
 from .._so3 import SO3
 from . import _tree_utils
 
 PytreeType = TypeVar("PytreeType")
 GroupType = TypeVar("GroupType", bound=MatrixLieGroup)
-CallableType = TypeVar("CallableType", bound=Callable)
 
 
-def _naive_auto_vmap(f: CallableType) -> CallableType:
-    def inner(*args, **kwargs):
-        batch_axes = None
-        for arg in args + tuple(kwargs.values()):
-            if isinstance(arg, MatrixLieGroup):
-                if batch_axes is None:
-                    batch_axes = arg.get_batch_axes()
-                else:
-                    assert arg.get_batch_axes() == batch_axes
-        assert batch_axes is not None
-
-        f_vmapped: Callable = f
-        for i in range(len(batch_axes)):
-            f_vmapped = jax.vmap(f_vmapped)
-        return f_vmapped(*args, **kwargs)
-
-    return inner  # type: ignore
-
-
-@_naive_auto_vmap
 def _rplus(transform: GroupType, delta: jax.Array) -> GroupType:
     assert isinstance(transform, MatrixLieGroup)
     assert isinstance(delta, (jax.Array, onp.ndarray))
     return transform @ type(transform).exp(delta)
 
 
 @overload
 def rplus(
     transform: GroupType,
     delta: hints.Array,
-) -> GroupType:
-    ...
+) -> GroupType: ...
 
 
 @overload
 def rplus(
     transform: PytreeType,
     delta: _tree_utils.TangentPytree,
-) -> PytreeType:
-    ...
+) -> PytreeType: ...
 
 
 # Using our typevars in the overloaded signature will cause errors.
 def rplus(
     transform: Union[MatrixLieGroup, Any],
     delta: Union[hints.Array, Any],
 ) -> Union[MatrixLieGroup, Any]:
@@ -70,28 +47,25 @@
 
     Supports pytrees containing Lie group instances recursively; simple Euclidean
     addition will be performed for all other arrays.
     """
     return _tree_utils._map_group_trees(_rplus, jnp.add, transform, delta)
 
 
-@_naive_auto_vmap
 def _rminus(a: GroupType, b: GroupType) -> jax.Array:
     assert isinstance(a, MatrixLieGroup) and isinstance(b, MatrixLieGroup)
     return (a.inverse() @ b).log()
 
 
 @overload
-def rminus(a: GroupType, b: GroupType) -> jax.Array:
-    ...
+def rminus(a: GroupType, b: GroupType) -> jax.Array: ...
 
 
 @overload
-def rminus(a: PytreeType, b: PytreeType) -> _tree_utils.TangentPytree:
-    ...
+def rminus(a: PytreeType, b: PytreeType) -> _tree_utils.TangentPytree: ...
 
 
 # Using our typevars in the overloaded signature will cause errors.
 def rminus(
     a: Union[MatrixLieGroup, Any], b: Union[MatrixLieGroup, Any]
 ) -> Union[jax.Array, _tree_utils.TangentPytree]:
     """Manifold right minus. Computes
@@ -124,73 +98,79 @@
 
     Args:
         transform: Transform to linearize around.
 
     Returns:
         Jacobian. Shape should be `(Group.parameters_dim, Group.tangent_dim)`.
     """
-    if type(transform) is SO2:
+    if isinstance(transform, SO2):
         # Jacobian row indices: cos, sin
         # Jacobian col indices: theta
 
-        transform_so2 = cast(SO2, transform)
-        J = jnp.zeros((2, 1))
-
-        cos, sin = transform_so2.unit_complex
-        J = J.at[0].set(-sin).at[1].set(cos)
+        J = jnp.zeros((*transform.get_batch_axes(), 2, 1))
+        cos, sin = jnp.moveaxis(transform.unit_complex, -1, 0)
+        J = J.at[..., 0, 0].set(-sin).at[..., 1, 0].set(cos)
 
-    elif type(transform) is SE2:
+    elif isinstance(transform, SE2):
         # Jacobian row indices: cos, sin, x, y
         # Jacobian col indices: vx, vy, omega
-
-        transform_se2 = cast(SE2, transform)
-        J = jnp.zeros((4, 3))
+        J = jnp.zeros((*transform.get_batch_axes(), 4, 3))
 
         # Translation terms.
-        J = J.at[2:, :2].set(transform_se2.rotation().as_matrix())
+        J = J.at[..., 2:, :2].set(transform.rotation().as_matrix())
 
         # Rotation terms.
-        J = J.at[:2, 2:3].set(
-            rplus_jacobian_parameters_wrt_delta(transform_se2.rotation())
+        J = J.at[..., :2, 2:3].set(
+            rplus_jacobian_parameters_wrt_delta(transform.rotation())
         )
 
-    elif type(transform) is SO3:
+    elif isinstance(transform, SO3):
         # Jacobian row indices: qw, qx, qy, qz
         # Jacobian col indices: omega x, omega y, omega z
-
-        transform_so3 = cast(SO3, transform)
-
-        w, x, y, z = transform_so3.wxyz
-        _unused_neg_w, neg_x, neg_y, neg_z = -transform_so3.wxyz
+        w, x, y, z = jnp.moveaxis(transform.wxyz, -1, 0)
+        neg_x = -x
+        neg_y = -y
+        neg_z = -z
 
         J = (
-            jnp.array(
+            jnp.stack(
                 [
-                    [neg_x, neg_y, neg_z],
-                    [w, neg_z, y],
-                    [z, w, neg_x],
-                    [neg_y, x, w],
-                ]
-            )
+                    neg_x,
+                    neg_y,
+                    neg_z,
+                    w,
+                    neg_z,
+                    y,
+                    z,
+                    w,
+                    neg_x,
+                    neg_y,
+                    x,
+                    w,
+                ],
+                axis=-1,
+            ).reshape((*transform.get_batch_axes(), 4, 3))
             / 2.0
         )
 
-    elif type(transform) is SE3:
+    elif isinstance(transform, SE3):
         # Jacobian row indices: qw, qx, qy, qz, x, y, z
         # Jacobian col indices: vx, vy, vz, omega x, omega y, omega z
-
-        transform_se3 = cast(SE3, transform)
-        J = jnp.zeros((7, 6))
+        J = jnp.zeros((*transform.get_batch_axes(), 7, 6))
 
         # Translation terms.
-        J = J.at[4:, :3].set(transform_se3.rotation().as_matrix())
+        J = J.at[..., 4:, :3].set(transform.rotation().as_matrix())
 
         # Rotation terms.
-        J = J.at[:4, 3:6].set(
-            rplus_jacobian_parameters_wrt_delta(transform_se3.rotation())
+        J = J.at[..., :4, 3:6].set(
+            rplus_jacobian_parameters_wrt_delta(transform.rotation())
         )
 
     else:
         assert False, f"Unsupported type: {type(transform)}"
 
-    assert J.shape == (transform.parameters_dim, transform.tangent_dim)
+    assert J.shape == (
+        *transform.get_batch_axes(),
+        transform.parameters_dim,
+        transform.tangent_dim,
+    )
     return J
```

### Comparing `jaxlie-1.3.4/jaxlie/manifold/_tree_utils.py` & `jaxlie-1.4.0/jaxlie/manifold/_tree_utils.py`

 * *Files identical despite different names*

### Comparing `jaxlie-1.3.4/jaxlie.egg-info/PKG-INFO` & `jaxlie-1.4.0/jaxlie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxlie
-Version: 1.3.4
+Version: 1.4.0
 Summary: Matrix Lie groups in JAX
 Home-page: http://github.com/brentyi/jaxlie
 Author: brentyi
 Author-email: brentyi@berkeley.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -14,14 +14,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jax>=0.3.18
 Requires-Dist: jax_dataclasses>=1.4.4
 Requires-Dist: numpy
+Requires-Dist: typing_extensions>=4.0.0
 Requires-Dist: tyro
 Provides-Extra: testing
 Requires-Dist: mypy; extra == "testing"
 Requires-Dist: jax!=0.3.19; extra == "testing"
 Requires-Dist: flax; extra == "testing"
 Requires-Dist: hypothesis[numpy]; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
@@ -85,14 +86,15 @@
   **`identity()`**, **`from_matrix()`**, and **`as_matrix()`** operations. (see
   [./examples/se3_example.py](./examples/se3_basics.py))
 - Helpers for optimization on manifolds (see
   [./examples/se3_optimization.py](./examples/se3_optimization.py),
   <code>jaxlie.<strong>manifold.\*</strong></code>).
 - Compatibility with standard JAX function transformations. (see
   [./examples/vmap_example.py](./examples/vmap_example.py))
+- Broadcasting for leading axes.
 - (Un)flattening as pytree nodes.
 - Serialization using [flax](https://github.com/google/flax).
 
 We also implement various common utilities for things like uniform random
 sampling (**`sample_uniform()`**) and converting from/to Euler angles (in the
 `SO3` class).
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 2.1 Name: jaxlie Version: 1.3.4 Summary: Matrix Lie groups in
+Metadata-Version: 2.1 Name: jaxlie Version: 1.4.0 Summary: Matrix Lie groups in
 JAX Home-page: http://github.com/brentyi/jaxlie Author: brentyi Author-email:
 brentyi@berkeley.edu License: MIT Classifier: Programming Language :: Python ::
 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: jax>=0.3.18 Requires-Dist:
-jax_dataclasses>=1.4.4 Requires-Dist: numpy Requires-Dist: tyro Provides-Extra:
-testing Requires-Dist: mypy; extra == "testing" Requires-Dist: jax!=0.3.19;
-extra == "testing" Requires-Dist: flax; extra == "testing" Requires-Dist:
-hypothesis[numpy]; extra == "testing" Requires-Dist: pytest; extra == "testing"
-Requires-Dist: pytest-xdist[psutil]; extra == "testing" Requires-Dist: pytest-
-cov; extra == "testing" # jaxlie ![build](https://github.com/brentyi/jaxlie/
-workflows/build/badge.svg) ![mypy](https://github.com/brentyi/jaxlie/workflows/
-mypy/badge.svg?branch=master) ![lint](https://github.com/brentyi/jaxlie/
-workflows/lint/badge.svg) [![codecov](https://codecov.io/gh/brentyi/jaxlie/
-branch/master/graph/badge.svg)](https://codecov.io/gh/brentyi/jaxlie) [!
-[pypi_dowlnoads](https://pepy.tech/badge/jaxlie)](https://pypi.org/project/
-jaxlie) **[ [API reference](https://brentyi.github.io/jaxlie) ]** **[ [PyPI]
-(https://pypi.org/project/jaxlie/) ]** `jaxlie` is a library containing
-implementations of Lie groups commonly used for rigid body transformations,
-targeted at computer vision & robotics applications written in JAX. Heavily
-inspired by the C++ library [Sophus](https://github.com/strasdat/Sophus). We
-implement Lie groups as high-level (data)classes:
+jax_dataclasses>=1.4.4 Requires-Dist: numpy Requires-Dist:
+typing_extensions>=4.0.0 Requires-Dist: tyro Provides-Extra: testing Requires-
+Dist: mypy; extra == "testing" Requires-Dist: jax!=0.3.19; extra == "testing"
+Requires-Dist: flax; extra == "testing" Requires-Dist: hypothesis[numpy]; extra
+== "testing" Requires-Dist: pytest; extra == "testing" Requires-Dist: pytest-
+xdist[psutil]; extra == "testing" Requires-Dist: pytest-cov; extra == "testing"
+# jaxlie ![build](https://github.com/brentyi/jaxlie/workflows/build/badge.svg)
+![mypy](https://github.com/brentyi/jaxlie/workflows/mypy/
+badge.svg?branch=master) ![lint](https://github.com/brentyi/jaxlie/workflows/
+lint/badge.svg) [![codecov](https://codecov.io/gh/brentyi/jaxlie/branch/master/
+graph/badge.svg)](https://codecov.io/gh/brentyi/jaxlie) [![pypi_dowlnoads]
+(https://pepy.tech/badge/jaxlie)](https://pypi.org/project/jaxlie) **[ [API
+reference](https://brentyi.github.io/jaxlie) ]** **[ [PyPI](https://pypi.org/
+project/jaxlie/) ]** `jaxlie` is a library containing implementations of Lie
+groups commonly used for rigid body transformations, targeted at computer
+vision & robotics applications written in JAX. Heavily inspired by the C++
+library [Sophus](https://github.com/strasdat/Sophus). We implement Lie groups
+as high-level (data)classes:
 GGrroouupp      DDeessccrriippttiioonn                    PPaarraammeetteerriizzaattiioonn
 jaxlie.SSOO22 Rotations in 2D.               ((rreeaall,, iimmaaggiinnaarryy)):: unit complex (â
                                           S1)
 jaxlie.SSEE22 Proper rigid transforms in 2D. ((rreeaall,, iimmaaggiinnaarryy,, xx,, yy)):: unit complex
                                           & translation
 jaxlie.SSOO33 Rotations in 3D.               ((qqww,, qqxx,, qqyy,, qqzz)):: wxyz quaternion
                                           (â S3)
@@ -35,26 +36,26 @@
 Where each group supports: - Forward- and reverse-mode AD-friendly **`exp()`**,
 **`log()`**, **`adjoint()`**, **`apply()`**, **`multiply()`**, **`inverse()`**,
 **`identity()`**, **`from_matrix()`**, and **`as_matrix()`** operations. (see
 [./examples/se3_example.py](./examples/se3_basics.py)) - Helpers for
 optimization on manifolds (see [./examples/se3_optimization.py](./examples/
 se3_optimization.py), jaxlie.mmaanniiffoolldd..\\**). - Compatibility with standard JAX
 function transformations. (see [./examples/vmap_example.py](./examples/
-vmap_example.py)) - (Un)flattening as pytree nodes. - Serialization using
-[flax](https://github.com/google/flax). We also implement various common
-utilities for things like uniform random sampling (**`sample_uniform()`**) and
-converting from/to Euler angles (in the `SO3` class). --- ### Install (Python
->=3.7) ```bash # Python 3.6 releases also exist, but are no longer being
-updated. pip install jaxlie ``` --- ### In the wild - [jaxfg](https://
-github.com/brentyi/jaxfg) applies `jaxlie` to nonlinear least squares problems
-with block-sparse structure. (for pose graph optimization, bundle adjustment,
-etc) - [tensorf-jax](https://github.com/brentyi/tensorf-jax) is an unofficial
-implementation of [Tensorial Radiance Fields (Chen et al, ECCV 2022)](https://
-apchenstu.github.io/TensoRF/) using `jaxlie`. ![Render of a lego](https://
-github.com/brentyi/tensorf-jax/raw/main/lego_render.gif) --- ### Misc `jaxlie`
-was originally written for our IROS 2021 paper ([link](https://github.com/
-brentyi/dfgo)). If it's useful for you, you're welcome to cite: ```
-@inproceedings{yi2021iros, author={Brent Yi and Michelle Lee and Alina Kloss
-and Roberto Mart\'in-Mart\'in and Jeannette Bohg}, title = {Differentiable
-Factor Graph Optimization for Learning Smoothers}, year = 2021, BOOKTITLE =
-{2021 IEEE/RSJ International Conference on Intelligent Robots and Systems
-(IROS)} } ```
+vmap_example.py)) - Broadcasting for leading axes. - (Un)flattening as pytree
+nodes. - Serialization using [flax](https://github.com/google/flax). We also
+implement various common utilities for things like uniform random sampling
+(**`sample_uniform()`**) and converting from/to Euler angles (in the `SO3`
+class). --- ### Install (Python >=3.7) ```bash # Python 3.6 releases also
+exist, but are no longer being updated. pip install jaxlie ``` --- ### In the
+wild - [jaxfg](https://github.com/brentyi/jaxfg) applies `jaxlie` to nonlinear
+least squares problems with block-sparse structure. (for pose graph
+optimization, bundle adjustment, etc) - [tensorf-jax](https://github.com/
+brentyi/tensorf-jax) is an unofficial implementation of [Tensorial Radiance
+Fields (Chen et al, ECCV 2022)](https://apchenstu.github.io/TensoRF/) using
+`jaxlie`. ![Render of a lego](https://github.com/brentyi/tensorf-jax/raw/main/
+lego_render.gif) --- ### Misc `jaxlie` was originally written for our IROS 2021
+paper ([link](https://github.com/brentyi/dfgo)). If it's useful for you, you're
+welcome to cite: ``` @inproceedings{yi2021iros, author={Brent Yi and Michelle
+Lee and Alina Kloss and Roberto Mart\'in-Mart\'in and Jeannette Bohg}, title =
+{Differentiable Factor Graph Optimization for Learning Smoothers}, year = 2021,
+BOOKTITLE = {2021 IEEE/RSJ International Conference on Intelligent Robots and
+Systems (IROS)} } ```
```

### Comparing `jaxlie-1.3.4/jaxlie.egg-info/SOURCES.txt` & `jaxlie-1.4.0/jaxlie.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -17,12 +17,13 @@
 jaxlie/manifold/__init__.py
 jaxlie/manifold/_backprop.py
 jaxlie/manifold/_deltas.py
 jaxlie/manifold/_tree_utils.py
 jaxlie/utils/__init__.py
 jaxlie/utils/_utils.py
 tests/test_autodiff.py
+tests/test_broadcast.py
 tests/test_examples.py
 tests/test_group_axioms.py
 tests/test_manifold.py
 tests/test_operations.py
 tests/test_serialization.py
```

### Comparing `jaxlie-1.3.4/setup.py` & `jaxlie-1.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="jaxlie",
-    version="1.3.4",
+    version="1.4.0",
     description="Matrix Lie groups in JAX",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/brentyi/jaxlie",
     author="brentyi",
     author_email="brentyi@berkeley.edu",
     license="MIT",
     packages=find_packages(),
     package_data={"jaxlie": ["py.typed"]},
     python_requires=">=3.8",
     install_requires=[
         "jax>=0.3.18",  # For jax.Array.
         "jax_dataclasses>=1.4.4",
         "numpy",
+        "typing_extensions>=4.0.0",
         "tyro",  # Only used in examples.
     ],
     extras_require={
         "testing": [
             "mypy",
             # https://github.com/google/jax/issues/12536
             "jax!=0.3.19",
```

### Comparing `jaxlie-1.3.4/tests/test_autodiff.py` & `jaxlie-1.4.0/tests/test_autodiff.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Compare forward- and reverse-mode Jacobians with a numerical Jacobian."""
 
 from functools import lru_cache
-from typing import Callable, Type, cast
+from typing import Callable, Tuple, Type, cast
 
 import jax
 import numpy as onp
 from jax import numpy as jnp
 from utils import assert_arrays_close, general_group_test, jacnumerical
 
 import jaxlie
@@ -52,120 +52,145 @@
 
     for omega in jnp.eye(3) * jnp.pi:
         a = jnp.array(omega, dtype=jnp.float32)
         assert all(onp.logical_not(onp.isnan(func(a))))
 
 
 @general_group_test
-def test_exp_random(Group: Type[jaxlie.MatrixLieGroup]):
+def test_exp_random(Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]):
     """Check that exp Jacobians are consistent, with randomly sampled transforms."""
+    del batch_axes  # Not used for autodiff tests.
     generator = onp.random.randn(Group.tangent_dim)
     _assert_jacobians_close(Group=Group, f=_exp, primal=generator)
 
 
 @general_group_test
-def test_exp_identity(Group: Type[jaxlie.MatrixLieGroup]):
+def test_exp_identity(Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]):
     """Check that exp Jacobians are consistent, with transforms close to the
     identity."""
+    del batch_axes  # Not used for autodiff tests.
     generator = onp.random.randn(Group.tangent_dim) * 1e-6
     _assert_jacobians_close(Group=Group, f=_exp, primal=generator)
 
 
 # Log tests.
 def _log(Group: Type[jaxlie.MatrixLieGroup], params: jax.Array) -> jax.Array:
     return Group.log(Group(params))
 
 
 @general_group_test
-def test_log_random(Group: Type[jaxlie.MatrixLieGroup]):
+def test_log_random(Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]):
     """Check that log Jacobians are consistent, with randomly sampled transforms."""
+    del batch_axes  # Not used for autodiff tests.
     params = Group.exp(onp.random.randn(Group.tangent_dim)).parameters()
     _assert_jacobians_close(Group=Group, f=_log, primal=params)
 
 
 @general_group_test
-def test_log_identity(Group: Type[jaxlie.MatrixLieGroup]):
+def test_log_identity(Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]):
     """Check that log Jacobians are consistent, with transforms close to the
     identity."""
     params = Group.exp(onp.random.randn(Group.tangent_dim) * 1e-6).parameters()
     _assert_jacobians_close(Group=Group, f=_log, primal=params)
 
 
 # Adjoint tests.
 def _adjoint(Group: Type[jaxlie.MatrixLieGroup], params: jax.Array) -> jax.Array:
     return cast(jax.Array, Group(params).adjoint().flatten())
 
 
 @general_group_test
-def test_adjoint_random(Group: Type[jaxlie.MatrixLieGroup]):
+def test_adjoint_random(
+    Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]
+):
     """Check that adjoint Jacobians are consistent, with randomly sampled transforms."""
+    del batch_axes  # Not used for autodiff tests.
     params = Group.exp(onp.random.randn(Group.tangent_dim)).parameters()
     _assert_jacobians_close(Group=Group, f=_adjoint, primal=params)
 
 
 @general_group_test
-def test_adjoint_identity(Group: Type[jaxlie.MatrixLieGroup]):
+def test_adjoint_identity(
+    Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]
+):
     """Check that adjoint Jacobians are consistent, with transforms close to the
     identity."""
+    del batch_axes  # Not used for autodiff tests.
     params = Group.exp(onp.random.randn(Group.tangent_dim) * 1e-6).parameters()
     _assert_jacobians_close(Group=Group, f=_adjoint, primal=params)
 
 
 # Apply tests.
 def _apply(Group: Type[jaxlie.MatrixLieGroup], params: jax.Array) -> jax.Array:
     return Group(params) @ onp.ones(Group.space_dim)
 
 
 @general_group_test
-def test_apply_random(Group: Type[jaxlie.MatrixLieGroup]):
+def test_apply_random(Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]):
     """Check that apply Jacobians are consistent, with randomly sampled transforms."""
+    del batch_axes  # Not used for autodiff tests.
     params = Group.exp(onp.random.randn(Group.tangent_dim)).parameters()
     _assert_jacobians_close(Group=Group, f=_apply, primal=params)
 
 
 @general_group_test
-def test_apply_identity(Group: Type[jaxlie.MatrixLieGroup]):
+def test_apply_identity(
+    Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]
+):
     """Check that apply Jacobians are consistent, with transforms close to the
     identity."""
+    del batch_axes  # Not used for autodiff tests.
     params = Group.exp(onp.random.randn(Group.tangent_dim) * 1e-6).parameters()
     _assert_jacobians_close(Group=Group, f=_apply, primal=params)
 
 
 # Multiply tests.
 def _multiply(Group: Type[jaxlie.MatrixLieGroup], params: jax.Array) -> jax.Array:
     return cast(jax.Array, (Group(params) @ Group(params)).parameters())
 
 
 @general_group_test
-def test_multiply_random(Group: Type[jaxlie.MatrixLieGroup]):
+def test_multiply_random(
+    Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]
+):
     """Check that multiply Jacobians are consistent, with randomly sampled
     transforms."""
+    del batch_axes  # Not used for autodiff tests.
     params = Group.exp(onp.random.randn(Group.tangent_dim)).parameters()
     _assert_jacobians_close(Group=Group, f=_multiply, primal=params)
 
 
 @general_group_test
-def test_multiply_identity(Group: Type[jaxlie.MatrixLieGroup]):
+def test_multiply_identity(
+    Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]
+):
     """Check that multiply Jacobians are consistent, with transforms close to the
     identity."""
+    del batch_axes  # Not used for autodiff tests.
     params = Group.exp(onp.random.randn(Group.tangent_dim) * 1e-6).parameters()
     _assert_jacobians_close(Group=Group, f=_multiply, primal=params)
 
 
 # Inverse tests.
 def _inverse(Group: Type[jaxlie.MatrixLieGroup], params: jax.Array) -> jax.Array:
     return cast(jax.Array, Group(params).inverse().parameters())
 
 
 @general_group_test
-def test_inverse_random(Group: Type[jaxlie.MatrixLieGroup]):
+def test_inverse_random(
+    Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]
+):
     """Check that inverse Jacobians are consistent, with randomly sampled transforms."""
+    del batch_axes  # Not used for autodiff tests.
     params = Group.exp(onp.random.randn(Group.tangent_dim)).parameters()
     _assert_jacobians_close(Group=Group, f=_inverse, primal=params)
 
 
 @general_group_test
-def test_inverse_identity(Group: Type[jaxlie.MatrixLieGroup]):
+def test_inverse_identity(
+    Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]
+):
     """Check that inverse Jacobians are consistent, with transforms close to the
     identity."""
+    del batch_axes  # Not used for autodiff tests.
     params = Group.exp(onp.random.randn(Group.tangent_dim) * 1e-6).parameters()
     _assert_jacobians_close(Group=Group, f=_inverse, primal=params)
```

### Comparing `jaxlie-1.3.4/tests/test_examples.py` & `jaxlie-1.4.0/tests/test_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tests with explicit examples."""
+
 import numpy as onp
-import pytest
 from hypothesis import given, settings
 from hypothesis import strategies as st
 from utils import assert_arrays_close, assert_transforms_close, sample_transform
 
 import jaxlie
 
 
@@ -58,24 +58,24 @@
     """Check that we can create an SO3 object from an xyzw quaternion."""
     assert_transforms_close(
         jaxlie.SO3.from_quaternion_xyzw(onp.array([0.0, 0.0, 0.0, 1.0])),
         jaxlie.SO3.identity(),
     )
 
 
-def test_so3_xyzw_dtype_error():
-    """Check that an incorrect data-type results in an AssertionError."""
-    with pytest.raises(AssertionError):
-        jaxlie.SO3(onp.array([1, 0, 0, 0])),
-
-
-def test_so3_xyzw_shape_error():
-    """Check that an incorrect shape results in an AssertionError."""
-    with pytest.raises(AssertionError):
-        jaxlie.SO3(onp.array([1.0, 0.0, 0.0, 0.0, 0.0]))
+# def test_so3_xyzw_dtype_error():
+#     """Check that an incorrect data-type results in an AssertionError."""
+#     with pytest.raises(AssertionError):
+#         jaxlie.SO3(onp.array([1, 0, 0, 0])),
+#
+#
+# def test_so3_xyzw_shape_error():
+#     """Check that an incorrect shape results in an AssertionError."""
+#     with pytest.raises(AssertionError):
+#         jaxlie.SO3(onp.array([1.0, 0.0, 0.0, 0.0, 0.0]))
 
 
 @settings(deadline=None)
 @given(_random_module=st.random_module())
 def test_se3_compose(_random_module):
     """Compare SE3 composition in matrix form vs compact form."""
     T1 = sample_transform(jaxlie.SE3)
```

### Comparing `jaxlie-1.3.4/tests/test_manifold.py` & `jaxlie-1.4.0/tests/test_manifold.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Test manifold helpers."""
-from typing import Type
+
+from typing import Tuple, Type
 
 import jax
 import numpy as onp
 import pytest
 from jax import numpy as jnp
 from jax import tree_util
 from utils import (
@@ -14,51 +15,61 @@
     sample_transform,
 )
 
 import jaxlie
 
 
 @general_group_test
-def test_rplus_rminus(Group: Type[jaxlie.MatrixLieGroup]):
+def test_rplus_rminus(Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]):
     """Check rplus and rminus on random inputs."""
-    T_wa = sample_transform(Group)
-    T_wb = sample_transform(Group)
+    T_wa = sample_transform(Group, batch_axes)
+    T_wb = sample_transform(Group, batch_axes)
     T_ab = T_wa.inverse() @ T_wb
 
     assert_transforms_close(jaxlie.manifold.rplus(T_wa, T_ab.log()), T_wb)
     assert_arrays_close(jaxlie.manifold.rminus(T_wa, T_wb), T_ab.log())
 
 
 @general_group_test
-def test_rplus_jacobian(Group: Type[jaxlie.MatrixLieGroup]):
+def test_rplus_jacobian(
+    Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]
+):
     """Check analytical rplus Jacobian.."""
-    T_wa = sample_transform(Group)
+    T_wa = sample_transform(Group, batch_axes)
 
     J_ours = jaxlie.manifold.rplus_jacobian_parameters_wrt_delta(T_wa)
-    J_jacfwd = _rplus_jacobian_parameters_wrt_delta(T_wa)
 
-    assert_arrays_close(J_ours, J_jacfwd)
+    if batch_axes == ():
+        J_jacfwd = _rplus_jacobian_parameters_wrt_delta(T_wa)
+        assert_arrays_close(J_ours, J_jacfwd)
+    else:
+        # Batch axes should match vmap.
+        jacfunc = jaxlie.manifold.rplus_jacobian_parameters_wrt_delta
+        for _ in batch_axes:
+            jacfunc = jax.vmap(jacfunc)
+        J_vmap = jacfunc(T_wa)
+        assert_arrays_close(J_ours, J_vmap)
 
 
 @jax.jit
 def _rplus_jacobian_parameters_wrt_delta(
     transform: jaxlie.MatrixLieGroup,
 ) -> jax.Array:
     # Copied from docstring for `rplus_jacobian_parameters_wrt_delta()`.
     return jax.jacfwd(
         lambda delta: jaxlie.manifold.rplus(transform, delta).parameters()
     )(onp.zeros(transform.tangent_dim))
 
 
 @general_group_test_faster
-def test_sgd(Group: Type[jaxlie.MatrixLieGroup]):
+def test_sgd(Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]):
     def loss(transform: jaxlie.MatrixLieGroup):
         return (transform.log() ** 2).sum()
 
-    transform = Group.exp(sample_transform(Group).log())
+    transform = Group.exp(sample_transform(Group, batch_axes).log())
     original_loss = loss(transform)
 
     @jax.jit
     def step(t):
         return jaxlie.manifold.rplus(t, -1e-3 * jaxlie.manifold.grad(loss)(t))
 
     for i in range(5):
```

### Comparing `jaxlie-1.3.4/tests/test_operations.py` & `jaxlie-1.4.0/tests/test_operations.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tests for general operation definitions."""
 
-from typing import Type
+from typing import Tuple, Type
 
 import numpy as onp
 from hypothesis import given, settings
 from hypothesis import strategies as st
 from jax import numpy as jnp
 from utils import (
     assert_arrays_close,
@@ -13,17 +13,19 @@
     sample_transform,
 )
 
 import jaxlie
 
 
 @general_group_test
-def test_sample_uniform_valid(Group: Type[jaxlie.MatrixLieGroup]):
+def test_sample_uniform_valid(
+    Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]
+):
     """Check that sample_uniform() returns valid group members."""
-    T = sample_transform(Group)  # Calls sample_uniform under the hood.
+    T = sample_transform(Group, batch_axes)  # Calls sample_uniform under the hood.
     assert_transforms_close(T, T.normalize())
 
 
 @settings(deadline=None)
 @given(_random_module=st.random_module())
 def test_so2_from_to_radians_bijective(_random_module):
     """Check that we can convert from and to radians."""
@@ -44,85 +46,106 @@
 def test_so3_rpy_bijective(_random_module):
     """Check that we can convert between quaternions and Euler angles."""
     T = sample_transform(jaxlie.SO3)
     assert_transforms_close(T, jaxlie.SO3.from_rpy_radians(*T.as_rpy_radians()))
 
 
 @general_group_test
-def test_log_exp_bijective(Group: Type[jaxlie.MatrixLieGroup]):
+def test_log_exp_bijective(
+    Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]
+):
     """Check 1-to-1 mapping for log <=> exp operations."""
-    transform = sample_transform(Group)
+    transform = sample_transform(Group, batch_axes)
 
     tangent = transform.log()
-    assert tangent.shape == (Group.tangent_dim,)
+    assert tangent.shape == (*batch_axes, Group.tangent_dim)
 
     exp_transform = Group.exp(tangent)
     assert_transforms_close(transform, exp_transform)
     assert_arrays_close(tangent, exp_transform.log())
 
 
 @general_group_test
-def test_inverse_bijective(Group: Type[jaxlie.MatrixLieGroup]):
+def test_inverse_bijective(
+    Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]
+):
     """Check inverse of inverse."""
-    transform = sample_transform(Group)
+    transform = sample_transform(Group, batch_axes)
     assert_transforms_close(transform, transform.inverse().inverse())
 
 
 @general_group_test
-def test_matrix_bijective(Group: Type[jaxlie.MatrixLieGroup]):
+def test_matrix_bijective(
+    Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]
+):
     """Check that we can convert to and from matrices."""
-    transform = sample_transform(Group)
+    transform = sample_transform(Group, batch_axes)
     assert_transforms_close(transform, Group.from_matrix(transform.as_matrix()))
 
 
 @general_group_test
-def test_adjoint(Group: Type[jaxlie.MatrixLieGroup]):
+def test_adjoint(Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]):
     """Check adjoint definition."""
-    transform = sample_transform(Group)
-    omega = onp.random.randn(Group.tangent_dim)
+    transform = sample_transform(Group, batch_axes)
+    omega = onp.random.randn(*batch_axes, Group.tangent_dim)
     assert_transforms_close(
         transform @ Group.exp(omega),
-        Group.exp(transform.adjoint() @ omega) @ transform,
+        Group.exp(onp.einsum("...ij,...j->...i", transform.adjoint(), omega))
+        @ transform,
     )
 
 
 @general_group_test
-def test_repr(Group: Type[jaxlie.MatrixLieGroup]):
+def test_repr(Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]):
     """Smoke test for __repr__ implementations."""
-    transform = sample_transform(Group)
+    transform = sample_transform(Group, batch_axes)
     print(transform)
 
 
 @general_group_test
-def test_apply(Group: Type[jaxlie.MatrixLieGroup]):
+def test_apply(Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]):
     """Check group action interfaces."""
-    T_w_b = sample_transform(Group)
-    p_b = onp.random.randn(Group.space_dim)
+    T_w_b = sample_transform(Group, batch_axes)
+    p_b = onp.random.randn(*batch_axes, Group.space_dim)
 
     if Group.matrix_dim == Group.space_dim:
         assert_arrays_close(
             T_w_b @ p_b,
             T_w_b.apply(p_b),
-            T_w_b.as_matrix() @ p_b,
+            onp.einsum("...ij,...j->...i", T_w_b.as_matrix(), p_b),
         )
     else:
         # Homogeneous coordinates.
         assert Group.matrix_dim == Group.space_dim + 1
         assert_arrays_close(
             T_w_b @ p_b,
             T_w_b.apply(p_b),
-            (T_w_b.as_matrix() @ onp.append(p_b, 1.0))[:-1],
+            onp.einsum(
+                "...ij,...j->...i",
+                T_w_b.as_matrix(),
+                onp.concatenate([p_b, onp.ones_like(p_b[..., :1])], axis=-1),
+            )[..., :-1],
         )
 
 
 @general_group_test
-def test_multiply(Group: Type[jaxlie.MatrixLieGroup]):
+def test_multiply(Group: Type[jaxlie.MatrixLieGroup], batch_axes: Tuple[int, ...]):
     """Check multiply interfaces."""
-    T_w_b = sample_transform(Group)
-    T_b_a = sample_transform(Group)
+    T_w_b = sample_transform(Group, batch_axes)
+    T_b_a = sample_transform(Group, batch_axes)
     assert_arrays_close(
-        T_w_b.as_matrix() @ T_w_b.inverse().as_matrix(), onp.eye(Group.matrix_dim)
+        onp.einsum(
+            "...ij,...jk->...ik", T_w_b.as_matrix(), T_w_b.inverse().as_matrix()
+        ),
+        onp.broadcast_to(
+            onp.eye(Group.matrix_dim), (*batch_axes, Group.matrix_dim, Group.matrix_dim)
+        ),
     )
     assert_arrays_close(
-        T_w_b.as_matrix() @ jnp.linalg.inv(T_w_b.as_matrix()), onp.eye(Group.matrix_dim)
+        onp.einsum(
+            "...ij,...jk->...ik", T_w_b.as_matrix(), jnp.linalg.inv(T_w_b.as_matrix())
+        ),
+        onp.broadcast_to(
+            onp.eye(Group.matrix_dim), (*batch_axes, Group.matrix_dim, Group.matrix_dim)
+        ),
     )
     assert_transforms_close(T_w_b @ T_b_a, Group.multiply(T_w_b, T_b_a))
```

