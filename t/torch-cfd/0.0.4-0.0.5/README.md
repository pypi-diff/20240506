# Comparing `tmp/torch_cfd-0.0.4.tar.gz` & `tmp/torch_cfd-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_cfd-0.0.4.tar", last modified: Fri May  3 03:47:34 2024, max compression
+gzip compressed data, was "torch_cfd-0.0.5.tar", last modified: Mon May  6 20:13:01 2024, max compression
```

## Comparing `torch_cfd-0.0.4.tar` & `torch_cfd-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:47:34.824221 torch_cfd-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-03 03:47:34.824221 torch_cfd-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 03:47:34.824221 torch_cfd-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-03 03:47:28.000000 torch_cfd-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:47:34.820221 torch_cfd-0.0.4/torch_cfd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/torch_cfd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/torch_cfd/equations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/torch_cfd/fast_diagonalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/torch_cfd/finite_differences.py
--rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/torch_cfd/forcings.py
--rw-r--r--   0 runner    (1001) docker     (127)    41005 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/torch_cfd/grids.py
--rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/torch_cfd/initial_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-05-03 03:46:01.000000 torch_cfd-0.0.4/torch_cfd/tensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 03:47:34.824221 torch_cfd-0.0.4/torch_cfd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-03 03:47:34.000000 torch_cfd-0.0.4/torch_cfd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-03 03:47:34.000000 torch_cfd-0.0.4/torch_cfd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 03:47:34.000000 torch_cfd-0.0.4/torch_cfd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 03:47:34.000000 torch_cfd-0.0.4/torch_cfd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 03:47:34.000000 torch_cfd-0.0.4/torch_cfd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:13:01.985019 torch_cfd-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 20:11:26.000000 torch_cfd-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-06 20:13:01.985019 torch_cfd-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-06 20:11:26.000000 torch_cfd-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:13:01.985019 torch_cfd-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-06 20:12:58.000000 torch_cfd-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:13:01.985019 torch_cfd-0.0.5/torch_cfd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:26.000000 torch_cfd-0.0.5/torch_cfd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-05-06 20:11:26.000000 torch_cfd-0.0.5/torch_cfd/equations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-06 20:11:26.000000 torch_cfd-0.0.5/torch_cfd/fast_diagonalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-05-06 20:11:26.000000 torch_cfd-0.0.5/torch_cfd/finite_differences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-05-06 20:11:26.000000 torch_cfd-0.0.5/torch_cfd/forcings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41005 2024-05-06 20:11:26.000000 torch_cfd-0.0.5/torch_cfd/grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-06 20:11:26.000000 torch_cfd-0.0.5/torch_cfd/initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-06 20:11:26.000000 torch_cfd-0.0.5/torch_cfd/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-05-06 20:11:26.000000 torch_cfd-0.0.5/torch_cfd/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:13:01.985019 torch_cfd-0.0.5/torch_cfd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-06 20:13:01.000000 torch_cfd-0.0.5/torch_cfd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-06 20:13:01.000000 torch_cfd-0.0.5/torch_cfd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:13:01.000000 torch_cfd-0.0.5/torch_cfd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 20:13:01.000000 torch_cfd-0.0.5/torch_cfd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 20:13:01.000000 torch_cfd-0.0.5/torch_cfd.egg-info/top_level.txt
```

### Comparing `torch_cfd-0.0.4/LICENSE` & `torch_cfd-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.4/PKG-INFO` & `torch_cfd-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-cfd
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyTorch CFD
 Home-page: https://github.com/scaomath/torch-cfd
 Author: Shuhao Cao
 Author-email: scao.math@gmail.com
 License: Apache-2.0
 Keywords: pytorch,cfd,pde,spectral
 Classifier: Development Status :: 4 - Beta
```

### Comparing `torch_cfd-0.0.4/README.md` & `torch_cfd-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.4/setup.py` & `torch_cfd-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'torch-cfd',
   packages=find_packages(include=['torch_cfd', 'torch_cfd.*']),
