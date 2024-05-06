# Comparing `tmp/torch_kf-0.0.3.tar.gz` & `tmp/torch_kf-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_kf-0.0.3.tar", last modified: Wed Apr 24 13:00:34 2024, max compression
+gzip compressed data, was "torch_kf-0.0.4.tar", last modified: Mon May  6 16:54:49 2024, max compression
```

## Comparing `torch_kf-0.0.3.tar` & `torch_kf-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:00:34.881488 torch_kf-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-24 13:00:30.000000 torch_kf-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-04-24 13:00:34.881488 torch_kf-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-24 13:00:30.000000 torch_kf-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 13:00:30.000000 torch_kf-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-24 13:00:34.881488 torch_kf-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 13:00:30.000000 torch_kf-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:00:34.881488 torch_kf-0.0.3/torch_kf/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 13:00:30.000000 torch_kf-0.0.3/torch_kf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21789 2024-04-24 13:00:30.000000 torch_kf-0.0.3/torch_kf/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:00:30.000000 torch_kf-0.0.3/torch_kf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:00:34.881488 torch_kf-0.0.3/torch_kf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-04-24 13:00:34.000000 torch_kf-0.0.3/torch_kf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-24 13:00:34.000000 torch_kf-0.0.3/torch_kf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:00:34.000000 torch_kf-0.0.3/torch_kf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 13:00:34.000000 torch_kf-0.0.3/torch_kf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 13:00:34.000000 torch_kf-0.0.3/torch_kf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:54:49.468736 torch_kf-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-06 16:54:45.000000 torch_kf-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-06 16:54:49.468736 torch_kf-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-06 16:54:45.000000 torch_kf-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-06 16:54:45.000000 torch_kf-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-06 16:54:49.468736 torch_kf-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-06 16:54:45.000000 torch_kf-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:54:49.468736 torch_kf-0.0.4/torch_kf/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-06 16:54:45.000000 torch_kf-0.0.4/torch_kf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24426 2024-05-06 16:54:45.000000 torch_kf-0.0.4/torch_kf/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:54:45.000000 torch_kf-0.0.4/torch_kf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:54:49.468736 torch_kf-0.0.4/torch_kf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-06 16:54:49.000000 torch_kf-0.0.4/torch_kf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-06 16:54:49.000000 torch_kf-0.0.4/torch_kf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:54:49.000000 torch_kf-0.0.4/torch_kf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 16:54:49.000000 torch_kf-0.0.4/torch_kf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 16:54:49.000000 torch_kf-0.0.4/torch_kf.egg-info/top_level.txt
```

### Comparing `torch_kf-0.0.3/LICENSE` & `torch_kf-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_kf-0.0.3/PKG-INFO` & `torch_kf-0.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: torch-kf
-Version: 0.0.3
-Summary: Kalman Filter implementation with PyTorch
-Home-page: https://github.com/raphaelreme/torch-kf
-Author: Raphael Reme
-Author-email: raphaelreme-dev@protonmail.com
-License: MIT
-Keywords: Kalman filter,statistics,pytorch
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch
-
 # torch-kf
 
 [![Lint and Test](https://github.com/raphaelreme/torch-kf/actions/workflows/tests.yml/badge.svg)](https://github.com/raphaelreme/torch-kf/actions/workflows/tests.yml)
 
 PyTorch implementation of Kalman filters. It supports filtering of batch of signals, runs on gpu (supported by PyTorch) or multiple cpus.
 
 This is based on rlabbe's [filterpy](https://github.com/rlabbe/filterpy) and [interactive book](https://github.com/rlabbe/Kalman-and-Bayesian-Filters-in-Python/) on kalman filters. Currently only traditional Kalman filters are implemented without any smoothing.
@@ -58,65 +34,79 @@
 
 ```python
 
 import torch
 from torch_kf import KalmanFilter, GaussianState
 
 # Some noisy_data to filter
-# 1000 timessteps, 100 signals, 2D and an additional dimension to have vertical vectors (required for correct matmult)
+# 1000 timesteps, 100 signals, 2D and an additional dimension to have vertical vectors (required for correct matmult)
 noisy_data = torch.randn(1000, 100, 2, 1)
 
-# Create a Kalman Filter (for instance a constant velocity filter) (See this is fully implemented, or rlabbe's book)
+# Create a Kalman Filter (for instance a constant velocity filter) (See example or rlabbe's book)
 F = torch.tensor([  # x_{t+1} = x_{t} + v_{t} * dt     (dt = 1)
-    [1, 0, 1, 0],
+    [1, 0, 1, 0.],
     [0, 1, 0, 1],
     [0, 0, 1, 0],
     [0, 0, 0, 1],
 ])
-Q = torch.eye(4) * 1.5 **2  # 1.5 std on both pos and velocity (See full implementation to build a better Q)
+Q = torch.eye(4) * 1.5 **2  # 1.5 std on both pos and velocity (See examples or rlabee's book to build a better Q)
 H = torch.tensor([  # Only x and y are measured
-    [1, 0, 0, 0],
+    [1, 0, 0, 0.],
     [0, 1, 0, 0],
 ])
 R = torch.eye(2) * 3**2
 
 kf = KalmanFilter(F, H, Q, R)
 
 # Create an inital belief for each signal
 # For instance let's start from 0 pos and 0 vel with a huge uncertainty
 state = GaussianState(
-    torch.zeros_like(100, 4, 1),  # Shape (100, 4, 1)
+    torch.zeros(100, 4, 1),  # Shape (100, 4, 1)
     torch.eye(4)[None].expand(100, 4, 4) * 150**2,  # Shape (100, 4, 4)
 )
 
 # And let's filter and save our signals all at once
-
-filtered_data = torch.empty_like(noisy_data)
+# Store the state (x, y, dx, dy) for each element in the batch and each time
+filtered_data = torch.empty((1000, 100, 4, 1))
 
 for t, measure in enumerate(noisy_data):  # Update first and then predict in this case
     # Update with measure at time t
     state = kf.update(state, measure)
 
     # Save state at time t
     filtered_data[t] = state.mean
 
     # Predict for t + 1
     state = kf.predict(state)
 
+# Alternatively you can use the already implemented filter method:
+states = kf.filter(state, noisy_data, update_first=True, return_all=True)
+# states.mean: (1000, 100, 4, 1)
+# states.covariance: (1000, 100, 4, 4)
+
+# And optionnally smooth the data (not online: all data should already be available and collected) using RTS smoothing
+smoothed = kf.rts_smooth(states)
+# smoothed.mean: (1000, 100, 4, 1)
+# smoothed.covariance: (1000, 100, 4, 4)
+
 ```
 
 ## Examples
 
-We provide a simple example of constant velocity kalman filter (1d, 2d, ...) in the `example` folder using batch of signals and show when our implementation is worth to use.
+We provide simple examples of constant velocity kalman filter (1d, 2d, ...) in the `example` folder using batch of signals.
+
+For instance, if system is a sinusoidal function with noisy measurement we can filter and smooth the data using kalman filters. Here is such an example with `nan` measurements in the middle of the filtering process:
+![Sinusoidal position](images/sinusoidal_pos.png)
+![Sinusoidal position](images/sinusoidal_vel.png)
 
-On a laptop with pretty good cpus and a GPU (a bit rusty), we have typically these performances:
+We also benchmark our implementation to check when it is faster than filterpy. On a laptop with pretty good cpus and a GPU (a bit rusty), we have typically these performances:
 
 ![Computational time](images/computational_time.png)
 
-One can see that both cpus and gpu version have a large overhead when the batch is small. But they may lead to a 200x speed up or more when numerous signals are filtered together.
+One can see that both cpus and gpu version have a large overhead when the batch is small. But they may lead to a 200x (and 500x for gpu) speed up or more when numerous signals are filtered together.
 
 
 ## Contribute
 
 Please feel free to open a PR or an issue at any time.
 
 Many variants of Kalman filtering/smoothing are still missing and the documentation is pretty poor, in comparison [filterpy](https://github.com/rlabbe/filterpy) is a much more complete library and may give some ideas of what is missing.
```

### Comparing `torch_kf-0.0.3/README.md` & `torch_kf-0.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: torch-kf
+Version: 0.0.4
+Summary: Kalman Filter implementation with PyTorch
+Home-page: https://github.com/raphaelreme/torch-kf
+Author: Raphael Reme
+Author-email: raphaelreme-dev@protonmail.com
+License: MIT
+Keywords: Kalman filter,statistics,pytorch
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch
+
 # torch-kf
 
 [![Lint and Test](https://github.com/raphaelreme/torch-kf/actions/workflows/tests.yml/badge.svg)](https://github.com/raphaelreme/torch-kf/actions/workflows/tests.yml)
 
 PyTorch implementation of Kalman filters. It supports filtering of batch of signals, runs on gpu (supported by PyTorch) or multiple cpus.
 
 This is based on rlabbe's [filterpy](https://github.com/rlabbe/filterpy) and [interactive book](https://github.com/rlabbe/Kalman-and-Bayesian-Filters-in-Python/) on kalman filters. Currently only traditional Kalman filters are implemented without any smoothing.
@@ -34,65 +58,79 @@
 
 ```python
 
 import torch
 from torch_kf import KalmanFilter, GaussianState
 
 # Some noisy_data to filter
-# 1000 timessteps, 100 signals, 2D and an additional dimension to have vertical vectors (required for correct matmult)
+# 1000 timesteps, 100 signals, 2D and an additional dimension to have vertical vectors (required for correct matmult)
 noisy_data = torch.randn(1000, 100, 2, 1)
 
-# Create a Kalman Filter (for instance a constant velocity filter) (See this is fully implemented, or rlabbe's book)
+# Create a Kalman Filter (for instance a constant velocity filter) (See example or rlabbe's book)
 F = torch.tensor([  # x_{t+1} = x_{t} + v_{t} * dt     (dt = 1)
-    [1, 0, 1, 0],
+    [1, 0, 1, 0.],
     [0, 1, 0, 1],
     [0, 0, 1, 0],
     [0, 0, 0, 1],
 ])
-Q = torch.eye(4) * 1.5 **2  # 1.5 std on both pos and velocity (See full implementation to build a better Q)
+Q = torch.eye(4) * 1.5 **2  # 1.5 std on both pos and velocity (See examples or rlabee's book to build a better Q)
 H = torch.tensor([  # Only x and y are measured
-    [1, 0, 0, 0],
+    [1, 0, 0, 0.],
     [0, 1, 0, 0],
 ])
 R = torch.eye(2) * 3**2
 
 kf = KalmanFilter(F, H, Q, R)
 
 # Create an inital belief for each signal
 # For instance let's start from 0 pos and 0 vel with a huge uncertainty
 state = GaussianState(
-    torch.zeros_like(100, 4, 1),  # Shape (100, 4, 1)
+    torch.zeros(100, 4, 1),  # Shape (100, 4, 1)
     torch.eye(4)[None].expand(100, 4, 4) * 150**2,  # Shape (100, 4, 4)
 )
 
 # And let's filter and save our signals all at once
-
-filtered_data = torch.empty_like(noisy_data)
+# Store the state (x, y, dx, dy) for each element in the batch and each time
+filtered_data = torch.empty((1000, 100, 4, 1))
 
 for t, measure in enumerate(noisy_data):  # Update first and then predict in this case
     # Update with measure at time t
     state = kf.update(state, measure)
 
     # Save state at time t
     filtered_data[t] = state.mean
 
     # Predict for t + 1
     state = kf.predict(state)
 
+# Alternatively you can use the already implemented filter method:
+states = kf.filter(state, noisy_data, update_first=True, return_all=True)
+# states.mean: (1000, 100, 4, 1)
+# states.covariance: (1000, 100, 4, 4)
+
+# And optionnally smooth the data (not online: all data should already be available and collected) using RTS smoothing
+smoothed = kf.rts_smooth(states)
+# smoothed.mean: (1000, 100, 4, 1)
+# smoothed.covariance: (1000, 100, 4, 4)
+
 ```
 
 ## Examples
 
-We provide a simple example of constant velocity kalman filter (1d, 2d, ...) in the `example` folder using batch of signals and show when our implementation is worth to use.
+We provide simple examples of constant velocity kalman filter (1d, 2d, ...) in the `example` folder using batch of signals.
+
+For instance, if system is a sinusoidal function with noisy measurement we can filter and smooth the data using kalman filters. Here is such an example with `nan` measurements in the middle of the filtering process:
+![Sinusoidal position](images/sinusoidal_pos.png)
+![Sinusoidal position](images/sinusoidal_vel.png)
 
-On a laptop with pretty good cpus and a GPU (a bit rusty), we have typically these performances:
+We also benchmark our implementation to check when it is faster than filterpy. On a laptop with pretty good cpus and a GPU (a bit rusty), we have typically these performances:
 
 ![Computational time](images/computational_time.png)
 
-One can see that both cpus and gpu version have a large overhead when the batch is small. But they may lead to a 200x speed up or more when numerous signals are filtered together.
+One can see that both cpus and gpu version have a large overhead when the batch is small. But they may lead to a 200x (and 500x for gpu) speed up or more when numerous signals are filtered together.
 
 
 ## Contribute
 
 Please feel free to open a PR or an issue at any time.
 
 Many variants of Kalman filtering/smoothing are still missing and the documentation is pretty poor, in comparison [filterpy](https://github.com/rlabbe/filterpy) is a much more complete library and may give some ideas of what is missing.
```

### Comparing `torch_kf-0.0.3/setup.cfg` & `torch_kf-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `torch_kf-0.0.3/torch_kf/kalman_filter.py` & `torch_kf-0.0.4/torch_kf/kalman_filter.py`

 * *Files 5% similar despite different names*

```diff
@@ -430,23 +430,25 @@
 
         # XXX: Did not use the more robust P = (I-KH)P(I-KH)' + KRK' from filterpy (as it is slower)
         # Again for robustness you should go with filterpy
         covariance = state.covariance - kalman_gain @ measurement_matrix @ state.covariance
 
         return GaussianState(mean, covariance)
 
-    def batch_filter(
+    def filter(
         self, state: GaussianState, measures: torch.Tensor, update_first=False, return_all=False
     ) -> GaussianState:
-        """Filter a batch of signal with given measures
+        """Filter signals with given measures
 
         It handles most of the default use-cases but it remains very standard, you probably will have to rewrite
-        it for a specific problem.
+        it for a specific problem. It supports nan values in measures. The states associated with a nan measure
+        are not updated. For a multidimensional measure, a single nan value will invalidate all the measure
+        (because the measurement matrix cannot be infered).
 
-        For instance:
+        Limitations examples:
         It only works if states and measures are already aligned (associated).
         It is memory intensive as it requires the input (and output if `return_all`) to be stored in a tensor.
         It does not support changing the Kalman model (F, Q, H, R) in time.
 
         Again all of this can be done manually using this function as a baseline for a more precise code.
 
         Args:
@@ -464,20 +466,30 @@
         """
         # Convert state to the right dtype and device
         state = state.to(self.dtype).to(self.device)
 
         saver: GaussianState
 
         for t, measure in enumerate(measures):
-            if t or not update_first:  # Do not predict on the first t /
+            if t or not update_first:  # Do not predict on the first t
                 state = self.predict(state)
 
             # Convert on the fly the measure to avoid to store them all in cuda memory
             # To avoid this overhead, the conversion can be done by the user before calling `batch_filter`
-            state = self.update(state, measure.to(self.dtype).to(self.device, non_blocking=True))  # Update
+            measure = measure.to(self.dtype).to(self.device, non_blocking=True)
+
+            # Support for nan measure: Do not update state associated with a nan measure
+            mask = torch.isnan(measure[..., 0]).any(dim=-1)
+            if mask.any():
+                valid_state = GaussianState(state.mean[~mask], state.covariance[~mask])
+                valid_state = self.update(valid_state, measure[~mask])  # Update states with valid measures
+                state.mean[~mask] = valid_state.mean
+                state.covariance[~mask] = valid_state.covariance
+            else:
+                state = self.update(state, measure)  # Update states
 
             if return_all:
                 if t == 0:  # Create the saver now that we know the size of an updated state
                     # In this implementation, it cannot evolve in time, but it still supports
                     # to have a change from the initial_state shape to the first updated state (with the first measure)
                     saver = GaussianState(
                         torch.empty(
@@ -494,14 +506,52 @@
                 saver.covariance[t] = state.covariance
 
         if return_all:
             return saver
 
         return state
 
+    def rts_smooth(self, state: GaussianState, inplace=False) -> GaussianState:
+        """Smooth filtered signals using Rauch-Tung-Striebel smoothing.
+
+        It handles most of the default use-cases but it remains very standard, you may have to rewrite it for
+        a specific smoothing problem. For instance it does not support changing the Kalman model (F, Q, H, R) in time.
+
+        Smoothing can be done manually using this function as a baseline for a more precise code.
+
+        Args:
+            state (GaussianState): All filtered states in time. (Typically returned by filter with `return_all=True`)
+                The first dimension of the state is seen as time: for instance mean is expected
+                to be (T, *, dim_x, 1)
+            inplace (bool): Modify inplace state
+                Default: False (will allocate twice more memory)
+
+        Returns:
+            GaussianState: All smoothed states in time
+                The first dimension is time: for instance the covariance is (T, *, dim_x, dim_x)
+        """
+        if inplace:
+            out = state
+        else:
+            out = GaussianState(
+                state.mean.clone(),
+                state.covariance.clone(),
+            )
+
+        # Iterate backward to update all states (except the last one which is already fine)
+        for t in range(state.mean.shape[0] - 2, -1, -1):
+            cov_at_process = state.covariance[t] @ self.process_matrix.mT
+            predicted_covariance = self.process_matrix @ cov_at_process + self.process_noise
+
+            kalman_gain = cov_at_process @ predicted_covariance.inverse().mT
+            out.mean[t] += kalman_gain @ (out.mean[t + 1] - self.process_matrix @ state.mean[t])
+            out.covariance[t] += kalman_gain @ (out.covariance[t + 1] - predicted_covariance) @ kalman_gain.mT
+
+        return out
+
     def __repr__(self) -> str:
         return "\n".join(
             [
                 f"Kalman Filter (State: {self.state_dim}, Measure: {self.measure_dim})",
                 f"F: {tuple(self.process_matrix.shape)}",
                 f"Q: {tuple(self.process_noise.shape)}",
                 f"H: {tuple(self.measurement_matrix.shape)}",
```

### Comparing `torch_kf-0.0.3/torch_kf.egg-info/PKG-INFO` & `torch_kf-0.0.4/torch_kf.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-kf
-Version: 0.0.3
+Version: 0.0.4
 Summary: Kalman Filter implementation with PyTorch
 Home-page: https://github.com/raphaelreme/torch-kf
 Author: Raphael Reme
 Author-email: raphaelreme-dev@protonmail.com
 License: MIT
 Keywords: Kalman filter,statistics,pytorch
 Classifier: Development Status :: 4 - Beta
@@ -58,65 +58,79 @@
 
 ```python
 
 import torch
 from torch_kf import KalmanFilter, GaussianState
 
 # Some noisy_data to filter
-# 1000 timessteps, 100 signals, 2D and an additional dimension to have vertical vectors (required for correct matmult)
+# 1000 timesteps, 100 signals, 2D and an additional dimension to have vertical vectors (required for correct matmult)
 noisy_data = torch.randn(1000, 100, 2, 1)
 
-# Create a Kalman Filter (for instance a constant velocity filter) (See this is fully implemented, or rlabbe's book)
+# Create a Kalman Filter (for instance a constant velocity filter) (See example or rlabbe's book)
 F = torch.tensor([  # x_{t+1} = x_{t} + v_{t} * dt     (dt = 1)
-    [1, 0, 1, 0],
+    [1, 0, 1, 0.],
     [0, 1, 0, 1],
     [0, 0, 1, 0],
     [0, 0, 0, 1],
 ])
-Q = torch.eye(4) * 1.5 **2  # 1.5 std on both pos and velocity (See full implementation to build a better Q)
+Q = torch.eye(4) * 1.5 **2  # 1.5 std on both pos and velocity (See examples or rlabee's book to build a better Q)
 H = torch.tensor([  # Only x and y are measured
-    [1, 0, 0, 0],
+    [1, 0, 0, 0.],
     [0, 1, 0, 0],
 ])
 R = torch.eye(2) * 3**2
 
 kf = KalmanFilter(F, H, Q, R)
 
 # Create an inital belief for each signal
 # For instance let's start from 0 pos and 0 vel with a huge uncertainty
 state = GaussianState(
-    torch.zeros_like(100, 4, 1),  # Shape (100, 4, 1)
+    torch.zeros(100, 4, 1),  # Shape (100, 4, 1)
     torch.eye(4)[None].expand(100, 4, 4) * 150**2,  # Shape (100, 4, 4)
 )
 
 # And let's filter and save our signals all at once
-
-filtered_data = torch.empty_like(noisy_data)
+# Store the state (x, y, dx, dy) for each element in the batch and each time
+filtered_data = torch.empty((1000, 100, 4, 1))
 
 for t, measure in enumerate(noisy_data):  # Update first and then predict in this case
     # Update with measure at time t
     state = kf.update(state, measure)
 
     # Save state at time t
     filtered_data[t] = state.mean
 
     # Predict for t + 1
     state = kf.predict(state)
 
+# Alternatively you can use the already implemented filter method:
+states = kf.filter(state, noisy_data, update_first=True, return_all=True)
+# states.mean: (1000, 100, 4, 1)
+# states.covariance: (1000, 100, 4, 4)
+
+# And optionnally smooth the data (not online: all data should already be available and collected) using RTS smoothing
+smoothed = kf.rts_smooth(states)
+# smoothed.mean: (1000, 100, 4, 1)
+# smoothed.covariance: (1000, 100, 4, 4)
+
 ```
 
 ## Examples
 
-We provide a simple example of constant velocity kalman filter (1d, 2d, ...) in the `example` folder using batch of signals and show when our implementation is worth to use.
+We provide simple examples of constant velocity kalman filter (1d, 2d, ...) in the `example` folder using batch of signals.
+
+For instance, if system is a sinusoidal function with noisy measurement we can filter and smooth the data using kalman filters. Here is such an example with `nan` measurements in the middle of the filtering process:
+![Sinusoidal position](images/sinusoidal_pos.png)
+![Sinusoidal position](images/sinusoidal_vel.png)
 
-On a laptop with pretty good cpus and a GPU (a bit rusty), we have typically these performances:
+We also benchmark our implementation to check when it is faster than filterpy. On a laptop with pretty good cpus and a GPU (a bit rusty), we have typically these performances:
 
 ![Computational time](images/computational_time.png)
 
-One can see that both cpus and gpu version have a large overhead when the batch is small. But they may lead to a 200x speed up or more when numerous signals are filtered together.
+One can see that both cpus and gpu version have a large overhead when the batch is small. But they may lead to a 200x (and 500x for gpu) speed up or more when numerous signals are filtered together.
 
 
 ## Contribute
 
 Please feel free to open a PR or an issue at any time.
 
 Many variants of Kalman filtering/smoothing are still missing and the documentation is pretty poor, in comparison [filterpy](https://github.com/rlabbe/filterpy) is a much more complete library and may give some ideas of what is missing.
```

