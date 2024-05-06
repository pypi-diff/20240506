# Comparing `tmp/hexfft-0.1.1.tar.gz` & `tmp/hexfft-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexfft-0.1.1.tar", last modified: Fri May  3 02:59:59 2024, max compression
+gzip compressed data, was "hexfft-0.1.2.tar", last modified: Mon May  6 04:12:34 2024, max compression
```

## Comparing `hexfft-0.1.1.tar` & `hexfft-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-03 02:59:59.797245 hexfft-0.1.1/
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-03 02:59:59.790383 hexfft-0.1.1/.github/
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-03 02:59:59.792371 hexfft-0.1.1/.github/workflows/
--rw-r--r--   0 chris      (501) staff       (20)     1094 2024-04-24 02:26:15.000000 hexfft-0.1.1/.github/workflows/python-package-conda.yml
--rw-r--r--   0 chris      (501) staff       (20)     1078 2024-04-06 16:16:22.000000 hexfft-0.1.1/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)     1102 2024-05-03 02:59:59.796955 hexfft-0.1.1/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      840 2024-04-25 02:53:04.000000 hexfft-0.1.1/README.md
--rw-r--r--   0 chris      (501) staff       (20)       55 2024-04-25 02:06:04.000000 hexfft-0.1.1/environment.yml
--rw-r--r--   0 chris      (501) staff       (20)      359 2024-05-03 02:58:27.000000 hexfft-0.1.1/pyproject.toml
--rw-r--r--   0 chris      (501) staff       (20)       22 2024-04-25 02:06:20.000000 hexfft-0.1.1/requirements.txt
--rw-r--r--   0 chris      (501) staff       (20)       38 2024-05-03 02:59:59.797287 hexfft-0.1.1/setup.cfg
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-03 02:59:59.790620 hexfft-0.1.1/src/
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-03 02:59:59.794534 hexfft-0.1.1/src/hexfft/
--rw-r--r--   0 chris      (501) staff       (20)       84 2024-04-25 00:42:25.000000 hexfft-0.1.1/src/hexfft/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     4435 2024-05-03 01:21:02.000000 hexfft-0.1.1/src/hexfft/array.py
--rw-r--r--   0 chris      (501) staff       (20)     2245 2024-04-23 19:01:41.000000 hexfft-0.1.1/src/hexfft/grids.py
--rw-r--r--   0 chris      (501) staff       (20)    21147 2024-05-03 02:57:35.000000 hexfft-0.1.1/src/hexfft/hexfft.py
--rw-r--r--   0 chris      (501) staff       (20)     3722 2024-04-26 04:17:34.000000 hexfft-0.1.1/src/hexfft/plot.py
--rw-r--r--   0 chris      (501) staff       (20)     2896 2024-04-30 13:13:15.000000 hexfft-0.1.1/src/hexfft/reference.py
--rw-r--r--   0 chris      (501) staff       (20)     3841 2024-04-25 02:21:17.000000 hexfft-0.1.1/src/hexfft/utils.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-03 02:59:59.796617 hexfft-0.1.1/src/hexfft.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     1102 2024-05-03 02:59:59.000000 hexfft-0.1.1/src/hexfft.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      450 2024-05-03 02:59:59.000000 hexfft-0.1.1/src/hexfft.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2024-05-03 02:59:59.000000 hexfft-0.1.1/src/hexfft.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)        7 2024-05-03 02:59:59.000000 hexfft-0.1.1/src/hexfft.egg-info/top_level.txt
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-03 02:59:59.796158 hexfft-0.1.1/tests/
--rw-r--r--   0 chris      (501) staff       (20)     4025 2024-05-03 02:57:35.000000 hexfft-0.1.1/tests/test_api.py
--rw-r--r--   0 chris      (501) staff       (20)     9604 2024-05-03 02:57:35.000000 hexfft-0.1.1/tests/test_hexfft.py
--rw-r--r--   0 chris      (501) staff       (20)     3180 2024-04-25 02:31:28.000000 hexfft-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-06 04:12:34.803244 hexfft-0.1.2/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-06 04:12:34.793331 hexfft-0.1.2/.github/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-06 04:12:34.795053 hexfft-0.1.2/.github/workflows/
+-rw-r--r--   0 chris      (501) staff       (20)     1094 2024-04-24 02:26:15.000000 hexfft-0.1.2/.github/workflows/python-package-conda.yml
+-rw-r--r--   0 chris      (501) staff       (20)     1078 2024-04-06 16:16:22.000000 hexfft-0.1.2/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)      954 2024-05-06 04:12:34.802992 hexfft-0.1.2/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      691 2024-05-06 04:06:16.000000 hexfft-0.1.2/README.md
+-rw-r--r--   0 chris      (501) staff       (20)       55 2024-04-25 02:06:04.000000 hexfft-0.1.2/environment.yml
+-rw-r--r--   0 chris      (501) staff       (20)      359 2024-05-06 04:11:25.000000 hexfft-0.1.2/pyproject.toml
+-rw-r--r--   0 chris      (501) staff       (20)       22 2024-04-25 02:06:20.000000 hexfft-0.1.2/requirements.txt
+-rw-r--r--   0 chris      (501) staff       (20)       38 2024-05-06 04:12:34.803290 hexfft-0.1.2/setup.cfg
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-06 04:12:34.793542 hexfft-0.1.2/src/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-06 04:12:34.798412 hexfft-0.1.2/src/hexfft/
+-rw-r--r--   0 chris      (501) staff       (20)       84 2024-04-25 00:42:25.000000 hexfft-0.1.2/src/hexfft/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     4435 2024-05-03 01:21:02.000000 hexfft-0.1.2/src/hexfft/array.py
+-rw-r--r--   0 chris      (501) staff       (20)     2245 2024-05-05 20:31:48.000000 hexfft-0.1.2/src/hexfft/grids.py
+-rw-r--r--   0 chris      (501) staff       (20)    21129 2024-05-06 04:00:00.000000 hexfft-0.1.2/src/hexfft/hexfft.py
+-rw-r--r--   0 chris      (501) staff       (20)     3722 2024-04-26 04:17:34.000000 hexfft-0.1.2/src/hexfft/plot.py
+-rw-r--r--   0 chris      (501) staff       (20)     2896 2024-05-06 04:04:31.000000 hexfft-0.1.2/src/hexfft/reference.py
+-rw-r--r--   0 chris      (501) staff       (20)     3841 2024-04-25 02:21:17.000000 hexfft-0.1.2/src/hexfft/utils.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-06 04:12:34.802693 hexfft-0.1.2/src/hexfft.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)      954 2024-05-06 04:12:34.000000 hexfft-0.1.2/src/hexfft.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      450 2024-05-06 04:12:34.000000 hexfft-0.1.2/src/hexfft.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2024-05-06 04:12:34.000000 hexfft-0.1.2/src/hexfft.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)        7 2024-05-06 04:12:34.000000 hexfft-0.1.2/src/hexfft.egg-info/top_level.txt
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-06 04:12:34.802274 hexfft-0.1.2/tests/
+-rw-r--r--   0 chris      (501) staff       (20)     4025 2024-05-03 02:57:35.000000 hexfft-0.1.2/tests/test_api.py
+-rw-r--r--   0 chris      (501) staff       (20)     9893 2024-05-06 04:04:02.000000 hexfft-0.1.2/tests/test_hexfft.py
+-rw-r--r--   0 chris      (501) staff       (20)     3180 2024-04-25 02:31:28.000000 hexfft-0.1.2/tests/test_utils.py
```

### Comparing `hexfft-0.1.1/.github/workflows/python-package-conda.yml` & `hexfft-0.1.2/.github/workflows/python-package-conda.yml`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.1/LICENSE` & `hexfft-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.1/src/hexfft/array.py` & `hexfft-0.1.2/src/hexfft/array.py`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.1/src/hexfft/grids.py` & `hexfft-0.1.2/src/hexfft/grids.py`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.1/src/hexfft/hexfft.py` & `hexfft-0.1.2/src/hexfft/hexfft.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
 class RectPeriodicFFT(HexagonalFFT):
     def __init__(self, shape, dtype):
         super().__init__(shape, dtype)
 
     def _precompute(self):
         N1, N2 = self.shape
         self.phase_shift = np.exp(
-            1.0j * np.pi * np.array([i * np.arange(N2) for i in range(N1)]) / N1
+            1.0j * np.pi * np.array([i * np.arange(N2) for i in range(N1)]) / N2
         )
         self.phase_shift_conj = np.conj(self.phase_shift)
 
     def _forward(self, x):
         assert (
             x.shape[-2:] == self.shape
         ), f"Input array with shape {x.shape} does not match FFT object shape {self.shape}"
@@ -250,17 +250,17 @@
         if shift:
             x = rect_shift(x)
 
         squeeze = x.ndim == 2
         if squeeze:
             x = np.expand_dims(x, 0)
 
-        F1 = scipy.fft.fft(x, axis=1)
+        F1 = scipy.fft.fft(x, axis=2)
         F2 = F1 * self.phase_shift
-        X = scipy.fft.fft(F2, axis=2)
+        X = scipy.fft.fft(F2, axis=1)
 
         if squeeze:
             X = np.squeeze(X)
 
         if shift:
             X = rect_unshift(HexArray(X, "oblique"))
         else:
@@ -280,17 +280,17 @@
         if shift:
             X = rect_shift(X)
 
         squeeze = X.ndim == 2
         if squeeze:
             X = np.expand_dims(X, 0)
 
-        F2 = scipy.fft.ifft(X, axis=2)
+        F2 = scipy.fft.ifft(X, axis=1)
         F1 = F2 * self.phase_shift_conj
-        x = HexArray(scipy.fft.ifft(F1, axis=1), "oblique")
+        x = HexArray(scipy.fft.ifft(F1, axis=2), "oblique")
 
         if squeeze:
             x = np.squeeze(x)
 
         if shift:
             x = rect_unshift(HexArray(x, "oblique"))
         else:
@@ -664,30 +664,30 @@
 
 
 def rect_fft(x):
     dtype = x.dtype
     cdtype = complex_type(dtype)
 
     N1, N2 = x.shape
-    F1 = HexArray(scipy.fft.fft(x, axis=0), "oblique")
+    F1 = scipy.fft.fft(x, axis=1)
     exp_factor = np.exp(
-        1.0j * np.pi * np.array([i * np.arange(N2) for i in range(N1)]) / N1
+        1.0j * np.pi * np.array([i * np.arange(N2) for i in range(N1)]) / N2
     ).astype(cdtype)
     F2 = F1 * exp_factor
-    F = HexArray(np.fft.fft(F2, axis=1), "oblique")
+    F = HexArray(scipy.fft.fft(F2, axis=0), "oblique")
 
     return F
 
 
 def rect_ifft(X):
     dtype = X.dtype
     cdtype = complex_type(dtype)
 
     N1, N2 = X.shape
-    F2 = scipy.fft.ifft(X, axis=1)
+    F2 = scipy.fft.ifft(X, axis=0)
     exp_factor = np.exp(
-        -1.0j * np.pi * np.array([i * np.arange(N2) for i in range(N1)]) / N1
+        -1.0j * np.pi * np.array([i * np.arange(N2) for i in range(N1)]) / N2
     ).astype(cdtype)
     F1 = F2 * exp_factor
-    x = HexArray(scipy.fft.ifft(F1, axis=0), "oblique")
+    x = HexArray(scipy.fft.ifft(F1, axis=1), "oblique")
 
     return x
```

