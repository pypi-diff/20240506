# Comparing `tmp/pygradflow-0.4.0.tar.gz` & `tmp/pygradflow-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygradflow-0.4.0.tar", max compression
+gzip compressed data, was "pygradflow-0.4.1.tar", max compression
```

## Comparing `pygradflow-0.4.0.tar` & `pygradflow-0.4.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    10847 2024-04-30 13:32:32.760728 pygradflow-0.4.0/LICENSE
--rw-r--r--   0        0        0      984 2024-04-30 13:32:32.760728 pygradflow-0.4.0/README.md
--rw-r--r--   0        0        0        0 2024-04-30 13:32:32.760728 pygradflow-0.4.0/pygradflow/__init__.py
--rw-r--r--   0        0        0      872 2024-04-30 13:32:32.760728 pygradflow-0.4.0/pygradflow/active_set.py
--rw-r--r--   0        0        0     4458 2024-04-30 13:32:32.760728 pygradflow-0.4.0/pygradflow/cons_problem.py
--rw-r--r--   0        0        0     1749 2024-04-30 13:32:32.760728 pygradflow-0.4.0/pygradflow/controller.py
--rw-r--r--   0        0        0     2487 2024-04-30 13:32:32.760728 pygradflow-0.4.0/pygradflow/deriv_check.py
--rw-r--r--   0        0        0     4645 2024-04-30 13:32:32.760728 pygradflow-0.4.0/pygradflow/display.py
--rw-r--r--   0        0        0     4839 2024-04-30 13:32:32.760728 pygradflow-0.4.0/pygradflow/eval.py
--rw-r--r--   0        0        0     6380 2024-04-30 13:32:32.760728 pygradflow-0.4.0/pygradflow/implicit_func.py
--rw-r--r--   0        0        0     5146 2024-04-30 13:32:32.760728 pygradflow-0.4.0/pygradflow/iterate.py
--rw-r--r--   0        0        0       55 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/log.py
--rw-r--r--   0        0        0     6570 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/newton.py
--rw-r--r--   0        0        0     5166 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/params.py
--rw-r--r--   0        0        0     5111 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/penalty.py
--rw-r--r--   0        0        0     5845 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/problem.py
--rw-r--r--   0        0        0        0 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/py.typed
--rw-r--r--   0        0        0     3437 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/runners/cutest_runner.py
--rw-r--r--   0        0        0      366 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/runners/instance.py
--rw-r--r--   0        0        0     2045 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/runners/qplib_runner.py
--rw-r--r--   0        0        0     7417 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/runners/runner.py
--rw-r--r--   0        0        0     4181 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/scale.py
--rw-r--r--   0        0        0    16425 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/solver.py
--rw-r--r--   0        0        0     1284 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/step/__init__.py
--rw-r--r--   0        0        0     4439 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/step/asymmetric_step_solver.py
--rw-r--r--   0        0        0     5493 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/step/box_control.py
--rw-r--r--   0        0        0     2710 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/step/cond_estimate.py
--rw-r--r--   0        0        0     2424 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/step/distance_ratio_control.py
--rw-r--r--   0        0        0     1913 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/step/exact_control.py
--rw-r--r--   0        0        0     3173 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/step/extended_step_solver.py
--rw-r--r--   0        0        0      536 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/step/fixed_control.py
--rw-r--r--   0        0        0     2669 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/step/linear_solver.py
--rw-r--r--   0        0        0     7413 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/step/opti_control.py
--rw-r--r--   0        0        0     2007 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/step/residuum_ratio_control.py
--rw-r--r--   0        0        0     2401 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/step/scaled_step_solver.py
--rw-r--r--   0        0        0     2467 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/step/standard_step_solver.py
--rw-r--r--   0        0        0     4611 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/step/step_control.py
--rw-r--r--   0        0        0     2048 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/step/step_solver.py
--rw-r--r--   0        0        0     4120 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/step/symmetric_step_solver.py
--rw-r--r--   0        0        0     1711 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/transform.py
--rw-r--r--   0        0        0      232 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pygradflow/util.py
--rw-r--r--   0        0        0     1138 2024-04-30 13:32:32.764728 pygradflow-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pygradflow-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    10847 2024-05-06 10:06:35.504787 pygradflow-0.4.1/LICENSE
+-rw-r--r--   0        0        0      984 2024-05-06 10:06:35.504787 pygradflow-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 10:06:35.504787 pygradflow-0.4.1/pygradflow/__init__.py
+-rw-r--r--   0        0        0      872 2024-05-06 10:06:35.504787 pygradflow-0.4.1/pygradflow/active_set.py
+-rw-r--r--   0        0        0     4458 2024-05-06 10:06:35.504787 pygradflow-0.4.1/pygradflow/cons_problem.py
+-rw-r--r--   0        0        0     1749 2024-05-06 10:06:35.504787 pygradflow-0.4.1/pygradflow/controller.py
+-rw-r--r--   0        0        0     2487 2024-05-06 10:06:35.504787 pygradflow-0.4.1/pygradflow/deriv_check.py
+-rw-r--r--   0        0        0     4645 2024-05-06 10:06:35.504787 pygradflow-0.4.1/pygradflow/display.py
+-rw-r--r--   0        0        0     4839 2024-05-06 10:06:35.504787 pygradflow-0.4.1/pygradflow/eval.py
+-rw-r--r--   0        0        0     6380 2024-05-06 10:06:35.504787 pygradflow-0.4.1/pygradflow/implicit_func.py
+-rw-r--r--   0        0        0     5146 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/iterate.py
+-rw-r--r--   0        0        0       55 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/log.py
+-rw-r--r--   0        0        0     6570 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/newton.py
+-rw-r--r--   0        0        0     5166 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/params.py
+-rw-r--r--   0        0        0     5111 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/penalty.py
+-rw-r--r--   0        0        0     5845 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/problem.py
+-rw-r--r--   0        0        0        0 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/py.typed
+-rw-r--r--   0        0        0     3378 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/runners/cutest_runner.py
+-rw-r--r--   0        0        0      366 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/runners/instance.py
+-rw-r--r--   0        0        0     2045 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/runners/qplib_runner.py
+-rw-r--r--   0        0        0     7417 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/runners/runner.py
+-rw-r--r--   0        0        0     4181 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/scale.py
+-rw-r--r--   0        0        0    16425 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/solver.py
+-rw-r--r--   0        0        0     1284 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/step/__init__.py
+-rw-r--r--   0        0        0     4439 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/step/asymmetric_step_solver.py
+-rw-r--r--   0        0        0     5493 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/step/box_control.py
+-rw-r--r--   0        0        0     2710 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/step/cond_estimate.py
+-rw-r--r--   0        0        0     2424 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/step/distance_ratio_control.py
+-rw-r--r--   0        0        0     1913 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/step/exact_control.py
+-rw-r--r--   0        0        0     3173 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/step/extended_step_solver.py
+-rw-r--r--   0        0        0      536 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/step/fixed_control.py
+-rw-r--r--   0        0        0     2669 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/step/linear_solver.py
+-rw-r--r--   0        0        0     7462 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/step/opti_control.py
+-rw-r--r--   0        0        0     2007 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/step/residuum_ratio_control.py
+-rw-r--r--   0        0        0     2401 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/step/scaled_step_solver.py
+-rw-r--r--   0        0        0     2467 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/step/standard_step_solver.py
+-rw-r--r--   0        0        0     4611 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/step/step_control.py
+-rw-r--r--   0        0        0     2048 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/step/step_solver.py
+-rw-r--r--   0        0        0     4120 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/step/symmetric_step_solver.py
+-rw-r--r--   0        0        0     1711 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/transform.py
+-rw-r--r--   0        0        0      232 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pygradflow/util.py
+-rw-r--r--   0        0        0     1138 2024-05-06 10:06:35.508787 pygradflow-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pygradflow-0.4.1/PKG-INFO
```

### Comparing `pygradflow-0.4.0/LICENSE` & `pygradflow-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/README.md` & `pygradflow-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/active_set.py` & `pygradflow-0.4.1/pygradflow/active_set.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/cons_problem.py` & `pygradflow-0.4.1/pygradflow/cons_problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/controller.py` & `pygradflow-0.4.1/pygradflow/controller.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/deriv_check.py` & `pygradflow-0.4.1/pygradflow/deriv_check.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/display.py` & `pygradflow-0.4.1/pygradflow/display.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/eval.py` & `pygradflow-0.4.1/pygradflow/eval.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/implicit_func.py` & `pygradflow-0.4.1/pygradflow/implicit_func.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/iterate.py` & `pygradflow-0.4.1/pygradflow/iterate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/newton.py` & `pygradflow-0.4.1/pygradflow/newton.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/params.py` & `pygradflow-0.4.1/pygradflow/params.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/penalty.py` & `pygradflow-0.4.1/pygradflow/penalty.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/problem.py` & `pygradflow-0.4.1/pygradflow/problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/runners/cutest_runner.py` & `pygradflow-0.4.1/pygradflow/runners/cutest_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 
     def obj_grad(self, x):
         obj, grad = self.instance.obj(x, gradient=True)
         return grad
 
     def cons(self, x):
         return self.instance.cons(x)
