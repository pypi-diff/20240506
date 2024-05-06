# Comparing `tmp/doppy-0.1.4.tar.gz` & `tmp/doppy-0.2.0.tar.gz`

## Comparing `doppy-0.1.4.tar` & `doppy-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
--rw-r--r--   0     1001      127      206 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doprs/Cargo.toml
--rw-r--r--   0     1001      127       21 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doprs/.gitignore
--rw-r--r--   0     1001      127       13 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doprs/src/lib.rs
--rw-r--r--   0     1001      127     2043 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doprs/src/raw/error.rs
--rw-r--r--   0     1001      127     9448 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doprs/src/raw/halo_hpl.rs
--rw-r--r--   0     1001      127       33 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doprs/src/raw.rs
--rw-r--r--   0        0        0      420 1970-01-01 00:00:00.000000 doppy-0.1.4/crates/doppy_rs/Cargo.toml
--rw-r--r--   0     1001      127      279 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doppy_rs/src/lib.rs
--rw-r--r--   0     1001      127     4526 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doppy_rs/src/raw/halo_hpl.rs
--rw-r--r--   0     1001      127      204 2024-04-23 13:09:28.000000 doppy-0.1.4/crates/doppy_rs/src/raw.rs
--rw-r--r--   0     1001      127    18041 2024-04-23 13:09:39.000000 doppy-0.1.4/Cargo.lock
--rw-r--r--   0        0        0      182 1970-01-01 00:00:00.000000 doppy-0.1.4/Cargo.toml
--rw-r--r--   0     1001      127     2398 2024-04-23 13:09:28.000000 doppy-0.1.4/pyproject.toml
--rw-r--r--   0     1001      127      205 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/options.py
--rw-r--r--   0     1001      127        0 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/py.typed
--rw-r--r--   0     1001      127     4809 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/raw/halo_bg.py
--rw-r--r--   0     1001      127    18625 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/raw/halo_hpl.py
--rw-r--r--   0     1001      127     9685 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/raw/windcube.py
--rw-r--r--   0     1001      127     3937 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/raw/halo_sys_params.py
--rw-r--r--   0     1001      127      194 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/raw/__init__.py
--rw-r--r--   0     1001      127     1735 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/data/api.py
--rw-r--r--   0     1001      127      996 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/data/cache.py
--rw-r--r--   0     1001      127        0 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/data/__init__.py
--rw-r--r--   0     1001      127       89 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/data/exceptions.py
--rw-r--r--   0     1001      127      191 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/__init__.py
--rw-r--r--   0     1001      127      248 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/bench.py
--rw-r--r--   0     1001      127    19733 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/product/stare.py
--rw-r--r--   0     1001      127      103 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/product/__init__.py
--rw-r--r--   0     1001      127    11133 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/product/wind.py
--rw-r--r--   0     1001      127      346 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/__main__.py
--rw-r--r--   0     1001      127       38 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/defaults.py
--rw-r--r--   0     1001      127      138 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/exceptions.py
--rw-r--r--   0     1001      127     3416 2024-04-23 13:09:28.000000 doppy-0.1.4/src/doppy/netcdf.py
--rw-r--r--   0     1001      127      279 2024-04-23 13:09:28.000000 doppy-0.1.4/README.md
--rw-r--r--   0     1001      127     1089 2024-04-23 13:09:28.000000 doppy-0.1.4/LICENSE
--rw-r--r--   0        0        0     1794 1970-01-01 00:00:00.000000 doppy-0.1.4/PKG-INFO
+-rw-r--r--   0     1001      127      206 2024-05-06 14:29:18.000000 doppy-0.2.0/crates/doprs/Cargo.toml
+-rw-r--r--   0     1001      127       21 2024-05-06 14:29:18.000000 doppy-0.2.0/crates/doprs/.gitignore
+-rw-r--r--   0     1001      127       13 2024-05-06 14:29:18.000000 doppy-0.2.0/crates/doprs/src/lib.rs
+-rw-r--r--   0     1001      127     2047 2024-05-06 14:29:18.000000 doppy-0.2.0/crates/doprs/src/raw/error.rs
+-rw-r--r--   0     1001      127     9448 2024-05-06 14:29:18.000000 doppy-0.2.0/crates/doprs/src/raw/halo_hpl.rs
+-rw-r--r--   0     1001      127     6876 2024-05-06 14:29:18.000000 doppy-0.2.0/crates/doprs/src/raw/wls70.rs
+-rw-r--r--   0     1001      127       48 2024-05-06 14:29:18.000000 doppy-0.2.0/crates/doprs/src/raw.rs
+-rw-r--r--   0        0        0      420 1970-01-01 00:00:00.000000 doppy-0.2.0/crates/doppy_rs/Cargo.toml
+-rw-r--r--   0     1001      127      279 2024-05-06 14:29:18.000000 doppy-0.2.0/crates/doppy_rs/src/lib.rs
+-rw-r--r--   0     1001      127     4526 2024-05-06 14:29:18.000000 doppy-0.2.0/crates/doppy_rs/src/raw/halo_hpl.rs
+-rw-r--r--   0     1001      127     2282 2024-05-06 14:29:18.000000 doppy-0.2.0/crates/doppy_rs/src/raw/wls70.rs
+-rw-r--r--   0     1001      127      269 2024-05-06 14:29:18.000000 doppy-0.2.0/crates/doppy_rs/src/raw.rs
+-rw-r--r--   0     1001      127    18041 2024-05-06 14:29:22.000000 doppy-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0      182 1970-01-01 00:00:00.000000 doppy-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      127     2393 2024-05-06 14:29:18.000000 doppy-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      127      205 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/options.py
+-rw-r--r--   0     1001      127        0 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/py.typed
+-rw-r--r--   0     1001      127     4809 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/raw/halo_bg.py
+-rw-r--r--   0     1001      127    18625 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/raw/halo_hpl.py
+-rw-r--r--   0     1001      127     9685 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/raw/windcube.py
+-rw-r--r--   0     1001      127     6792 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/raw/wls70.py
+-rw-r--r--   0     1001      127     3937 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/raw/halo_sys_params.py
+-rw-r--r--   0     1001      127      228 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/raw/__init__.py
+-rw-r--r--   0     1001      127     1863 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/data/api.py
+-rw-r--r--   0     1001      127      996 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/data/cache.py
+-rw-r--r--   0     1001      127        0 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/data/__init__.py
+-rw-r--r--   0     1001      127       89 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/data/exceptions.py
+-rw-r--r--   0     1001      127      191 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/__init__.py
+-rw-r--r--   0     1001      127      248 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/bench.py
+-rw-r--r--   0     1001      127    19844 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/product/stare.py
+-rw-r--r--   0     1001      127      103 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/product/__init__.py
+-rw-r--r--   0     1001      127    12014 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/product/wind.py
+-rw-r--r--   0     1001      127      346 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/__main__.py
+-rw-r--r--   0     1001      127       38 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/defaults.py
+-rw-r--r--   0     1001      127      138 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/exceptions.py
+-rw-r--r--   0     1001      127     3416 2024-05-06 14:29:18.000000 doppy-0.2.0/src/doppy/netcdf.py
+-rw-r--r--   0     1001      127      279 2024-05-06 14:29:18.000000 doppy-0.2.0/README.md
+-rw-r--r--   0     1001      127     1089 2024-05-06 14:29:18.000000 doppy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1789 1970-01-01 00:00:00.000000 doppy-0.2.0/PKG-INFO
```

### Comparing `doppy-0.1.4/crates/doprs/src/raw/error.rs` & `doppy-0.2.0/crates/doprs/src/raw/error.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use std::fmt;
 
 #[derive(Debug, Clone)]
 pub struct RawParseError {
-    message: String,
+    pub message: String,
 }
 
 impl Default for RawParseError {
     fn default() -> Self {
         Self::new()
     }
 }