### Comparing `hexfft-0.1.1/src/hexfft/plot.py` & `hexfft-0.1.2/src/hexfft/plot.py`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.1/src/hexfft/reference.py` & `hexfft-0.1.2/src/hexfft/reference.py`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.1/src/hexfft/utils.py` & `hexfft-0.1.2/src/hexfft/utils.py`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.1/tests/test_api.py` & `hexfft-0.1.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `hexfft-0.1.1/tests/test_hexfft.py` & `hexfft-0.1.2/tests/test_hexfft.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from hexfft.reference import (
     _hexdft_slow,
     _hexidft_slow,
     _rect_dft_slow,
     _rect_idft_slow,
 )
 import numpy as np
+import pytest
 
 
 def hregion(n1, n2, center, size, pattern="oblique"):
     """
     return mask for a hexagonal region of support
     with side length size centered at center
     """
@@ -108,30 +109,31 @@
         impulse_p_T = _hexidft_pgram_stack(IMPULSE_P)
         impulse_single_p_T = _hexidft_pgram(IMPULSE_SINGLE_P)
         assert np.allclose(impulse_p_T[0], impulse_single_p_T)
 
         assert np.allclose(impulse_p, impulse_p_T, atol=1e-12)
 
 
-def test_rect_hexdft():
+@pytest.mark.skip(reason="reference slow DFT implementation TODO")
+def test_rect_dft():
     # test rect dft and idft
     for shape in [(4, 5), (8, 8), (11, 16), (19, 19)]:
         N1, N2 = shape
         # N2 must be even
         N2 = N1 + N1 % 2
         n1, n2 = np.meshgrid(np.arange(N1), np.arange(N2))
         center = (N1 / 2 - 1, N2 / 2 - 1)
         d = hregion(n1, n2, center, 1)
 
         D = _rect_dft_slow(d)
         dd = _rect_idft_slow(D)
