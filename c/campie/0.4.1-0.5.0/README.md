# Comparing `tmp/campie-0.4.1.tar.gz` & `tmp/campie-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "campie-0.4.1.tar", max compression
+gzip compressed data, was "campie-0.5.0.tar", max compression
```

## Comparing `campie-0.4.1.tar` & `campie-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11356 2024-04-04 00:23:23.721804 campie-0.4.1/LICENSE
--rw-r--r--   0        0        0     3400 2024-04-04 00:23:23.721935 campie-0.4.1/README.md
--rw-r--r--   0        0        0     1222 2024-04-04 00:23:23.722168 campie-0.4.1/campie/__init__.py
--rw-r--r--   0        0        0    12332 2024-04-04 00:24:41.350085 campie-0.4.1/campie/cam.py
--rw-r--r--   0        0        0     5980 2024-04-04 00:23:23.722499 campie-0.4.1/campie/kernel.py
--rw-r--r--   0        0        0        0 2024-04-04 00:23:23.722558 campie-0.4.1/campie/py.typed
--rw-r--r--   0        0        0     9194 2024-04-04 00:23:23.722763 campie-0.4.1/campie/run.py
--rw-r--r--   0        0        0     4020 2024-04-04 00:23:23.722894 campie-0.4.1/campie/types.py
--rw-r--r--   0        0        0      801 2024-04-04 00:23:23.723083 campie-0.4.1/campie/util/__init__.py
--rw-r--r--   0        0        0     4011 2024-04-04 00:23:23.723209 campie-0.4.1/campie/util/flip_indices.py
--rw-r--r--   0        0        0     1288 2024-04-04 00:23:23.723329 campie-0.4.1/campie/util/helpers.py
--rw-r--r--   0        0        0     3075 2024-04-04 00:23:23.723457 campie-0.4.1/campie/validation.py
--rw-r--r--   0        0        0      845 2024-04-04 00:24:05.165839 campie-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4330 1970-01-01 00:00:00.000000 campie-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-06 21:41:47.132207 campie-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3400 2024-05-06 21:41:47.132269 campie-0.5.0/README.md
+-rw-r--r--   0        0        0     1398 2024-05-06 21:41:47.132357 campie-0.5.0/campie/__init__.py
+-rw-r--r--   0        0        0    18325 2024-05-06 21:45:00.400800 campie-0.5.0/campie/cam.py
+-rw-r--r--   0        0        0     7807 2024-05-06 21:41:47.132549 campie-0.5.0/campie/kernel.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:41:47.132573 campie-0.5.0/campie/py.typed
+-rw-r--r--   0        0        0     9189 2024-05-06 21:41:47.132676 campie-0.5.0/campie/run.py
+-rw-r--r--   0        0        0     4405 2024-05-06 21:41:47.132768 campie-0.5.0/campie/types.py
+-rw-r--r--   0        0        0      801 2024-05-06 21:41:47.132875 campie-0.5.0/campie/util/__init__.py
+-rw-r--r--   0        0        0     4011 2024-05-06 21:41:47.132948 campie-0.5.0/campie/util/flip_indices.py
+-rw-r--r--   0        0        0     1288 2024-05-06 21:41:47.133016 campie-0.5.0/campie/util/helpers.py
+-rw-r--r--   0        0        0     3367 2024-05-06 21:41:47.133100 campie-0.5.0/campie/validation.py
+-rw-r--r--   0        0        0      845 2024-05-06 21:44:10.997789 campie-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4330 1970-01-01 00:00:00.000000 campie-0.5.0/PKG-INFO
```

### Comparing `campie-0.4.1/LICENSE` & `campie-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `campie-0.4.1/README.md` & `campie-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `campie-0.4.1/campie/__init__.py` & `campie-0.5.0/campie/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,24 +18,30 @@
 Python APIs to simulate various CAMs (Content Addressable Memory) on GPUs at scale.
 """
 
 import importlib.metadata
 
 from .cam import (
     acam_count_mismatches,
+    acam_double_count_mismatches,
+    acam_double_match,
+    acam_double_reduce_sum,
     acam_match,
     acam_reduce_sum,
     tcam_hamming_distance,
     tcam_match,
     tcam_reduce_sum,
 )
 from .util import flip_indices
 
 __all__ = [
     "acam_count_mismatches",
+    "acam_double_count_mismatches",
+    "acam_double_match",
+    "acam_double_reduce_sum",
     "acam_match",
     "acam_reduce_sum",
     "flip_indices",
     "tcam_hamming_distance",
     "tcam_match",
     "tcam_reduce_sum",
 ]
```

### Comparing `campie-0.4.1/campie/cam.py` & `campie-0.5.0/campie/cam.py`

 * *Files 18% similar despite different names*

```diff
@@ -258,7 +258,131 @@
     """
     variant, op, result_dtype = CamVariant.ACAM, CamOp.REDUCE_SUM, values.dtype
     validate_args(variant, op, inputs, cam, values)
     kernel = generate_kernel(variant, op, inputs.dtype, cam.dtype, result_dtype)
     if noise is not None:
         cam = add_noise(cam, noise)
     return run_kernel(kernel, variant, op, inputs, cam, result_dtype, values)