-        raise NotImplementedError("Unconstrained problem")
 
     def cons_jac(self, x):
         cons, jac = self.instance.scons(x, gradient=True)
         return jac
 
     def lag_hess(self, x, y):
         return self.instance.sphess(x, v=y)
```

### Comparing `pygradflow-0.4.0/pygradflow/runners/qplib_runner.py` & `pygradflow-0.4.1/pygradflow/runners/qplib_runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/runners/runner.py` & `pygradflow-0.4.1/pygradflow/runners/runner.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/scale.py` & `pygradflow-0.4.1/pygradflow/scale.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/solver.py` & `pygradflow-0.4.1/pygradflow/solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/step/__init__.py` & `pygradflow-0.4.1/pygradflow/step/__init__.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/step/asymmetric_step_solver.py` & `pygradflow-0.4.1/pygradflow/step/asymmetric_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/step/box_control.py` & `pygradflow-0.4.1/pygradflow/step/box_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/step/cond_estimate.py` & `pygradflow-0.4.1/pygradflow/step/cond_estimate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/step/distance_ratio_control.py` & `pygradflow-0.4.1/pygradflow/step/distance_ratio_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/step/exact_control.py` & `pygradflow-0.4.1/pygradflow/step/exact_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/step/extended_step_solver.py` & `pygradflow-0.4.1/pygradflow/step/extended_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/step/fixed_control.py` & `pygradflow-0.4.1/pygradflow/step/fixed_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/step/linear_solver.py` & `pygradflow-0.4.1/pygradflow/step/linear_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/step/opti_control.py` & `pygradflow-0.4.1/pygradflow/step/opti_control.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import math
 
 import cyipopt
 import numpy as np
 