-
         assert np.allclose(d, dd, atol=1e-12)
 
 
+@pytest.mark.skip(reason="reference slow DFT implementation TODO")
 def test_rect_fft():
     for pattern in ["oblique", "offset"]:
         for shape in [(4, 5), (8, 8), (11, 16), (19, 19)]:
             N1, N2 = shape
             n1, n2 = np.meshgrid(np.arange(N1), np.arange(N2))
             center = (N1 // 2 - 1, N2 // 2 - 1)
             d = rect_shift(hregion(n1, n2, center, 1, "offset"))
@@ -143,22 +145,26 @@
 
             dd = rect_ifft(D)
             dd_slow = _rect_idft_slow(D_slow)
 
             assert np.allclose(dd, dd_slow)
 
 
-# def test_validate_rect_fft():
-#     for shape in [ (8, 8), (11, 16), (19, 19)]:
-#         N1, N2 = shape
-#         n1, n2 = np.meshgrid(np.arange(N1), np.arange(N2), indexing="ij")
-#         mode1 = HexArray(np.exp(-2 * np.pi * 1.0j * n1/N1), "oblique")
+@pytest.mark.parametrize("shape", [(16, 16), (17, 17), (16, 17), (17, 16)])
+@pytest.mark.parametrize("mode", [(0, 0), (1, 0), (0, 1), (1, 1), (2, 2), (5, 7)])
+def test_validate_rect_fft(shape, mode):
+    N1, N2 = shape
+    k1, k2 = mode
+    n1, n2 = np.meshgrid(np.arange(N2), np.arange(N1))
+    fmode = HexArray(
+        np.exp(2 * np.pi * 1.0j * (k1 * (n1 - n2 / 2) / N2 + k2 * n2 / N1)), "oblique"
+    )
+    FMODE = rect_fft(fmode)
 
-#         M1 = fft(rect_unshift(mode1))
-#         assert np.real(M1[0, 1]) == 1.
+    assert np.allclose(FMODE[k2, k1], N1 * N2)
 
 
 def test_rect_fft_stack():
     # create a stack of data
     nstack, N1, N2 = 5, 8, 12
     n1, n2 = np.meshgrid(np.arange(N1), np.arange(N2))
     center = (N1 / 2 - 1, N2 / 2 - 1)
```

### Comparing `hexfft-0.1.1/tests/test_utils.py` & `hexfft-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