+
+
+def acam_double_match(
+    inputs: NDArray[TN], cam: NDArray[TN], *, noise: Optional[float] = None
+) -> NDArray[np.int8]:
+    """
+    Performs the matching operation of a ACAM (Analog CAM) with double precision on a given set of inputs and
+    ACAMs.
+
+    ### Positional Arguments:
+    - `inputs` (`numpy.ndarray` or `cupy.ndarray`): The input columns stacked in rows.
+      The two innermost dimensions of `inputs` are of shape `input_rows x columns`.
+    - `cam` (`numpy.ndarray` or `cupy.ndarray`): The ACAM matrix itself.
+      The lower and upper thresholds are encoded side-by-side within the column.
+      This means that your CAM columns should be twice as wide as your input columns.
+      "Don't Care" (or "X") thresholds are encoded as `numpy.nan` values when using
+      float types and as negative integers when using integer types.
+      The two innermost dimensions of `cam` are of shape `cam_rows x (columns * 2)`.
+
+    ### Keyword Arguments:
+    - `noise` (`float` [optional]): Standard deviation for a normal distribution
+      `N(0, noise)` that is randomly sampled from and added to the ACAM thresholds
+      to simulate analog inaccuracies before performing the operation. Noise is only
+      added if this argument is defined.
+
+    ### Returns:
+    `cupy.ndarray`: The resulting matrix of matches encoded as `np.int8`s.
+    The two innermost dimensions are of shape `input_rows x cam_rows`.
+
+    ### Notes:
+    - The arguments for ACAM operations must contain floating point data types.
+    """
+    variant, op, result_dtype = CamVariant.ACAM_DOUBLE, CamOp.MATCH, np.int8
+    validate_args(variant, op, inputs, cam)
+    kernel = generate_kernel(variant, op, inputs.dtype, cam.dtype, result_dtype)
+    if noise is not None:
+        cam = add_noise(cam, noise)
+    return run_kernel(kernel, variant, op, inputs, cam, result_dtype)
+
+
+def acam_double_count_mismatches(
+    inputs: NDArray[TN], cam: NDArray[TN], *, noise: Optional[float] = None
+) -> NDArray[np.int64]:
+    """
+    Determines the number of mismatches per row in a ACAM (Analog CAM) matching
+    operation for a given set of inputs and ACAMs.
+
+    ### Positional Arguments:
+    - `inputs` (`numpy.ndarray` or `cupy.ndarray`): The input columns stacked in rows.
+      The two innermost dimensions of `inputs` are of shape `input_rows x columns`.
+    - `cam` (`numpy.ndarray` or `cupy.ndarray`): The ACAM matrix itself.
+      The lower and upper thresholds are encoded side-by-side within the column.
+      This means that your CAM columns should be twice as wide as your input columns.
+      "Don't Care" (or "X") thresholds are encoded as `numpy.nan` values when using
+      float types and as negative integers when using integer types.
+      The two innermost dimensions of `cam` are of shape `cam_rows x (columns * 2)`.
+
+    ### Keyword Arguments:
+    - `noise` (`float` [optional]): Standard deviation for a normal distribution
+      `N(0, noise)` that is randomly sampled from and added to the ACAM thresholds
+      to simulate analog inaccuracies before performing the operation. Noise is only
+      added if this argument is defined.
+
+    ### Returns:
+    `cupy.ndarray`: The resulting matrix of mismatch counts encoded as `np.int64`s.
+    The two innermost dimensions are of shape `input_rows x cam_rows`.
+
+    ### Notes:
+    - The arguments for ACAM operations must contain floating point data types.
+    """
+    variant, op, result_dtype = CamVariant.ACAM_DOUBLE, CamOp.COUNT_MISMATCHES, np.int64
+    validate_args(variant, op, inputs, cam)
+    kernel = generate_kernel(variant, op, inputs.dtype, cam.dtype, result_dtype)
+    if noise is not None:
+        cam = add_noise(cam, noise)
+    return run_kernel(kernel, variant, op, inputs, cam, result_dtype)
+
+
+def acam_double_reduce_sum(
+    inputs: NDArray[TN],
+    cam: NDArray[TN],
+    *,
+    values: NDArray[UF],
+    noise: Optional[float] = None,
+) -> NDArray[UF]:
+    """
+    First performs the matching operation of a ACAM (Analog CAM) on a given set
+    of inputs and ACAMs, then reduces each row of inputs down to a single number
+    by accumulating over a set of values for every matched row.
+
+    Note that reduction operations do not support broadcasting.
+
+    ### Positional Arguments:
+    - `inputs` (`numpy.ndarray` or `cupy.ndarray`): The input columns stacked in rows.
+      The two innermost dimensions of `inputs` are of shape `input_rows x columns`.
+    - `cam` (`numpy.ndarray` or `cupy.ndarray`): The ACAM matrix itself.
+      The lower and upper thresholds are encoded side-by-side within the column.
+      This means that your CAM columns should be twice as wide as your input columns.
+      "Don't Care" (or "X") thresholds are encoded as `numpy.nan` values when using
+      float types and as negative integers when using integer types.
+      The two innermost dimensions of `cam` are of shape `cam_rows x (columns * 2)`.
+
+    ### Keyword Arguments:
+    - `values` (`numpy.ndarray` or `cupy.ndarray`): The values to reduce.
+      The dimensions of `values` must be the same as the dimensions of `cam`,
+      except for the omission of the `columns` dimension.
+    - `noise` (`float` [optional]): Standard deviation for a normal distribution
+      `N(0, noise)` that is randomly sampled from and added to the ACAM thresholds
+      to simulate analog inaccuracies before performing the operation. Noise is only
+      added if this argument is defined.
+
+    ### Returns:
+    `cupy.ndarray`: The reduction result matrix.
+    The innermost dimension is `input_rows`.
+
+    ### Notes:
+    - The arguments for ACAM operations must contain floating point data types.
+    """
+    variant, op, result_dtype = CamVariant.ACAM_DOUBLE, CamOp.REDUCE_SUM, values.dtype
+    validate_args(variant, op, inputs, cam, values)
+    kernel = generate_kernel(variant, op, inputs.dtype, cam.dtype, result_dtype)
+    if noise is not None:
+        cam = add_noise(cam, noise)
+    return run_kernel(kernel, variant, op, inputs, cam, result_dtype, values)
```

### Comparing `campie-0.4.1/campie/run.py` & `campie-0.5.0/campie/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     The reason behind this is that the CUDA kernels themselves only support inputs with
     equal dimensions for simplicity. This function makes the necessary calculations such
     that asymmetrical dimensions are flattened down to symmetrical ones before the
     kernel call, and restored later before returning the results.
     """
 
     input_rows, cam_rows = inputs.shape[-2], cam.shape[-2]
-    columns = cam.shape[-1] // variant.cell_encoding_width
+    columns = cam.shape[-1] // variant.cam_cell_width
 
     # while the two innermost shapes of `inputs` and `cam` are `input_rows x columns`
     # and `cam_rows x columns` respectively, the remaining outer shapes hold all the
     # information on how the inputs are stacked and to be broadcasted.
     inputs_outer_shape, cam_outer_shape = inputs.shape[:-2], cam.shape[:-2]
 
     # sort the outer shapes by length. we expect the smaller shape (`sub_shape`) to be
```

### Comparing `campie-0.4.1/campie/types.py` & `campie-0.5.0/campie/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,27 +23,42 @@
 
 class CamVariant(Enum):
     """All supported variants of CAMs."""
 
     ACAM = auto()
     """Analog CAM."""
 
+    ACAM_DOUBLE = auto()
+    """Analog CAM with double the bit width."""
+
     TCAM = auto()
     """Ternary CAM."""
 
     @property
-    def cell_encoding_width(self) -> int:
+    def cam_cell_width(self) -> int:
         """