```

### Comparing `doppy-0.1.4/crates/doprs/src/raw/halo_hpl.rs` & `doppy-0.2.0/crates/doprs/src/raw/halo_hpl.rs`

 * *Files identical despite different names*

### Comparing `doppy-0.1.4/crates/doppy_rs/src/raw/halo_hpl.rs` & `doppy-0.2.0/crates/doppy_rs/src/raw/halo_hpl.rs`

 * *Files identical despite different names*

### Comparing `doppy-0.1.4/Cargo.lock` & `doppy-0.2.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -102,24 +102,24 @@
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "doppy_rs"
-version = "0.1.4"
+version = "0.2.0"
 dependencies = [
  "doprs",
  "numpy",
  "pyo3",
 ]
 
 [[package]]
 name = "doprs"
-version = "0.1.4"
+version = "0.2.0"
 dependencies = [
  "chrono",
  "rayon",
  "regex",
 ]
 
 [[package]]
```

### Comparing `doppy-0.1.4/pyproject.toml` & `doppy-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Operating System :: OS Independent"
 ]
 dependencies = [
   "requests",
   "urllib3",
   "numpy",
   "netCDF4",
-  "typer[all]",
+  "typer",
   "matplotlib",
   "scikit-learn",
   "scipy"
 ]
 
 [project.optional-dependencies]
 dev = ["mypy", "ruff", "pytest", "types-requests", "py-spy", "maturin==1.4", "release-version", "pre-commit"]