-  version='0.0.4',
+  version='0.0.5',
   license='Apache-2.0',
   description = 'PyTorch CFD',
   long_description='PyTorch Computational Fluid Dynamics Library',
   long_description_content_type="text/markdown",
   author = 'Shuhao Cao',
   author_email = 'scao.math@gmail.com',
   url = 'https://github.com/scaomath/torch-cfd',
```

### Comparing `torch_cfd-0.0.4/torch_cfd/equations.py` & `torch_cfd-0.0.5/torch_cfd/equations.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Modifications copyright (C) 2024 S.Cao
 # ported Google's Jax-CFD functional template to PyTorch's tensor ops
 
-from typing import Tuple, Callable, Dict, Optional
+from typing import Callable, Dict, Optional, Tuple
 
 import torch
-import torch.nn as nn
 import torch.fft as fft
-from . import grids
+import torch.nn as nn
 from tqdm.auto import tqdm
 
+from . import grids
+
 TQDM_ITERS = 500
 
 Array = torch.Tensor
 Grid = grids.Grid
 
 
 def stable_time_step(
@@ -51,15 +52,15 @@
       the range [0.5, 1).
     dx: spatial mesh size, can be min(grid.step).
     dt: time step.
     """
     dt_diffusion = dx
 
     if not implicit_diffusion:
-        dt_diffusion = dx ** 2 / (viscosity * 2 ** (ndim))
+        dt_diffusion = dx**2 / (viscosity * 2 ** (ndim))
     dt_advection = max_courant_number * dx / max_velocity
     dt = dt_advection if dt is None else dt
     return min(dt_diffusion, dt_advection, dt)
 
 
 class ImplicitExplicitODE(nn.Module):
     """Describes a set of ODEs with implicit & explicit terms.
@@ -260,15 +261,15 @@
         u,
         dt=dt,
         equation=equation,
         params=params,
     )
 
 
-class NavierStokes2DSpectral(nn.Module):
+class NavierStokes2DSpectral(ImplicitExplicitODE):
     """Breaks the Navier-Stokes equation into implicit and explicit parts.
 
     Implicit parts are the linear terms and explicit parts are the non-linear
     terms.
 
     Attributes:
       viscosity: strength of the diffusion term
@@ -353,20 +354,21 @@
             parallel scheme for the Fourier pseudospectral solver applied to 2D
             Navier-Stokes turbulence, Computers & Fluids, Volume 33, Issue 4, 2004,
             Pages 509-520, ISSN 0045-7930,
             https://doi.org/10.1016/j.compfluid.2003.06.003.
         """
         kx, ky = rfft_mesh if rfft_mesh is not None else grid.rfft_mesh()
         two_pi_i = 2 * torch.pi * 1j
+        assert kx.shape[-2:] == w_hat.shape[-2:]
         laplace = two_pi_i**2 * (abs(kx) ** 2 + abs(ky) ** 2)
-        laplace[0, 0] = 1
+        laplace[..., 0, 0] = 1
         psi_hat = -1 / laplace * w_hat
-        vxhat = two_pi_i * ky * psi_hat
-        vyhat = -two_pi_i * kx * psi_hat
-        return vxhat, vyhat
+        u_hat = two_pi_i * ky * psi_hat
+        v_hat = -two_pi_i * kx * psi_hat
+        return u_hat, v_hat
 
     def residual(
         self,
         vort_hat: Array,
         vort_t_hat: Array,
     ):
         residual = (
@@ -422,16 +424,23 @@
         record_every_steps=1,
         pbar=False,
         pbar_desc="",
         require_grad=False,
     ):
         """
         vorticity stacked in the time dimension
+        all inputs and outputs are in the frequency domain
+        input: w0 (*, n, n)
+        output:
+
+        vorticity (*, n_t, kx, ky)
+        velocity: tuple of (*, n_t, kx, ky)
         """
         w_all = []