-        The amount of elements in a CAM row that is used
+        The amount of cells in a CAM row that is used
         to encode a single CAM cell.
         """
 
         if self == CamVariant.ACAM:
             return 2
+        if self == CamVariant.ACAM_DOUBLE:
+            return 4
+        return 1
 
+    @property
+    def input_cell_width(self) -> int:
+        """
+        The amount of cells in an input row that is used
+        to encode a single input cell.
+        """
+
+        if self == CamVariant.ACAM_DOUBLE:
+            return 2
         return 1
 
 
 class CamOp(Enum):
     """All supported operations on CAMs."""
 
     MATCH = auto()
```

### Comparing `campie-0.4.1/campie/util/__init__.py` & `campie-0.5.0/campie/util/__init__.py`

 * *Files identical despite different names*

### Comparing `campie-0.4.1/campie/util/flip_indices.py` & `campie-0.5.0/campie/util/flip_indices.py`

 * *Files identical despite different names*

### Comparing `campie-0.4.1/campie/util/helpers.py` & `campie-0.5.0/campie/util/helpers.py`

 * *Files identical despite different names*

### Comparing `campie-0.4.1/campie/validation.py` & `campie-0.5.0/campie/validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,24 +52,32 @@
 
     if len(inputs.shape) < 2:
         raise ValueError("inputs are one-dimensional")
 
     if len(cam.shape) < 2:
         raise ValueError("cam is one-dimensional")
 
-    cell_encoding_width = variant.cell_encoding_width
+    cam_cell_width = variant.cam_cell_width
+    if cam.shape[-1] % cam_cell_width != 0:
+        raise ValueError(
+            "amount of CAM columns is not divisible by CAM cell encoding width: "
+            f"{cam_cell_width} (columns found: {cam.shape[-1]})"
+        )
 
-    if inputs.shape[-1] != cam.shape[-1] // cell_encoding_width:
+    input_cell_width = variant.input_cell_width
+    if inputs.shape[-1] % input_cell_width != 0:
         raise ValueError(
-            f"input and cam column sizes are not equal ({inputs.shape[-1]} vs {cam.shape[-1] // cell_encoding_width})"  # noqa: E501
+            "amount of input columns is not divisible by input cell encoding width: "
+            f"{input_cell_width} (columns found: {inputs.shape[-1]})"
         )
 
-    if cam.shape[-1] % cell_encoding_width != 0:
+    if inputs.shape[-1] // input_cell_width != cam.shape[-1] // cam_cell_width:
         raise ValueError(
-            f"amount of columns not divisible by cell encoding width {cell_encoding_width} (columns: {cam.shape[-1]})"  # noqa: E501
+            "input and cam column sizes do not match "
+            f"a ratio of {input_cell_width}:{cam_cell_width}"
         )
 
     if op.is_reduction:
         assert reduction_values is not None
         if len(reduction_values.shape) > 1:
             raise ValueError("reduction values must be one-dimensional")
         if len(inputs.shape) > 2 or len(cam.shape) > 2:
@@ -78,9 +86,10 @@
             raise ValueError("CAM shape does not match reduction value shape")
 
     inputs_outer_shape, cam_outer_shape = inputs.shape[:-2], cam.shape[:-2]
 
     for i in range(1, min(len(inputs_outer_shape), len(cam_outer_shape)) + 1):
         if inputs_outer_shape[-i] != cam_outer_shape[-i]:
             raise ValueError(
-                f"the outer shapes of input and cam are incompatible: {inputs_outer_shape} vs {cam_outer_shape}"  # noqa: E501
+                "the outer shapes of input and cam are incompatible: "
+                f"{inputs_outer_shape} vs {cam_outer_shape}"
             )
```

### Comparing `campie-0.4.1/pyproject.toml` & `campie-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "campie"
-version = "0.4.1"
+version = "0.5.0"
 description = "Python APIs to simulate various CAMs on GPUs at scale"
 readme = "README.md"
 authors = []
 repository = "https://github.com/HewlettPackard/CAMPIE"
 homepage = "https://github.com/HewlettPackard/CAMPIE#readme"
 packages = [{ include = "campie" }]
```

### Comparing `campie-0.4.1/PKG-INFO` & `campie-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: campie
-Version: 0.4.1
+Version: 0.5.0
 Summary: Python APIs to simulate various CAMs on GPUs at scale
 Home-page: https://github.com/HewlettPackard/CAMPIE#readme
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