+from pygradflow.eval import astype
 from pygradflow.implicit_func import ImplicitFunc
 from pygradflow.iterate import Iterate
 from pygradflow.step.step_control import (
     StepController,
     StepControlResult,
     StepSolverError,
 )
@@ -33,14 +34,15 @@
     """
 
     def __init__(self, iterate, lamb, rho):
         assert lamb >= 0
         assert rho >= 0
 
         self.iterate = iterate
+        self.eval = iterate.eval
         self.lamb = lamb
         self.rho = rho
 
         problem = iterate.problem
         prob_num_vars = problem.num_vars
         prob_num_cons = problem.num_cons
 
@@ -72,17 +74,17 @@
     def objective(self, z):
         assert z.shape == (self.num_vars,)
         (x, w) = np.split(z, [self.prob_num_vars])
 
         rho = self.rho
         lamb = self.lamb
 
-        problem = self.problem
-        obj = problem.obj(x)
-        cons = problem.cons(x)
+        eval = self.eval
+        obj = eval.obj(x)
+        cons = eval.cons(x)
         aug_obj = obj + (rho / 2) * np.dot(cons, cons)
 
         xdiff = x - self.iterate.x
 
         if rescaled:
             wdiff = w - math.sqrt(lamb) * self.iterate.y
             aug_obj += (lamb / 2) * np.dot(xdiff, xdiff) + (1 / 2) * np.dot(
@@ -90,24 +92,24 @@
             )
         else:
             wdiff = w - self.iterate.y
             aug_obj += (lamb / 2) * (np.dot(xdiff, xdiff) + np.dot(wdiff, wdiff))
 
         assert np.isfinite(aug_obj)
 
-        return aug_obj
+        return float(aug_obj)
 
     def gradient(self, z):
         assert z.shape == (self.num_vars,)
         (x, w) = np.split(z, [self.prob_num_vars])
 
-        problem = self.problem
-        obj_grad = problem.obj_grad(x)
-        cons_jac = problem.cons_jac(x)
-        cons = problem.cons(x)
+        eval = self.eval
+        obj_grad = eval.obj_grad(x)
+        cons_jac = eval.cons_jac(x)
+        cons = eval.cons(x)
 
         rho = self.rho
         lamb = self.lamb
 
         cons_prod = cons_jac.T.dot(cons)
 
         gradx = obj_grad + rho * cons_prod + lamb * (x - self.iterate.x)
@@ -116,65 +118,65 @@
             gradw = w - math.sqrt(lamb) * self.iterate.y
         else:
             gradw = lamb * (w - self.iterate.y)
         grad = np.concatenate([gradx, gradw])
 
         assert grad.shape == (self.num_vars,)
         assert np.isfinite(grad).all()
-        assert grad.dtype == np.float64
 
-        return grad
+        return astype(grad, np.float64)
 
     def constraints(self, z):
         assert z.shape == (self.num_vars,)
         (x, w) = np.split(z, [self.prob_num_vars])
 
-        prob_cons = self.problem.cons(x)
+        eval = self.eval
+        prob_cons = eval.cons(x)
         lamb = self.lamb
 
         if rescaled:
             cons = prob_cons + math.sqrt(lamb) * w
         else:
             cons = prob_cons + lamb * w
 
         assert cons.shape == (self.num_cons,)
         assert np.isfinite(cons).all()
-        assert cons.dtype == np.float64
 
-        return cons
+        return astype(cons, np.float64)
 
     def jacobian(self, z):
         assert z.shape == (self.num_vars,)
         (x, w) = np.split(z, [self.prob_num_vars])
 
+        eval = self.eval
         problem = self.problem
-        jac_x = problem.cons_jac(x).tocoo()
+        jac_x = eval.cons_jac(x).tocoo()
         data_x = jac_x.data
 
         if rescaled:
             data_w = np.full((problem.num_cons,), math.sqrt(self.lamb))
         else:
             data_w = np.full((problem.num_cons,), self.lamb)
 
         assert self._jac_nnz is not None
 
         data = np.concatenate([data_x, data_w])
 
         assert data.shape == (self._jac_nnz,)
         assert np.isfinite(data).all()
-        assert data.dtype == np.float64
 
-        return data
+        return astype(data, np.float64)
 
     def jacobianstructure(self):
         problem = self.problem
         iterate = self.iterate
         x = iterate.x
 
-        jac_x = problem.cons_jac(x).tocoo()
+        eval = self.eval
+        jac_x = eval.cons_jac(x).tocoo()
 
         (r_x, c_x) = (jac_x.row, jac_x.col)
         (r_w, c_w) = np.diag_indices(problem.num_cons)
         r_w = np.copy(r_w)
         c_w = np.copy(c_w)
 
         c_w += problem.num_vars
```

### Comparing `pygradflow-0.4.0/pygradflow/step/residuum_ratio_control.py` & `pygradflow-0.4.1/pygradflow/step/residuum_ratio_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/step/scaled_step_solver.py` & `pygradflow-0.4.1/pygradflow/step/scaled_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/step/standard_step_solver.py` & `pygradflow-0.4.1/pygradflow/step/standard_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/step/step_control.py` & `pygradflow-0.4.1/pygradflow/step/step_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/step/step_solver.py` & `pygradflow-0.4.1/pygradflow/step/step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/step/symmetric_step_solver.py` & `pygradflow-0.4.1/pygradflow/step/symmetric_step_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pygradflow/transform.py` & `pygradflow-0.4.1/pygradflow/transform.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.0/pyproject.toml` & `pygradflow-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygradflow"
-version = "0.4.0"
+version = "0.4.1"
 description = "PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs."
 authors = ["Christoph Hansknecht <christoph.hansknecht@tu-clausthal.de>"]
 readme = "README.md"
 repository = "https://github.com/chrhansk/pygradflow"
 documentation = "https://pygradflow.readthedocs.io"
```

### Comparing `pygradflow-0.4.0/PKG-INFO` & `pygradflow-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygradflow
-Version: 0.4.0
+Version: 0.4.1
 Summary: PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs.
 Home-page: https://github.com/chrhansk/pygradflow
 Author: Christoph Hansknecht
 Author-email: christoph.hansknecht@tu-clausthal.de
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