+        u_all = []
         v_all = []
         dwdt_all = []
         res_all = []
         w = w0
         time_steps = int(T / dt)
         update_iters = time_steps // TQDM_ITERS
         with tqdm(total=time_steps) as pbar:
@@ -441,34 +450,44 @@
                 dwdt.requires_grad_(require_grad)
 
                 if t % update_iters == 0:
                     pbar.set_description(pbar_desc)
                     pbar.update(update_iters)
 
                 if t % record_every_steps == 0:
-                    w_ = w.detach().clone()
-                    dwdt_ = dwdt.detach().clone()
-                    v = self.vorticity_to_velocity(self.grid, w_)
-                    res = self.residual(w_, dwdt_)
+                    u, v = self.vorticity_to_velocity(self.grid, w)
+                    res = self.residual(w, dwdt)
+
+                    w_, dwdt_, u, v, res = [
+                        var.detach().cpu().clone() for var in [w, dwdt, u, v, res]
+                    ]
 
-                    v = torch.stack(v, dim=0)
                     w_all.append(w_)
+                    u_all.append(u)
                     v_all.append(v)
                     dwdt_all.append(dwdt_)
                     res_all.append(res)
 
         result = {
-            var_name: torch.stack(var, dim=0)
+            var_name: torch.stack(var, dim=-3)
             for var_name, var in zip(
-                ["vorticity", "velocity", "vort_t", "residual"],
-                [w_all, v_all, dwdt_all, res_all],
+                ["vorticity", "u", "v", "vort_t", "residual"],
+                [w_all, u_all, v_all, dwdt_all, res_all],
             )
         }
         return result
 
     def step(self, *args, **kwargs):
         return self.forward(*args, **kwargs)
 
-    def forward(self, vort_hat, dt):
-        vort_hat_new = self.solver(vort_hat, dt, self)
-        dvortdt_hat = 1 / dt * (vort_hat_new - vort_hat)
-        return vort_hat_new, dvortdt_hat
+    def forward(self, vort_hat, dt, steps=1):
+        """
+        vort_hat: (B, kx, ky) or (n_t, kx, ky) or (kx, ky)
+        - if rfft2 is used then the shape is (*, kx, ky//2+1)
+        - if (n_t, kx, ky), then the time step marches in the time
+        dimension in parallel.
+        """
+        vort_old = vort_hat
+        for _ in range(steps):
+            vort_hat = self.solver(vort_hat, dt, self)
+        dvortdt_hat = 1 / (steps * dt) * (vort_hat - vort_old)
+        return vort_hat, dvortdt_hat
```

### Comparing `torch_cfd-0.0.4/torch_cfd/fast_diagonalization.py` & `torch_cfd-0.0.5/torch_cfd/fast_diagonalization.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.4/torch_cfd/finite_differences.py` & `torch_cfd-0.0.5/torch_cfd/finite_differences.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.4/torch_cfd/forcings.py` & `torch_cfd-0.0.5/torch_cfd/forcings.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.4/torch_cfd/grids.py` & `torch_cfd-0.0.5/torch_cfd/grids.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.4/torch_cfd/initial_conditions.py` & `torch_cfd-0.0.5/torch_cfd/initial_conditions.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Modifications copyright (C) 2024 S.Cao
 # ported Google's Jax-CFD functional template to PyTorch's tensor ops
 
 """Prepare initial conditions for simulations."""
-from typing import Callable, Optional, Sequence
 import math
+from typing import Callable, Optional, Sequence
+
 import torch
 import torch.fft as fft
-from . import grids
-from . import finite_differences as fd
-from . import fast_diagonalization as solver
+
+from . import grids, pressure
 
 Array = torch.Tensor
 GridArray = grids.GridArray
 GridArrayVector = grids.GridArrayVector
 GridVariable = grids.GridVariable
 GridVariableVector = grids.GridVariableVector
 BoundaryConditions = grids.BoundaryConditions
@@ -41,27 +41,32 @@
     """Wrap velocity arrays for input into simulations."""
     device = grid.device if device is None else device
     return tuple(
         GridVariable(GridArray(u, offset, grid).to(device), bc)
         for u, offset, bc in zip(v, grid.cell_faces, bcs)
     )
 