```

### Comparing `doppy-0.1.4/src/doppy/raw/halo_bg.py` & `doppy-0.2.0/src/doppy/raw/halo_bg.py`

 * *Files identical despite different names*

### Comparing `doppy-0.1.4/src/doppy/raw/halo_hpl.py` & `doppy-0.2.0/src/doppy/raw/halo_hpl.py`

 * *Files identical despite different names*

### Comparing `doppy-0.1.4/src/doppy/raw/windcube.py` & `doppy-0.2.0/src/doppy/raw/windcube.py`

 * *Files identical despite different names*

### Comparing `doppy-0.1.4/src/doppy/raw/halo_sys_params.py` & `doppy-0.2.0/src/doppy/raw/halo_sys_params.py`

 * *Files identical despite different names*

### Comparing `doppy-0.1.4/src/doppy/data/api.py` & `doppy-0.2.0/src/doppy/data/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,15 +33,21 @@
             )
         raise exceptions.ApiRequestError(f"Api request error: {res.status_code}")
 
     def get_raw_records(self, site: str, date: str) -> list:
         return self.get(
             "raw-files",
             params={
-                "instrument": ["halo-doppler-lidar", "wls100s", "wls200s", "wls400s"],
+                "instrument": [
+                    "halo-doppler-lidar",
+                    "wls100s",
+                    "wls200s",
+                    "wls400s",
+                    "wls70",
+                ],
                 "site": site,
                 "date": date,
             },
         )
 
     def get_record_content(self, rec: dict) -> io.BytesIO:
         if self.cache:
```

### Comparing `doppy-0.1.4/src/doppy/data/cache.py` & `doppy-0.2.0/src/doppy/data/cache.py`

 * *Files identical despite different names*

### Comparing `doppy-0.1.4/src/doppy/product/stare.py` & `doppy-0.2.0/src/doppy/product/stare.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,16 @@
 
         bg = (
             doppy.raw.HaloBg.merge(bgs_stare)
             .sorted_by_time()
             .non_strictly_increasing_timesteps_removed()
         )
         raw, intensity_bg_corrected = _correct_background(raw, bg, bg_correction_method)
+        if len(raw.time) == 0:
+            raise doppy.exceptions.NoDataError("No matching data and bg files")
         intensity_noise_bias_corrected = _correct_intensity_noise_bias(
             raw, intensity_bg_corrected
         )
         wavelength = defaults.Halo.wavelength
         beta = _compute_beta(
             intensity_noise_bias_corrected,
             raw.radial_distance,
```

### Comparing `doppy-0.1.4/src/doppy/product/wind.py` & `doppy-0.2.0/src/doppy/product/wind.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,14 +145,46 @@
             height=height,
             zonal_wind=wind[:, :, 0],
             meridional_wind=wind[:, :, 1],
             vertical_wind=wind[:, :, 2],
             mask=mask,
         )
 
+    @classmethod
+    def from_wls70_data(
+        cls,
+        data: Sequence[str]
+        | Sequence[Path]
+        | Sequence[bytes]
+        | Sequence[BufferedIOBase],
+    ) -> Wind:
+        raws = doppy.raw.Wls70.from_srcs(data)
+
+        if len(raws) == 0:
+            raise doppy.exceptions.NoDataError("Wls70 data missing")
+
+        raw = (
+            doppy.raw.Wls70.merge(raws)
+            .sorted_by_time()
+            .non_strictly_increasing_timesteps_removed()
+        )
+        mask = (
+            np.isnan(raw.meridional_wind)
+            | np.isnan(raw.zonal_wind)
+            | np.isnan(raw.vertical_wind)
+        )
+        return Wind(
+            time=raw.time,
+            height=raw.altitude,
+            zonal_wind=raw.zonal_wind,
+            meridional_wind=raw.meridional_wind,
+            vertical_wind=raw.vertical_wind,
+            mask=mask,
+        )
+
 
 def _compute_wind(
     raw: doppy.raw.HaloHpl | doppy.raw.WindCube,
 ) -> tuple[float, float, npt.NDArray[np.float64], npt.NDArray[np.float64]]:
     """
     Returns
     -------
```

### Comparing `doppy-0.1.4/src/doppy/netcdf.py` & `doppy-0.2.0/src/doppy/netcdf.py`

 * *Files identical despite different names*

### Comparing `doppy-0.1.4/LICENSE` & `doppy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `doppy-0.1.4/PKG-INFO` & `doppy-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.3
 Name: doppy
-Version: 0.1.4
+Version: 0.2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Requires-Dist: requests
 Requires-Dist: urllib3
 Requires-Dist: numpy
 Requires-Dist: netcdf4
-Requires-Dist: typer[all]
+Requires-Dist: typer
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: mypy ; extra == 'dev'
 Requires-Dist: ruff ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: types-requests ; extra == 'dev'
```