+
 def wrap_vorticity(
     w: Array,
     grid: grids.Grid,
     bc: BoundaryConditions,
     device: Optional[torch.device] = None,
 ) -> GridVariable:
     """Wrap vorticity arrays for input into simulations."""
     device = grid.device if device is None else device
     return GridVariable(GridArray(w, grid.cell_faces, grid).to(device), bc)
 
 
 def _log_normal_density(k, mode: float, variance=0.25):
-    """Unscaled PDF for a log normal given `mode` and log variance 1."""
+    """
+    Unscaled PDF for a log normal given `mode` and log variance 1.
+
+
+    """
     mean = math.log(mode) + variance
     logk = torch.log(k)
     return torch.exp(-((mean - logk) ** 2) / 2 / variance - logk)
 
 
 def McWilliams_density(k, mode: float, tau: float = 1.0):
     """Implements the McWilliams spectral density function.
@@ -70,14 +75,15 @@
     tau flattens the spectrum density at low wavenumbers to be bigger.
 
     Refs:
       McWilliams, J. C. (1984). The emergence of isolated coherent vortices in turbulent flow.
     """
     return (k * (tau**2 + (k / mode) ** 4)) ** (-1)
 
+
 def _angular_frequency_magnitude(grid: grids.Grid) -> Array:
     frequencies = [
         2 * torch.pi * fft.fftfreq(size, step)
         for size, step in zip(grid.shape, grid.step)
     ]
     freq_vector = torch.stack(torch.meshgrid(*frequencies, indexing="ij"), axis=0)
     return torch.linalg.norm(freq_vector, axis=0)
@@ -91,111 +97,27 @@
     """Filter an Array with white noise to match a prescribed spectral density."""
     k = _angular_frequency_magnitude(grid)
     filters = torch.where(k > 0, spectral_density(k), 0.0)
     # The output signal can safely be assumed to be real if our input signal was
     # real, because our spectral density only depends on norm(k).
     return fft.ifftn(fft.fftn(v) * filters).real
 
+
 def streamfunc_normalize(k, psi):
-    # only half the spectrum for real ffts, needs spectral normalisation
     nx, ny = psi.shape
     psih = fft.fft2(psi)
-    uh = k * psih
-    kinetic_energy = (2 * uh.abs() ** 2 / (nx * ny) ** 2).sum()
+    uh_mag = k * psih
+    kinetic_energy = (2 * uh_mag.abs() ** 2 / (nx * ny) ** 2).sum()
     return psi / kinetic_energy.sqrt()
 
-def _rhs_transform(
-    u: GridArray,
-    bc: BoundaryConditions,
-) -> Array:
-    """Transform the RHS of pressure projection equation for stability.
-
-    In case of poisson equation, the kernel is subtracted from RHS for stability.
-
-    Args:
-      u: a GridArray that solves ∇²x = u.
-      bc: specifies boundary of x.
-
-    Returns:
-      u' s.t. u = u' + kernel of the laplacian.
-    """
-    u_data = u.data
-    for axis in range(u.grid.ndim):
-        if (
-            bc.types[axis][0] == grids.BCType.NEUMANN
-            and bc.types[axis][1] == grids.BCType.NEUMANN
-        ):
-            # if all sides are neumann, poisson solution has a kernel of constant
-            # functions. We substact the mean to ensure consistency.
-            u_data = u_data - torch.mean(u_data)
-    return u_data
-
-
-def solve_fast_diag(
-    v: GridVariableVector,
-    q0: Optional[GridVariable] = None,
-    pressure_bc: Optional[grids.ConstantBoundaryConditions] = None,
-    implementation: Optional[str] = None,
-) -> GridArray:
-    """Solve for pressure using the fast diagonalization approach."""
-    del q0  # unused
-    if pressure_bc is None:
-        pressure_bc = grids.get_pressure_bc_from_velocity(v)
-    if grids.has_all_periodic_boundary_conditions(*v):
-        circulant = True
-    else:
-        circulant = False
-        # only matmul implementation supports non-circulant matrices
-        implementation = "matmul"
-    grid = grids.consistent_grid(*v)
-    rhs = fd.divergence(v)
-    laplacians = list(map(fd.laplacian_matrix, grid.shape, grid.step))
-    laplacians = [lap.to(grid.device) for lap in laplacians]
-    rhs_transformed = _rhs_transform(rhs, pressure_bc)
-    pinv = solver.pseudoinverse(
-        rhs_transformed,
-        laplacians,
-        rhs_transformed.dtype,
-        hermitian=True,
-        circulant=circulant,
-        implementation=implementation,
-    )
-    # return applied(pinv)(rhs_transformed)
-    return GridArray(pinv, rhs.offset, rhs.grid)
-
-
-def projection(
-    v: GridVariableVector,
-    solve: Callable = solve_fast_diag,
-) -> GridVariableVector:
-    """
-    Apply pressure projection (a discrete Helmholtz decomposition)
-    to make a velocity field divergence free.
-    
-    Note by S.Cao: this was originally implemented by the jax-cfd team
-    but using FDM results having a non-negligible error in fp32. 
-    One resolution is to use fp64 then cast back to fp32.
-    """
-    grid = grids.consistent_grid(*v)
-    pressure_bc = grids.get_pressure_bc_from_velocity(v)
-
-    q0 = GridArray(torch.zeros(grid.shape), grid.cell_center, grid)
-    q0 = pressure_bc.impose_bc(q0)
-
-    q = solve(v, q0, pressure_bc)
-    q = pressure_bc.impose_bc(q)
-    q_grad = fd.forward_difference(q)
-    v_projected = tuple(u.bc.impose_bc(u.array - q_g) for u, q_g in zip(v, q_grad))
-    return v_projected
-
 
 def project_and_normalize(
     v: GridVariableVector, maximum_velocity: float = 1
 ) -> GridVariableVector:
-    v = projection(v)
+    v = pressure.projection(v)
     vmax = torch.linalg.norm(torch.stack([u.data for u in v]), dim=0).max()
     v = tuple(GridVariable(maximum_velocity * u.array / vmax, u.bc) for u in v)
     return v
 
 
 def filtered_velocity_field(
     grid: grids.Grid,
@@ -252,15 +174,14 @@
 ) -> GridArray:
     """Create vorticity field with a spectral filtering
     using the McWilliams power spectrum density function.
 
     Args:
       rng_key: key for seeding the random initial vorticity field.
       grid: the grid on which the vorticity field is defined.
-      maximum_velocity: the maximum speed in the velocity field.
       peak_wavenumber: the velocity field will be filtered so that the largest
         magnitudes are associated with this wavenumber.
 
     Returns:
       A vorticity field with periodic boundary condition.
     """
 
@@ -273,8 +194,8 @@
     k = _angular_frequency_magnitude(grid)
     psi = spectral_filter(spectral_density, noise, grid)
     psi = streamfunc_normalize(k, psi)
     vorticity = fft.ifftn(fft.fftn(psi) * k**2).real
     boundary_condition = grids.periodic_boundary_conditions(grid.ndim)
     vorticity = wrap_vorticity(vorticity, grid, boundary_condition)
 
-    return vorticity
+    return vorticity
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `torch_cfd-0.0.4/torch_cfd/tensor_utils.py` & `torch_cfd-0.0.5/torch_cfd/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `torch_cfd-0.0.4/torch_cfd.egg-info/PKG-INFO` & `torch_cfd-0.0.5/torch_cfd.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-cfd
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyTorch CFD
 Home-page: https://github.com/scaomath/torch-cfd
 Author: Shuhao Cao
 Author-email: scao.math@gmail.com
 License: Apache-2.0
 Keywords: pytorch,cfd,pde,spectral
 Classifier: Development Status :: 4 - Beta
```

